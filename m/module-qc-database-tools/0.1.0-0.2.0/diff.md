# Comparing `tmp/module_qc_database_tools-0.1.0.tar.gz` & `tmp/module_qc_database_tools-0.2.0.tar.gz`

## Comparing `module_qc_database_tools-0.1.0.tar` & `module_qc_database_tools-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.env.template
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tbump.toml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    12566 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/README.md
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.env.template
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    15393 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/README.md
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/PKG-INFO
```

### Comparing `module_qc_database_tools-0.1.0/.gitlab-ci.yml` & `module_qc_database_tools-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/.pre-commit-config.yaml` & `module_qc_database_tools-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/tbump.toml` & `module_qc_database_tools-0.2.0/tbump.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e31 2e30 220a 0a23 2045  t = "0.1.0"..# E
+00000010: 7420 3d20 2230 2e32 2e30 220a 0a23 2045  t = "0.2.0"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -14,15 +14,15 @@
 000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 312e  mp version: 0.1.
+00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 322e  mp version: 0.2.
 00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section
```

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/chip_config_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import hashlib
 import io
 import logging
 import pickle
 
 import gridfs
 from bson.objectid import ObjectId
@@ -28,15 +29,15 @@
         """
         config_data = {"serialNumber": serial_number, "stage": stage, "branch": branch}
         record = self.database.fe_configs.find_one(config_data)
         if self.database.fe_configs.find_one(config_data) is None:
             result = self.database.fe_configs.insert_one(config_data)
             return str(result.inserted_id)
 
-        log.info("info: config for % already exists.", config_data)
+        log.info("info: config for %s already exists.", config_data)
         return str(record.get("_id"))
 
     def get_info(self, config_id):
         """
         Get information about the config id.
         """
         return self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
@@ -137,16 +138,16 @@
             return None
 
         revision_doc = self.database.fe_config_revision.find_one(
             {"_id": ObjectId(revision)}
         )
         config_data = revision_doc.get("config_data")
 
-        if add_pixel_cfg is True:
-            pixcfg_id = revision_doc.get("pix_config")
+        if add_pixel_cfg is True and revision_doc.get("pix_config") is not None:
+            pixcfg_id = revision_doc.get("pix_config").get("_id")
 
             filesystem = gridfs.GridFS(self.client.localdb)
 
             data = filesystem.get(pixcfg_id).read()
 
             pixcfg = pickle.load(io.BytesIO(data))
 
@@ -158,62 +159,85 @@
         """
         Commit the config for a given commit_id with some message.
         """
         pixelcfg = fe_cfg.get("RD53B").get("PixelConfig")
 
         keys_to_remove = []
 
+        is_pixelcfg_revised = None
+
         if pixelcfg is not None:
+            log.info("pickling pixelcfg...")
             binary = pickle.dumps(pixelcfg)
 
             keys_to_remove = [
                 var
                 for var, contents in fe_cfg.get("RD53B").items()
                 if var not in ["GlobalConfig", "Parameter"]
             ]
 
             filesystem = gridfs.GridFS(self.client.localdb)
 
             md5 = hashlib.md5(binary).hexdigest()
 
             log.info("pixelcfg md5 hash = %s", md5)
 
-            if self.client.localdb.filesystem.files.find_one({"md5": md5}) is not None:
+            if self.client.localdb.fs.files.find_one({"md5": md5}) is not None:
                 log.info(
                     "info: identified the same pixel config data in gridfs, reusing it."
                 )
-                pixelcfg_id = filesystem.put(binary)
+                pixelcfg_id = self.client.localdb.fs.files.find_one({"md5": md5})
+                is_pixelcfg_revised = False
             else:
-                pixelcfg_id = self.database.fs.files.find_one({"md5": md5})
+                pixelcfg_id = filesystem.put(binary)
+                is_pixelcfg_revised = True
 
         else:
+            log.info("pixelcfg is None, skipping pickling")
             pixelcfg_id = None
+            is_pixelcfg_revised = True
 
         _ = [fe_cfg.get("RD53B").pop(key) for key in keys_to_remove]
 
         config = self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
         previous_revision_id = config.get("current_revision_id")
 
         # Compute the diff between the previous and new configuration
         if previous_revision_id is None:
             the_diff = fe_cfg
         else:
             previous_revision = self.database.fe_config_revision.find_one(
                 {"_id": previous_revision_id}
             )
+            if not previous_revision:
+                log.error(
+                    "Corrupted!! Previous revision ID %s is present for config %s but the object is not recorded in database",
+                    previous_revision_id,
+                    config_id,
+                )
+                return None
+
             previous_data = previous_revision.get("config_data", {})
             the_diff = diff(previous_data, fe_cfg, dump=True)
 
+        timestamp = datetime.datetime.utcnow()
+
+        # If no change in config, do not commit and return the previous revision_id
+        if the_diff == "{}" and is_pixelcfg_revised is False:
+            log.info("Nothing to commit (identical config as previous)")
+            return previous_revision_id
+
         # Save the revision and update the config to point to it
         revision_doc = {
             "parent_revision_id": previous_revision_id,
             "config_data": fe_cfg,
             "diff": the_diff,
             "pix_config": pixelcfg_id,
             "message": message,
+            "timestamp": timestamp,
             "tags": [],
         }
 
         result = self.database.fe_config_revision.insert_one(revision_doc)
         revision_id = result.inserted_id
         self.database.fe_configs.update_one(
             {"_id": ObjectId(config_id)}, {"$set": {"current_revision_id": revision_id}}
```

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/core.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import copy
+import json
 import logging
 import math
 from pathlib import Path
 
 import pandas as pd
 
 from module_qc_database_tools.utils import chip_serial_number_to_uid
 
 log = logging.getLogger(__name__)
+log.setLevel(logging.INFO)
 
 
 class Module:
     """
     Module class.
     """
 
@@ -43,15 +45,15 @@
         if len(self.bare_modules) == 3 and len(self.chips) == 3:
             self.module_type = "triplet"
             log.info("triplet %s initiated.", self.serial_number)
         else:
             self.module_type = "quad"
             log.info("quad module %s initiated.", self.serial_number)
 
-    def generate_config(self, chip_template, layer_config, suffix):
+    def generate_config(self, chip_template, layer_config, suffix, version):
         """
         Generate module config.
         """
         log.info(
             "generating module config for module %s with %s",
             self.serial_number,
             layer_config,
@@ -70,14 +72,15 @@
                     copy.deepcopy(
                         chip_template
                     ),  # NB: make sure we copy as Chip::generate_config modifies this in-place
                     chip_index,
                     layer_config,
                     self.module_type,
                     suffix=suffix,
+                    version=version,
                 )
             )
 
             # relative path: e.g. L2_warm/0x15499_L2_warm.json
             chip_config_path = (
                 Path(f"{layer_config}{'_'+suffix if suffix else ''}")
                 / f"{chip.uid}_{layer_config}{'_'+suffix if suffix else ''}.json"
@@ -103,19 +106,30 @@
     """
 
     def __init__(self, client, serial_number, module_name=None):
         self.client = client
         self.serial_number = serial_number
         self.uid = chip_serial_number_to_uid(serial_number)
         self.module_name = module_name or self.serial_number
-        self.chip = client.get("getComponent", json={"component": serial_number})
+        self.chip = client.get(
+            "getComponent", json={"component": serial_number, "noEosToken": False}
+        )
+        self.attachments = [
+            item for item in self.chip["attachments"] if item["type"] == "eos"
+        ]
         self.test_run = None
 
         log.info("chip %s initiated.", self.uid)
 
+    def get_latest_configs(self, item):
+        """use title for filename: 'title': '0x12345_<layer_config>_<suffix>.json'"""
+        infile = self.client.get(item["url"])
+        with Path(infile.filename).open(mode="r", encoding="UTF-8") as fsnake:
+            return json.loads(fsnake.read())
+
     def load_wafer_probing_data(self):
         """
         Load chip wafer probing data.
         """
         test_id = None
         tests = pd.DataFrame(self.chip["tests"])
         if len(tests[tests["code"] == "FECHIP_TEST"]) > 0:
@@ -126,220 +140,262 @@
             msg = (
                 f"No wafer probing data in production DB for chip {self.serial_number}!"
             )
             raise RuntimeError(msg)
         self.test_run = TestRun(self.client, test_id)
 
     def generate_config(
-        self, chip_template, chip_index, layer_config, module_type, suffix=""
+        self,
+        chip_template,
+        chip_index,
+        layer_config,
+        module_type,
+        suffix="",
+        version="latest",
     ):
         """
         Generate chip config.
         """
-        log.info("generating chip config for chip %s with %s", self.uid, layer_config)
-
-        power_config = "LP" if suffix == "LP" else layer_config
+        if version == "latest" and len(self.attachments) >= 3:
+            checklist = [".json", layer_config, suffix]
+            for item in self.attachments:
+                if all(check in item["title"] for check in checklist):
+                    log.info(
+                        " Latest chip configs found for %s %s!", layer_config, suffix
+                    )
+                    try:
+                        return self.get_latest_configs(item)
+                    except RuntimeError as esnake:
+                        log.warning(
+                            " Unable to find latest config: %s. Make sure all sets of configs are present in the database.",
+                            esnake,
+                        )
+                        continue
 
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreComp"] = {
-            "R0": 350,
-            "R0.5": 350,
-            "L0": 350,
-            "L1": 350,
-            "L2": 350,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampL"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampM"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampR"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampT"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampTL"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffPreampTR"] = {
-            "R0": 900,
-            "R0.5": 900,
-            "L0": 900,
-            "L1": 730,
-            "L2": 550,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["DiffVff"] = {
-            "R0": 150,
-            "R0.5": 150,
-            "L0": 150,
-            "L1": 150,
-            "L2": 60,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["EnCoreCol0"] = {
-            "R0": 65535,
-            "R0.5": 65535,
-            "L0": 65535,
-            "L1": 65535,
-            "L2": 65535,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["EnCoreCol1"] = {
-            "R0": 65535,
-            "R0.5": 65535,
-            "L0": 65535,
-            "L1": 65535,
-            "L2": 65535,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["EnCoreCol2"] = {
-            "R0": 65535,
-            "R0.5": 65535,
-            "L0": 65535,
-            "L1": 65535,
-            "L2": 65535,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["GlobalConfig"]["EnCoreCol3"] = {
-            "R0": 63,
-            "R0.5": 63,
-            "L0": 63,
-            "L1": 63,
-            "L2": 63,
-            "LP": 0,
-        }[power_config]
-        chip_template["RD53B"]["Parameter"]["Name"] = self.uid
-
-        if module_type == "triplet":
-            chip_template["RD53B"]["Parameter"]["ChipId"] = chip_index + 1
-            chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = {
-                "R0": 7,
-                "R0.5": 3,
-                "L0": 15,
-            }[
-                layer_config
-            ]  ## TODO: add source for R0 and R0.5
-            # chip_template["RD53B"]["GlobalConfig"]["MonitorEnable"] = 0
-            # chip_template["RD53B"]["GlobalConfig"]["MonitorV"] = 63
-            for index in range(4):
-                chip_template["RD53B"]["GlobalConfig"][f"DataMergeOutMux{index}"] = (
-                    0 + index
-                ) % 4
-            chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = {
-                "R0": 7,
-                "R0.5": 3,
-                "L0": 15,
-            }[layer_config]
-        else:
-            chip_template["RD53B"]["Parameter"]["ChipId"] = 12 + chip_index
-            chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = 1
-            for index in range(4):
-                chip_template["RD53B"]["GlobalConfig"][f"DataMergeOutMux{index}"] = (
-                    [2, 0, 1, 0][chip_index] + index
-                ) % 4
-            chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = [4, 1, 8, 1][
-                chip_index
-            ]
+                else:
+                    log.warning(
+                        " No layer_config %s or suffix %s found in %s",
+                        layer_config,
+                        suffix,
+                        item["title"],
+                    )
+                    continue
+        elif version == "TESTONWAFER" or len(self.attachments) == 0:
+            log.info(
+                "Generating chip config for chip %s with %s from wafer probing.",
+                self.uid,
+                layer_config,
+            )
+            power_config = "LP" if suffix == "LP" else layer_config
+
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreComp"] = {
+                "R0": 350,
+                "R0.5": 350,
+                "L0": 350,
+                "L1": 350,
+                "L2": 350,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampL"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampM"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampR"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampT"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampTL"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffPreampTR"] = {
+                "R0": 900,
+                "R0.5": 900,
+                "L0": 900,
+                "L1": 730,
+                "L2": 550,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["DiffVff"] = {
+                "R0": 150,
+                "R0.5": 150,
+                "L0": 150,
+                "L1": 150,
+                "L2": 60,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol0"] = {
+                "R0": 65535,
+                "R0.5": 65535,
+                "L0": 65535,
+                "L1": 65535,
+                "L2": 65535,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol1"] = {
+                "R0": 65535,
+                "R0.5": 65535,
+                "L0": 65535,
+                "L1": 65535,
+                "L2": 65535,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol2"] = {
+                "R0": 65535,
+                "R0.5": 65535,
+                "L0": 65535,
+                "L1": 65535,
+                "L2": 65535,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol3"] = {
+                "R0": 63,
+                "R0.5": 63,
+                "L0": 63,
+                "L1": 63,
+                "L2": 63,
+                "LP": 0,
+            }[power_config]
+            chip_template["RD53B"]["Parameter"]["Name"] = self.uid
+
+            if module_type == "triplet":
+                chip_template["RD53B"]["Parameter"]["ChipId"] = chip_index + 1
+                chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = {
+                    "R0": 7,
+                    "R0.5": 3,
+                    "L0": 15,
+                }[
+                    layer_config
+                ]  ## TODO: add source for R0 and R0.5
+                # chip_template["RD53B"]["GlobalConfig"]["MonitorEnable"] = 0
+                # chip_template["RD53B"]["GlobalConfig"]["MonitorV"] = 63
+                for index in range(4):
+                    chip_template["RD53B"]["GlobalConfig"][
+                        f"DataMergeOutMux{index}"
+                    ] = (0 + index) % 4
+                chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = {
+                    "R0": 7,
+                    "R0.5": 3,
+                    "L0": 15,
+                }[layer_config]
+            else:
+                chip_template["RD53B"]["Parameter"]["ChipId"] = 12 + chip_index
+                chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = 1
+                for index in range(4):
+                    chip_template["RD53B"]["GlobalConfig"][
+                        f"DataMergeOutMux{index}"
+                    ] = ([2, 0, 1, 0][chip_index] + index) % 4
+                chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = [4, 1, 8, 1][
+                    chip_index
+                ]
+
+            if not self.test_run:
+                self.load_wafer_probing_data()
+            if self.test_run:
+                chip_template["RD53B"]["GlobalConfig"][
+                    "SldoTrimA"
+                ] = self.test_run.get_result("VDDA_TRIM")
+                chip_template["RD53B"]["GlobalConfig"][
+                    "SldoTrimD"
+                ] = self.test_run.get_result("VDDD_TRIM")
+                chip_template["RD53B"]["Parameter"]["ADCcalPar"][0] = (
+                    self.test_run.get_result("ADC_OFFSET") * 1000
+                )
+                chip_template["RD53B"]["Parameter"]["ADCcalPar"][1] = (
+                    self.test_run.get_result("ADC_SLOPE") * 1000
+                )
+                chip_template["RD53B"]["Parameter"][
+                    "InjCap"
+                ] = self.test_run.get_result("InjectionCapacitance") * (10**15)
+
+                # For transistor sensors calibration, the ideality factor is calculated following the presentation:
+                # https://indico.cern.ch/event/1011941/contributions/4278988/attachments/2210633/3741190/RD53B_calibatrion_sensor_temperature.pdf
+                e_charge = 1.602e-19
+                kB = 1.38064852e-23
+                PC_NTC = self.test_run.get_result("PC_NTC") + 273
+                DeltaT = 2  # 2 degree difference between PC NTC and transistor sensors
+                chip_template["RD53B"]["Parameter"]["NfDSLDO"] = (
+                    self.test_run.get_result("TEMPERATURE_D")
+                    * e_charge
+                    / (kB * math.log(15) * (PC_NTC + DeltaT))
+                )
+                chip_template["RD53B"]["Parameter"]["NfASLDO"] = (
+                    self.test_run.get_result("TEMPERATURE_A")
+                    * e_charge
+                    / (kB * math.log(15) * (PC_NTC + DeltaT))
+                )
+                chip_template["RD53B"]["Parameter"]["NfACB"] = (
+                    self.test_run.get_result("TEMPERATURE_C")
+                    * e_charge
+                    / (kB * math.log(15) * (PC_NTC + DeltaT))
+                )
 
-        if not self.test_run:
-            self.load_wafer_probing_data()
-        if self.test_run:
-            chip_template["RD53B"]["GlobalConfig"][
-                "SldoTrimA"
-            ] = self.test_run.get_result("VDDA_TRIM")
-            chip_template["RD53B"]["GlobalConfig"][
-                "SldoTrimD"
-            ] = self.test_run.get_result("VDDD_TRIM")
-            chip_template["RD53B"]["Parameter"]["ADCcalPar"][0] = (
-                self.test_run.get_result("ADC_OFFSET") * 1000
-            )
-            chip_template["RD53B"]["Parameter"]["ADCcalPar"][1] = (
-                self.test_run.get_result("ADC_SLOPE") * 1000
-            )
-            chip_template["RD53B"]["Parameter"]["InjCap"] = self.test_run.get_result(
-                "InjectionCapacitance"
-            ) * (10**15)
-
-            # For transistor sensors calibration, the ideality factor is calculated following the presentation:
-            # https://indico.cern.ch/event/1011941/contributions/4278988/attachments/2210633/3741190/RD53B_calibatrion_sensor_temperature.pdf
-            e_charge = 1.602e-19
-            kB = 1.38064852e-23
-            PC_NTC = self.test_run.get_result("PC_NTC") + 273
-            DeltaT = 2  # 2 degree difference between PC NTC and transistor sensors
-            chip_template["RD53B"]["Parameter"]["NfDSLDO"] = (
-                self.test_run.get_result("TEMPERATURE_D")
-                * e_charge
-                / (kB * math.log(15) * (PC_NTC + DeltaT))
-            )
-            chip_template["RD53B"]["Parameter"]["NfASLDO"] = (
-                self.test_run.get_result("TEMPERATURE_A")
-                * e_charge
-                / (kB * math.log(15) * (PC_NTC + DeltaT))
-            )
-            chip_template["RD53B"]["Parameter"]["NfACB"] = (
-                self.test_run.get_result("TEMPERATURE_C")
-                * e_charge
-                / (kB * math.log(15) * (PC_NTC + DeltaT))
-            )
+                chip_template["RD53B"]["Parameter"]["VcalPar"] = [
+                    abs(
+                        self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_OFFSET") * 1000
+                    ),
+                    self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_SLOPE") * 1000,
+                ]
+                chip_template["RD53B"]["Parameter"][
+                    "IrefTrim"
+                ] = self.test_run.get_result("IREF_TRIM")
+                chip_template["RD53B"]["Parameter"][
+                    "KSenseInA"
+                ] = self.test_run.get_result("CURR_MULT_FAC_A")
+                chip_template["RD53B"]["Parameter"][
+                    "KSenseInD"
+                ] = self.test_run.get_result("CURR_MULT_FAC_D")
+                chip_template["RD53B"]["Parameter"]["KSenseShuntA"] = (
+                    self.test_run.get_result("CURR_MULT_FAC_A") * 26000.0 / 21000.0
+                )
+                chip_template["RD53B"]["Parameter"]["KSenseShuntD"] = (
+                    self.test_run.get_result("CURR_MULT_FAC_D") * 26000.0 / 21000.0
+                )
+                chip_template["RD53B"]["Parameter"][
+                    "KShuntA"
+                ] = self.test_run.get_result("VINA_SHUNT_KFACTOR")
+                chip_template["RD53B"]["Parameter"][
+                    "KShuntD"
+                ] = self.test_run.get_result("VIND_SHUNT_KFACTOR")
 
-            chip_template["RD53B"]["Parameter"]["VcalPar"] = [
-                abs(self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_OFFSET") * 1000),
-                self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_SLOPE") * 1000,
-            ]
-            chip_template["RD53B"]["Parameter"]["IrefTrim"] = self.test_run.get_result(
-                "IREF_TRIM"
-            )
-            chip_template["RD53B"]["Parameter"]["KSenseInA"] = self.test_run.get_result(
-                "CURR_MULT_FAC_A"
-            )
-            chip_template["RD53B"]["Parameter"]["KSenseInD"] = self.test_run.get_result(
-                "CURR_MULT_FAC_D"
-            )
-            chip_template["RD53B"]["Parameter"]["KSenseShuntA"] = (
-                self.test_run.get_result("CURR_MULT_FAC_A") * 26000.0 / 21000.0
-            )
-            chip_template["RD53B"]["Parameter"]["KSenseShuntD"] = (
-                self.test_run.get_result("CURR_MULT_FAC_D") * 26000.0 / 21000.0
-            )
-            chip_template["RD53B"]["Parameter"]["KShuntA"] = self.test_run.get_result(
-                "VINA_SHUNT_KFACTOR"
-            )
-            chip_template["RD53B"]["Parameter"]["KShuntD"] = self.test_run.get_result(
-                "VIND_SHUNT_KFACTOR"
+            return chip_template
+        else:
+            msg = (
+                "Not able to generate chip config. Chip configs might not be complete."
             )
-
-        return chip_template
+            raise RuntimeError(msg)
+        return None
 
 
 class TestRun:
     """
     TestRun class.
     """
```

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/utils.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from pathlib import Path
 from typing import List, Optional
 
 import itkdb
+import jsbeautifier
 import typer
 from pymongo import MongoClient
 
 import module_qc_database_tools
 from module_qc_database_tools.chip_config_api import ChipConfigAPI
 from module_qc_database_tools.core import Module
 from module_qc_database_tools.utils import (
@@ -40,14 +41,20 @@
     ),
     modes: List[str] = typer.Option(
         ["warm", "cold", "LP"],
         "-m",
         "--mode",
         help="Modes to generate configs for.",
     ),
+    version: str = typer.Option(
+        "latest",  ## "TESTONWAFER", "MODULE/INITIAL_WARM", "etc"], ## use stage/test names?
+        "-v",
+        "--version",
+        help="Generate chip configs, default is 'latest'. Possible choices: 'TESTONWAFER'...",
+    ),
     mongo_uri: str = typer.Option(
         "mongodb://localhost:27017",
         "-u",
         "--uri",
         help="mongo URI (see documentation for mongo client)",
     ),
     itkdb_access_code1: Optional[str] = typer.Option(
@@ -76,15 +83,15 @@
 
     for suffix in modes:
         connectivity_path = Path(output_dir or "", module.name).joinpath(
             f"{module.name}_{layer_config}{'_'+suffix if suffix else ''}.json"
         )
 
         generated_configs = module.generate_config(
-            chip_template, layer_config, suffix=suffix
+            chip_template, layer_config, suffix=suffix, version=version
         )
 
         if output_dir:
             save_configs_local(generated_configs, connectivity_path)
         else:
             mongo_client = MongoClient(mongo_uri)
             chip_config_client = ChipConfigAPI(mongo_client)
@@ -99,16 +106,21 @@
 
     connectivity_path.write_text(json.dumps(configs["module"], indent=4))
     typer.echo(f"module connectivity file saved to {connectivity_path}")
 
     for chip_config, chip_spec in zip(configs["module"]["chips"], configs["chips"]):
         output_path = connectivity_path.parent.joinpath(chip_config["config"])
         output_path.parent.mkdir(parents=True, exist_ok=True)
-
-        output_path.write_text(json.dumps(chip_spec, indent=4))
+        ## needed to avoid having chip config file at 14MB (but slow)
+        beautified = jsbeautifier.beautify(
+            json.dumps(chip_spec), jsbeautifier.default_options()
+        )
+        output_path.write_text(beautified)  ## file size 1.9MB
+        # output_path.write_text(json.dumps(chip_spec, indent=4)) ## file size 14MB due to linebreaks
+        # output_path.write_text(json.dumps(chip_spec)) ## file size is 1.8M, no linebreak
         typer.echo(f"chip config file saved to {output_path}")
 
 
 def save_configs_mongo(configs, chip_config_client, mode):
     """
     Save the configs generated to mongo.
     """
```

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/tests/test_cli.py` & `module_qc_database_tools-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/tests/test_config_api.py` & `module_qc_database_tools-0.2.0/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/.gitignore` & `module_qc_database_tools-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.1.0/README.md` & `module_qc_database_tools-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v0.1.0
+# Module QC Database Tools v0.2.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
@@ -70,15 +70,15 @@
 ```
 $ generateYARRConfig -sn [ATLAS SN] -o [outdir]
 $ mqdbt generate-yarr-config -sn [ATLAS SN] -o [outdir]
 
 Parameters:
 -sn, --sn, required=True: ATLAS serial number of the module
 -ch, --chipTemplate, default="configs/YARR/chip_template.json": provide the path of a chip config template to generate the new chip configs from
--o, --outdir, required=True: Path to output directory config folder will be placed in
+-o, --outdir, path to output directory config folder will be placed in. If not supplied, the config files will be pushed into mongoDB if connection is set up.
 ```
 
 For example, to generate the YARR configs for the module `20UPGR91301046` with
 all power configs:
 
 ```
 $ generateYARRConfig -sn 20UPGR91301046 -o ~/module_data/.
```

### Comparing `module_qc_database_tools-0.1.0/pyproject.toml` & `module_qc_database_tools-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 dependencies = [
     "itkdb>=0.4.0",  # for interface with production database
     "pandas",
     "typer",
     "pymongo",
     "jsondiff",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
+    "jsbeautifier", # for chip config linebreaks vs size
 ]
 
 [project.urls]
 Homepage = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues"
 Source = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
```

### Comparing `module_qc_database_tools-0.1.0/PKG-INFO` & `module_qc_database_tools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-database-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 Classifier: Development Status :: 1 - Planning
@@ -21,21 +21,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: itkdb>=0.4.0
+Requires-Dist: jsbeautifier
 Requires-Dist: jsondiff
 Requires-Dist: pandas
 Requires-Dist: pymongo
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v0.1.0
+# Module QC Database Tools v0.2.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
@@ -103,15 +104,15 @@
 ```
 $ generateYARRConfig -sn [ATLAS SN] -o [outdir]
 $ mqdbt generate-yarr-config -sn [ATLAS SN] -o [outdir]
 
 Parameters:
 -sn, --sn, required=True: ATLAS serial number of the module
 -ch, --chipTemplate, default="configs/YARR/chip_template.json": provide the path of a chip config template to generate the new chip configs from
--o, --outdir, required=True: Path to output directory config folder will be placed in
+-o, --outdir, path to output directory config folder will be placed in. If not supplied, the config files will be pushed into mongoDB if connection is set up.
 ```
 
 For example, to generate the YARR configs for the module `20UPGR91301046` with
 all power configs:
 
 ```
 $ generateYARRConfig -sn 20UPGR91301046 -o ~/module_data/.
```


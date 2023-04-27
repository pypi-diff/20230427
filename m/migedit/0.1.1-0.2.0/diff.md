# Comparing `tmp/migedit-0.1.1.tar.gz` & `tmp/migedit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migedit-0.1.1.tar", last modified: Mon Nov 21 16:16:18 2022, max compression
+gzip compressed data, was "migedit-0.2.0.tar", last modified: Thu Apr 27 13:35:02 2023, max compression
```

## Comparing `migedit-0.1.1.tar` & `migedit-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1799 2022-11-21 10:32:55.921117 migedit-0.1.1/.gitignore
--rw-r--r--   0        0        0     1079 2022-11-21 15:55:21.696838 migedit-0.1.1/LICENSE
--rw-r--r--   0        0        0       76 2022-11-21 10:32:55.921117 migedit-0.1.1/README.md
--rw-r--r--   0        0        0     4263 2022-11-21 16:15:36.836670 migedit-0.1.1/migedit.py
--rw-r--r--   0        0        0      429 2022-11-21 15:59:04.849942 migedit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 migedit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2022-11-21 15:55:21.696838 migedit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      396 2023-04-27 13:29:00.000478 migedit-0.2.0/README.md
+-rw-r--r--   0        0        0     5717 2023-04-27 13:26:45.655787 migedit-0.2.0/migedit.py
+-rw-r--r--   0        0        0      429 2023-04-27 13:26:38.491750 migedit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 migedit-0.2.0/PKG-INFO
```

### Comparing `migedit-0.1.1/LICENSE` & `migedit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `migedit-0.1.1/migedit.py` & `migedit-0.2.0/migedit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """MIG Editor. CLI/importable module to automatically delete and create MIG gpu/cpu instances."""
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 import argparse
 import os
 import time
 
 from subprocess import Popen, PIPE
 
@@ -12,14 +12,20 @@
 MIG_OPTIONS = {
     "1": "1g.5gb",
     "2": "2g.10gb",
     "3": "3g.20gb",
     "4": "4g.20gb",
     "7": "7g.40gb",
 }
+SMIG_OPTIONS = {
+    "s1": "1c.7g.40gb",
+    "s2": "2c.7g.40gb",
+    "s3": "3c.7g.40gb",
+    "s4": "4c.7g.40gb",
+}
 
 
 def execute_command(cmd, shell=False, vars={}):
     """
     Executes a (non-run) command.
     :param cmd -> Command to run.
 
@@ -83,34 +89,67 @@
     if "failed" in result or "unable" in result:
         raise ValueError(result)
 
     time.sleep(1)
 
     devicetemp = []
 
-    # Create new instances
+    # TODO: remove this temp code
+    shared_mig_gpui = {}
+
+    # This supports Multi-MIG, which doesn't actually work right now
+    # Tested on PyTorch (and failed), perhaps works for different frameworks
     for index, profile in enumerate(profiles):
-        instance = profile.lower()
+        instance = profile.lower().strip()
 
         if instance in MIG_OPTIONS:
             instance = MIG_OPTIONS[instance]
+        elif instance in SMIG_OPTIONS:
+            instance = SMIG_OPTIONS[instance]
 
+        # Normal MIG
         if instance in MIG_OPTIONS.values():
             other_mig_ids = get_mig_ids(gpu)
 
             result = "".join(
                 execute_command(f"sudo nvidia-smi mig -i {int(gpu)} -cgi {instance} -C")
             ).lower()
 
             gpu_instance = result.split("gpu instance id")[1].split("on gpu")[0].strip()
 
             if "failed" in result or "unable" in result:
                 raise ValueError(result)
 
-            mig_id = list(get_mig_ids(gpu) - other_mig_ids)[0]
+            mig_id = get_mig_ids(gpu) - other_mig_ids
+
+            devicetemp.append((index, gpu, instance, gpu_instance, mig_id))
+
+        elif instance in SMIG_OPTIONS.values():
+            # Shared MIG, TODO: make more flexible
+            if gpu not in shared_mig_gpui:
+                result = "".join(
+                    execute_command(f"sudo nvidia-smi mig -i {gpu} -cgi 7g.40gb")
+                ).lower()
+                instance_id = result.split("gpu instance id")[1].split("on")[0].strip()
+                shared_mig_gpui[gpu] = instance_id
+
+            other_mig_ids = get_mig_ids(gpu)
+
+            gpu_instance = shared_mig_gpui[gpu]
+
+            result = "".join(
+                execute_command(
+                    f"sudo nvidia-smi mig -gi {gpu_instance} -cci {list(SMIG_OPTIONS.values()).index(instance)}"
+                )
+            ).lower()
+
+            if "failed" in result or "unable" in result:
+                raise ValueError(result)
+
+            mig_id = get_mig_ids(gpu) - other_mig_ids
 
             devicetemp.append((index, gpu, instance, gpu_instance, mig_id))
 
         time.sleep(
             2.0
         )  # Wait for the rather slow DCGMI discovery to yield a GPU entity id
 
@@ -142,15 +181,15 @@
         help="ID instance number of the GPU to manage MIG on.",
     )
     parser.add_argument(
         "-p",
         "--profiles",
         metavar="PROFILES",
         nargs="+",
-        help="""Space seperated list of MIG profiles to use. Options: "1" or "1g.5gb", "2" or "2g.10gb", "3" or "3g.20gb", "4" or "4g.20gb", "7" or "7g.40gb".""",
+        help="""Space seperated list of MIG profiles to use. Options: "1" or "1g.5gb", "2" or "2g.10gb", "3" or "3g.20gb", "4" or "4g.20gb", "7" or "7g.40gb", "s1" or "1c.7g.40gb", "s2" or "2c.7g.40gb", "s3" or "3c.7g.40gb", "s4" or "4c.7g.40gb".""",
         required=True,
     )
 
     args = parser.parse_args()
 
     make_mig_devices(args.instance, args.profiles)
```


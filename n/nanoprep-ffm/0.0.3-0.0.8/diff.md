# Comparing `tmp/nanoprep-ffm-0.0.3.tar.gz` & `tmp/nanoprep-ffm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoprep-ffm-0.0.3.tar", last modified: Tue Sep 13 09:08:44 2022, max compression
+gzip compressed data, was "nanoprep-ffm-0.0.8.tar", last modified: Thu Apr 27 13:17:46 2023, max compression
```

## Comparing `nanoprep-ffm-0.0.3.tar` & `nanoprep-ffm-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.057300 nanoprep-ffm-0.0.3/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     1068 2022-09-04 07:10:08.000000 nanoprep-ffm-0.0.3/LICENSE
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/NanoPreP/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-12 08:58:39.000000 nanoprep-ffm-0.0.3/NanoPreP/__init__.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     5413 2022-09-13 08:56:00.000000 nanoprep-ffm-0.0.3/NanoPreP/__main__.py
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/NanoPreP/aligntools/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-12 08:58:55.000000 nanoprep-ffm-0.0.3/NanoPreP/aligntools/__init__.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     1278 2022-09-12 08:58:54.000000 nanoprep-ffm-0.0.3/NanoPreP/aligntools/edlibAligner.py
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/NanoPreP/paramtools/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-12 08:58:53.000000 nanoprep-ffm-0.0.3/NanoPreP/paramtools/__init__.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     3803 2022-09-12 08:58:53.000000 nanoprep-ffm-0.0.3/NanoPreP/paramtools/argParser.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     1592 2022-09-12 08:58:52.000000 nanoprep-ffm-0.0.3/NanoPreP/paramtools/paramsets.py
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/NanoPreP/preptools/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     4620 2022-09-13 08:50:03.000000 nanoprep-ffm-0.0.3/NanoPreP/preptools/Annotator.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     1287 2022-09-13 08:50:03.000000 nanoprep-ffm-0.0.3/NanoPreP/preptools/Processor.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-12 08:58:51.000000 nanoprep-ffm-0.0.3/NanoPreP/preptools/__init__.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     1332 2022-09-13 08:50:03.000000 nanoprep-ffm-0.0.3/NanoPreP/preptools/polyFinder.py
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/NanoPreP/seqtools/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)      545 2022-09-13 08:50:03.000000 nanoprep-ffm-0.0.3/NanoPreP/seqtools/FastqIO.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)     6094 2022-09-12 08:58:43.000000 nanoprep-ffm-0.0.3/NanoPreP/seqtools/SeqFastq.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-12 08:58:47.000000 nanoprep-ffm-0.0.3/NanoPreP/seqtools/__init__.py
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)    10585 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/PKG-INFO
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)    10255 2022-09-13 09:06:39.000000 nanoprep-ffm-0.0.3/README.md
-drwxrwxr-x   0 b05b01002  (1003) b05b01002  (1003)        0 2022-09-13 09:08:44.053300 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)    10585 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/PKG-INFO
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)      669 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/SOURCES.txt
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        1 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/dependency_links.txt
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)       48 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/entry_points.txt
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)       19 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/requires.txt
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)        9 2022-09-13 09:08:43.000000 nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/top_level.txt
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)       38 2022-09-13 09:08:44.057300 nanoprep-ffm-0.0.3/setup.cfg
--rw-rw-r--   0 b05b01002  (1003) b05b01002  (1003)      659 2022-09-13 09:08:38.000000 nanoprep-ffm-0.0.3/setup.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1068 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/LICENSE
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     5425 2023-04-25 04:19:21.000000 nanoprep-ffm-0.0.8/NanoPreP/__main__.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/aligntools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/aligntools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     2824 2023-04-08 08:29:17.000000 nanoprep-ffm-0.0.8/NanoPreP/aligntools/edlibAligner.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/optimize/
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-18 09:25:14.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/__init__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     6211 2023-04-20 12:53:07.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/__main__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     2066 2023-04-19 12:45:10.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/argParser.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/paramtools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     3802 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/argParser.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1592 2023-04-07 06:07:14.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/paramsets.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/preptools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     9302 2023-04-14 07:32:11.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/Annotator.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1287 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/Processor.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1332 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/polyFinder.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/seqtools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      545 2023-04-07 05:16:25.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/FastqIO.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     6094 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/SeqFastq.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/__init__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/PKG-INFO
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)    10255 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/README.md
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/PKG-INFO
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      760 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        1 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      104 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/entry_points.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       26 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/requires.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        9 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/top_level.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       38 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/setup.cfg
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      776 2023-04-27 13:17:22.000000 nanoprep-ffm-0.0.8/setup.py
```

### Comparing `nanoprep-ffm-0.0.3/LICENSE` & `nanoprep-ffm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/__main__.py` & `nanoprep-ffm-0.0.8/NanoPreP/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#!usr/bin/env Python
-from pathlib import Path
-import re
 from NanoPreP.preptools.Annotator import Annotator
 from NanoPreP.preptools.Processor import Processor
 from NanoPreP.seqtools.FastqIO import FastqIO
 from NanoPreP.seqtools.SeqFastq import SeqFastq
 from NanoPreP.paramtools.paramsets import Params, Defaults
 from NanoPreP.paramtools.argParser import parser
 from datetime import datetime
+from pathlib import Path
 import sys
 import json
+import gzip
 
 def main():
     # parse arguments
     args = parser.parse_args()
 
     # collect parameters
     params = Defaults.copy()
@@ -27,15 +26,14 @@
             opts = ", ".join([i.__repr__() for i in Params.keys()])
             raise Exception(msg + opts)
 
     # get parameter from config
     if args.config:
         config = json.load(open(args.config))
         params.update(config)
-        pass
 
     # get command line arguments from ArgumentParser
     for k, v in vars(args).items():
         if not v == Defaults[k]:
             params[k] = v    
         elif f"--{k}" in sys.argv:
             params[k] = v
@@ -75,46 +73,48 @@
             pid_body=params["pid_body"],
             w=params["poly_w"],
             k=params["poly_k"]
         )
         
 
     # open output files
+    def openg(p:Path, mode:str):
+        if p.suffix == ".gz":
+            return gzip.open(p, mode + "t")
+        else:
+            return open(p, mode)
+        
     handle_out = {}
     for name in ["output_fusion", "output_truncated", "output_full_length"]:
         cls = {
             "output_fusion": "fusion",
             "output_truncated": "truncated",
             "output_full_length": "full-length"
         }[name]
         # output passed
         if params[name] == "-":
             handle_out[(cls, "passed")] = sys.stdout
         elif params[name]:
-            # open new file (clear if already exist)
-            fout = Path(params[name])
-            open(fout, "w").close()
-            handle_out[(cls, "passed")] = open(fout, "a")
+            # open new file (truncate if already exist)
+            handle_out[(cls, "passed")] = openg(Path(params[name]), "w")
         else:
             handle_out[(cls, "passed")] = None
 
         # output filtered
         if params[name] and params["suffix_filtered"]:
-            # open new file (clear if already exist)
+            # open new file (truncate if already exist)
                 fout = Path(params[name])
                 fout = fout.stem + "_" + params["suffix_filtered"] + fout.suffix
-                open(fout, "w").close()
-                # record to `handle_out`
-                handle_out[(cls, "filtered")] = open(fout, "a")
+                handle_out[(cls, "filtered")] = openg(fout, "w")
         else:
             handle_out[(cls, "filtered")] = None
 
 
     # open `input_fq`
-    with open(params["input_fq"], "r") as handle_in:
+    with openg(Path(params["input_fq"]), "r") as handle_in:
         # stream processing
         for read in FastqIO.read(handle_in):
             # add read count
             report_dict["total reads"] += 1
 
             # skip too-short reads if `skip_short`
             if params["skip_short"] > len(read):
@@ -168,12 +168,12 @@
 
     # get the stopping time 
     report_dict["stop time"] = datetime.now().strftime("%Y/%m/%d-%H:%M:%S")
 
 
     # output report.json
     if params["report"]:
-        with open(params["report"], "w") as handle:
+        with openg(Path(params["report"]), "w") as handle:
             handle.write(json.dumps(report_dict, indent=4))
 
 if __name__ == "__main__":
     main()
```

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/aligntools/edlibAligner.py` & `nanoprep-ffm-0.0.8/NanoPreP/aligntools/edlibAligner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,106 @@
 """Caller of edlib.align()"""
-from typing import Tuple
+from typing import Tuple, List
 import edlib
 
 class edlibAligner:
     def singleAlign(
         query: str,
         target: str,
         mode: str,
         task: str,
-        pid: float
+        pid: float,
+        tie_breaking: str = "middle"
     ) -> dict:
         # call edlib for the alignment
+        k = -1 if pid == -1 else round((1 - pid) * len(query))
         res = edlib.align(
             query,
             target,
             mode,
             task,
-            round((1 - pid) * len(query))
+            k
         )
 
-        # add pid to result
+        # add 2 fields: `pid` and `location` to `res`
         if res["editDistance"] >= 0:
+            # pid
             res["pid"] = 1 - res["editDistance"] / len(query)
+            
+            # tie-breaking if edlib.align report more than one location
+            idx = {
+                "left": 0,
+                "middle": len(res["locations"]) // 2,
+                "right": -1
+            }
+            res["location"] = res.pop("locations")[idx[tie_breaking]] 
         else:
             res["pid"] = -1
-
+            res["location"] = (-1, -1)
+        
         return res
 
     def bestAlign(
         querys: dict,
         target: str,
         mode: str,
         task: str,
-        pid: float
+        pid: float,
+        tie_breaking: str = "middle"
     ) -> Tuple[str, dict]:
         res = name = None
         # iterate over querys to find the best-aligned query
         for qname, query in querys.items():
-            new = edlibAligner.singleAlign(query, target, mode, task, pid)
+            new = edlibAligner.singleAlign(
+                query,
+                target,
+                mode,
+                task,
+                pid,
+                tie_breaking
+            )
+            
             # the first alingment result
             if not res:
                 res = new
                 name = qname
                 continue
 
             # if the new alignment result is better
             if new["pid"] > res["pid"]:
                 res = new
                 name = qname
 
         return name, res
+
+
+    def ntopAligns(
+            query: str,
+            target: str,
+            mode: str,
+            task: str,
+            pid: float,
+            n: int,
+            tie_breaking: str = "middle"
+        ) -> List[dict]:
+        out = []
+        lastloc = None
+        for _ in range(n):
+            # mask target sequence
+            if lastloc:
+                target = target[:lastloc[0]] + \
+                    "N" * (lastloc[1] - lastloc[0]) + \
+                    target[lastloc[1]:]
+            
+            # align
+            res =  edlibAligner.singleAlign(
+                    query,
+                    target,
+                    mode,
+                    task,
+                    pid,
+                    tie_breaking
+                )
+            lastloc = res["location"] if res["pid"] != -1 else None
+            out.append(res)            
+                
+        return out
```

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/paramtools/argParser.py` & `nanoprep-ffm-0.0.8/NanoPreP/paramtools/argParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     type=str,
     help="input FASTQ"
 )
 
 # general options
 parser.add_argument(
     "--mode",
-    metavar="[strandard|annotate|report]",
+    metavar="[standard|annotate|report]",
     type=str,
     help="use parameter presets "
     "(can be overriden by `config` and command line arguments) "
 )
 parser.add_argument(
     "--config",
     metavar="PATH",
```

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/paramtools/paramsets.py` & `nanoprep-ffm-0.0.8/NanoPreP/paramtools/paramsets.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/preptools/Processor.py` & `nanoprep-ffm-0.0.8/NanoPreP/preptools/Processor.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/preptools/polyFinder.py` & `nanoprep-ffm-0.0.8/NanoPreP/preptools/polyFinder.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/seqtools/FastqIO.py` & `nanoprep-ffm-0.0.8/NanoPreP/seqtools/FastqIO.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/NanoPreP/seqtools/SeqFastq.py` & `nanoprep-ffm-0.0.8/NanoPreP/seqtools/SeqFastq.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/PKG-INFO` & `nanoprep-ffm-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoprep-ffm
-Version: 0.0.3
+Version: 0.0.8
 Summary: A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data
 Home-page: https://github.com/Woodformation1136/NanoPreP
 Author: Chia-Chen Chu
 Author-email: jerry955071@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nanoprep-ffm-0.0.3/README.md` & `nanoprep-ffm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/PKG-INFO` & `nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoprep-ffm
-Version: 0.0.3
+Version: 0.0.8
 Summary: A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data
 Home-page: https://github.com/Woodformation1136/NanoPreP
 Author: Chia-Chen Chu
 Author-email: jerry955071@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nanoprep-ffm-0.0.3/nanoprep_ffm.egg-info/SOURCES.txt` & `nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
 README.md
 setup.py
 NanoPreP/__init__.py
 NanoPreP/__main__.py
 NanoPreP/aligntools/__init__.py
 NanoPreP/aligntools/edlibAligner.py
+NanoPreP/optimize/__init__.py
+NanoPreP/optimize/__main__.py
+NanoPreP/optimize/argParser.py
 NanoPreP/paramtools/__init__.py
 NanoPreP/paramtools/argParser.py
 NanoPreP/paramtools/paramsets.py
 NanoPreP/preptools/Annotator.py
 NanoPreP/preptools/Processor.py
 NanoPreP/preptools/__init__.py
 NanoPreP/preptools/polyFinder.py
```

### Comparing `nanoprep-ffm-0.0.3/setup.py` & `nanoprep-ffm-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 
 # read README.md
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoprep-ffm",
-    version="0.0.3",
+    version="0.0.8",
     author="Chia-Chen Chu",
     author_email="jerry955071@gmail.com",
     description="A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Woodformation1136/NanoPreP",
     packages=find_packages(),
-    install_requires=["edlib>=1.3.8", "numpy"],
-    entry_points={"console_scripts": ["nanoprep = NanoPreP.main:main"]}
+    install_requires=["edlib>=1.3.8", "numpy", "plotly"],
+    entry_points={
+        "console_scripts": [
+            "nanoprep = NanoPreP.__main__:main",
+            "nanoprep-optimize = NanoPreP.optimize.__main__:main"
+        ]
+    }
 )
```


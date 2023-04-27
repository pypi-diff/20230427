# Comparing `tmp/varvamp-0.8.tar.gz` & `tmp/varvamp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.8.tar", last modified: Tue Apr 25 07:38:33 2023, max compression
+gzip compressed data, was "varvamp-0.8.1.tar", last modified: Thu Apr 27 09:12:29 2023, max compression
```

## Comparing `varvamp-0.8.tar` & `varvamp-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-25 07:38:33.757910 varvamp-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-25 07:38:17.000000 varvamp-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:38:33.757910 varvamp-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 07:38:17.000000 varvamp-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.753910 varvamp-0.8/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:29.197724 varvamp-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-27 09:12:29.197724 varvamp-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-27 09:12:11.000000 varvamp-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:12:29.197724 varvamp-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-27 09:12:11.000000 varvamp-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:29.189724 varvamp-0.8.1/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:29.197724 varvamp-0.8.1/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-27 09:12:11.000000 varvamp-0.8.1/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:29.193724 varvamp-0.8.1/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:12:29.000000 varvamp-0.8.1/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.8/PKG-INFO` & `varvamp-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8
+Version: 0.8.1
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.8/README.md` & `varvamp-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/setup.py` & `varvamp-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/command.py` & `varvamp-0.8.1/varvamp/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
     # estimate threshold or number of ambiguous bases if args were not supplied
     if args.threshold is None or args.n_ambig is None:
         args.threshold, args.n_ambig = param_estimation.get_parameters(preprocessed_alignment, args, log_file)
     if args.mode == "qpcr" and args.n_ambig >= 1 and args.pn_ambig is None:
         args.pn_ambig = args.n_ambig - 1
         with open(log_file, "a") as f:
-            print(f"Automatic parameter selection set -pn {args.pn_ambig}.", file=f)
+            print(f"Automatic parameter selection set -pa {args.pn_ambig}.", file=f)
 
     # check arguments
     logging.raise_arg_errors(args, log_file)
 
     # config check
     logging.confirm_config(args, log_file)
     logging.varvamp_progress(
```

### Comparing `varvamp-0.8/varvamp/scripts/alignment.py` & `varvamp-0.8.1/varvamp/scripts/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,17 +211,20 @@
 
     all_gaps = find_gaps_in_alignment(preprocessed_alignment)
     unique_gaps = find_unique_gaps(all_gaps)
 
     if unique_gaps:
         gap_dic = create_gap_dictionary(unique_gaps, all_gaps)
         gaps_to_mask = find_gaps_to_mask(gap_dic, gap_cutoff)
-        alignment_cleaned = clean_gaps(
-            preprocessed_alignment, gaps_to_mask
-        )
+        if gaps_to_mask:
+            alignment_cleaned = alignment.clean_gaps(
+                preprocessed_alignment, gaps_to_mask
+            )
+        else:
+            alignment_cleaned = preprocessed_alignment
     else:
         gaps_to_mask = []
         alignment_cleaned = preprocessed_alignment
 
     return alignment_cleaned, gaps_to_mask
```

### Comparing `varvamp-0.8/varvamp/scripts/config.py` & `varvamp-0.8.1/varvamp/scripts/config.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/consensus.py` & `varvamp-0.8.1/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/logging.py` & `varvamp-0.8.1/varvamp/scripts/logging.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/param_estimation.py` & `varvamp-0.8.1/varvamp/scripts/param_estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     nuc freq that fell below the cutoff
     """
 
     current_dis = 0
     previous_dis = 0
     all_dis = []
 
-    for freq in all_freqs:
+    for idx, freq in enumerate(all_freqs):
         if freq < threshold:
             current_dis = 0
         current_dis += 1
-        if current_dis <= previous_dis:
+        if current_dis <= previous_dis or idx == len(all_freqs)-1:
             all_dis.append(previous_dis)
 
         previous_dis = current_dis
 
     return all_dis
 
 
@@ -81,15 +81,15 @@
             distances = calculate_distances(frequencys, args.threshold)
             # calculate the cummulative sum of the sum of n conseq. streches
             # that are together larger than the min primer length
             covered_pos = sum(
                 [distances[x] for x in range(0, len(distances)) if sum(distances[x:x+args.n_ambig+1]) >= config.PRIMER_SIZES[0]]
             )
             # calculate coverage
-            coverage = covered_pos/len(preprocessed_alignment[0][1])
+            coverage = (covered_pos+1)/len(preprocessed_alignment[0][1])
             # change the non fixed param if threshold has not been reached
             if coverage >= 0.5:
                 # write each iteration to log
                 print(round(args.threshold, 2), args.n_ambig, round(coverage*100, 1), sep="\t", file=f)
                 if fixed:
                     args.n_ambig -= 1
                 else:
```

### Comparing `varvamp-0.8/varvamp/scripts/primers.py` & `varvamp-0.8.1/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/qpcr.py` & `varvamp-0.8.1/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/regions.py` & `varvamp-0.8.1/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/reporting.py` & `varvamp-0.8.1/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp/scripts/scheme.py` & `varvamp-0.8.1/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8/varvamp.egg-info/PKG-INFO` & `varvamp-0.8.1/varvamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8
+Version: 0.8.1
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.8/varvamp.egg-info/SOURCES.txt` & `varvamp-0.8.1/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


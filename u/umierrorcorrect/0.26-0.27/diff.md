# Comparing `tmp/umierrorcorrect-0.26.tar.gz` & `tmp/umierrorcorrect-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/xsteto/new/umierrorcorrect/dist/tmpzdatilqv/umierrorcorrect-0.26.tar", last modified: Fri Apr 14 12:15:47 2023, max compression
+gzip compressed data, was "dist/umierrorcorrect-0.27.tar", last modified: Thu Apr 27 14:07:05 2023, max compression
```

## Comparing `umierrorcorrect-0.26.tar` & `umierrorcorrect-0.27.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:46.000000 umierrorcorrect-0.26/umierrorcorrect/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect/src/
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4943 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/src/check_args.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    18485 2023-04-06 11:29:48.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2022-08-30 07:25:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/group.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2022-03-22 13:55:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/umierrorcorrect/call_variants.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_bam.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    11999 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/preprocess.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/run_mapping.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     9404 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    25529 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-04-14 12:12:43.000000 umierrorcorrect-0.26/umierrorcorrect/version.py
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO
--rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-04-14 12:15:45.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/dependency_links.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/not-zip-safe
--rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/requires.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/top_level.txt
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.26/LICENSE.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)     2715 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/README.md
--rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/setup.cfg
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/setup.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/PKG-INFO
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/umierrorcorrect/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/umierrorcorrect/src/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/src/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4943 2023-04-14 12:03:38.000000 umierrorcorrect-0.27/umierrorcorrect/src/check_args.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.27/umierrorcorrect/src/get_cons_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    18634 2023-04-27 13:30:25.000000 umierrorcorrect-0.27/umierrorcorrect/src/get_consensus3.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.27/umierrorcorrect/src/get_regions_from_bed.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2023-04-21 09:25:03.000000 umierrorcorrect-0.27/umierrorcorrect/src/group.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2023-04-21 08:52:28.000000 umierrorcorrect-0.27/umierrorcorrect/src/handle_sequences.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.27/umierrorcorrect/src/umi_cluster.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 10:10:04.000000 umierrorcorrect-0.27/umierrorcorrect/call_variants.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.27/umierrorcorrect/downsampling_plots.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/filter_bam.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/filter_cons.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/filter_cons2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/filter_vcf.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.27/umierrorcorrect/fit_background_model.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.27/umierrorcorrect/get_consensus_statistics.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.27/umierrorcorrect/get_consensus_statistics2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.27/umierrorcorrect/get_umi_cluster_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    11999 2023-04-21 09:02:11.000000 umierrorcorrect-0.27/umierrorcorrect/preprocess.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.27/umierrorcorrect/run_mapping.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     9404 2023-04-14 12:03:38.000000 umierrorcorrect-0.27/umierrorcorrect/run_umierrorcorrect.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.27/umierrorcorrect/test_cons_info_indel.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    25529 2023-04-27 13:29:13.000000 umierrorcorrect-0.27/umierrorcorrect/umi_error_correct.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-04-27 14:06:09.000000 umierrorcorrect-0.27/umierrorcorrect/version.py
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3818 2023-04-27 14:07:03.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/PKG-INFO
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-04-27 14:07:03.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/SOURCES.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-04-27 14:07:03.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/dependency_links.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/not-zip-safe
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-04-27 14:07:03.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/requires.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-04-27 14:07:03.000000 umierrorcorrect-0.27/umierrorcorrect.egg-info/top_level.txt
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.27/LICENSE.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     2715 2023-04-06 10:10:04.000000 umierrorcorrect-0.27/README.md
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/setup.cfg
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.27/setup.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3818 2023-04-27 14:07:05.000000 umierrorcorrect-0.27/PKG-INFO
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/check_args.py` & `umierrorcorrect-0.27/umierrorcorrect/src/check_args.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py` & `umierrorcorrect-0.27/umierrorcorrect/src/get_cons_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py` & `umierrorcorrect-0.27/umierrorcorrect/src/get_consensus3.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
                         if base not in consensus[refpos]:
                             consensus[refpos][base] = []
                         consensus[refpos][base].append(get_phred(qual[qpos]))
                     elif not refpos == ref + 1:
                         # deletion
                         dellength = refpos - (ref+1) #get the length of the deletion
                         delpos = refpos - dellength
+                        #print(consensus[delpos])
                         if delpos not in consensus:
                             consensus[delpos] = {}
                         if 'D' not in consensus[delpos]:
                             consensus[delpos]['D'] = {}
                         if dellength not in consensus[delpos]['D']:
                             consensus[delpos]['D'][dellength] = 0
                         consensus[delpos]['D'][dellength] += 1
@@ -266,15 +267,14 @@
                         if refpos not in consensus:
                             consensus[refpos] = {}
                         if base not in consensus[refpos]:
                             consensus[refpos][base] = []
                         consensus[refpos][base].append(get_phred(qual[qpos]))
                     q = qpos
                     ref = refpos
-    
     if len(consensus) > 0:
         #generate the consensus sequence
         consensus_sorted = sorted(consensus)
         consread = None
         add_consensus = True
         skippos = [] #if position is del
         prevpos = consensus_sorted[0] - 1
@@ -299,22 +299,24 @@
                         consread.add_insertion(sequence)
                     del(consensus[pos]['I'])
                     if poscov < 50:
                         cons_base, cons_qual = calc_consensus_probabilities(consensus[pos])
                     else:
                         cons_base, percent = get_most_common_allele(consensus[pos])
                         cons_qual = 60
-                    consread.add_base(cons_base, get_ascii(cons_qual))
+                    if not cons_base.startswith('D'):
+                        consread.add_base(cons_base, get_ascii(cons_qual))
 
                 elif 'D' in consensus[pos] and poscov >= 2:
                     # add the deletions
                     a, percent = get_most_common_allele(consensus[pos])
                     if a.startswith('D'):
                         if percent >= indel_freq_threshold:
                             dellength = int(a.lstrip('D'))
+                            #print(dellength)
                             consread.add_deletion(dellength)
                             if dellength > 1:
                                 for i in range(1,dellength):
                                     skippos.append(pos + i)
                         else:
                             consread.add_base('N', get_ascii(0))
                             add_consensus = False
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py` & `umierrorcorrect-0.27/umierrorcorrect/src/get_regions_from_bed.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/group.py` & `umierrorcorrect-0.27/umierrorcorrect/src/group.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py` & `umierrorcorrect-0.27/umierrorcorrect/src/handle_sequences.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py` & `umierrorcorrect-0.27/umierrorcorrect/src/umi_cluster.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/call_variants.py` & `umierrorcorrect-0.27/umierrorcorrect/call_variants.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py` & `umierrorcorrect-0.27/umierrorcorrect/downsampling_plots.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_bam.py` & `umierrorcorrect-0.27/umierrorcorrect/filter_bam.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_cons.py` & `umierrorcorrect-0.27/umierrorcorrect/filter_cons.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py` & `umierrorcorrect-0.27/umierrorcorrect/filter_cons2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py` & `umierrorcorrect-0.27/umierrorcorrect/filter_vcf.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py` & `umierrorcorrect-0.27/umierrorcorrect/fit_background_model.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py` & `umierrorcorrect-0.27/umierrorcorrect/get_consensus_statistics.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py` & `umierrorcorrect-0.27/umierrorcorrect/get_consensus_statistics2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py` & `umierrorcorrect-0.27/umierrorcorrect/get_umi_cluster_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/preprocess.py` & `umierrorcorrect-0.27/umierrorcorrect/preprocess.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/run_mapping.py` & `umierrorcorrect-0.27/umierrorcorrect/run_mapping.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py` & `umierrorcorrect-0.27/umierrorcorrect/run_umierrorcorrect.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py` & `umierrorcorrect-0.27/umierrorcorrect/test_cons_info_indel.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py` & `umierrorcorrect-0.27/umierrorcorrect/umi_error_correct.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO` & `umierrorcorrect-0.27/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: umierrorcorrect
-Version: 0.26
-Summary: UMI error correct
-Home-page: http://github.com/stahlberggroup/umierrorcorrect
-Author: Tobias Osterlund
-Author-email: tobias.osterlund@gu.se
-License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-License-File: LICENSE.txt
-
 # umierrorcorrect
 
 Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
 
 
 Reference
 ---------
@@ -95,9 +82,7 @@
 [Link to the Umierrorcorrect tutorial](https://github.com/stahlberggroup/umierrorcorrect/wiki/Tutorial)
 
 
 Example of UMI definition options
 ----------------------------------
 
 [UMI definition options](https://github.com/stahlberggroup/umierrorcorrect/wiki/UMI-definition-options)
-
-
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt` & `umierrorcorrect-0.27/umierrorcorrect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/LICENSE.txt` & `umierrorcorrect-0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/README.md` & `umierrorcorrect-0.27/umierrorcorrect.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,100 @@
-# umierrorcorrect
-
-Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
-
-
-Reference
----------
-
-UMIErrorCorrect has been published in Clinical Chemistry.
-
-[Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
-
-Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
-
-Installation
-------------
-
-To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
-
-To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
-
-```
-pip install umierrorcorrect
-```
-    
-After installation, try to run the pipeline:
-
-```
-run_umierrorcorrect.py -h
-```
-
-Dependencies
-------------
-
-Umi-errorcorrect runs using Python 3 and requires the following programs/libraries to be installed (if you run through docker all dependencies are already handled):
-
-Python-libraries (should be installed automatically):
-
-    pysam (v 0.8.4 or greater)
-
-External programs:
-
-    bwa (bwa mem command is used)
-    Either of gzip or pigz (parallel gzip)
-
-Install the external programs and add them to the path.
-
-Since the umierrorcorrect pipeline is using `bwa` for mapping of reads, a bwa-indexed reference genome is needed. Index the reference genome with the command `bwa index -a bwtsw reference.fa`.
-
-Usage
------
-
-Example syntax for running the whole pipeline:
-
-    run_umierrorcorrect.py -r1 read1.fastq.gz -r2 read2.fastq.gz -ul umi_length -sl spacer_length -r reference_fasta_file.fasta -o output_directory
-
-The ``run_umierrorcorrect.py`` pipeline performs the following steps:
-
-- Preprocessing of fastq files (remove the UMI and spacer and puts the UMI in the header)
-- Mapping of preprocessed fastq reads to the reference genome
-- Perform UMI clustering, then error correcion of each UMI cluster
-- Create consensus reads (one representative read per UMI cluster written to a BAM file)
-- Create a consensus output file (collapsed counts per position)
-- Perform variant calling.
-
-It is also to possible to run the pipeline step-by-step.
-
-To see the options for each step, type the following:
-
-```
-preprocess.py -h
-run_mapping.py -h
-umi_error_correct.py -h
-get_consensus_statistics.py -h
-call_variants.py -h
-filter_bam.py -h
-filter_cons.py -h
-```
-Tutorial
---------
-
-[Link to the Umierrorcorrect tutorial](https://github.com/stahlberggroup/umierrorcorrect/wiki/Tutorial)
-
-
-Example of UMI definition options
-----------------------------------
-
-[UMI definition options](https://github.com/stahlberggroup/umierrorcorrect/wiki/UMI-definition-options)
+Metadata-Version: 1.1
+Name: umierrorcorrect
+Version: 0.27
+Summary: UMI error correct
+Home-page: http://github.com/stahlberggroup/umierrorcorrect
+Author: Tobias Osterlund
+Author-email: tobias.osterlund@gu.se
+License: mit
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.27.tar.gz
+Description: # umierrorcorrect
+        
+        Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
+        
+        
+        Reference
+        ---------
+        
+        UMIErrorCorrect has been published in Clinical Chemistry.
+        
+        [Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
+        
+        Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
+        
+        Installation
+        ------------
+        
+        To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
+        
+        To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
+        
+        ```
+        pip install umierrorcorrect
+        ```
+            
+        After installation, try to run the pipeline:
+        
+        ```
+        run_umierrorcorrect.py -h
+        ```
+        
+        Dependencies
+        ------------
+        
+        Umi-errorcorrect runs using Python 3 and requires the following programs/libraries to be installed (if you run through docker all dependencies are already handled):
+        
+        Python-libraries (should be installed automatically):
+        
+            pysam (v 0.8.4 or greater)
+        
+        External programs:
+        
+            bwa (bwa mem command is used)
+            Either of gzip or pigz (parallel gzip)
+        
+        Install the external programs and add them to the path.
+        
+        Since the umierrorcorrect pipeline is using `bwa` for mapping of reads, a bwa-indexed reference genome is needed. Index the reference genome with the command `bwa index -a bwtsw reference.fa`.
+        
+        Usage
+        -----
+        
+        Example syntax for running the whole pipeline:
+        
+            run_umierrorcorrect.py -r1 read1.fastq.gz -r2 read2.fastq.gz -ul umi_length -sl spacer_length -r reference_fasta_file.fasta -o output_directory
+        
+        The ``run_umierrorcorrect.py`` pipeline performs the following steps:
+        
+        - Preprocessing of fastq files (remove the UMI and spacer and puts the UMI in the header)
+        - Mapping of preprocessed fastq reads to the reference genome
+        - Perform UMI clustering, then error correcion of each UMI cluster
+        - Create consensus reads (one representative read per UMI cluster written to a BAM file)
+        - Create a consensus output file (collapsed counts per position)
+        - Perform variant calling.
+        
+        It is also to possible to run the pipeline step-by-step.
+        
+        To see the options for each step, type the following:
+        
+        ```
+        preprocess.py -h
+        run_mapping.py -h
+        umi_error_correct.py -h
+        get_consensus_statistics.py -h
+        call_variants.py -h
+        filter_bam.py -h
+        filter_cons.py -h
+        ```
+        Tutorial
+        --------
+        
+        [Link to the Umierrorcorrect tutorial](https://github.com/stahlberggroup/umierrorcorrect/wiki/Tutorial)
+        
+        
+        Example of UMI definition options
+        ----------------------------------
+        
+        [UMI definition options](https://github.com/stahlberggroup/umierrorcorrect/wiki/UMI-definition-options)
+        
+Platform: UNKNOWN
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `umierrorcorrect-0.26/setup.py` & `umierrorcorrect-0.27/setup.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/PKG-INFO` & `umierrorcorrect-0.27/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,100 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: umierrorcorrect
-Version: 0.26
+Version: 0.27
 Summary: UMI error correct
 Home-page: http://github.com/stahlberggroup/umierrorcorrect
 Author: Tobias Osterlund
 Author-email: tobias.osterlund@gu.se
 License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.27.tar.gz
+Description: # umierrorcorrect
+        
+        Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
+        
+        
+        Reference
+        ---------
+        
+        UMIErrorCorrect has been published in Clinical Chemistry.
+        
+        [Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
+        
+        Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
+        
+        Installation
+        ------------
+        
+        To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
+        
+        To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
+        
+        ```
+        pip install umierrorcorrect
+        ```
+            
+        After installation, try to run the pipeline:
+        
+        ```
+        run_umierrorcorrect.py -h
+        ```
+        
+        Dependencies
+        ------------
+        
+        Umi-errorcorrect runs using Python 3 and requires the following programs/libraries to be installed (if you run through docker all dependencies are already handled):
+        
+        Python-libraries (should be installed automatically):
+        
+            pysam (v 0.8.4 or greater)
+        
+        External programs:
+        
+            bwa (bwa mem command is used)
+            Either of gzip or pigz (parallel gzip)
+        
+        Install the external programs and add them to the path.
+        
+        Since the umierrorcorrect pipeline is using `bwa` for mapping of reads, a bwa-indexed reference genome is needed. Index the reference genome with the command `bwa index -a bwtsw reference.fa`.
+        
+        Usage
+        -----
+        
+        Example syntax for running the whole pipeline:
+        
+            run_umierrorcorrect.py -r1 read1.fastq.gz -r2 read2.fastq.gz -ul umi_length -sl spacer_length -r reference_fasta_file.fasta -o output_directory
+        
+        The ``run_umierrorcorrect.py`` pipeline performs the following steps:
+        
+        - Preprocessing of fastq files (remove the UMI and spacer and puts the UMI in the header)
+        - Mapping of preprocessed fastq reads to the reference genome
+        - Perform UMI clustering, then error correcion of each UMI cluster
+        - Create consensus reads (one representative read per UMI cluster written to a BAM file)
+        - Create a consensus output file (collapsed counts per position)
+        - Perform variant calling.
+        
+        It is also to possible to run the pipeline step-by-step.
+        
+        To see the options for each step, type the following:
+        
+        ```
+        preprocess.py -h
+        run_mapping.py -h
+        umi_error_correct.py -h
+        get_consensus_statistics.py -h
+        call_variants.py -h
+        filter_bam.py -h
+        filter_cons.py -h
+        ```
+        Tutorial
+        --------
+        
+        [Link to the Umierrorcorrect tutorial](https://github.com/stahlberggroup/umierrorcorrect/wiki/Tutorial)
+        
+        
+        Example of UMI definition options
+        ----------------------------------
+        
+        [UMI definition options](https://github.com/stahlberggroup/umierrorcorrect/wiki/UMI-definition-options)
+        
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-License-File: LICENSE.txt
-
-# umierrorcorrect
-
-Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
-
-
-Reference
----------
-
-UMIErrorCorrect has been published in Clinical Chemistry.
-
-[Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
-
-Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
-
-Installation
-------------
-
-To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
-
-To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
-
-```
-pip install umierrorcorrect
-```
-    
-After installation, try to run the pipeline:
-
-```
-run_umierrorcorrect.py -h
-```
-
-Dependencies
-------------
-
-Umi-errorcorrect runs using Python 3 and requires the following programs/libraries to be installed (if you run through docker all dependencies are already handled):
-
-Python-libraries (should be installed automatically):
-
-    pysam (v 0.8.4 or greater)
-
-External programs:
-
-    bwa (bwa mem command is used)
-    Either of gzip or pigz (parallel gzip)
-
-Install the external programs and add them to the path.
-
-Since the umierrorcorrect pipeline is using `bwa` for mapping of reads, a bwa-indexed reference genome is needed. Index the reference genome with the command `bwa index -a bwtsw reference.fa`.
-
-Usage
------
-
-Example syntax for running the whole pipeline:
-
-    run_umierrorcorrect.py -r1 read1.fastq.gz -r2 read2.fastq.gz -ul umi_length -sl spacer_length -r reference_fasta_file.fasta -o output_directory
-
-The ``run_umierrorcorrect.py`` pipeline performs the following steps:
-
-- Preprocessing of fastq files (remove the UMI and spacer and puts the UMI in the header)
-- Mapping of preprocessed fastq reads to the reference genome
-- Perform UMI clustering, then error correcion of each UMI cluster
-- Create consensus reads (one representative read per UMI cluster written to a BAM file)
-- Create a consensus output file (collapsed counts per position)
-- Perform variant calling.
-
-It is also to possible to run the pipeline step-by-step.
-
-To see the options for each step, type the following:
-
-```
-preprocess.py -h
-run_mapping.py -h
-umi_error_correct.py -h
-get_consensus_statistics.py -h
-call_variants.py -h
-filter_bam.py -h
-filter_cons.py -h
-```
-Tutorial
---------
-
-[Link to the Umierrorcorrect tutorial](https://github.com/stahlberggroup/umierrorcorrect/wiki/Tutorial)
-
-
-Example of UMI definition options
-----------------------------------
-
-[UMI definition options](https://github.com/stahlberggroup/umierrorcorrect/wiki/UMI-definition-options)
-
-
```


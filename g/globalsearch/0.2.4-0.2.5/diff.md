# Comparing `tmp/globalsearch-0.2.4.tar.gz` & `tmp/globalsearch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.2.4.tar", last modified: Tue Apr 18 21:04:14 2023, max compression
+gzip compressed data, was "globalsearch-0.2.5.tar", last modified: Thu Apr 27 17:47:40 2023, max compression
```

## Comparing `globalsearch-0.2.4.tar` & `globalsearch-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.095470 globalsearch-0.2.4/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-18 21:04:14.095543 globalsearch-0.2.4/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.4/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.091241 globalsearch-0.2.4/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.4/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.4/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.090272 globalsearch-0.2.4/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.092435 globalsearch-0.2.4/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.4/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.4/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.095214 globalsearch-0.2.4/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.4/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7239 2023-04-18 20:14:08.000000 globalsearch-0.2.4/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.4/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.4/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.4/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.4/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.4/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.4/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.4/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    13278 2023-04-11 22:07:15.000000 globalsearch-0.2.4/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3662 2023-04-18 21:03:09.000000 globalsearch-0.2.4/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-18 21:04:14.092214 globalsearch-0.2.4/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-18 21:04:14.000000 globalsearch-0.2.4/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-18 21:04:14.000000 globalsearch-0.2.4/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-18 21:04:14.000000 globalsearch-0.2.4/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.4/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-18 21:04:14.000000 globalsearch-0.2.4/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-18 21:04:14.000000 globalsearch-0.2.4/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-18 21:04:14.095802 globalsearch-0.2.4/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-18 21:03:18.000000 globalsearch-0.2.4/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.857352 globalsearch-0.2.5/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-27 17:47:40.857422 globalsearch-0.2.5/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.5/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.853001 globalsearch-0.2.5/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.5/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.5/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.852151 globalsearch-0.2.5/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.854265 globalsearch-0.2.5/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.5/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.5/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.857114 globalsearch-0.2.5/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.5/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7239 2023-04-18 20:14:08.000000 globalsearch-0.2.5/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.5/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.5/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.5/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.5/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.5/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.5/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    15368 2023-04-27 17:44:05.000000 globalsearch-0.2.5/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    13279 2023-04-27 17:44:05.000000 globalsearch-0.2.5/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3662 2023-04-18 21:03:09.000000 globalsearch-0.2.5/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 17:47:40.854027 globalsearch-0.2.5/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-27 17:47:40.000000 globalsearch-0.2.5/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-27 17:47:40.000000 globalsearch-0.2.5/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-27 17:47:40.000000 globalsearch-0.2.5/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.5/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-27 17:47:40.000000 globalsearch-0.2.5/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-27 17:47:40.000000 globalsearch-0.2.5/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-27 17:47:40.857622 globalsearch-0.2.5/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-27 17:47:06.000000 globalsearch-0.2.5/setup.py
```

### Comparing `globalsearch-0.2.4/PKG-INFO` & `globalsearch-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.4
+Version: 0.2.5
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.4/bin/gs_prepare` & `globalsearch-0.2.5/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/bin/gs_submit` & `globalsearch-0.2.5/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/control/gs_prepare.py` & `globalsearch-0.2.5/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/find_files.py` & `globalsearch-0.2.5/globalsearch/rnaseq/find_files.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/index_star.py` & `globalsearch-0.2.5/globalsearch/rnaseq/index_star.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.2.5/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.2.5/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.2.5/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.2.5/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.2.5/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.2.5/globalsearch/rnaseq/run_spladder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 #############################################################
 ##### RNASeq Analysis Pipeline - SplAdder               #####
-##### Last update: 2023/03/01 by Yaqiao Li              #####
+##### Last update: 2023/03/31 by Yaqiao Li              #####
 ##### Institute for Systems Biology                     #####
 #############################################################
 import glob, sys, os, string, datetime, re, errno, time
 import argparse
 from multiprocessing import Pool, cpu_count, Manager
 from subprocess import *
 #from pathos.multiprocessing import ProcessingPoll as Pool
@@ -198,23 +198,33 @@
                 for f in files:
                     if f.endswith('pickle'):
                         cf.write('rm ' + os.path.join(root, f) + '\n')
     errOut.close()
     cf.close()
     return cleanUp
 
+####################### Write Clean.sh  #####################################
+def Write_Clean():
+    cf = open('cleanUp.sh','w')
+    cf.write('#Remove temporary files\n\n')
+    for root, dirs, files in os.walk(spladder_out_dir):
+                for f in files:
+                    if f.endswith('pickle'):
+                        cf.write('rm ' + os.path.join(root, f) + '\n')
+    cf.close()
+
 ####################### Clean Up temporary files  ###############################
 def Clean_Up(spladder_out_dir):
     for root, dirs, files in os.walk(spladder_out_dir):
         for f in files:
             if f.endswith('pickle'):
                 os.remove(os.path.join(root, f))
 
 ####################### Run SplAdder ############################################
-def run_spladder(spladder_work_dir, spladder_out_dir, parsed_event_dir, input_bam_list, genome_annotation, all_contrasts, contrast_dir, sampleType, args):
+def run_spladder(spladder_work_dir, spladder_out_dir, parsed_event_dir, input_bam_list, genome_annotation, all_contrasts, contrast_dir, sample_type, args):
     # Run create directories function to create directory structure
     create_dirs(spladder_work_dir, spladder_out_dir, parsed_event_dir)
     
     #---run step 1
     bamlist = open(input_bam_list, 'r')
     bams = []
     for line in bamlist:
@@ -297,22 +307,22 @@
 one_ldf$spec <- c("'''
 
     strR3_1 = r'''")
 
 #write out the results as one table
 write.table(one_ldf, paste0("'''
 
-    if(sampleType == 'host'):
+    if(sample_type == 'host'):
         strR4 = parsed_event_dir + '/host_all_events'
-    elif(sampleType == 'sym'):
+    elif(sample_type == 'sym'):
         strR4 = parsed_event_dir + '/sym_all_events'
     else:
         strR4 = parsed_event_dir + '/other_all_events'
     strR5 = r'",var1,const,"_vs_",var2,const,".tsv"), quote = F, row.names = F)'
-    strR = strR1 + strR2 + strR3 + sampleType + strR3_1 + strR4 + strR5 + '\n'
+    strR = strR1 + strR2 + strR3 + sample_type + strR3_1 + strR4 + strR5 + '\n'
     parseR = open(parseRscript, 'w')
     parseR.write(strR)
     parseR.close()
 
     partial_work_step7 = partial(SplAdder_step7_parsing_statistic, parseRscript=parseRscript)
     cpus = 16
     pool = Pool(processes=cpus)
@@ -326,57 +336,63 @@
 
 
 
 ####################### Main ####################################################
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description=DESCRIPTION)
-    parser.add_argument('-w', '--WorkDir', help='work directory')
-    parser.add_argument('-i', '--inputBamFileList', help='input .bam file name list')
-    parser.add_argument('-a', '--genomeAnnotation', help='genome GFF/GTF file')
-    parser.add_argument('-c', '--allContrasts', help='sample contrasts information: all_contrasts.txt')
-    parser.add_argument('-d', '--contrastDir', help='sample contrasts information: contrast_file')
-    parser.add_argument('-s', '--sampleType', help='sample is host or symbiont or Other')
+    #parser.add_argument('WorkDir', type=str, help='work directory')
+    parser.add_argument('-w', '--WorkDir', type=str, help='work directory')
+    parser.add_argument('-i', '--inputBamFileList',  type=str, help='input .bam file name list')
+    parser.add_argument('-a', '--genomeAnnotation',  type=str, help='genome GFF/GTF file')
+    parser.add_argument('-c', '--allContrasts',  type=str, help='sample contrasts information: all_contrasts.txt')
+    parser.add_argument('-d', '--contrastDir',  type=str, help='sample contrasts information: contrast_file')
+    parser.add_argument('-s', '--sampleType',  type=str, help='sample is host or symbiont or Other')
+    #parser.add_argument('-s', '--sampleType',  type=str, help='sample is host or symbiont or Other', default='host')
     
     args = parser.parse_args()
     
     work_dir = args.WorkDir
     input_bam_list = args.inputBamFileList
     genome_annotation = args.genomeAnnotation
     all_contrasts = args.allContrasts
     contrast_dir = args.contrastDir
-    sampleType = args.sampleType
+    sample_type = args.sampleType
     
-    spladder_work_dir = work_dir + '/' + sampleType + '_spladder_jobs'
-    spladder_out_dir = work_dir + '/' + sampleType + '_spladder_jobs' + '/array_spladder_out'
-    if sampleType == 'host' or sampleType == 'sym':
+    spladder_work_dir = work_dir + '/' + sample_type + '_spladder_jobs'
+    spladder_out_dir = work_dir + '/' + sample_type + '_spladder_jobs' + '/array_spladder_out'
+    if sample_type == 'host' or sample_type == 'sym':
         parsed_event_dir = work_dir + '/host_sym_parsed_event_files'
     else:
-        parsed_event_dir = work_dir + '/' + sampleType + '_parsed_event_files'
+        parsed_event_dir = work_dir + '/' + sample_type + '_parsed_event_files'
 
     errOut = open('ErrorReport.txt','w')
     starttime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
     errOut.write('Start: ' + starttime + '\n\n')
     errOut.close()
-    run_spladder(spladder_work_dir, spladder_out_dir, parsed_event_dir, input_bam_list, genome_annotation, all_contrasts, contrast_dir, sampleType, args)
+    run_spladder(spladder_work_dir, spladder_out_dir, parsed_event_dir, input_bam_list, genome_annotation, all_contrasts, contrast_dir, sample_type, args)
     errOut = open('ErrorReport.txt','a')
     endtime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
     errOut.write('\nEnd: ' + endtime + '\n\n')
     errOut.close()
     
     # check errors
-    cleanUp = Check_Error_Report()
+    #cleanUp = Check_Error_Report()
     
+
+    # write clean.sh
+    Write_Clean()
+
     # clean up
-    errOut = open('ErrorReport.txt','a')
-    if cleanUp:
-        Clean_Up(spladder_out_dir)
-        cleantime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-        errOut.write('\nCleanedUp: ' + cleantime + '\n\n')
-    else:
-        cleantime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-        errOut.write('\nCan not cleanedUp: ' + cleantime + '\n\n')     
-    errOut.close()
+    #errOut = open('ErrorReport.txt','a')
+    #if cleanUp:
+    #    Clean_Up(spladder_out_dir)
+    #    cleantime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+    #    errOut.write('\nCleanedUp: ' + cleantime + '\n\n')
+    #else:
+    #    cleantime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+    #    errOut.write('\nCan not cleanedUp: ' + cleantime + '\n\n')     
+    #errOut.close()
```

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.2.5/globalsearch/rnaseq/run_star_salmon.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     ## STAR based BAM duplicate removal
     # Mark duplicates with STAR
     print('STAR mark duplicates run command:%s' % star_markdup_cmd, flush=True)
     compl_proc = subprocess.run(star_markdup_command, check=True, capture_output=False, cwd=results_dir)
 
     # Remove marked duplicates withh samtools
     print('Samtools  STAR Dedup Remove run command:%s' % rmsingletonsSTAR_cmd, flush=True)
-    compl_proc = subprocess.run(rmsingletonSTAR_command, check=True, capture_output=False, cwd=results_dir)
+    compl_proc = subprocess.run(rmsingletonsSTAR_command, check=True, capture_output=False, cwd=results_dir)
 
     # Remove marked duplicates withh samtools
     print('Samtools  Collate reads by read name run command:%s' % collatereadsSTAR_cmd, flush=True)
     compl_proc = subprocess.run(collatereadsSTAR_command, check=True, capture_output=False, cwd=results_dir)
 
 
 ####################### Run Salmon Count ###############################
```

### Comparing `globalsearch-0.2.4/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.2.5/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.2.5/globalsearch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.4
+Version: 0.2.5
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.4/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.2.5/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.4/setup.py` & `globalsearch-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```


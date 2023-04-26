# Comparing `tmp/pssm-promoter-tool-1.0.0.tar.gz` & `tmp/pssm-promoter-tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssm-promoter-tool-1.0.0.tar", last modified: Wed Apr 26 03:59:34 2023, max compression
+gzip compressed data, was "pssm-promoter-tool-1.0.1.tar", last modified: Wed Apr 26 10:51:52 2023, max compression
```

## Comparing `pssm-promoter-tool-1.0.0.tar` & `pssm-promoter-tool-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 03:59:34.747793 pssm-promoter-tool-1.0.0/
--rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.0/LICENSE.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.0/MANIFEST.in
--rw-r--r--   0 ellinium   (501) staff       (20)     3628 2023-04-26 03:59:34.747631 pssm-promoter-tool-1.0.0/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)     3171 2023-04-26 01:45:11.000000 pssm-promoter-tool-1.0.0/README.md
--rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.0/free_energy_coeffs.npy
--rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.0/model_intercept.npy
--rw-r--r--   0 ellinium   (501) staff       (20)    12084 2023-04-26 02:03:27.000000 pssm-promoter-tool-1.0.0/pssm_promoter_calculator.py
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 03:59:34.747423 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/
--rw-r--r--   0 ellinium   (501) staff       (20)     3628 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/not-zip-safe
--rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/requires.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.0/pssm_promoter_tool.egg-info/top_level.txt
--rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.0/pyproject.toml
--rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-04-26 03:59:34.747839 pssm-promoter-tool-1.0.0/setup.cfg
--rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-04-26 03:58:51.000000 pssm-promoter-tool-1.0.0/setup.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 10:51:52.453030 pssm-promoter-tool-1.0.1/
+-rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.1/LICENSE.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.1/MANIFEST.in
+-rw-r--r--   0 ellinium   (501) staff       (20)     4703 2023-04-26 10:51:52.452864 pssm-promoter-tool-1.0.1/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)     4246 2023-04-26 10:47:55.000000 pssm-promoter-tool-1.0.1/README.md
+-rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.1/free_energy_coeffs.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.1/model_intercept.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)    12158 2023-04-26 05:57:16.000000 pssm-promoter-tool-1.0.1/pssm_promoter_calculator.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 10:51:52.452614 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/
+-rw-r--r--   0 ellinium   (501) staff       (20)     4703 2023-04-26 10:51:52.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-04-26 10:51:52.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 10:51:52.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/not-zip-safe
+-rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-04-26 10:51:52.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/requires.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-04-26 10:51:52.000000 pssm-promoter-tool-1.0.1/pssm_promoter_tool.egg-info/top_level.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.1/pyproject.toml
+-rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-04-26 10:51:52.453080 pssm-promoter-tool-1.0.1/setup.cfg
+-rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-04-26 10:50:27.000000 pssm-promoter-tool-1.0.1/setup.py
```

### Comparing `pssm-promoter-tool-1.0.0/LICENSE.txt` & `pssm-promoter-tool-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.0/free_energy_coeffs.npy` & `pssm-promoter-tool-1.0.1/free_energy_coeffs.npy`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.0/pssm_promoter_calculator.py` & `pssm-promoter-tool-1.0.1/pssm_promoter_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 from datetime import datetime
-from Bio import Seq, SeqIO
+from Bio.Seq import Seq
+from Bio import SeqIO
 import sys
 #For colab
 #from google.colab import files
 ##sys.path.append(os.path.abspath('PSSM_PromoterTool/'))
 import pssm_util
 
 OUTPUT_FILE_NAME = "PSSMPromoterCalculator"
@@ -20,14 +21,16 @@
     f_content = f.read()
 
     if '>' in f_content:
         records = list(SeqIO.parse(gene_file_name, "fasta"))
         gene_sequence = str(records[0].seq)
     else:
         gene_sequence = f_content
+
+    print("processing " + gene_file_name)
     return str.upper(gene_sequence)
 
 
 if __name__ == "__main__":
 
     from dask.distributed import Client, LocalCluster
     # cluster = LocalCluster()  # Launches a scheduler and workers locally
@@ -170,55 +173,55 @@
     res_final_df_min_rev_df = res_final_df_min.loc[res_final_df_min["direction"] == 'rev']
     new_min_rev_Tx_rate_df = res_final_df_min_rev_df.sort_values(by='Tx_rate', ascending=False)
     new_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
     column_list = ["new_gene_sequence", "promoter_sequence", "TSS", "Tx_rate", "UP", "hex35", "PSSM_hex35", "AA_hex35", "spacer", "hex10", "PSSM_hex10", "AA_hex10", "disc", "ITR", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
 
     print("\n")
-    print("The minimum transcription rate for the sequence (forward) " + str(def_fwd_min_tx_rate))
+    print("The minimum transcription rate for the sequence (forward) is " + str(def_fwd_min_tx_rate))
     if len(res_final_df_min_fwd_df) > 1:
         min_fwd_output_file = OUTPUT_FILE_NAME + "_MIN_FWD_results.csv"
         if float(new_min_fwd_Tx_rate) < float(def_fwd_min_tx_rate):
             print ("can be decreased up to " + str(new_min_fwd_Tx_rate))
             print("using the promoters in the " + min_fwd_output_file)
             res_final_df_max_fwd_df.to_csv(min_fwd_output_file, columns = column_list)
 
             ##files.download(min_fwd_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\n")
-    print("The minimum transcription rate for the sequence (reverse) " + str(def_rev_min_tx_rate))
+    print("The minimum transcription rate for the sequence (reverse) is " + str(def_rev_min_tx_rate))
     if len(res_final_df_min_rev_df) > 1:
         min_rev_output_file = OUTPUT_FILE_NAME + "_MIN_REV_results.csv"
         if float(new_min_rev_Tx_rate) < float(def_rev_min_tx_rate):
             print ("can be decreased up to " + str(new_min_rev_Tx_rate))
             print("using the promoters in the " + min_rev_output_file)
             res_final_df_max_fwd_df.to_csv(min_rev_output_file, columns = column_list)
 
             ##files.download(min_rev_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\n")
-    print("The maximum transcription rate for the sequence (forward) " + str(def_fwd_max_tx_rate))
+    print("The maximum transcription rate for the sequence (forward) is " + str(def_fwd_max_tx_rate))
     if len(res_final_df_max_fwd_df) > 1:
         max_fwd_output_file = OUTPUT_FILE_NAME + "_MAX_FWD_results.csv"
         if float(new_max_fwd_Tx_rate) > float(def_fwd_max_tx_rate):
             print ("can be increased up to " + str(new_max_fwd_Tx_rate))
             print("using the promoters in the " + max_fwd_output_file)
             res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list)
             ##files.download(max_fwd_output_file)
 
     else:
         print(" cannot be further increased")
     print("\n")
-    print("The maximum transcription rate for the sequence (reverse) " + str(def_rev_max_tx_rate))
+    print("The maximum transcription rate for the sequence (reverse) is " + str(def_rev_max_tx_rate))
     if len(res_final_df_max_rev_df) > 1:
         max_rev_output_file = OUTPUT_FILE_NAME + "_MAX_REV_results.csv"
         if float(new_max_rev_Tx_rate) > float(def_rev_max_tx_rate):
             print ("can be increased up to " + str(new_max_rev_Tx_rate))
             print("using the promoters in the " + max_rev_output_file)
             res_final_df_max_fwd_df.to_csv(max_rev_output_file, columns = column_list)
             ##files.download(max_rev_output_file)
```

### Comparing `pssm-promoter-tool-1.0.0/setup.py` & `pssm-promoter-tool-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pssm-promoter-tool',
-      version='1.0.0',
+      version='1.0.1',
       description='The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ellinium/PSSM_PromoterTool',
       author='Ellina Trofimova',
       author_email='ellina.trofimova@gmail.com',
       license='GNU General Public License',
```


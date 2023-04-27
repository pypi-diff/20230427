# Comparing `tmp/str_analysis-0.9.7.tar.gz` & `tmp/str_analysis-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/str_analysis-0.9.7.tar", last modified: Tue May 17 05:14:49 2022, max compression
+gzip compressed data, was "dist/str_analysis-0.9.8.tar", last modified: Tue Oct 18 03:27:04 2022, max compression
```

## Comparing `str_analysis-0.9.7.tar` & `str_analysis-0.9.8.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-05-17 05:14:49.000000 str_analysis-0.9.7/
--rw-r--r--   0 root         (0) staff       (20)    20624 2022-05-17 05:14:49.000000 str_analysis-0.9.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    17525 2022-01-21 17:46:01.000000 str_analysis-0.9.7/README.md
--rw-r--r--   0 root         (0) staff       (20)     6350 2022-01-21 01:49:15.000000 str_analysis-0.9.7/README.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2022-05-17 05:14:49.000000 str_analysis-0.9.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2897 2022-05-17 05:13:35.000000 str_analysis-0.9.7/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis/
--rw-r--r--   0 root         (0) staff       (20)        0 2021-08-15 22:19:51.000000 str_analysis-0.9.7/str_analysis/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    56915 2022-01-21 14:15:11.000000 str_analysis-0.9.7/str_analysis/call_non_ref_pathogenic_motifs.py
--rw-r--r--   0 root         (0) staff       (20)    18338 2022-04-25 05:51:26.000000 str_analysis-0.9.7/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
--rwxr-xr-x   0 root         (0) staff       (20)    19745 2022-01-10 02:40:22.000000 str_analysis-0.9.7/str_analysis/check_trios_for_mendelian_violations.py
--rw-r--r--   0 root         (0) staff       (20)     1627 2021-10-21 15:05:22.000000 str_analysis-0.9.7/str_analysis/check_trios_for_mendelian_violations_tests.py
--rwxr-xr-x   0 root         (0) staff       (20)    19735 2022-01-04 00:49:53.000000 str_analysis-0.9.7/str_analysis/combine_expansion_hunter_json_to_tsv.py
--rw-r--r--   0 root         (0) staff       (20)    12147 2022-01-04 00:50:03.000000 str_analysis-0.9.7/str_analysis/combine_expansion_hunter_json_to_tsv_tests.py
--rwxr-xr-x   0 root         (0) staff       (20)     9144 2021-10-21 15:05:22.000000 str_analysis-0.9.7/str_analysis/combine_json_to_tsv.py
--rw-r--r--   0 root         (0) staff       (20)     2855 2022-01-04 00:49:53.000000 str_analysis-0.9.7/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
--rw-r--r--   0 root         (0) staff       (20)     3623 2022-02-08 18:43:09.000000 str_analysis-0.9.7/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
--rw-r--r--   0 root         (0) staff       (20)     7787 2022-01-09 18:15:07.000000 str_analysis-0.9.7/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
--rw-r--r--   0 root         (0) staff       (20)     6195 2022-01-11 03:40:51.000000 str_analysis-0.9.7/str_analysis/convert_strling_calls_to_expansion_hunter_json.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis/data/
--rw-r--r--   0 root         (0) staff       (20)     2203 2022-01-04 00:49:06.000000 str_analysis-0.9.7/str_analysis/data/non_ref_motif.locus_info.json
--rw-r--r--   0 root         (0) staff       (20)    31832 2021-08-20 15:25:44.000000 str_analysis-0.9.7/str_analysis/data/non_ref_motif.offtarget_regions.json.gz
--rw-r--r--   0 root         (0) staff       (20)    13552 2022-05-16 04:46:12.000000 str_analysis-0.9.7/str_analysis/filter_vcf_to_STR_variants.py
--rw-r--r--   0 root         (0) staff       (20)     3044 2022-05-11 21:34:59.000000 str_analysis-0.9.7/str_analysis/filter_vcf_to_STR_variants_tests.py
--rw-r--r--   0 root         (0) staff       (20)    61685 2022-02-16 19:29:27.000000 str_analysis-0.9.7/str_analysis/generate_gnomad_json.py
--rw-r--r--   0 root         (0) staff       (20)      915 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/generate_gnomad_json_tests.py
--rw-r--r--   0 root         (0) staff       (20)    21388 2021-10-21 15:05:22.000000 str_analysis-0.9.7/str_analysis/simulate_str_expansions.py
--rw-r--r--   0 root         (0) staff       (20)     1492 2021-10-21 15:05:22.000000 str_analysis-0.9.7/str_analysis/simulate_str_expansions_tests.py
--rw-r--r--   0 root         (0) staff       (20)     3614 2022-01-11 03:43:11.000000 str_analysis-0.9.7/str_analysis/trim_repeat_loci.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis/utils/
--rw-r--r--   0 root         (0) staff       (20)        0 2021-08-15 19:10:09.000000 str_analysis-0.9.7/str_analysis/utils/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7133 2021-10-21 15:05:22.000000 str_analysis-0.9.7/str_analysis/utils/bam_utils.py
--rw-r--r--   0 root         (0) staff       (20)     2147 2022-05-15 19:58:41.000000 str_analysis-0.9.7/str_analysis/utils/canonical_repeat_unit.py
--rw-r--r--   0 root         (0) staff       (20)     1757 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/utils/canonical_repeat_unit_tests.py
--rw-r--r--   0 root         (0) staff       (20)     4925 2021-12-09 03:44:25.000000 str_analysis-0.9.7/str_analysis/utils/ehdn_info_for_locus.py
--rw-r--r--   0 root         (0) staff       (20)     1157 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/utils/export_json.py
--rw-r--r--   0 root         (0) staff       (20)     1221 2021-08-25 16:27:04.000000 str_analysis-0.9.7/str_analysis/utils/fasta_utils.py
--rw-r--r--   0 root         (0) staff       (20)      492 2022-05-06 00:56:11.000000 str_analysis-0.9.7/str_analysis/utils/find_repeat_unit.py
--rw-r--r--   0 root         (0) staff       (20)      943 2022-05-06 02:30:34.000000 str_analysis-0.9.7/str_analysis/utils/find_repeat_unit_tests.py
--rw-r--r--   0 root         (0) staff       (20)     4796 2022-01-20 19:56:03.000000 str_analysis-0.9.7/str_analysis/utils/known_pathogenic_strs_tsv.py
--rw-r--r--   0 root         (0) staff       (20)     2276 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/utils/misc_utils.py
--rw-r--r--   0 root         (0) staff       (20)     1866 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/utils/most_frequent_repeat_unit.py
--rw-r--r--   0 root         (0) staff       (20)     1239 2021-11-19 17:05:07.000000 str_analysis-0.9.7/str_analysis/utils/most_frequent_repeat_unit_tests.py
--rw-r--r--   0 root         (0) staff       (20)     1628 2022-01-09 18:02:32.000000 str_analysis-0.9.7/str_analysis/utils/strling_info_for_locus.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    20624 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1891 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      323 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       77 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2022-05-17 05:14:49.000000 str_analysis-0.9.7/str_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/
+-rw-r--r--   0 weisburd   (502) staff       (20)    20624 2022-10-18 03:27:04.000000 str_analysis-0.9.8/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)    17525 2022-01-21 17:46:01.000000 str_analysis-0.9.8/README.md
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2022-10-18 03:27:04.000000 str_analysis-0.9.8/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     2871 2022-10-18 03:25:56.000000 str_analysis-0.9.8/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 22:19:51.000000 str_analysis-0.9.8/str_analysis/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    56915 2022-01-21 14:15:11.000000 str_analysis-0.9.8/str_analysis/call_non_ref_pathogenic_motifs.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    18286 2022-06-21 13:30:13.000000 str_analysis-0.9.8/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)    19732 2022-06-21 13:30:13.000000 str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1627 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations_tests.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)     9144 2022-10-10 22:03:14.000000 str_analysis-0.9.8/str_analysis/combine_json_to_tsv.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)    22723 2022-10-09 22:08:17.000000 str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    12146 2022-06-21 13:31:54.000000 str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2855 2022-01-04 00:49:53.000000 str_analysis-0.9.8/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     3623 2022-02-08 18:43:09.000000 str_analysis-0.9.8/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     9148 2022-06-20 04:10:53.000000 str_analysis-0.9.8/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     6195 2022-01-11 03:40:51.000000 str_analysis-0.9.8/str_analysis/convert_strling_calls_to_expansion_hunter_json.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/data/
+-rw-r--r--   0 weisburd   (502) staff       (20)     2203 2022-01-04 00:49:06.000000 str_analysis-0.9.8/str_analysis/data/non_ref_motif.locus_info.json
+-rw-r--r--   0 weisburd   (502) staff       (20)    31832 2021-08-20 15:25:44.000000 str_analysis-0.9.8/str_analysis/data/non_ref_motif.offtarget_regions.json.gz
+-rw-r--r--   0 weisburd   (502) staff       (20)    24794 2022-06-21 16:43:40.000000 str_analysis-0.9.8/str_analysis/filter_vcf_to_STR_variants.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    16239 2022-06-21 14:11:35.000000 str_analysis-0.9.8/str_analysis/filter_vcf_to_STR_variants_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    61985 2022-07-11 14:21:21.000000 str_analysis-0.9.8/str_analysis/generate_gnomad_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      915 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/generate_gnomad_json_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    21388 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/simulate_str_expansions.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1492 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/simulate_str_expansions_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     3614 2022-01-11 03:43:11.000000 str_analysis-0.9.8/str_analysis/trim_repeat_loci.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/utils/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 19:10:09.000000 str_analysis-0.9.8/str_analysis/utils/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     7133 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/utils/bam_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2147 2022-05-15 19:58:41.000000 str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1757 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4223 2019-07-28 15:41:24.000000 str_analysis-0.9.8/str_analysis/utils/dat_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4925 2021-12-09 03:44:25.000000 str_analysis-0.9.8/str_analysis/utils/ehdn_info_for_locus.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1157 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/export_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1221 2021-08-25 16:27:04.000000 str_analysis-0.9.8/str_analysis/utils/fasta_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2669 2022-06-13 01:13:43.000000 str_analysis-0.9.8/str_analysis/utils/find_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      952 2022-06-12 05:38:06.000000 str_analysis-0.9.8/str_analysis/utils/find_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4796 2022-01-20 19:56:03.000000 str_analysis-0.9.8/str_analysis/utils/known_pathogenic_strs_tsv.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2267 2022-06-12 13:37:10.000000 str_analysis-0.9.8/str_analysis/utils/misc_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1866 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1239 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1628 2022-01-09 18:02:32.000000 str_analysis-0.9.8/str_analysis/utils/strling_info_for_locus.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4036 2022-06-08 20:53:36.000000 str_analysis-0.9.8/str_analysis/utils/trf_runner.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)    20624 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     1919 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      297 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       77 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       13 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/top_level.txt
```

### Comparing `str_analysis-0.9.7/PKG-INFO` & `str_analysis-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: str_analysis
-Version: 0.9.7
+Version: 0.9.8
 Summary: Utilities  short tandem repeats (STRs)
 Home-page: https://github.com/broadinstitute/str-analysis
 License: MIT
 Description: # str-analysis
         ---
         This package contains scripts and utilities for analyzing short tandem repeats (STRs).
```

### Comparing `str_analysis-0.9.7/README.md` & `str_analysis-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/setup.py` & `str_analysis-0.9.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,26 @@
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('str_analysis', pattern='*tests.py')
     return test_suite
 
 
 setup(
     name='str_analysis',
-    version="0.9.7",
+    version="0.9.8",
     description="Utilities  short tandem repeats (STRs)",
     install_requires=requirements,
     cmdclass={
         'coverage': CoverageCommand,
         'publish': PublishCommand,
     },
     entry_points = {
         'console_scripts': [
             'call_non_ref_pathogenic_motifs = str_analysis.call_non_ref_pathogenic_motifs:main',
             'combine_json_to_tsv = str_analysis.combine_json_to_tsv:main',
-            'combine_expansion_hunter_json_to_tsv = str_analysis.combine_expansion_hunter_json_to_tsv:main',
+            'combine_str_json_to_tsv = str_analysis.combine_str_json_to_tsv:main',
             'simulate_str_expansions = str_analysis.simulate_str_expansions:main',
         ],
     },
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=["str_analysis", "str_analysis.utils"],
     data_files=[
```

### Comparing `str_analysis-0.9.7/str_analysis/call_non_ref_pathogenic_motifs.py` & `str_analysis-0.9.8/str_analysis/call_non_ref_pathogenic_motifs.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py` & `str_analysis-0.9.8/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This script makes it easier to manually look through genotypes of many samples at known pathogenic loci and
 check for samples that may be expanded into the pathogenic range.
 
-The script's main input file is a .tsv file generated by the combine_expansion_hunter_json_to_tsv.py script which
+The script's main input file is a .tsv file generated by the combine_str_json_to_tsv.py script which
 combines multiple ExpansionHunter .json output files into a single .tsv table. It's assumed that this input .tsv will
 have at least the columns listed below. One way to add these Sample_* and VariantCatalog_* columns is to run
-combine_expansion_hunter_json_to_tsv.py with the --sample-metadata and the --variant-catalog args.
+combine_str_json_to_tsv.py with the --sample-metadata and the --variant-catalog args.
 
 The input .tsv must have at least these input columns:
 
     "LocusId", "SampleId", "Sample_affected", "Sample_sex",
     "Num Repeats: Allele 1", "Num Repeats: Allele 2", "CI end: Allele 1", "CI end: Allele 2",
 
 """
@@ -74,15 +74,15 @@
         "that have smaller expansions at that locus will be ignored")
     p.add_argument("--use-gnomad", action="store_true", help="Include samples from the gnomAD v3.1 STR release"
         "@ https://gnomad.broadinstitute.org/downloads#v3-short-tandem-repeats")
     p.add_argument("-l", "--locus", action="append", help="If specified, only these locus ids will be processed")
     p.add_argument("--highlight-samples", nargs="*", help="If specified, this can be the path of a text file that "
         "contains sample ids (one per line) or just 1 or more sample ids listed on the commandline - one per line")
     p.add_argument("combined_tsv_path", nargs="+", help="Path of combined ExpansionHunter .tsv table generated by the "
-        "combine_expansion_hunter_json_to_tsv.py script. It's assumed that combine_expansion_hunter_json_to_tsv.py "
+        "combine_str_json_to_tsv.py script. It's assumed that combine_str_json_to_tsv.py "
         "was run with --sample-metadata and --variant-catalog args to add sample-level and locus-level metadata columns")
 
     # Parse and validate command-line args + read in the combined table(s) from the given command_tsv_path(s)
     args = p.parse_args()
 
     if args.use_gnomad:
         print("Loading gnomAD STR table...")
```

### Comparing `str_analysis-0.9.7/str_analysis/check_trios_for_mendelian_violations.py` & `str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             logging.info(f"ERROR: duplicate key: {idx}")
             logging.info(row)
 
         raise ValueError(f"Found {num_duplicate_keys} duplicate keys in {file_path}")
 
 
 def parse_combined_str_calls_tsv_path(combined_str_calls_tsv_path):
-    """Parse a tsv table generated by combine_expansion_hunter_json_to_tsv.py, check for duplicates that have the same
+    """Parse a tsv table generated by combine_str_json_to_tsv.py, check for duplicates that have the same
     ("SampleId", "LocusId", "VariantId") and then return the table as a pandas DataFrame.
 
     Raises:
         ValueError: if it finds duplicates by ("SampleId", "LocusId", "VariantId")
     """
 
     combined_str_calls_df = pd.read_table(combined_str_calls_tsv_path)
```

### Comparing `str_analysis-0.9.7/str_analysis/check_trios_for_mendelian_violations_tests.py` & `str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/combine_expansion_hunter_json_to_tsv.py` & `str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,23 @@
     p.add_argument(
         "--sample-metadata-key",
         help="The column name in the --sample-metdata table that contains a sample id. "
              "If not specified, 'sample_id' and other variations like 'SampleId', 'sample', and 'ParticipantId' "
              "will be tried."
     )
     p.add_argument(
-        "--include-all-fields",
+        "--include-extra-expansion-hunter-fields",
         action="store_true",
-        help="If specified, all fields from the ExpansionHunter will be added."
+        help="If specified, additional fields from the ExpansionHunter will be added."
+    )
+    p.add_argument(
+        "--include-extra-gangstr-fields",
+        action="store_true",
+        help="If specified, additional fields from GangSTR will be added. The input json files are expected to be the "
+             "result of running convert_gangstr_vcf_to_expansion_hunter_json."
     )
 
     p.add_argument(
         "-o",
         "--output-prefix",
         help="Combined table output filename prefix",
     )
@@ -95,15 +101,15 @@
         #for d in variant_catalog_contents:
         #    logging.info("    " + d["LocusId"])
 
     sample_metadata_lookup = collections.defaultdict(list)
     if args.sample_metadata:
         sample_metadata_df = pd.read_table(args.sample_metadata)
         sample_id_column_idx = get_sample_id_column_index(sample_metadata_df, column_name=args.sample_metadata_key)
-        if sample_id_column_idx is -1:
+        if sample_id_column_idx == -1:
             raise ValueError(f"'sample_id' column not found in sample metadata table. The columns found were: {sample_metadata_df.columns}")
         sample_id_column = sample_metadata_df.columns[sample_id_column_idx]
         for _, row in sample_metadata_df.iterrows():
             if args.verbose and len(sample_metadata_lookup[row[sample_id_column]]) > 0:
                 logging.info(f"  {row[sample_id_column]} is a duplicate sample id in {args.sample_metadata}")
             sample_metadata_lookup[row[sample_id_column]].append(row)
         logging.info(f"Parsed {len(sample_metadata_df)} rows from {args.sample_metadata}")
@@ -136,15 +142,16 @@
             for record in convert_expansion_hunter_json_to_tsv_columns(
                 json_contents,
                 variant_catalog_contents=combined_variant_catalog_contents,
                 sample_metadata_lookup=sample_metadata_lookup,
                 sample_metadata_lookup_counters=sample_metadata_lookup_counters,
                 json_file_path=json_path,
                 return_allele_records=False,
-                include_all_fields=args.include_all_fields,
+                include_extra_expansion_hunter_fields=args.include_extra_expansion_hunter_fields,
+                include_extra_gangstr_fields=args.include_extra_gangstr_fields,
             ):
                 if just_get_header:
                     variant_table_columns.extend([k for k in record.keys() if k not in variant_table_columns])
                 else:
                     if not wrote_variant_table_header:
                         variant_output_file.write("\t".join(variant_table_columns) + "\n")
                         wrote_variant_table_header = True
@@ -153,15 +160,16 @@
 
             for record in convert_expansion_hunter_json_to_tsv_columns(
                 json_contents,
                 variant_catalog_contents=combined_variant_catalog_contents,
                 sample_metadata_lookup=sample_metadata_lookup,
                 json_file_path=json_path,
                 return_allele_records=True,
-                include_all_fields=args.include_all_fields,
+                include_extra_expansion_hunter_fields=args.include_extra_expansion_hunter_fields,
+                include_extra_gangstr_fields=args.include_extra_gangstr_fields,
             ):
                 if just_get_header:
                     allele_table_columns.extend([k for k in record.keys() if k not in allele_table_columns])
                 else:
                     if not wrote_allele_table_header:
                         allele_output_file.write("\t".join(allele_table_columns) + "\n")
                         wrote_allele_table_header = True
@@ -225,30 +233,32 @@
     json_contents,
     variant_catalog_contents=None,
     sample_metadata_lookup=None,
     sample_metadata_lookup_counters=None,
     variant_info=None,
     json_file_path="",
     return_allele_records=True,
-    include_all_fields=False,
+    include_extra_expansion_hunter_fields=False,
+    include_extra_gangstr_fields=False,
 ):
     """Converts a dictionary that represents the contents of an ExpansionHunter v3 or v4 json output file to
     a dictionary of tsv column values.
 
     Args:
         json_contents (dict): a dict with the contents of an ExpansionHunter v3 or v4 json output file
         variant_catalog_contents (dict): optional dict with the contents of the variant catalog used when running
             expansion hunter. If provided, the fields will be added to the output table.
         sample_metadata_lookup (dict): maps sample id to row of sample metadata
         sample_metadata_lookup_counters (dict): dictionary for accumulating counters and stats about the
             ability to find samples in sample_metadata_lookup
         variant_info (dict): if provided, results will be added to this dict. Otherwise, a new dict will be created.
         json_file_path (str): if provided, it will be added as a field to the output table, and also used for logging
         return_allele_records (bool): if True, the returned list will have one record per allele rather than per variant
-        include_all_fields (bool): if True, include all fields in the returned records, not just the basic ones.
+        include_extra_expansion_hunter_fields (bool): if True, include additional fields provided by ExpansionHunter.
+        include_extra_gangstr_fields (bool): if True, include additional fields provided by GangSTR.
 
     Returns:
         list: a list of tsv rows
     """
 
     if variant_info is None:
         variant_info = collections.OrderedDict()
@@ -328,32 +338,46 @@
             variant_record = collections.OrderedDict(locus_record)
             variant_record["VariantId"] = variant_json.get("VariantId", "")
             variant_record["VariantSubtype"] = variant_json.get("VariantSubtype", "")
             variant_record["RepeatUnit"] = variant_json["RepeatUnit"]
             variant_record["RepeatUnitLength"] = len(variant_json["RepeatUnit"])
             variant_record["ReferenceRegion"] = variant_json["ReferenceRegion"]
 
-            if include_all_fields:
+            if include_extra_expansion_hunter_fields:
                 variant_record["CountsOfSpanningReads"] = variant_json["CountsOfSpanningReads"]
                 variant_record["CountsOfFlankingReads"] = variant_json["CountsOfFlankingReads"]
                 variant_record["CountsOfInrepeatReads"] = variant_json["CountsOfInrepeatReads"]
 
                 spanning_read_tuples = parse_read_count_tuples(variant_json["CountsOfSpanningReads"])
                 flanking_read_tuples = parse_read_count_tuples(variant_json["CountsOfFlankingReads"])
                 inrepeat_read_tuples = parse_read_count_tuples(variant_json["CountsOfInrepeatReads"])
 
                 variant_record["NumSpanningReads"] = sum(t[1] for t in spanning_read_tuples)
                 variant_record["NumFlankingReads"] = sum(t[1] for t in flanking_read_tuples)
                 variant_record["NumInrepeatReads"] = sum(t[1] for t in inrepeat_read_tuples)
-                variant_record["NumReadsTotal"] = sum([variant_record[k] for k in ("NumSpanningReads", "NumFlankingReads", "NumInrepeatReads")])
+                variant_record["NumReadsTotal"] = sum([variant_record[k] for k in (
+                    "NumSpanningReads", "NumFlankingReads", "NumInrepeatReads")])
 
                 variant_record["NumAllelesSupportedBySpanningReads"] = len(spanning_read_tuples)
                 variant_record["NumAllelesSupportedByFlankingReads"] = len(flanking_read_tuples)
                 variant_record["NumAllelesSupportedByInrepeatReads"] = len(inrepeat_read_tuples)
-                variant_record["NumAllelesSupportedTotal"] = sum([variant_record[k] for k in ("NumAllelesSupportedBySpanningReads", "NumAllelesSupportedByFlankingReads", "NumAllelesSupportedByInrepeatReads")])
+                variant_record["NumAllelesSupportedTotal"] = sum([variant_record[k] for k in (
+                    "NumAllelesSupportedBySpanningReads", "NumAllelesSupportedByFlankingReads", "NumAllelesSupportedByInrepeatReads")])
+
+            if include_extra_gangstr_fields:
+                variant_record["RC"] = variant_json["RC"]
+                variant_record["ENCLREADS"] = variant_json["ENCLREADS"]
+                variant_record["FLNKREADS"] = variant_json["FLNKREADS"]
+                enclosing, spanning, FRR, flanking = variant_json["RC"].split(",")
+                variant_record["NumSpanningReads"] = int(enclosing)
+                variant_record["NumFlankingReads"] = int(flanking)  # + int(spanning)
+                variant_record["NumInrepeatReads"] = int(FRR)
+                variant_record["NumReadsTotal"] = sum([variant_record[k] for k in (
+                    "NumSpanningReads", "NumFlankingReads", "NumInrepeatReads")])
+                variant_record["Q"] = float(variant_json["Q"])
 
             variant_record["Genotype"] = variant_json["Genotype"]
             variant_record["GenotypeConfidenceInterval"] = variant_json["GenotypeConfidenceInterval"]
             genotype_tuples = list(zip(
                 variant_json["Genotype"].split("/"),
                 variant_json["GenotypeConfidenceInterval"].split("/"),
             ))
@@ -369,30 +393,47 @@
                 confidence_interval_start, confidence_interval_end = genotypeCI.split("-")
                 allele_record[f"Allele Number{suffix}"] = i + 1
                 allele_record[f"Num Repeats{suffix}"] = int(genotype)
                 allele_record[f"Repeat Size (bp){suffix}"] = int(genotype) * len(variant_json.get("RepeatUnit", ""))
                 allele_record[f"CI start{suffix}"] = int(confidence_interval_start)
                 allele_record[f"CI end{suffix}"] = int(confidence_interval_end)
                 allele_record[f"CI size{suffix}"] = int(confidence_interval_end) - int(confidence_interval_start)
+                allele_record[f"CI ratio{suffix}"] = allele_record[f"CI size{suffix}"]/(allele_record[f"Num Repeats{suffix}"] or 1)
 
-                if include_all_fields:
+                if include_extra_expansion_hunter_fields:
                     is_homozygous = len(genotype_tuples) > 1 and genotype_tuples[0][0] == genotype_tuples[1][0]
                     divisor = 2 if is_homozygous else 1
                     allele_record[f"NumSpanningReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in spanning_read_tuples if t[0] == int(genotype)) / divisor
                     allele_record[f"NumFlankingReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in flanking_read_tuples if t[0] == int(genotype)) / divisor
                     allele_record[f"NumInrepeatReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in inrepeat_read_tuples if t[0] == int(genotype)) / divisor
                     allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
                         allele_record[f"NumSpanningReadsThatSupportGenotype{suffix}"] +
                         allele_record[f"NumFlankingReadsThatSupportGenotype{suffix}"] +
                         allele_record[f"NumInrepeatReadsThatSupportGenotype{suffix}"]
                     )
                     allele_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
                         allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(allele_record["NumReadsTotal"]) if int(allele_record["NumReadsTotal"]) > 0 else 0
                     )
+                if include_extra_gangstr_fields:
+                    # ex. "2,10|3,7|4,14"
+                    for source_field, dest_field in [("ENCLREADS", f"NumSpanningReadsThatSupportGenotype{suffix}"),
+                                                     ("FLNKREADS", f"NumFlankingReadsThatSupportGenotype{suffix}")]:
+                        if variant_json[source_field] != "NULL":
+                            read_support = dict([key_value.split(",") for key_value in variant_json[source_field].split("|")])
+                            allele_record[dest_field] = int(read_support.get(genotype, 0))
+                        else:
+                            allele_record[dest_field] = 0
 
+                    allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
+                            allele_record.get(f"NumSpanningReadsThatSupportGenotype{suffix}", 0) +
+                            allele_record.get(f"NumFlankingReadsThatSupportGenotype{suffix}", 0)
+                    )
+                    allele_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
+                        allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(allele_record["NumReadsTotal"]) if int(allele_record["NumReadsTotal"]) > 0 else 0
+                    )
                 if return_allele_records:
                     records_to_return.append(allele_record)
 
             if not return_allele_records:
                 records_to_return.append(allele_record)
 
     return records_to_return
```

### Comparing `str_analysis-0.9.7/str_analysis/combine_expansion_hunter_json_to_tsv_tests.py` & `str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import unittest
 
-from combine_expansion_hunter_json_to_tsv import (
-    convert_expansion_hunter_json_to_tsv_columns, parse_read_count_tuples)
+from combine_str_json_to_tsv import convert_expansion_hunter_json_to_tsv_columns, parse_read_count_tuples
 
 VARIANT_CATALOG_CONTENTS = json.loads("""[{
   "LocusId": "X-149631736-149631780-TMEM185A",
   "LocusStructure": "(CGC)*",
   "ReferenceRegion": "chrX:149631735-149631780",
   "VariantType": "Repeat",
   "IsOfficial": false,
@@ -212,15 +211,15 @@
 
     def test_convert_expansion_hunter_json_to_tsv_columns_for_variants(self):
         variant_rows = convert_expansion_hunter_json_to_tsv_columns(
             EHv4_JSON,
             variant_catalog_contents=VARIANT_CATALOG_CONTENTS,
             json_file_path="",
             return_allele_records=False,
-            include_all_fields=True,
+            include_extra_expansion_hunter_fields=True,
         )
         self.assertEqual(len(variant_rows), 4)
         for row in variant_rows:
             self.assertIn('InVariantCatalog', row)
             self.assertIn('AlleleCount', row)
             self.assertListEqual(list(row.keys()), get_expected_columns(row, with_allele_records=False, with_json_file_path=False))
```

### Comparing `str_analysis-0.9.7/str_analysis/combine_json_to_tsv.py` & `str_analysis-0.9.8/str_analysis/combine_json_to_tsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,19 +166,19 @@
         sample_metadata_df_sample_id_column (str): Name of the column in sample_metadata_df that should be used as the join key.
         verbose (bool): Whether to print additional log statements.
 
     Return:
         pandas.DataFrame: The DataFrame resulting from a LEFT join between df and sample_metadata_df
     """
     sample_id_column_idx1 = get_sample_id_column_index(df, column_name=df_sample_id_columns)
-    if sample_id_column_idx1 is -1:
+    if sample_id_column_idx1 == -1:
         raise ValueError(f"'sample_id' field not found in json files. The fields found were: {df.columns}")
 
     sample_id_column_idx2 = get_sample_id_column_index(sample_metadata_df, column_name=sample_metadata_df_sample_id_column)
-    if sample_id_column_idx2 is -1:
+    if sample_id_column_idx2 == -1:
         raise ValueError(f"'sample_id' column not found in sample metadata table. The columns found were: {sample_metadata_df.columns}")
 
     sample_id_column1 = df.columns[sample_id_column_idx1]
     sample_id_column2 = sample_metadata_df.columns[sample_id_column_idx2]
     print(f"Doing a LEFT JOIN with sample metadata table using keys {sample_id_column1} and {sample_id_column2}")
 
     set1 = set(df[sample_id_column1])
```

### Comparing `str_analysis-0.9.7/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py` & `str_analysis-0.9.8/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py` & `str_analysis-0.9.8/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py` & `str_analysis-0.9.8/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -140,14 +140,29 @@
             start_1based = int(fields[1])
             ref = fields[3]
             alts = fields[4].split(",")
             info = fields[7]
             if not fields[9] or fields[9] == ".":  # no genotype
                 continue
 
+            # example1: chr8	141029449	.	gtggtggtg	.	.	.
+            #    END=141029457;RU=gtg;PERIOD=3;REF=3;GRID=1,6;STUTTERUP=0.05;STUTTERDOWN=0.05;STUTTERP=0.9;EXPTHRESH=-1
+            #    GT:DP:Q:REPCN:REPCI:RC:ENCLREADS:FLNKREADS:ML:INS:STDERR:QEXP
+            #    0/0:47:1:3,3:3-3,3-3:38,9,0,0:3,38:NULL:232.623:342,114:0,0:-1,-1,-1
+            #
+            # example2: chr8	140697417	.	tgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtg	tgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtg	.	.
+            #   END=140697454;RU=tg;PERIOD=2;REF=19;GRID=13,23;STUTTERUP=0.05;STUTTERDOWN=0.05;STUTTERP=0.9;EXPTHRESH=-1
+            #   GT:DP:Q:REPCN:REPCI:RC:ENCLREADS:FLNKREADS:ML:INS:STDERR:QEXP
+            #   0/1:41:0.999999:19,20:19-19,19-20:24,7,0,9:19,14|20,10:6,1|8,1|9,2|11,1|13,1|14,1|15,1|17,1:247.512:342,114:0.29703,0.564617:-1,-1,-1
+            #
+            # example3: chr8	140594826	.	tgtgtgtgtgtgtgtgtgtgtgtgtgtg	tgtgtgtgtgtgtgtgtgtgtgtgtgtgtg,tgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtgtg	.	.
+            #   END=140594853;RU=tg;PERIOD=2;REF=14;GRID=12,26;STUTTERUP=0.05;STUTTERDOWN=0.05;STUTTERP=0.9;EXPTHRESH=-1
+            #   GT:DP:Q:REPCN:REPCI:RC:ENCLREADS:FLNKREADS:ML:INS:STDERR:QEXP
+            #   1/2:36:0.994974:15,23:15-15,20-23:21,7,0,8:15,19|23,2:5,1|8,1|9,1|10,1|11,1|14,1|20,2:227.086:342,114:0,1.56141:-1,-1,-1
+
             info_dict = dict([key_value.split("=") for key_value in info.split(";")])
             genotype_fields = fields[8].split(":")
             genotype_values = fields[9].split(":")
             genotype_dict = dict(zip(genotype_fields, genotype_values))
 
             try:
                 repeat_unit = info_dict["RU"].upper()
@@ -164,15 +179,15 @@
                 locus_results["LocusResults"][locus_id] = {
                     "AlleleCount": genotype_dict["REPCN"].count(",") + 1,
                     "LocusId": locus_id,
                     "Coverage": float(genotype_dict["DP"]),  #10.757737459978655,
                     "ReadLength": None,
                     "FragmentLength": None,
                     "Variants": {
-                        locus_id: {
+                        locus_id: info_dict | genotype_dict | {
                             "Genotype": genotype_dict["REPCN"].replace(",", "/"), #"17/17",
                             "GenotypeConfidenceInterval": genotype_dict["REPCI"].replace(",", "/"), #"17-17/17-17",
                             "ReferenceRegion": f"{chrom}:{start_1based - 1}-{end_1based}",
                             "RepeatUnit": repeat_unit,
                             "VariantId": variant_id,
                             "VariantSubtype": "Repeat",
                             "VariantType": "Repeat",
```

### Comparing `str_analysis-0.9.7/str_analysis/convert_strling_calls_to_expansion_hunter_json.py` & `str_analysis-0.9.8/str_analysis/convert_strling_calls_to_expansion_hunter_json.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/data/non_ref_motif.locus_info.json` & `str_analysis-0.9.8/str_analysis/data/non_ref_motif.locus_info.json`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/data/non_ref_motif.offtarget_regions.json.gz` & `str_analysis-0.9.8/str_analysis/data/non_ref_motif.offtarget_regions.json.gz`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/generate_gnomad_json.py` & `str_analysis-0.9.8/str_analysis/generate_gnomad_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     'NOTCH2NLC': 'ENSG00000286219',
     'PABPN1': 'ENSG00000100836',
     'PHOX2B': 'ENSG00000109132',
     'PPP2R2B': 'ENSG00000156475',
     'PRDM12': 'ENSG00000130711',
     'PRNP': 'ENSG00000171867',
     'RAPGEF2': 'ENSG00000109756',
+    'RILPL1': 'ENSG00000188026',
     'RFC1': 'ENSG00000035928',
     'RUNX2': 'ENSG00000124813',
     'SAMD12': 'ENSG00000177570',
     'SOX3': 'ENSG00000134595',
     'STARD7': 'ENSG00000084090',
     'TBP': 'ENSG00000112592',
     'TBX1': 'ENSG00000184058',
@@ -187,14 +188,17 @@
     'VWA1': 'ENSG00000179403',
     'XYLT1': 'ENSG00000103489',
     'YEATS2': 'ENSG00000163872',
     'ZIC2': 'ENSG00000043355',
     'ZIC3': 'ENSG00000156925',
 }
 
+# Discard samples with read length below the MIN_READ_LENGTH threshold (in base pairs)
+MIN_READ_LENGTH = 150
+
 # Round ages to the nearest N years so that they can be shared publicly without increasing identifiability
 AGE_RANGE_SIZE = 5
 
 # Truncate the age distribution at this lower and upper bound.
 LOWER_AGE_CUTOFF = 20
 UPPER_AGE_CUTOFF = 80
 
@@ -218,15 +222,15 @@
 # Fraction of samples that can be missing age information before generating an error
 MISSING_AGE_THRESHOLD = 0.5
 
 # Fraction of samples that can be pcr-free/pcr-plus information before generating an error
 MISSING_PCR_PROTOCOL_THRESHOLD = 0.25
 
 # Expected number of known pathogenic repeats
-EXPECTED_N_KNOWN_PATHOGENIC_REPEATS = 59
+EXPECTED_N_KNOWN_PATHOGENIC_REPEATS = 60
 
 # Add this "salt" value to the sha512 hash to prevent dictionary attacks on the encrypted sample ids
 salt = pwd.getpwuid(os.getuid()).pw_name
 
 
 def parse_args():
     """Parse command-line args, perform basic validation, and then return the args object."""
@@ -435,14 +439,17 @@
               f"were not found in the gnomAD metadata table, or were found but are not 'release': ", unknown_sample_ids)
 
     # Merge the data frames
     print(f"Combining STR data tables with gnomAD metadata")
     df = pd.merge(left=df, right=gnomad_df, how="inner", left_on="SampleId", right_on="s").drop(columns="s")
 
     print(f"Found {len(set(df.SampleId))} gnomAD 'release' samples")
+    df = df[df.read_length >= MIN_READ_LENGTH]
+    print(f"Kept {len(set(df.SampleId))} gnomAD samples after filtering to ReadLength >= {MIN_READ_LENGTH}")
+
     locus_id_with_max_samples = None
     max_num_samples = 0
     for locus_id in sorted(set(df.LocusId)):
         num_samples = len(set(df[df.LocusId == locus_id].SampleId))
         if num_samples > max_num_samples:
             locus_id_with_max_samples = locus_id
             max_num_samples = num_samples
```

### Comparing `str_analysis-0.9.7/str_analysis/generate_gnomad_json_tests.py` & `str_analysis-0.9.8/str_analysis/generate_gnomad_json_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/simulate_str_expansions.py` & `str_analysis-0.9.8/str_analysis/simulate_str_expansions.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/simulate_str_expansions_tests.py` & `str_analysis-0.9.8/str_analysis/simulate_str_expansions_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/trim_repeat_loci.py` & `str_analysis-0.9.8/str_analysis/trim_repeat_loci.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/bam_utils.py` & `str_analysis-0.9.8/str_analysis/utils/bam_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/canonical_repeat_unit.py` & `str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/canonical_repeat_unit_tests.py` & `str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/ehdn_info_for_locus.py` & `str_analysis-0.9.8/str_analysis/utils/ehdn_info_for_locus.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/export_json.py` & `str_analysis-0.9.8/str_analysis/utils/export_json.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/fasta_utils.py` & `str_analysis-0.9.8/str_analysis/utils/fasta_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/find_repeat_unit_tests.py` & `str_analysis-0.9.8/str_analysis/utils/find_repeat_unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from str_analysis.utils.find_repeat_unit import find_repeat_unit
 
 
 class Test(unittest.TestCase):
 
     def test_compute_most_frequent_repeat_unit(self):
 
-        for repeat_unit in "A", "AC", "ACG", "ACGT", "ACGTA":
+        for repeat_unit in "A", "AC", "ACG", "ACGT", "ACGTA", "ACGATA":
             for num_repeats in 1, 2, 3, 4, 5:
                 if len(repeat_unit) == 1 and num_repeats == 1:
                     self.assertRaises(ValueError, find_repeat_unit, repeat_unit)
                     continue
 
                 found_repeat_unit, found_num_repeats = find_repeat_unit(
-                    repeat_unit * num_repeats, min_fraction_covered_by_repeat=0.95)
+                    repeat_unit * num_repeats, min_fraction_covered_by_repeat=0.8)
                 self.assertEqual(found_repeat_unit, repeat_unit,
                                  f"repeat unit not detected correctly for {repeat_unit}*{num_repeats}")
                 self.assertEqual(num_repeats, num_repeats,
                                  f"repeat count not detected correctly for {repeat_unit}*{num_repeats}")
```

### Comparing `str_analysis-0.9.7/str_analysis/utils/known_pathogenic_strs_tsv.py` & `str_analysis-0.9.8/str_analysis/utils/known_pathogenic_strs_tsv.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/misc_utils.py` & `str_analysis-0.9.8/str_analysis/utils/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Parses interval string like "chr1:12345-54321" and returns 3-tuple (chrom, start, end)"""
 
     try:
         tokens = interval_string.split(":")
         chrom = ":".join(tokens[:-1])  # some super-contig names have : in them
         start, end = map(int, tokens[-1].split("-"))
     except Exception as e:
-        raise ValueError(f"Unable to parse off_target_region: '{interval_string}': {e}")
+        raise ValueError(f"Unable to parse interval: '{interval_string}': {e}")
 
     return chrom, start, end
 
 
 def run(command):
     """Run a shell command and return its output. Raises an exception if the command exits with a non-zero exit code"""
```

### Comparing `str_analysis-0.9.7/str_analysis/utils/most_frequent_repeat_unit.py` & `str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/most_frequent_repeat_unit_tests.py` & `str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis/utils/strling_info_for_locus.py` & `str_analysis-0.9.8/str_analysis/utils/strling_info_for_locus.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.7/str_analysis.egg-info/PKG-INFO` & `str_analysis-0.9.8/str_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: str-analysis
-Version: 0.9.7
+Version: 0.9.8
 Summary: Utilities  short tandem repeats (STRs)
 Home-page: https://github.com/broadinstitute/str-analysis
 License: MIT
 Description: # str-analysis
         ---
         This package contains scripts and utilities for analyzing short tandem repeats (STRs).
```

### Comparing `str_analysis-0.9.7/str_analysis.egg-info/SOURCES.txt` & `str_analysis-0.9.8/str_analysis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 README.md
-README.txt
 setup.py
 str_analysis/__init__.py
 str_analysis/call_non_ref_pathogenic_motifs.py
 str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
 str_analysis/check_trios_for_mendelian_violations.py
 str_analysis/check_trios_for_mendelian_violations_tests.py
-str_analysis/combine_expansion_hunter_json_to_tsv.py
-str_analysis/combine_expansion_hunter_json_to_tsv_tests.py
 str_analysis/combine_json_to_tsv.py
+str_analysis/combine_str_json_to_tsv.py
+str_analysis/combine_str_json_to_tsv_tests.py
 str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
 str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
 str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
 str_analysis/convert_strling_calls_to_expansion_hunter_json.py
 str_analysis/filter_vcf_to_STR_variants.py
 str_analysis/filter_vcf_to_STR_variants_tests.py
 str_analysis/generate_gnomad_json.py
@@ -28,17 +27,19 @@
 str_analysis.egg-info/top_level.txt
 str_analysis/data/non_ref_motif.locus_info.json
 str_analysis/data/non_ref_motif.offtarget_regions.json.gz
 str_analysis/utils/__init__.py
 str_analysis/utils/bam_utils.py
 str_analysis/utils/canonical_repeat_unit.py
 str_analysis/utils/canonical_repeat_unit_tests.py
+str_analysis/utils/dat_utils.py
 str_analysis/utils/ehdn_info_for_locus.py
 str_analysis/utils/export_json.py
 str_analysis/utils/fasta_utils.py
 str_analysis/utils/find_repeat_unit.py
 str_analysis/utils/find_repeat_unit_tests.py
 str_analysis/utils/known_pathogenic_strs_tsv.py
 str_analysis/utils/misc_utils.py
 str_analysis/utils/most_frequent_repeat_unit.py
 str_analysis/utils/most_frequent_repeat_unit_tests.py
-str_analysis/utils/strling_info_for_locus.py
+str_analysis/utils/strling_info_for_locus.py
+str_analysis/utils/trf_runner.py
```


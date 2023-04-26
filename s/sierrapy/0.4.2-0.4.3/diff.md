# Comparing `tmp/sierrapy-0.4.2.tar.gz` & `tmp/sierrapy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierrapy-0.4.2.tar", last modified: Tue Mar 14 20:17:07 2023, max compression
+gzip compressed data, was "sierrapy-0.4.3.tar", last modified: Wed Apr 26 22:33:14 2023, max compression
```

## Comparing `sierrapy-0.4.2.tar` & `sierrapy-0.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.622526 sierrapy-0.4.2/
--rw-r--r--   0 philip     (501) staff       (20)       59 2020-08-26 18:43:37.000000 sierrapy-0.4.2/MANIFEST.in
--rw-r--r--   0 philip     (501) staff       (20)      820 2023-03-14 20:17:07.622660 sierrapy-0.4.2/PKG-INFO
--rw-r--r--   0 philip     (501) staff       (20)     7583 2023-03-14 20:10:06.000000 sierrapy-0.4.2/README.md
--rw-r--r--   0 philip     (501) staff       (20)      734 2023-03-14 20:16:17.000000 sierrapy-0.4.2/requirements.txt
--rw-r--r--   0 philip     (501) staff       (20)      337 2023-03-14 20:17:07.623311 sierrapy-0.4.2/setup.cfg
--rw-r--r--   0 philip     (501) staff       (20)     1838 2023-03-14 20:15:24.000000 sierrapy-0.4.2/setup.py
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.599995 sierrapy-0.4.2/sierrapy/
--rw-r--r--   0 philip     (501) staff       (20)      163 2021-10-31 23:13:51.000000 sierrapy-0.4.2/sierrapy/__init__.py
--rw-r--r--   0 philip     (501) staff       (20)      112 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/cmds.py
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.610654 sierrapy-0.4.2/sierrapy/commands/
--rw-r--r--   0 philip     (501) staff       (20)      105 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/commands/__init__.py
--rw-r--r--   0 philip     (501) staff       (20)     1231 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/commands/cli.py
--rw-r--r--   0 philip     (501) staff       (20)     3515 2023-03-14 20:10:06.000000 sierrapy-0.4.2/sierrapy/commands/fasta.py
--rw-r--r--   0 philip     (501) staff       (20)      602 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/commands/introspection.py
--rw-r--r--   0 philip     (501) staff       (20)     1520 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/commands/mutations.py
--rw-r--r--   0 philip     (501) staff       (20)     3163 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/commands/options.py
--rw-r--r--   0 philip     (501) staff       (20)     3967 2023-03-14 20:10:06.000000 sierrapy-0.4.2/sierrapy/commands/patterns.py
--rw-r--r--   0 philip     (501) staff       (20)      666 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/commands/recipe.py
--rw-r--r--   0 philip     (501) staff       (20)     7533 2022-12-14 20:22:46.000000 sierrapy-0.4.2/sierrapy/commands/seqreads.py
--rw-r--r--   0 philip     (501) staff       (20)     1592 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/common_types.py
--rw-r--r--   0 philip     (501) staff       (20)      832 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fastareader.py
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.616044 sierrapy-0.4.2/sierrapy/fragments/
--rw-r--r--   0 philip     (501) staff       (20)      576 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/__init__.py
--rw-r--r--   0 philip     (501) staff       (20)      449 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/hiv1_mutations_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)     1080 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/hiv1_sequence_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)     1850 2023-03-14 20:11:38.000000 sierrapy-0.4.2/sierrapy/fragments/hiv1_sequence_reads_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)     1080 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/hiv2_sequence_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)      179 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/sars2_mutations_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)      612 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/sars2_sequence_analysis_default.gql
--rw-r--r--   0 philip     (501) staff       (20)      879 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/fragments/sars2_sequence_reads_analysis_default.gql
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.618381 sierrapy-0.4.2/sierrapy/recipes/
--rw-r--r--   0 philip     (501) staff       (20)      162 2020-08-26 18:43:37.000000 sierrapy-0.4.2/sierrapy/recipes/__init__.py
--rw-r--r--   0 philip     (501) staff       (20)     3603 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/recipes/alignment.py
--rw-r--r--   0 philip     (501) staff       (20)     2138 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/recipes/mutationtsv.py
--rw-r--r--   0 philip     (501) staff       (20)     1952 2021-11-01 01:12:40.000000 sierrapy-0.4.2/sierrapy/recipes/sequencetsv.py
--rw-r--r--   0 philip     (501) staff       (20)     8978 2023-03-14 20:15:09.000000 sierrapy-0.4.2/sierrapy/sierraclient.py
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.622014 sierrapy-0.4.2/sierrapy/viruses/
--rw-r--r--   0 philip     (501) staff       (20)      142 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/viruses/__init__.py
--rw-r--r--   0 philip     (501) staff       (20)     1581 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/viruses/hiv1.py
--rw-r--r--   0 philip     (501) staff       (20)     1331 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/viruses/hiv2.py
--rw-r--r--   0 philip     (501) staff       (20)     8391 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/viruses/sars2.py
--rw-r--r--   0 philip     (501) staff       (20)     2315 2022-08-02 19:11:49.000000 sierrapy-0.4.2/sierrapy/viruses/virus.py
-drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-03-14 20:17:07.604765 sierrapy-0.4.2/sierrapy.egg-info/
--rw-r--r--   0 philip     (501) staff       (20)      820 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/PKG-INFO
--rw-r--r--   0 philip     (501) staff       (20)     1335 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/SOURCES.txt
--rw-r--r--   0 philip     (501) staff       (20)        1 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/dependency_links.txt
--rw-r--r--   0 philip     (501) staff       (20)       49 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/entry_points.txt
--rw-r--r--   0 philip     (501) staff       (20)      520 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/requires.txt
--rw-r--r--   0 philip     (501) staff       (20)       80 2023-03-14 20:17:07.000000 sierrapy-0.4.2/sierrapy.egg-info/top_level.txt
--rw-r--r--   0 philip     (501) staff       (20)        1 2020-11-12 22:47:28.000000 sierrapy-0.4.2/sierrapy.egg-info/zip-safe
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.510493 sierrapy-0.4.3/
+-rw-r--r--   0 philip     (501) staff       (20)       59 2020-08-26 18:43:37.000000 sierrapy-0.4.3/MANIFEST.in
+-rw-r--r--   0 philip     (501) staff       (20)      820 2023-04-26 22:33:14.510619 sierrapy-0.4.3/PKG-INFO
+-rw-r--r--   0 philip     (501) staff       (20)     7843 2023-03-31 21:36:25.000000 sierrapy-0.4.3/README.md
+-rw-r--r--   0 philip     (501) staff       (20)      734 2023-03-14 20:16:17.000000 sierrapy-0.4.3/requirements.txt
+-rw-r--r--   0 philip     (501) staff       (20)      337 2023-04-26 22:33:14.511180 sierrapy-0.4.3/setup.cfg
+-rw-r--r--   0 philip     (501) staff       (20)     1838 2023-04-26 22:22:29.000000 sierrapy-0.4.3/setup.py
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.397177 sierrapy-0.4.3/sierrapy/
+-rw-r--r--   0 philip     (501) staff       (20)      163 2021-10-31 23:13:51.000000 sierrapy-0.4.3/sierrapy/__init__.py
+-rw-r--r--   0 philip     (501) staff       (20)      112 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/cmds.py
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.453371 sierrapy-0.4.3/sierrapy/commands/
+-rw-r--r--   0 philip     (501) staff       (20)      105 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/commands/__init__.py
+-rw-r--r--   0 philip     (501) staff       (20)     1231 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/commands/cli.py
+-rw-r--r--   0 philip     (501) staff       (20)     3515 2023-03-14 20:10:06.000000 sierrapy-0.4.3/sierrapy/commands/fasta.py
+-rw-r--r--   0 philip     (501) staff       (20)      602 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/commands/introspection.py
+-rw-r--r--   0 philip     (501) staff       (20)     1520 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/commands/mutations.py
+-rw-r--r--   0 philip     (501) staff       (20)     3163 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/commands/options.py
+-rw-r--r--   0 philip     (501) staff       (20)     3967 2023-03-14 20:10:06.000000 sierrapy-0.4.3/sierrapy/commands/patterns.py
+-rw-r--r--   0 philip     (501) staff       (20)      666 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/commands/recipe.py
+-rw-r--r--   0 philip     (501) staff       (20)     7532 2023-03-31 21:36:25.000000 sierrapy-0.4.3/sierrapy/commands/seqreads.py
+-rw-r--r--   0 philip     (501) staff       (20)     1592 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/common_types.py
+-rw-r--r--   0 philip     (501) staff       (20)      832 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fastareader.py
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.461642 sierrapy-0.4.3/sierrapy/fragments/
+-rw-r--r--   0 philip     (501) staff       (20)      576 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/__init__.py
+-rw-r--r--   0 philip     (501) staff       (20)      449 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/hiv1_mutations_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)     1080 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/hiv1_sequence_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)     1974 2023-03-31 21:36:25.000000 sierrapy-0.4.3/sierrapy/fragments/hiv1_sequence_reads_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)     1080 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/hiv2_sequence_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)      179 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/sars2_mutations_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)      612 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/sars2_sequence_analysis_default.gql
+-rw-r--r--   0 philip     (501) staff       (20)      879 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/fragments/sars2_sequence_reads_analysis_default.gql
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.505003 sierrapy-0.4.3/sierrapy/recipes/
+-rw-r--r--   0 philip     (501) staff       (20)      162 2020-08-26 18:43:37.000000 sierrapy-0.4.3/sierrapy/recipes/__init__.py
+-rw-r--r--   0 philip     (501) staff       (20)     3603 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/recipes/alignment.py
+-rw-r--r--   0 philip     (501) staff       (20)     2138 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/recipes/mutationtsv.py
+-rw-r--r--   0 philip     (501) staff       (20)     1952 2021-11-01 01:12:40.000000 sierrapy-0.4.3/sierrapy/recipes/sequencetsv.py
+-rw-r--r--   0 philip     (501) staff       (20)     8978 2023-04-26 22:22:58.000000 sierrapy-0.4.3/sierrapy/sierraclient.py
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.509754 sierrapy-0.4.3/sierrapy/viruses/
+-rw-r--r--   0 philip     (501) staff       (20)      142 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/viruses/__init__.py
+-rw-r--r--   0 philip     (501) staff       (20)     2346 2023-03-31 21:36:25.000000 sierrapy-0.4.3/sierrapy/viruses/hiv1.py
+-rw-r--r--   0 philip     (501) staff       (20)     1331 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/viruses/hiv2.py
+-rw-r--r--   0 philip     (501) staff       (20)     8391 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/viruses/sars2.py
+-rw-r--r--   0 philip     (501) staff       (20)     2315 2022-08-02 19:11:49.000000 sierrapy-0.4.3/sierrapy/viruses/virus.py
+drwxr-xr-x   0 philip     (501) staff       (20)        0 2023-04-26 22:33:14.401521 sierrapy-0.4.3/sierrapy.egg-info/
+-rw-r--r--   0 philip     (501) staff       (20)      820 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/PKG-INFO
+-rw-r--r--   0 philip     (501) staff       (20)     1335 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/SOURCES.txt
+-rw-r--r--   0 philip     (501) staff       (20)        1 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/dependency_links.txt
+-rw-r--r--   0 philip     (501) staff       (20)       49 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/entry_points.txt
+-rw-r--r--   0 philip     (501) staff       (20)      520 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/requires.txt
+-rw-r--r--   0 philip     (501) staff       (20)       80 2023-04-26 22:33:14.000000 sierrapy-0.4.3/sierrapy.egg-info/top_level.txt
+-rw-r--r--   0 philip     (501) staff       (20)        1 2020-11-12 22:47:28.000000 sierrapy-0.4.3/sierrapy.egg-info/zip-safe
```

### Comparing `sierrapy-0.4.2/PKG-INFO` & `sierrapy-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierrapy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Client of HIVdb Sierra GraphQL Webservice.
 Home-page: https://github.com/hivdb/sierra-client/tree/master/python
 Author: Philip Tzou
 Author-email: philiptz@stanford.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sierrapy-0.4.2/README.md` & `sierrapy-0.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -84,27 +84,36 @@
 assuming it is saved at `path/to/your/query/file.gql`, use this command to get
 the customized result:
 
 ```shell
 sierrapy fasta fasta1.fasta fasta2.fasta -q path/to/your/query/file.gql
 ```
 
-By default, SierraPy stores every 100 sequence results in a single JSON file
-in case of memory exhaustion. This behavior can be overridden by passing a
+For further infomations on how to write queries in GraphQL, please visit
+[graphql.org/learn][graphql-learn]. For API reference and a playground of HIVDB
+GraphQL service, please visit [hivdb.stanford.edu/page/graphiql][graphiql].
+
+#### Sharding
+
+By default, SierraPy stores the results of every 100 sequences in a single JSON
+file to prevent memory exhaustion. You can override this behavior by passing the
 `--sharding` parameter to the command. It is safe to increase the `--sharding`
-to 200 or even 500. However, as it gets larger, the JSON file will become
-increasely difficult to read or write with most popular JSON parsers:
+value to 200 or even 500. However, as the value increases, the JSON file will
+become increasingly difficult to read or write with most popular JSON parsers:
 
 ```shell
 sierrapy fasta fasta1.fasta fasta2.fasta --sharding 200
 ```
 
-For further infomations on how to write queries in GraphQL, please visit
-[graphql.org/learn][graphql-learn]. For API reference and a playground of HIVDB
-GraphQL service, please visit [hivdb.stanford.edu/page/graphiql][graphiql].
+You can also disable the sharding mechanism completely by using the `--no-sharding`
+flag. This will prevent the addition of a suffix to the output JSON file.
+
+```
+sierrapy fasta fasta1.fasta fasta2.fasta --no-sharding
+```
 
 ### Input Sequence Reads (CodFreq File)
 
 This method is corresponding to the [HIVDB "Input sequence
 reads"][hivdb-seqreadsinput] tab. It can accept a list of CodFreq files or
 directories that containing CodFreq files. JSON format reports will be
 generated for each CodFreq files when the analysis completed.
```

### Comparing `sierrapy-0.4.2/requirements.txt` & `sierrapy-0.4.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/setup.py` & `sierrapy-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: UTF-8 -*-
 
 import os
 import setuptools  # type: ignore
 
 from typing import List
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 
 
 def strip_comments(line: str) -> str:
     if line.startswith('-i '):
         return ''
     return line.split('#', 1)[0].strip()
```

### Comparing `sierrapy-0.4.2/sierrapy/commands/cli.py` & `sierrapy-0.4.3/sierrapy/commands/cli.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/fasta.py` & `sierrapy-0.4.3/sierrapy/commands/fasta.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/introspection.py` & `sierrapy-0.4.3/sierrapy/commands/introspection.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/mutations.py` & `sierrapy-0.4.3/sierrapy/commands/mutations.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/options.py` & `sierrapy-0.4.3/sierrapy/commands/options.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/patterns.py` & `sierrapy-0.4.3/sierrapy/commands/patterns.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/recipe.py` & `sierrapy-0.4.3/sierrapy/commands/recipe.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/commands/seqreads.py` & `sierrapy-0.4.3/sierrapy/commands/seqreads.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
               type=float, default=0.1, show_default=True,
               help=('Minimal prevalence cutoff for this sequence reads '
                     '(range: 0-1.0)'))
 @click.option('-m', '--mixture-cutoff',
               type=float, default=0.0005, show_default=True,
               help=('Maximum mixture rate for this sequence reads '
                     '(range: 0-1.0)'))
-@click.option('-d', '--min-codon-reads', type=int, default=10,
+@click.option('-d', '--min-codon-reads', type=int, default=1,
               show_default=True,
               help=('Minimal read depth applied to '
                     'each codon of this sequence'))
 @click.option('-D', '--min-position-reads', type=int, default=1,
               show_default=True,
               help=('Minimal read depth applied to '
                     'each position of this sequence'))
```

### Comparing `sierrapy-0.4.2/sierrapy/common_types.py` & `sierrapy-0.4.3/sierrapy/common_types.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fastareader.py` & `sierrapy-0.4.3/sierrapy/fastareader.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fragments/__init__.py` & `sierrapy-0.4.3/sierrapy/fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fragments/hiv1_sequence_analysis_default.gql` & `sierrapy-0.4.3/sierrapy/fragments/hiv1_sequence_analysis_default.gql`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fragments/hiv1_sequence_reads_analysis_default.gql` & `sierrapy-0.4.3/sierrapy/fragments/hiv1_sequence_reads_analysis_default.gql`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 name
 bestMatchingSubtype {
     display
     referenceAccession
 }
 availableGenes { name }
+maxMixtureRate
+minCodonReads
 minPositionReads
 minPrevalence
+actualMinPrevalence
+mixtureRate
+assembledConsensus
 readDepthStats {
     mean standardDeviation min max n
     p5: percentile(p: 5)
     p10: percentile(p: 10)
     p25: percentile(p: 25)
     p50: percentile(p: 50)
     p75: percentile(p: 75)
@@ -22,14 +27,18 @@
     p10: percentile(p: 10)
     p25: percentile(p: 25)
     p50: percentile(p: 50)
     p75: percentile(p: 75)
     p90: percentile(p: 90)
     p95: percentile(p: 95)
 }
+validationResults {
+    level
+    message
+}
 allGeneSequenceReads {
     firstAA lastAA
     gene { name, length }
     mutations {
         reference,
         position,
         AAs,
```

### Comparing `sierrapy-0.4.2/sierrapy/fragments/hiv2_sequence_analysis_default.gql` & `sierrapy-0.4.3/sierrapy/fragments/hiv2_sequence_analysis_default.gql`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fragments/sars2_sequence_analysis_default.gql` & `sierrapy-0.4.3/sierrapy/fragments/sars2_sequence_analysis_default.gql`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/fragments/sars2_sequence_reads_analysis_default.gql` & `sierrapy-0.4.3/sierrapy/fragments/sars2_sequence_reads_analysis_default.gql`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/recipes/alignment.py` & `sierrapy-0.4.3/sierrapy/recipes/alignment.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/recipes/mutationtsv.py` & `sierrapy-0.4.3/sierrapy/recipes/mutationtsv.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/recipes/sequencetsv.py` & `sierrapy-0.4.3/sierrapy/recipes/sequencetsv.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/sierraclient.py` & `sierrapy-0.4.3/sierrapy/sierraclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gql.transport.requests import RequestsHTTPTransport
 from requests.exceptions import HTTPError  # type: ignore
 from graphql.language.ast import DocumentNode as gqlDocument
 
 from .common_types import Sequence, SeqReads, ServerVer
 
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 DEFAULT_URL = 'https://hivdb.stanford.edu/graphql'
 
 
 class ResponseError(Exception):
     pass
```

### Comparing `sierrapy-0.4.2/sierrapy/viruses/hiv2.py` & `sierrapy-0.4.3/sierrapy/viruses/hiv2.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/viruses/sars2.py` & `sierrapy-0.4.3/sierrapy/viruses/sars2.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy/viruses/virus.py` & `sierrapy-0.4.3/sierrapy/viruses/virus.py`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy.egg-info/PKG-INFO` & `sierrapy-0.4.3/sierrapy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierrapy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Client of HIVdb Sierra GraphQL Webservice.
 Home-page: https://github.com/hivdb/sierra-client/tree/master/python
 Author: Philip Tzou
 Author-email: philiptz@stanford.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sierrapy-0.4.2/sierrapy.egg-info/SOURCES.txt` & `sierrapy-0.4.3/sierrapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sierrapy-0.4.2/sierrapy.egg-info/requires.txt` & `sierrapy-0.4.3/sierrapy.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-graphql-core==3.2.3
-voluptuous==0.13.1
+more-itertools==9.1.0
 click==8.1.3
-requests-toolbelt==0.10.1
-promise==2.3
 requests==2.28.2
-six==1.16.0
-tqdm==4.65.0
-more-itertools==9.1.0
 gql==3.4.0
+tqdm==4.65.0
+graphql-core==3.2.3
+promise==2.3
+six==1.16.0
+voluptuous==0.13.1
+requests-toolbelt==0.10.1
 
 [:python_full_version >= "3.7.0"]
 multidict==6.0.4
-yarl==1.8.2
 charset-normalizer==3.1.0
+yarl==1.8.2
 
 [:python_version < "4.0" and python_full_version >= "3.7.0"]
 backoff==2.2.1
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
 urllib3==1.26.15
```


# Comparing `tmp/cladeomatic-0.1.0.tar.gz` & `tmp/cladeomatic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cladeomatic-0.1.0.tar", last modified: Mon Apr 24 17:18:22 2023, max compression
+gzip compressed data, was "cladeomatic-0.1.1.tar", last modified: Thu Apr 27 12:21:25 2023, max compression
```

## Comparing `cladeomatic-0.1.0.tar` & `cladeomatic-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.354730 cladeomatic-0.1.0/
--rw-r--r--   0 jrobertson   (502) staff       (20)    11357 2022-06-27 19:03:32.000000 cladeomatic-0.1.0/LICENSE
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-27 19:04:06.000000 cladeomatic-0.1.0/MANIFEST.in
--rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-24 17:18:22.353746 cladeomatic-0.1.0/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)     9241 2023-03-31 20:37:18.000000 cladeomatic-0.1.0/README.md
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.337570 cladeomatic-0.1.0/cladeomatic/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 18:18:38.000000 cladeomatic-0.1.0/cladeomatic/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    12959 2022-11-14 20:52:10.000000 cladeomatic-0.1.0/cladeomatic/benchmark.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    51241 2023-04-20 20:04:29.000000 cladeomatic-0.1.0/cladeomatic/clades.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     2545 2023-04-20 19:54:43.000000 cladeomatic-0.1.0/cladeomatic/constants.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    51815 2023-04-19 17:46:08.000000 cladeomatic-0.1.0/cladeomatic/create.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    17214 2023-04-20 20:07:06.000000 cladeomatic-0.1.0/cladeomatic/genotype.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    34892 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/kmers.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1602 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/main.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     2694 2022-12-08 20:22:59.000000 cladeomatic-0.1.0/cladeomatic/namer.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     7514 2023-04-19 15:06:51.000000 cladeomatic-0.1.0/cladeomatic/snps.py
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 17:34:28.000000 cladeomatic-0.1.0/cladeomatic/test.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.352278 cladeomatic-0.1.0/cladeomatic/utils/
--rw-r--r--   0 jrobertson   (502) staff       (20)     3440 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      961 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/jellyfish.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     6588 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/kmerSearch.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     9377 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/phylo_tree.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    10264 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/seqdata.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      742 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/snpdists.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     3207 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/vcfhelper.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1308 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/visualization.py
--rw-r--r--   0 jrobertson   (502) staff       (20)       21 2023-04-21 13:45:27.000000 cladeomatic-0.1.0/cladeomatic/version.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1071 2023-04-04 17:14:30.000000 cladeomatic-0.1.0/cladeomatic/visualize.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     5491 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/writers.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.343284 cladeomatic-0.1.0/cladeomatic.egg-info/
--rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)      815 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/SOURCES.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/dependency_links.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       54 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/entry_points.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)      283 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/requires.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       12 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/top_level.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-04-24 17:18:22.355036 cladeomatic-0.1.0/setup.cfg
--rw-r--r--   0 jrobertson   (502) staff       (20)     2152 2023-04-24 17:18:06.000000 cladeomatic-0.1.0/setup.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-27 12:21:25.001001 cladeomatic-0.1.1/
+-rw-r--r--   0 jrobertson   (502) staff       (20)    11357 2022-06-27 19:03:32.000000 cladeomatic-0.1.1/LICENSE
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-27 19:04:06.000000 cladeomatic-0.1.1/MANIFEST.in
+-rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-27 12:21:25.000058 cladeomatic-0.1.1/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)    10472 2023-04-26 20:35:11.000000 cladeomatic-0.1.1/README.md
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-27 12:21:24.983651 cladeomatic-0.1.1/cladeomatic/
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 18:18:38.000000 cladeomatic-0.1.1/cladeomatic/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     8857 2023-04-26 20:00:36.000000 cladeomatic-0.1.1/cladeomatic/benchmark.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    51241 2023-04-20 20:04:29.000000 cladeomatic-0.1.1/cladeomatic/clades.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2869 2023-04-26 20:00:36.000000 cladeomatic-0.1.1/cladeomatic/constants.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    51817 2023-04-26 17:23:21.000000 cladeomatic-0.1.1/cladeomatic/create.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    17249 2023-04-26 20:00:36.000000 cladeomatic-0.1.1/cladeomatic/genotype.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    34892 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/kmers.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1602 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/main.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2327 2023-04-27 12:01:47.000000 cladeomatic-0.1.1/cladeomatic/namer.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     7514 2023-04-19 15:06:51.000000 cladeomatic-0.1.1/cladeomatic/snps.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 17:34:28.000000 cladeomatic-0.1.1/cladeomatic/test.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-27 12:21:24.998881 cladeomatic-0.1.1/cladeomatic/utils/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3444 2023-04-26 18:32:45.000000 cladeomatic-0.1.1/cladeomatic/utils/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      961 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/jellyfish.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     6588 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/kmerSearch.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     9377 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/phylo_tree.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    10264 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/seqdata.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      742 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/snpdists.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3207 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/vcfhelper.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1308 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/utils/visualization.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)       21 2023-04-27 12:18:47.000000 cladeomatic-0.1.1/cladeomatic/version.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1071 2023-04-04 17:14:30.000000 cladeomatic-0.1.1/cladeomatic/visualize.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     5491 2023-04-19 14:55:01.000000 cladeomatic-0.1.1/cladeomatic/writers.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-27 12:21:24.987702 cladeomatic-0.1.1/cladeomatic.egg-info/
+-rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)      815 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       54 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/entry_points.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)      252 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/requires.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       12 2023-04-27 12:21:24.000000 cladeomatic-0.1.1/cladeomatic.egg-info/top_level.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-04-27 12:21:25.001333 cladeomatic-0.1.1/setup.cfg
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2109 2023-04-27 12:11:59.000000 cladeomatic-0.1.1/setup.py
```

### Comparing `cladeomatic-0.1.0/LICENSE` & `cladeomatic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/PKG-INFO` & `cladeomatic-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cladeomatic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Clade-O-Matic: Automatic recognition of population structures based on canonical SNPs
 Home-page: https://github.com/phac-nml/cladeomaticc
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Keywords: Genotyping,population structure,kmer
 Classifier: Development Status :: 3 - Alpha
@@ -14,9 +14,9 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8.0,<4
+Requires-Python: >=3.9.0,<4
 License-File: LICENSE
```

### Comparing `cladeomatic-0.1.0/README.md` & `cladeomatic-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-[![PyPI](https://img.shields.io/badge/Install%20with-PyPI-blue)](https://pypi.org/project/chewBBACA/#description)
-[![Bioconda](https://img.shields.io/badge/Install%20with-bioconda-green)](https://anaconda.org/bioconda/chewbbaca)
-[![Conda](https://img.shields.io/conda/dn/bioconda/cladeomatic?color=green)](https://anaconda.org/bioconda/chewbbaca)
-[![License: GPL v3](https://img.shields.io/github/license/phac-nml/cladeomatic)](https://www.apache.org/licenses/LICENSE-2.0)
-[![DOI:10.1099/](https://img.shields.io/badge/DOI-10.1099%2F-blue)]
+[![PyPI](https://img.shields.io/badge/Install%20with-PyPI-blue)](https://pypi.org/project/cladeomatic/#description)
+[![Bioconda](https://img.shields.io/badge/Install%20with-bioconda-green)](https://anaconda.org/bioconda/cladeomatic)
+[![Conda](https://img.shields.io/conda/dn/bioconda/cladeomatic?color=green)](https://anaconda.org/bioconda/cladeomatic)
+[![License: Apache-2.0](https://img.shields.io/github/license/phac-nml/cladeomatic)](https://www.apache.org/licenses/LICENSE-2.0)
+
 
 <p align="left"><img src="logo.png" alt="Clade-o-matic" height="150" width="400"></p>
 
 ## Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
@@ -19,20 +19,24 @@
 
 ## Introduction
 
 Identification of population structure based on genomic data is a routine problem in molecular epidemiology and numerous approaches have been developed to partition large collections of sequences into clusters at different levels of granularity and resolution based on the goals of the researchers and underlying genetic diversity of the dataset. There is a confusing variety of terms in use to describe these units of genetic relatedness depending on the level of resolution provided and the specific taxon: clades, clones, clades, groups, genotypes, haplotypes, lineages, and subtypes.
 
 Clade-o-matic is a phylogenetic approach for identification of hierarchal genotypes based on canonical SNPs that are exclusive and conserved within phylogenetic clades. It works best with organisms that have low rates of recombination and limited genetic diversity, but it is possible to analyze species-wide phylogenies. A major distinction of Clade-o-matic from other population structure tools such as rheirbaps is that it provides the distinguishing features for each clade in the form of a SNP typing scheme with unique kmers for identification of these SNPs from raw sequencing data. Furthermore, Clade-o-matic does not use a fixed set of levels for hierarchy as there will be uneven groupings between different clades. It uses the underlying distance distributions to compress the hierarchy into the minimum set of levels that retain the tree structure. The granularity of the scheme can be changed by specifiying different numbers of SNPs required to support a clade along with the number of members assigned to a clade for it to be considered valid.
 
+### Check the [documentation](https://cladeomatic-documentation.readthedocs.io/en/latest/) for implementation details and guidance on using Clade-O-Matic.
 
 ## Installation
 
 Python dependencies (defined in the [requirements](https://github.com/phac-nml/cladeomatic/blob/main/requirements.txt) file, should be automatically installed when using conda or pip)
 
-In addition to the python dependencies, Clade-o-Matic requires [Jellyfish 2.3.0](https://github.com/gmarcais/Jellyfish/)
+In addition to the python dependencies, Clade-o-Matic requires:
+[Jellyfish 2.3.0](https://github.com/gmarcais/Jellyfish/)
+[snp-dists 0.8.2](https://github.com/tseemann/snp-dists/)
+
 
 Install the latest released version from conda:
 
         conda create -c bioconda -c conda-forge -n cladeomatic cladeomatic
 
 Install using pip:
 
@@ -56,34 +60,36 @@
     To get full help for a command use one of:
     cladeomatic command -h
     cladeomatic command --help
 
 
     Available commands:
 
-    create  Define lineages and create a kmer scheme
-    benchmark  Benchmark a kmer scheme
-    test     Test parsityper functionality on a small dataset [ not implemented]
-    version  Print version and exit
+    create     Identify population structure and develop typing scheme
+    genotype   Call genotypes from a VCF and a scheme file
+    benchmark  Test developed scheme using labeled samples and scheme
+    namer      Rename genotypes within a scheme*
+    
+    *Coming soon
 
 Quick start
 =====
 **Create scheme:**
 
 Option 1 - De novo tree-based <br />
 This mode will discover clades and lineages which meet membership size and SNP requirements. 
 Input requirements are: 
 * newick formatted tree
 * Reference (Outgroup) sequence (.fasta / .gbk)
 * VCF (Must use the same reference sequence as above)
 * Name of Reference (Outgroup) sequence (Must be the same as the reference sequence)
 * Metadata file<br />
-  
 
-    cladeomatic create --in_nwk tree.nwk  --in_var variants.vcf --in_meta metadata.txt --outdir scheme/ --root_name ref --reference ref.gbk
+
+        cladeomatic create --in_nwk examples/small_test/tree.nwk  --in_var examples/small_test/snps.vcf --in_meta examples/small_test/sample.meta.txt --outdir small_test_cladeomatic/ --root_name root.0 --reference examples/small_test/root.gbk
 
 Option 2 - Predefined groups <br />
 This mode will attempt to define a scheme based on a group manifest which meet membership size and SNP requirements.
 Note every group id must be unique accross all ranks to use this feature.Cladeomatic uses this for internal representation 
 of the genotypes but they can be mapped to whatever nomenclature is desired to have as an output
 
 | sample_id     | invalid_genotype | valid_genotype |
@@ -99,93 +105,94 @@
 
 Input requirements are: 
 * TSV formatted group file (sample_id, genotype)
 * VCF
 * Reference sequence (.fasta / .gbk)
 * Name of outgroup sequence
 * Metadata file<br />
-  
 
-    cladeomatic create --in_groups groups.tsv --in_var variants.vcf --in_meta metadata.txt --outdir scheme/ --root_name ref --reference ref.gbk
+
+        cladeomatic create --in_groups examples/small_test/groups.tsv --in_var examples/small_test/snps.vcf --in_meta examples/small_test/sample.meta.txt --outdir small_test_cladeomatic_groups/ --root_name root.0 --reference examples/small_test/root.gbk
   
 
 **Outputs:**
 
 ```
-OutputFolderName
-├── {prefix}-params.log - Selected parameters for the run
+{Output folder name}
+├── {prefix}-altseq.fasta - Artificial sequence which has a different base from the reference at every position in scheme
+├── {prefix}-biohansel.fasta  - biohansel formatted kmer fasta file
+├── {prefix}-biohansel.meta.txt - descriptions of biohansel kmers: kmername,target_position,target_base
 ├── {prefix}-clades.info.txt - Information on each individual clade, including supporting SNPs and metadata associations
+├── {prefix}-dist.mat.txt - tab delimeted distance matrix from snp-dists
 ├── {prefix}-extracted.kmers.txt - Raw kmer output of extracted kmers with positions mapped
+├── {prefix}-filtered.vcf - VCF file where invalid sites have been removed
+├── {prefix}-genotypes.distance.txt - Histogram of node distances
 ├── {prefix}-genotypes.raw.txt - Tree or group file without filtering
-├── {prefix}-genotypes.supported.txt - Nodes which meet the user criteria
-├── {prefix}-genotypes.selected.txt - Nodes which were selected based on the supported nodes
+├── {prefix}-genotypes.selected.txt - Nodes which meet the user criteria
+├── {prefix}-genotypes.supported.txt - Nodes which were selected based on the supported nodes
+├── {prefix}-kmer.scheme.txt - Cladeomatic kmer based scheme
+├── {prefix}-params.log - Selected parameters for the run
 ├── {prefix}-sample.distances.html - Histogram of node distances
-├── {prefix}-scheme.txt - Cladeomatic kmer based scheme
-├── {prefix}-snp.scheme.txt - Cladeomatic SNP based scheme
-├── {prefix}-filtered.vcf - VCF file where invalid sites have been removed
+├── {prefix}-snps.scheme.txt - Cladeomatic SNP based scheme
+├── {prefix}-snps.info.txt
 ├── pseudo.seqs.fasta - reconstructed fasta sequences based on reference sequence and vcf
-├── {prefix}-dist.mat.txt - tab delimeted distance matrix from snp-dists
-├── {prefix}-biohansel.fasta - biohansel formatted kmer fasta file
-├── {prefix}-biohansel.meta.txt - descriptions of biohansel kmers: kmername,target_position,target_base
-├── {prefix}-genotypes.distance.txt - defined threshold {single,average,complete}-linkage clusters
 └──
 ```
 
 **Genotype:**
 Genotype samples using the developed scheme based on a VCF file with the same reference selected to build the scheme
 Input requirements are: 
 * VCF
 * Clade-O-Matic Scheme
+* Metadata file (sample_id,genotype) * Produced by "create" {prefix}-genotypes.selected.txt
 * (Optional) Metadata file (sample_id,genotype) * Produced by "create" {prefix}-genotypes.selected.txt
-  
 
-    cladeomatic genotype --in_var variants.vcf --in_scheme cladeomatic-scheme.txt --in_meta metadata.txt --outdir benchmark/ 
+
+    cladeomatic genotype --in_var examples/small_test/snps.vcf --in_scheme examples/small_test/cladeomatic-snp.scheme.txt --sample_meta examples/small_test/sample.meta.txt --genotype_meta examples/small_test/genotype.meta.txt --outfile genotype.calls.txt
 
 VCF files will not include positions which are exclusively the reference sequence or missing and this poses an issue for calling
 genotypes based on the VCF file where missing and reference state cannot be distinguished. A work around for this issue is the inclusion 
 of a sequence which is different from the reference sequence for every position targeted by the scheme. The create module generates a sequence 
 where every position used by the scheme is flipped to be a different base from the reference. This is not an ideal solution but it will allow
 users to use the genotype module using SNIPPY-CORE with their query sequence and the "alt" sequence.
 
 
 **Outputs:**
 Outputs a file with the genotype calls for each input sample
-```
-OutputFolderName
-└──  {prefix}.txt
-```
-
 
 
 **Benchmark Scheme:**
 Benchmark the scheme based on the output of genotype tool. At this point only vcf based genotyping is supported
 Input requirements are: 
-* TXT file produced by genotype module with predicted and expected genotypes
-
-
-    cladeomatic benchmark --in_var variants.vcf --in_scheme cladeomatic-scheme.txt --in_meta metadata.txt --outdir benchmark/ 
+* TXT file produced by genotype module with predicted and expected genotypes, or tsv with predicted and submitted genotype information
+* Clade-O-Matic scheme file used to call genotypes
+* VCF
+* Name of column for predicted genotype
+* Name of column for submitted genotype
 
-Evaluate the results for any conflicting genotypes
+    cladeomatic benchmark --in_var examples/small_test/snps.vcf --in_scheme examples/small_test/cladeomatic-kmer.scheme.txt --in_genotype examples/small_test/genotype.calls.txt --submitted_genotype_col genotype --predicted_genotype_col predicted_genotype  --outdir benchmark
 
+The benchmark tool will identify the F1 scores for calling genotypes based on the provided scheme and will report per sample any sites which are responsible for 
+the submitted genotype not being called
 
 **Outputs:**
 
 ```
 OutputFolderName
 ├── {prefix}-scheme.scores.txt
-└── {prefix}-scheme.calls.txt
+└── {prefix}-sample.results.txt
 ```
 
 ## FAQ
 
 ## Citation
 
 ## Legal
 
-Copyright Government of Canada 2022
+Copyright Government of Canada 2023
 
 Written by: National Microbiology Laboratory, Public Health Agency of Canada
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this work except in compliance with the License. You may obtain a copy of the
 License at:
```

### Comparing `cladeomatic-0.1.0/cladeomatic/benchmark.py` & `cladeomatic-0.1.1/cladeomatic/genotype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-import os
 import sys
-
+import os
 import ray
 from cladeomatic.version import __version__
 from cladeomatic.utils.vcfhelper import vcfReader
 from cladeomatic.utils import init_console_logger
 from cladeomatic.utils import parse_metadata
 import pandas as pd
 from argparse import (ArgumentParser, ArgumentDefaultsHelpFormatter, RawDescriptionHelpFormatter)
-from sklearn.metrics import f1_score
-import time
+from cladeomatic.constants import GENOTYPE_REPORT_HEADER, MIN_FILE_SIZE
+from datetime import datetime
+
 
 def parse_args():
     class CustomFormatter(ArgumentDefaultsHelpFormatter, RawDescriptionHelpFormatter):
         pass
 
     parser = ArgumentParser(
         description="Clade-O-Matic: Genotyping scheme development v. {}".format(__version__),
         formatter_class=CustomFormatter)
     parser.add_argument('--in_var', type=str, required=True,
                         help='Either Variant Call SNP data (.vcf) or TSV SNP data (.txt)')
     parser.add_argument('--in_scheme', type=str, required=True, help='Tab delimited scheme file produced by clade-o-matic',
                         default=None)
-    parser.add_argument('--in_meta', type=str, required=True, help='Tab delimited file of genotype assignments', default=None)
-    parser.add_argument('--outdir', type=str, required=True, help='Output Directory to put results')
+    parser.add_argument('--sample_meta', type=str, required=True, help='Tab delimited sample metadata', default=None)
+    parser.add_argument('--genotype_meta', type=str, required=False, help='Tab delimited genotype metadata', default=None)
+    parser.add_argument('--outfile', type=str, required=True, help='Output Directory to put results')
+    parser.add_argument('--max_missing_positions', type=int, required=False, help='Maximum number of missing positions for the genotype', default=1)
     parser.add_argument('--num_threads', type=int, required=False, help='Number of threads to use', default=1)
-    parser.add_argument('--prefix', type=str, required=False, help='Prefix for output files', default='cladeomatic')
-    parser.add_argument('--debug', required=False, help='Show debug information', action='store_true')
     parser.add_argument('-V', '--version', action='version', version="%(prog)s " + __version__)
 
     return parser.parse_args()
 
-
 def get_snp_profiles(valid_positions, vcf_file):
     '''
     Accepts SNP position list and vcf file
     :param valid_positions: list of integers
     :param vcf_file: str path to vcf or tsv snp data
     :return: dict of snp_data data structure
     '''
@@ -61,19 +60,96 @@
             profiles[sample_id][pos] = base
         count_snps += 1
 
         data = vcf.process_row()
 
     return profiles
 
+def parse_scheme_features(scheme_file):
+
+    features = {
+        'scheme':{},
+        'num_positions':0,
+        'num_mutations':0,
+        'total_scheme_features':0,
+        'mutation_lookup':{}
+    }
+
+    scheme = {}
+    df = pd.read_csv(scheme_file, sep="\t", header=0, low_memory=False)
+    snp_states = {}
+    num_positions = df['variant_start'].nunique()
+    num_features = df['mutation_key'].nunique()
+    features['total_scheme_features'] = len(df)
+    features['num_positions'] = num_positions
+    features['num_mutations'] = num_features
+
+    for row in df.itertuples():
+        state = row.state
+        mutation_key = row.mutation_key
+        target_variant = row.target_variant
+        variant_start = int(row.variant_start)
+        if not variant_start in features['mutation_lookup']:
+            features['mutation_lookup'][variant_start] = {'alt':{},'ref':{}}
+        features['mutation_lookup'][variant_start][state][target_variant] = mutation_key
+
+        positive_genotypes = row.positive_genotypes
+        if isinstance(positive_genotypes, float):
+            positive_genotypes = []
+        else:
+            positive_genotypes = positive_genotypes.split(',')
+
+        genotypes = positive_genotypes
+        for genotype in positive_genotypes:
+
+            if not genotype in scheme:
+                scheme[genotype] = {'positive': {}, 'partial': {}, 'allowed': {}}
+            if not variant_start in scheme[genotype]['positive']:
+                scheme[genotype]['positive'][variant_start] = set()
+            scheme[genotype]['positive'][variant_start].add(target_variant)
+
+        partial_genotypes = row.partial_genotypes
+
+        if not variant_start in snp_states:
+            snp_states[variant_start] = set()
+        snp_states[variant_start].add(target_variant)
+
+        if isinstance(partial_genotypes, float):
+            partial_genotypes = []
+        else:
+            partial_genotypes = partial_genotypes.split(',')
+        genotypes += partial_genotypes
+        if len(partial_genotypes) == 0:
+            continue
+        for genotype in partial_genotypes:
+            if not genotype in scheme:
+                scheme[genotype] = {'positive': {}, 'partial': {}, 'allowed': {}}
+            if not variant_start in scheme[genotype]['partial']:
+                scheme[genotype]['partial'][variant_start] = set()
+            scheme[genotype]['partial'][variant_start].add(target_variant)
+
+    for genotype in scheme:
+        for pos in snp_states:
+            allowed_bases = set()
+            if pos in scheme[genotype]['partial']:
+                allowed_bases = allowed_bases | set(scheme[genotype]['partial'][pos])
+            if pos in scheme[genotype]['positive']:
+                allowed_bases = allowed_bases | set(scheme[genotype]['positive'][pos])
+            if len(allowed_bases) == 0:
+                allowed_bases = snp_states[pos]
+            scheme[genotype]['allowed'][pos] = allowed_bases
+
+    features['scheme'] = scheme
+    return features
+
+
+
 def parse_scheme_genotypes(scheme_file):
     scheme = {}
     df = pd.read_csv(scheme_file, sep="\t", header=0, low_memory=False)
-    variant_positions = list(df['variant_start'].unique())
-    geno_seqs = {}
     snp_states = {}
     for row in df.itertuples():
         target_variant = row.target_variant
         variant_start = int(row.variant_start)
         positive_genotypes = row.positive_genotypes
         if isinstance(positive_genotypes,float):
             positive_genotypes = []
@@ -117,226 +193,258 @@
                 allowed_bases = allowed_bases | set(scheme[genotype]['partial'][pos])
             if pos in scheme[genotype]['positive']:
                 allowed_bases = allowed_bases | set(scheme[genotype]['positive'][pos])
             if len(allowed_bases) == 0:
                 allowed_bases = snp_states[pos]
             scheme[genotype]['allowed'][pos] = allowed_bases
 
-
-    genotypes = list(scheme.keys())
-
-    for i in range(0,len(genotypes)):
-        g1 = genotypes[i]
-        a1 = scheme[g1]['allowed']
-        for k in range(i+1,len(genotypes)):
-            g2 = genotypes[k]
-            dist = 0
-            a2 = scheme[g2]['allowed']
-            for pos in a1:
-                int1 = a1[pos] & a2[pos]
-                if len(int1) == 1:
-                    dist+=1
-            if dist == 0:
-                print("{}\t{}\t{}".format(g1,g2,dist))
-
     return scheme
 
 @ray.remote
 def call_genotypes(genotype_rules,metadata,variants,max_dist=0):
     result = {}
     for sample_id in metadata:
-        if not 'genotype' in metadata[sample_id]:
-            continue
+
         if not sample_id in variants:
             continue
-        genotype = metadata[sample_id]['genotype']
+
         result[sample_id] = {
-            'submitted_genotype':genotype,
             'predicted_genotype(s)':[],
-            'predicted_genotype_dist': 1,
-            'genoytpe_results':{},
-            'genoytpe_dists': {}
+            'predicted_genotype_dist': [],
+            'genoytpe_results':[],
+            'genoytpe_dists': {},
+
         }
         genoytpe_results = {}
         dists = {}
         for genotype in genotype_rules:
             genoytpe_results[genotype] = {'match':{},'mismatch':{}}
             dists[genotype] = 1
 
         for pos in variants[sample_id]:
             found_base = set(variants[sample_id][pos])
             if '*' in found_base  or '-' in found_base or 'N' in found_base:
-
                 continue
 
             for genotype in genotype_rules:
                 allowed_bases = genotype_rules[genotype]['allowed'][pos]
 
                 if len(found_base & allowed_bases) == 1:
                     genoytpe_results[genotype]['match'][pos] = found_base
 
                 else:
                     genoytpe_results[genotype]['mismatch'][pos] = found_base
 
-
-
         for genotype in genoytpe_results:
             matches = len(genoytpe_results[genotype]['match'])
             mismatches = len(genoytpe_results[genotype]['mismatch'])
             total = matches + mismatches
             if total > 0:
                 dists[genotype] = 1 - matches /total
 
-
+                
         result[sample_id]['genoytpe_dists'] =  {k: v for k, v in sorted(dists.items(), key=lambda item: item[1])}
+
         pdist = 1
+
         for genotype in result[sample_id]['genoytpe_dists']:
             dist =  result[sample_id]['genoytpe_dists'][genotype]
 
             if dist <= pdist and dist <= max_dist:
                 result[sample_id]['predicted_genotype(s)'].append(genotype)
-                result[sample_id]['predicted_genotype_dist'] = dist
+                result[sample_id]['predicted_genotype_dist'].append(dist)
+                result[sample_id]['genoytpe_results'].append({'match':genoytpe_results[genotype]['match'],
+                                    'mismatch':genoytpe_results[genotype]['mismatch']})
                 pdist = dist
 
-        num_geno = len(result[sample_id]['predicted_genotype(s)'])
-        if num_geno > 1:
-            filt = []
-            for i in range(0,num_geno):
-                is_substring = False
-                for k in range(i+1,num_geno):
-                    if "{}.".format(result[sample_id]['predicted_genotype(s)'][i]) in result[sample_id]['predicted_genotype(s)'][k]:
-                        is_substring = True
-                if not is_substring:
-                    filt.append(result[sample_id]['predicted_genotype(s)'][i])
-            result[sample_id]['predicted_genotype(s)'] = filt
         del result[sample_id]['genoytpe_dists']
 
-        #del result[sample_id]['genoytpe_results']
-        #print("{}\t{}".format(sample_id,time.time() - stime))
     return result
 
+
+def convert_features_to_mutations(feature_lookup,snp_profile):
+    found_features = {
+        'alt':set(),
+        'ref':set()
+    }
+    for pos in snp_profile:
+        if pos not in feature_lookup:
+            continue
+        base = snp_profile[pos]
+        for state in feature_lookup[pos]:
+            if base in feature_lookup[pos][state]:
+                found_features[state].add(feature_lookup[pos][state][base])
+                break
+
+
+    return found_features
+
+
+
+
+
+def write_genotype_calls(header,scheme_name,outfile,genotype_results,sample_metadata,genotype_meta, scheme_data, sample_variants,min_positions=1):
+
+    #get all additional_fields
+    sample_fields = set()
+    for sample_id in sample_metadata:
+        for field in sample_metadata[sample_id]:
+            sample_fields.add(field)
+    sample_fields = sorted(list(sample_fields))
+    genotype_fields = set()
+    for genotype in genotype_meta:
+        for field in genotype_meta[genotype]:
+            genotype_fields.add(field)
+    genotype_fields = sorted(list(genotype_fields))
+    header = header + sample_fields + genotype_fields
+
+    #initialize file
+    fh = open(outfile, 'w')
+    fh.write("{}\n".format("\t".join([str(x) for x in header])))
+
+    analysis_date = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+
+
+    num_positions = scheme_data['num_positions']
+    total_scheme_features = scheme_data['total_scheme_features']
+
+
+    for sample_id in genotype_results:
+        row = {}
+        status = 'Pass'
+        for field_id in header:
+            row[field_id] = ''
+        row['sample_id'] = sample_id
+        row['predicted_genotype'] = '-'
+        row['scheme'] = scheme_name
+        row['analysis_date'] = analysis_date
+        row['total_scheme_features'] = total_scheme_features
+        row['unique_scheme_positions'] = num_positions
+
+        detected_mutations = convert_features_to_mutations(scheme_data['mutation_lookup'],sample_variants[sample_id])
+        row['num_detected_positions'] =  len(detected_mutations['alt'] | detected_mutations['ref'])
+        row['detected_alt_mutations'] = ";".join([str(x) for x in sorted(list(detected_mutations['alt']))])
+
+        for field_id in sample_metadata[sample_id]:
+            row[field_id] = sample_metadata[sample_id][field_id]
+
+        if len(genotype_results[sample_id]['predicted_genotype(s)']) == 1:
+            row['predicted_genotype'] = genotype_results[sample_id]['predicted_genotype(s)'][0]
+            row['predicted_genotype_distance'] = genotype_results[sample_id]['predicted_genotype_dist'][0]
+            genotype = str(row['predicted_genotype'])
+            if genotype in genotype_meta:
+                for field_id in genotype_meta[genotype]:
+                    row[field_id] = genotype_meta[genotype][field_id]
+
+        elif len(genotype_results[sample_id]['predicted_genotype(s)']) > 1:
+            status = 'Warning'
+            row['qc_messages'] = "Ambiguous genotype assignement, possible genotypes: {}".format(";".join([str(x) for x in genotype_results[sample_id]['predicted_genotype(s)']]))
+        else:
+            status = 'Warning'
+            row['qc_messages'] = 'No genotypes were compatible with the sample'
+
+
+        if row['num_detected_positions'] < min_positions:
+            status = 'Fail'
+            row['qc_messages'] = 'Sample is missing too many positions for genotype call'
+
+        row['qc_status'] = status
+        fh.write("{}\n".format("\t".join([str(x) for x in row.values()])))
+
+    fh.close()
+
+def is_valid_file(filename):
+    status = True
+    if not os.path.isfile(filename) or os.path.getsize(filename) <= MIN_FILE_SIZE :
+        status = False
+    return status
+
+
 def run():
     cmd_args = parse_args()
     scheme_file = cmd_args.in_scheme
     variant_file = cmd_args.in_var
-    metadata_file = cmd_args.in_meta
-    prefix = cmd_args.prefix
-    outdir = cmd_args.outdir
+    metadata_file = cmd_args.sample_meta
+    genotype_meta_file = cmd_args.genotype_meta
+    outfile = cmd_args.outfile
     num_threads = cmd_args.num_threads
+    max_missing_positions = cmd_args.max_missing_positions
 
     if not ray.is_initialized():
         ray.init(ignore_reinit_error=True, num_cpus=num_threads)
 
 
     logging = init_console_logger(3)
     logging.info("Starting analysis")
 
-    if not os.path.isdir(outdir):
-        logging.info("Creating temporary analysis directory {}".format(outdir))
-        os.mkdir(outdir, 0o755)
-
     logging.info("Reading metadata file {}".format(metadata_file))
-    metadata = parse_metadata(metadata_file)
+    if not is_valid_file(metadata_file):
+        logging.error("Error file {} was not found or is empty".format(metadata_file))
+        sys.exit()
+    sample_metadata = parse_metadata(metadata_file)
+
+    genotype_metadata = {}
+    if genotype_meta_file is not None:
+        logging.info("Reading metadata file {}".format(genotype_meta_file))
+        if not is_valid_file(genotype_meta_file):
+            logging.error("Error file {} was not found or is empty".format(genotype_meta_file))
+            sys.exit()
+        logging.info("Reading metadata file {}".format(genotype_meta_file))
+        genotype_metadata = parse_metadata(genotype_meta_file,column='key')
 
 
     logging.info("Reading scheme file {}".format(scheme_file))
-    genotype_rules = parse_scheme_genotypes(scheme_file)
+    if not is_valid_file(scheme_file):
+        logging.error("Error file {} was not found or is empty".format(scheme_file))
+        sys.exit()
+
+    scheme_data = parse_scheme_features(scheme_file)
+    genotype_rules = scheme_data['scheme']
+
     for genotype in genotype_rules:
         if len(genotype_rules[genotype]['positive']) == 0:
             logging.warn("Genotype {} has no required kmers".format(genotype))
+
     rule_id = ray.put(genotype_rules)
     num_genotypes = len(genotype_rules)
 
-
     valid_positions = []
     for genotype in genotype_rules:
         for state in genotype_rules[genotype]:
             valid_positions += list(genotype_rules[genotype][state].keys())
     valid_positions = list(set(valid_positions))
+    min_positions = len(valid_positions) -max_missing_positions
 
     logging.info("Extracted {} genotyping positions".format(len(valid_positions)))
-
     logging.info("Reading snp data from vcf file {}".format(variant_file))
     variants = get_snp_profiles(valid_positions, variant_file)
 
-    logging.info("Calling genotypes for {} samples based on {} genotypes".format(len(metadata),num_genotypes))
-    batch_size = int(len(metadata) / num_threads)
+
+    logging.info("Calling genotypes for {} samples based on {} genotypes".format(len(sample_metadata),num_genotypes))
+    batch_size = int(len(sample_metadata) / num_threads)
     ray_results = []
     if batch_size < 1:
         batch_size = 1
     sub_metadata = {}
     sub_variants = {}
-    for sample_id in metadata:
-        sub_metadata[sample_id] = metadata[sample_id]
+    for sample_id in sample_metadata:
+        sub_metadata[sample_id] = sample_metadata[sample_id]
         sub_variants[sample_id] = variants[sample_id]
         if len(sub_metadata) == batch_size:
             ray_results.append(call_genotypes.remote(rule_id, sub_metadata, sub_variants))
             sub_metadata = {}
             sub_variants = {}
     if len(sub_metadata) > 0:
         ray_results.append(call_genotypes.remote(rule_id, sub_metadata, sub_variants))
-        sub_metadata = {}
-        sub_variants = {}
     results = ray.get(ray_results)
-    genoytpe_results = {}
+
+    genotype_results = {}
     for r in results:
         for sample_id in r:
-            genoytpe_results[sample_id] = r[sample_id]
+            genotype_results[sample_id] = r[sample_id]
     del(results)
     del(ray_results)
 
-
-    fh = open(os.path.join(outdir,"{}-scheme.calls.txt".format(prefix)),'w')
-    fh.write("sample_id\tsubmited_genotype\tpredicted_genotype\tis_match\n")
-    for sample_id in genoytpe_results:
-        g = genoytpe_results[sample_id]['submitted_genotype']
-        c = ",".join([str(x) for x in genoytpe_results[sample_id]['predicted_genotype(s)']])
-        m = g == c
-        fh.write("{}\t{}\t{}\t{}\n".format(sample_id, g, c,m))
-
-    logging.info("Calcualting F1 for {} samples".format(len(metadata)))
-    truth = []
-    pred = []
-    group_samples = {}
-    num_ambig = 0
-    num_correct = 0
-    for sample_id in genoytpe_results:
-        genotype = str(genoytpe_results[sample_id]['submitted_genotype'])
-
-        if genotype not in group_samples:
-            group_samples[genotype] = {'truth': [], 'pred': []}
-        pgenotypes = genoytpe_results[sample_id]['predicted_genotype(s)']
-
-        if len(pgenotypes) > 1:
-            num_ambig+=1
-
-        if len(pgenotypes) >= 1 and genotype == str(pgenotypes[0]):
-            pred.append(genotype)
-            group_samples[genotype]['pred'].append(sample_id)
-            num_correct+=1
-        else:
-            pred.append('X')
-        truth.append(genotype)
-        group_samples[genotype]['truth'].append(sample_id)
-
-    scheme_f1 = f1_score(truth,pred,average='micro')
-    fh = open(os.path.join(outdir,"{}-scheme.scores.txt".format(prefix)),'w')
-    fh.write("genotype\tnum_true\tnum_pred\tf1\n")
-    fh.write("overall\t{}\t{}\t{}\n".format(len(metadata),num_correct,scheme_f1))
-    for genotype in group_samples:
-        num_true = len(group_samples[genotype]['truth'])
-        samples = list(set(group_samples[genotype]['truth'] + group_samples[genotype]['pred']))
-        num_samples = len(samples)
-        truth = [0] * num_samples
-        pred = [0] * num_samples
-        for i in range(0,num_samples):
-            sample_id = samples[i]
-            if sample_id in group_samples[genotype]['truth']:
-                truth[i] = 1
-            if sample_id in group_samples[genotype]['pred']:
-                pred[i] = 1
-        geno_f1 = f1_score(truth, pred)
-        fh.write("{}\t{}\t{}\t{}\n".format(genotype,num_true,sum(pred),geno_f1))
-    fh.close()
+    write_genotype_calls(GENOTYPE_REPORT_HEADER, os.path.basename(scheme_file), outfile, genotype_results, sample_metadata, genotype_metadata, scheme_data,variants, min_positions)
 
     logging.info("Analysis complete")
```

### Comparing `cladeomatic-0.1.0/cladeomatic/clades.py` & `cladeomatic-0.1.1/cladeomatic/clades.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/constants.py` & `cladeomatic-0.1.1/cladeomatic/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,35 @@
     'predicted_genotype',
     'predicted_genotype_distance',
     'qc_status',
     'qc_messages',
     'detected_alt_mutations'
 ]
 
+SCHEME_SCORES_REPORT_HEADER = [
+    'label',
+    'scheme',
+    'analysis_date',
+    'num_submitted',
+    'num_predicted',
+    'f1_score',
+]
+
+SCHEME_SAMPLE_REPORT_HEADER = [
+    'sample_id',
+    'scheme',
+    'analysis_date',
+    'submitted_genotype',
+    'predicted_genotype',
+    'is_match',
+    'problem_feature(s)',
+]
+
+
+
 NODE_INFO_HEADER = [
         'clade_id',
         'pos',
         'base',
         'min_dist',
         'max_dist',
         'ave_dist',
```

### Comparing `cladeomatic-0.1.0/cladeomatic/create.py` & `cladeomatic-0.1.1/cladeomatic/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,23 +57,23 @@
     parser.add_argument('--root_name', type=str, required=False, help='Name of sample to root tree', default='')
     parser.add_argument('--root_method', type=str, required=False, help='Method to root tree (midpoint,outgroup)',
                         default=None)
     parser.add_argument('--klen', type=int, required=False, help='kmer length', default=18)
     parser.add_argument('--min_members', type=int, required=False,
                         help='Minimum number of members for a clade to be valid', default=1)
     parser.add_argument('--min_snp_count', type=int, required=False,
-                        help='Minimum number of unique snps for a clade to be valid',
+                        help='Minimum number of unique SNPs for a clade to be valid',
                         default=1)
     parser.add_argument('--max_snp_count', type=int, required=False,
                         help='Maximum number of SNPs to be selected for defining each genotype to prevent large numbers of redundant SNPs',
                         default=-1)
     parser.add_argument('--min_perc', type=float, required=False,
                         help='Minimum percentage of clade members to be positive for a kmer to be valid', default=0.1)
     parser.add_argument('--max_site_ambig', type=float, required=False,
-                        help='Maximum percentage of input sequences which can be mising a site for it to still be valid', default=0.25)
+                        help='Maximum percentage of input sequences which can be missing a site for it to still be valid', default=0.25)
     parser.add_argument('--max_states', type=int, required=False,
                         help='Maximum number of states for a position [A,T,C,G,N,-]',
                         default=6)
     parser.add_argument('--max_ambig', type=int, required=False,
                         help='Maximum number of ambiguous bases allowed in a kmer',
                         default=0)
     parser.add_argument('--rcor_thresh', type=float, required=False, help='Correlation coefficient threshold',
@@ -81,16 +81,16 @@
     parser.add_argument('--delim', type=str, required=False, help='Genotype delimiter in group file',
                         default=None)
     parser.add_argument('--num_threads', type=int, required=False, help='Number of threads to use', default=1)
     parser.add_argument('--no_plots', required=False, help='Disable plotting', action='store_true')
     parser.add_argument('--keep_tmp', required=False, help='Keep interim files', action='store_true')
     parser.add_argument('--debug', required=False, help='Show debug information', action='store_true')
     parser.add_argument('--resume', required=False, help='Resume previous analysis', action='store_true')
-    parser.add_argument('--no_compression', required=False, help='Skip compression of tree heirarchy', action='store_true')
-    parser.add_argument('--force', required=False, help='Force overwite of existing results directory',
+    parser.add_argument('--no_compression', required=False, help='Skip compression of tree hierarchy', action='store_true')
+    parser.add_argument('--force', required=False, help='Force overwrite of existing results directory',
                         action='store_true')
     parser.add_argument('-V', '--version', action='version', version="%(prog)s " + __version__)
 
     return parser.parse_args()
 
 def validate_file(file):
     """
```

### Comparing `cladeomatic-0.1.0/cladeomatic/kmers.py` & `cladeomatic-0.1.1/cladeomatic/kmers.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/main.py` & `cladeomatic-0.1.1/cladeomatic/main.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/namer.py` & `cladeomatic-0.1.1/cladeomatic/namer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,60 @@
 from argparse import (ArgumentParser, ArgumentDefaultsHelpFormatter, RawDescriptionHelpFormatter)
 import pandas as pd
 from cladeomatic.version import __version__
-
+from cladeomatic.utils import parse_metadata
 
 def parse_args():
     class CustomFormatter(ArgumentDefaultsHelpFormatter, RawDescriptionHelpFormatter):
         pass
 
     parser = ArgumentParser(
         description="Clade-O-Matic: Genotyping scheme genotype namer v. {}".format(__version__),
         formatter_class=CustomFormatter)
     parser.add_argument('--in_scheme', type=str, required=True,
                         help='Cladeomatic scheme file')
-    parser.add_argument('--in_names', type=str, required=True, help='Tab delimited file of (genotype, name)', default=None)
+    parser.add_argument('--in_names', type=str, required=True, help='Tab delimited file of (node, name)', default=None)
     parser.add_argument('--outfile', type=str, required=True, help='Output file for updated scheme')
     parser.add_argument('-V', '--version', action='version', version="%(prog)s " + __version__)
 
     return parser.parse_args()
 
-def parse_names(file):
-    '''
-    Parses metadata file into a dict with genotype as the keys
-    :param file: str path to metdata file with 'genotype and name' as a columns
-    :return: dict
-    '''
-    df = pd.read_csv(file, sep="\t", header=0)
-    if not 'genotype' in df.columns.tolist():
-        return {}
-    metadata = {}
-    for index, row in df.iterrows():
-        metadata[row['genotype']] = row['name']
-    return metadata
+
 
 def rename(lookup,queries):
     out = []
     for name in queries:
         if name in lookup:
-            name = lookup[name]
+            name = lookup[name]['name']
         out.append(name)
     return out
 
-def main():
+def run():
     cmd_args = parse_args()
     in_scheme = cmd_args.in_scheme
     in_names = cmd_args.in_names
     outfile = cmd_args.outfile
 
-    names = parse_names(in_names)
+    name_data = parse_metadata(in_names,colum='node')
+
+
     df = pd.read_csv(in_scheme, sep="\t", header=0)
     for index, row in df.iterrows():
         positive_genotypes = row['positive_genotypes']
         if isinstance(positive_genotypes,float):
             positive_genotypes = []
         else:
             positive_genotypes = positive_genotypes.split(',')
-        positive_genotypes = rename(names,positive_genotypes)
+        positive_genotypes = rename(name_data,positive_genotypes)
 
         partial_genotypes = row['partial_genotypes']
         if isinstance(partial_genotypes,float):
             partial_genotypes = []
         else:
             partial_genotypes = partial_genotypes.split(',')
-        partial_genotypes = rename(names, partial_genotypes)
+        partial_genotypes = rename(name_data, partial_genotypes)
         row['positive_genotypes'] = ",".join([str(x) for x in positive_genotypes])
         row['partial_genotypes'] = ",".join([str(x) for x in partial_genotypes])
         df.loc[index, ['positive_genotypes','partial_genotypes']] = [row['positive_genotypes'],row['partial_genotypes']]
 
     df.to_csv(outfile,sep="\t",header=True,index=False)
 
-
-    return
```

### Comparing `cladeomatic-0.1.0/cladeomatic/snps.py` & `cladeomatic-0.1.1/cladeomatic/snps.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/__init__.py` & `cladeomatic-0.1.1/cladeomatic/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,32 +62,32 @@
     Calculates the adjusted rand score between two clusterings
     :param category_1: list - a list of int values for cluster 1
     :param category_2: list - a list of int values for cluster 2
     :return: float - the value of the ARI score for the two clusters
     """
     return adjusted_rand_score(category_1, category_2)
 
-def parse_metadata(file):
+def parse_metadata(file,column='sample_id'):
     """
     Parses the metadata file into a dictionary with sample ids as the keys.
     Will dynamically add the other columns and values to the dictionary
     :param file: string - path to tsv metadata file with 'sample_id' as a
     mandatory column
     :return: dictionary - a dictionary of the parsed metadata values organized
     wtih the sample id as a key
     """
     #read the file into a pandas datafram
     df = pd.read_csv(file, sep="\t", header=0)
-    if not 'sample_id' in df.columns.tolist():
+    if not column in df.columns.tolist():
         return {}
-    columns = set(df.columns.tolist()) - set('sample_id')
+    columns = set(df.columns.tolist()) - set(column)
     metadata = {}
     for index, row in df.iterrows():
-        metadata[row['sample_id']] = {}
+        metadata[str(row[column])] = {}
         #parse out any additional columns and their row values
         for field in columns:
             field = str(field)
-            if field == 'sample_id':
+            if field == column:
                 continue
             value = str(row[field])
-            metadata[row['sample_id']][field] = value
+            metadata[str(row[column])][field] = value
     return metadata
```

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/jellyfish.py` & `cladeomatic-0.1.1/cladeomatic/utils/jellyfish.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/kmerSearch.py` & `cladeomatic-0.1.1/cladeomatic/utils/kmerSearch.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/phylo_tree.py` & `cladeomatic-0.1.1/cladeomatic/utils/phylo_tree.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/seqdata.py` & `cladeomatic-0.1.1/cladeomatic/utils/seqdata.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/snpdists.py` & `cladeomatic-0.1.1/cladeomatic/utils/snpdists.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/vcfhelper.py` & `cladeomatic-0.1.1/cladeomatic/utils/vcfhelper.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/utils/visualization.py` & `cladeomatic-0.1.1/cladeomatic/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/visualize.py` & `cladeomatic-0.1.1/cladeomatic/visualize.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic/writers.py` & `cladeomatic-0.1.1/cladeomatic/writers.py`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/cladeomatic.egg-info/PKG-INFO` & `cladeomatic-0.1.1/cladeomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cladeomatic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Clade-O-Matic: Automatic recognition of population structures based on canonical SNPs
 Home-page: https://github.com/phac-nml/cladeomaticc
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Keywords: Genotyping,population structure,kmer
 Classifier: Development Status :: 3 - Alpha
@@ -14,9 +14,9 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8.0,<4
+Requires-Python: >=3.9.0,<4
 License-File: LICENSE
```

### Comparing `cladeomatic-0.1.0/cladeomatic.egg-info/SOURCES.txt` & `cladeomatic-0.1.1/cladeomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.1.0/setup.py` & `cladeomatic-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 exec(open('cladeomatic/version.py').read())
 
 setup(
     name='cladeomatic',
     include_package_data=True,
     version=__version__,
-    python_requires='>=3.8.0,<4',
+    python_requires='>=3.9.0,<4',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     packages=find_packages(exclude=['tests']),
     url='https://github.com/phac-nml/cladeomaticc',
     license='GPLv3',
     author='James Robertson',
     author_email='james.robertson@phac-aspc.gc.ca',
@@ -44,32 +44,31 @@
     classifiers=classifiers,
     package_dir={'cladeomatic': 'cladeomatic'},
     package_data={
         "": ["*.txt", "*.fasta","*.html","*.gb"],
     },
 
     install_requires=[
-        'numpy==1.23.0',
-        'pandas==2.0.1',
-        'biopython==1.81',
-        'six==1.16.0',
-        'matplotlib==3.7.1',
-        'argparse==1.4.0',
-        'statistics==1.0.3.5',
-        'plotly==5.14.1',
+        'numpy>=1.23.0',
+        'pandas>=2.0.1',
+        'biopython>=1.81',
+        'six>=1.16.0',
+        'matplotlib>=3.7.1',
+        'statistics>=1.0.3.5',
+        'plotly>=5.14.1',
         'ete3==3.1.2',
-        'jellyfish==0.9.0',
+        'jellyfish',
         'DendroPy==4.5.2',
-        'PyQt5==5.15.9',
-        'ray==2.3.1',
-        'deprecated==1.2.13',
+        'ray>=2.3.1',
+        'deprecated>=1.2.13',
         'psutil==5.9.1',
-        'scikit-learn==1.1.1',
-        'scipy==1.10.1',
-        'pyahocorasick==1.4.4',
+        'scikit-learn>=1.1.1',
+        'scipy>=1.10.1',
+        'pyahocorasick>=1.4.4',
+        'PyQt5'
 
     ],
 
     entry_points={
         'console_scripts': [
             'cladeomatic=cladeomatic.main:main',
         ],
```


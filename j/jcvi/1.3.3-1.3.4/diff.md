# Comparing `tmp/jcvi-1.3.3.tar.gz` & `tmp/jcvi-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.3.3.tar", last modified: Fri Feb 17 10:13:36 2023, max compression
+gzip compressed data, was "jcvi-1.3.4.tar", last modified: Thu Apr 27 08:18:35 2023, max compression
```

## Comparing `jcvi-1.3.3.tar` & `jcvi-1.3.4.tar`

### file list

```diff
@@ -1,214 +1,215 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.716559 jcvi-1.3.3/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.3/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.3/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8739 2023-02-17 10:13:36.716673 jcvi-1.3.3/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.3/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.677381 jcvi-1.3.3/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.3/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.680505 jcvi-1.3.3/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.3/jcvi/algorithms/maxsum.py
--rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/ml.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.3/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.682381 jcvi-1.3.3/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.688408 jcvi-1.3.3/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16407 2023-02-17 09:58:57.000000 jcvi-1.3.3/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    67826 2023-02-17 08:59:11.000000 jcvi-1.3.3/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.3/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18480 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/grid.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/ks.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/apps/script.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.693743 jcvi-1.3.3/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.3/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-17 08:59:49.000000 jcvi-1.3.3/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    39860 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16153 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.695637 jcvi-1.3.3/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/compara/__main__.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9811 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    27158 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)     9199 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7931 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10324 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    61622 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.700446 jcvi-1.3.3/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    72552 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    41254 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.3/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.3/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.3/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.705509 jcvi-1.3.3/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    21825 2023-02-17 09:02:17.000000 jcvi-1.3.3/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.3/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14847 2023-02-17 09:00:39.000000 jcvi-1.3.3/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.3/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/grabseeds.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/graphics/graph.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.3/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.3/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/graphics/logo.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.3/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.3/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.3/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/graphics/wheel.py
--rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.3/jcvi/graphics/whisker.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.709179 jcvi-1.3.3/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/alfalfa.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/heterosis.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.3/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/pistachio.py
--rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    19735 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11915 2021-06-19 19:45:56.000000 jcvi-1.3.3/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.712080 jcvi-1.3.3/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.3/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.714830 jcvi-1.3.3/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.3/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.3/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.3/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.716427 jcvi-1.3.3/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.3/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.3/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.3/jcvi/variation/tassel.py
--rw-r--r--   0 bao        (501) staff       (20)      160 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-02-17 10:13:36.678311 jcvi-1.3.3/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8739 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4706 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.3/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      206 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2023-02-17 10:13:36.000000 jcvi-1.3.3/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.3/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1219 2023-02-17 10:13:36.717109 jcvi-1.3.3/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.3/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.621805 jcvi-1.3.4/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.4/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.4/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-04-27 08:18:35.621885 jcvi-1.3.4/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.4/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.589952 jcvi-1.3.4/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.4/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.592869 jcvi-1.3.4/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/algorithms/maxsum.py
+-rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/ml.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.4/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.594583 jcvi-1.3.4/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/train.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.598898 jcvi-1.3.4/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.3.4/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    68248 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18480 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/grid.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/ks.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/apps/script.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.602596 jcvi-1.3.4/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/ca.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.4/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.3.4/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    39860 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/assembly/syntenypath.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.604653 jcvi-1.3.4/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4210 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    27413 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.609323 jcvi-1.3.4/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    72552 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    42610 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.4/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.4/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.4/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.613548 jcvi-1.3.4/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    22166 2023-02-23 05:35:25.000000 jcvi-1.3.4/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/grabseeds.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/graph.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.4/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.4/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/logo.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.4/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.4/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/wheel.py
+-rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.4/jcvi/graphics/whisker.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.616232 jcvi-1.3.4/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/alfalfa.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/heterosis.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/pistachio.py
+-rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    26165 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.618577 jcvi-1.3.4/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.4/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.620394 jcvi-1.3.4/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.4/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.4/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.4/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.621681 jcvi-1.3.4/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/tassel.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.590801 jcvi-1.3.4/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4727 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.4/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      206 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.4/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1219 2023-04-27 08:18:35.622240 jcvi-1.3.4/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.4/setup.py
```

### Comparing `jcvi-1.3.3/LICENSE` & `jcvi-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/PKG-INFO` & `jcvi-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
@@ -216,7 +217,9 @@
 python -m jcvi.formats.fasta extract
 ```
 
 This will tell you the options and arguments it expects.
 
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
+
+
```

### Comparing `jcvi-1.3.3/README.md` & `jcvi-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/__init__.py` & `jcvi-1.3.4/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/ec.py` & `jcvi-1.3.4/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/formula.py` & `jcvi-1.3.4/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/graph.py` & `jcvi-1.3.4/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/lis.py` & `jcvi-1.3.4/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/lpsolve.py` & `jcvi-1.3.4/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/matrix.py` & `jcvi-1.3.4/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/maxsum.py` & `jcvi-1.3.4/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/ml.py` & `jcvi-1.3.4/jcvi/algorithms/ml.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/supermap.py` & `jcvi-1.3.4/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/algorithms/tsp.py` & `jcvi-1.3.4/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/ahrd.py` & `jcvi-1.3.4/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/automaton.py` & `jcvi-1.3.4/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/depth.py` & `jcvi-1.3.4/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/evm.py` & `jcvi-1.3.4/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/maker.py` & `jcvi-1.3.4/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/pasa.py` & `jcvi-1.3.4/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/qc.py` & `jcvi-1.3.4/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/reformat.py` & `jcvi-1.3.4/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/stats.py` & `jcvi-1.3.4/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/annotation/train.py` & `jcvi-1.3.4/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/align.py` & `jcvi-1.3.4/jcvi/apps/align.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 same and does parallelization both in core and on grid.
 """
 import os.path as op
 import sys
 import shutil
 import logging
 
-from subprocess import CalledProcessError
+from subprocess import CalledProcessError, STDOUT
 
 from jcvi.utils.cbook import depends
 from jcvi.apps.base import (
     ActionDispatcher,
     OptionParser,
     cleanup,
     get_abs_path,
@@ -554,20 +554,36 @@
         extra += " -r1 -q{0} -a{0} -b{0}".format(mm)
     if extra:
         cmd += " " + extra.strip()
 
     lastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
     # Make several attempts to run LASTAL
     try:
-        sh(cmd + f" -P {cpus} {subjectdb} {query}", outfile=lastfile, check=True)
-    except CalledProcessError:  # multi-threading disabled
-        logging.error("Failed to run `lastal` with multi-threading. Trying again.")
+        sh(
+            cmd + f" -P {cpus} {subjectdb} {query}",
+            outfile=lastfile,
+            check=True,
+            redirect_error=STDOUT,
+        )
+    except CalledProcessError as e:  # multi-threading disabled
+        message = "lastal failed with message:"
+        message += "\n{0}".format(e.output.decode())
+        logging.error(message)
         try:
-            sh(cmd + f" -P 1 {subjectdb} {query}", outfile=lastfile, check=True)
-        except CalledProcessError:
+            logging.debug("Failed to run `lastal` with multi-threading. Trying again.")
+            sh(
+                cmd + f" -P 1 {subjectdb} {query}",
+                outfile=lastfile,
+                check=True,
+                redirect_error=STDOUT,
+            )
+        except CalledProcessError as e:
+            message = "lastal failed with message:"
+            message += "\n{0}".format(e.output.decode())
+            logging.error(message)
             logging.fatal("Failed to run `lastal`. Aborted.")
             cleanup(lastfile)
             sys.exit(1)
     return lastfile
 
 
 if __name__ == "__main__":
```

### Comparing `jcvi-1.3.3/jcvi/apps/base.py` & `jcvi-1.3.4/jcvi/apps/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ConfigParser,
     RawConfigParser,
     NoOptionError,
     NoSectionError,
     ParsingError,
 )
 from socket import gethostname
-from subprocess import PIPE, call, check_call
+from subprocess import PIPE, call, check_output
 from optparse import OptionParser as OptionP, OptionGroup, SUPPRESS_HELP
 from typing import Any, Collection, List, Optional, Union
 
 from natsort import natsorted
 from rich.logging import Console, RichHandler
 
 from jcvi import __copyright__, __version__
@@ -449,15 +449,15 @@
         compreh_pctid=None,
         compreh_pctcov=None,
         intron=None,
         bpsplice=None,
     ):
         if pctid is not None:
             self.add_option(
-                "--pctid", default=pctid, type="int", help="Sequence percent identity"
+                "--pctid", default=pctid, type="float", help="Sequence percent identity"
             )
         if hitlen is not None:
             self.add_option(
                 "--hitlen", default=hitlen, type="int", help="Minimum overlap length"
             )
         if pctcov is not None:
             self.add_option(
@@ -584,14 +584,23 @@
 
         opts, args = self.parse_args(args)
 
         assert opts.dpi > 0
         assert "x" in opts.figsize
 
         iopts = ImageOptions(opts)
+
+        if opts.notex:
+            logging.info("--notex={}. latex use is disabled.".format(opts.notex))
+        elif not is_tex_available():
+            if not bool(which("latex")):
+                logging.info("`latex` not found. latex use is disabled.")
+            if not bool(which("lp")):
+                logging.info("`lp` not found. latex use is disabled.")
+
         setup_theme(style=opts.style, font=opts.font, usetex=iopts.usetex)
 
         return opts, args, iopts
 
     def set_dotplot_opts(self, theme: int = 2) -> OptionGroup:
         """Used in compara.catalog and graphics.dotplot"""
         from jcvi.graphics.base import set1
@@ -1136,14 +1145,15 @@
     background=False,
     threaded=None,
     log=True,
     grid_opts=None,
     silent=False,
     shell="/bin/bash",
     check=False,
+    redirect_error=None,
 ):
     """
     simple wrapper for system calls
     """
     if not cmd:
         return 1
     if silent:
@@ -1180,16 +1190,16 @@
             cmd += " 2>{0}".format(errfile)
         if background:
             cmd += " &"
 
         if log:
             logging.debug(cmd)
 
-        call_func = check_call if check else call
-        return call_func(cmd, shell=True, executable=shell)
+        call_func = check_output if check else call
+        return call_func(cmd, shell=True, executable=shell, stderr=redirect_error)
 
 
 def Popen(cmd, stdin=None, stdout=PIPE, debug=False, shell="/bin/bash"):
     """
     Capture the cmd stdout output to a file handle.
     """
     from subprocess import Popen as P
```

### Comparing `jcvi-1.3.3/jcvi/apps/biomart.py` & `jcvi-1.3.4/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/blastplus.py` & `jcvi-1.3.4/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/bowtie.py` & `jcvi-1.3.4/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/bwa.py` & `jcvi-1.3.4/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/cdhit.py` & `jcvi-1.3.4/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/emboss.py` & `jcvi-1.3.4/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/fetch.py` & `jcvi-1.3.4/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/gbsubmit.py` & `jcvi-1.3.4/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/gmap.py` & `jcvi-1.3.4/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/grid.py` & `jcvi-1.3.4/jcvi/apps/grid.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/ks.py` & `jcvi-1.3.4/jcvi/apps/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/lastz.py` & `jcvi-1.3.4/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/mask.py` & `jcvi-1.3.4/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/phylo.py` & `jcvi-1.3.4/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/r.py` & `jcvi-1.3.4/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/restriction.py` & `jcvi-1.3.4/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/script.py` & `jcvi-1.3.4/jcvi/apps/script.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/softlink.py` & `jcvi-1.3.4/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/uclust.py` & `jcvi-1.3.4/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/uniprot.py` & `jcvi-1.3.4/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/apps/vecscreen.py` & `jcvi-1.3.4/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/allmaps.py` & `jcvi-1.3.4/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/allpaths.py` & `jcvi-1.3.4/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/automaton.py` & `jcvi-1.3.4/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/base.py` & `jcvi-1.3.4/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/ca.py` & `jcvi-1.3.4/jcvi/assembly/ca.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/chic.pyx` & `jcvi-1.3.4/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/coverage.py` & `jcvi-1.3.4/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/gaps.py` & `jcvi-1.3.4/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/geneticmap.py` & `jcvi-1.3.4/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/goldenpath.py` & `jcvi-1.3.4/jcvi/assembly/goldenpath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/hic.py` & `jcvi-1.3.4/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/kmer.py` & `jcvi-1.3.4/jcvi/assembly/kmer.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/opticalmap.py` & `jcvi-1.3.4/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/patch.py` & `jcvi-1.3.4/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/postprocess.py` & `jcvi-1.3.4/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/preprocess.py` & `jcvi-1.3.4/jcvi/assembly/preprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/sim.py` & `jcvi-1.3.4/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/soap.py` & `jcvi-1.3.4/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/assembly/syntenypath.py` & `jcvi-1.3.4/jcvi/assembly/syntenypath.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,17 +124,18 @@
 def bed(args):
     """
     %prog bed anchorsfile
 
     Convert ANCHORS file to BED format.
     """
     from collections import defaultdict
-    from jcvi.compara.synteny import AnchorFile, check_beds
+    from jcvi.compara.synteny import check_beds
     from jcvi.formats.bed import Bed
     from jcvi.formats.base import get_number
+    from ..compara.base import AnchorFile
 
     p = OptionParser(bed.__doc__)
     p.add_option(
         "--switch",
         default=False,
         action="store_true",
         help="Switch reference and aligned map elements",
```

### Comparing `jcvi-1.3.3/jcvi/assembly/trinity.py` & `jcvi-1.3.4/jcvi/assembly/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/compara/blastfilter.py` & `jcvi-1.3.4/jcvi/compara/blastfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 def filter_exclude(blast_list, exclude=None):
     """Filter gene pairs from an excluded list
 
     Args:
         blast_list (List[BlastLine]): List of BlastLines
         exclude (str, optional): Path to the excluded anchors file. Defaults to None.
     """
-    from jcvi.compara.synteny import AnchorFile
+    from .base import AnchorFile
 
     excluded_pairs = set()
     ac = AnchorFile(exclude)
     for a, b, block in ac.iter_pairs():
         excluded_pairs.add((a, b))
         excluded_pairs.add((b, a))
     for b in blast_list:
```

### Comparing `jcvi-1.3.3/jcvi/compara/catalog.py` & `jcvi-1.3.4/jcvi/compara/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 
 from jcvi.formats.blast import BlastLine
 from jcvi.formats.fasta import Fasta
 from jcvi.formats.bed import Bed
 from jcvi.formats.base import must_open, BaseFile
 from jcvi.utils.grouper import Grouper
 from jcvi.utils.cbook import gene_name
-from jcvi.compara.synteny import AnchorFile, check_beds
 from jcvi.apps.base import (
     OptionParser,
     glob,
     ActionDispatcher,
     need_update,
     sh,
     mkdir,
 )
+from .base import AnchorFile
+from .synteny import check_beds
 
 
 class OMGFile(BaseFile):
     def __init__(self, filename):
         super(OMGFile, self).__init__(filename)
         fp = open(filename)
         inblock = False
@@ -638,14 +639,20 @@
         type="int",
         default=4,
         help="minimum number of anchors in a cluster",
     )
     p.add_option("--quota", help="Quota align parameter")
     p.add_option("--exclude", help="Remove anchors from a previous run")
     p.add_option(
+        "--self_remove",
+        default=98,
+        type="float",
+        help="Remove self hits that are above this percent identity",
+    )
+    p.add_option(
         "--no_strip_names",
         default=False,
         action="store_true",
         help="Do not strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
     )
     p.add_option(
         "--liftover_dist",
@@ -682,18 +689,21 @@
     bprefix = op.basename(b)
     pprefix = ".".join((aprefix, bprefix))
     qprefix = ".".join((bprefix, aprefix))
     last = pprefix + ".last"
     if need_update((afasta, bfasta), last, warn=True):
         last_main([bfasta, afasta, cpus_flag], dbtype)
 
+    self_remove = opts.self_remove
     if a == b:
-        lastself = last + ".P98L0.inverse"
+        lastself = last + f".P{self_remove}L0.inverse"
         if need_update(last, lastself, warn=True):
-            filter([last, "--hitlen=0", "--pctid=98", "--inverse", "--noself"])
+            filter(
+                [last, "--hitlen=0", f"--pctid={self_remove}", "--inverse", "--noself"]
+            )
         last = lastself
 
     filtered_last = last + ".filtered"
     if need_update(last, filtered_last, warn=True):
         # If we are doing filtering based on another file then we don't run cscore anymore
         dargs = [last, "--cscore={}".format(ccscore)]
         if exclude:
```

### Comparing `jcvi-1.3.3/jcvi/compara/fractionation.py` & `jcvi-1.3.4/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/compara/pad.py` & `jcvi-1.3.4/jcvi/compara/pad.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 import sys
 import logging
 from math import log
 
 import numpy as np
 from more_itertools import pairwise
 
-from jcvi.compara.synteny import AnchorFile, check_beds
+from jcvi.compara.synteny import check_beds
 from jcvi.formats.bed import Bed
 from jcvi.formats.blast import BlastLine
 from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from .base import AnchorFile
 
 
 def main():
 
     actions = (
         ("cluster", "cluster the segments"),
         ("pad", "test and reconstruct candidate PADs"),
```

### Comparing `jcvi-1.3.3/jcvi/compara/phylogeny.py` & `jcvi-1.3.4/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/compara/quota.py` & `jcvi-1.3.4/jcvi/compara/quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 """
 
 import logging
 import os.path as op
 import sys
 
 from jcvi.algorithms.lpsolve import MIPDataModel
-from jcvi.compara.synteny import AnchorFile, _score, check_beds
+from jcvi.compara.synteny import _score, check_beds
 from jcvi.formats.base import must_open
 from jcvi.apps.base import OptionParser
+from .base import AnchorFile
 
 
 def get_1D_overlap(eclusters, depth=1):
     """
     Find blocks that are 1D overlapping,
     returns cliques of block ids that are in conflict
     """
```

### Comparing `jcvi-1.3.3/jcvi/compara/reconstruct.py` & `jcvi-1.3.4/jcvi/compara/reconstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import sys
 import logging
 
 from itertools import zip_longest
 from math import sqrt
 from more_itertools import pairwise
 
-from jcvi.compara.synteny import AnchorFile, check_beds
+from jcvi.compara.synteny import check_beds
 from jcvi.formats.base import get_number
 from jcvi.formats.bed import Bed
 from jcvi.utils.grouper import Grouper
 from jcvi.apps.base import OptionParser, ActionDispatcher
+from .base import AnchorFile
 
 
 def main():
 
     actions = (
         ("collinear", "reduce synteny blocks to strictly collinear"),
         ("zipbed", "build ancestral contig from collinear blocks"),
```

### Comparing `jcvi-1.3.3/jcvi/compara/synfind.py` & `jcvi-1.3.4/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/compara/synteny.py` & `jcvi-1.3.4/jcvi/compara/synteny.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,123 +15,17 @@
 
 from jcvi.algorithms.lis import heaviest_increasing_subsequence as his
 from jcvi.formats.bed import Bed, BedLine
 from jcvi.formats.blast import Blast
 from jcvi.formats.base import BaseFile, SetFile, read_block, must_open
 from jcvi.utils.grouper import Grouper
 from jcvi.utils.cbook import gene_name, human_size
-from jcvi.utils.range import Range, range_chain
+from jcvi.utils.range import range_chain
 from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup
-
-
-class AnchorFile(BaseFile):
-    def __init__(self, filename, minsize=0):
-        super(AnchorFile, self).__init__(filename)
-        self.blocks = list(self.iter_blocks(minsize=minsize))
-
-    def iter_blocks(self, minsize=0):
-        fp = open(self.filename)
-        for _, lines in read_block(fp, "#"):
-            lines = [x.split() for x in lines]
-            if len(lines) >= minsize:
-                yield lines
-
-    def iter_pairs(self, minsize=0):
-        block_id = -1
-        for rows in self.iter_blocks(minsize=minsize):
-            block_id += 1
-            for row in rows:
-                a, b = row[:2]
-                yield a, b, block_id
-
-    def make_ranges(self, order, clip=10):
-        """Prepare anchors information into a set of ranges for chaining"""
-        ranges = []
-        block_pairs = defaultdict(dict)
-        blocks = self.blocks
-        for i, ib in enumerate(blocks):
-            q, s, t = zip(*ib)
-            if q[0] not in order:
-                q, s = s, q
-
-            r = make_range(q, s, t, i, order, block_pairs, clip=clip)
-            ranges.append(r)
-
-            assert q[0] in order
-            if s[0] not in order:
-                continue
-
-            # is_self comparison
-            q, s = s, q
-            r = make_range(q, s, t, i, order, block_pairs, clip=clip)
-            ranges.append(r)
-        return ranges, block_pairs
-
-    def print_to_file(self, filename="stdout", accepted=None):
-        fw = must_open(filename, "w")
-        blocks = self.blocks
-        nremoved = 0
-        ncorrected = 0
-        for block in blocks:
-            print("###", file=fw)
-            for line in block:
-                a, b, score = line
-                pair = (a, b)
-                if accepted:
-                    if pair not in accepted:
-                        nremoved += 1
-                        continue
-                    av = accepted[pair]
-                    if score != av and score != av + "L":
-                        score = av
-                        ncorrected += 1
-                print("\t".join((a, b, score)), file=fw)
-        fw.close()
-
-        logging.debug("Removed %d existing anchors.", nremoved)
-        logging.debug("Corrected scores for %d anchors.", ncorrected)
-        logging.debug("Anchors written to `%s`.", filename)
-
-    def blast(self, blastfile=None, outfile=None):
-        """
-        convert anchor file to 12 col blast file
-        """
-        from jcvi.formats.blast import BlastSlow, BlastLineByConversion
-
-        if not outfile:
-            outfile = self.filename + ".blast"
-
-        if blastfile is not None:
-            blasts = BlastSlow(blastfile).to_dict()
-        else:
-            blasts = None
-
-        fw = must_open(outfile, "w", checkexists=True)
-        nlines = 0
-        for a, b, _ in self.iter_pairs():
-            if (a, b) in blasts:
-                bline = blasts[(a, b)]
-            elif (b, a) in blasts:
-                bline = blasts[(b, a)]
-            else:
-                line = "\t".join((a, b))
-                bline = BlastLineByConversion(line, mode="110000000000")
-
-            print(bline, file=fw)
-            nlines += 1
-        fw.close()
-
-        logging.debug("A total of %d BLAST lines written to `%s`.", nlines, outfile)
-
-        return outfile
-
-    @property
-    def is_empty(self):
-        blocks = self.blocks
-        return not blocks or not blocks[0]
+from .base import AnchorFile
 
 
 class BlockFile(BaseFile):
     """Parse .blocks file which is the mcscan output with multiple columns as 'tracks'"""
 
     def __init__(self, filename, defaultcolor="#fb8072", header=False):
         super(BlockFile, self).__init__(filename)
@@ -1544,42 +1438,14 @@
     print(file=sys.stderr)
     print(
         "Orthologous matches: {0}".format(percentage(orthologous, matches)),
         file=sys.stderr,
     )
 
 
-def get_best_pair(qs, ss, ts):
-    pairs = {}
-    for q, s, t in zip(qs, ss, ts):
-        t = int(t[:-1]) if t[-1] == "L" else int(t)
-        if q not in pairs or pairs[q][1] < t:
-            pairs[q] = (s, t)
-
-    # Discard score
-    spairs = dict((q, s) for q, (s, t) in pairs.items())
-    return spairs
-
-
-def make_range(q, s, t, i, order, block_pairs, clip=10):
-    pairs = get_best_pair(q, s, t)
-    score = len(pairs)
-    block_pairs[i].update(pairs)
-
-    q = [order[x][0] for x in q]
-    q.sort()
-    qmin = q[0]
-    qmax = q[-1]
-    if qmax - qmin >= 2 * clip:
-        qmin += clip / 2
-        qmax -= clip / 2
-
-    return Range("0", qmin, qmax, score=score, id=i)
-
-
 def mcscan(args):
     """
     %prog mcscan bedfile anchorfile [options]
 
     Stack synteny blocks on a reference bed, MCSCAN style. The first column in
     the output is the reference order, given in the bedfile. Then each column
     next to it are separate 'tracks'.
```

### Comparing `jcvi-1.3.3/jcvi/formats/agp.py` & `jcvi-1.3.4/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/base.py` & `jcvi-1.3.4/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/bed.py` & `jcvi-1.3.4/jcvi/formats/bed.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/blast.py` & `jcvi-1.3.4/jcvi/formats/blast.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from jcvi.formats.sizes import Sizes
 from jcvi.utils.grouper import Grouper
 from jcvi.utils.orderedcollections import OrderedDict
 from jcvi.utils.range import range_distance
 from jcvi.utils.cbook import percentage
 from jcvi.assembly.base import calculate_A50
 from jcvi.apps.base import OptionParser, ActionDispatcher, sh, popen
+from ..compara.base import AnchorFile
 
 
 try:
     from .cblast import BlastLine
 except:
     from .pyblast import BlastLine
 
@@ -317,17 +318,15 @@
         opts.score,
         opts.pctid,
         opts.hitlen,
         opts.evalue,
         opts.noself,
     )
     newblastfile = (
-        blastfile + ".P{0}L{1}".format(int(pctid), hitlen)
-        if outfile is None
-        else outfile
+        blastfile + ".P{0}L{1}".format(pctid, hitlen) if outfile is None else outfile
     )
     if inverse:
         newblastfile += ".inverse"
     fw = must_open(newblastfile, "w")
     for row in fp:
         if row[0] == "#":
             continue
@@ -369,14 +368,15 @@
         ("completeness", "print completeness statistics for each query"),
         ("annotation", "create tabular file with the annotations"),
         ("top10", "count the most frequent 10 hits"),
         ("filter", "filter BLAST file (based on score, id%, alignlen)"),
         ("covfilter", "filter BLAST file (based on id% and cov%)"),
         ("cscore", "calculate C-score for BLAST pairs"),
         ("best", "get best BLAST hit per query"),
+        ("anchors", "keep only the BLAST pairs that are in the anchors file"),
         ("pairs", "print paired-end reads of BLAST tabular file"),
         ("bed", "get bed file from BLAST tabular file"),
         ("condense", "group HSPs together for same query-subject pair"),
         ("chain", "chain adjacent HSPs together"),
         ("swap", "swap query and subjects in BLAST tabular file"),
         ("sort", "sort lines so that query grouped together and scores desc"),
         ("subset", "extract hits from some query and subject chrs"),
@@ -1313,14 +1313,50 @@
     (blastfile,) = targs
     bedfile = bed([blastfile])
     args[args.index(blastfile)] = bedfile
 
     return jcvi.formats.bed.pairs(args)
 
 
+def anchors(args):
+    """
+    %prog anchors blastfile anchorsfile
+
+    Extract a subset of the BLAST file based on the anchors file. The anchors
+    file is a tab-delimited file with two columns, likely generated from synteny
+    pipeline. This is useful to filter down BLAST.
+    """
+    p = OptionParser(anchors.__doc__)
+    p.set_outfile()
+    p.add_option(
+        "--best", default=False, action="store_true", help="Keep only the best hit"
+    )
+    opts, args = p.parse_args(args)
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    blastfile, anchorsfile = args
+    anchor_file = AnchorFile(anchorsfile)
+    anchor_pairs = set((a, b) for a, b, _ in anchor_file.iter_pairs())
+    blast = Blast(blastfile)
+    found, total = 0, 0
+    fw = must_open(opts.outfile, "w")
+    seen = set()
+    for rec in blast:
+        pp = (rec.query, rec.subject)
+        if pp in anchor_pairs:
+            found += 1
+            if opts.best and pp in seen:
+                continue
+            print(rec, file=fw)
+            seen.add(pp)
+        total += 1
+    logging.info("Found %s", percentage(found, total))
+
+
 def best(args):
     """
     %prog best blastfile
 
     print the best hit for each query in the blastfile
     """
     p = OptionParser(best.__doc__)
@@ -1381,14 +1417,18 @@
 
 def summary(args):
     """
     %prog summary blastfile
 
     Provide summary on id% and cov%, for both query and reference. Often used in
     comparing genomes (based on NUCMER results).
+
+    Columns:
+    filename, identicals, qrycovered, pct_qrycovered, refcovered, pct_refcovered,
+    qryspan, pct_qryspan, refspan, pct_refspan
     """
     p = OptionParser(summary.__doc__)
     p.add_option(
         "--strict",
         default=False,
         action="store_true",
         help="Strict 'gapless' mode. Exclude gaps from covered base.",
```

### Comparing `jcvi-1.3.3/jcvi/formats/cblast.pyx` & `jcvi-1.3.4/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/cdt.py` & `jcvi-1.3.4/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/chain.py` & `jcvi-1.3.4/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/contig.py` & `jcvi-1.3.4/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/coords.py` & `jcvi-1.3.4/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/excel.py` & `jcvi-1.3.4/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/fasta.py` & `jcvi-1.3.4/jcvi/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/fastq.py` & `jcvi-1.3.4/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/genbank.py` & `jcvi-1.3.4/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/gff.py` & `jcvi-1.3.4/jcvi/formats/gff.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/html.py` & `jcvi-1.3.4/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/maf.py` & `jcvi-1.3.4/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/obo.py` & `jcvi-1.3.4/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/paf.py` & `jcvi-1.3.4/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/pdf.py` & `jcvi-1.3.4/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/psl.py` & `jcvi-1.3.4/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/pyblast.py` & `jcvi-1.3.4/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/sam.py` & `jcvi-1.3.4/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/sizes.py` & `jcvi-1.3.4/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/formats/vcf.py` & `jcvi-1.3.4/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/align.py` & `jcvi-1.3.4/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/assembly.py` & `jcvi-1.3.4/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/base.py` & `jcvi-1.3.4/jcvi/graphics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import copy
 import os.path as op
+from os import remove
 import sys
 import logging
 
 logging.getLogger("matplotlib").setLevel(logging.WARNING)
 logging.getLogger("numexpr").setLevel(logging.WARNING)
 logging.getLogger("PIL").setLevel(logging.INFO)
 
@@ -310,21 +311,27 @@
 
 def savefig(figname, dpi=150, iopts=None, cleanup=True):
     try:
         format = figname.rsplit(".", 1)[-1].lower()
     except:
         format = "pdf"
     try:
+        logging.debug(f"Matplotlib backend is: {mpl.get_backend()}")
+        logging.debug(f"Attempting save as: {figname}")
         plt.savefig(figname, dpi=dpi, format=format)
     except Exception as e:
-        message = "savefig failed. Reset usetex to False."
+        message = "savefig failed with message:"
         message += "\n{0}".format(str(e))
-        logging.info(message)
-        rc("text", usetex=False)
-        plt.savefig(figname, dpi=dpi)
+        logging.error(message)
+        logging.info("Try running again with --notex option to disable latex.")
+        if op.exists(figname):
+            if op.getsize(figname) < 1000:
+                logging.debug(f"Cleaning up empty file: {figname}")
+                remove(figname)
+        sys.exit(1)
 
     msg = "Figure saved to `{0}`".format(figname)
     if iopts:
         msg += " {0}".format(iopts)
     logging.debug(msg)
 
     if cleanup:
```

### Comparing `jcvi-1.3.3/jcvi/graphics/blastplot.py` & `jcvi-1.3.4/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/chromosome.py` & `jcvi-1.3.4/jcvi/graphics/chromosome.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/coverage.py` & `jcvi-1.3.4/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/dotplot.py` & `jcvi-1.3.4/jcvi/graphics/dotplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,29 +29,30 @@
 import os.path as op
 import sys
 import logging
 import string
 
 from random import sample
 
-from jcvi.compara.synteny import AnchorFile, batch_scan, check_beds, get_orientation
+from jcvi.compara.synteny import batch_scan, check_beds, get_orientation
 from jcvi.utils.cbook import seqid_parse, thousands
 from jcvi.apps.base import OptionParser, need_update
 from jcvi.graphics.base import (
     plt,
     Rectangle,
     set_human_axis,
     savefig,
     draw_cmap,
     TextHandler,
     latex,
     markup,
     normalize_axes,
     set1,
 )
+from ..compara.base import AnchorFile
 
 
 class Palette(dict):
     def __init__(self, palettedict=None, palettefile=None):
         """Instantiate a palette to map from block_id to color
 
         Args:
```

### Comparing `jcvi-1.3.3/jcvi/graphics/glyph.py` & `jcvi-1.3.4/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/grabseeds.py` & `jcvi-1.3.4/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/graph.py` & `jcvi-1.3.4/jcvi/graphics/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/heatmap.py` & `jcvi-1.3.4/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/histogram.py` & `jcvi-1.3.4/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/karyotype.py` & `jcvi-1.3.4/jcvi/graphics/karyotype.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/landscape.py` & `jcvi-1.3.4/jcvi/graphics/landscape.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/logo.py` & `jcvi-1.3.4/jcvi/graphics/logo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/mummerplot.py` & `jcvi-1.3.4/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/synteny.py` & `jcvi-1.3.4/jcvi/graphics/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/table.py` & `jcvi-1.3.4/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/tree.py` & `jcvi-1.3.4/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/wheel.py` & `jcvi-1.3.4/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/graphics/whisker.py` & `jcvi-1.3.4/jcvi/graphics/whisker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/age.py` & `jcvi-1.3.4/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/alfalfa.py` & `jcvi-1.3.4/jcvi/projects/alfalfa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/allmaps.py` & `jcvi-1.3.4/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/bites.py` & `jcvi-1.3.4/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/heterosis.py` & `jcvi-1.3.4/jcvi/projects/heterosis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/ies.py` & `jcvi-1.3.4/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/misc.py` & `jcvi-1.3.4/jcvi/projects/misc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/napus.py` & `jcvi-1.3.4/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/pineapple.py` & `jcvi-1.3.4/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/pistachio.py` & `jcvi-1.3.4/jcvi/projects/pistachio.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/str.py` & `jcvi-1.3.4/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/sugarcane.py` & `jcvi-1.3.4/jcvi/projects/sugarcane.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 #
 # Created by Haibao Tang on 12/02/19
 # Copyright © 2019 Haibao Tang. All rights reserved.
 #
 import logging
 import os.path as op
 import sys
+
+from collections import Counter, defaultdict
+from glob import glob
+from itertools import combinations, groupby, product
 from random import random, sample
-from itertools import groupby
-from collections import Counter
+from typing import Dict
+
 import numpy as np
 import matplotlib.pyplot as plt
+import seaborn as sns
+import pandas as pd
 
 from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir
 from jcvi.graphics.base import adjust_spines, markup, normalize_axes, savefig
 from jcvi.utils.validator import validate_in_choices
+from ..formats.blast import Blast
 
 SoColor = "#7436a4"  # Purple
 SsColor = "#5a8340"  # Green
 
 # Computed using prepare(), corrected with real sizes
 ChrSizes = {
     "SO-chr01": 148750011,
@@ -404,16 +411,14 @@
     - nx2+n: merger between a doubled germline and a germline
 
     These two modes would impact the sequence diversity in the progeny
     genome in F1, F2, BCn ... the goal of this simulation, is thus to
     understand the mode and the spread of such diversity in the hybrid
     progenies.
     """
-    import seaborn as sns
-
     sns.set_style("darkgrid")
 
     p = OptionParser(simulate.__doc__)
     p.add_option(
         "--verbose",
         default=False,
         action="store_true",
@@ -579,30 +584,200 @@
 def prepare(args):
     """
     %prog SoChrLen.txt SsChrLen.txt
 
     Calculate lengths from real sugarcane data.
     """
     p = OptionParser(prepare.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     solist, sslist = args
     # The haploid set of LA Purple is 957.2 Mb and haploid set of US56-14-4 is 732.5 Mb
     sizes = _get_sizes(solist, 5, "SO", target_size=int(957.2 * 1e6))
     sizes.update(_get_sizes(sslist, 4, "SS", target_size=int(732.5 * 1e6)))
     print(sizes)
 
 
+def get_genome_wide_pct(summary: str) -> Dict[tuple, list]:
+    """Collect genome-wide ungapped percent identity.
+    Specifically, from file `SS_SR_SO.summary.txt`.
+
+    Args:
+        summary (str): File that contains per chromosome pct identity info,
+        collected via `formats.blast.summary()`.
+
+    Returns:
+        Dict[tuple, list]: Genome pair to list of pct identities.
+    """
+    COLUMNS = "filename, identicals, qry_gapless, qry_gapless_pct, ref_gapless, ref_gapless_pct, qryspan, pct_qryspan, refspan, pct_refspan".split(
+        ", "
+    )
+    df = pd.read_csv(summary, sep="\t", names=COLUMNS)
+    data_by_genomes = defaultdict(list)
+    for _, row in df.iterrows():
+        filename = row["filename"]
+        # e.g. SO_Chr01A.SO_Chr01B.1-1.blast
+        chr1, chr2 = filename.split(".")[:2]
+        genome1, chr1 = chr1.split("_")
+        genome2, chr2 = chr2.split("_")
+        chr1, chr2 = chr1[:5], chr2[:5]
+        if (  # Special casing for SS certain chromosomes that are non-collinear with SO/SR
+            genome1 != "SS"
+            and genome2 == "SS"
+            and chr2 not in ("Chr01", "Chr03", "Chr04")
+        ):
+            continue
+        qry_gapless_pct, ref_gapless_pct = (
+            row["qry_gapless_pct"],
+            row["ref_gapless_pct"],
+        )
+        data_by_genomes[(genome1, genome2)] += [qry_gapless_pct, ref_gapless_pct]
+    return data_by_genomes
+
+
+def get_anchors_pct(filename: str, min_pct: int = 94) -> list:
+    """Collect CDS-wide ungapped percent identity.
+
+    Args:
+        filename (str): Input file name, which is a LAST file.
+
+    Returns:
+        list: List of pct identities from this LAST file.
+    """
+    blast = Blast(filename)
+    pct = []
+    for c in blast:
+        if c.pctid < min_pct:
+            continue
+        identicals = c.hitlen - c.nmismatch - c.ngaps
+        qstart, qstop = c.qstart, c.qstop
+        sstart, sstop = c.sstart, c.sstop
+        qrycovered = qstop - qstart + 1
+        refcovered = sstop - sstart + 1
+        pct.append(identicals * 100 / qrycovered)
+        pct.append(identicals * 100 / refcovered)
+    return pct
+
+
+def divergence(args):
+    """
+    %prog divergence SS_SR_SO.summary.txt anchors
+
+    Plot divergence between and within SS/SR/SO genomes.
+    """
+    sns.set_style("white")
+
+    p = OptionParser(divergence.__doc__)
+    _, args, iopts = p.set_image_options(args, figsize="8x8")
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    (summary, anchors_dir) = args
+    data_by_genomes = get_genome_wide_pct(summary)
+    # Print summary statistics
+    print("Genome-wide ungapped percent identity:")
+    for (genome1, genome2), pct in sorted(data_by_genomes.items()):
+        print(genome1, genome2, np.mean(pct), np.std(pct))
+
+    # Find CDS matches
+    """
+    anchors_last_files = glob(op.join(anchors_dir, "*.anchors.last"))
+    anchors_by_genomes = defaultdict(list)
+    GENOME_NAME_MAPPER = {"robustum": "SR", "officinarum": "SO", "spontaneum": "SS"}
+    for filename in anchors_last_files:
+        genome1, genome2 = op.basename(filename).split(".")[:2]
+        genome1, genome2 = GENOME_NAME_MAPPER[genome1], GENOME_NAME_MAPPER[genome2]
+        pct = get_anchors_pct(filename)
+        anchors_by_genomes[(genome1, genome2)] = pct
+    # Print summary statistics
+    print("CDS anchors ungapped percent identity:")
+    for (genome1, genome2), pct in sorted(anchors_by_genomes.items()):
+        print(genome1, genome2, np.mean(pct), np.std(pct))
+    """
+
+    # Plotting genome-wide divergence
+    fig = plt.figure(figsize=(iopts.w, iopts.h))
+    root = fig.add_axes([0, 0, 1, 1])
+    SPECIES_CONFIG = {
+        "SS": {"label": "S. spontaneum", "pos": (0.5, 0.67)},
+        "SR": {"label": "S. robustum", "pos": (0.2, 0.3)},
+        "SO": {"label": "S. officinarum", "pos": (0.8, 0.3)},
+    }
+    # Get median for each genome pair
+    medians = {}
+    for (g1, g2) in product(SPECIES_CONFIG.keys(), repeat=2):
+        g1, g2 = sorted((g1, g2))
+        d = data_by_genomes[(g1, g2)]
+        medians[(g1, g2)] = np.median(d)
+    for g, config in SPECIES_CONFIG.items():
+        x, y = config["pos"]
+        text = f'*{config["label"]}*' + f"\n{medians[(g, g)]:.1f} %"
+        text = markup(text)
+        root.text(x, y, text, color="darkslategray", ha="center", va="center")
+
+    # Connect lines
+    PAD, YPAD = 0.09, 0.045
+    for g1, g2 in combinations(SPECIES_CONFIG.keys(), 2):
+        g1, g2 = sorted((g1, g2))
+        x1, y1 = SPECIES_CONFIG[g1]["pos"]
+        x2, y2 = SPECIES_CONFIG[g2]["pos"]
+        x1, x2 = (x1 + PAD, x2 - PAD) if x1 < x2 else (x1 - PAD, x2 + PAD)
+        if y1 != y2:
+            y1, y2 = (y1 + YPAD, y2 - YPAD) if y1 < y2 else (y1 - YPAD, y2 + YPAD)
+        xmid, ymid = (x1 + x2) / 2, (y1 + y2) / 2
+        text = f"{medians[(g1, g2)]:.1f} %"
+        text = markup(text)
+        root.text(xmid, ymid, text, ha="center", va="center", backgroundcolor="w")
+        root.plot([x1, x2], [y1, y2], "-", lw=4, color="darkslategray")
+
+    # Pct identity histograms
+    PCT_CONFIG = {
+        ("SS", "SS"): {"pos": (0.5, 0.82)},
+        ("SR", "SR"): {"pos": (0.1, 0.2)},
+        ("SO", "SO"): {"pos": (0.9, 0.2)},
+        ("SR", "SS"): {"pos": (0.3 - PAD, 0.55)},
+        ("SO", "SS"): {"pos": (0.7 + PAD, 0.55)},
+        ("SO", "SR"): {"pos": (0.5, 0.18)},
+    }
+    HIST_WIDTH = 0.15
+    for genome_pair, config in PCT_CONFIG.items():
+        x, y = config["pos"]
+        ax = fig.add_axes(
+            [x - HIST_WIDTH / 2, y - HIST_WIDTH / 2, HIST_WIDTH, HIST_WIDTH]
+        )
+        d = data_by_genomes[genome_pair]
+        sns.histplot(d, ax=ax, bins=5, kde=False)
+        ax.set_xlim(95, 100)
+        ax.get_yaxis().set_visible(False)
+        ax.set_xticks([95, 100])
+        adjust_spines(ax, ["bottom"], outward=True)
+        ax.spines["bottom"].set_color("lightslategray")
+
+    root.text(
+        0.5,
+        0.95,
+        "Gapless identities between and within SS/SR/SO genomes",
+        size=14,
+        ha="center",
+        va="center",
+    )
+    normalize_axes(root)
+    image_name = "SO_SR_SS.pct_id." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
+
+
 def main():
 
     actions = (
         ("prepare", "Calculate lengths from real sugarcane data"),
         ("simulate", "Run simulation on female restitution"),
+        # Plotting scripts to illustrate divergence between and within genomes
+        ("divergence", "Plot divergence between and within SS/SR/SO genomes"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.3.3/jcvi/projects/synfind.py` & `jcvi-1.3.4/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/tgbs.py` & `jcvi-1.3.4/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/projects/vanilla.py` & `jcvi-1.3.4/jcvi/projects/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 """
 Plotting scripts for the vanilla genome paper.
 """
 import logging
 import sys
 
 from jcvi.apps.base import ActionDispatcher, OptionParser
-from jcvi.compara.synteny import AnchorFile, check_beds
+from jcvi.compara.synteny import check_beds
 from jcvi.formats.base import get_number
 from jcvi.formats.bed import Bed
 from jcvi.graphics.base import normalize_axes, panel_labels, plt, savefig
 from jcvi.graphics.glyph import TextCircle
 from jcvi.graphics.synteny import Synteny, draw_gene_legend
+from ..compara.base import AnchorFile
 
 
 def main():
     actions = (
         # Chromosome painting since WGD
         ("ancestral", "paint 14 chromosomes following alpha WGD (requires data)"),
         # main figures in text
```

### Comparing `jcvi-1.3.3/jcvi/utils/aws.py` & `jcvi-1.3.4/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/cbook.py` & `jcvi-1.3.4/jcvi/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/Airswing.ttf` & `jcvi-1.3.4/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/Collegia.ttf` & `jcvi-1.3.4/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.3.4/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.3.4/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.3.4/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/adapters.fasta` & `jcvi-1.3.4/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/blosum80.mat` & `jcvi-1.3.4/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.3.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/hg38.band.txt` & `jcvi-1.3.4/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.3.4/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/data/instance.json` & `jcvi-1.3.4/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/db.py` & `jcvi-1.3.4/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/ez_setup.py` & `jcvi-1.3.4/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/grouper.py` & `jcvi-1.3.4/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/orderedcollections.py` & `jcvi-1.3.4/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/range.py` & `jcvi-1.3.4/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/table.py` & `jcvi-1.3.4/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/taxonomy.py` & `jcvi-1.3.4/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/validator.py` & `jcvi-1.3.4/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/utils/webcolors.py` & `jcvi-1.3.4/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/cnv.py` & `jcvi-1.3.4/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/deconvolute.py` & `jcvi-1.3.4/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/delly.py` & `jcvi-1.3.4/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/impute.py` & `jcvi-1.3.4/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/phase.py` & `jcvi-1.3.4/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/snp.py` & `jcvi-1.3.4/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/str.py` & `jcvi-1.3.4/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi/variation/tassel.py` & `jcvi-1.3.4/jcvi/variation/tassel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/jcvi.egg-info/PKG-INFO` & `jcvi-1.3.4/jcvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
@@ -216,7 +217,9 @@
 python -m jcvi.formats.fasta extract
 ```
 
 This will tell you the options and arguments it expects.
 
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
+
+
```

### Comparing `jcvi-1.3.3/jcvi.egg-info/SOURCES.txt` & `jcvi-1.3.4/jcvi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 jcvi/assembly/preprocess.py
 jcvi/assembly/sim.py
 jcvi/assembly/soap.py
 jcvi/assembly/syntenypath.py
 jcvi/assembly/trinity.py
 jcvi/compara/__init__.py
 jcvi/compara/__main__.py
+jcvi/compara/base.py
 jcvi/compara/blastfilter.py
 jcvi/compara/catalog.py
 jcvi/compara/fractionation.py
 jcvi/compara/pad.py
 jcvi/compara/phylogeny.py
 jcvi/compara/quota.py
 jcvi/compara/reconstruct.py
```

### Comparing `jcvi-1.3.3/setup.cfg` & `jcvi-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.3/setup.py` & `jcvi-1.3.4/setup.py`

 * *Files identical despite different names*


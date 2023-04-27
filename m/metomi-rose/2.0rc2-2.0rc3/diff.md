# Comparing `tmp/metomi-rose-2.0rc2.tar.gz` & `tmp/metomi-rose-2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metomi-rose-2.0rc2.tar", last modified: Thu Mar 24 12:21:38 2022, max compression
+gzip compressed data, was "metomi-rose-2.0rc3.tar", last modified: Fri May 20 12:44:04 2022, max compression
```

## Comparing `metomi-rose-2.0rc2.tar` & `metomi-rose-2.0rc3.tar`

### file list

```diff
@@ -1,422 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.233779 metomi-rose-2.0rc2/metomi/rose/
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19321 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/app_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/apps/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/apps/ana_builtin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/ana_builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21577 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/ana_builtin/grepper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/cumf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/exact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/mandatory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/output_grepper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/prohibited.py
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/comparisons/within.py
--rw-r--r--   0 runner    (1001) docker     (121)    11819 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/fcm_make.py
--rw-r--r--   0 runner    (1001) docker     (121)    33581 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_ana.py
--rw-r--r--   0 runner    (1001) docker     (121)    21791 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_ana_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    23070 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_arch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py
--rw-r--r--   0 runner    (1001) docker     (121)    20796 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_bunch.py
--rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/apps/rose_prune.py
--rw-r--r--   0 runner    (1001) docker     (121)     7988 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/c3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12092 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/check_software.py
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)    64089 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7736 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/config_processors/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_processors/env.py
--rw-r--r--   0 runner    (1001) docker     (121)    33931 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_processors/fileinstall.py
--rw-r--r--   0 runner    (1001) docker     (121)    15431 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/config_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    15351 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/date.py
--rw-r--r--   0 runner    (1001) docker     (121)     8243 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/date_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5855 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/env_cat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.221779 metomi-rose-2.0rc2/metomi/rose/etc/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/lib/bash/
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/lib/bash/rose_log
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/lib/bash/rose_usage
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.221779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/fcm_make/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/fcm_make/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.221779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/etc/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-app-conf/
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.221779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/rose-macro-add.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.237779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-conf/
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_bunch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_bunch/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_prune/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_prune/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf-mode.el
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.lang
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.vim
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.241779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/.validate
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/map-template/.validate
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/queues-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/queues-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/retries-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/.validate
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/kgo.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/rose-stem/
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/rose-stem/rose-suite.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.245779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.225779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/rose-app-test.conf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.249779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/rose-suite.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-introduction/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      457 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-introduction/bin/get-observations
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/rose-app.conf
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/external.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/formats/
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14235 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/formats/namelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/fs_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    24700 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/host_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/host_select_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9251 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/job_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.253779 metomi-rose-2.0rc2/metomi/rose/loc_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/namelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/rsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/rsync_remote_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/loc_handlers/svn.py
--rw-r--r--   0 runner    (1001) docker     (121)    68500 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.257779 metomi-rose-2.0rc2/metomi/rose/macros/
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12374 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/compulsory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/format.py
--rw-r--r--   0 runner    (1001) docker     (121)    16940 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    26691 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)    14522 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/macros/value.py
--rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/meta_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    16583 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/metadata_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/metadata_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)    13680 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/metadata_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/namelist_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)    43854 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/opt_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    13966 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/popen.py
--rw-r--r--   0 runner    (1001) docker     (121)     9438 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9457 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/rose.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/run_source_vc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scheme_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.257779 metomi-rose-2.0rc2/metomi/rose/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1343 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rosa-db-create
--rwxr-xr-x   0 runner    (1001) docker     (121)     1217 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rosa-svn-post-commit
--rwxr-xr-x   0 runner    (1001) docker     (121)     1214 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rosa-svn-pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (121)     1430 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rosa-ws
--rwxr-xr-x   0 runner    (1001) docker     (121)    10359 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rose-mpi-launch
--rwxr-xr-x   0 runner    (1001) docker     (121)     2919 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/scripts/rose-tutorial
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/section.py
--rw-r--r--   0 runner    (1001) docker     (121)    17868 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/suite_engine_proc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.257779 metomi-rose-2.0rc2/metomi/rose/suite_engine_procs/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/suite_engine_procs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18898 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/suite_engine_procs/cylc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8409 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/task_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     6607 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/task_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.257779 metomi-rose-2.0rc2/metomi/rose/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.257779 metomi-rose-2.0rc2/metomi/rose/tests/suite_engine_procs/
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/suite_engine_procs/test_cylc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7580 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_host_select_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_popen.py
--rw-r--r--   0 runner    (1001) docker     (121)     4855 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_resource_locator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_trigger_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/tests/test_unicode_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/unicode_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    35890 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)    15668 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rose/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.261779 metomi-rose-2.0rc2/metomi/rosie/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15908 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/db.py
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/db_create.py
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rosie/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rosie/lib/html/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.261779 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.261779 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   121260 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     7678 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (121)    17203 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/jquery.dataTables.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.261779 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    20127 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)   108738 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (121)    45404 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    23424 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    18028 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.261779 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_desc_disabled.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    36868 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (121)   434957 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (121)    78746 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    95786 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/livestamp.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    18053 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     5281 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/rosie-disco.js
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/static/rosie-favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.229779 metomi-rose-2.0rc2/metomi/rosie/lib/html/template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/metomi/rosie/lib/html/template/rosie-disco/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/template/rosie-disco/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     9235 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html
--rw-r--r--   0 runner    (1001) docker     (121)    22335 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/suite_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     5892 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/svn_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    20364 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/svn_post_commit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13444 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/svn_pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/metomi/rosie/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/tests/test_suite_id.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/metomi/rosie/usertools/
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/usertools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/usertools/ldaptool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/usertools/passwdtool.py
--rw-r--r--   0 runner    (1001) docker     (121)    29449 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/vc.py
--rw-r--r--   0 runner    (1001) docker     (121)    21705 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)    16254 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/ws_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19597 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/ws_client_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    11407 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/metomi/rosie/ws_client_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/metomi_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14400 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-24 12:21:37.000000 metomi-rose-2.0rc2/metomi_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-03-24 12:21:38.265779 metomi-rose-2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-24 12:21:34.000000 metomi-rose-2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19321 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/app_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21577 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/grepper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/
+-rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/cumf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/exact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/mandatory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/output_grepper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/prohibited.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/within.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11819 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/fcm_make.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33581 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_ana.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21791 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_ana_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23070 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20796 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_prune.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7988 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/c3.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12092 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/check_software.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (121)    64089 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7736 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/config_processors/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33931 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/fileinstall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15431 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17852 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/date.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/date_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5855 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/env_cat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_log
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_usage
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/rose-macro-add.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf-mode.el
+-rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.lang
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.vim
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process
+-rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/.validate
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/queues-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/queues-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/retries-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/kgo.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/rose-suite.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/rose-app-test.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process
+-rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/rose-suite.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      457 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/bin/get-observations
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/.validate
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/rose-app.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/external.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/formats/
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14235 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/formats/namelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24700 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/host_select_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9251 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/job_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/loc_handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/namelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync_remote_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/svn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68500 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macro.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/macros/
+-rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12374 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/compulsory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/format.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16940 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26691 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14522 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/meta_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16583 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_gen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13680 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/namelist_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43854 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/opt_parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13966 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/popen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9456 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/rose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/run_source_vc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scheme_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1343 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-db-create
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1217 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1214 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1430 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-ws
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10543 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rose-mpi-launch
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2919 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rose-tutorial
+-rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/section.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17868 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_proc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19425 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/cylc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8409 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/task_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6607 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/task_run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/test_cylc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7580 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_date_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_env_cat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_host_select_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_popen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4855 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_resource_locator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_trigger_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_unicode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/unicode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35890 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15668 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15908 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10011 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/db_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/html/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)   121260 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)     7678 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (121)    17203 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/jquery.dataTables.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)    20127 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   108738 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    45404 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    23424 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    18028 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc_disabled.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)    36868 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (121)   434957 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (121)    78746 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    95786 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/livestamp.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    18053 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5281 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/rosie-disco.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/rosie-favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     9235 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html
+-rw-r--r--   0 runner    (1001) docker     (121)    22335 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/suite_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5892 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20364 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_post_commit.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/tests/test_suite_id.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/usertools/
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/ldaptool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/passwdtool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29449 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/vc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21705 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16254 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19597 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11407 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/metomi_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14500 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/setup.py
```

### Comparing `metomi-rose-2.0rc2/COPYING` & `metomi-rose-2.0rc3/COPYING`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/PKG-INFO` & `metomi-rose-2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metomi-rose
-Version: 2.0rc2
+Version: 2.0rc3
 Summary: Rose, a framework for meteorological suites.
 Home-page: https://metomi.github.io/rose/doc/html/index.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: hpc,weather-modelling,weather-model,meteorological-suites,meteorological-modelling,meteorological-models
 Platform: any
```

### Comparing `metomi-rose-2.0rc2/README.md` & `metomi-rose-2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,8 +140,8 @@
 FILE_VAR_CHECKSUM = "checksum"
 FILE_VAR_MODE = "mode"
 FILE_VAR_SOURCE = "source"
 
 # Paths in the Rose distribution.
 FILEPATH_README = "README.md"
 
-__version__ = "2.0rc2"
+__version__ = "2.0rc3"
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/app_run.py` & `metomi-rose-2.0rc3/metomi/rose/app_run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/ana_builtin/grepper.py` & `metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/grepper.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/cumf.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/cumf.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/exact.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/exact.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/mandatory.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/mandatory.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/output_grepper.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/output_grepper.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/prohibited.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/prohibited.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/comparisons/within.py` & `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/within.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/fcm_make.py` & `metomi-rose-2.0rc3/metomi/rose/apps/fcm_make.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_ana.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_ana.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_ana_v1.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_ana_v1.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_arch.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_bunch.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_bunch.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/apps/rose_prune.py` & `metomi-rose-2.0rc3/metomi/rose/apps/rose_prune.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/c3.py` & `metomi-rose-2.0rc3/metomi/rose/c3.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/check_software.py` & `metomi-rose-2.0rc3/metomi/rose/check_software.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/checksum.py` & `metomi-rose-2.0rc3/metomi/rose/checksum.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config.py` & `metomi-rose-2.0rc3/metomi/rose/config.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_cli.py` & `metomi-rose-2.0rc3/metomi/rose/config_cli.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_diff.py` & `metomi-rose-2.0rc3/metomi/rose/config_diff.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_dump.py` & `metomi-rose-2.0rc3/metomi/rose/config_dump.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_processor.py` & `metomi-rose-2.0rc3/metomi/rose/config_processor.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_processors/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/config_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_processors/env.py` & `metomi-rose-2.0rc3/metomi/rose/config_processors/env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_processors/fileinstall.py` & `metomi-rose-2.0rc3/metomi/rose/config_processors/fileinstall.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/config_tree.py` & `metomi-rose-2.0rc3/metomi/rose/config_tree.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/date.py` & `metomi-rose-2.0rc3/metomi/rose/date.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 from metomi.isodatetime.dumpers import TimePointDumper
 from metomi.isodatetime.parsers import DurationParser, TimePointParser
 from metomi.rose.env import UnboundEnvironmentVariableError
 from metomi.rose.opt_parse import RoseOptionParser
 from metomi.rose.reporter import Reporter
 
 
+LEGACY_OFFSET = re.compile(r'-?(?P<value>\d+)(?P<unit>[wdhms])')
+CYLC5_FORMAT = re.compile(r'\d{10}')
+UNIX_FORMAT = re.compile(
+    r'\w{3} \w{3} \d{1,2} \d\d:\d\d:\d\d (?P<timezone>\w*\/?\w*) \d{4}'
+)
+
+
 class OffsetValueError(ValueError):
 
     """Bad offset value."""
 
     def __str__(self):
         return "%s: bad offset value" % self.args[0]
 
@@ -142,15 +149,14 @@
                           Otherwise, use ref time.
 
         """
         if time_point_str is None or time_point_str == self.STR_REF:
             time_point_str = self.ref_point_str
         if time_point_str is None or time_point_str == self.STR_NOW:
             time_point = get_timepoint_for_now()
-            time_point.set_time_zone_to_local()
             if self.utc_mode or time_point.get_time_zone_utc():  # is in UTC
                 parse_format = self.CURRENT_TIME_DUMP_FORMAT_Z
             else:
                 parse_format = self.CURRENT_TIME_DUMP_FORMAT
         elif self.custom_parse_format is not None:
             parse_format = self.custom_parse_format
             time_point = self.strptime(time_point_str, parse_format)
@@ -173,15 +179,15 @@
                     pass
             if time_point is None:
                 time_point = self.time_point_parser.parse(
                     time_point_str, dump_as_parsed=True
                 )
                 parse_format = time_point.dump_format
         if self.utc_mode:
-            time_point.set_time_zone_to_utc()
+            time_point = time_point.to_utc()
         return time_point, parse_format
 
     def date_shift(self, time_point=None, offset=None):
         """Return a date string with an offset.
 
         time_point -- A time point or time point string.
                       Otherwise, use current time.
@@ -298,16 +304,15 @@
             )
         except ValueError:
             return self.get_datetime_strptime(time_point_str, parse_format)
 
     @classmethod
     def get_datetime_strftime(cls, time_point, print_format):
         """Use the datetime library's strftime as a fallback."""
-        calendar_date = time_point.copy().to_calendar_date()
-        year, month, day = calendar_date.get_calendar_date()
+        year, month, day = time_point.get_calendar_date()
         hour, minute, second = time_point.get_hour_minute_second()
         microsecond = int(1.0e6 * (second - int(second)))
         hour = int(hour)
         minute = int(minute)
         second = int(second)
         date_time = datetime(
             year, month, day, hour, minute, second, microsecond
@@ -423,9 +428,102 @@
         print(
             'Invalid date/time format, please use one of H, M, S '
             + '(hours, minutes, seconds)'
         )
         sys.exit(1)
 
 
+def upgrade_offset(offset: str) -> str:
+    """Convert offset values in the legacy format
+
+    Args:
+        offset: offset matching [0-9]+[wdhms]
+
+    Returns: Offset in isodate compatible format.
+
+    URL:
+        https://github.com/metomi/rose/issues/2577
+
+    Examples:
+        >>> upgrade_offset('1w')
+        'P7DT0H0M0S'
+        >>> upgrade_offset('1w1d1h')
+        'P8DT1H0M0S'
+        >>> upgrade_offset('1h1d')
+        'P1DT1H0M0S'
+    """
+
+    sign = '-' if offset[0] == '-' else ''
+    offsets = LEGACY_OFFSET.findall(offset)
+    offsets = {unit.upper(): number for number, unit in offsets}
+
+    # Rose 2019 did not make any distinction between 1s1m and 1m1s,
+    # so we do an implicit sort here:
+    weeks, days, hours, minutes, seconds = [0 for _ in range(5)]
+    for unit, value in offsets.items():
+        if unit == 'W':
+            weeks = int(value)
+        if unit == 'D':
+            days = int(value)
+        if unit == 'H':
+            hours = int(value)
+        if unit == 'M':
+            minutes = int(value)
+        if unit == 'S':
+            seconds = int(value)
+
+    days = days + weeks * 7
+
+    result = f'{sign}P{days}DT{hours}H{minutes}M{seconds}S'
+
+    print(
+        f'[WARN] This offset syntax {offset} is deprecated: Using {result}',
+        file=sys.stderr,
+    )
+
+    return result
+
+
+def upgrade_cylc5_datetime(datetime: str) -> str:
+    """Replace a Cylc 5 style (%Y%m%d%h) datetime with a ISO8601 datetime.
+
+    Examples:
+        >>> upgrade_cylc5_datetime('2022010101')
+        '20220101T01'
+    """
+    upgraded = f'{datetime[:-2]}T{datetime[-2:]}'
+
+    print(
+        f'[WARN] This datetime syntax {datetime}'
+        f' is deprecated. Use {upgraded} instead',
+        file=sys.stderr
+    )
+
+    return upgraded
+
+
+def upgrade_unix_datetime(datetime_str: str) -> str:
+    """Replace a Unix Style Datetime string with an ISO8601 Datetime String.
+
+    Examples:
+        >>> upgrade_unix_datetime('Tue May 10 22:09:01 GMT 2022')
+        '2022-05-10T22:09:01'
+
+    Note:
+        Support of Timezones seems to be dependent on system setup and
+        may be very variable.
+    """
+    upgraded = datetime.strptime(
+        datetime_str, "%a %b %d %H:%M:%S %Z %Y"
+    ).strftime("%Y-%m-%dT%H:%M:%S%z")
+
+    print(
+        f'[WARN] This datetime syntax {datetime_str} '
+        f'is deprecated. Use {upgraded} instead',
+        file=sys.stderr
+    )
+
+    return upgraded
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/date_cli.py` & `metomi-rose-2.0rc3/metomi/rose/date_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     If not specified, the system will attempt to parse `DATE-TIME` using
     the following formats:
 
     * ctime: `%a %b %d %H:%M:%S %Y`
     * Unix date: `%a %b %d %H:%M:%S %Z %Y`
     * Basic ISO8601: `%Y-%m-%dT%H:%M:%S`, `%Y%m%dT%H%M%S`
-    * Cylc: `%Y%m%d%H`
+    * Cylc 5: `%Y%m%d%H` (deprecated)
 
     If none of these match, the date time point will be parsed according to
     the full ISO 8601 date/time standard.
 
 PRINT FORMAT
     For printing a date time point, the print format will default to the same
     format as the parse format. Also supports the isodatetime library dump
@@ -173,28 +173,91 @@
 """
 
 import sys
 import os
 
 from metomi.isodatetime.main import main as iso_main
 
+from metomi.rose.date import (
+    LEGACY_OFFSET, upgrade_offset,
+    CYLC5_FORMAT, upgrade_cylc5_datetime,
+    UNIX_FORMAT, upgrade_unix_datetime
+)
+
+
+def _handle_old_offsets(args: list) -> list:
+    """Handle Legacy Rose date --offset values:
+
+    # https://github.com/metomi/rose/issues/2577
+
+
+    Examples:
+    >>> _handle_old_offsets(['rose-date', '--offset=1d1s'])
+    ['rose-date', '--offset=P1DT0H0M1S']
+    >>> _handle_old_offsets(['rose-date', '-s', '1d1s'])
+    ['rose-date', '-s', 'P1DT0H0M1S']
+    """
+    for index, arg in enumerate(args):
+        if arg.startswith(('--offset', '-s')):
+            # Case: --offset=<offset> is a single item in args list:
+            if (
+                '=' in arg
+                and LEGACY_OFFSET.match(arg.split('=')[1])
+            ):
+                offset = upgrade_offset(arg.split("=")[1])
+                args[index] = f'{arg.split("=")[0]}={offset}'
+            # Case: --offset <offset> is two items in args list:
+            elif (
+                index + 1 < len(args)
+                and LEGACY_OFFSET.match(args[index + 1])
+            ):
+                args[index] = args[index].replace('=', '')
+                args[index + 1] = upgrade_offset(args[index + 1])
+    return args
+
+
+def _handle_old_datetimes(args: list) -> list:
+    """Handle Legacy Rose date formats
+
+    # https://github.com/metomi/rose/issues/2589
+
+    Examples
+
+    """
+    for i, arg in enumerate(args[1:], start=1):
+        if (
+            not (
+                args[i - 1].startswith('--')
+                and '=' not in args[i - 1]
+            )
+            and not arg.startswith('--')
+        ):
+            if CYLC5_FORMAT.match(arg):
+                args[i] = upgrade_cylc5_datetime(arg)
+            elif UNIX_FORMAT.match(arg):
+                args[i] = upgrade_unix_datetime(arg)
+    return args
+
 
 def main():
     """Implement rose date."""
     if sys.stdin.isatty():
         print(
             'WARNING: "rose date" is deprecated, use the "isodatetime" '
             'command.',
             file=sys.stderr
         )
 
     if '--help' in sys.argv:
         print('\n' + __doc__)
         sys.exit()
 
+    sys.argv = _handle_old_datetimes(sys.argv)
+    sys.argv = _handle_old_offsets(sys.argv)
+
     # Handle Legacy Rose-date -c functionality
     if '-c' in sys.argv or '--use-task-cycle-time' in sys.argv:
         if os.getenv('ROSE_TASK_CYCLE_TIME'):
             os.environ['ISODATETIMEREF'] = os.getenv('ROSE_TASK_CYCLE_TIME')
         elif not os.getenv('ISODATETIMEREF'):
             sys.exit(
                 "[FAIL] [UNDEFINED ENVIRONMENT VARIABLE] ROSE_TASK_CYCLE_TIME")
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/env.py` & `metomi-rose-2.0rc3/metomi/rose/env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/env_cat.py` & `metomi-rose-2.0rc3/metomi/rose/env_cat.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,58 @@
 # along with Rose. If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """Implements "rose env-cat"."""
 
 
 import sys
 
+from metomi.rose.reporter import Reporter
 from metomi.rose.env import UnboundEnvironmentVariableError, env_var_process
 from metomi.rose.opt_parse import RoseOptionParser
 
 
+def rose_env_cat(args, opts):
+    if not args:
+        args = ["-"]
+    if not opts.output_file or opts.output_file == "-":
+        out_handle = sys.stdout
+    else:
+        out_handle = open(opts.output_file, "w")
+    for arg in args:
+        if arg == "-":
+            in_handle = sys.stdin
+        else:
+            try:
+                in_handle = open(arg)
+            except FileNotFoundError as exc:
+                Reporter().report(exc)
+                if opts.debug_mode:
+                    raise exc
+                return
+        line_num = 0
+        while True:
+            line_num += 1
+            line = in_handle.readline()
+            if not line:
+                break
+            try:
+                out_handle.write(
+                    env_var_process(
+                        line, opts.unbound, opts.match_mode
+                    )
+                )
+            except UnboundEnvironmentVariableError as exc:
+                name = arg
+                if arg == "-":
+                    name = "<STDIN>"
+                sys.exit("%s:%s: %s" % (name, line_num, str(exc)))
+        in_handle.close()
+    out_handle.close()
+
+
 def main():
     """Implement "rose env-cat"."""
     opt_parser = RoseOptionParser(
         usage='rose env-cat [OPTIONS] [FILE ...]',
         description=r'''
 Substitute environment variables in input files and print.
 
@@ -50,39 +90,12 @@
         help=(
             "Specify an output file."
             "\nIf no output file is specified or if `FILE`"
             "is `-`, write output to STDOUT."
         ),
     )
     opts, args = opt_parser.parse_args()
-    if not args:
-        args = ["-"]
-    if not opts.output_file or opts.output_file == "-":
-        out_handle = sys.stdout
-    else:
-        out_handle = open(opts.output_file, "wb")
-    for arg in args:
-        if arg == "-":
-            in_handle = sys.stdin
-        else:
-            in_handle = open(arg)
-        line_num = 0
-        while True:
-            line_num += 1
-            line = in_handle.readline()
-            if not line:
-                break
-            try:
-                out_handle.write(
-                    env_var_process(line, opts.unbound, opts.match_mode)
-                )
-            except UnboundEnvironmentVariableError as exc:
-                name = arg
-                if arg == "-":
-                    name = "<STDIN>"
-                sys.exit("%s:%s: %s" % (name, line_num, str(exc)))
-        in_handle.close()
-    out_handle.close()
+    rose_env_cat(args, opts)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/lib/bash/rose_log` & `metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_log`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/lib/bash/rose_usage` & `metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_usage`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf-mode.el` & `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf-mode.el`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.lang` & `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.lang`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.vim` & `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.vim`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/syntax/rose-conf.xml` & `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.xml`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/forecast-script/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/map-template/map-template.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/queues-tutorial/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/queues-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/kgo.txt` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/kgo.txt`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-introduction/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/runtime-tutorial/runtime` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/rainfall.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py` & `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/external.py` & `metomi-rose-2.0rc3/metomi/rose/external.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/formats/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/formats/namelist.py` & `metomi-rose-2.0rc3/metomi/rose/formats/namelist.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/fs_util.py` & `metomi-rose-2.0rc3/metomi/rose/fs_util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/host_select.py` & `metomi-rose-2.0rc3/metomi/rose/host_select.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/host_select_client.py` & `metomi-rose-2.0rc3/metomi/rose/host_select_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/job_runner.py` & `metomi-rose-2.0rc3/metomi/rose/job_runner.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/fs.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/fs.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/namelist.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/namelist.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/rsync.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/rsync_remote_check.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync_remote_check.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/loc_handlers/svn.py` & `metomi-rose-2.0rc3/metomi/rose/loc_handlers/svn.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macro.py` & `metomi-rose-2.0rc3/metomi/rose/macro.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/compulsory.py` & `metomi-rose-2.0rc3/metomi/rose/macros/compulsory.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/duplicate.py` & `metomi-rose-2.0rc3/metomi/rose/macros/duplicate.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/format.py` & `metomi-rose-2.0rc3/metomi/rose/macros/format.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/rule.py` & `metomi-rose-2.0rc3/metomi/rose/macros/rule.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/trigger.py` & `metomi-rose-2.0rc3/metomi/rose/macros/trigger.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/macros/value.py` & `metomi-rose-2.0rc3/metomi/rose/macros/value.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/meta_type.py` & `metomi-rose-2.0rc3/metomi/rose/meta_type.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/metadata_check.py` & `metomi-rose-2.0rc3/metomi/rose/metadata_check.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/metadata_gen.py` & `metomi-rose-2.0rc3/metomi/rose/metadata_gen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/metadata_graph.py` & `metomi-rose-2.0rc3/metomi/rose/metadata_graph.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/namelist_dump.py` & `metomi-rose-2.0rc3/metomi/rose/namelist_dump.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/opt_parse.py` & `metomi-rose-2.0rc3/metomi/rose/opt_parse.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/popen.py` & `metomi-rose-2.0rc3/metomi/rose/popen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/reporter.py` & `metomi-rose-2.0rc3/metomi/rose/reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Rose. If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """Reporter for diagnostic messages."""
 
 
+import doctest
 import sys
 import time
 from typing import Optional
 
 
 class Reporter:
 
@@ -234,21 +235,25 @@
 
     def is_closed(self):
         """Return True if the context's handle is closed."""
         return self.handle.closed
 
     def write(self, message):
         """Write the message to the context's handle."""
-        try:
-            ret_code = self.handle.buffer.write(message.encode("utf-8"))
-        except TypeError:
+        if isinstance(self.handle, doctest._SpoofOut):
+            # If context is a doctest:
             ret_code = self.handle.write(message)
-        except AttributeError:
-            ret_code = self.handle.write(message.encode('UTF-8'))
-        self.handle.flush()
+        else:
+            try:
+                ret_code = self.handle.buffer.write(message.encode("utf-8"))
+            except TypeError:
+                ret_code = self.handle.write(message)
+            except AttributeError:
+                ret_code = self.handle.write(message.encode('UTF-8'))
+            self.handle.flush()
         return ret_code
 
     def _tty_colour_err(self, str_):
         """Colour error string for terminal."""
         try:
             if self.handle.isatty():
                 return "%s%s%s" % (
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/resource.py` & `metomi-rose-2.0rc3/metomi/rose/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 EXAMPLES
     # List top-level resources:
     $ rose resource
 
     # List the contents of the "syntax" directory:
     $ rose resource syntax
 
-    # Extract the Rose syntax file for the Vim text editor:
+    # Locate the Rose syntax file for the Vim text editor:
     $ rose resource syntax/rose-conf.vim
         ''',
         epilog='''
 ARGUMENTS
     RESOURCE_PATH
         Path of the resource to extract.
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/rose.py` & `metomi-rose-2.0rc3/metomi/rose/rose.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/run.py` & `metomi-rose-2.0rc3/metomi/rose/run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/run_source_vc.py` & `metomi-rose-2.0rc3/metomi/rose/run_source_vc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scheme_handler.py` & `metomi-rose-2.0rc3/metomi/rose/scheme_handler.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rosa-db-create` & `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-db-create`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rosa-svn-post-commit` & `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-post-commit`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rosa-svn-pre-commit` & `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-pre-commit`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rosa-ws` & `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-ws`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rose-mpi-launch` & `metomi-rose-2.0rc3/metomi/rose/scripts/rose-mpi-launch`

 * *Files 3% similar despite different names*

```diff
@@ -232,16 +232,19 @@
 fi
 
 #-------------------------------------------------------------------------------
 # 2. Find the full path of ROSE_LAUNCHER and set up the pre/post options.
 #-------------------------------------------------------------------------------
 ROSE_LAUNCHER_BASE=
 if [[ -n $ROSE_LAUNCHER ]]; then
-    # Path
-    if ! ROSE_LAUNCHER_PATH="$(type -P "$ROSE_LAUNCHER")"; then
+    # ROSE_LAUNCHER should be able to contain multiple commands.
+    # Each command should be handled separately by `type -P` so we must
+    # allow word splitting.
+    # shellcheck disable=SC2086
+    if ! ROSE_LAUNCHER_PATH="$(type -P $ROSE_LAUNCHER)"; then
         err "ROSE_LAUNCHER: $ROSE_LAUNCHER: command not found"
     fi
     ROSE_LAUNCHER=$ROSE_LAUNCHER_PATH
     ROSE_LAUNCHER_BASE="$(basename "$ROSE_LAUNCHER")"
 fi
 
 #-------------------------------------------------------------------------------
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/scripts/rose-tutorial` & `metomi-rose-2.0rc3/metomi/rose/scripts/rose-tutorial`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/section.py` & `metomi-rose-2.0rc3/metomi/rose/section.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/suite_engine_proc.py` & `metomi-rose-2.0rc3/metomi/rose/suite_engine_proc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/suite_engine_procs/__init__.py` & `metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/suite_engine_procs/cylc.py` & `metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/cylc.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,24 +94,37 @@
         return hosts
 
     def get_task_auth(
         self, suite_name: str, task_name: str
     ) -> Union[str, None]:
         """Get host for a remote task from a Cylc workflow definition.
 
-        Returns: Hostname or None if:
+        Returns: Hostname, or None if:
           - task does not run remotely.
           - task has not been defined.
+          - cylc-rose is not installed(*)
+
+        (*) This function is only used by the fcm_make built-in app. Returning
+        None is equivalent to there being no fcm_make2 task found or no
+        workflow file found which is fine - 2 stage fcm_make is only supported
+        on the localhost install target (the workflow files aren't mirrored).
+
         """
         # n.b. Imports inside function to avoid dependency on Cylc and
         # Cylc-Rose is Rose is being used with a different workflow engine.
         from cylc.flow.exceptions import WorkflowFilesError
         from cylc.flow.hostuserutil import is_remote_platform
         from cylc.flow.platforms import get_host_from_platform
-        from cylc.rose.platform_utils import get_platform_from_task_def
+        try:
+            from cylc.rose.platform_utils import get_platform_from_task_def
+        except ModuleNotFoundError:
+            # Allow single stage fcm_make app to work without requiring
+            # cylc.rose
+            return None
+
         try:
             platform = get_platform_from_task_def(suite_name, task_name)
         except KeyError:
             return None
         except (WorkflowFilesError):
             raise WorkflowFileNotFoundError
         else:
```

### Comparing `metomi-rose-2.0rc2/metomi/rose/task_env.py` & `metomi-rose-2.0rc3/metomi/rose/task_env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/task_run.py` & `metomi-rose-2.0rc3/metomi/rose/task_run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/conftest.py` & `metomi-rose-2.0rc3/metomi/rose/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/suite_engine_procs/test_cylc.py` & `metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/test_cylc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_config.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_env.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_host_select_client.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_host_select_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_popen.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_popen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_resource_locator.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_resource_locator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_trigger_file.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_trigger_file.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/tests/test_unicode_utils.py` & `metomi-rose-2.0rc3/metomi/rose/tests/test_unicode_utils.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/unicode_utils.py` & `metomi-rose-2.0rc3/metomi/rose/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/upgrade.py` & `metomi-rose-2.0rc3/metomi/rose/upgrade.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rose/variable.py` & `metomi-rose-2.0rc3/metomi/rose/variable.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/__init__.py` & `metomi-rose-2.0rc3/metomi/rosie/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/db.py` & `metomi-rose-2.0rc3/metomi/rosie/db.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/db_create.py` & `metomi-rose-2.0rc3/metomi/rosie/db_create.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/graph.py` & `metomi-rose-2.0rc3/metomi/rosie/graph.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/bootstrap.min.css` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/css/jquery.dataTables.css` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_asc.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_asc_disabled.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_both.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_desc.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/images/sort_desc_disabled.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/bootstrap.min.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.dataTables.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/jquery.min.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/livestamp.min.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/livestamp.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/moment.min.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/js/rosie-disco.js` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/rosie-disco.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/static/rosie-favicon.png` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/rosie-favicon.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/template/rosie-disco/index.html` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/index.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html` & `metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/suite_id.py` & `metomi-rose-2.0rc3/metomi/rosie/suite_id.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/svn_hook.py` & `metomi-rose-2.0rc3/metomi/rosie/svn_hook.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/svn_post_commit.py` & `metomi-rose-2.0rc3/metomi/rosie/svn_post_commit.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/svn_pre_commit.py` & `metomi-rose-2.0rc3/metomi/rosie/svn_pre_commit.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/tests/test_suite_id.py` & `metomi-rose-2.0rc3/metomi/rosie/tests/test_suite_id.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/usertools/__init__.py` & `metomi-rose-2.0rc3/metomi/rosie/usertools/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/usertools/ldaptool.py` & `metomi-rose-2.0rc3/metomi/rosie/usertools/ldaptool.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/usertools/passwdtool.py` & `metomi-rose-2.0rc3/metomi/rosie/usertools/passwdtool.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/vc.py` & `metomi-rose-2.0rc3/metomi/rosie/vc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/ws.py` & `metomi-rose-2.0rc3/metomi/rosie/ws.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/ws_client.py` & `metomi-rose-2.0rc3/metomi/rosie/ws_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/ws_client_auth.py` & `metomi-rose-2.0rc3/metomi/rosie/ws_client_auth.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi/rosie/ws_client_cli.py` & `metomi-rose-2.0rc3/metomi/rosie/ws_client_cli.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi_rose.egg-info/PKG-INFO` & `metomi-rose-2.0rc3/metomi_rose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metomi-rose
-Version: 2.0rc2
+Version: 2.0rc3
 Summary: Rose, a framework for meteorological suites.
 Home-page: https://metomi.github.io/rose/doc/html/index.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: hpc,weather-modelling,weather-model,meteorological-suites,meteorological-modelling,meteorological-models
 Platform: any
```

### Comparing `metomi-rose-2.0rc2/metomi_rose.egg-info/SOURCES.txt` & `metomi-rose-2.0rc3/metomi_rose.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,18 @@
 metomi/rose/scripts/rosa-ws
 metomi/rose/scripts/rose-mpi-launch
 metomi/rose/scripts/rose-tutorial
 metomi/rose/suite_engine_procs/__init__.py
 metomi/rose/suite_engine_procs/cylc.py
 metomi/rose/tests/conftest.py
 metomi/rose/tests/test_config.py
+metomi/rose/tests/test_date.py
+metomi/rose/tests/test_date_cli.py
 metomi/rose/tests/test_env.py
+metomi/rose/tests/test_env_cat.py
 metomi/rose/tests/test_host_select_client.py
 metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
 metomi/rose/tests/test_popen.py
 metomi/rose/tests/test_resource_locator.py
 metomi/rose/tests/test_trigger_file.py
 metomi/rose/tests/test_unicode_utils.py
 metomi/rose/tests/suite_engine_procs/test_cylc.py
```

### Comparing `metomi-rose-2.0rc2/metomi_rose.egg-info/entry_points.txt` & `metomi-rose-2.0rc3/metomi_rose.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc2/metomi_rose.egg-info/requires.txt` & `metomi-rose-2.0rc3/metomi_rose.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 aiofiles
 jinja2>=2.10.1
 ldap3
-metomi-isodatetime
+metomi-isodatetime==1!3.*
 psutil>=5.6.0
 requests
 sqlalchemy
 
 [all]
 cylc-sphinx-extensions[all]>=1.2.0
 hieroglyph>=2.1.0
```

### Comparing `metomi-rose-2.0rc2/setup.cfg` & `metomi-rose-2.0rc3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 packages = find_namespace:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
 	aiofiles
 	jinja2>=2.10.1
 	ldap3
-	metomi-isodatetime
+	metomi-isodatetime==1!3.*
 	psutil>=5.6.0
 	requests
 	sqlalchemy
 
 [options.packages.find]
 include = metomi*
```

### Comparing `metomi-rose-2.0rc2/setup.py` & `metomi-rose-2.0rc3/setup.py`

 * *Files identical despite different names*


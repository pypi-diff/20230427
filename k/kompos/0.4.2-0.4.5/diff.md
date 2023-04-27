# Comparing `tmp/kompos-0.4.2.tar.gz` & `tmp/kompos-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kompos-0.4.2.tar", last modified: Tue Oct 11 19:41:46 2022, max compression
+gzip compressed data, was "kompos-0.4.5.tar", last modified: Thu Apr 27 13:57:08 2023, max compression
```

## Comparing `kompos-0.4.2.tar` & `kompos-0.4.5.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2022-10-11 19:41:33.000000 kompos-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5998 2022-10-11 19:41:46.000000 kompos-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3866 2022-10-11 19:41:33.000000 kompos-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (116)      140 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/.komposconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      692 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/compositions/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/compositions/terraform/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/compositions/terraform/cluster/
--rw-r--r--   0 runner    (1001) docker     (116)      164 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/compositions/terraform/cluster/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/compositions/terraform/network/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/compositions/terraform/network/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=cluster/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=cluster/conf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=network/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=network/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/conf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/cluster2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=cluster/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=cluster/cluster1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=network/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=network/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      206 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/config/cloud=aws/env=dev/dev.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/modules/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/modules/cluster/
--rw-r--r--   0 runner    (1001) docker     (116)       82 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/modules/cluster/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/examples/features/hierarchical/modules/network/
--rw-r--r--   0 runner    (1001) docker     (116)      152 2022-10-11 19:41:33.000000 kompos-0.4.2/examples/features/hierarchical/modules/network/main.tf
--rw-r--r--   0 runner    (1001) docker     (116)       97 2022-10-11 19:41:33.000000 kompos-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2022-10-11 19:41:46.000000 kompos-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2423 2022-10-11 19:41:33.000000 kompos-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos/
--rw-r--r--   0 runner    (1001) docker     (116)     1502 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos/data/
--rw-r--r--   0 runner    (1001) docker     (116)     3496 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/data/config_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4086 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/helpers/himl_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     3940 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/helpers/nix.py
--rw-r--r--   0 runner    (1001) docker     (116)     5490 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/komposconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     4444 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     3842 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     9413 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos/runners/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2756 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/runners/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     6022 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/runners/helmfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     5946 2022-10-11 19:41:33.000000 kompos-0.4.2/src/kompos/runners/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5998 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1752 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       97 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-10-11 19:41:46.000000 kompos-0.4.2/src/kompos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.817836 kompos-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-27 13:56:44.000000 kompos-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 13:56:44.000000 kompos-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-27 13:57:08.817836 kompos-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-27 13:56:44.000000 kompos-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.805836 kompos-0.4.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.805836 kompos-0.4.5/examples/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/.komposconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.805836 kompos-0.4.5/examples/features/hierarchical/compositions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.805836 kompos-0.4.5/examples/features/hierarchical/compositions/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/compositions/terraform/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/compositions/terraform/cluster/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/compositions/terraform/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/compositions/terraform/network/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.809836 kompos-0.4.5/examples/features/hierarchical/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.809836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=cluster/conf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/composition=terraform/terraform=network/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster1/conf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/cluster2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.809836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=cluster/cluster1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/cluster=cluster2/composition=terraform/terraform=network/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/config/cloud=aws/env=dev/dev.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.809836 kompos-0.4.5/examples/features/hierarchical/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/modules/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/modules/cluster/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/examples/features/hierarchical/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 13:56:44.000000 kompos-0.4.5/examples/features/hierarchical/modules/network/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-27 13:56:44.000000 kompos-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 13:57:08.817836 kompos-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-27 13:56:44.000000 kompos-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.809836 kompos-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.813836 kompos-0.4.5/src/kompos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.817836 kompos-0.4.5/src/kompos/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/data/config_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.817836 kompos-0.4.5/src/kompos/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/helpers/himl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/helpers/nix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/komposconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.817836 kompos-0.4.5/src/kompos/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/runners/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/runners/helmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-27 13:56:44.000000 kompos-0.4.5/src/kompos/runners/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:08.817836 kompos-0.4.5/src/kompos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 13:57:08.000000 kompos-0.4.5/src/kompos.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kompos-0.4.2/PKG-INFO` & `kompos-0.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,157 @@
 Metadata-Version: 2.1
 Name: kompos
-Version: 0.4.2
+Version: 0.4.5
 Summary: Kompos - k8s cloud automation
 Home-page: https://github.com/adobe/kompos
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
-Description: # kompos
-        
-        [![Build Status](https://www.travis-ci.com/adobe/kompos.svg?token=8uHqfhgsxdvJ93qWAxhn&branch=main)](https://www.travis-ci.com/adobe/kompos) [![Docker pull](https://img.shields.io/docker/pulls/adobe/kompos)](https://hub.docker.com/r/adobe/kompos) [![](https://images.microbadger.com/badges/version/adobe/kompos.svg)](https://microbadger.com/images/adobe/kompos "Get your own version badge on microbadger.com") [![License](https://img.shields.io/github/license/adobe/kompos)](https://github.com/adobe/kompos/blob/master/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kompos.svg)](https://pypi.python.org/pypi/kompos/)
-        
-        ![kompos](img/kompos.png)
-        
-        **Kompos** is a configuration driven tool for provisioning and managing
-        Kubernetes infrastructure across AWS and Azure. It uses a hierarchical folder
-        structure and yaml files to store and generate configurations, with pluggable
-        compositions that encapsulates the infrastructure code and state. Terraform and
-        helmfile are supported as provisioners.
-        
-        Below is a graphical representation of the data flow.
-        
-        ![kompos-data-flow](img/kompos-diagram.svg)
-        
-        ## Installation
-        
-        _**NOTE**: Only Python 3 is supported._
-        
-        ### PyPI
-        
-        ```bash
-        pip install kompos
-        ```
-        
-        ### Locally for development
-        
-        Using virtualenv
-        
-        ```bash
-        pip install virtualenv
-        virtualenv .env
-        source .env/bin/activate
-        (env) cd kompos/
-        (env) pip install --editable .
-        ```
-        
-        ## Hierarchical configuration
-        
-        Kompos leverages [himl](https://github.com/adobe/himl) to provide a
-        [hiera](https://puppet.com/docs/puppet/latest/hiera_intro.html#concept-7256)-like
-        configuration structure.
-        
-        Checkout the [examples](./examples) for more information.
-        
-        ## Nix integration
-        
-        With kompos you can leverage [nix](https://nixos.org/nix/) to pin your
-        infrastructure code (i.e terraform & helmfile releases) on a specific version.
-        This enables you to finely control your deployments and use different
-        infrastructure versions per environment, cluster etc.
-        
-        #### Prerequisites
-        
-        Install `nix` and `nix-prefetch-git`.
-        
-        ```bash
-        $ curl -L https://nixos.org/nix/install | bash
-        
-        $ nix-env -f '<nixpkgs>' -iA nix-prefetch-git
-        ```
-        
-        #### Configuration
-        
-        The integration can be globally enabled or diabled with the flag `nix: [true|false]` and a disable overwrite
-        with `--no-nix` argument. Below are the
-        necessary parts of komposconfig regarding nix & versioning:
-        
-        ```yaml
-        terraform:
-          # This is the place to look for the terraform repo locally.
-          # Used as the default if nix is not enabled.
-          local_path: '/home/user/terraform-stack'
-        
-          # This is needed in case the modules are not in the root of the repo.
-          root_path: 'src/terraform'
-        
-          repo:
-            # This will be the name of the nix derivation for terraform.
-            name: 'terraform-stack'
-        
-            # The repo we would like to version.
-            url: "git@github.com:my-org/terraform-stack.git"
-        
-        # Likewise for helmfile.
-        helmfile:
-          local_path: '/home/user/helmfile-releases'
-          root_path: 'src/helmfiles'
-        
-          repo:
-            name: 'helmfile-releases'
-            url: "git@github.com:my-org/helmfile-releases.git"
-        
-        nix: true
-        ```
-        
-        And in the hierarchical configuration you'll need the following keys:
-        
-        ```yaml
-        infrastructure:
-          terraform:
-            version: "0.1.0" # A git tag or a commit sha.
-        
-            # This is an optional field.
-            # The sha256 hash of the repo provides data integrity and ensures that we
-            # always get the same input.
-            #
-            # It can be omitted when you're using a tag that is periodically updated.
-            # (e.g in a dev/nightly environment). Since this is a mandatory field for nix,
-            # nix-prefetch-git will be used as a fallback to caclulate it.
-            sha256: "ab9190b0ecc8060a54f1fac7de606e6b2c4757c227f2ce529668eb145d9a9516"
-        
-          # Likewise for helmfile.
-          helmfile:
-            version: "0.1.0"
-            sha256: "139cd5119d398d06f6535f42d775986a683a90e16ce129a5fb7f48870613a1a5"
-        ```
-        
-        ### Docker Image
-        
-        ## License
-        
-        [Apache License 2.0](/LICENSE)
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# kompos
+
+[![Build Status](https://www.travis-ci.com/adobe/kompos.svg?token=8uHqfhgsxdvJ93qWAxhn&branch=main)](https://www.travis-ci.com/adobe/kompos) [![Docker pull](https://img.shields.io/docker/pulls/adobe/kompos)](https://hub.docker.com/r/adobe/kompos) [![](https://images.microbadger.com/badges/version/adobe/kompos.svg)](https://microbadger.com/images/adobe/kompos "Get your own version badge on microbadger.com") [![License](https://img.shields.io/github/license/adobe/kompos)](https://github.com/adobe/kompos/blob/master/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kompos.svg)](https://pypi.python.org/pypi/kompos/)
+
+![kompos](img/kompos.png)
+
+**Kompos** is a configuration driven tool for provisioning and managing
+Kubernetes infrastructure across AWS and Azure. It uses a hierarchical folder
+structure and yaml files to store and generate configurations, with pluggable
+compositions that encapsulates the infrastructure code and state. Terraform and
+helmfile are supported as provisioners.
+
+Below is a graphical representation of the data flow.
+
+![kompos-data-flow](img/kompos-diagram.svg)
+
+## Installation
+
+_**NOTE**: Only Python 3 is supported._
+
+### PyPI
+
+```bash
+pip install kompos
+```
+
+### Locally for development
+
+Using virtualenv
+
+```bash
+pip install virtualenv
+virtualenv .env
+source .env/bin/activate
+(env) cd kompos/
+(env) pip install --editable .
+```
+
+## Hierarchical configuration
+
+Kompos leverages [himl](https://github.com/adobe/himl) to provide a
+[hiera](https://puppet.com/docs/puppet/latest/hiera_intro.html#concept-7256)-like
+configuration structure.
+
+Checkout the [examples](./examples) for more information.
+
+## Nix integration
+
+With kompos you can leverage [nix](https://nixos.org/nix/) to pin your
+infrastructure code (i.e terraform & helmfile releases) on a specific version.
+This enables you to finely control your deployments and use different
+infrastructure versions per environment, cluster etc.
+
+#### Prerequisites
+
+Install `nix` and `nix-prefetch-git`.
+
+```bash
+$ curl -L https://nixos.org/nix/install | bash
+
+$ nix-env -f '<nixpkgs>' -iA nix-prefetch-git
+```
+
+#### Configuration
+
+The integration can be globally enabled or diabled with the flag `nix: [true|false]` and a disable overwrite
+with `--no-nix` argument. Below are the
+necessary parts of komposconfig regarding nix & versioning:
+
+```yaml
+terraform:
+  # This is the place to look for the terraform repo locally.
+  # Used as the default if nix is not enabled.
+  local_path: '/home/user/terraform-stack'
+
+  # This is needed in case the modules are not in the root of the repo.
+  root_path: 'src/terraform'
+
+  repo:
+    # This will be the name of the nix derivation for terraform.
+    name: 'terraform-stack'
+
+    # The repo we would like to version.
+    url: "git@github.com:my-org/terraform-stack.git"
+
+# Likewise for helmfile.
+helmfile:
+  local_path: '/home/user/helmfile-releases'
+  root_path: 'src/helmfiles'
+
+  repo:
+    name: 'helmfile-releases'
+    url: "git@github.com:my-org/helmfile-releases.git"
+
+nix: true
+```
+
+And in the hierarchical configuration you'll need the following keys:
+
+```yaml
+infrastructure:
+  terraform:
+    version: "0.1.0" # A git tag or a commit sha.
+
+    # This is an optional field.
+    # The sha256 hash of the repo provides data integrity and ensures that we
+    # always get the same input.
+    #
+    # It can be omitted when you're using a tag that is periodically updated.
+    # (e.g in a dev/nightly environment). Since this is a mandatory field for nix,
+    # nix-prefetch-git will be used as a fallback to caclulate it.
+    sha256: "ab9190b0ecc8060a54f1fac7de606e6b2c4757c227f2ce529668eb145d9a9516"
+
+  # Likewise for helmfile.
+  helmfile:
+    version: "0.1.0"
+    sha256: "139cd5119d398d06f6535f42d775986a683a90e16ce129a5fb7f48870613a1a5"
+```
+
+### Docker Image
+
+## License
+
+[Apache License 2.0](/LICENSE)
+
+
+
+
```

### Comparing `kompos-0.4.2/README.md` & `kompos-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/examples/features/hierarchical/README.md` & `kompos-0.4.5/examples/features/hierarchical/README.md`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/setup.py` & `kompos-0.4.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,35 @@
 with open('README.md') as f:
     _readme = f.read()
 
 _mydir = os.path.abspath(os.path.dirname(sys.argv[0]))
 _requires = [r for r in open(os.path.sep.join((_mydir, 'requirements.txt')), "r").read().split('\n') if len(r) > 1]
 setup(
     name='kompos',
-    version='0.4.2',
+    version='0.4.5',
     description='Kompos - k8s cloud automation',
     long_description=_readme + '\n\n',
     long_description_content_type='text/markdown',
     url='https://github.com/adobe/kompos',
-    python_requires='>=3.5',
+    python_requires='>=3.9',
     author='Adobe',
     author_email='noreply@adobe.com',
     license='Apache2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing :: Markup :: HTML'
     ],
     package_dir={'': 'src'},
```

### Comparing `kompos-0.4.2/src/kompos/__init__.py` & `kompos-0.4.5/src/kompos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 from subprocess import call
 
 from termcolor import colored
 
-__version__ = "0.4.2"
+__version__ = "0.4.5"
 
 
 def display(msg, color):
     print(colored(msg, color))
 
 
 class Executor:
```

### Comparing `kompos-0.4.2/src/kompos/data/config_schema.json` & `kompos-0.4.5/src/kompos/data/config_schema.json`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/helpers/himl_helper.py` & `kompos-0.4.5/src/kompos/helpers/himl_helper.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/helpers/nix.py` & `kompos-0.4.5/src/kompos/helpers/nix.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/komposconfig.py` & `kompos-0.4.5/src/kompos/komposconfig.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/main.py` & `kompos-0.4.5/src/kompos/main.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/parser.py` & `kompos-0.4.5/src/kompos/parser.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/runner.py` & `kompos-0.4.5/src/kompos/runner.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/runners/config.py` & `kompos-0.4.5/src/kompos/runners/config.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/runners/helmfile.py` & `kompos-0.4.5/src/kompos/runners/helmfile.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos/runners/terraform.py` & `kompos-0.4.5/src/kompos/runners/terraform.py`

 * *Files identical despite different names*

### Comparing `kompos-0.4.2/src/kompos.egg-info/PKG-INFO` & `kompos-0.4.5/src/kompos.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,157 @@
 Metadata-Version: 2.1
 Name: kompos
-Version: 0.4.2
+Version: 0.4.5
 Summary: Kompos - k8s cloud automation
 Home-page: https://github.com/adobe/kompos
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
-Description: # kompos
-        
-        [![Build Status](https://www.travis-ci.com/adobe/kompos.svg?token=8uHqfhgsxdvJ93qWAxhn&branch=main)](https://www.travis-ci.com/adobe/kompos) [![Docker pull](https://img.shields.io/docker/pulls/adobe/kompos)](https://hub.docker.com/r/adobe/kompos) [![](https://images.microbadger.com/badges/version/adobe/kompos.svg)](https://microbadger.com/images/adobe/kompos "Get your own version badge on microbadger.com") [![License](https://img.shields.io/github/license/adobe/kompos)](https://github.com/adobe/kompos/blob/master/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kompos.svg)](https://pypi.python.org/pypi/kompos/)
-        
-        ![kompos](img/kompos.png)
-        
-        **Kompos** is a configuration driven tool for provisioning and managing
-        Kubernetes infrastructure across AWS and Azure. It uses a hierarchical folder
-        structure and yaml files to store and generate configurations, with pluggable
-        compositions that encapsulates the infrastructure code and state. Terraform and
-        helmfile are supported as provisioners.
-        
-        Below is a graphical representation of the data flow.
-        
-        ![kompos-data-flow](img/kompos-diagram.svg)
-        
-        ## Installation
-        
-        _**NOTE**: Only Python 3 is supported._
-        
-        ### PyPI
-        
-        ```bash
-        pip install kompos
-        ```
-        
-        ### Locally for development
-        
-        Using virtualenv
-        
-        ```bash
-        pip install virtualenv
-        virtualenv .env
-        source .env/bin/activate
-        (env) cd kompos/
-        (env) pip install --editable .
-        ```
-        
-        ## Hierarchical configuration
-        
-        Kompos leverages [himl](https://github.com/adobe/himl) to provide a
-        [hiera](https://puppet.com/docs/puppet/latest/hiera_intro.html#concept-7256)-like
-        configuration structure.
-        
-        Checkout the [examples](./examples) for more information.
-        
-        ## Nix integration
-        
-        With kompos you can leverage [nix](https://nixos.org/nix/) to pin your
-        infrastructure code (i.e terraform & helmfile releases) on a specific version.
-        This enables you to finely control your deployments and use different
-        infrastructure versions per environment, cluster etc.
-        
-        #### Prerequisites
-        
-        Install `nix` and `nix-prefetch-git`.
-        
-        ```bash
-        $ curl -L https://nixos.org/nix/install | bash
-        
-        $ nix-env -f '<nixpkgs>' -iA nix-prefetch-git
-        ```
-        
-        #### Configuration
-        
-        The integration can be globally enabled or diabled with the flag `nix: [true|false]` and a disable overwrite
-        with `--no-nix` argument. Below are the
-        necessary parts of komposconfig regarding nix & versioning:
-        
-        ```yaml
-        terraform:
-          # This is the place to look for the terraform repo locally.
-          # Used as the default if nix is not enabled.
-          local_path: '/home/user/terraform-stack'
-        
-          # This is needed in case the modules are not in the root of the repo.
-          root_path: 'src/terraform'
-        
-          repo:
-            # This will be the name of the nix derivation for terraform.
-            name: 'terraform-stack'
-        
-            # The repo we would like to version.
-            url: "git@github.com:my-org/terraform-stack.git"
-        
-        # Likewise for helmfile.
-        helmfile:
-          local_path: '/home/user/helmfile-releases'
-          root_path: 'src/helmfiles'
-        
-          repo:
-            name: 'helmfile-releases'
-            url: "git@github.com:my-org/helmfile-releases.git"
-        
-        nix: true
-        ```
-        
-        And in the hierarchical configuration you'll need the following keys:
-        
-        ```yaml
-        infrastructure:
-          terraform:
-            version: "0.1.0" # A git tag or a commit sha.
-        
-            # This is an optional field.
-            # The sha256 hash of the repo provides data integrity and ensures that we
-            # always get the same input.
-            #
-            # It can be omitted when you're using a tag that is periodically updated.
-            # (e.g in a dev/nightly environment). Since this is a mandatory field for nix,
-            # nix-prefetch-git will be used as a fallback to caclulate it.
-            sha256: "ab9190b0ecc8060a54f1fac7de606e6b2c4757c227f2ce529668eb145d9a9516"
-        
-          # Likewise for helmfile.
-          helmfile:
-            version: "0.1.0"
-            sha256: "139cd5119d398d06f6535f42d775986a683a90e16ce129a5fb7f48870613a1a5"
-        ```
-        
-        ### Docker Image
-        
-        ## License
-        
-        [Apache License 2.0](/LICENSE)
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# kompos
+
+[![Build Status](https://www.travis-ci.com/adobe/kompos.svg?token=8uHqfhgsxdvJ93qWAxhn&branch=main)](https://www.travis-ci.com/adobe/kompos) [![Docker pull](https://img.shields.io/docker/pulls/adobe/kompos)](https://hub.docker.com/r/adobe/kompos) [![](https://images.microbadger.com/badges/version/adobe/kompos.svg)](https://microbadger.com/images/adobe/kompos "Get your own version badge on microbadger.com") [![License](https://img.shields.io/github/license/adobe/kompos)](https://github.com/adobe/kompos/blob/master/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kompos.svg)](https://pypi.python.org/pypi/kompos/)
+
+![kompos](img/kompos.png)
+
+**Kompos** is a configuration driven tool for provisioning and managing
+Kubernetes infrastructure across AWS and Azure. It uses a hierarchical folder
+structure and yaml files to store and generate configurations, with pluggable
+compositions that encapsulates the infrastructure code and state. Terraform and
+helmfile are supported as provisioners.
+
+Below is a graphical representation of the data flow.
+
+![kompos-data-flow](img/kompos-diagram.svg)
+
+## Installation
+
+_**NOTE**: Only Python 3 is supported._
+
+### PyPI
+
+```bash
+pip install kompos
+```
+
+### Locally for development
+
+Using virtualenv
+
+```bash
+pip install virtualenv
+virtualenv .env
+source .env/bin/activate
+(env) cd kompos/
+(env) pip install --editable .
+```
+
+## Hierarchical configuration
+
+Kompos leverages [himl](https://github.com/adobe/himl) to provide a
+[hiera](https://puppet.com/docs/puppet/latest/hiera_intro.html#concept-7256)-like
+configuration structure.
+
+Checkout the [examples](./examples) for more information.
+
+## Nix integration
+
+With kompos you can leverage [nix](https://nixos.org/nix/) to pin your
+infrastructure code (i.e terraform & helmfile releases) on a specific version.
+This enables you to finely control your deployments and use different
+infrastructure versions per environment, cluster etc.
+
+#### Prerequisites
+
+Install `nix` and `nix-prefetch-git`.
+
+```bash
+$ curl -L https://nixos.org/nix/install | bash
+
+$ nix-env -f '<nixpkgs>' -iA nix-prefetch-git
+```
+
+#### Configuration
+
+The integration can be globally enabled or diabled with the flag `nix: [true|false]` and a disable overwrite
+with `--no-nix` argument. Below are the
+necessary parts of komposconfig regarding nix & versioning:
+
+```yaml
+terraform:
+  # This is the place to look for the terraform repo locally.
+  # Used as the default if nix is not enabled.
+  local_path: '/home/user/terraform-stack'
+
+  # This is needed in case the modules are not in the root of the repo.
+  root_path: 'src/terraform'
+
+  repo:
+    # This will be the name of the nix derivation for terraform.
+    name: 'terraform-stack'
+
+    # The repo we would like to version.
+    url: "git@github.com:my-org/terraform-stack.git"
+
+# Likewise for helmfile.
+helmfile:
+  local_path: '/home/user/helmfile-releases'
+  root_path: 'src/helmfiles'
+
+  repo:
+    name: 'helmfile-releases'
+    url: "git@github.com:my-org/helmfile-releases.git"
+
+nix: true
+```
+
+And in the hierarchical configuration you'll need the following keys:
+
+```yaml
+infrastructure:
+  terraform:
+    version: "0.1.0" # A git tag or a commit sha.
+
+    # This is an optional field.
+    # The sha256 hash of the repo provides data integrity and ensures that we
+    # always get the same input.
+    #
+    # It can be omitted when you're using a tag that is periodically updated.
+    # (e.g in a dev/nightly environment). Since this is a mandatory field for nix,
+    # nix-prefetch-git will be used as a fallback to caclulate it.
+    sha256: "ab9190b0ecc8060a54f1fac7de606e6b2c4757c227f2ce529668eb145d9a9516"
+
+  # Likewise for helmfile.
+  helmfile:
+    version: "0.1.0"
+    sha256: "139cd5119d398d06f6535f42d775986a683a90e16ce129a5fb7f48870613a1a5"
+```
+
+### Docker Image
+
+## License
+
+[Apache License 2.0](/LICENSE)
+
+
+
+
```

### Comparing `kompos-0.4.2/src/kompos.egg-info/SOURCES.txt` & `kompos-0.4.5/src/kompos.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 examples/features/hierarchical/.komposconfig.yaml
 examples/features/hierarchical/README.md
```


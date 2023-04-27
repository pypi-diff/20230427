# Comparing `tmp/singularity-hpc-0.1.2.tar.gz` & `tmp/singularity-hpc-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularity-hpc-0.1.2.tar", last modified: Thu Mar  9 03:00:32 2023, max compression
+gzip compressed data, was "singularity-hpc-0.1.21.tar", last modified: Thu Apr 27 19:37:56 2023, max compression
```

## Comparing `singularity-hpc-0.1.2.tar` & `singularity-hpc-0.1.21.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7728 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6870 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.526093 singularity-hpc-0.1.2/shpc/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.526093 singularity-hpc-0.1.2/shpc/client/
--rw-r--r--   0 runner    (1001) docker     (122)    15764 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/add.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/docgen.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/help.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/install.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/listing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/namespace.py
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/shell.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/show.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/sync.py
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      990 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/client/view.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     6116 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.526093 singularity-hpc-0.1.2/shpc/main/
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7584 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.526093 singularity-hpc-0.1.2/shpc/main/container/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6050 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9472 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/podman.py
--rw-r--r--   0 runner    (1001) docker     (122)    14004 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/singularity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/container/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/templates/container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/container/update/
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/update/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/update/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/container/update/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/lmod.py
--rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/module.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/tcl.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/template.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/modules/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/default_version
--rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/docker.lua
--rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/docker.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/docs.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/modules/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/includes/default_version.lua
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/includes/load_view.lua
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/includes/load_view.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/singularity.lua
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/singularity.tcl
--rwxr-xr-x   0 runner    (1001) docker     (122)      405 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/test.sh
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/view_module.lua
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/templates/view_module.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/versions.py
--rw-r--r--   0 runner    (1001) docker     (122)    18795 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/modules/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.530093 singularity-hpc-0.1.2/shpc/main/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/registry/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/registry/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/registry/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13562 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5150 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/bases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/bases/shell-script-base.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/container.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/exec.sh
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/inspect.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      650 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/shell.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      730 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/container.sh
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/exec.sh
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/inspect-deffile.sh
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/inspect-runscript.sh
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/shell.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      794 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/main/wrappers/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/main/wrappers/templates/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3931 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.534093 singularity-hpc-0.1.2/shpc/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/helpers.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      474 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test-registry-module.sh
--rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_client.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3757 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_client.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_container_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     4150 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/shpc/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/alias-container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/empty_singularity.sh
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/hashtest.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/overrides-invalid.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/python-container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/quay-container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.522093 singularity-hpc-0.1.2/shpc/tests/testdata/registry/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.522093 singularity-hpc-0.1.2/shpc/tests/testdata/registry/dinosaur/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/shpc/tests/testdata/registry/dinosaur/salad/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/registry/dinosaur/salad/container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/shpc/tests/testdata/samtools/
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/samtools/1.15--h3843a85_0.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/samtools/container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/tests/testdata/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/shpc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-03-09 03:00:10.000000 singularity-hpc-0.1.2/shpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 03:00:32.538093 singularity-hpc-0.1.2/singularity_hpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7728 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4167 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-09 03:00:32.000000 singularity-hpc-0.1.2/singularity_hpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.305627 singularity-hpc-0.1.21/
+-rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-04-27 19:37:56.305627 singularity-hpc-0.1.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6870 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-04-27 19:37:56.305627 singularity-hpc-0.1.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.281627 singularity-hpc-0.1.21/shpc/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.285627 singularity-hpc-0.1.21/shpc/client/
+-rw-r--r--   0 runner    (1001) docker     (122)    15764 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/docgen.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/help.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/listing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/client/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6116 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.285627 singularity-hpc-0.1.21/shpc/main/
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7584 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.285627 singularity-hpc-0.1.21/shpc/main/container/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6050 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9472 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/podman.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14004 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/singularity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.285627 singularity-hpc-0.1.21/shpc/main/container/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/templates/container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.289627 singularity-hpc-0.1.21/shpc/main/container/update/
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/update/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/update/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/container/update/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.289627 singularity-hpc-0.1.21/shpc/main/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/modules/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/default_version
+-rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/docker.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/docker.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/docs.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/modules/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/includes/default_version.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/includes/load_view.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/includes/load_view.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/singularity.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/singularity.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (122)      405 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/view_module.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/templates/view_module.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18795 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/modules/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/registry/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/registry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/registry/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13562 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5150 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/wrappers/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.293627 singularity-hpc-0.1.21/shpc/main/wrappers/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/bases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/bases/shell-script-base.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.297627 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/exec.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/inspect.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      650 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/shell.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      730 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.297627 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/container.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/exec.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/inspect-deffile.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/inspect-runscript.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/shell.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      794 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.297627 singularity-hpc-0.1.21/shpc/main/wrappers/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/main/wrappers/templates/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.301627 singularity-hpc-0.1.21/shpc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/helpers.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      474 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test-registry-module.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3757 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_client.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_container_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4150 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.301627 singularity-hpc-0.1.21/shpc/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/alias-container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/empty_singularity.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/hashtest.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/overrides-invalid.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/python-container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/quay-container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.277627 singularity-hpc-0.1.21/shpc/tests/testdata/registry/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.277627 singularity-hpc-0.1.21/shpc/tests/testdata/registry/dinosaur/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.301627 singularity-hpc-0.1.21/shpc/tests/testdata/registry/dinosaur/salad/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/registry/dinosaur/salad/container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.301627 singularity-hpc-0.1.21/shpc/tests/testdata/samtools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/samtools/1.15--h3843a85_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/samtools/container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/tests/testdata/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.305627 singularity-hpc-0.1.21/shpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-04-27 19:37:22.000000 singularity-hpc-0.1.21/shpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 19:37:56.305627 singularity-hpc-0.1.21/singularity_hpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4167 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-27 19:37:56.000000 singularity-hpc-0.1.21/singularity_hpc.egg-info/top_level.txt
```

### Comparing `singularity-hpc-0.1.2/LICENSE` & `singularity-hpc-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/PKG-INFO` & `singularity-hpc-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singularity-hpc
-Version: 0.1.2
+Version: 0.1.21
 Summary: Local registry intended for HPC using containers and system modules.
 Home-page: https://github.com/singularityhub/singularity-hpc
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: singularity,containers,hpc,lmd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.2 Summary: Local
+Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.21 Summary: Local
 registry intended for HPC using containers and system modules. Home-page:
 https://github.com/singularityhub/singularity-hpc Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa Sochat
 License: LICENSE Keywords: singularity,containers,hpc,lmd Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C Classifier: Programming Language ::
```

### Comparing `singularity-hpc-0.1.2/README.md` & `singularity-hpc-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/setup.py` & `singularity-hpc-0.1.21/setup.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/__init__.py` & `singularity-hpc-0.1.21/shpc/client/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/add.py` & `singularity-hpc-0.1.21/shpc/client/add.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/check.py` & `singularity-hpc-0.1.21/shpc/client/check.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/config.py` & `singularity-hpc-0.1.21/shpc/client/config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/docgen.py` & `singularity-hpc-0.1.21/shpc/client/docgen.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/get.py` & `singularity-hpc-0.1.21/shpc/client/get.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/help.py` & `singularity-hpc-0.1.21/shpc/client/help.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/inspect.py` & `singularity-hpc-0.1.21/shpc/client/inspect.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/install.py` & `singularity-hpc-0.1.21/shpc/client/install.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/listing.py` & `singularity-hpc-0.1.21/shpc/client/listing.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/namespace.py` & `singularity-hpc-0.1.21/shpc/client/namespace.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/pull.py` & `singularity-hpc-0.1.21/shpc/client/pull.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/remove.py` & `singularity-hpc-0.1.21/shpc/client/remove.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/shell.py` & `singularity-hpc-0.1.21/shpc/client/shell.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/show.py` & `singularity-hpc-0.1.21/shpc/client/show.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/sync.py` & `singularity-hpc-0.1.21/shpc/client/sync.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/test.py` & `singularity-hpc-0.1.21/shpc/client/test.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/uninstall.py` & `singularity-hpc-0.1.21/shpc/client/uninstall.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/client/view.py` & `singularity-hpc-0.1.21/shpc/client/view.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/defaults.py` & `singularity-hpc-0.1.21/shpc/defaults.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/logger.py` & `singularity-hpc-0.1.21/shpc/logger.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/__init__.py` & `singularity-hpc-0.1.21/shpc/main/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/client.py` & `singularity-hpc-0.1.21/shpc/main/client.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/base.py` & `singularity-hpc-0.1.21/shpc/main/container/base.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/config.py` & `singularity-hpc-0.1.21/shpc/main/container/config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/docker.py` & `singularity-hpc-0.1.21/shpc/main/container/docker.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/podman.py` & `singularity-hpc-0.1.21/shpc/main/container/podman.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/singularity.py` & `singularity-hpc-0.1.21/shpc/main/container/singularity.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/update/__init__.py` & `singularity-hpc-0.1.21/shpc/main/container/update/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/update/diff.py` & `singularity-hpc-0.1.21/shpc/main/container/update/diff.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/update/docker.py` & `singularity-hpc-0.1.21/shpc/main/container/update/docker.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/container/update/versions.py` & `singularity-hpc-0.1.21/shpc/main/container/update/versions.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/base.py` & `singularity-hpc-0.1.21/shpc/main/modules/base.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/module.py` & `singularity-hpc-0.1.21/shpc/main/modules/module.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/tcl.py` & `singularity-hpc-0.1.21/shpc/main/modules/tcl.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/template.py` & `singularity-hpc-0.1.21/shpc/main/modules/template.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/templates/docker.lua` & `singularity-hpc-0.1.21/shpc/main/modules/templates/docker.lua`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/templates/docker.tcl` & `singularity-hpc-0.1.21/shpc/main/modules/templates/docker.tcl`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/templates/docs.md` & `singularity-hpc-0.1.21/shpc/main/modules/templates/docs.md`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/templates/singularity.lua` & `singularity-hpc-0.1.21/shpc/main/modules/templates/singularity.lua`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/templates/singularity.tcl` & `singularity-hpc-0.1.21/shpc/main/modules/templates/singularity.tcl`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/versions.py` & `singularity-hpc-0.1.21/shpc/main/modules/versions.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/modules/views.py` & `singularity-hpc-0.1.21/shpc/main/modules/views.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/registry/__init__.py` & `singularity-hpc-0.1.21/shpc/main/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/registry/filesystem.py` & `singularity-hpc-0.1.21/shpc/main/registry/filesystem.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/registry/provider.py` & `singularity-hpc-0.1.21/shpc/main/registry/provider.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/registry/remote.py` & `singularity-hpc-0.1.21/shpc/main/registry/remote.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/schemas.py` & `singularity-hpc-0.1.21/shpc/main/schemas.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/settings.py` & `singularity-hpc-0.1.21/shpc/main/settings.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/__init__.py` & `singularity-hpc-0.1.21/shpc/main/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/base.py` & `singularity-hpc-0.1.21/shpc/main/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/generators.py` & `singularity-hpc-0.1.21/shpc/main/wrappers/generators.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/exec.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/exec.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/run.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/run.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker/shell.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker/shell.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/docker.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/docker.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/exec.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/exec.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/run.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/run.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity/shell.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity/shell.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/main/wrappers/templates/singularity.sh` & `singularity-hpc-0.1.21/shpc/main/wrappers/templates/singularity.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/settings.yml` & `singularity-hpc-0.1.21/shpc/settings.yml`

 * *Files 2% similar despite different names*

```diff
@@ -99,8 +99,7 @@
 # container features like gpu will modify generated recipes
 container_features:
   gpu:      # one of null, amd, or nvidia
   x11:      # one of null, true, false, or a path
             # defaults to ~/.Xauthority if set to true and the container has x11: true
   home:     # one of null, or a single path or src:dest path.
             # home: true in a container.yaml will use this path, if defines
-updated_at: '2022-08-26T20:38:06Z'
```

### Comparing `singularity-hpc-0.1.2/shpc/tests/helpers.py` & `singularity-hpc-0.1.21/shpc/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/helpers.sh` & `singularity-hpc-0.1.21/shpc/tests/helpers.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_client.py` & `singularity-hpc-0.1.21/shpc/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_client.sh` & `singularity-hpc-0.1.21/shpc/tests/test_client.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_config.py` & `singularity-hpc-0.1.21/shpc/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_container.py` & `singularity-hpc-0.1.21/shpc/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_container_config.py` & `singularity-hpc-0.1.21/shpc/tests/test_container_config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_settings.py` & `singularity-hpc-0.1.21/shpc/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_sync.py` & `singularity-hpc-0.1.21/shpc/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_utils.py` & `singularity-hpc-0.1.21/shpc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_views.py` & `singularity-hpc-0.1.21/shpc/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/test_wrappers.py` & `singularity-hpc-0.1.21/shpc/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/testdata/alias-container.yaml` & `singularity-hpc-0.1.21/shpc/tests/testdata/alias-container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/testdata/python-container.yaml` & `singularity-hpc-0.1.21/shpc/tests/testdata/python-container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/testdata/registry/dinosaur/salad/container.yaml` & `singularity-hpc-0.1.21/shpc/tests/testdata/registry/dinosaur/salad/container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml` & `singularity-hpc-0.1.21/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/tests/testdata/samtools/container.yaml` & `singularity-hpc-0.1.21/shpc/tests/testdata/samtools/container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/utils/fileio.py` & `singularity-hpc-0.1.21/shpc/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/utils/terminal.py` & `singularity-hpc-0.1.21/shpc/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.2/shpc/version.py` & `singularity-hpc-0.1.21/shpc/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright 2021-2023, Vanessa Sochat"
 __license__ = "MPL 2.0"
 
-__version__ = "0.1.2"
+__version__ = "0.1.21"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "singularity-hpc"
 PACKAGE_URL = "https://github.com/singularityhub/singularity-hpc"
 KEYWORDS = "singularity, containers, hpc, lmd"
 DESCRIPTION = "Local registry intended for HPC using containers and system modules."
 LICENSE = "LICENSE"
```

### Comparing `singularity-hpc-0.1.2/singularity_hpc.egg-info/PKG-INFO` & `singularity-hpc-0.1.21/singularity_hpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singularity-hpc
-Version: 0.1.2
+Version: 0.1.21
 Summary: Local registry intended for HPC using containers and system modules.
 Home-page: https://github.com/singularityhub/singularity-hpc
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: singularity,containers,hpc,lmd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.2 Summary: Local
+Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.21 Summary: Local
 registry intended for HPC using containers and system modules. Home-page:
 https://github.com/singularityhub/singularity-hpc Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa Sochat
 License: LICENSE Keywords: singularity,containers,hpc,lmd Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C Classifier: Programming Language ::
```

### Comparing `singularity-hpc-0.1.2/singularity_hpc.egg-info/SOURCES.txt` & `singularity-hpc-0.1.21/singularity_hpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*


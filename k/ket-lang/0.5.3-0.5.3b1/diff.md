# Comparing `tmp/ket-lang-0.5.3.tar.gz` & `tmp/ket-lang-0.5.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.5.3.tar", last modified: Thu Apr 27 20:09:20 2023, max compression
+gzip compressed data, was "ket-lang-0.5.3b1.tar", last modified: Thu Apr 13 18:04:47 2023, max compression
```

## Comparing `ket-lang-0.5.3.tar` & `ket-lang-0.5.3b1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.824649 ket-lang-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)    11455 2023-04-27 20:09:08.000000 ket-lang-0.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-27 20:09:08.000000 ket-lang-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7164 2023-04-27 20:09:20.824649 ket-lang-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6412 2023-04-27 20:09:08.000000 ket-lang-0.5.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-27 20:09:08.000000 ket-lang-0.5.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-27 20:09:20.825649 ket-lang-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-27 20:09:08.000000 ket-lang-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.792647 ket-lang-0.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.799647 ket-lang-0.5.3/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    28956 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.800647 ket-lang-0.5.3/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.801648 ket-lang-0.5.3/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.804648 ket-lang-0.5.3/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-27 20:09:09.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/kbw.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.808648 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/c_wrapper.rs
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    20501 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     9825 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    20230 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.808648 ket-lang-0.5.3/src/ket/clib/libs/kbw/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/kbw/tests/shor.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.811648 ket-lang-0.5.3/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-27 20:09:09.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/libket.h
--rw-rw-rw-   0 root         (0) root         (0)    10365 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/libket.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.815648 ket-lang-0.5.3/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.817649 ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/error.rs
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     6838 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    10966 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     5725 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/code_block.rs
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     6275 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/gates.rs
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/instruction.rs
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/object.rs
--rw-rw-rw-   0 root         (0) root         (0)    20114 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-27 20:09:10.000000 ket-lang-0.5.3/src/ket/clib/libs/libket/src/serialize.rs
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/clib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.818649 ket-lang-0.5.3/src/ket/gates/
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/gates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/gates/base_gates.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/gates/quantum_gate.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/import_ket.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.820649 ket-lang-0.5.3/src/ket/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/preprocessor/statements.py
--rw-rw-rw-   0 root         (0) root         (0)     8995 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/preprocessor/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.821649 ket-lang-0.5.3/src/ket/standard/
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/standard/adj.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-27 20:09:08.000000 ket-lang-0.5.3/src/ket/standard/ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.824649 ket-lang-0.5.3/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7164 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2215 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 20:09:20.000000 ket-lang-0.5.3/src/ket_lang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 20:09:20.824649 ket-lang-0.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-04-27 20:09:08.000000 ket-lang-0.5.3/tests/test_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/
+-rw-rw-rw-   0 root         (0) root         (0)    11455 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-13 18:04:47.266780 ket-lang-0.5.3b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.236778 ket-lang-0.5.3b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.242778 ket-lang-0.5.3b1/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28956 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     8828 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.247779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-13 18:04:35.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20501 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9825 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20230 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/shor.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.253779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h
+-rw-rw-rw-   0 root         (0) root         (0)    10365 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.257779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.258780 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6838 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    10966 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     5725 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20114 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.259780 ket-lang-0.5.3b1/src/ket/gates/
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/base_gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/import_ket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.261780 ket-lang-0.5.3b1/src/ket/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/statements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8995 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.262780 ket-lang-0.5.3b1/src/ket/standard/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/adj.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.264780 ket-lang-0.5.3b1/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/tests/test_gates.py
```

### Comparing `ket-lang-0.5.3/LICENSE` & `ket-lang-0.5.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/PKG-INFO` & `ket-lang-0.5.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.3
+Version: 0.5.3b1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: ev.crr97@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.5.3/README.md` & `ket-lang-0.5.3b1/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/setup.cfg` & `ket-lang-0.5.3b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/__init__.py` & `ket-lang-0.5.3b1/src/ket/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .process import *
 from .gates import __all__ as all_gate
 from .import_ket import __all__ as all_import
 from .base import __all__ as all_base
 from .standard import __all__ as all_standard
 from .process import __all__ as all_process
 
-__version__ = '0.5.3'
+__version__ = '0.5.3b1'
 __all__ = all_gate + all_import + all_base + all_standard + all_process
 
 from .import_ket import code_ket
 
 from .base import QUANTUM_EXECUTION_TARGET
 if QUANTUM_EXECUTION_TARGET is None:
     from .kbw import use_sparse
```

### Comparing `ket-lang-0.5.3/src/ket/__main__.py` & `ket-lang-0.5.3b1/src/ket/__main__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/base.py` & `ket-lang-0.5.3b1/src/ket/base.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/kbw.py` & `ket-lang-0.5.3b1/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libket.py` & `ket-lang-0.5.3b1/src/ket/clib/libket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/__init__.py` & `ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/CHANGELOG.md` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/README.md` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/kbw.h` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/c_wrapper.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/kbw/tests/shor.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/shor.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/README.md` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/libket.h` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/libket.hpp` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/objects.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/c_wrapper/process.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/code_block.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/gates.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/instruction.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/ir.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/object.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/process.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/libs/libket/src/serialize.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/clib/wrapper.py` & `ket-lang-0.5.3b1/src/ket/clib/wrapper.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/gates/__init__.py` & `ket-lang-0.5.3b1/src/ket/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/gates/base_gates.py` & `ket-lang-0.5.3b1/src/ket/gates/base_gates.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/gates/quantum_gate.py` & `ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/import_ket.py` & `ket-lang-0.5.3b1/src/ket/import_ket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/kbw.py` & `ket-lang-0.5.3b1/src/ket/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/lib.py` & `ket-lang-0.5.3b1/src/ket/lib.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/plugins.py` & `ket-lang-0.5.3b1/src/ket/plugins.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/preprocessor/statements.py` & `ket-lang-0.5.3b1/src/ket/preprocessor/statements.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/preprocessor/transformer.py` & `ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/process.py` & `ket-lang-0.5.3b1/src/ket/process.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/standard/__init__.py` & `ket-lang-0.5.3b1/src/ket/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/standard/adj.py` & `ket-lang-0.5.3b1/src/ket/standard/adj.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket/standard/ctrl.py` & `ket-lang-0.5.3b1/src/ket/standard/ctrl.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.3
+Version: 0.5.3b1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: ev.crr97@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.5.3/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3/tests/test_gates.py` & `ket-lang-0.5.3b1/tests/test_gates.py`

 * *Files identical despite different names*


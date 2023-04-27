# Comparing `tmp/perpetuo-0.2.0.tar.gz` & `tmp/perpetuo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perpetuo-0.2.0.tar", last modified: Tue Apr 25 01:54:44 2023, max compression
+gzip compressed data, was "perpetuo-0.3.0.tar", last modified: Thu Apr 27 06:53:13 2023, max compression
```

## Comparing `perpetuo-0.2.0.tar` & `perpetuo-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    50176 2023-04-25 01:54:36.000000 perpetuo-0.2.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 01:54:36.000000 perpetuo-0.2.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 01:54:36.000000 perpetuo-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-25 01:54:44.552439 perpetuo-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-25 01:54:36.000000 perpetuo-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 01:54:36.000000 perpetuo-0.2.0/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 01:54:36.000000 perpetuo-0.2.0/prep-manylinux-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-25 01:54:36.000000 perpetuo-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.548439 perpetuo-0.2.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.548439 perpetuo-0.2.0/python/perpetuo/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/_perpetuo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/python/perpetuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:54:44.552439 perpetuo-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-25 01:54:36.000000 perpetuo-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/shmem.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    50192 2023-04-27 06:53:04.000000 perpetuo-0.3.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 06:53:04.000000 perpetuo-0.3.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 06:53:04.000000 perpetuo-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 06:53:13.948888 perpetuo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 06:53:04.000000 perpetuo-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 06:53:04.000000 perpetuo-0.3.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 06:53:04.000000 perpetuo-0.3.0/prep-manylinux-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 06:53:04.000000 perpetuo-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.944888 perpetuo-0.3.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_perpetuo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_tests/test_perpetuo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:53:13.948888 perpetuo-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-27 06:53:04.000000 perpetuo-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/shmem.rs
```

### Comparing `perpetuo-0.2.0/Cargo.lock` & `perpetuo-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android_system_properties"
 version = "0.1.5"
@@ -70,17 +70,17 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
+checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -109,17 +109,17 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
@@ -178,15 +178,15 @@
 version = "0.60.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "062dddbc1ba4aca46de6338e2bf87771414c335f7b2f2036e8f3e9befebf88e6"
 dependencies = [
  "bitflags",
  "cexpr",
  "clang-sys",
- "clap 3.2.23",
+ "clap 3.2.24",
  "env_logger 0.9.3",
  "lazy_static",
  "lazycell",
  "log",
  "peeking_take_while",
  "proc-macro2",
  "quote",
@@ -200,17 +200,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
@@ -288,68 +288,69 @@
  "textwrap 0.11.0",
  "unicode-width",
  "vec_map",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "eef2b3ded6a26dfaec672a742c93c8cf6b689220324da509ec5caa20de55dc83"
 dependencies = [
  "atty",
  "bitflags",
- "clap_derive 3.2.18",
+ "clap_derive 3.2.24",
  "clap_lex 0.2.4",
  "indexmap",
  "once_cell",
  "strsim 0.10.0",
  "termcolor",
  "terminal_size",
  "textwrap 0.16.0",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.2"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
+checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.2"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
+checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim 0.10.0",
+ "terminal_size",
 ]
 
 [[package]]
 name = "clap_complete"
 version = "3.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f7a2e0a962c45ce25afce14220bc24f9dade0a1787f185cecf96bfba7847cd8"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.24",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.18"
+version = "3.2.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
+checksum = "d756c5824fc5c0c1ee8e36000f576968dbcb2081def956c83fad6f40acd46f96"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
@@ -766,15 +767,15 @@
 [[package]]
 name = "inferno"
 version = "0.11.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fb7c1b80a1dfa604bb4a649a5c5aeef3d913f7c520cb42b40e534e8a61bcdfc"
 dependencies = [
  "ahash 0.8.3",
- "clap 4.2.2",
+ "clap 4.2.4",
  "crossbeam-channel",
  "crossbeam-utils",
  "dashmap",
  "env_logger 0.10.0",
  "indexmap",
  "is-terminal",
  "itoa",
@@ -843,17 +844,17 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -895,17 +896,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1114,24 +1115,24 @@
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "perpetuo"
-version = "0.1.0"
+version = "0.3.0"
 dependencies = [
  "anyhow",
  "bytemuck",
- "clap 4.2.2",
+ "clap 4.2.4",
  "indoc 2.0.1",
  "libc",
  "memmap",
  "once_cell",
- "proc-maps 0.3.0",
+ "proc-maps 0.3.1",
  "py-spy",
  "pyo3",
  "pyo3-build-config",
  "remoteprocess",
  "windows-sys 0.48.0",
 ]
 
@@ -1192,17 +1193,17 @@
  "libproc 0.10.0",
  "mach2",
  "winapi",
 ]
 
 [[package]]
 name = "proc-maps"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c790484f98e8b00e2385ebde989077698f99417307a74361001ada102f8c2ce"
+checksum = "3d17946c951c8e8c4233375fdbfc212b215bd14ea1b18388eae8c95bb03a0174"
 dependencies = [
  "anyhow",
  "bindgen 0.60.1",
  "libc",
  "libproc 0.12.0",
  "mach2",
  "winapi",
@@ -1212,15 +1213,15 @@
 name = "py-spy"
 version = "0.3.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08585ad9771560e3243153e5194ba15910507bfb2e8000285cfe0432ae17ba6"
 dependencies = [
  "anyhow",
  "chrono",
- "clap 3.2.23",
+ "clap 3.2.24",
  "clap_complete",
  "console",
  "cpp_demangle 0.3.5",
  "ctrlc",
  "env_logger 0.9.3",
  "goblin 0.5.4",
  "indicatif",
@@ -1389,28 +1390,28 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "remoteprocess"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3ed67d3fade907d519c2edd07329a8f16296a64f91b6f3c35570769cf6b25d"
 dependencies = [
@@ -1421,15 +1422,15 @@
  "libproc 0.12.0",
  "log",
  "mach",
  "mach_o_sys",
  "memmap",
  "nix 0.25.1",
  "object",
- "proc-maps 0.3.0",
+ "proc-maps 0.3.1",
  "read-process-memory",
  "regex",
  "winapi",
 ]
 
 [[package]]
 name = "rgb"
@@ -1450,17 +1451,17 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.11"
+version = "0.37.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
+checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
 dependencies = [
  "bitflags",
  "errno 0.3.1",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1594,17 +1595,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
```

### Comparing `perpetuo-0.2.0/Cargo.toml` & `perpetuo-0.3.0/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "perpetuo"
-version = "0.2.0"
+version = "0.3.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "perpetuo"
@@ -12,15 +12,15 @@
 
 [[bin]]
 name = "perpetuo"
 
 [dependencies]
 anyhow = "1.0.70"
 bytemuck = { version = "1.13.1", features = ["derive", "zeroable_atomics"] }
-clap = { version = "4.2.2", features = ["derive"] }
+clap = { version = "4.2.2", features = ["derive", "wrap_help"] }
 indoc = "2.0.1"
 memmap = "0.7.0"
 once_cell = "1.17.1"
 proc-maps = "0.3.0"
 py-spy = "0.3.14"
 pyo3 = { version = "0.18.3", features = ["extension-module", "abi3", "abi3-py39"] }
 remoteprocess = "0.4.11"
```

### Comparing `perpetuo-0.2.0/LICENSE.APACHE2` & `perpetuo-0.3.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `perpetuo-0.2.0/LICENSE.MIT` & `perpetuo-0.3.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `perpetuo-0.2.0/PKG-INFO` & `perpetuo-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.2.0
+Version: 0.3.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.2.0/README.md` & `perpetuo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `perpetuo-0.2.0/prep-manylinux-container.sh` & `perpetuo-0.3.0/prep-manylinux-container.sh`

 * *Files identical despite different names*

### Comparing `perpetuo-0.2.0/pyproject.toml` & `perpetuo-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "perpetuo"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   {name = "Nathaniel J. Smith", email = "njs@pobox.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT OR Apache-2.0"}
 description = "A stall tracker for Python's GIL and Trio tasks"
```

### Comparing `perpetuo-0.2.0/python/perpetuo/_setup.py` & `perpetuo-0.3.0/python/perpetuo/_setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 import os
 import sys
-import warnings
 import threading
 import subprocess
 
 from ._perpetuo import StallTracker
 
 
-WATCHER = None
+WATCHER: subprocess.Popen | None = None
+GIL_STALLTRACKER: StallTracker | None = None
 
 
-def start_watcher() -> None:
+def start_watcher(*, poll_interval: float | None = None) -> None:
     global WATCHER
     if WATCHER is None:
-        subprocess.Popen(["perpetuo", "watch", str(os.getpid())])
+        if poll_interval is not None:
+            poll_args = ["--poll-interval", str(poll_interval)]
+        else:
+            poll_args = []
+        subprocess.Popen(["perpetuo", "watch", str(os.getpid())] + poll_args)
+
+
+def stop_watcher() -> None:
+    global WATCHER
+    if WATCHER is not None:
+        WATCHER.kill()
+        WATCHER.wait()
+        WATCHER = None
 
 
 def instrument_gil() -> None:
+    global GIL_STALLTRACKER
+    if GIL_STALLTRACKER is not None:
+        return
     if hasattr(sys, "_set_stall_counter"):
-        gil_tracker = StallTracker("GIL", "gil")
-        sys._set_stall_counter(gil_tracker.counter_address())
+        GILL_STALLTRACKER = StallTracker("GIL", "gil")
+        sys._set_stall_counter(GILL_STALLTRACKER.counter_address())
     else:
         raise RuntimeError(
             "This Python was not built with the perpetuo GIL instrumentation patch"
         )
 
 
 def instrument_trio() -> None:
@@ -31,35 +46,44 @@
 
     class TrioStallInstrument(trio.abc.Instrument):
         def __init__(self):
             # We construct the tracker lazily, to make sure that we're already in Trio
             # before it becomes active
             self.stall_tracker: StallTracker | None = None
 
+        def _init(self):
+            assert self.stall_tracker is None
+            thread = threading.current_thread().ident
+            self.stall_tracker = StallTracker(
+                f"Trio run loop (thread {thread:#_x})", thread
+            )
+
         def before_task_step(self, _: trio.lowlevel.Task) -> None:
             if self.stall_tracker is None:
-                self.stall_tracker = StallTracker(
-                    "Trio run loop", threading.current_thread().ident
-                )
-                # New StallTracker starts out in the "active" state
+                self._init()
+                # New StallTracker starts out in the "active" state, which is what we
+                # want
             else:
                 self.stall_tracker.go_active()
 
         def after_task_step(self, _: trio.lowlevel.Task) -> None:
             if self.stall_tracker is None:
-                self.stall_tracker = StallTracker(
-                    "Trio run loop", threading.current_thread().ident
-                )
-                # New StallTracker starts out in the "active" state
+                self._init()
+                assert self.stall_tracker is not None
+                # New StallTracker starts out in the "active" state, so need to toggle
+                # it
             self.stall_tracker.go_idle()
 
+        def after_run(self) -> None:
+            self.stall_tracker.close()
+
     trio.lowlevel.add_instrument(TrioStallInstrument())
 
 
-def dwim() -> list[str]:
+def dwim(*, poll_interval: float | None = None) -> list[str]:
     did = []
 
     try:
         instrument_gil()
     except RuntimeError:
         pass
     else:
@@ -70,11 +94,11 @@
             instrument_trio()
         except RuntimeError:
             pass
         else:
             did.append("instrumented Trio")
 
     if did:
-        start_watcher()
+        start_watcher(poll_interval=poll_interval)
         did.append("started out of process watcher")
 
     return did
```

### Comparing `perpetuo-0.2.0/python/perpetuo.egg-info/PKG-INFO` & `perpetuo-0.3.0/python/perpetuo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.2.0
+Version: 0.3.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.2.0/src/shmem.rs` & `perpetuo-0.3.0/src/shmem.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#[allow(dead_code)]
-use anyhow::{bail, Result};
+use anyhow::{anyhow, bail, Result};
 use bytemuck::{Pod, Zeroable};
 use once_cell::sync::Lazy;
 use py_spy::StackTrace;
 use remoteprocess::ProcessMemory;
 use std::{
     mem::{align_of, size_of},
     sync::{
@@ -117,47 +116,56 @@
     // Safety: we're about to leak 'page', so we can cast its lifetime to 'static
     let static_slots: &'static mut _ = unsafe { std::mem::transmute(slots) };
     //eprintln!("set up slots in page at {page_raw_ptr:?}");
     std::mem::forget(page);
     static_slots
 }
 
-static UNUSED_SLOTS: Mutex<Option<&'static mut [StallTracker]>> = Mutex::new(None);
+static SLOT_FREELIST: Mutex<Option<Vec<&'static mut StallTracker>>> = Mutex::new(None);
 
 pub fn alloc_slot(name: &str, thread_hint: ThreadHint) -> Result<&'static mut StallTracker> {
-    let mut guard = UNUSED_SLOTS.lock().unwrap();
+    let mut guard = SLOT_FREELIST.lock().unwrap();
     if guard.is_none() {
-        *guard = Some(create_exported_slots());
+        *guard = Some(create_exported_slots().iter_mut().collect());
     }
 
     let string_to_leak = name.to_owned();
     let name_ptr = string_to_leak.as_str() as *const str as *const () as usize;
     let name_len = string_to_leak.len();
     std::mem::forget(string_to_leak);
     let metadata = SlotMetadata {
         name_ptr,
         name_len,
         thread_hint,
     };
 
-    let unused_slots: &'static mut [StallTracker] = guard.take().unwrap();
-    if unused_slots.is_empty() {
-        bail!("Ran out of stall tracker slots in the instrumentation page")
-    }
-    let (head, tail) = unused_slots.split_at_mut(1);
-    let slot = &mut head[0];
-    *guard = Some(tail);
+    let freelist = guard.as_mut().unwrap();
+
+    let slot = freelist.pop().ok_or_else(|| {
+        anyhow!("Ran out of stall tracker slots in the perpetuo instrumentation page")
+    })?;
+    assert!(!slot.is_active());
     slot.metadata = metadata;
     // Release ordering to ensure that 'metadata' update is published before the store
     // becomes visible, to maintain the invariant that out-of-process reads should never
-    // see a Slot with non-zero count + invalid metadata.
-    slot.count.store(1, Ordering::Release);
+    // see a Slot with odd count + invalid metadata.
+    slot.count.fetch_add(1, Ordering::Release);
     Ok(slot)
 }
 
+pub fn release_slot(slot: &'static mut StallTracker) -> Result<()> {
+    if slot.is_active() {
+        bail!("attempt to release active StallTracker");
+    }
+    let mut guard = SLOT_FREELIST.lock().unwrap();
+    let freelist = guard.as_mut().unwrap();
+    freelist.push(slot);
+    Ok(())
+}
+
 struct StallTrackerSnapshot {
     stall_tracker: StallTracker,
     last_updated: Instant,
 }
 
 pub struct PerpetuoProc {
     slots_ptr: usize,
```


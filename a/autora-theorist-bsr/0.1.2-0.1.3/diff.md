# Comparing `tmp/autora-theorist-bsr-0.1.2.tar.gz` & `tmp/autora-theorist-bsr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bsr-0.1.2.tar", last modified: Thu Apr 27 16:56:53 2023, max compression
+gzip compressed data, was "autora-theorist-bsr-0.1.3.tar", last modified: Thu Apr 27 18:13:27 2023, max compression
```

## Comparing `autora-theorist-bsr-0.1.2.tar` & `autora-theorist-bsr-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.090435 autora-theorist-bsr-0.1.2/
--rw-r--r--   0 benwandrew   (501) staff       (20)     2664 2023-04-27 16:56:53.089921 autora-theorist-bsr-0.1.2/PKG-INFO
--rw-r--r--   0 benwandrew   (501) staff       (20)     2204 2023-04-27 16:56:17.000000 autora-theorist-bsr-0.1.2/README.md
--rw-r--r--   0 benwandrew   (501) staff       (20)      652 2023-04-27 16:56:17.000000 autora-theorist-bsr-0.1.2/pyproject.toml
--rw-r--r--   0 benwandrew   (501) staff       (20)       38 2023-04-27 16:56:53.090599 autora-theorist-bsr-0.1.2/setup.cfg
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.074255 autora-theorist-bsr-0.1.2/src/
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.073921 autora-theorist-bsr-0.1.2/src/autora/
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.074051 autora-theorist-bsr-0.1.2/src/autora/theorist/
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.079136 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/
--rw-r--r--   0 benwandrew   (501) staff       (20)      107 2023-04-25 20:16:17.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/__init__.py
--rw-r--r--   0 benwandrew   (501) staff       (20)    32217 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/funcs.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     1430 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/misc.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     6521 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/node.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     2117 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/operation.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     5114 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/prior.py
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.082647 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/
--rw-r--r--   0 benwandrew   (501) staff       (20)     2664 2023-04-27 16:56:53.000000 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/PKG-INFO
--rw-r--r--   0 benwandrew   (501) staff       (20)      674 2023-04-27 16:56:53.000000 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/SOURCES.txt
--rw-r--r--   0 benwandrew   (501) staff       (20)        1 2023-04-27 16:56:53.000000 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/dependency_links.txt
--rw-r--r--   0 benwandrew   (501) staff       (20)       49 2023-04-27 16:56:53.000000 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/requires.txt
--rw-r--r--   0 benwandrew   (501) staff       (20)        7 2023-04-27 16:56:53.000000 autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/top_level.txt
-drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 16:56:53.089228 autora-theorist-bsr-0.1.2/tests/
--rw-r--r--   0 benwandrew   (501) staff       (20)     3703 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_1d_recovery.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     2555 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_2d_recovery.py
--rw-r--r--   0 benwandrew   (501) staff       (20)      121 2023-04-25 19:03:04.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_example.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     6672 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_mcmc_actions.py
--rw-r--r--   0 benwandrew   (501) staff       (20)     4048 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_node_and_operator.py
--rw-r--r--   0 benwandrew   (501) staff       (20)      546 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.2/tests/test_bsr_tree_operation.py
--rw-r--r--   0 benwandrew   (501) staff       (20)      121 2023-04-27 16:23:51.000000 autora-theorist-bsr-0.1.2/tests/test_theorist_bsr.py
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.436570 autora-theorist-bsr-0.1.3/
+-rw-r--r--   0 benwandrew   (501) staff       (20)     2698 2023-04-27 18:13:27.436030 autora-theorist-bsr-0.1.3/PKG-INFO
+-rw-r--r--   0 benwandrew   (501) staff       (20)     2204 2023-04-27 16:56:17.000000 autora-theorist-bsr-0.1.3/README.md
+-rw-r--r--   0 benwandrew   (501) staff       (20)      686 2023-04-27 18:13:21.000000 autora-theorist-bsr-0.1.3/pyproject.toml
+-rw-r--r--   0 benwandrew   (501) staff       (20)       38 2023-04-27 18:13:27.436972 autora-theorist-bsr-0.1.3/setup.cfg
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.402615 autora-theorist-bsr-0.1.3/src/
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.402140 autora-theorist-bsr-0.1.3/src/autora/
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.402343 autora-theorist-bsr-0.1.3/src/autora/theorist/
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.409764 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/
+-rw-r--r--   0 benwandrew   (501) staff       (20)      107 2023-04-25 20:16:17.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/__init__.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)    32217 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/funcs.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     1430 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/misc.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     6521 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/node.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     2117 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/operation.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     5114 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/prior.py
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.418882 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/
+-rw-r--r--   0 benwandrew   (501) staff       (20)     2698 2023-04-27 18:13:27.000000 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/PKG-INFO
+-rw-r--r--   0 benwandrew   (501) staff       (20)      674 2023-04-27 18:13:27.000000 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/SOURCES.txt
+-rw-r--r--   0 benwandrew   (501) staff       (20)        1 2023-04-27 18:13:27.000000 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/dependency_links.txt
+-rw-r--r--   0 benwandrew   (501) staff       (20)       49 2023-04-27 18:13:27.000000 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/requires.txt
+-rw-r--r--   0 benwandrew   (501) staff       (20)        7 2023-04-27 18:13:27.000000 autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/top_level.txt
+drwxr-xr-x   0 benwandrew   (501) staff       (20)        0 2023-04-27 18:13:27.435279 autora-theorist-bsr-0.1.3/tests/
+-rw-r--r--   0 benwandrew   (501) staff       (20)     3703 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_1d_recovery.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     2555 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_2d_recovery.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)      121 2023-04-25 19:03:04.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_example.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     6672 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_mcmc_actions.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)     4048 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_node_and_operator.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)      546 2023-04-25 17:56:22.000000 autora-theorist-bsr-0.1.3/tests/test_bsr_tree_operation.py
+-rw-r--r--   0 benwandrew   (501) staff       (20)      121 2023-04-27 16:23:51.000000 autora-theorist-bsr-0.1.3/tests/test_theorist_bsr.py
```

### Comparing `autora-theorist-bsr-0.1.2/PKG-INFO` & `autora-theorist-bsr-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bsr
-Version: 0.1.2
-Summary: AutoRA BSR Theorist
+Version: 0.1.3
+Summary: Bayesian Symbolic Regression Theorist (BSR) for AutoRA
 Author-email: Ben Andrew <benwallaceandrew@gmail.com>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bsr
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <3.11,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA BSR Theorist
```

### Comparing `autora-theorist-bsr-0.1.2/README.md` & `autora-theorist-bsr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/pyproject.toml` & `autora-theorist-bsr-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "autora-theorist-bsr"
-description = "AutoRA BSR Theorist"
+description = "Bayesian Symbolic Regression Theorist (BSR) for AutoRA"
 authors = [{ name = "Ben Andrew", email = "benwallaceandrew@gmail.com" }]
-version = "0.1.2"
+version = "0.1.3"
 
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8.10,<3.11"
 
 dependencies = [
     "autora-core",
@@ -15,14 +15,14 @@
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
 
 [project.urls]
-homepage = "https://www.empiricalresearch.ai"
+homepage = "http://www.empiricalresearch.ai"
 repository = "https://github.com/AutoResearch/autora-theorist-bsr"
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/funcs.py` & `autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/funcs.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/misc.py` & `autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/misc.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/node.py` & `autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/node.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/operation.py` & `autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/operation.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/src/autora/theorist/bsr/prior.py` & `autora-theorist-bsr-0.1.3/src/autora/theorist/bsr/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/PKG-INFO` & `autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bsr
-Version: 0.1.2
-Summary: AutoRA BSR Theorist
+Version: 0.1.3
+Summary: Bayesian Symbolic Regression Theorist (BSR) for AutoRA
 Author-email: Ben Andrew <benwallaceandrew@gmail.com>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bsr
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <3.11,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA BSR Theorist
```

### Comparing `autora-theorist-bsr-0.1.2/src/autora_theorist_bsr.egg-info/SOURCES.txt` & `autora-theorist-bsr-0.1.3/src/autora_theorist_bsr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/tests/test_bsr_1d_recovery.py` & `autora-theorist-bsr-0.1.3/tests/test_bsr_1d_recovery.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/tests/test_bsr_2d_recovery.py` & `autora-theorist-bsr-0.1.3/tests/test_bsr_2d_recovery.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/tests/test_bsr_mcmc_actions.py` & `autora-theorist-bsr-0.1.3/tests/test_bsr_mcmc_actions.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/tests/test_bsr_node_and_operator.py` & `autora-theorist-bsr-0.1.3/tests/test_bsr_node_and_operator.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-0.1.2/tests/test_bsr_tree_operation.py` & `autora-theorist-bsr-0.1.3/tests/test_bsr_tree_operation.py`

 * *Files identical despite different names*


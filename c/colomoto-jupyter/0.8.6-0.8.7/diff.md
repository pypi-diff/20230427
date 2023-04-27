# Comparing `tmp/colomoto_jupyter-0.8.6.tar.gz` & `tmp/colomoto_jupyter-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colomoto_jupyter-0.8.6.tar", last modified: Wed Apr 26 10:33:42 2023, max compression
+gzip compressed data, was "colomoto_jupyter-0.8.7.tar", last modified: Thu Apr 27 20:07:21 2023, max compression
```

## Comparing `colomoto_jupyter-0.8.6.tar` & `colomoto_jupyter-0.8.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/cellcollective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.354047 colomoto_jupyter-0.8.6/colomoto/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27199 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/minibn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/modelchecking.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/setup_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/temporal_logics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/colomoto_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/jupyter_ext.js
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/sessionfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/widget_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/wui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/espresso_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/itstools.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/itstools_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/nusmv.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/nusmv_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:07:21.988268 colomoto_jupyter-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 20:07:21.988268 colomoto_jupyter-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/cellcollective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:07:21.988268 colomoto_jupyter-0.8.7/colomoto/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/minibn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/modelchecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/setup_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/temporal_logics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:07:21.988268 colomoto_jupyter-0.8.7/colomoto_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/jupyter_ext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/sessionfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/widget_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/colomoto_jupyter/wui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:07:21.988268 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 20:07:21.000000 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 20:07:21.000000 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:07:21.000000 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 20:07:21.000000 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 20:07:21.000000 colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/espresso_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/itstools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/itstools_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/nusmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/nusmv_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:07:21.992268 colomoto_jupyter-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 20:07:10.000000 colomoto_jupyter-0.8.7/setup.py
```

### Comparing `colomoto_jupyter-0.8.6/PKG-INFO` & `colomoto_jupyter-0.8.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colomoto_jupyter
-Version: 0.8.6
+Version: 0.8.7
 Summary: CoLoMoTo helper functions for Juypter integration
 Home-page: https://github.com/colomoto/colomoto-jupyter
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: LGPL v3+/CeCILL-C
 Keywords: jupyter,computational systems biology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `colomoto_jupyter-0.8.6/README.md` & `colomoto_jupyter-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/cellcollective.py` & `colomoto_jupyter-0.8.7/cellcollective.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto/helpers.py` & `colomoto_jupyter-0.8.7/colomoto/helpers.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto/minibn.py` & `colomoto_jupyter-0.8.7/colomoto/minibn.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,25 +128,18 @@
                 v = self.ba.parse(v)
             if not isinstance(k, self.ba.Symbol):
                 k = self.v(k)
             ntr[k] = self._autobool(v)
         return ntr
 
     def __call__(self, cfg):
-        tr = self._normalize_tr(cfg)
-        def _autostate(expr):
-            if expr == self.ba.TRUE:
-                return 1
-            elif expr == self.ba.FALSE:
-                return 0
-            return expr
-        return {a: _autostate(self[a].subs(tr).simplify()) for a in self}
+        return {a: int(self[a](**cfg)) for a in self}
 
     def zero(self):
-        return {a:0 for a in self}
+        return {a: 0 for a in self}
 
     def rewrite(self, a, tr, simplify=True):
         tr = self._normalize_tr(tr)
         self[a] = self[a].subs(tr, simplify=simplify)
 
     def __setitem__(self, a, f):
         if isinstance(f, str):
```

### Comparing `colomoto_jupyter-0.8.6/colomoto/modelchecking.py` & `colomoto_jupyter-0.8.7/colomoto/modelchecking.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto/setup_helper.py` & `colomoto_jupyter-0.8.7/colomoto/setup_helper.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto/temporal_logics.py` & `colomoto_jupyter-0.8.7/colomoto/temporal_logics.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto/types.py` & `colomoto_jupyter-0.8.7/colomoto/types.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/__init__.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/formatters.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/formatters.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/io.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/io.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/jupyter_ext.js` & `colomoto_jupyter-0.8.7/colomoto_jupyter/jupyter_ext.js`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/sessionfiles.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/sessionfiles.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/upload.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/upload.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/widget_utils.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/widget_utils.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter/wui.py` & `colomoto_jupyter-0.8.7/colomoto_jupyter/wui.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/SOURCES.txt` & `colomoto_jupyter-0.8.7/colomoto_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/itstools.py` & `colomoto_jupyter-0.8.7/itstools.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/nusmv.py` & `colomoto_jupyter-0.8.7/nusmv.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.6/setup.py` & `colomoto_jupyter-0.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf8 -*-
 
 from setuptools import setup, find_packages
 
 NAME = "colomoto_jupyter"
 
 setup(name=NAME,
-    version='0.8.6',
+    version='0.8.7',
     author = "Loïc Paulevé",
     author_email = "loic.pauleve@ens-cachan.org",
     url = "https://github.com/colomoto/colomoto-jupyter",
     description = "CoLoMoTo helper functions for Juypter integration",
     long_description = """
 Provides helper functions for integration in the CoLoMoTo Jupyter notebook.
```


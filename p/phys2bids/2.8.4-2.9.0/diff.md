# Comparing `tmp/phys2bids-2.8.4.tar.gz` & `tmp/phys2bids-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phys2bids-2.8.4.tar", last modified: Wed Apr 26 22:56:47 2023, max compression
+gzip compressed data, was "dist/phys2bids-2.9.0.tar", last modified: Thu Apr 27 00:42:40 2023, max compression
```

## Comparing `phys2bids-2.8.4.tar` & `phys2bids-2.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (122)    68611 2023-04-26 22:56:31.000000 phys2bids-2.8.4/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (122)    20731 2023-04-26 22:56:47.000000 phys2bids-2.8.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (122)    13923 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_bids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4505 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7736 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    12153 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_physio_obj.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_phys2bids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/data/tutorial_file_INFO.json
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20501 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/phys2bids.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/due.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    26697 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/physio_obj.py
--rw-r--r--   0 runner    (1001) docker     (122)    17662 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/heuristics/
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_euskalibur.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/participant.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_test_multifreq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_test_acq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9045 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/viz.py
--rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/bids.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/slice4phys.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/cli/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 22:56:31.000000 phys2bids-2.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-26 22:56:31.000000 phys2bids-2.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20731 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-26 22:56:31.000000 phys2bids-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18538 2023-04-26 22:56:31.000000 phys2bids-2.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-04-26 22:56:47.000000 phys2bids-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-26 22:56:31.000000 phys2bids-2.8.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    68448 2023-04-27 00:42:20.000000 phys2bids-2.9.0/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20754 2023-04-27 00:42:40.000000 phys2bids-2.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14067 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4009 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8881 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11546 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_physio_obj.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2113 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/test_phys2bids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/tests/data/tutorial_file_INFO.json
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20702 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/phys2bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/due.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26780 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/physio_obj.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20773 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/heuristics/heur_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/heuristics/heur_euskalibur.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/heuristics/participant.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/heuristics/heur_test_multifreq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/heuristics/heur_test_acq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/viz.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10337 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9531 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6775 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/slice4phys.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5890 2023-04-27 00:42:20.000000 phys2bids-2.9.0/phys2bids/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-27 00:42:20.000000 phys2bids-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-27 00:42:20.000000 phys2bids-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20754 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-27 00:42:40.000000 phys2bids-2.9.0/phys2bids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-27 00:42:39.000000 phys2bids-2.9.0/phys2bids.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-27 00:42:20.000000 phys2bids-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18538 2023-04-27 00:42:20.000000 phys2bids-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-04-27 00:42:40.000000 phys2bids-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-27 00:42:20.000000 phys2bids-2.9.0/MANIFEST.in
```

### Comparing `phys2bids-2.8.4/versioneer.py` & `phys2bids-2.9.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,33 +304,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(me), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -344,14 +348,15 @@
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +373,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +423,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +1000,78 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        ["describe", "--tags", "--dirty", "--always", "--long", "--match", "%s*" % tag_prefix],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1086,50 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (full_tag, tag_prefix)
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1177,30 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1221,26 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1264,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1378,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1404,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1433,15 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1487,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1542,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1575,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1604,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1637,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1674,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(target_versionfile, self._versioneer_generated_versions)
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1730,37 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (EnvironmentError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1794,15 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(" appending versionfile_source ('%s') to MANIFEST.in" % cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

### Comparing `phys2bids-2.8.4/PKG-INFO` & `phys2bids-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2bids
-Version: 2.8.4
+Version: 2.9.0
 Summary: Python library to convert physiological data files into BIDS format
 Home-page: https://github.com/physiopy/phys2bids
 Author: phys2bids developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/physiopy/phys2bids
@@ -157,15 +157,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: phys2bids
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: doc
-Provides-Extra: interfaces
-Provides-Extra: acq
+Provides-Extra: mat
 Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: all
+Provides-Extra: spike2
 Provides-Extra: duecredit
 Provides-Extra: style
-Provides-Extra: mat
-Provides-Extra: all
+Provides-Extra: acq
+Provides-Extra: interfaces
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_viz.py` & `phys2bids-2.9.0/phys2bids/tests/test_viz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import os
 
 import pytest
 
-from phys2bids import io
-from phys2bids import viz
+from phys2bids import io, viz
 
 
 def test_plot_all(samefreq_full_acq_file):
     chtrig = 3
     test_path, test_filename = os.path.split(samefreq_full_acq_file)
     phys_obj = io.load_acq(samefreq_full_acq_file, chtrig)
-    viz.plot_all(phys_obj.ch_name, phys_obj.timeseries, phys_obj.units,
-                 phys_obj.freq, test_filename, outfile=test_path)
-    assert os.path.isfile(os.path.join(test_path,
-                          os.path.splitext(os.path.basename(test_filename))[0] + '.png'))
+    viz.plot_all(
+        phys_obj.ch_name,
+        phys_obj.timeseries,
+        phys_obj.units,
+        phys_obj.freq,
+        test_filename,
+        outfile=test_path,
+    )
+    assert os.path.isfile(
+        os.path.join(test_path, os.path.splitext(os.path.basename(test_filename))[0] + ".png")
+    )
 
 
 # Expected to fail due to trigger plot issue
 @pytest.mark.xfail
 def test_plot_trigger(samefreq_full_acq_file):
     chtrig = 3
     test_path, test_filename = os.path.split(samefreq_full_acq_file)
-    out = os.path.join(test_path, 'Test_belt_pulse_samefreq')
+    out = os.path.join(test_path, "Test_belt_pulse_samefreq")
     phys_obj = io.load_acq(samefreq_full_acq_file, chtrig)
-    viz.plot_trigger(phys_obj.timeseries[0], phys_obj.timeseries[chtrig],
-                     out, 1.5, 1.6, 60, test_filename)
-    assert os.path.isfile(out + '_trigger_time.png')
+    viz.plot_trigger(
+        phys_obj.timeseries[0], phys_obj.timeseries[chtrig], out, 1.5, 1.6, 60, test_filename
+    )
+    assert os.path.isfile(out + "_trigger_time.png")
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_integration.py` & `phys2bids-2.9.0/phys2bids/tests/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,346 +2,380 @@
 import json
 import math
 import re
 import shutil
 import subprocess
 from os import remove
 from os.path import isfile, join, split
-from pkg_resources import resource_filename
 
 import pytest
+from pkg_resources import resource_filename
 
 from phys2bids._version import get_versions
 from phys2bids.phys2bids import phys2bids
 
 
 def check_string(str_container, str_to_find, str_expected, is_num=True):
-    idx = [log_idx for log_idx, log_str in enumerate(
-                      str_container) if str_to_find in log_str]
+    idx = [log_idx for log_idx, log_str in enumerate(str_container) if str_to_find in log_str]
     str_found = str_container[idx[0]]
     if is_num:
         num_found = re.findall(r"[-+]?\d*\.\d+|\d+", str_found)
         return str_expected in num_found
     else:
         return str_expected in str_found
 
 
 def test_integration_acq(skip_integration, samefreq_full_acq_file):
     """
     Does the integration test for an acq file
     """
 
     if skip_integration:
-        pytest.skip('Skipping integration test')
+        pytest.skip("Skipping integration test")
 
     test_path, test_filename = split(samefreq_full_acq_file)
     test_chtrig = 3
-    conversion_path = join(test_path, 'code', 'conversion')
+    conversion_path = join(test_path, "code", "conversion")
 
-    phys2bids(filename=test_filename, indir=test_path, outdir=test_path,
-              chtrig=test_chtrig, num_timepoints_expected=60, tr=1.5)
+    phys2bids(
+        filename=test_filename,
+        indir=test_path,
+        outdir=test_path,
+        chtrig=test_chtrig,
+        num_timepoints_expected=60,
+        tr=1.5,
+    )
 
     # Check that files are generated
-    for suffix in ['.json', '.tsv.gz']:
-        assert isfile(join(test_path, 'Test_belt_pulse_samefreq' + suffix))
+    for suffix in [".json", ".tsv.gz"]:
+        assert isfile(join(test_path, "Test_belt_pulse_samefreq" + suffix))
 
     # Check files in extra are generated
-    for suffix in ['.log']:
-        assert isfile(join(conversion_path, 'Test_belt_pulse_samefreq' + suffix))
+    for suffix in [".log"]:
+        assert isfile(join(conversion_path, "Test_belt_pulse_samefreq" + suffix))
 
     # Read log file (note that this file is not the logger file)
-    with open(join(conversion_path, 'Test_belt_pulse_samefreq.log')) as log_info:
+    with open(join(conversion_path, "Test_belt_pulse_samefreq.log")) as log_info:
         log_info = log_info.readlines()
 
     # Check timepoints expected
-    assert check_string(log_info, 'Timepoints expected', '60')
+    assert check_string(log_info, "Timepoints expected", "60")
     # Check timepoints found
-    assert check_string(log_info, 'Timepoints found', '60')
+    assert check_string(log_info, "Timepoints found", "60")
     # Check sampling frequency
-    assert check_string(log_info, 'Sampling Frequency', '10000.0')
+    assert check_string(log_info, "Sampling Frequency", "10000.0")
     # Check sampling started
-    assert check_string(log_info, 'Sampling started', '10.4251')
+    assert check_string(log_info, "Sampling started", "10.4251")
     # Check start time
-    assert check_string(log_info, 'first trigger', 'Time 0', is_num=False)
+    assert check_string(log_info, "first trigger", "Time 0", is_num=False)
 
     # Checks json file
-    with open(join(test_path, 'Test_belt_pulse_samefreq.json')) as json_file:
+    with open(join(test_path, "Test_belt_pulse_samefreq.json")) as json_file:
         json_data = json.load(json_file)
 
     # Compares values in json file with ground truth
-    assert math.isclose(json_data['SamplingFrequency'], 10000.0)
-    assert math.isclose(json_data['StartTime'], 10.4251)
-    assert json_data['Columns'] == ['time', 'RESP - RSP100C', 'PULSE - Custom, DA100C',
-                                    'MR TRIGGER - Custom, HLT100C - A 5', 'PPG100C', 'CO2', 'O2']
+    assert math.isclose(json_data["SamplingFrequency"], 10000.0)
+    assert math.isclose(json_data["StartTime"], 10.4251)
+    assert json_data["Columns"] == [
+        "time",
+        "RESP - RSP100C",
+        "PULSE - Custom, DA100C",
+        "MR TRIGGER - Custom, HLT100C - A 5",
+        "PPG100C",
+        "CO2",
+        "O2",
+    ]
 
     # Remove generated files
-    for filename in glob.glob(join(conversion_path, 'phys2bids*')):
+    for filename in glob.glob(join(conversion_path, "phys2bids*")):
         remove(filename)
-    for filename in glob.glob(join(test_path, 'Test_belt_pulse_samefreq*')):
+    for filename in glob.glob(join(test_path, "Test_belt_pulse_samefreq*")):
         remove(filename)
     shutil.rmtree(conversion_path)
 
 
 def test_integration_heuristic(skip_integration, multifreq_lab_file):
     """
     Does integration test of tutorial file with heurositics
     """
 
     if skip_integration:
-        pytest.skip('Skipping integration test')
+        pytest.skip("Skipping integration test")
 
     test_path, test_filename = split(multifreq_lab_file)
     test_full_path = join(test_path, test_filename)
     test_chtrig = 1
     test_outdir = test_path
-    conversion_path = join(test_path, 'code', 'conversion')
+    conversion_path = join(test_path, "code", "conversion")
     test_ntp = 30
     test_tr = 1.2
     test_thr = 0.735
-    heur_path = resource_filename('phys2bids', 'heuristics')
-    test_heur = join(heur_path, 'heur_test_multifreq.py')
+    heur_path = resource_filename("phys2bids", "heuristics")
+    test_heur = join(heur_path, "heur_test_multifreq.py")
 
     # Move into folder
-    subprocess.run(f'cd {test_path}', shell=True, check=True)
+    subprocess.run(f"cd {test_path}", shell=True, check=True)
     # Phys2bids call through terminal
-    command_str = (f'phys2bids -in {test_full_path} ',
-                   f'-chtrig {test_chtrig} -outdir {test_outdir} ',
-                   f'-tr {test_tr} -ntp {test_ntp} -thr {test_thr} ',
-                   f'-sub 006 -ses 01 -heur {test_heur}')
-    command_str = ''.join(command_str)
+    command_str = (
+        f"phys2bids -in {test_full_path} ",
+        f"-chtrig {test_chtrig} -outdir {test_outdir} ",
+        f"-tr {test_tr} -ntp {test_ntp} -thr {test_thr} ",
+        f"-sub 006 -ses 01 -heur {test_heur}",
+    )
+    command_str = "".join(command_str)
     subprocess.run(command_str, shell=True, check=True)
 
     # Check that call.sh is generated
-    assert isfile(join(conversion_path, 'call.sh'))
+    assert isfile(join(conversion_path, "call.sh"))
 
     # Read logger file
-    logger_file = glob.glob(join(conversion_path, '*phys2bids*'))[0]
+    logger_file = glob.glob(join(conversion_path, "*phys2bids*"))[0]
     with open(logger_file) as logger_info:
         logger_info = logger_info.readlines()
 
     # Get version info
     current_version = get_versions()
-    assert check_string(logger_info, 'phys2bids version', current_version['version'], is_num=False)
+    assert check_string(logger_info, "phys2bids version", current_version["version"], is_num=False)
 
-    assert check_string(logger_info, '01. Trigger; sampled at', '1000.0')
+    assert check_string(logger_info, "01. Trigger; sampled at", "1000.0")
     # Should be 500.0 for sampling, but new faster multifreq version does not detect it.
-    assert check_string(logger_info, '04. Belt; sampled at', '1000.0')
+    assert check_string(logger_info, "04. Belt; sampled at", "1000.0")
 
     # Check that files are generated in conversion path
     # There should be a 500 too, but labchart export doesn't work well.
-    for freq in ['40', '100', '1000']:
-        assert isfile(join(conversion_path,
-                           'sub-006_ses-01_task-test_rec-biopac_run-01_'
-                           f'recording-{freq}Hz_physio.log'))
+    for freq in ["40", "100", "1000"]:
+        assert isfile(
+            join(
+                conversion_path,
+                "sub-006_ses-01_task-test_rec-biopac_run-01_" f"recording-{freq}Hz_physio.log",
+            )
+        )
     # assert isfile(join(conversion_path,
     #                    'Test1_multifreq_onescan_sub-006_ses-01_trigger_time.png'))
-    assert isfile(join(conversion_path, 'Test1_multifreq_onescan.png'))
-    assert isfile(join(conversion_path, 'heur_test_multifreq.py'))
-    test_path_output = join(test_path, 'sub-006/ses-01/func')
+    assert isfile(join(conversion_path, "Test1_multifreq_onescan.png"))
+    assert isfile(join(conversion_path, "heur_test_multifreq.py"))
+    test_path_output = join(test_path, "sub-006/ses-01/func")
 
     # Check that files are generated
-    base_filename = 'sub-006_ses-01_task-test_rec-biopac_run-01_recording-'
-    for suffix in ['.json', '.tsv.gz']:
+    base_filename = "sub-006_ses-01_task-test_rec-biopac_run-01_recording-"
+    for suffix in [".json", ".tsv.gz"]:
         # There should be a 500 too, but labchart export doesn't work well.
-        for freq in ['40', '100', '1000']:
-            assert isfile(join(test_path_output,
-                               f'{base_filename}{freq}Hz_physio{suffix}'))
+        for freq in ["40", "100", "1000"]:
+            assert isfile(join(test_path_output, f"{base_filename}{freq}Hz_physio{suffix}"))
 
     # ##### Checks for 40 Hz files
     # Read log file (note that this file is not the logger file)
-    log_filename = 'sub-006_ses-01_task-test_rec-biopac_run-01_recording-40Hz_physio.log'
+    log_filename = "sub-006_ses-01_task-test_rec-biopac_run-01_recording-40Hz_physio.log"
     with open(join(conversion_path, log_filename)) as log_info:
         log_info = log_info.readlines()
 
     # Check timepoints expected
-    assert check_string(log_info, 'Timepoints expected', '30')
+    assert check_string(log_info, "Timepoints expected", "30")
     # Check timepoints found
-    assert check_string(log_info, 'Timepoints found', '30')
+    assert check_string(log_info, "Timepoints found", "30")
     # Check sampling frequency
-    assert check_string(log_info, 'Sampling Frequency', '40.0')
+    assert check_string(log_info, "Sampling Frequency", "40.0")
     # Check sampling started
-    assert check_string(log_info, 'Sampling started', '3.6960')
+    assert check_string(log_info, "Sampling started", "3.6960")
     # Check first trigger
-    assert check_string(log_info, 'first trigger', 'Time 0', is_num=False)
+    assert check_string(log_info, "first trigger", "Time 0", is_num=False)
 
     # Checks json file
-    json_filename = 'sub-006_ses-01_task-test_rec-biopac_run-01_recording-40Hz_physio.json'
+    json_filename = "sub-006_ses-01_task-test_rec-biopac_run-01_recording-40Hz_physio.json"
     with open(join(test_path_output, json_filename)) as json_file:
         json_data = json.load(json_file)
 
     # Compares values in json file with ground truth
-    assert math.isclose(json_data['SamplingFrequency'], 40.0,)
-    assert math.isclose(json_data['StartTime'], 3.6960,)
-    assert json_data['Columns'] == ['time', 'Trigger', 'O2']
+    assert math.isclose(
+        json_data["SamplingFrequency"],
+        40.0,
+    )
+    assert math.isclose(
+        json_data["StartTime"],
+        3.6960,
+    )
+    assert json_data["Columns"] == ["time", "Trigger", "O2"]
 
     # ##### Checks for 100 Hz files
     # Read log file (note that this file is not the logger file)
-    log_filename = 'sub-006_ses-01_task-test_rec-biopac_run-01_recording-100Hz_physio.log'
+    log_filename = "sub-006_ses-01_task-test_rec-biopac_run-01_recording-100Hz_physio.log"
     with open(join(conversion_path, log_filename)) as log_info:
         log_info = log_info.readlines()
 
     # Check timepoints expected
-    assert check_string(log_info, 'Timepoints expected', '30')
+    assert check_string(log_info, "Timepoints expected", "30")
     # Check timepoints found
-    assert check_string(log_info, 'Timepoints found', '30')
+    assert check_string(log_info, "Timepoints found", "30")
     # Check sampling frequency
-    assert check_string(log_info, 'Sampling Frequency', '100.0')
+    assert check_string(log_info, "Sampling Frequency", "100.0")
     # Check sampling started
-    assert check_string(log_info, 'Sampling started', '3.6960')
+    assert check_string(log_info, "Sampling started", "3.6960")
     # Check first trigger
-    assert check_string(log_info, 'first trigger', 'Time 0', is_num=False)
+    assert check_string(log_info, "first trigger", "Time 0", is_num=False)
 
     # Checks json file
-    json_filename = 'sub-006_ses-01_task-test_rec-biopac_run-01_recording-100Hz_physio.json'
+    json_filename = "sub-006_ses-01_task-test_rec-biopac_run-01_recording-100Hz_physio.json"
     with open(join(test_path_output, json_filename)) as json_file:
         json_data = json.load(json_file)
 
     # Compares values in json file with ground truth
-    assert math.isclose(json_data['SamplingFrequency'], 100.0,)
-    assert math.isclose(json_data['StartTime'], 3.6960,)
-    assert json_data['Columns'] == ['time', 'Trigger', 'CO2']
+    assert math.isclose(
+        json_data["SamplingFrequency"],
+        100.0,
+    )
+    assert math.isclose(
+        json_data["StartTime"],
+        3.6960,
+    )
+    assert json_data["Columns"] == ["time", "Trigger", "CO2"]
 
     # Remove generated files
     shutil.rmtree(test_path_output)
     shutil.rmtree(conversion_path)
-    for filename in glob.glob(join(test_path, 'Test1_multifreq_onescan*')):
+    for filename in glob.glob(join(test_path, "Test1_multifreq_onescan*")):
         remove(filename)
 
 
 def test_integration_multirun(skip_integration, multi_run_file):
-
     if skip_integration:
-        pytest.skip('Skipping integration test')
+        pytest.skip("Skipping integration test")
 
     test_path, test_filename = split(multi_run_file)
     test_chtrig = 1
-    conversion_path = join(test_path, 'code', 'conversion')
+    conversion_path = join(test_path, "code", "conversion")
 
-    phys2bids(filename=test_filename, indir=test_path, outdir=test_path,
-              chtrig=test_chtrig, num_timepoints_expected=[534, 513], tr=[1.2, 1.2])
+    phys2bids(
+        filename=test_filename,
+        indir=test_path,
+        outdir=test_path,
+        chtrig=test_chtrig,
+        num_timepoints_expected=[534, 513],
+        tr=[1.2, 1.2],
+    )
 
     # Check that files are generated in outdir
-    base_filename = 'Test2_samefreq_TWOscans_'
-    for suffix in ['.json', '.tsv.gz']:
-        for run in ['01', '02']:
-            assert isfile(join(test_path, f'{base_filename}{run}{suffix}'))
+    base_filename = "Test2_samefreq_TWOscans_"
+    for suffix in [".json", ".tsv.gz"]:
+        for run in ["01", "02"]:
+            assert isfile(join(test_path, f"{base_filename}{run}{suffix}"))
 
-    assert isfile(join(test_path, 'Test2_samefreq_TWOscans.txt'))
+    assert isfile(join(test_path, "Test2_samefreq_TWOscans.txt"))
 
     # Check that files are generated in conversion_path
-    for run in ['01', '02']:
-        assert isfile(join(conversion_path, f'Test2_samefreq_TWOscans_{run}.log'))
+    for run in ["01", "02"]:
+        assert isfile(join(conversion_path, f"Test2_samefreq_TWOscans_{run}.log"))
 
     # Check that plots are generated in conversion_path
     # base_filename = 'Test2_samefreq_TWOscans_'
     # for run in ['1', '2']:
     #     assert isfile(join(conversion_path, f'Test2_samefreq_TWOscans_{run}_trigger_time.png'))
-    assert isfile(join(conversion_path, 'Test2_samefreq_TWOscans.png'))
+    assert isfile(join(conversion_path, "Test2_samefreq_TWOscans.png"))
+
 
 def test_integration_gep_onefile(skip_integration, ge_one_gep_file):
     """
     Does the integration test for a single GE file
     Input file is PPG
     """
 
     if skip_integration:
-        pytest.skip('Skipping integration test')
+        pytest.skip("Skipping integration test")
 
     test_path, test_filename = split(ge_one_gep_file)
-    conversion_path = join(test_path, 'code', 'conversion')
+    conversion_path = join(test_path, "code", "conversion")
 
     phys2bids(filename=test_filename, indir=test_path, outdir=test_path)
 
     # Check that files are generated
-    for suffix in ['.json', '.tsv.gz']:
+    for suffix in [".json", ".tsv.gz"]:
         assert isfile(join(test_path, test_filename[:-4] + suffix))
 
     # Check files in extra are generated
-    for suffix in ['.log']:
+    for suffix in [".log"]:
         assert isfile(join(conversion_path, test_filename[:-4] + suffix))
 
     # Read log file (note that this file is not the logger file)
-    with open(join(conversion_path, test_filename[:-4] + '.log')) as log_info:
+    with open(join(conversion_path, test_filename[:-4] + ".log")) as log_info:
         log_info = log_info.readlines()
 
     # Check timepoints expected
-    assert check_string(log_info, 'Timepoints expected', 'None', is_num=False)
+    assert check_string(log_info, "Timepoints expected", "None", is_num=False)
     # Check timepoints found
-    assert check_string(log_info, 'Timepoints found', 'None', is_num=False)
+    assert check_string(log_info, "Timepoints found", "None", is_num=False)
     # Check sampling frequency
-    assert check_string(log_info, 'Sampling Frequency', '100')
+    assert check_string(log_info, "Sampling Frequency", "100")
     # Check sampling started
-    assert check_string(log_info, 'Sampling started', '30.0000')
+    assert check_string(log_info, "Sampling started", "30.0000")
     # Check start time
-    assert check_string(log_info, 'first trigger', 'Time 0', is_num=False)
+    assert check_string(log_info, "first trigger", "Time 0", is_num=False)
 
     # Checks json file
-    with open(join(test_path, test_filename[:-4] + '.json')) as json_file:
+    with open(join(test_path, test_filename[:-4] + ".json")) as json_file:
         json_data = json.load(json_file)
 
     # Compares values in json file with ground truth
-    assert math.isclose(json_data['SamplingFrequency'], 100)
-    assert math.isclose(json_data['StartTime'], 30.0)
-    assert json_data['Columns'] == ['time', 'trigger', 'cardiac']
+    assert math.isclose(json_data["SamplingFrequency"], 100)
+    assert math.isclose(json_data["StartTime"], 30.0)
+    assert json_data["Columns"] == ["time", "trigger", "cardiac"]
 
     # Remove generated files
-    for filename in glob.glob(join(conversion_path, 'phys2bids*')):
+    for filename in glob.glob(join(conversion_path, "phys2bids*")):
         remove(filename)
-    for filename in glob.glob(join(test_path, test_filename+'*')):
+    for filename in glob.glob(join(test_path, test_filename + "*")):
         remove(filename)
     shutil.rmtree(conversion_path)
 
 
 def test_integration_gep_multifile(skip_integration, ge_two_gep_files_ppg):
     """
     Does the integration test for a set of two GE files
     Input file is PPG with RESP file also in folder
     """
 
     if skip_integration:
-        pytest.skip('Skipping integration test')
+        pytest.skip("Skipping integration test")
 
     test_path, test_filename = split(ge_two_gep_files_ppg)
-    conversion_path = join(test_path, 'code', 'conversion')
+    conversion_path = join(test_path, "code", "conversion")
 
     phys2bids(filename=test_filename, indir=test_path, outdir=test_path)
 
     # Check that files are generated
-    for suffix in ['.json', '.tsv.gz']:
-        assert isfile(join(test_path, test_filename[:-4] + '_100Hz' + suffix))
-        assert isfile(join(test_path, test_filename[:-4] + '_25Hz' + suffix))
+    for suffix in [".json", ".tsv.gz"]:
+        assert isfile(join(test_path, test_filename[:-4] + "_100Hz" + suffix))
+        assert isfile(join(test_path, test_filename[:-4] + "_25Hz" + suffix))
 
     # Check files in extra are generated
-    for suffix in ['.log']:
-        assert isfile(join(conversion_path, test_filename[:-4] + '_100Hz' + suffix))
-        assert isfile(join(conversion_path, test_filename[:-4] + '_25Hz' + suffix))
+    for suffix in [".log"]:
+        assert isfile(join(conversion_path, test_filename[:-4] + "_100Hz" + suffix))
+        assert isfile(join(conversion_path, test_filename[:-4] + "_25Hz" + suffix))
 
     # Read log file (note that this file is not the logger file)
-    with open(join(conversion_path, test_filename[:-4] + '_100Hz.log')) as log_info:
+    with open(join(conversion_path, test_filename[:-4] + "_100Hz.log")) as log_info:
         log_info = log_info.readlines()
 
     # Check timepoints expected
-    assert check_string(log_info, 'Timepoints expected', 'None', is_num=False)
+    assert check_string(log_info, "Timepoints expected", "None", is_num=False)
     # Check timepoints found
-    assert check_string(log_info, 'Timepoints found', 'None', is_num=False)
+    assert check_string(log_info, "Timepoints found", "None", is_num=False)
     # Check sampling frequency
-    assert check_string(log_info, 'Sampling Frequency', '100')
+    assert check_string(log_info, "Sampling Frequency", "100")
     # Check sampling started
-    assert check_string(log_info, 'Sampling started', '30.0000')
+    assert check_string(log_info, "Sampling started", "30.0000")
     # Check start time
-    assert check_string(log_info, 'first trigger', 'Time 0', is_num=False)
+    assert check_string(log_info, "first trigger", "Time 0", is_num=False)
 
     # Checks json file
-    with open(join(test_path, test_filename[:-4] + '_100Hz.json')) as json_file:
+    with open(join(test_path, test_filename[:-4] + "_100Hz.json")) as json_file:
         json_data = json.load(json_file)
 
     # Compares values in json file with ground truth
-    assert math.isclose(json_data['SamplingFrequency'], 100)
-    assert math.isclose(json_data['StartTime'], 30.0)
-    assert json_data['Columns'] == ['time', 'trigger', 'cardiac']
+    assert math.isclose(json_data["SamplingFrequency"], 100)
+    assert math.isclose(json_data["StartTime"], 30.0)
+    assert json_data["Columns"] == ["time", "trigger", "cardiac"]
 
     # Remove generated files
-    for filename in glob.glob(join(conversion_path, 'phys2bids*')):
+    for filename in glob.glob(join(conversion_path, "phys2bids*")):
         remove(filename)
-    for filename in glob.glob(join(test_path, test_filename+'*')):
+    for filename in glob.glob(join(test_path, test_filename + "*")):
         remove(filename)
     shutil.rmtree(conversion_path)
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_utils.py` & `phys2bids-2.9.0/phys2bids/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,124 @@
 """
     Runs unit tests on utils.py
 """
 
 import json
 import os
 from csv import reader
+
 from pytest import raises
 
 from phys2bids import utils
 
 
 # Tests check_input_ext
 def test_check_input_ext():
-    test_filename = 'help'
-    ext = 'py'
+    test_filename = "help"
+    ext = "py"
     out_filename = utils.check_input_ext(test_filename, ext)
-    assert str(out_filename) == f'{test_filename}.{ext}'
+    assert str(out_filename) == f"{test_filename}.{ext}"
 
-    test_filename = 'help.txt.gz'
-    assert str(utils.check_input_ext(test_filename, ext)) == 'help.py'
+    test_filename = "help.txt.gz"
+    assert str(utils.check_input_ext(test_filename, ext)) == "help.py"
 
 
 # Tests check_input_type
 def test_check_input_type(testpath, samefreq_full_acq_file):
     assert utils.check_input_type(samefreq_full_acq_file, testpath)
 
     with raises(Exception) as errorinfo:
-        utils.check_input_type('nobel_prize.win', testpath)
+        utils.check_input_type("nobel_prize.win", testpath)
     assert "was not found" in str(errorinfo.value)
 
 
 # Tests check_file_exists
 def test_check_file_exists(samefreq_full_acq_file):
     utils.check_file_exists(samefreq_full_acq_file)
 
     with raises(Exception) as errorinfo:
-        utils.check_file_exists('')
-    assert 'does not exist' in str(errorinfo.value)
+        utils.check_file_exists("")
+    assert "does not exist" in str(errorinfo.value)
 
 
 # Tests copy_file
 def test_copy_file(tmpdir):
-    ext = '.txt'
-    test_old_path = tmpdir.join('foo.txt')
-    test_new_path = tmpdir.join('mrmeeseeks')
-    open(f'{test_old_path}.txt', 'a').close()
+    ext = ".txt"
+    test_old_path = tmpdir.join("foo.txt")
+    test_new_path = tmpdir.join("mrmeeseeks")
+    open(f"{test_old_path}.txt", "a").close()
     utils.copy_file(test_old_path, test_new_path, ext)
 
 
 # Tests write_file
 def test_write_file(tmpdir):
-    ext = '.txt'
-    test_old_path = tmpdir.join('foo.txt')
-    test_text = 'Wubba lubba dub dub!'
+    ext = ".txt"
+    test_old_path = tmpdir.join("foo.txt")
+    test_text = "Wubba lubba dub dub!"
     utils.write_file(test_old_path, ext, test_text)
 
 
 # Tests write_json
 def test_write_json(tmpdir):
-    test_json_filename = tmpdir.join('foo')
-    test_json_data = dict(SamplingFrequency=42,
-                          StartTime='00:00 ET',
-                          Columns='Rick')
+    test_json_filename = tmpdir.join("foo")
+    test_json_data = dict(SamplingFrequency=42, StartTime="00:00 ET", Columns="Rick")
     utils.write_json(str(test_json_filename), test_json_data, indent=4, sort_keys=False)
-    test_json_filename += '.json'
+    test_json_filename += ".json"
     assert os.path.isfile(test_json_filename)
-    with open(test_json_filename, 'r') as src:
+    with open(test_json_filename, "r") as src:
         loaded_data = json.load(src)
     assert test_json_data == loaded_data
 
 
 # Tests load_heuristics
 def test_load_heuristics():
-    test_heuristic = 'heur_test_acq'
+    test_heuristic = "heur_test_acq"
     heuristic_output_filename = utils.load_heuristic(test_heuristic).filename
     assert test_heuristic in heuristic_output_filename
 
     with raises(Exception) as errorinfo:
-        utils.load_heuristic('')
-    assert 'Failed to import heuristic' in str(errorinfo.value)
+        utils.load_heuristic("")
+    assert "Failed to import heuristic" in str(errorinfo.value)
 
 
 # Test writing rows util
 def test_append_list_as_row(tmpdir):
-    file_name = tmpdir.join('test_row.tsv')
-    list_of_elem = ["01", "32", 'some_info', "132.98", 'M']
+    file_name = tmpdir.join("test_row.tsv")
+    list_of_elem = ["01", "32", "some_info", "132.98", "M"]
     utils.append_list_as_row(file_name, list_of_elem)
-    with open(file_name, mode='r') as tsv:
+    with open(file_name, mode="r") as tsv:
         tsv_read = reader(tsv, delimiter="\t")
         for row in tsv_read:
             assert row == list_of_elem
 
 
 # Test check_ge's ability to catch improperly formatted GE files
 def test_check_ge_bad_files(ge_badfiles):
     str_fname = os.path.split(ge_badfiles)
 
     # Catch string
     with raises(Exception) as errorinfo:
         utils.check_ge(str_fname[1], str_fname[0])
-    assert 'not numerical' in str(errorinfo.value)
+    assert "not numerical" in str(errorinfo.value)
 
     # Catch multiple columns in csv file
     with raises(Exception) as errorinfo:
-        utils.check_ge('PPGData_epiRT_columnscsv_00_00_000',
-                       str_fname[0])
-    assert 'not numerical' in str(errorinfo.value)
+        utils.check_ge("PPGData_epiRT_columnscsv_00_00_000", str_fname[0])
+    assert "not numerical" in str(errorinfo.value)
 
     # Catch multiple columns in tsv file
     with raises(Exception) as errorinfo:
-        utils.check_ge('PPGData_epiRT_columnstsv_00_00_000',
-                       str_fname[0])
-    assert 'multiple columns' in str(errorinfo.value)
+        utils.check_ge("PPGData_epiRT_columnstsv_00_00_000", str_fname[0])
+    assert "multiple columns" in str(errorinfo.value)
 
 
 # Test that check_ge adds suffix to files appropriately
 def test_check_ge_add_suffix(ge_one_raw_file, ge_two_raw_files):
     # Single file
     in_fname = os.path.split(ge_one_raw_file)
-    utils.check_ge('PPGData_epiRT_0000000000_00_00_000', in_fname[0])
-    assert os.path.isfile(os.path.join(in_fname[0], in_fname[1]+'.gep'))
+    utils.check_ge("PPGData_epiRT_0000000000_00_00_000", in_fname[0])
+    assert os.path.isfile(os.path.join(in_fname[0], in_fname[1] + ".gep"))
 
     # Multiple files
     in_fname = os.path.split(ge_two_raw_files)
-    utils.check_ge('PPGData_epiRT_0000000000_00_00_000', in_fname[0])
-    assert os.path.isfile(os.path.join(in_fname[0],
-                                       'RESPData_epiRT_0000000000_00_00_000.gep'))
+    utils.check_ge("PPGData_epiRT_0000000000_00_00_000", in_fname[0])
+    assert os.path.isfile(os.path.join(in_fname[0], "RESPData_epiRT_0000000000_00_00_000.gep"))
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_io.py` & `phys2bids-2.9.0/phys2bids/tests/test_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,83 @@
-from phys2bids import io
-
-import os
 import math
+import os
+import sys
+
 import numpy as np
 import pytest
 from pytest import raises
 
+from phys2bids import io
+
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def loaded_acq_file(samefreq_short_txt_file):
     chtrig = 2
     header_acq, channels_acq = io.read_header_and_channels(samefreq_short_txt_file)
 
     # just a few quick checks to make sure the data loaded correctly
     assert len(header_acq) == 9  # check proper header length
     assert len(channels_acq[0]) == 1048559  # check proper number of timepoints
     assert len(header_acq[-1]) == 2  # check extra line is deleted
-    assert 'acq' in header_acq[0][0]
+    assert "acq" in header_acq[0][0]
 
     return header_acq, channels_acq, chtrig
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def loaded_lab_file(multifreq_lab_file):
     chtrig = 1
     header_lab, channels_lab = io.read_header_and_channels(multifreq_lab_file)
 
     # just a few quick checks to make sure the data loaded correctly
     assert len(channels_lab) == 5
-    assert 'Interval=' in header_lab[0]
+    assert "Interval=" in header_lab[0]
 
     return header_lab, channels_lab, chtrig
 
 
 def test_load_txt(samefreq_short_txt_file, multifreq_lab_file):
     # testing for AcqKnowledge files
     io.load_txt(samefreq_short_txt_file, chtrig=2)
     # testing for LabChart files
     io.load_txt(multifreq_lab_file, chtrig=1)
 
 
-@pytest.mark.parametrize('units, expected', [
-    ('1 µsec/sample', 1000000),
-    ('1 msec/sample', 1000),
-    ('0.01 sec/sample', 100),
-    ('0.001 min/sample', 100 / 6),
-    ('100 Hz', 100),
-    ('1 kHz', 1000),
-    ('1 MHz', 1000000)
-])
+@pytest.mark.parametrize(
+    "units, expected",
+    [
+        ("1 µsec/sample", 1000000),
+        ("1 msec/sample", 1000),
+        ("0.01 sec/sample", 100),
+        ("0.001 min/sample", 100 / 6),
+        ("100 Hz", 100),
+        ("1 kHz", 1000),
+        ("1 MHz", 1000000),
+    ],
+)
 def test_generate_blueprint_for_acq(loaded_acq_file, units, expected):
     header, channels, chtrig = loaded_acq_file
 
     # set units to test that expected frequency is generated correctly
     header[1][0] = units
     interval, orig_units, orig_names = io.extract_header_items(header)
     phys_obj = io.generate_blueprint(channels, chtrig, interval, orig_units, orig_names)
     assert math.isclose(phys_obj.freq[0], expected)
 
 
-@pytest.mark.parametrize('units, expected', [
-    ('0.001 s', 1000),
-    ('0.001 min', 16.666666666666668),
-    ('0.001 hr', 0.2777777777777778),
-    ('1 ms', 1000),
-    ('1000 µs', 1000)
-])
+@pytest.mark.parametrize(
+    "units, expected",
+    [
+        ("0.001 s", 1000),
+        ("0.001 min", 16.666666666666668),
+        ("0.001 hr", 0.2777777777777778),
+        ("1 ms", 1000),
+        ("1000 µs", 1000),
+    ],
+)
 def test_generate_blueprint_for_labchart(loaded_lab_file, units, expected):
     header, channels, chtrig = loaded_lab_file
     header[0][1] = units
     interval, orig_units, orig_names = io.extract_header_items(header)
     phys_obj = io.generate_blueprint(channels, chtrig, interval, orig_units, orig_names)
     assert math.isclose(phys_obj.freq[0], expected)
 
@@ -82,99 +90,100 @@
     assert len(phys_obj.timeseries) == len(channels) + 1
 
 
 def test_generate_blueprint_items_errors(loaded_lab_file):
     header, channels, chtrig = loaded_lab_file
     # test file without header
     # test when units are not valid
-    header[0][1] = ' 1 gHz'
+    header[0][1] = " 1 gHz"
     interval, orig_units, orig_names = io.extract_header_items(header)
     with raises(AttributeError) as errorinfo:
         io.generate_blueprint(channels, chtrig, interval, orig_units, orig_names)
     assert 'Interval unit "gHz" is not in a valid frequency' in str(errorinfo.value)
 
 
 def test_extract_header_items_errors(loaded_lab_file):
     header, channels, chtrig = loaded_lab_file
     # test file without header
     with raises(NotImplementedError) as errorinfo:
         io.extract_header_items(header=[])
-    assert 'without header' in str(errorinfo.value)
+    assert "without header" in str(errorinfo.value)
 
     # test Labchart header missing entries
-    header = [['Interval=', '0.001 s'],
-              ['Range=', '2.000 V', '50.0 mmHg', '180.0 mmHg', '10.000 V', '10.000 V']]
+    header = [
+        ["Interval=", "0.001 s"],
+        ["Range=", "2.000 V", "50.0 mmHg", "180.0 mmHg", "10.000 V", "10.000 V"],
+    ]
     with raises(NotImplementedError) as errorinfo:
         io.extract_header_items(header)
-    assert 'supported by phys2bids yet' in str(errorinfo.value)
+    assert "supported by phys2bids yet" in str(errorinfo.value)
 
     # test when header is not valid
     with raises(NotImplementedError) as errorinfo:
-        io.extract_header_items(header=['hello', 'bye'])
-    assert 'supported by phys2bids yet' in str(errorinfo.value)
+        io.extract_header_items(header=["hello", "bye"])
+    assert "supported by phys2bids yet" in str(errorinfo.value)
 
 
 def test_multifreq(loaded_lab_file):
     header, channels, chtrig = loaded_lab_file
     interval, orig_units, orig_names = io.extract_header_items(header)
 
     new_timeseries, new_freq = io.check_multifreq(
-                                            channels,
-                                            [1 / float(interval[0])] * len(channels)
-                                        )
+        channels, [1 / float(interval[0])] * len(channels)
+    )
     assert new_freq[-3:] == [100.0, 40.0, 1000.0]
     # In fairness, last frequency should be 500, but labchart export does not work well.
 
 
 def test_load_acq(samefreq_full_acq_file):
     # Read data to test
     chtrig = 3
     phys_obj = io.load_acq(samefreq_full_acq_file, chtrig)
 
     # checks that the outputs make sense
-    assert phys_obj.ch_name[0] == 'time'
+    assert phys_obj.ch_name[0] == "time"
     assert phys_obj.freq[0] == 10000.0
-    assert phys_obj.units[0] == 's'
+    assert phys_obj.units[0] == "s"
 
     # checks that the trigger is in the right channel
-    assert phys_obj.ch_name[chtrig] == 'MR TRIGGER - Custom, HLT100C - A 5'
+    assert phys_obj.ch_name[chtrig] == "MR TRIGGER - Custom, HLT100C - A 5"
     assert phys_obj.freq[chtrig] == 10000.0
-    assert phys_obj.units[chtrig] == 'Volts'
+    assert phys_obj.units[chtrig] == "Volts"
 
 
 def test_load_mat(matlab_file_labchart, matlab_file_acq):
     # Read data to test labchart in mat extension
     chtrig = 1
     phys_obj = io.load_mat(matlab_file_labchart, chtrig)
 
     # Check channel names are the same.
-    orig_channels = ['time', 'Trigger', 'CO2', 'O2', 'Belt', 'Pulse']
+    orig_channels = ["time", "Trigger", "CO2", "O2", "Belt", "Pulse"]
     assert phys_obj.ch_name == orig_channels
 
     # Check frequencies are the same.
     orig_freq = [1000.0, 1000.0, 100.0, 40.0, 400.0, 1000.0]
     assert phys_obj.freq == orig_freq
 
     # Check units are the same
-    orig_units = ['s', 'V', 'mmHg', 'mmHg', 'V', 'V']
+    orig_units = ["s", "V", "mmHg", "mmHg", "V", "V"]
     assert phys_obj.units == orig_units
 
     # Read data to test acq in mat extension
     chtrig = 3
     phys_obj = io.load_mat(matlab_file_acq, chtrig)
 
     # checks that the outputs make sense
-    assert phys_obj.ch_name[0] == 'time'
+    assert phys_obj.ch_name[0] == "time"
     assert phys_obj.freq[0] == 10000.0
-    assert phys_obj.units[0] == 's'
+    assert phys_obj.units[0] == "s"
 
     # checks that the trigger is in the right channel
-    assert phys_obj.ch_name[chtrig] == 'MR TRIGGER - Custom, HLT100C - A 5'
+    assert phys_obj.ch_name[chtrig] == "MR TRIGGER - Custom, HLT100C - A 5"
     assert phys_obj.freq[chtrig] == 10000.0
-    assert phys_obj.units[chtrig] == 'Volts'
+    assert phys_obj.units[chtrig] == "Volts"
 
 
 # Check single GE file is loaded correctly
 # To read downloaded files in conftest, use the same name of the fixture function
 def test_load_gep_one_file(ge_one_gep_file):
     # Load data
     phys_obj = io.load_gep(ge_one_gep_file)
@@ -187,24 +196,56 @@
 # Check two GE files are loaded correctly, PPG user defined
 def test_load_gep_two_files_ppg(ge_two_gep_files_ppg, testpath):
     # Load data
     phys_obj = io.load_gep(ge_two_gep_files_ppg)
 
     # Check the channel data is as expected
     gep_data1 = np.loadtxt(ge_two_gep_files_ppg)
-    gep_data2 = np.loadtxt(os.path.join(testpath,
-                                        'RESPData_epiRT_0000000000_00_00_000.gep'))
+    gep_data2 = np.loadtxt(os.path.join(testpath, "RESPData_epiRT_0000000000_00_00_000.gep"))
     assert np.array_equal(gep_data1, phys_obj.timeseries[2])
     assert np.array_equal(gep_data2, phys_obj.timeseries[3])
 
 
 # Check two GE files are loaded correctly, RESP user defined
 def test_load_gep_two_files_resp(ge_two_gep_files_resp, testpath):
     # Load data
     phys_obj = io.load_gep(ge_two_gep_files_resp)
 
     # Check the channel data is as expected
     gep_data1 = np.loadtxt(ge_two_gep_files_resp)
-    gep_data2 = np.loadtxt(os.path.join(testpath,
-                                        'PPGData_epiRT_0000000000_00_00_000.gep'))
+    gep_data2 = np.loadtxt(os.path.join(testpath, "PPGData_epiRT_0000000000_00_00_000.gep"))
     assert np.array_equal(gep_data1, phys_obj.timeseries[2])
     assert np.array_equal(gep_data2, phys_obj.timeseries[3])
+
+
+@pytest.mark.skipif(
+    sys.version_info < (3, 7) or sys.version_info > (3, 9),
+    reason="Requires python between 3.7 and 3.9",
+)
+@pytest.mark.xfail(reason="We need to fix sonpy install")
+def test_load_smr(spike2_smr_file, spike2_smrx_file):
+    chtrig = 5
+
+    # 32-bit file
+    phys_obj = io.load_smr(spike2_smr_file, chtrig)
+    assert phys_obj.ch_name[0] == "time"
+    assert phys_obj.freq[0] == 1000.0
+    assert phys_obj.units[0] == "s"
+
+    # checks that the scanner strigger is in the right channel
+    # the marker channels are stored as binary
+    assert phys_obj.ch_name[chtrig] == "Scan Vol"
+    assert phys_obj.freq[chtrig] == 200.0
+    assert phys_obj.units[chtrig] == ""
+    assert len(phys_obj.timeseries[chtrig]) == 60
+
+    # 64-bit file should have the same
+    phys_obj = io.load_smr(spike2_smrx_file, chtrig)
+    assert phys_obj.ch_name[0] == "time"
+    assert phys_obj.freq[0] == 1000.0
+    assert phys_obj.units[0] == "s"
+    # checks that the scanner trigger is in the right channel
+    # the marker channels are stored as binary
+    assert phys_obj.ch_name[chtrig] == "Scan Vol"
+    assert phys_obj.freq[chtrig] == 200.0
+    assert phys_obj.units[chtrig] == ""
+    assert len(phys_obj.timeseries[chtrig]) == 60
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_physio_obj.py` & `phys2bids-2.9.0/phys2bids/tests/test_physio_obj.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test physio_obj.py ."""
 
 import numpy as np
 from pytest import raises
+
 from phys2bids import physio_obj as po
 
 
 # Tests is_valid
 def test_is_valid():
     test_list = [0, 1, 1, 2, 3, 5, 8, 13]
     valid_output = po.is_valid(test_list, list, int)
@@ -17,15 +18,15 @@
 
     test_list = [test_array, test_array]
     valid_output = po.is_valid(test_list, list, np.ndarray)
     assert valid_output == test_list
 
     with raises(AttributeError) as errorinfo:
         valid_output = po.is_valid(test_array, int)
-    assert 'The given variable is not a' in str(errorinfo.value)
+    assert "The given variable is not a" in str(errorinfo.value)
 
 
 # Tests has_size
 def test_has_size():
     # Check padding is correct
     test_list = [0, 1, 1, 2, 3, 5, 8, 13]
     test_length = 10
@@ -39,40 +40,39 @@
     size_output = po.has_size(test_list, test_length, 0)
     assert len(size_output) == test_length
     assert size_output == test_list
 
 
 def test_are_equal():
     """Test are_equal ."""
-    test_string = 'So Long, and Thanks for All the Fish'
+    test_string = "So Long, and Thanks for All the Fish"
     test_time = np.array([0, 1, 1, 2, 3, 5, 8, 13])
     test_trigger = np.array([0, 1, 0, 0, 0, 0, 0, 0])
 
     class C(object):
-        c = 'c'
+        c = "c"
 
     c1 = C()
     c1.ts = [test_time, test_trigger]
 
     c2 = C()
     c2.ts = [test_time]
 
     test_half = np.array([0, 1, 2])
     test_twice = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     test_timeseries = [test_time, test_trigger, test_half, test_twice]
     test_freq = [1, 1, 0.5, 2]
-    test_chn_name = ['time', 'trigger', 'half', 'twice']
-    test_units = ['s', 'V', 'V', 'V']
+    test_chn_name = ["time", "trigger", "half", "twice"]
+    test_units = ["s", "V", "V", "V"]
     test_chtrig = 1
 
-    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                test_units, test_chtrig)
-    phys_out = po.BlueprintInput([test_trigger, test_half, test_twice],
-                                 test_freq, test_chn_name,
-                                 test_units, test_chtrig)
+    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name, test_units, test_chtrig)
+    phys_out = po.BlueprintInput(
+        [test_trigger, test_half, test_twice], test_freq, test_chn_name, test_units, test_chtrig
+    )
 
     assert po.are_equal(test_string, test_string)
     assert po.are_equal(c1, c1)
     assert po.are_equal(phys_in, phys_in)
     assert po.are_equal(c1, c1.__dict__)
     assert po.are_equal(c1.__dict__, c1)
     assert not po.are_equal(c1, c2)
@@ -86,26 +86,27 @@
 # Tests BlueprintInput
 def test_BlueprintInput():
     test_time = np.array([0, 1, 1, 2, 3, 5, 8, 13])
     test_trigger = np.array([0, 1, 0, 0, 0, 0, 0, 0])
     test_chocolate = np.array([1, 0, 0, 1, 0, 0, 1, 0])
     test_timeseries = [test_time, test_trigger, test_chocolate]
     test_freq = [42.0, 3.14, 20.0]
-    test_chn_name = ['time', 'trigger', 'chocolate']
-    test_units = ['s', 's', 'sweetness']
+    test_chn_name = ["time", "trigger", "chocolate"]
+    test_units = ["s", "s", "sweetness"]
     test_chtrig = 1
     num_channnels = len(test_timeseries)
 
-    blueprint_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                     test_units, test_chtrig)
+    blueprint_in = po.BlueprintInput(
+        test_timeseries, test_freq, test_chn_name, test_units, test_chtrig
+    )
 
     # Tests rename_channels
-    new_names = ['trigger', 'time', 'lindt']
+    new_names = ["trigger", "time", "lindt"]
     blueprint_in.rename_channels(new_names)
-    assert blueprint_in.ch_name == ['time', 'trigger', 'lindt']
+    assert blueprint_in.ch_name == ["time", "trigger", "lindt"]
 
     # Tests return_index
     test_index = blueprint_in.return_index(1)
     assert test_index[0] is not test_trigger
     assert (test_index[0] == test_trigger).all()
     assert test_index[1] == len(test_timeseries)
     assert test_index[2] == test_freq[1]
@@ -129,29 +130,30 @@
     assert blueprint_in.trigger_idx == 0
 
     # Test __eq__
     assert blueprint_in == blueprint_in
 
     with raises(IndexError) as errorinfo:
         blueprint_in.__getitem__(1000)
-    assert 'out of bounds' in str(errorinfo.value)
+    assert "out of bounds" in str(errorinfo.value)
 
 
 def test_cta_time_interp():
     """Test BlueprintInput.check_trigger_amount with time resampling."""
     test_time = np.array([0, 7])
     test_trigger = np.array([0, 1, 0, 0, 0, 0, 0, 0])
     test_timeseries = [test_time, test_trigger]
     test_freq = [42.0, 3.14]
-    test_chn_name = ['time', 'trigger']
-    test_units = ['s', 's']
+    test_chn_name = ["time", "trigger"]
+    test_units = ["s", "s"]
     test_chtrig = 1
 
-    blueprint_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                     test_units, test_chtrig)
+    blueprint_in = po.BlueprintInput(
+        test_timeseries, test_freq, test_chn_name, test_units, test_chtrig
+    )
     # Test check_trigger_amount with time resampling
     blueprint_in.check_trigger_amount(thr=0.9, num_timepoints_expected=1)
     assert blueprint_in.num_timepoints_found == 1
     assert blueprint_in.time_offset == 1
     test_offset_time = test_time - 1
     assert np.array_equal(blueprint_in.timeseries[0], test_offset_time)
 
@@ -160,96 +162,103 @@
     """Test BlueprintInput_slice.__getitem__ ."""
     test_time = np.array([0, 1, 2, 3, 4])
     test_trigger = np.array([0, 1, 2, 3, 4])
     test_half = np.array([0, 1, 2])
     test_twice = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     test_timeseries = [test_time, test_trigger, test_half, test_twice]
     test_freq = [1, 1, 0.5, 2]
-    test_chn_name = ['time', 'trigger', 'half', 'twice']
-    test_units = ['s', 'V', 'V', 'V']
+    test_chn_name = ["time", "trigger", "half", "twice"]
+    test_units = ["s", "V", "V", "V"]
     test_chtrig = 1
 
-    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                test_units, test_chtrig)
+    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name, test_units, test_chtrig)
 
-    phys_d = po.BlueprintInput(test_timeseries,
-                               test_freq,
-                               ['time', 'trigger', 'half', 'twice'],
-                               ['s', 'V', 'V', 'V'],
-                               1)
+    phys_d = po.BlueprintInput(
+        test_timeseries, test_freq, ["time", "trigger", "half", "twice"], ["s", "V", "V", "V"], 1
+    )
 
     phys_d.num_timepoints_found = None
     phys_d.thr = None
     phys_d.time_offset = 0
     phys_d._time_resampled_to_trigger = None
 
     # Test all-comprehensive slice
-    assert phys_in[0:len(test_trigger)] == phys_d
+    assert phys_in[0 : len(test_trigger)] == phys_d
 
     # Test instantaneous slice first and last
-    phys_d.timeseries = [np.array([test_time[0]]),
-                         np.array([test_trigger[0]]),
-                         np.array([test_half[0]]),
-                         np.array([test_twice[0]])]
+    phys_d.timeseries = [
+        np.array([test_time[0]]),
+        np.array([test_trigger[0]]),
+        np.array([test_half[0]]),
+        np.array([test_twice[0]]),
+    ]
     assert phys_in[0] == phys_d
 
-    phys_d.timeseries = [np.array([test_time[-1]]),
-                         np.array([test_trigger[-1]]),
-                         np.array([test_half[-1]]),
-                         np.array([test_twice[-2]])]
+    phys_d.timeseries = [
+        np.array([test_time[-1]]),
+        np.array([test_trigger[-1]]),
+        np.array([test_half[-1]]),
+        np.array([test_twice[-2]]),
+    ]
     assert phys_in[-1] == phys_d
 
     # Test slice in the middle
-    phys_d.timeseries = [np.array(test_time[2:4]),
-                         np.array(test_trigger[2:4]),
-                         np.array(test_half[1:2]),
-                         np.array(test_twice[4:8])]
+    phys_d.timeseries = [
+        np.array(test_time[2:4]),
+        np.array(test_trigger[2:4]),
+        np.array(test_half[1:2]),
+        np.array(test_twice[4:8]),
+    ]
     assert phys_in[2:4] == phys_d
 
     # Test slice in the middle with steps
-    phys_d.timeseries = [np.array(test_time[1:4:2]),
-                         np.array(test_trigger[1:4:2]),
-                         np.array(test_half[0:2:1]),
-                         np.array(test_twice[4:8:4])]
+    phys_d.timeseries = [
+        np.array(test_time[1:4:2]),
+        np.array(test_trigger[1:4:2]),
+        np.array(test_half[0:2:1]),
+        np.array(test_twice[4:8:4]),
+    ]
     assert phys_in[1:4:2] == phys_d
 
 
 def test_BlueprintOutput():
     test_time = np.array([0, 1, 1, 2, 3, 5, 8, 13])
     test_trigger = np.array([0, 1, 0, 0, 0, 0, 0, 0])
     test_chocolate = np.array([1, 0, 0, 1, 0, 0, 1, 0])
     test_timeseries = [test_time, test_trigger, test_chocolate]
     test_freq = [42.0, 3.14, 20.0]
-    test_chn_name = ['trigger', 'time', 'chocolate']
-    test_units = ['s', 's', 'sweetness']
+    test_chn_name = ["trigger", "time", "chocolate"]
+    test_units = ["s", "s", "sweetness"]
     test_chtrig = 1
     num_channnels = len(test_timeseries)
 
-    blueprint_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                     test_units, test_chtrig)
+    blueprint_in = po.BlueprintInput(
+        test_timeseries, test_freq, test_chn_name, test_units, test_chtrig
+    )
 
     # Tests init_from_blueprint
     blueprint_out = po.BlueprintOutput.init_from_blueprint(blueprint_in)
     start_time = blueprint_out.start_time
     assert (blueprint_out.timeseries == np.asarray(test_timeseries).T).all()
     assert blueprint_out.freq == test_freq[0]
     assert blueprint_out.ch_name == test_chn_name
     assert blueprint_out.units == test_units
     assert blueprint_out.start_time == 0
 
     # Tests return_index
-    test_timeseries = np.array([[0, 1, 1, 2, 3, 5, 8, 13],
-                                [0, 1, 0, 0, 0, 0, 0, 0],
-                                [1, 0, 0, 1, 0, 0, 1, 0]]).T
+    test_timeseries = np.array(
+        [[0, 1, 1, 2, 3, 5, 8, 13], [0, 1, 0, 0, 0, 0, 0, 0], [1, 0, 0, 1, 0, 0, 1, 0]]
+    ).T
     test_freq = 42.0
-    test_chn_name = ['trigger', 'time', 'chocolate']
-    test_units = ['s', 's', 'sweetness']
+    test_chn_name = ["trigger", "time", "chocolate"]
+    test_units = ["s", "s", "sweetness"]
     num_channnels = test_timeseries.shape[1]
-    blueprint_out = po.BlueprintOutput(test_timeseries, test_freq, test_chn_name, test_units,
-                                       start_time)
+    blueprint_out = po.BlueprintOutput(
+        test_timeseries, test_freq, test_chn_name, test_units, start_time
+    )
     test_index = blueprint_out.return_index(1)
     assert (test_index[0] == test_trigger).all()
     assert test_index[1] == test_timeseries.shape[1]
     assert test_index[3] == test_chn_name[1]
     assert test_index[4] == test_units[1]
 
     # Tests delete_at_index
@@ -267,55 +276,53 @@
     """Test auto_trigger_selection."""
     test_time = np.array([0, 1, 2, 3, 4])
     test_trigger = np.array([0, 1, 2, 3, 4])
     test_half = np.array([0, 1, 2])
     test_twice = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     test_timeseries = [test_time, test_trigger, test_half, test_twice, test_twice, test_twice]
     test_freq = [1, 1, 0.5, 2, 2, 2]
-    test_chn_name = ['time', 'trigger', 'half', 'CO2', 'CO 2', 'strigose']
-    test_units = ['s', 'V', 'V', 'V', 'V', 'V']
+    test_chn_name = ["time", "trigger", "half", "CO2", "CO 2", "strigose"]
+    test_units = ["s", "V", "V", "V", "V", "V"]
 
     # test when trigger is not the name of the channel
     test_chtrig = 2
-    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                test_units, test_chtrig)
-    assert 'Trigger channel name is not' in caplog.text
+    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name, test_units, test_chtrig)
+    assert "Trigger channel name is not" in caplog.text
 
     # test when trigger is 0 and that the trigger channel is recognized by name:
     test_chtrig = 0
-    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                test_units, test_chtrig)
+    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name, test_units, test_chtrig)
     assert phys_in.trigger_idx == 1
     # test when no trigger is found
-    test_chn_name = ['time', 'trigger', 'TRIGGER', 'CO2', 'CO 2', 'strigose']
+    test_chn_name = ["time", "trigger", "TRIGGER", "CO2", "CO 2", "strigose"]
     with raises(Exception) as errorinfo:
-        phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                    test_units, test_chtrig)
-        assert 'More than one possible trigger channel' in str(errorinfo.value)
+        phys_in = po.BlueprintInput(
+            test_timeseries, test_freq, test_chn_name, test_units, test_chtrig
+        )
+        assert "More than one possible trigger channel" in str(errorinfo.value)
 
 
 def test_auto_trigger_selection_time():
     """Test auto_trigger_selection in time domain."""
     # Simulate 10 s of a trigger, O2 and ECG
     T = 10
     nSamp = 100
-    fs = nSamp/T
+    fs = nSamp / T
     test_time = np.linspace(0, T, nSamp)
     test_freq = [fs, fs, fs, fs]
 
     # O2 as a sinusoidal of 0.5 Hz
-    test_O2 = np.sin(2*np.pi*0.5*test_time)
+    test_O2 = np.sin(2 * np.pi * 0.5 * test_time)
     # ECG as a sinusoidal with 1.5 Hz
-    test_ecg = np.sin(2*np.pi*1.5*test_time)
+    test_ecg = np.sin(2 * np.pi * 1.5 * test_time)
     # Trigger as a binary signal
     test_trigger = np.zeros(nSamp)
     test_trigger[1:nSamp:4] = 1
 
     test_timeseries = [test_time, test_O2, test_ecg, test_trigger]
-    test_chn_name = ['time', 'O2', 'ecg', 'tiger']
-    test_units = ['s', 'V', 'V', 'V']
+    test_chn_name = ["time", "O2", "ecg", "tiger"]
+    test_units = ["s", "V", "V", "V"]
 
     # test when chtrig is 0 and the trigger is not recognized by text matching:
     test_chtrig = 0
-    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name,
-                                test_units, test_chtrig)
+    phys_in = po.BlueprintInput(test_timeseries, test_freq, test_chn_name, test_units, test_chtrig)
     assert phys_in.trigger_idx == 3
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/test_phys2bids.py` & `phys2bids-2.9.0/phys2bids/tests/test_phys2bids.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,80 @@
 """
 Tests phys2bids.py
 """
 
 import json
 import os
+
 from pytest import raises
 
 from phys2bids import phys2bids
 
 
 def test_print_summary(tmpdir):
-    test_filename = 'input.txt'
-    test_ntp_expected = [10, ]
+    test_filename = "input.txt"
+    test_ntp_expected = [
+        10,
+    ]
     test_ntp_found = 5
     test_samp_freq = 0.2
     test_time_offset = 0.8
-    test_outfile = tmpdir.join('summary')
-    test_outfile_log = tmpdir.join('summary.log')
+    test_outfile = tmpdir.join("summary")
+    test_outfile_log = tmpdir.join("summary.log")
 
-    phys2bids.print_summary(test_filename, test_ntp_expected, test_ntp_found,
-                            test_samp_freq, test_time_offset, str(test_outfile))
+    phys2bids.print_summary(
+        test_filename,
+        test_ntp_expected,
+        test_ntp_found,
+        test_samp_freq,
+        test_time_offset,
+        str(test_outfile),
+    )
 
     assert os.path.isfile(str(test_outfile_log))
 
 
 def test_print_json(tmpdir):
-    test_outfile = tmpdir.join('json_test')
-    test_outfile_json = tmpdir.join('json_test.json')
+    test_outfile = tmpdir.join("json_test")
+    test_outfile_json = tmpdir.join("json_test.json")
     test_samp_freq = 0.1
     test_time_offset = -0.5
-    test_ch_name = 'foo'
+    test_ch_name = "foo"
 
     phys2bids.print_json(str(test_outfile), test_samp_freq, test_time_offset, test_ch_name)
 
     assert os.path.isfile(test_outfile_json)
 
-    test_json_data = dict(SamplingFrequency=0.1,
-                          StartTime=0.5,
-                          Columns='foo')
-    with open(test_outfile_json, 'r') as src:
+    test_json_data = dict(SamplingFrequency=0.1, StartTime=0.5, Columns="foo")
+    with open(test_outfile_json, "r") as src:
         loaded_data = json.load(src)
 
     assert test_json_data == loaded_data
 
 
 def test_raise_exception(samefreq_full_acq_file):
     test_path, test_filename = os.path.split(samefreq_full_acq_file)
     with raises(Exception) as errorinfo:
         phys2bids.phys2bids(filename=test_filename, indir=test_path, outdir=test_path, chtrig=-1)
-    assert 'Wrong trigger' in str(errorinfo.value)
+    assert "Wrong trigger" in str(errorinfo.value)
 
     with raises(Exception) as errorinfo:
-        phys2bids.phys2bids(filename=test_filename, num_timepoints_expected=[70], tr=[1.3, 2],
-                            indir=test_path, outdir=test_path, chtrig=3)
+        phys2bids.phys2bids(
+            filename=test_filename,
+            num_timepoints_expected=[70],
+            tr=[1.3, 2],
+            indir=test_path,
+            outdir=test_path,
+            chtrig=3,
+        )
     assert "doesn't match" in str(errorinfo.value)
 
     with raises(Exception) as errorinfo:
-        phys2bids.phys2bids(filename=test_filename, num_timepoints_expected=[20, 300], chtrig=3,
-                            tr=1.5, indir=test_path, outdir=test_path)
-    assert 'stop now' in str(errorinfo.value)
+        phys2bids.phys2bids(
+            filename=test_filename,
+            num_timepoints_expected=[20, 300],
+            chtrig=3,
+            tr=1.5,
+            indir=test_path,
+            outdir=test_path,
+        )
+    assert "stop now" in str(errorinfo.value)
```

### Comparing `phys2bids-2.8.4/phys2bids/tests/data/README.md` & `phys2bids-2.9.0/phys2bids/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.4/phys2bids/phys2bids.py` & `phys2bids-2.9.0/phys2bids/phys2bids.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 import os
 import sys
 from copy import deepcopy
 from shutil import copy as cp
 
 import numpy as np
 
-from phys2bids import utils, viz, _version, bids
+from phys2bids import _version, bids, utils, viz
 from phys2bids.cli.run import _get_parser
 from phys2bids.physio_obj import BlueprintOutput
 from phys2bids.slice4phys import slice4phys
 
 from . import __version__
-from .due import due, Doi
+from .due import Doi, due
 
 LGR = logging.getLogger(__name__)
 LGR.setLevel(logging.INFO)
 
 
 def print_summary(filename, ntp_expected, ntp_found, samp_freq, time_offset, outfile):
     """
@@ -71,25 +71,27 @@
     Outcome:
     summary: str
         Prints the summary on screen
     outfile: .log file
         File containing summary
     """
     start_time = -time_offset
-    summary = (f'\n------------------------------------------------\n'
-               f'Filename:            {filename}\n'
-               f'\n'
-               f'Timepoints expected: {ntp_expected}\n'
-               f'Timepoints found:    {ntp_found}\n'
-               f'Sampling Frequency:  {samp_freq} Hz\n'
-               f'Sampling started at: {start_time:.4f} s\n'
-               f'Tip: Time 0 is the time of first trigger\n'
-               f'------------------------------------------------\n')
+    summary = (
+        f"\n------------------------------------------------\n"
+        f"Filename:            {filename}\n"
+        f"\n"
+        f"Timepoints expected: {ntp_expected}\n"
+        f"Timepoints found:    {ntp_found}\n"
+        f"Sampling Frequency:  {samp_freq} Hz\n"
+        f"Sampling started at: {start_time:.4f} s\n"
+        f"Tip: Time 0 is the time of first trigger\n"
+        f"------------------------------------------------\n"
+    )
     LGR.info(summary)
-    utils.write_file(outfile, '.log', summary)
+    utils.write_file(outfile, ".log", summary)
 
 
 def print_json(outfile, samp_freq, time_offset, ch_name):
     """
     Print the json required by BIDS format.
 
     Parameters
@@ -106,34 +108,50 @@
     Notes
     -----
     Outcome:
     outfile: .json file
         File containing information for BIDS.
     """
     start_time = -time_offset
-    summary = dict(SamplingFrequency=samp_freq,
-                   StartTime=round(start_time, 4),
-                   Columns=ch_name)
+    summary = dict(SamplingFrequency=samp_freq, StartTime=round(start_time, 4), Columns=ch_name)
     utils.write_json(outfile, summary, indent=4, sort_keys=False)
 
 
 @due.dcite(
-     Doi('10.5281/zenodo.3470091'),
-     path='phys2bids',
-     description='Conversion of physiological trace data to BIDS format',
-     version=__version__,
-     cite_module=True)
+    Doi("10.5281/zenodo.3470091"),
+    path="phys2bids",
+    description="Conversion of physiological trace data to BIDS format",
+    version=__version__,
+    cite_module=True,
+)
 @due.dcite(
-    Doi('10.1038/sdata.2016.44'),
-    path='phys2bids',
-    description='The BIDS specification',
-    cite_module=True)
-def phys2bids(filename, info=False, indir='.', outdir='.', heur_file=None,
-              sub=None, ses=None, chtrig=0, chsel=None, num_timepoints_expected=None,
-              tr=None, thr=None, pad=9, ch_name=[], yml='', debug=False, quiet=False):
+    Doi("10.1038/sdata.2016.44"),
+    path="phys2bids",
+    description="The BIDS specification",
+    cite_module=True,
+)
+def phys2bids(
+    filename,
+    info=False,
+    indir=".",
+    outdir=".",
+    heur_file=None,
+    sub=None,
+    ses=None,
+    chtrig=0,
+    chsel=None,
+    num_timepoints_expected=None,
+    tr=None,
+    thr=None,
+    pad=9,
+    ch_name=[],
+    yml="",
+    debug=False,
+    quiet=False,
+):
     """
     Run main workflow of phys2bids.
 
     Runs the parser, does some checks on input, then imports
     the right interface file to read the input. If only info is required,
     it returns a summary onscreen.
     Otherwise, it operates on the input to return a .tsv.gz file, possibly
@@ -144,236 +162,277 @@
     RuntimeError[NotImplementedError]
         If invalid input data is provided or if the file extension is not supported yet.
     """
     # Check options to make them internally coherent pt. I
     # #!# This can probably be done while parsing?
     outdir = os.path.abspath(outdir)
     os.makedirs(outdir, exist_ok=True)
-    os.makedirs(os.path.join(outdir, 'code'), exist_ok=True)
-    conversion_path = os.path.join(outdir, 'code', 'conversion')
+    os.makedirs(os.path.join(outdir, "code"), exist_ok=True)
+    conversion_path = os.path.join(outdir, "code", "conversion")
     os.makedirs(conversion_path, exist_ok=True)
 
     # Create logfile name
-    basename = 'phys2bids_'
-    extension = 'tsv'
-    isotime = datetime.datetime.now().strftime('%Y-%m-%dT%H%M%S')
-    logname = os.path.join(conversion_path, (basename + isotime + '.' + extension))
+    basename = "phys2bids_"
+    extension = "tsv"
+    isotime = datetime.datetime.now().strftime("%Y-%m-%dT%H%M%S")
+    logname = os.path.join(conversion_path, (basename + isotime + "." + extension))
 
     # Set logging format
     log_formatter = logging.Formatter(
-        '%(asctime)s\t%(name)-12s\t%(levelname)-8s\t%(message)s',
-        datefmt='%Y-%m-%dT%H:%M:%S')
+        "%(asctime)s\t%(name)-12s\t%(levelname)-8s\t%(message)s", datefmt="%Y-%m-%dT%H:%M:%S"
+    )
 
     # Set up logging file and open it for writing
     log_handler = logging.FileHandler(logname)
     log_handler.setFormatter(log_formatter)
     sh = logging.StreamHandler()
 
     if quiet:
-        logging.basicConfig(level=logging.WARNING,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
+        logging.basicConfig(
+            level=logging.WARNING,
+            handlers=[log_handler, sh],
+            format="%(levelname)-10s %(message)s",
+        )
     elif debug:
-        logging.basicConfig(level=logging.DEBUG,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
+        logging.basicConfig(
+            level=logging.DEBUG, handlers=[log_handler, sh], format="%(levelname)-10s %(message)s"
+        )
     else:
-        logging.basicConfig(level=logging.INFO,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
-
-    version_number = _version.get_versions()['version']
-    LGR.info(f'Currently running phys2bids version {version_number}')
-    LGR.info(f'Input file is {filename}')
+        logging.basicConfig(
+            level=logging.INFO, handlers=[log_handler, sh], format="%(levelname)-10s %(message)s"
+        )
+
+    version_number = _version.get_versions()["version"]
+    LGR.info(f"Currently running phys2bids version {version_number}")
+    LGR.info(f"Input file is {filename}")
 
     # Save call.sh
-    arg_str = ' '.join(sys.argv[1:])
-    call_str = f'phys2bids {arg_str}'
-    f = open(os.path.join(conversion_path, 'call.sh'), "a")
-    f.write(f'#!bin/bash \n{call_str}')
+    arg_str = " ".join(sys.argv[1:])
+    call_str = f"phys2bids {arg_str}"
+    f = open(os.path.join(conversion_path, "call.sh"), "a")
+    f.write(f"#!bin/bash \n{call_str}")
     f.close()
 
     # Check options to make them internally coherent pt. II
     # #!# This can probably be done while parsing?
     indir = os.path.abspath(indir)
     if chtrig and chtrig < 0:
-        raise RuntimeError('Wrong trigger channel. Channel indexing starts with 0!')
+        raise RuntimeError("Wrong trigger channel. Channel indexing starts with 0!")
 
     utils.check_ge(filename, indir)
-    filename, ftype = utils.check_input_type(filename,
-                                             indir)
+    filename, ftype = utils.check_input_type(filename, indir)
 
     if heur_file:
-        heur_file = utils.check_input_ext(heur_file, '.py')
+        heur_file = utils.check_input_ext(heur_file, ".py")
         utils.check_file_exists(heur_file)
 
     infile = os.path.join(indir, filename)
     utils.check_file_exists(infile)
 
     if isinstance(num_timepoints_expected, int):
         num_timepoints_expected = [num_timepoints_expected]
     if isinstance(tr, (int, float)):
         tr = [tr]
 
     if tr is not None and num_timepoints_expected is not None:
         # If tr and ntp were specified, check that tr is either length one or ntp.
         if len(num_timepoints_expected) != len(tr) and len(tr) != 1:
-            raise RuntimeError('Number of sequence types listed with TR '
-                               'doesn\'t match expected number of runs in '
-                               'the session')
+            raise RuntimeError(
+                "Number of sequence types listed with TR "
+                "doesn't match expected number of runs in "
+                "the session"
+            )
 
     # Read file!
-    LGR.info(f'Reading the file {infile}')
-    if ftype == 'acq':
+    LGR.info(f"Reading the file {infile}")
+    if ftype == "acq":
         from phys2bids.io import load_acq
+
         phys_in = load_acq(infile, chtrig)
-    elif ftype == 'txt':
+    elif ftype == "txt":
         from phys2bids.io import load_txt
+
         phys_in = load_txt(infile, chtrig)
-    elif ftype == 'mat':
+    elif ftype == "mat":
         from phys2bids.io import load_mat
+
         phys_in = load_mat(infile, chtrig)
-    elif ftype == 'gep':
+    elif ftype == "gep":
         from phys2bids.io import load_gep
+
         phys_in = load_gep(infile)
 
-    LGR.info('Checking that units of measure are BIDS compatible')
+    LGR.info("Checking that units of measure are BIDS compatible")
     for index, unit in enumerate(phys_in.units):
         phys_in.units[index] = bids.bidsify_units(unit)
 
-    LGR.info('Reading infos')
+    LGR.info("Reading infos")
     phys_in.print_info(filename)
     # #!# Here the function viz.plot_channel should be called
-    viz.plot_all(phys_in.ch_name, phys_in.timeseries, phys_in.units,
-                 phys_in.freq, infile, conversion_path)
+    viz.plot_all(
+        phys_in.ch_name, phys_in.timeseries, phys_in.units, phys_in.freq, infile, conversion_path
+    )
     # If only info were asked, end here.
     if info:
         return
 
     # The next few lines remove the undesired channels from phys_in.
     if chsel:
-        LGR.info('Dropping unselected channels')
+        LGR.info("Dropping unselected channels")
         chsel.insert(0, 0)
         if phys_in.trigger_idx not in chsel:
-            LGR.warning(f'The selected channels {tuple(chsel)} do not '
-                        f'contain the trigger channel ({phys_in.trigger_idx}). '
-                        f'Adding channel {phys_in.trigger_idx} to the selection.')
+            LGR.warning(
+                f"The selected channels {tuple(chsel)} do not "
+                f"contain the trigger channel ({phys_in.trigger_idx}). "
+                f"Adding channel {phys_in.trigger_idx} to the selection."
+            )
             chsel.extend(phys_in.trigger_idx)
         chsel.sort()
-        for i in range(phys_in.ch_amount-1, 0, -1):
+        for i in range(phys_in.ch_amount - 1, 0, -1):
             if i not in chsel:
                 phys_in.delete_at_index(i)
         # Update trigger index
         phys_in.trigger_idx = chsel.index(phys_in.trigger_idx)
 
     # If requested, change channel names.
     if ch_name:
-        LGR.info('Renaming channels with given names')
+        LGR.info("Renaming channels with given names")
         phys_in.rename_channels(ch_name)
 
     # Checking acquisition type via user's input
     if tr is not None and num_timepoints_expected is not None:
-
         #  Multi-run acquisition type section
         #  Check list length, more than 1 means multi-run
         if len(num_timepoints_expected) > 1:
             # if multi-run of same sequence type, pad list with ones
             # and multiply array with user's input
             if len(tr) == 1:
                 tr = np.ones(len(num_timepoints_expected)) * tr[0]
 
             # Sum of values in ntp_list should be equivalent to num_timepoints_found
-            phys_in.check_trigger_amount(thr=thr,
-                                         num_timepoints_expected=sum(num_timepoints_expected),
-                                         tr=1)
+            phys_in.check_trigger_amount(
+                thr=thr, num_timepoints_expected=sum(num_timepoints_expected), tr=1
+            )
 
             # Check that sum of tp expected is equivalent to num_timepoints_found,
             # if it passes call slice4phys
             if phys_in.num_timepoints_found != sum(num_timepoints_expected):
-                raise RuntimeError('The number of triggers found is different '
-                                   'than expected. Better stop now than break '
-                                   'something.')
+                raise RuntimeError(
+                    "The number of triggers found is different "
+                    "than expected. Better stop now than break "
+                    "something."
+                )
 
             # slice the recording based on user's entries
             # !!! ATTENTION: PHYS_IN GETS OVERWRITTEN AS DICTIONARY
-            phys_in = slice4phys(phys_in, num_timepoints_expected, tr,
-                                 phys_in.thr, pad)
+            phys_in = slice4phys(phys_in, num_timepoints_expected, tr, phys_in.thr, pad)
             # returns a dictionary in the form {take_idx: phys_in[startpoint, endpoint]}
 
             # save a figure for each take | give the right acquisition parameters for takes
-            fileprefix = os.path.join(conversion_path,
-                                      os.path.splitext(os.path.basename(filename))[0])
+            fileprefix = os.path.join(
+                conversion_path, os.path.splitext(os.path.basename(filename))[0]
+            )
             for i, take in enumerate(phys_in.keys()):
-                plot_fileprefix = f'{fileprefix}_{take:02d}'
-                viz.export_trigger_plot(phys_in[take], phys_in[take].trigger_idx,
-                                        plot_fileprefix, tr[i],
-                                        num_timepoints_expected[i], filename,
-                                        sub, ses)
+                plot_fileprefix = f"{fileprefix}_{take:02d}"
+                viz.export_trigger_plot(
+                    phys_in[take],
+                    phys_in[take].trigger_idx,
+                    plot_fileprefix,
+                    tr[i],
+                    num_timepoints_expected[i],
+                    filename,
+                    sub,
+                    ses,
+                )
 
         # Single take acquisition type, or : nothing to split workflow
         else:
             # Run analysis on trigger channel to get first timepoint
             # and the time offset.
             phys_in.check_trigger_amount(thr, num_timepoints_expected[0], tr[0])
             # save a figure of the trigger
-            fileprefix = os.path.join(conversion_path,
-                                      os.path.splitext(os.path.basename(filename))[0])
-            viz.export_trigger_plot(phys_in, phys_in.trigger_idx, fileprefix, tr[0],
-                                    num_timepoints_expected[0], filename,
-                                    sub, ses)
+            fileprefix = os.path.join(
+                conversion_path, os.path.splitext(os.path.basename(filename))[0]
+            )
+            viz.export_trigger_plot(
+                phys_in,
+                phys_in.trigger_idx,
+                fileprefix,
+                tr[0],
+                num_timepoints_expected[0],
+                filename,
+                sub,
+                ses,
+            )
 
             # Reassign phys_in as dictionary
             # !!! ATTENTION: PHYS_IN GETS OVERWRITTEN AS DICTIONARY
             phys_in = {1: phys_in}
 
     else:
-        LGR.warning('Skipping trigger pulse count. If you want to run it, '
-                    'call phys2bids using both "-ntp" and "-tr" arguments')
+        LGR.warning(
+            "Skipping trigger pulse count. If you want to run it, "
+            'call phys2bids using both "-ntp" and "-tr" arguments'
+        )
         # !!! ATTENTION: PHYS_IN GETS OVERWRITTEN AS DICTIONARY
         phys_in = {1: phys_in}
 
     # The next few lines create a dictionary of different BlueprintInput
     # objects, one for each unique frequency for each take in phys_in
     # they also save the amount of runs and unique frequencies
     take_amount = len(phys_in)
     uniq_freq_list = set(phys_in[1].freq)
     freq_amount = len(uniq_freq_list)
     if freq_amount > 1:
-        LGR.info(f'Found {freq_amount} different frequencies in input!')
+        LGR.info(f"Found {freq_amount} different frequencies in input!")
 
     if take_amount > 1:
-        LGR.info(f'Found {take_amount} different takes in input!')
+        LGR.info(f"Found {take_amount} different takes in input!")
 
-    LGR.info(f'Preparing {freq_amount*take_amount} output files.')
+    LGR.info(f"Preparing {freq_amount*take_amount} output files.")
     # Create phys_out dict that will have a blueprint object for each different frequency
     phys_out = {}
 
     if heur_file is not None and sub is not None:
-        LGR.info(f'Preparing BIDS output using {heur_file}')
+        LGR.info(f"Preparing BIDS output using {heur_file}")
         # If heuristics are used, init a dict of arguments to pass to use_heuristic
-        heur_args = {'heur_file': heur_file, 'sub': sub, 'ses': ses,
-                     'filename': filename, 'outdir': outdir, 'take': '',
-                     'record_label': ''}
+        heur_args = {
+            "heur_file": heur_file,
+            "sub": sub,
+            "ses": ses,
+            "filename": filename,
+            "outdir": outdir,
+            "take": "",
+            "record_label": "",
+        }
         # Generate participants.tsv file if it doesn't exist already.
         # Update the file if the subject is not in the file.
         # Do not update if the subject is already in the file.
         bids.participants_file(outdir, yml, sub)
         # Generate dataset_description.json file if it doesn't exist already.
         bids.dataset_description_file(outdir)
         # Generate README file if it doesn't exist already.
         bids.readme_file(outdir)
-        cp(heur_file, os.path.join(conversion_path,
-           os.path.splitext(os.path.basename(heur_file))[0] + '.py'))
+        cp(
+            heur_file,
+            os.path.join(
+                conversion_path, os.path.splitext(os.path.basename(heur_file))[0] + ".py"
+            ),
+        )
     elif heur_file is not None and sub is None:
-        LGR.warning('While "-heur" was specified, option "-sub" was not.\n'
-                    'Skipping BIDS formatting.')
+        LGR.warning(
+            'While "-heur" was specified, option "-sub" was not.\n' "Skipping BIDS formatting."
+        )
 
     # Export a (set of) phys_out for each element in phys_in
     # run keys start from 1 (human friendly)
     for take in phys_in.keys():
         for uniq_freq in uniq_freq_list:
             # Initialise the key for the (possibly huge amount of) dictionary entries
-            key = f'{take}_{uniq_freq}'
+            key = f"{take}_{uniq_freq}"
             # copy the phys_in object to the new dict entry
             phys_out[key] = deepcopy(phys_in[take])
             # this counter will take into account how many channels are eliminated
             count = 0
             # for each channel in the original phys_in object
             # take the frequency
             for idx, i in enumerate(phys_in[take].freq):
@@ -388,88 +447,108 @@
             # Also create a BlueprintOutput object for each unique frequency found.
             # Populate it with the corresponding blueprint input and replace it
             # in the dictionary.
             # Add time channel in the proper frequency.
             if uniq_freq != phys_in[take].freq[0]:
                 phys_out[key].ch_name.insert(0, phys_in[take].ch_name[0])
                 phys_out[key].units.insert(0, phys_in[take].units[0])
-                phys_out[key].timeseries.insert(0, np.linspace(phys_in[take].timeseries[0][0],
-                                                phys_in[take].timeseries[0][-1],
-                                                num=phys_out[key].timeseries[0].shape[0]))
+                phys_out[key].timeseries.insert(
+                    0,
+                    np.linspace(
+                        phys_in[take].timeseries[0][0],
+                        phys_in[take].timeseries[0][-1],
+                        num=phys_out[key].timeseries[0].shape[0],
+                    ),
+                )
             # Add trigger channel in the proper frequency.
             if uniq_freq != phys_in[take].freq[phys_in[take].trigger_idx]:
                 phys_out[key].ch_name.insert(1, phys_in[take].ch_name[phys_in[take].trigger_idx])
                 phys_out[key].units.insert(1, phys_in[take].units[phys_in[take].trigger_idx])
                 phys_out[key].timeseries.insert(
                     1,
                     np.interp(
                         phys_out[key].timeseries[0],
                         phys_in[take].timeseries[0],
-                        phys_in[take].timeseries[phys_in[take].trigger_idx]
-                    )
+                        phys_in[take].timeseries[phys_in[take].trigger_idx],
+                    ),
                 )
             phys_out[key] = BlueprintOutput.init_from_blueprint(phys_out[key])
 
         # Preparing output parameters: name and folder.
         for uniq_freq in uniq_freq_list:
-            key = f'{take}_{uniq_freq}'
+            key = f"{take}_{uniq_freq}"
             # If possible, prepare bids renaming.
             if heur_file is not None and sub is not None:
                 # Add take info to heur_args if more than one take is present
                 if take_amount > 1:
-                    heur_args['take'] = f'{take:02d}'
+                    heur_args["take"] = f"{take:02d}"
 
                 # Append "recording-freq" to filename if more than one freq
                 if freq_amount > 1:
-                    heur_args['record_label'] = f'{uniq_freq:.0f}Hz'
+                    heur_args["record_label"] = f"{uniq_freq:.0f}Hz"
 
                 phys_out[key].filename = bids.use_heuristic(**heur_args)
 
                 # If any filename exists already because of multi-take, append labels
                 # But warn about the non-validity of this BIDS-like name.
                 if take_amount > 1:
                     for n, k in enumerate(phys_out.keys()):
                         if k != key and phys_out[key].filename == phys_out[k].filename:
-                            phys_out[key].filename = (f'{phys_out[key].filename}'
-                                                      f'_take-{take:02d}')
-                            LGR.warning('Identified multiple outputs with the same name.\n'
-                                        'Appending fake label to avoid overwriting.\n'
-                                        '!!! ATTENTION !!! the output is not BIDS compliant.\n'
-                                        'Please check heuristics to solve the problem.')
+                            phys_out[key].filename = (
+                                f"{phys_out[key].filename}" f"_take-{take:02d}"
+                            )
+                            LGR.warning(
+                                "Identified multiple outputs with the same name.\n"
+                                "Appending fake label to avoid overwriting.\n"
+                                "!!! ATTENTION !!! the output is not BIDS compliant.\n"
+                                "Please check heuristics to solve the problem."
+                            )
 
             else:
-                phys_out[key].filename = os.path.join(outdir,
-                                                      os.path.splitext(os.path.basename(filename)
-                                                                       )[0])
+                phys_out[key].filename = os.path.join(
+                    outdir, os.path.splitext(os.path.basename(filename))[0]
+                )
                 # Append "take" to filename if more than one take
                 if take_amount > 1:
-                    phys_out[key].filename = f'{phys_out[key].filename}_{take:02d}'
+                    phys_out[key].filename = f"{phys_out[key].filename}_{take:02d}"
                 # Append "freq" to filename if more than one freq
                 if freq_amount > 1:
-                    phys_out[key].filename = f'{phys_out[key].filename}_{uniq_freq:.0f}Hz'
+                    phys_out[key].filename = f"{phys_out[key].filename}_{uniq_freq:.0f}Hz"
 
-            LGR.info(f'Exporting files for take {take} freq {uniq_freq}')
-            np.savetxt(phys_out[key].filename + '.tsv.gz',
-                       phys_out[key].timeseries, fmt='%.8e', delimiter='\t')
-            print_json(phys_out[key].filename, phys_out[key].freq,
-                       phys_out[key].start_time, phys_out[key].ch_name)
-            print_summary(filename, num_timepoints_expected,
-                          phys_in[take].num_timepoints_found, uniq_freq,
-                          phys_out[key].start_time,
-                          os.path.join(conversion_path,
-                                       os.path.splitext(os.path.basename(phys_out[key].filename)
-                                                        )[0]))
+            LGR.info(f"Exporting files for take {take} freq {uniq_freq}")
+            np.savetxt(
+                phys_out[key].filename + ".tsv.gz",
+                phys_out[key].timeseries,
+                fmt="%.8e",
+                delimiter="\t",
+            )
+            print_json(
+                phys_out[key].filename,
+                phys_out[key].freq,
+                phys_out[key].start_time,
+                phys_out[key].ch_name,
+            )
+            print_summary(
+                filename,
+                num_timepoints_expected,
+                phys_in[take].num_timepoints_found,
+                uniq_freq,
+                phys_out[key].start_time,
+                os.path.join(
+                    conversion_path, os.path.splitext(os.path.basename(phys_out[key].filename))[0]
+                ),
+            )
 
 
 def _main(argv=None):
     options = _get_parser().parse_args(argv)
     phys2bids(**vars(options))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _main(sys.argv[1:])
 
 """
 Copyright 2019, The Phys2BIDS community.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `phys2bids-2.8.4/phys2bids/due.py` & `phys2bids-2.9.0/phys2bids/due.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,55 +13,60 @@
 License:    BSD-2
 
 # emacs: at the end of the file
 # ex: set sts=4 ts=4 sw=4 et:
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### #
 """
 
-from builtins import str
-from builtins import object
-__version__ = '0.0.5'
+from builtins import object, str
+
+__version__ = "0.0.5"
 
 
 class InactiveDueCreditCollector(object):
     """Just a stub at the Collector which would not do anything."""
 
     def _donothing(self, *args, **kwargs):
         """Perform no good and no bad."""
         pass
 
     def dcite(self, *args, **kwargs):
         """If I could cite I would."""
+
         def nondecorating_decorator(func):
             return func
+
         return nondecorating_decorator
 
     cite = load = add = _donothing
 
     def __repr__(self):
         """Return class function."""
-        return self.__class__.__name__ + '()'
+        return self.__class__.__name__ + "()"
 
 
 def _donothing_func(*args, **kwargs):
     """Perform no good and no bad."""
     pass
 
 
 try:
-    from duecredit import due, BibTeX, Doi, Url
-    if 'due' in locals() and not hasattr(due, 'cite'):
-        raise RuntimeError(
-            "Imported due lacks .cite. DueCredit is now disabled")
+    from duecredit import BibTeX, Doi, Url, due
+
+    if "due" in locals() and not hasattr(due, "cite"):
+        raise RuntimeError("Imported due lacks .cite. DueCredit is now disabled")
 except Exception as e:
-    if type(e).__name__ != 'ImportError':
+    if type(e).__name__ != "ImportError":
         import logging
+
         logging.getLogger("duecredit").error(
             'Module `duecredit` not successfully imported due to "%s". '
-            'Package functionality unaffected.', str(e))
+            "Package functionality unaffected.",
+            str(e),
+        )
 
     # Initiate due stub
     due = InactiveDueCreditCollector()
     BibTeX = Doi = Url = _donothing_func
 
 # Emacs mode definitions
 # Local Variables:
```

### Comparing `phys2bids-2.8.4/phys2bids/physio_obj.py` & `phys2bids-2.9.0/phys2bids/physio_obj.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     Raises
     ------
     AttributeError
         If var is not of var_type
     """
     if not isinstance(var, var_type):
-        raise AttributeError(f'The given variable is not a {var_type}')
+        raise AttributeError(f"The given variable is not a {var_type}")
 
     if var_type is list and list_type is not None:
         for element in var:
             _ = is_valid(element, list_type)
 
     return var
 
@@ -103,33 +103,34 @@
     -------
     boolean
     """
 
     def _deal_with_dict_value_error(self, other):
         # Check if "self" has a 'timeseries' key. If not, return False.
         try:
-            self['timeseries']
+            self["timeseries"]
         except KeyError:
             return False
         except TypeError:
             return False
         else:
             # Check that the two objects have the same keys.
             # If not, return False, otherwise loop through the timeseries key.
             if self.keys() == other.keys():
-                alltrue_timeseries = [False] * len(self['timeseries'])
+                alltrue_timeseries = [False] * len(self["timeseries"])
                 alltrue_keys = [False] * len(self)
                 for j, key in enumerate(self.keys()):
-                    if key == 'timeseries':
-                        for i in range(len(self['timeseries'])):
-                            alltrue_timeseries[i] = (self['timeseries'][i].all()
-                                                     == other['timeseries'][i].all())
+                    if key == "timeseries":
+                        for i in range(len(self["timeseries"])):
+                            alltrue_timeseries[i] = (
+                                self["timeseries"][i].all() == other["timeseries"][i].all()
+                            )
                         alltrue_keys[j] = all(alltrue_timeseries)
                     else:
-                        alltrue_keys[j] = (self[key] == other[key])
+                        alltrue_keys[j] = self[key] == other[key]
                 return all(alltrue_keys)
             else:
                 return False
 
     try:
         # Try to compare the dictionary format of the two objects
         return self.__dict__ == other.__dict__
@@ -154,15 +155,15 @@
                 # Try to compare self with the two object.
                 try:
                     return self == other
                 except ValueError:
                     return _deal_with_dict_value_error(self, other)
 
 
-class BlueprintInput():
+class BlueprintInput:
     """
     Main input object for phys2bids.
 
     Contains the blueprint to be populated.
     !!! Pay attention: there's rules on how to populate this object.
     See below ("Attention") !!!
 
@@ -226,31 +227,41 @@
     As a consequence:
     - freq[0] == freq[chtrig]
     - ch_name[0] = 'time'
     - units[0] = 's'
     - Actual number of channels +1 <= ch_amount
     """
 
-    def __init__(self, timeseries, freq, ch_name, units, trigger_idx,
-                 num_timepoints_found=None, thr=None, time_offset=0):
+    def __init__(
+        self,
+        timeseries,
+        freq,
+        ch_name,
+        units,
+        trigger_idx,
+        num_timepoints_found=None,
+        thr=None,
+        time_offset=0,
+    ):
         """Initialise BlueprintInput (see class docstring)."""
         self.timeseries = deepcopy(is_valid(timeseries, list, list_type=np.ndarray))
-        self.freq = deepcopy(has_size(is_valid(freq, list,
-                                      list_type=(int, float)),
-                             self.ch_amount, 0.0))
-        self.ch_name = deepcopy(has_size(ch_name, self.ch_amount, 'unknown'))
-        self.units = deepcopy(has_size(units, self.ch_amount, '[]'))
-
+        self.freq = deepcopy(
+            has_size(is_valid(freq, list, list_type=(int, float)), self.ch_amount, 0.0)
+        )
+        self.ch_name = deepcopy(has_size(ch_name, self.ch_amount, "unknown"))
+        self.units = deepcopy(has_size(units, self.ch_amount, "[]"))
         self.trigger_idx = deepcopy(is_valid(trigger_idx, int))
         if trigger_idx == 0:
             self.auto_trigger_selection()
         else:
             if ch_name[trigger_idx] not in TRIGGER_NAMES:
-                LGR.info('Trigger channel name is not in our trigger channel name alias list. '
-                         'Please make sure you choose the proper channel.')
+                LGR.info(
+                    "Trigger channel name is not in our trigger channel name alias list. "
+                    "Please make sure you choose the proper channel."
+                )
 
         self.num_timepoints_found = deepcopy(num_timepoints_found)
         self.thr = deepcopy(thr)
         self.time_offset = deepcopy(time_offset)
         self._time_resampled_to_trigger = None
 
     @property
@@ -316,41 +327,49 @@
         if idx.start is None:
             idx = slice(0, idx.stop)
         if idx.stop is None:
             idx = slice(idx.start, trigger_length)
 
         # Check that the indexes are not out of bounds
         if idx.start >= trigger_length or idx.stop > trigger_length:
-            raise IndexError(f'Slice ({idx.start}, {idx.stop}) is out of '
-                             f'bounds for channel {self.trigger_idx} '
-                             f'with size {trigger_length}')
+            raise IndexError(
+                f"Slice ({idx.start}, {idx.stop}) is out of "
+                f"bounds for channel {self.trigger_idx} "
+                f"with size {trigger_length}"
+            )
 
         # Operate on each channel on its own
         for n, channel in enumerate(self.timeseries):
-            idx_dict = {'start': idx.start, 'stop': idx.stop, 'step': idx.step}
+            idx_dict = {"start": idx.start, "stop": idx.stop, "step": idx.step}
             # Adapt the slicing indexes to the right frequency
-            for i in ['start', 'stop', 'step']:
+            for i in ["start", "stop", "step"]:
                 if idx_dict[i]:
-                    idx_dict[i] = int(np.floor(self.freq[n]
-                                               / self.freq[self.trigger_idx]
-                                               * idx_dict[i]))
+                    idx_dict[i] = int(
+                        np.floor(self.freq[n] / self.freq[self.trigger_idx] * idx_dict[i])
+                    )
 
             # Correct the slicing stop if necessary
-            if idx_dict['start'] == idx_dict['stop'] or return_instant:
-                idx_dict['stop'] = idx_dict['start'] + 1
+            if idx_dict["start"] == idx_dict["stop"] or return_instant:
+                idx_dict["stop"] = idx_dict["start"] + 1
             elif trigger_length == idx.stop:
-                idx_dict['stop'] = len(channel)
+                idx_dict["stop"] = len(channel)
 
-            new_idx = slice(idx_dict['start'], idx_dict['stop'], idx_dict['step'])
+            new_idx = slice(idx_dict["start"], idx_dict["stop"], idx_dict["step"])
             sliced_timeseries[n] = channel[new_idx]
 
-        sliced_bp = BlueprintInput(sliced_timeseries, self.freq, self.ch_name,
-                                   self.units, self.trigger_idx,
-                                   self.num_timepoints_found, self.thr,
-                                   self.time_offset)
+        sliced_bp = BlueprintInput(
+            sliced_timeseries,
+            self.freq,
+            self.ch_name,
+            self.units,
+            self.trigger_idx,
+            self.num_timepoints_found,
+            self.thr,
+            self.time_offset,
+        )
 
         sliced_bp._time_resampled_to_trigger = self._time_resampled_to_trigger
         return sliced_bp
 
     def __eq__(self, other):
         """
         Return test of equality between two objects.
@@ -379,21 +398,24 @@
 
         Notes
         -----
         Outcome:
         self.ch_name: list of str
             Changes content to new_name.
         """
-        if 'time' in new_names:
-            del new_names[new_names.index('time')]
-
-        new_names = ['time', ] + new_names
+        if "time" in new_names:
+            del new_names[new_names.index("time")]
 
-        self.ch_name = has_size(is_valid(new_names, list, list_type=str),
-                                self.ch_amount, 'unknown')
+        new_names = [
+            "time",
+        ] + new_names
+
+        self.ch_name = has_size(
+            is_valid(new_names, list, list_type=str), self.ch_amount, "unknown"
+        )
 
     def return_index(self, idx):
         """
         Return the list entries of all the object properties, given an index.
 
         Parameters
         ----------
@@ -402,16 +424,21 @@
 
         Returns
         -------
         out: tuple
             Tuple containing the proper list entry of all the
             properties of the object with index `idx`
         """
-        return (self.timeseries[idx], self.ch_amount, self.freq[idx],
-                self.ch_name[idx], self.units[idx])
+        return (
+            self.timeseries[idx],
+            self.ch_amount,
+            self.freq[idx],
+            self.ch_name[idx],
+            self.units[idx],
+        )
 
     def delete_at_index(self, idx):
         """
         Delete the list entries of the object properties, given their index.
 
         Parameters
         ----------
@@ -434,16 +461,15 @@
         """
         del self.timeseries[idx]
         del self.freq[idx]
         del self.ch_name[idx]
         del self.units[idx]
 
         if self.trigger_idx == idx:
-            LGR.warning('Removing trigger channel - are you sure you are doing'
-                        'the right thing?')
+            LGR.warning("Removing trigger channel - are you sure you are doing" "the right thing?")
             self.trigger_idx = 0
 
     def check_trigger_amount(self, thr=None, num_timepoints_expected=0, tr=0):
         """
         Count trigger points and correct time offset in channel "time".
 
         Parameters
@@ -466,80 +492,88 @@
             Property of the `BlueprintInput` class.
             Contains the number of timepoints found
             with the automatic estimation.
         self.timeseries:
             The property `timeseries` is shifted with the 0 being
             the time of first trigger.
         """
-        LGR.info('Counting trigger points')
+        LGR.info("Counting trigger points")
         # Use the trigger channel to find the TRs,
         # comparing it to a given threshold.
         trigger = self.timeseries[self.trigger_idx]
         time = self.timeseries[0]
-        LGR.info(f'The trigger is in channel {self.trigger_idx}')
+        LGR.info(f"The trigger is in channel {self.trigger_idx}")
         # Check that trigger and time channels have the same length.
         # If not, resample time to the length of the trigger
         if len(time) != len(trigger):
-            LGR.warning('The trigger channel has a different sampling '
-                        'from the registered time. Using a resampled version '
-                        'of time to find the starting time.')
+            LGR.warning(
+                "The trigger channel has a different sampling "
+                "from the registered time. Using a resampled version "
+                "of time to find the starting time."
+            )
             time = np.linspace(time[0], time[-1], len(trigger))
 
             self._time_resampled_to_trigger = time
 
         flag = 0
         if thr is None:
             # If trigger channels are binary
             # (i.e., "on" is a higher value and "off" is a lower value)
             # and each "on" and "off" are each always approzimately the same value
             # then any value above the mean is "on" and every value below the mean
             # is "off".
             thr = np.mean(trigger)
             flag = 1
         timepoints = trigger > thr
-        num_timepoints_found = len([is_true for is_true, _ in groupby(timepoints,
-                                    lambda x: x != 0) if is_true])
+        num_timepoints_found = len(
+            [is_true for is_true, _ in groupby(timepoints, lambda x: x != 0) if is_true]
+        )
         if flag == 1:
-            LGR.info(f'The number of timepoints according to the std_thr method '
-                     f'is {num_timepoints_found}. The computed threshold is {thr:.4f}')
+            LGR.info(
+                f"The number of timepoints according to the std_thr method "
+                f"is {num_timepoints_found}. The computed threshold is {thr:.4f}"
+            )
         else:
-            LGR.info(f'The number of timepoints found with the manual threshold of {thr:.4f} '
-                     f'is {num_timepoints_found}')
+            LGR.info(
+                f"The number of timepoints found with the manual threshold of {thr:.4f} "
+                f"is {num_timepoints_found}"
+            )
         time_offset = time[timepoints.argmax()]
 
         if num_timepoints_expected:
-            LGR.info('Checking number of timepoints')
+            LGR.info("Checking number of timepoints")
             if num_timepoints_found > num_timepoints_expected:
-                timepoints_extra = (num_timepoints_found
-                                    - num_timepoints_expected)
-                LGR.warning(f'Found {timepoints_extra} timepoints'
-                            ' more than expected!\n'
-                            'Assuming extra timepoints are at the end '
-                            '(try again with a more liberal thr)')
+                timepoints_extra = num_timepoints_found - num_timepoints_expected
+                LGR.warning(
+                    f"Found {timepoints_extra} timepoints"
+                    " more than expected!\n"
+                    "Assuming extra timepoints are at the end "
+                    "(try again with a more liberal thr)"
+                )
 
             elif num_timepoints_found < num_timepoints_expected:
-                timepoints_missing = (num_timepoints_expected
-                                      - num_timepoints_found)
-                LGR.warning(f'Found {timepoints_missing} timepoints'
-                            ' less than expected!')
+                timepoints_missing = num_timepoints_expected - num_timepoints_found
+                LGR.warning(f"Found {timepoints_missing} timepoints" " less than expected!")
                 if tr:
-                    LGR.warning('Correcting time offset, assuming missing '
-                                'timepoints are at the beginning (try again '
-                                'with a more conservative thr)')
-                    time_offset -= (timepoints_missing * tr)
+                    LGR.warning(
+                        "Correcting time offset, assuming missing "
+                        "timepoints are at the beginning (try again "
+                        "with a more conservative thr)"
+                    )
+                    time_offset -= timepoints_missing * tr
                 else:
-                    LGR.warning('Can\'t correct time offset - you should '
-                                'specify the TR')
+                    LGR.warning("Can't correct time offset - you should " "specify the TR")
 
             else:
-                LGR.info('Found just the right amount of timepoints!')
+                LGR.info("Found just the right amount of timepoints!")
 
         else:
-            LGR.warning('The necessary options to find the amount of timepoints '
-                        'were not provided.')
+            LGR.warning(
+                "The necessary options to find the amount of timepoints " "were not provided."
+            )
         self.thr = thr
         self.time_offset = time_offset
         self.timeseries[0] = self.timeseries[0] - time_offset
         self.num_timepoints_found = num_timepoints_found
 
     def print_info(self, filename):
         """
@@ -553,20 +587,20 @@
         Notes
         -----
         Outcome:
         ch:
             Returns to stdout (e.g. on screen) channels,
             their names and their sampling rate.
         """
-        info = (f'\n------------------------------------------------'
-                f'\nFile {filename} contains:\n')
+        info = (
+            f"\n------------------------------------------------" f"\nFile {filename} contains:\n"
+        )
         for ch in range(1, self.ch_amount):
-            info = info + (f'{ch:02d}. {self.ch_name[ch]};'
-                           f' sampled at {self.freq[ch]} Hz\n')
-        info = info + '------------------------------------------------\n'
+            info = info + (f"{ch:02d}. {self.ch_name[ch]};" f" sampled at {self.freq[ch]} Hz\n")
+        info = info + "------------------------------------------------\n"
 
         LGR.info(info)
 
     def auto_trigger_selection(self):
         """
         Find a trigger index automatically.
 
@@ -585,34 +619,36 @@
 
         Notes
         -----
         Outcome:
             trigger_idx : int
                 Automatically retrieved trigger index
         """
-        LGR.info('Running automatic trigger detection.')
-        LGR.info('Matching channel names with known trigger names first.')
-        joint_match = '§'.join(TRIGGER_NAMES)
+        LGR.info("Running automatic trigger detection.")
+        LGR.info("Matching channel names with known trigger names first.")
+        joint_match = "§".join(TRIGGER_NAMES)
         indexes = []
         for n, case in enumerate(self.ch_name):
-            name = re.split(r'(\W+|\d|_|\s)', case)
+            name = re.split(r"(\W+|\d|_|\s)", case)
             name = list(filter(None, name))
 
-            if re.search('|'.join(name), joint_match, re.IGNORECASE):
+            if re.search("|".join(name), joint_match, re.IGNORECASE):
                 indexes = indexes + [n]
 
         if indexes:
             if len(indexes) > 1:
-                raise Exception('More than one possible trigger channel was automatically found. '
-                                'Please run phys2bids specifying the -chtrig argument.')
+                raise Exception(
+                    "More than one possible trigger channel was automatically found. "
+                    "Please run phys2bids specifying the -chtrig argument."
+                )
             else:
                 self.trigger_idx = int(indexes[0])
         else:
             # Time-domain automatic trigger detection
-            LGR.info('Find the trigger channel by measuring data distance from its value limits.')
+            LGR.info("Find the trigger channel by measuring data distance from its value limits.")
             # Create numpy array with all channels (excluding time)
             channel_ts = np.array(self.timeseries[1:])
 
             # Normalize each signal to [0,1]
             min_ts = np.min(channel_ts, axis=1)[:, None]
             max_ts = np.max(channel_ts, axis=1)[:, None]
             channel_ts = (channel_ts - min_ts) / (max_ts - min_ts)
@@ -620,18 +656,18 @@
             # Compute distance to the closest signal limit (0 or 1)
             distance = np.minimum(abs(channel_ts - 0), abs(channel_ts - 1))
             distance_mean = np.mean(distance, axis=1)
 
             # Set the trigger as the channel with the smallest distance
             self.trigger_idx = int(np.nanargmin(distance_mean) + 1)
 
-        LGR.info(f'{self.ch_name[self.trigger_idx]} selected as trigger channel')
+        LGR.info(f"{self.ch_name[self.trigger_idx]} selected as trigger channel")
 
 
-class BlueprintOutput():
+class BlueprintOutput:
     """
     Main output object for phys2bids.
 
     Contains the blueprint to be exported.
 
     Attributes
     ----------
@@ -664,20 +700,20 @@
     delete_at_index:
         Returns all the proper list entry of the
         properties of the object, given an index.
     init_from_blueprint:
         method to populate from input blueprint instead of init
     """
 
-    def __init__(self, timeseries, freq, ch_name, units, start_time, filename=''):
+    def __init__(self, timeseries, freq, ch_name, units, start_time, filename=""):
         """Initialise BlueprintOutput (see class docstring)."""
         self.timeseries = deepcopy(is_valid(timeseries, np.ndarray))
         self.freq = deepcopy(is_valid(freq, (int, float)))
-        self.ch_name = deepcopy(has_size(ch_name, self.ch_amount, 'unknown'))
-        self.units = deepcopy(has_size(units, self.ch_amount, '[]'))
+        self.ch_name = deepcopy(has_size(ch_name, self.ch_amount, "unknown"))
+        self.units = deepcopy(has_size(units, self.ch_amount, "[]"))
         self.start_time = deepcopy(start_time)
         self.filename = deepcopy(is_valid(filename, str))
 
     @property
     def ch_amount(self):
         """
         Property. Returns number of channels (ch).
@@ -715,16 +751,22 @@
 
         Returns
         -------
         out: tuple
             Tuple containing the proper list entry of all the
             properties of the object with index `idx`
         """
-        return (self.timeseries[:, idx], self.ch_amount, self.freq,
-                self.ch_name[idx], self.units[idx], self.start_time)
+        return (
+            self.timeseries[:, idx],
+            self.ch_amount,
+            self.freq,
+            self.ch_name[idx],
+            self.units[idx],
+            self.start_time,
+        )
 
     def delete_at_index(self, idx):
         """
         Delete the list entries of the object properties, given their index.
 
         Parameters
         ----------
```

### Comparing `phys2bids-2.8.4/phys2bids/io.py` & `phys2bids-2.9.0/phys2bids/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 import numpy as np
 
 from phys2bids.physio_obj import BlueprintInput
 
 LGR = logging.getLogger(__name__)
 OPEN_ISSUE = (
-    'The file you are trying to convert might not be supported by phys2bids yet. '
-    'Please open an issue on GitHub '
-    '(https://github.com/physiopy/phys2bids/issues/new/choose) '
-    'so that we can improve file support!'
+    "The file you are trying to convert might not be supported by phys2bids yet. "
+    "Please open an issue on GitHub "
+    "(https://github.com/physiopy/phys2bids/issues/new/choose) "
+    "so that we can improve file support!"
 )
 
 
 def check_multifreq(timeseries, freq, start=0, endat=None):
     """
     Check if there are channels with different frequency than the maximum one.
 
@@ -39,15 +39,15 @@
     Returns
     -------
     multifreq_timeseries : list of numpy.ndarrays
         new list with the channels in their own frequency
     multifreq_freq : list of floats
         new list with the real frequency of the channels
     """
-    LGR.info('Checking if frequencies are different across channels')
+    LGR.info("Checking if frequencies are different across channels")
     multifreq_freq = deepcopy(freq)
     multifreq_timeseries = deepcopy(timeseries)
 
     # Skip time
     for n, ch in enumerate(timeseries[1:]):
         n = n + 1
         # Find lengths of repetitions
@@ -98,69 +98,88 @@
         https://www.adinstruments.com/support/knowledge-base/how-can-channel-titles-ranges-intervals-etc-text-file-be-imported-labchart
         https://www.biopac.com/wp-content/uploads/acqknowledge_software_guide.pdf page 194
 
     See Also
     --------
     physio_obj.BlueprintInput
     """
-    if interval[-1] not in ['min', 'sec', 'µsec', 'msec', 'MHz', 'kHz', 'Hz', 'hr', 'min', 's',
-                            'ms', 'µs']:
-        raise AttributeError(f'Interval unit "{interval[-1]}" is not in a '
-                             'valid frequency or time unit format, this probably '
-                             'means your file is not in min, sec, msec, µsec, hr, min, s, ms, µs, '
-                             'Mhz, KHz or Hz')
+    if interval[-1] not in [
+        "min",
+        "sec",
+        "µsec",
+        "msec",
+        "MHz",
+        "kHz",
+        "Hz",
+        "hr",
+        "min",
+        "s",
+        "ms",
+        "µs",
+    ]:
+        raise AttributeError(
+            f'Interval unit "{interval[-1]}" is not in a '
+            "valid frequency or time unit format, this probably "
+            "means your file is not in min, sec, msec, µsec, hr, min, s, ms, µs, "
+            "Mhz, KHz or Hz"
+        )
     # Check if the header is in frequency or sampling interval
-    if 'Hz' in interval[-1]:
-        LGR.info('Retrieving frequency from file header, calculating sample interval, '
-                 'and standardizing to Hz if needed')
+    if "Hz" in interval[-1]:
+        LGR.info(
+            "Retrieving frequency from file header, calculating sample interval, "
+            "and standardizing to Hz if needed"
+        )
         freq = float(interval[0])
         freq_unit = interval[-1]
-        if freq_unit == 'MHz':
+        if freq_unit == "MHz":
             freq = freq * (1000000)
-        elif freq_unit == 'kHz':
+        elif freq_unit == "kHz":
             freq = freq * 1000
         interval[0] = 1 / freq
         freq = [freq] * len(timeseries)
     else:
         # check if interval is in seconds, if not change the units to seconds and
         # calculate frequency
-        if interval[-1] not in ('s', 'sec'):
-            LGR.warning('Sampling interval not expressed in seconds. '
-                        'Converting its value and unit.')
-            if interval[-1] == 'min':
+        if interval[-1] not in ("s", "sec"):
+            LGR.warning(
+                "Sampling interval not expressed in seconds. " "Converting its value and unit."
+            )
+            if interval[-1] == "min":
                 interval[0] = float(interval[0]) * 60
-            elif interval[-1] == 'msec':
+            elif interval[-1] == "msec":
                 interval[0] = float(interval[0]) / 1000
-            elif interval[-1] == 'µsec':
+            elif interval[-1] == "µsec":
                 interval[0] = float(interval[0]) / 1000000
-            elif interval[-1] == 'hr':
+            elif interval[-1] == "hr":
                 interval[0] = float(interval[0]) * 3600
-            elif interval[-1] == 'ms':
+            elif interval[-1] == "ms":
                 interval[0] = float(interval[0]) / 1000
-            elif interval[-1] == 'µs':
+            elif interval[-1] == "µs":
                 interval[0] = float(interval[0]) / 1000000
-            interval[-1] = 's'
+            interval[-1] = "s"
         else:
             interval[0] = float(interval[0])
         # get frequency
         freq = [1 / interval[0]] * len(timeseries)
     # reorder channels names
-    names = ['time', ]
+    names = ["time"]
     names = names + orig_names
     # reorder channels units
-    units = ['s', ]
+    units = ["s"]
     units = units + orig_units
     # Check if the file has a time channel, otherwise create it.
     # As the "time" doesn't have a column header, if the number of header names
     # is less than the number of timeseries, then "time" is column 0...
     # ...otherwise, create the time channel
     if not (len(orig_names) < len(timeseries)):
         duration = (timeseries[0].shape[0] + 1) * interval[0]
-        t_ch = np.ogrid[0:duration:interval[0]][:-1]  # create time channel
-        timeseries = [t_ch, ] + timeseries
+        t_ch = np.ogrid[0 : duration : interval[0]][:-1]  # create time channel
+        timeseries = [
+            t_ch,
+        ] + timeseries
         freq = [max(freq)] + freq
     timeseries, freq = check_multifreq(timeseries, freq)
     return BlueprintInput(timeseries, freq, names, units, chtrig)
 
 
 def read_header_and_channels(filename):
     """
@@ -177,34 +196,34 @@
         header lines
     channel_list : list of strings
         The channels of the recording
 
     """
     header = []
     # Read in the header until it's numbers
-    with open(filename, 'r') as f:
+    with open(filename, "r") as f:
         for n, line in enumerate(f):
-            line = line.rstrip('\n').split('\t')
-            if line[-1] == '':
-                line.remove('')
+            line = line.rstrip("\n").split("\t")
+            if line[-1] == "":
+                line.remove("")
             try:
                 float(line[0])
                 break
             except ValueError:
                 header.append(line)
                 continue
     # Read in the rest paying attention to possible differences
-    if 'Interval=' in header[0]:
+    if "Interval=" in header[0]:
         # Not specifying delimiters will ignore comments
         channel_list = np.genfromtxt(filename, skip_header=n)
-    elif 'acq' in header[0][0]:
+    elif "acq" in header[0][0]:
         # Specifying delimiters will avoid missing values in the files
-        channel_list = np.genfromtxt(filename, skip_header=n, delimiter='\t')
+        channel_list = np.genfromtxt(filename, skip_header=n, delimiter="\t")
         # Remove extra (empty?) columns, if present
-        ch_number = int(header[2][0].split(' ')[0])
+        ch_number = int(header[2][0].split(" ")[0])
         channel_list = channel_list[:, :ch_number]
         # Set all remaining NaNs to 0
         channel_list = np.nan_to_num(channel_list)
         # Take first row and assign it back to header.
         header.append(list(channel_list[0, :].astype(int)))
         channel_list = channel_list[1:, :]
 
@@ -240,40 +259,40 @@
     NotImplementedError
         If len(header) == 0 and therefore there is no header
         If Labchart headers cannot be processed
         If files are not in acq or txt format
     """
     # check header is not empty and detect if it is in labchart or Acqknoledge format
     if len(header) == 0:
-        raise NotImplementedError('Files without header are not supported yet')
-    elif 'Interval=' in header[0]:
-        LGR.info('phys2bids detected that your file is in Labchart format')
+        raise NotImplementedError("Files without header are not supported yet")
+    elif "Interval=" in header[0]:
+        LGR.info("phys2bids detected that your file is in Labchart format")
 
         interval = None
         orig_names = None
         range_list = None
         for line in header:
-            if 'Interval=' in line:
+            if "Interval=" in line:
                 interval = line[1].split(" ")
-            if 'ChannelTitle=' in line:
+            if "ChannelTitle=" in line:
                 orig_names = line[1:]
-            if 'Range=' in line:
+            if "Range=" in line:
                 range_list = line[1:]
 
         if None in [interval, orig_names, range_list]:
             raise NotImplementedError(OPEN_ISSUE)
 
         orig_units = []
         for item in range_list:
-            orig_units.append(item.split(' ')[1])
+            orig_units.append(item.split(" ")[1])
 
-    elif 'acq' in header[0][0]:
-        LGR.info('phys2bids detected that your file is in AcqKnowledge format')
+    elif "acq" in header[0][0]:
+        LGR.info("phys2bids detected that your file is in AcqKnowledge format")
         interval = header[1][0].split()
-        interval[-1] = interval[-1].split('/')[0]
+        interval[-1] = interval[-1].split("/")[0]
         # get units and names
         orig_units = []
         orig_names = []
         # the for loop starts at index1 at 3 because that's the first line of the header
         # with channel name info and ends in 2 + twice the number of channels because
         # that should be the last channel name
         for index1 in range(3, 3 + len(header[-1]) * 2, 2):
@@ -333,25 +352,26 @@
     to time is added at the beginning - that is already taken into account!
 
     See Also
     --------
     physio_obj.BlueprintInput
     """
     from bioread import read_file
+
     with warnings.catch_warnings():
-        warnings.filterwarnings('ignore', category=DeprecationWarning)
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
         data = read_file(filename).channels
 
-    freq = [data[0].samples_per_second, ]
-    timeseries = [data[0].time_index, ]
-    units = ['s', ]
-    names = ['time', ]
+    freq = [data[0].samples_per_second]
+    timeseries = [data[0].time_index]
+    units = ["s"]
+    names = ["time"]
 
     for k, ch in enumerate(data):
-        LGR.info(f'{k:02d}. {ch}')
+        LGR.info(f"{k:02d}. {ch}")
         timeseries.append(ch.data)
         freq.append(ch.samples_per_second)
         units.append(ch.units)
         names.append(ch.name)
 
     return BlueprintInput(timeseries, freq, names, units, chtrig)
 
@@ -380,48 +400,57 @@
 
     See Also
     --------
     physio_obj.BlueprintInput
     """
     # Load MATLAB file into dictionary.
     from pymatreader import read_mat
+
     mat_dict = read_mat(filename)
-    if '__header__' in mat_dict:
-        orig_names = list(mat_dict['labels'])
-        orig_units = list(mat_dict['units'])
-        interval = [mat_dict['isi'], mat_dict['isi_units']]
-        channel_list = mat_dict['data']
+    if "__header__" in mat_dict:
+        orig_names = list(mat_dict["labels"])
+        orig_units = list(mat_dict["units"])
+        interval = [mat_dict["isi"], mat_dict["isi_units"]]
+        channel_list = mat_dict["data"]
         channel_list = [ch for ch in channel_list.T]
         return generate_blueprint(channel_list, chtrig, interval, orig_units, orig_names)
     else:
         # Convert data into 1d numpy array for easier indexing.
-        data = np.squeeze(np.asarray(mat_dict['data']))
+        data = np.squeeze(np.asarray(mat_dict["data"]))
 
         # Extract number of channels and tick rate.
-        n_channels = len(mat_dict['titles'])
-        t_freq = mat_dict['tickrate']
+        n_channels = len(mat_dict["titles"])
+        t_freq = mat_dict["tickrate"]
 
         # Stores MATLAB data into lists.
         timeseries = []
-        freq = [t_freq, ]
-        units = ['s', ]
-        names = ['time', ]
+        freq = [
+            t_freq,
+        ]
+        units = [
+            "s",
+        ]
+        names = [
+            "time",
+        ]
 
         for ch in range(n_channels):
-            units.append(mat_dict['unittext'][int(mat_dict['unittextmap'][ch] - 1)].strip())
-            names.append(mat_dict['titles'][ch].strip())
-            freq.append(mat_dict['samplerate'][ch])
-            idx_start = int(mat_dict['datastart'][ch])
-            idx_end = int(mat_dict['dataend'][ch])
+            units.append(mat_dict["unittext"][int(mat_dict["unittextmap"][ch] - 1)].strip())
+            names.append(mat_dict["titles"][ch].strip())
+            freq.append(mat_dict["samplerate"][ch])
+            idx_start = int(mat_dict["datastart"][ch])
+            idx_end = int(mat_dict["dataend"][ch])
             timeseries.append(data[idx_start:idx_end])
         # Calculate duration based on frequency and create time channel.
         interval = 1 / t_freq
         duration = (timeseries[0].shape[0] + 1) * interval
         t_ch = np.ogrid[0:duration:interval][:-1]
-        timeseries = [t_ch, ] + timeseries
+        timeseries = [
+            t_ch,
+        ] + timeseries
         return BlueprintInput(timeseries, freq, names, units, chtrig)
 
 
 def load_gep(filename):
     """
     Populate object phys_input from GE physiological files.
 
@@ -457,56 +486,140 @@
     physio_obj.BlueprintInput
     """
     import os
     from glob import glob
     from pathlib import Path
 
     # Initiate lists of column names and units with time and trigger
-    names = ['time', 'trigger']
-    units = ['s', 'mV']  # Assuming recording units are mV...
+    names = ["time", "trigger"]
+    units = ["s", "mV"]  # Assuming recording units are mV...
 
     # Add column for file given by user
-    if 'PPGData' in filename:
+    if "PPGData" in filename:
         freq = [100, 100, 100]
-        names.append('cardiac')
-    elif 'RESPData' in filename:
+        names.append("cardiac")
+    elif "RESPData" in filename:
         freq = [25, 25, 25]
-        names.append('respiratory')
-    elif 'ECGData' in filename:
+        names.append("respiratory")
+    elif "ECGData" in filename:
         freq = [1000, 1000, 1000]
-        names.append('cardiac')
+        names.append("cardiac")
 
     # Load in user file data
     data = [np.loadtxt(filename)]
 
     # Calculate time in seconds for first input (starts from -30s)
     interval = 1 / freq[0]
     duration = data[0].shape[0] * interval
-    t_ch = np.ogrid[-30:duration - 30:interval]
+    t_ch = np.ogrid[-30 : duration - 30 : interval]
 
     # Find and add additional data files
     filename = Path(filename)
-    fnames = glob(os.path.join(filename.parent, f'*{filename.name[-24:-4]}.gep'))
+    fnames = glob(os.path.join(filename.parent, f"*{filename.name[-24:-4]}.gep"))
     fnames.remove(str(filename))  # Drop the original file
     if not len(fnames) == 0:
         for fname in fnames:
-            if 'PPGData' in fname:
+            if "PPGData" in fname:
                 freq.append(100)
-                names.append('cardiac')
+                names.append("cardiac")
                 data.append(np.loadtxt(fname))
-            elif 'RESPData' in fname:
+            elif "RESPData" in fname:
                 freq.append(25)
-                names.append('respiratory')
+                names.append("respiratory")
                 data.append(np.loadtxt(fname))
-            elif 'ECGData' in fname:
+            elif "ECGData" in fname:
                 freq.append(1000)
-                names.append('cardiac')
+                names.append("cardiac")
                 data.append(np.loadtxt(fname))
 
     # Create trigger channel
-    trigger = np.hstack((np.zeros(int(30 / interval)),
-                         np.ones(int((duration - 30) / interval))))
+    trigger = np.hstack((np.zeros(int(30 / interval)), np.ones(int((duration - 30) / interval))))
 
     # Create final list of timeseries
     timeseries = [t_ch, trigger]
     timeseries.extend(data)
     return BlueprintInput(timeseries, freq, names, units, 1)
+
+
+def load_smr(filename, chtrig=0):
+    """Load Spike2 smr file and populate object phys_input.
+
+    Parameters
+    ----------
+    filename: str
+        Path to the spike smr or smrx file.
+
+    chtrig : int
+        Index of trigger channel.
+
+    Returns
+    -------
+    BlueprintInput
+
+    Note
+    ----
+    Index of chtrig is 1-index (i.e. spike2 channel number).
+
+    See Also
+    --------
+    physio_obj.BlueprintInput
+    """
+    import sonpy
+
+    # taken from sonpy demo
+    read_data = {
+        sonpy.lib.DataType.Adc: sonpy.lib.SonFile.ReadInts,
+        sonpy.lib.DataType.EventFall: sonpy.lib.SonFile.ReadEvents,
+        sonpy.lib.DataType.EventRise: sonpy.lib.SonFile.ReadEvents,
+        sonpy.lib.DataType.EventBoth: sonpy.lib.SonFile.ReadEvents,
+        sonpy.lib.DataType.Marker: sonpy.lib.SonFile.ReadMarkers,
+        sonpy.lib.DataType.AdcMark: sonpy.lib.SonFile.ReadWaveMarks,
+        sonpy.lib.DataType.RealMark: sonpy.lib.SonFile.ReadRealMarks,
+        sonpy.lib.DataType.TextMark: sonpy.lib.SonFile.ReadTextMarks,
+        sonpy.lib.DataType.RealWave: sonpy.lib.SonFile.ReadFloats,
+    }
+
+    smrfile = sonpy.lib.SonFile(filename, True)
+    time_base = smrfile.GetTimeBase()
+    n_channels = smrfile.MaxChannels()
+    freq, names, units, timeseries = [], [], [], []
+    for i in range(n_channels):
+        current_channel = smrfile.ChannelType(i)
+        max_n_tick = smrfile.ChannelMaxTime(i)
+        if current_channel != sonpy.lib.DataType.Off and max_n_tick > 0:
+            max_n_tick = smrfile.ChannelMaxTime(i)
+            sample_rate = smrfile.GetIdealRate(i)
+            if current_channel == sonpy.lib.DataType.Adc:
+                divide = smrfile.ChannelDivide(i)
+            else:  # marker channels
+                divide = 1 / (time_base * sample_rate)
+            # conversion factor from CED spike2 doc
+            # http://ced.co.uk/img/Spike9.pdf
+            gain = smrfile.GetChannelScale(i) / 6553.6
+            offset = smrfile.GetChannelOffset(i)
+            name = smrfile.GetChannelTitle(chan=i)
+            unit = smrfile.GetChannelUnits(chan=i)
+
+            n_samples = int(np.floor((max_n_tick) / divide))
+            raw_signal = read_data[current_channel](
+                smrfile, chan=i, nMax=n_samples, tFrom=0, tUpto=max_n_tick
+            )
+
+            signal = np.array(raw_signal) * gain + offset
+
+            # save the data
+            freq.append(sample_rate)
+            names.append(name)
+            units.append(unit)
+            timeseries.append(signal)
+
+    # use the channel with highest sample rate to create time stamps
+    idx_max = np.argmax(freq)
+    n_timepoints = len(timeseries[idx_max])  # end point included
+    time = np.arange(n_timepoints) * freq[idx_max]
+
+    # prepend to the existing list
+    freq = [freq[idx_max]] + freq
+    timeseries = [time] + timeseries
+    units = ["s"] + units
+    names = ["time"] + names
+    return BlueprintInput(timeseries, freq, names, units, chtrig)
```

### Comparing `phys2bids-2.8.4/phys2bids/heuristics/heur_tutorial.py` & `phys2bids-2.9.0/phys2bids/heuristics/heur_test_multifreq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import fnmatch
 
 
-def heur(physinfo, take=''):
+def heur(physinfo, take=""):
     """
     Set of if .. elif statements to fill BIDS names.
 
     It requires the user (you!) to adjust it accordingly!
     It needs an ``if`` or ``elif`` statement for each file that
     needs to be processed.
     The statement will test if the ``physinfo``:
@@ -52,20 +52,20 @@
     # ##    -info['dir']             ## #
     # ##                             ## #
     # ##  Remember that they are     ## #
     # ##  dictionary keys            ## #
     # ##  See example below          ## #
     # ################################# #
 
-    if fnmatch.fnmatchcase(physinfo, '*tutorial*'):
-        info['task'] = 'test'
-        info['run'] = '01'
-        info['rec'] = 'labchart'
-    elif physinfo == 'Example':
-        info['task'] = 'rest'
-        info['run'] = '01'
-        info['acq'] = 'resp'
+    if fnmatch.fnmatchcase(physinfo, "*onescan*"):
+        info["task"] = "test"
+        info["run"] = "01"
+        info["rec"] = "biopac"
+    elif physinfo == "Example":
+        info["task"] = "rest"
+        info["run"] = "01"
+        info["acq"] = "resp"
 
     # ############################## #
     # ## Don't modify below this! ## #
     # ############################## #
     return info
```

### Comparing `phys2bids-2.8.4/phys2bids/heuristics/heur_euskalibur.py` & `phys2bids-2.9.0/phys2bids/heuristics/heur_euskalibur.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import fnmatch
 
 
-def heur(physinfo, take=''):
+def heur(physinfo, take=""):
     """
     Set of if .. elif statements to fill BIDS names.
 
     It requires the user (you!) to adjust it accordingly!
     It needs an ``if`` or ``elif`` statement for each file that
     needs to be processed.
     The statement will test if the ``physinfo``:
@@ -52,37 +52,37 @@
     # ##    -info['dir']             ## #
     # ##                             ## #
     # ##  Remember that they are     ## #
     # ##  dictionary keys            ## #
     # ##  See example below          ## #
     # ################################# #
 
-    if physinfo == 'origfilename1':
-        info['task'] = 'newname1'
-    elif physinfo == 'origfilename2':
-        info['task'] = 'newname2'
-        info['run'] = 'runnum'
-    elif physinfo == 'BH4':
-        info['task'] = 'breathhold'
-    elif fnmatch.fnmatchcase(physinfo, 'MOTOR?'):
-        info['task'] = 'motor'
-    elif fnmatch.fnmatchcase(physinfo, 'LOCALIZER?'):
-        info['task'] = 'pinel'
-    elif fnmatch.fnmatchcase(physinfo, 'SIMON?'):
-        info['task'] = 'simon'
-    elif physinfo == 'RS1':
-        info['task'] = 'rest'
-        info['run'] = '01'
-    elif physinfo == 'RS2':
-        info['task'] = 'rest'
-        info['run'] = '02'
-    elif physinfo == 'RS3':
-        info['task'] = 'rest'
-        info['run'] = '03'
-    elif physinfo == 'RS4':
-        info['task'] = 'rest'
-        info['run'] = '04'
+    if physinfo == "origfilename1":
+        info["task"] = "newname1"
+    elif physinfo == "origfilename2":
+        info["task"] = "newname2"
+        info["run"] = "runnum"
+    elif physinfo == "BH4":
+        info["task"] = "breathhold"
+    elif fnmatch.fnmatchcase(physinfo, "MOTOR?"):
+        info["task"] = "motor"
+    elif fnmatch.fnmatchcase(physinfo, "LOCALIZER?"):
+        info["task"] = "pinel"
+    elif fnmatch.fnmatchcase(physinfo, "SIMON?"):
+        info["task"] = "simon"
+    elif physinfo == "RS1":
+        info["task"] = "rest"
+        info["run"] = "01"
+    elif physinfo == "RS2":
+        info["task"] = "rest"
+        info["run"] = "02"
+    elif physinfo == "RS3":
+        info["task"] = "rest"
+        info["run"] = "03"
+    elif physinfo == "RS4":
+        info["task"] = "rest"
+        info["run"] = "04"
 
     # ############################## #
     # ## Don't modify below this! ## #
     # ############################## #
     return info
```

### Comparing `phys2bids-2.8.4/phys2bids/heuristics/heur_test_multifreq.py` & `phys2bids-2.9.0/phys2bids/heuristics/heur_tutorial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import fnmatch
 
 
-def heur(physinfo, take=''):
+def heur(physinfo, take=""):
     """
     Set of if .. elif statements to fill BIDS names.
 
     It requires the user (you!) to adjust it accordingly!
     It needs an ``if`` or ``elif`` statement for each file that
     needs to be processed.
     The statement will test if the ``physinfo``:
@@ -52,20 +52,20 @@
     # ##    -info['dir']             ## #
     # ##                             ## #
     # ##  Remember that they are     ## #
     # ##  dictionary keys            ## #
     # ##  See example below          ## #
     # ################################# #
 
-    if fnmatch.fnmatchcase(physinfo, '*onescan*'):
-        info['task'] = 'test'
-        info['run'] = '01'
-        info['rec'] = 'biopac'
-    elif physinfo == 'Example':
-        info['task'] = 'rest'
-        info['run'] = '01'
-        info['acq'] = 'resp'
+    if fnmatch.fnmatchcase(physinfo, "*tutorial*"):
+        info["task"] = "test"
+        info["run"] = "01"
+        info["rec"] = "labchart"
+    elif physinfo == "Example":
+        info["task"] = "rest"
+        info["run"] = "01"
+        info["acq"] = "resp"
 
     # ############################## #
     # ## Don't modify below this! ## #
     # ############################## #
     return info
```

### Comparing `phys2bids-2.8.4/phys2bids/heuristics/heur_test_acq.py` & `phys2bids-2.9.0/phys2bids/heuristics/heur_test_acq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import fnmatch
 
 
-def heur(physinfo, take=''):
+def heur(physinfo, take=""):
     """
     Set of if .. elif statements to fill BIDS names.
 
     It requires the user (you!) to adjust it accordingly!
     It needs an ``if`` or ``elif`` statement for each file that
     needs to be processed.
     The statement will test if the ``physinfo``:
@@ -52,20 +52,20 @@
     # ##    -info['dir']             ## #
     # ##                             ## #
     # ##  Remember that they are     ## #
     # ##  dictionary keys            ## #
     # ##  See example below          ## #
     # ################################# #
 
-    if fnmatch.fnmatchcase(physinfo, '*samefreq*'):
-        info['task'] = 'test'
-        info['run'] = '01'
-        info['rec'] = 'biopac'
-    elif physinfo == 'Example':
-        info['task'] = 'rest'
-        info['run'] = '01'
-        info['acq'] = 'resp'
+    if fnmatch.fnmatchcase(physinfo, "*samefreq*"):
+        info["task"] = "test"
+        info["run"] = "01"
+        info["rec"] = "biopac"
+    elif physinfo == "Example":
+        info["task"] = "rest"
+        info["run"] = "01"
+        info["acq"] = "resp"
 
     # ############################## #
     # ## Don't modify below this! ## #
     # ############################## #
     return info
```

### Comparing `phys2bids-2.8.4/phys2bids/viz.py` & `phys2bids-2.9.0/phys2bids/viz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """Visualization functions for phys2bids package."""
-import os
 import logging
+import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 LGR = logging.getLogger(__name__)
 
 SET_DPI = 100
 FIGSIZE = (18, 10)
 
 
-def plot_trigger(time, trigger, fileprefix, tr, thr, num_timepoints_expected,
-                 filename, figsize=FIGSIZE, dpi=SET_DPI):
+def plot_trigger(
+    time,
+    trigger,
+    fileprefix,
+    tr,
+    thr,
+    num_timepoints_expected,
+    filename,
+    figsize=FIGSIZE,
+    dpi=SET_DPI,
+):
     """
     Produce a figure with three plots.
 
     1. Plots the triggers in blue, a block in orange that indicates
     the time from the first trigger to the last, and a red line showing
     the threshold used for trigger detection
     2. Same plot but showing only the initial trigger
@@ -59,83 +68,94 @@
     """
 
     def time2ntr(x):
         return x / tr
 
     def ntr2time(x):
         return x * tr
+
     # get filename
     outname = os.path.splitext(os.path.basename(filename))[0]
     # create threshold line
     thrline = np.ones(time.shape) * thr
     # define figure and space between plots
     fig = plt.figure(figsize=figsize, dpi=dpi)
     block = time > 0
     d = np.zeros(len(time))
     plt.subplots_adjust(hspace=0.7)
     # plot of the hole trigger
     subplot = fig.add_subplot(211)
-    subplot.set_title(f'Trigger and time for {outname}.tsv.gz')
+    subplot.set_title(f"Trigger and time for {outname}.tsv.gz")
     subplot.set_ylim([-0.2, thr * 3])
-    subplot.set_xlabel('Seconds')
-    subplot.set_ylabel('Volts')
-    subplot.plot(time, trigger, '-', time, thrline, 'r-.', time, block, '-')
-    subplot.fill_between(time, block, where=block >= d, interpolate=True, color='#ffbb6e')
-    subplot.legend(['trigger', 'Trigger detection threshold', 'time block'], loc='upper right')
+    subplot.set_xlabel("Seconds")
+    subplot.set_ylabel("Volts")
+    subplot.plot(time, trigger, "-", time, thrline, "r-.", time, block, "-")
+    subplot.fill_between(time, block, where=block >= d, interpolate=True, color="#ffbb6e")
+    subplot.legend(["trigger", "Trigger detection threshold", "time block"], loc="upper right")
     # plot the first spike according to the user threshold
     subplot = fig.add_subplot(223)
     subplot.set_xlim([-tr * 4, tr * 4])
     subplot.set_ylim([-0.2, thr * 3])
-    subplot.set_xlabel('Seconds')
-    subplot.set_ylabel('Volts')
+    subplot.set_xlabel("Seconds")
+    subplot.set_ylabel("Volts")
     ax2 = subplot.twiny()
-    ax2.set_xticklabels('')
+    ax2.set_xticklabels("")
     ax2.tick_params(
-                    axis='x',          # changes apply to the x-axis
-                    which='both',      # both major and minor ticks are affected
-                    bottom=False,      # ticks along the bottom edge are off
-                    top=False,         # ticks along the top edge are off
-                    labelbottom=False,
-                    pad=15)
+        axis="x",  # changes apply to the x-axis
+        which="both",  # both major and minor ticks are affected
+        bottom=False,  # ticks along the bottom edge are off
+        top=False,  # ticks along the top edge are off
+        labelbottom=False,
+        pad=15,
+    )
     # add secondary axis ticks
-    subplot.secondary_xaxis('top', functions=(time2ntr, ntr2time))
+    subplot.secondary_xaxis("top", functions=(time2ntr, ntr2time))
     # add secondary axis labelS
-    ax2.set_xlabel('TR')
-    subplot.plot(time, trigger, '-', time, block, '-')
-    subplot.fill_between(time, block, where=block >= d, interpolate=True, color='#ffbb6e')
-    ax2.set_title('Starting triggers for selected threshold')
+    ax2.set_xlabel("TR")
+    subplot.plot(time, trigger, "-", time, block, "-")
+    subplot.fill_between(time, block, where=block >= d, interpolate=True, color="#ffbb6e")
+    ax2.set_title("Starting triggers for selected threshold")
     # plot the last spike according to the user threshold
     subplot = fig.add_subplot(224)
-    subplot.set_xlim([tr * (num_timepoints_expected) - 4,
-                      tr * (num_timepoints_expected) + 4])
-    subplot.set_xlabel('Seconds')
-    subplot.set_ylabel('Volts')
+    subplot.set_xlim([tr * (num_timepoints_expected) - 4, tr * (num_timepoints_expected) + 4])
+    subplot.set_xlabel("Seconds")
+    subplot.set_ylabel("Volts")
     subplot.set_ylim([-0.2, thr * 3])
     ax2 = subplot.twiny()
-    ax2.set_xticklabels('')
+    ax2.set_xticklabels("")
     ax2.tick_params(
-                    axis='x',          # changes apply to the x-axis
-                    which='both',      # both major and minor ticks are affected
-                    bottom=False,      # ticks along the bottom edge are off
-                    top=False,         # ticks along the top edge are off
-                    labelbottom=False,
-                    pad=15)
-    subplot.secondary_xaxis('top', functions=(time2ntr, ntr2time))
-    ax2.set_xlabel('TR')
-    ax2.set_title('Ending triggers for selected threshold')
-    subplot.plot(time, trigger, '-', time, block, '-')
-    subplot.fill_between(time, block, where=block >= d, interpolate=True, color='#ffbb6e')
-    if 'PYTEST_CURRENT_TEST' not in os.environ:
-        plt.savefig(fileprefix + '_trigger_time.png', dpi=dpi)
+        axis="x",  # changes apply to the x-axis
+        which="both",  # both major and minor ticks are affected
+        bottom=False,  # ticks along the bottom edge are off
+        top=False,  # ticks along the top edge are off
+        labelbottom=False,
+        pad=15,
+    )
+    subplot.secondary_xaxis("top", functions=(time2ntr, ntr2time))
+    ax2.set_xlabel("TR")
+    ax2.set_title("Ending triggers for selected threshold")
+    subplot.plot(time, trigger, "-", time, block, "-")
+    subplot.fill_between(time, block, where=block >= d, interpolate=True, color="#ffbb6e")
+    if "PYTEST_CURRENT_TEST" not in os.environ:
+        plt.savefig(fileprefix + "_trigger_time.png", dpi=dpi)
     plt.close()
 
 
-def export_trigger_plot(phys_in, chtrig, fileprefix, tr, num_timepoints_expected,
-                        filename, sub=None, ses=None, figsize=FIGSIZE,
-                        dpi=SET_DPI):
+def export_trigger_plot(
+    phys_in,
+    chtrig,
+    fileprefix,
+    tr,
+    num_timepoints_expected,
+    filename,
+    sub=None,
+    ses=None,
+    figsize=FIGSIZE,
+    dpi=SET_DPI,
+):
     """
     Save a trigger plot.
 
     Used in main workflow (`phys2bids`), this function minimizes repetition in code for parallel
     workflow (multi-run workflow and default workflow) and maintains readability of code
 
     Parameters
@@ -162,31 +182,39 @@
     figsize: tuple or list of floats
         Size of the figure expressed as (size_x, size_y),
         Default is {FIGSIZE}
     dpi: int
         Desired DPI of the figure,
         Default is {SET_DPI}
     """
-    LGR.info('Plot trigger')
+    LGR.info("Plot trigger")
     # Create trigger plot. If possible, to have multiple outputs in the same
     # place, adds sub and ses label.
     if sub is not None:
-        fileprefix += f'_sub-{sub}'
+        fileprefix += f"_sub-{sub}"
     if ses is not None:
-        fileprefix += f'_ses-{ses}'
+        fileprefix += f"_ses-{ses}"
 
     if phys_in._time_resampled_to_trigger is None:
         timeseries_plot = phys_in.timeseries[0]
     else:
         timeseries_plot = phys_in._time_resampled_to_trigger
 
     # adjust for multi run arguments, iterate through acquisition attributes
-    plot_trigger(timeseries_plot, phys_in.timeseries[chtrig],
-                 fileprefix, tr, phys_in.thr, num_timepoints_expected,
-                 filename, figsize, dpi)
+    plot_trigger(
+        timeseries_plot,
+        phys_in.timeseries[chtrig],
+        fileprefix,
+        tr,
+        phys_in.thr,
+        num_timepoints_expected,
+        filename,
+        figsize,
+        dpi,
+    )
 
 
 def plot_all(ch_name, timeseries, units, freq, infile, outfile, dpi=SET_DPI, size=FIGSIZE):
     """
     Plot all the channels for visualizations and saves them in outfile.
 
     Parameters
@@ -227,15 +255,15 @@
     time = timeseries[0]  # assume time is first channel
     fig.suptitle(os.path.basename(infile))
     for row, timeser in enumerate(timeseries[1:]):
         if timeser.shape != time.shape:
             time_old = np.linspace(0, time[-1], num=timeser.shape[0])
             timeser = np.interp(time, time_old, timeser)
         ax[row].plot(time, timeser)
-        ax[row].set_title(f' Channel {row + 1}: {ch_name[row + 1]}')
+        ax[row].set_title(f" Channel {row + 1}: {ch_name[row + 1]}")
         ax[row].set_ylabel(units[row + 1])
         ax[row].xlim = 30 * 60 * freq[0]  # maximum display of half an hour
         ax[row].grid()
-    ax[row].set_xlabel('seconds')
-    outfile = os.path.join(outfile, os.path.splitext(os.path.basename(infile))[0] + '.png')
-    LGR.info(f'saving channel plot to {outfile}')
-    fig.savefig(outfile, dpi=dpi, bbox_inches='tight')
+    ax[row].set_xlabel("seconds")
+    outfile = os.path.join(outfile, os.path.splitext(os.path.basename(infile))[0] + ".png")
+    LGR.info(f"saving channel plot to {outfile}")
+    fig.savefig(outfile, dpi=dpi, bbox_inches="tight")
```

### Comparing `phys2bids-2.8.4/phys2bids/bids.py` & `phys2bids-2.9.0/phys2bids/bids.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import yaml
 
 from phys2bids import utils
 
 LGR = logging.getLogger(__name__)
 
+# fmt: off
 UNIT_ALIASES = {
                 # kelvin: thermodynamic temperature
                 'kelvin': 'K', 'kelvins': 'K',
                 # mole: amount of substance
                 'mol': 'mol', 'mole': 'mol',
                 # newton: force, weight
                 'newton': 'N', 'newtons': 'N',
@@ -47,14 +48,15 @@
                     # Submultipliers
                     'd': 'd', 'deci': 'd', 'c': 'c', 'centi': 'c',
                     'milli': 'm', 'm': 'm', 'µ': 'µ', 'micro': 'µ',
                     'n': 'n', 'nano': 'n', 'p': 'p', 'pico': 'p',
                     'f': 'f', 'femto': 'f', 'a': 'a', 'atto': 'a',
                     'z': 'z', 'zepto': 'z', 'y': 'y', 'yocto': 'y',
 }
+# fmt: on
 
 
 def bidsify_units(orig_unit):
     """
     Read the input unit of measure and use the dictionary of aliases to bidsify its value.
 
     It is possible to make simple conversions.
@@ -77,34 +79,34 @@
     """
     # for every unit alias in the dict
     unit = orig_unit.lower()
     for u_key in UNIT_ALIASES.keys():
         # check that u_key is part of unit
         if unit.endswith(u_key):
             new_unit = UNIT_ALIASES[u_key]
-            unit = unit[:-len(u_key)]
-            if unit != '':
+            unit = unit[: -len(u_key)]
+            if unit != "":
                 # for every prefix alias
-                prefix = PREFIX_ALIASES.get(unit, '')
-                if prefix == '':
-                    LGR.warning(f'The given unit prefix {unit} does not '
-                                'have aliases, passing it as is')
-                    prefix = orig_unit[:len(unit)]
+                prefix = PREFIX_ALIASES.get(unit, "")
+                if prefix == "":
+                    LGR.warning(
+                        f"The given unit prefix {unit} does not " "have aliases, passing it as is"
+                    )
+                    prefix = orig_unit[: len(unit)]
 
                 return prefix + new_unit
             else:
                 return new_unit
 
     # If we conclude the loop without returning, it means the unit doesn't have aliases
-    LGR.warning(f'The given unit {orig_unit} does not have aliases, '
-                f'passing it as is')
+    LGR.warning(f"The given unit {orig_unit} does not have aliases, " f"passing it as is")
     return orig_unit
 
 
-def use_heuristic(heur_file, sub, ses, filename, outdir, take='', record_label=''):
+def use_heuristic(heur_file, sub, ses, filename, outdir, take="", record_label=""):
     """
     Import and use the heuristic specified by the user to rename the file.
 
     Parameters
     ----------
     heur_file: path
         Fullpath to heuristic file.
@@ -129,55 +131,63 @@
     ------
     KeyError
         if `bids_keys['task']` is empty
     """
     utils.check_file_exists(heur_file)
 
     # Initialise a dictionary of bids_keys that has already "recording"
-    bids_keys = {'sub': '', 'ses': '', 'task': '', 'acq': '', 'ce': '',
-                 'dir': '', 'rec': '', 'run': '', 'recording': record_label}
+    bids_keys = {
+        "sub": "",
+        "ses": "",
+        "task": "",
+        "acq": "",
+        "ce": "",
+        "dir": "",
+        "rec": "",
+        "run": "",
+        "recording": record_label,
+    }
 
     # Start filling bids_keys dictionary and path with subject and session
-    if sub.startswith('sub-'):
-        bids_keys['sub'] = sub[4:]
+    if sub.startswith("sub-"):
+        bids_keys["sub"] = sub[4:]
         fldr = os.path.join(outdir, sub)
     else:
-        bids_keys['sub'] = sub
-        fldr = os.path.join(outdir, f'sub-{sub}')
+        bids_keys["sub"] = sub
+        fldr = os.path.join(outdir, f"sub-{sub}")
 
     if ses:
-        if ses.startswith('ses-'):
-            bids_keys['ses'] = ses[4:]
+        if ses.startswith("ses-"):
+            bids_keys["ses"] = ses[4:]
             fldr = os.path.join(fldr, ses)
         else:
-            bids_keys['ses'] = ses
-            fldr = os.path.join(fldr, f'ses-{ses}')
+            bids_keys["ses"] = ses
+            fldr = os.path.join(fldr, f"ses-{ses}")
 
     # Load heuristic and use it to fill dictionary
     heur = utils.load_heuristic(heur_file)
     bids_keys.update(heur.heur(Path(filename).stem, take))
 
     # If bids_keys['task'] is still empty, stop the program
-    if not bids_keys['task']:
-        LGR.warning(f'The heuristic {heur_file} could not deal with'
-                    f'{Path(filename).stem}')
+    if not bids_keys["task"]:
+        LGR.warning(f"The heuristic {heur_file} could not deal with" f"{Path(filename).stem}")
         raise KeyError('No "task" attribute found')
 
     # Compose name by looping in the bids_keys dictionary
     # and adding nonempty keys
-    name = ''
+    name = ""
     for key in bids_keys:
-        if bids_keys[key] != '':
-            name = f'{name}{key}-{bids_keys[key]}_'
+        if bids_keys[key] != "":
+            name = f"{name}{key}-{bids_keys[key]}_"
 
     # Finish path, create it, add filename, export
-    fldr = os.path.join(fldr, 'func')
+    fldr = os.path.join(fldr, "func")
     os.makedirs(fldr, exist_ok=True)
 
-    heurpath = os.path.join(fldr, f'{name}physio')
+    heurpath = os.path.join(fldr, f"{name}physio")
 
     return heurpath
 
 
 def participants_file(outdir, yml, sub):
     """
     Create participants.tsv file if it does not exist.
@@ -191,65 +201,66 @@
         Full path to the output directory.
     yml: path
         Full path to the yaml file.
     sub: str
         Subject ID.
 
     """
-    LGR.info('Updating participants.tsv ...')
-    file_path = os.path.join(outdir, 'participants.tsv')
+    LGR.info("Updating participants.tsv ...")
+    file_path = os.path.join(outdir, "participants.tsv")
     if not os.path.exists(file_path):
-        LGR.warning('phys2bids could not find participants.tsv')
+        LGR.warning("phys2bids could not find participants.tsv")
         # Read yaml info if file exists
-        if '.yml' in yml and os.path.exists(yml):
-            LGR.info('Using yaml data to populate participants.tsv')
+        if ".yml" in yml and os.path.exists(yml):
+            LGR.info("Using yaml data to populate participants.tsv")
             with open(yml) as f:
                 yaml_data = yaml.load(f, Loader=yaml.FullLoader)
-            p_id = f'sub-{sub}'
-            p_age = yaml_data['participant']['age']
-            p_sex = yaml_data['participant']['sex']
-            p_handedness = yaml_data['participant']['handedness']
+            p_id = f"sub-{sub}"
+            p_age = yaml_data["participant"]["age"]
+            p_sex = yaml_data["participant"]["sex"]
+            p_handedness = yaml_data["participant"]["handedness"]
         else:
-            LGR.info('No yaml file was provided. Using phys2bids data to '
-                     'populate participants.tsv')
+            LGR.info(
+                "No yaml file was provided. Using phys2bids data to " "populate participants.tsv"
+            )
             # Fill in with data from phys2bids
-            p_id = f'sub-{sub}'
-            p_age = 'n/a'
-            p_sex = 'n/a'
-            p_handedness = 'n/a'
+            p_id = f"sub-{sub}"
+            p_age = "n/a"
+            p_sex = "n/a"
+            p_handedness = "n/a"
 
         # Write to participants.tsv file
-        header = ['participant_id', 'age', 'sex', 'handedness']
+        header = ["participant_id", "age", "sex", "handedness"]
         utils.append_list_as_row(file_path, header)
 
         participants_data = [p_id, p_age, p_sex, p_handedness]
         utils.append_list_as_row(file_path, participants_data)
 
     else:  # If participants.tsv exists only update when subject is not there
-        LGR.info('phys2bids found participants.tsv. Updating if needed...')
+        LGR.info("phys2bids found participants.tsv. Updating if needed...")
         # Find participant_id column in header
-        pf = open(file_path, 'r')
+        pf = open(file_path, "r")
         header = pf.readline().split("\t")
         header_length = len(header)
         pf.close()
-        p_id_idx = header.index('participant_id')
+        p_id_idx = header.index("participant_id")
 
         # Check if subject is already in the file
         sub_exists = False
         with open(file_path) as pf:
             tsvreader = reader(pf, delimiter="\t")
             for line in tsvreader:
                 if sub in line[p_id_idx]:
                     sub_exists = True
                     break
         # Only append to file if subject is not in the file
         if not sub_exists:
-            LGR.info(f'Appending subject sub-{sub} to participants.tsv ...')
-            participants_data = ['n/a'] * header_length
-            participants_data[p_id_idx] = f'sub-{sub}'
+            LGR.info(f"Appending subject sub-{sub} to participants.tsv ...")
+            participants_data = ["n/a"] * header_length
+            participants_data[p_id_idx] = f"sub-{sub}"
             utils.append_list_as_row(file_path, participants_data)
 
 
 def dataset_description_file(outdir):
     """
     Create dataset_description.json file if it does not exist.
 
@@ -258,21 +269,25 @@
     Parameters
     ----------
     outdir: path
         Full path to the output directory.
 
     """
     # dictionary that will be written for the basic dataset description version
-    data_dict = {"Name": os.path.splitext(os.path.basename(outdir))[0],
-                 "BIDSVersion": "1.4.0", "DatasetType": "raw"}
-    file_path = os.path.join(outdir, 'dataset_description.json')
+    data_dict = {
+        "Name": os.path.splitext(os.path.basename(outdir))[0],
+        "BIDSVersion": "1.4.0",
+        "DatasetType": "raw",
+    }
+    file_path = os.path.join(outdir, "dataset_description.json")
     # check if dataset_description.json exists, if it doesn't create it
     if not os.path.exists(file_path):
-        LGR.warning('phys2bids could not find dataset_description.json,'
-                    'generating it with provided info')
+        LGR.warning(
+            "phys2bids could not find dataset_description.json," "generating it with provided info"
+        )
         utils.write_json(file_path, data_dict)
 
 
 def readme_file(outdir):
     """
     Create README file if it does not exist.
 
@@ -280,13 +295,15 @@
 
     Parameters
     ----------
     outdir: path
         Full path to the output directory.
 
     """
-    file_path = os.path.join(outdir, 'README')
+    file_path = os.path.join(outdir, "README")
     if not os.path.exists(file_path):
-        text = 'Empty README, please fill in describing the dataset in more detail.'
-        LGR.warning('phys2bids could not find README,'
-                    'generating it EMPTY, please fill in the necessary info')
-        utils.write_file(file_path, '', text)
+        text = "Empty README, please fill in describing the dataset in more detail."
+        LGR.warning(
+            "phys2bids could not find README,"
+            "generating it EMPTY, please fill in the necessary info"
+        )
+        utils.write_file(file_path, "", text)
```

### Comparing `phys2bids-2.8.4/phys2bids/utils.py` & `phys2bids-2.9.0/phys2bids/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 from csv import writer
 from pathlib import Path
 
 LGR = logging.getLogger(__name__)
 
-SUPPORTED_FTYPES = ('acq', 'txt', 'mat', 'gep')
+SUPPORTED_FTYPES = ("acq", "txt", "mat", "gep")
 
 
 def check_input_ext(filename, ext):
     """
     Check that the given file has the given extension.
 
     It also treats composite extensions such as `.tsv.gz`,
@@ -27,19 +27,19 @@
         Desired file name extension. Doesn't matter if preceded by `.`
 
     Returns
     -------
     Path(filename).with_suffix(ext): path
         Path representing the input filename, but with corrected extension.
     """
-    if filename.endswith('.gz'):
+    if filename.endswith(".gz"):
         filename = filename[:-3]
 
-    if not ext.startswith('.'):
-        ext = '.' + ext
+    if not ext.startswith("."):
+        ext = "." + ext
 
     return Path(filename).with_suffix(ext)
 
 
 def check_input_type(filename, indir):
     """
     Check which supported type is the filename.
@@ -74,22 +74,24 @@
     for ftype in SUPPORTED_FTYPES:
         fname = check_input_ext(filename, ftype)
         if os.path.isfile(os.path.join(indir, fname)):
             fftype_found = True
             break
 
     if fftype_found:
-        LGR.info(f'File extension is .{ftype}')
-        LGR.warning('If both acq and txt files exist in the path, acq will be selected.')
+        LGR.info(f"File extension is .{ftype}")
+        LGR.warning("If both acq and txt files exist in the path, acq will be selected.")
         return fname, ftype
     else:
-        raise Exception(f'The file {filename} was not found in {indir}'
-                        f' or {ftype} is not supported yet.\n'
-                        f'phys2bids currently supports:'
-                        f' {", ".join(SUPPORTED_FTYPES)}')
+        raise Exception(
+            f"The file {filename} was not found in {indir}"
+            f" or {ftype} is not supported yet.\n"
+            f"phys2bids currently supports:"
+            f' {", ".join(SUPPORTED_FTYPES)}'
+        )
 
 
 def check_file_exists(filename):
     """
     Check if file exists.
 
     Parameters
@@ -100,15 +102,15 @@
 
     Raises
     ------
     FileNotFoundError
         If the file doesn't exists.
     """
     if not os.path.isfile(filename) and filename is not None:
-        raise FileNotFoundError(f'The file {filename} does not exist!')
+        raise FileNotFoundError(f"The file {filename} does not exist!")
 
 
 def check_ge(filename, indir):
     """
     Check if the input file is from a GE scanner.
 
     If so, copy the file while adding a ".gep" filename extension.
@@ -119,75 +121,74 @@
         A string representing a file name or a fullpath
         to a file
     indir: str or path
         A string representing a folder in which the file is,
         or a fullpath to such folder
 
     """
-    from numpy import loadtxt
     from glob import glob
 
-    ge_types = ['ECGData', 'PPGData', 'RESPData']
+    from numpy import loadtxt
+
+    ge_types = ["ECGData", "PPGData", "RESPData"]
 
     # Ensure the file exists
     if not os.path.isfile(os.path.join(indir, filename)) and filename is not None:
-        raise FileNotFoundError(f'The file {filename} does not exist!')
+        raise FileNotFoundError(f"The file {filename} does not exist!")
 
     # Check if it's a GE file and add file extension
     # Do the same for other linked files
     if any(ge_type in filename for ge_type in ge_types):
-        LGR.info('Filename with the form of GE physiological data entered')
+        LGR.info("Filename with the form of GE physiological data entered")
         #  Check that the file contents correspond to the format of GE files
         try:
             test_data = loadtxt(os.path.join(indir, filename))
             if len(test_data.shape) > 1:
-                LGR.info('File contents do not match GE format: multiple columns')
-                raise TypeError('File contents do not match GE format: multiple columns')
+                LGR.info("File contents do not match GE format: multiple columns")
+                raise TypeError("File contents do not match GE format: multiple columns")
         except ValueError:
-            LGR.info('File contents do not match GE format: not numerical')
-            raise TypeError('File contents do not match GE format: not numerical') from None
+            LGR.info("File contents do not match GE format: not numerical")
+            raise TypeError("File contents do not match GE format: not numerical") from None
         # Look for related GE files based on timestamp in name
-        fnames = glob(os.path.join(indir, f'*{filename[-20:]}*'))
+        fnames = glob(os.path.join(indir, f"*{filename[-20:]}*"))
         # Catch any tsv or json files
         for fname in fnames[:]:
-            if '.tsv.gz' in fname:
+            if ".tsv.gz" in fname:
                 fnames.remove(fname)
-            if '.json' in fname:
+            if ".json" in fname:
                 fnames.remove(fname)
         # Add extension to original so it's logged appropriately
-        if 'gep' not in filename[:-3]:
-            new_filename = filename + '.gep'
-            copy_file(os.path.join(indir, filename),
-                      os.path.join(indir, new_filename))
+        if "gep" not in filename[:-3]:
+            new_filename = filename + ".gep"
+            copy_file(os.path.join(indir, filename), os.path.join(indir, new_filename))
             LGR.info(f'Appending ".gep" extension to {filename}')
         else:
             LGR.info(f'".gep" extension already present in {filename}.')
         # Add extension to additional files and log these
         # Remove the original filename from the list
         fnames.remove(os.path.join(indir, filename))
         try:
-            fnames.remove(os.path.join(indir, filename + '.gep'))
+            fnames.remove(os.path.join(indir, filename + ".gep"))
         except ValueError:
             pass
         # Log if there are no additional files
         if len(fnames) == 0:
-            LGR.info('No additional GE physiological files found')
+            LGR.info("No additional GE physiological files found")
         else:
-            LGR.info('Additional GE physiological file(s) found')
+            LGR.info("Additional GE physiological file(s) found")
             for fname in fnames[:]:
-                if 'gep' in fname[-3:]:
+                if "gep" in fname[-3:]:
                     LGR.info(f'".gep" extension already present in {fname.split("/")[-1]}.')
                 else:
-                    new_fname = fname + '.gep'
-                    copy_file(os.path.join(indir, fname),
-                              os.path.join(indir, new_fname))
+                    new_fname = fname + ".gep"
+                    copy_file(os.path.join(indir, fname), os.path.join(indir, new_fname))
                     LGR.info(f'Appending ".gep" extension to {fname.split("/")[-1]}.')
 
 
-def copy_file(oldpath, newpath, ext=''):
+def copy_file(oldpath, newpath, ext=""):
     """
     Copy file from oldpath to newpath.
 
     If file already exists, remove it first.
 
     Parameters
     ----------
@@ -232,15 +233,15 @@
 
     Notes
     -----
     Outcome:
     filename + ext:
         Creates new file `filename.ext`.
     """
-    with open(filename + ext, 'w') as text_file:
+    with open(filename + ext, "w") as text_file:
         print(text, file=text_file)
 
 
 def write_json(filename, data, **kwargs):
     """
     Output a json file with the given data inside.
 
@@ -254,17 +255,17 @@
 
     Notes
     -----
     Outcome:
     filename:
         Creates new file `filename.json`.
     """
-    if not filename.endswith('.json'):
-        filename += '.json'
-    with open(filename, 'w') as out:
+    if not filename.endswith(".json"):
+        filename += ".json"
+    with open(filename, "w") as out:
         json.dump(data, out, **kwargs)
 
 
 def load_heuristic(heuristic):
     """
     Load `heuristic`, returning a callable Python module.
 
@@ -275,26 +276,27 @@
     """
     if os.path.lexists(heuristic):
         heuristic_file = os.path.realpath(heuristic)
         path, fname = os.path.split(heuristic_file)
         try:
             old_syspath = sys.path[:]
             sys.path.append(path)
-            mod = __import__(fname.split('.')[0])
+            mod = __import__(fname.split(".")[0])
             mod.filename = heuristic_file
         finally:
             sys.path = old_syspath
     else:
         from importlib import import_module
+
         try:
-            mod = import_module(f'phys2bids.heuristics.{heuristic}')
+            mod = import_module(f"phys2bids.heuristics.{heuristic}")
             # remove c or o from pyc/pyo
-            mod.filename = mod.__file__.rstrip('co')
+            mod.filename = mod.__file__.rstrip("co")
         except Exception as exc:
-            raise ImportError(f'Failed to import heuristic {heuristic}: {exc}')
+            raise ImportError(f"Failed to import heuristic {heuristic}: {exc}")
     return mod
 
 
 def append_list_as_row(file_name, list_of_elem):
     """
     Append list as row.
 
@@ -303,12 +305,12 @@
     filename: str or path
         A string representing a file name or a fullpath
         to a file
     list_of_elem: list
         The list to be appended to the file.
     """
     # Open file in append mode
-    with open(file_name, 'a+', newline='') as write_obj:
+    with open(file_name, "a+", newline="") as write_obj:
         # Create a writer object from csv module
-        csv_writer = writer(write_obj, delimiter='\t')
+        csv_writer = writer(write_obj, delimiter="\t")
         # Add contents of list as last row in the csv file
         csv_writer.writerow(list_of_elem)
```

### Comparing `phys2bids-2.8.4/phys2bids/slice4phys.py` & `phys2bids-2.9.0/phys2bids/slice4phys.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,18 @@
     take_timestamps = {}
 
     # Express the padding in samples equivalent
     padding_fr = padding * phys_in.freq[0]
 
     # enumerate user input  num_timepoints_expected
     for take_idx, take_tps in enumerate(ntp_list):
-
         # correct time offset for this iteration's object
-        phys_in.check_trigger_amount(thr=thr, num_timepoints_expected=take_tps,
-                                     tr=tr_list[take_idx])
+        phys_in.check_trigger_amount(
+            thr=thr, num_timepoints_expected=take_tps, tr=tr_list[take_idx]
+        )
         # If it's the very first take, start the take at sample 0,
         # otherwise start is first trigger (adjust with padding later)
         if take_idx == 0:
             take_start = 0
         else:
             take_start = int(np.where(np.isclose(phys_in.timeseries[0], 0))[0])
 
@@ -69,17 +69,19 @@
         # pick first value of time array that is over specified take length
         # where returns list of values over end_sec and its dtype, choose [list][first value]
         # Check if end_sec is above the end of the timeseries (it happens for noisy cases)
         if phys_in.timeseries[0][-1] > end_sec:
             take_end = int(np.where(phys_in.timeseries[0] > end_sec)[0][0] + padding_fr)
         else:
             take_end = int(phys_in.timeseries[0].shape[0] - 1)
-            LGR.warning(f'The computed end point in second was {end_sec}, '
-                        'but current timeseries only lasts up to '
-                        f'{phys_in.timeseries[0][-1]}')
+            LGR.warning(
+                f"The computed end point in second was {end_sec}, "
+                "but current timeseries only lasts up to "
+                f"{phys_in.timeseries[0][-1]}"
+            )
 
         update = int(take_end - padding_fr + 1)
 
         # if the padding is too much for the remaining timeseries length
         # then the padding stops at the end of recording
         if phys_in.timeseries[0].shape[0] < take_end:
             take_end = phys_in.timeseries[0].shape[0]
@@ -94,22 +96,27 @@
             take_start = int(take_start + previous_end_index - 2 * padding_fr)
             # update take_end, removing the padding of the previous end
             take_end = int(take_end + previous_end_index - padding_fr)
 
         # Save *start* and *end_index* in dictionary along with *time_offset* and *ntp found*
         # dict key must be readable by human
         # LGRinfo
-        LGR.info('\n--------------------------------------------------------------\n'
-                 f'Slicing between {(take_start/phys_in.freq[phys_in.trigger_idx])} seconds and '
-                 f'{take_end/phys_in.freq[phys_in.trigger_idx]} seconds\n'
-                 '--------------------------------------------------------------')
-
-        take_timestamps[take_idx + 1] = (take_start, take_end,
-                                         phys_in.time_offset,
-                                         phys_in.num_timepoints_found)
+        LGR.info(
+            "\n--------------------------------------------------------------\n"
+            f"Slicing between {(take_start/phys_in.freq[phys_in.trigger_idx])} seconds and "
+            f"{take_end/phys_in.freq[phys_in.trigger_idx]} seconds\n"
+            "--------------------------------------------------------------"
+        )
+
+        take_timestamps[take_idx + 1] = (
+            take_start,
+            take_end,
+            phys_in.time_offset,
+            phys_in.num_timepoints_found,
+        )
 
         # update the object so that next iteration will look for the first trigger
         # after previous take's last trigger. maybe padding extends to next take
         phys_in = deepcopy(phys_in[update:-1])
 
     return take_timestamps
 
@@ -137,26 +144,27 @@
     phys_in_slices: dict
         keys start by `take 1` until last (`take n`).
         items are slices of BlueprintInput objects based on take attributes returned by
         internal function (`slice4phys` takes the same arguments as `find_takes`)
     """
     phys_in_slices = {}
     # inform the user
-    LGR.warning('\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~'
-                '\nphys2bids will split the input file according to the given -tr and -ntp'
-                ' arguments'
-                '\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~')
+    LGR.warning(
+        "\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"
+        "\nphys2bids will split the input file according to the given -tr and -ntp"
+        " arguments"
+        "\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"
+    )
     # Find the timestamps
     take_timestamps = find_takes(phys_in, ntp_list, tr_list, thr, padding)
     for n, take in enumerate(take_timestamps.keys()):
-
         # tmp variable to collect take's info
         take_attributes = take_timestamps[take]
 
-        phys_in_slices[take] = deepcopy(phys_in[take_attributes[0]:take_attributes[1]])
+        phys_in_slices[take] = deepcopy(phys_in[take_attributes[0] : take_attributes[1]])
 
         # take check_trigger amount
-        phys_in_slices[take].check_trigger_amount(thr=thr,
-                                                  num_timepoints_expected=ntp_list[n],
-                                                  tr=tr_list[n])
+        phys_in_slices[take].check_trigger_amount(
+            thr=thr, num_timepoints_expected=ntp_list[n], tr=tr_list[n]
+        )
 
     return phys_in_slices
```

### Comparing `phys2bids-2.8.4/phys2bids.egg-info/PKG-INFO` & `phys2bids-2.9.0/phys2bids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2bids
-Version: 2.8.4
+Version: 2.9.0
 Summary: Python library to convert physiological data files into BIDS format
 Home-page: https://github.com/physiopy/phys2bids
 Author: phys2bids developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/physiopy/phys2bids
@@ -157,15 +157,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: phys2bids
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: doc
-Provides-Extra: interfaces
-Provides-Extra: acq
+Provides-Extra: mat
 Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: all
+Provides-Extra: spike2
 Provides-Extra: duecredit
 Provides-Extra: style
-Provides-Extra: mat
-Provides-Extra: all
+Provides-Extra: acq
+Provides-Extra: interfaces
```

### Comparing `phys2bids-2.8.4/phys2bids.egg-info/SOURCES.txt` & `phys2bids-2.9.0/phys2bids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.4/LICENSE` & `phys2bids-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.4/README.md` & `phys2bids-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.4/setup.cfg` & `phys2bids-2.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -32,31 +32,36 @@
 	pytest >=5.3
 test_suite = pytest
 zip_safe = False
 packages = find:
 include_package_data = True
 
 [options.extras_require]
+spike2 = 
+	sonpy >=1.7.5;python_version=='3.7.*,3.8.*,3.9.*'
 acq = 
 	bioread >=1.0.5
 mat = 
 	pymatreader >=0.0.24
 duecredit = 
 	duecredit
 doc = 
 	sphinx >=2.0
 	sphinx-argparse
 	sphinx_rtd_theme
 style = 
-	flake8 >=3.7
-	flake8-docstrings >=1.5
+	flake8 >=4.0
+	black
+	isort <6.0.0
+	pydocstyle
 	codespell
 interfaces = 
 	%(acq)s
 	%(mat)s
+	%(spike2)s
 test = 
 	pytest >=5.3
 	pytest-cov
 	coverage
 	%(interfaces)s
 	%(style)s
 all = 
@@ -73,26 +78,44 @@
 	phys2bids/tests/data/*
 
 [options.entry_points]
 console_scripts = 
 	phys2bids=phys2bids.phys2bids:_main
 
 [flake8]
+doctest = True
 exclude = 
 	*build/
 	heuristics
 	tests
 	_version.py
 	./phys2bids/cli/__init__.py
 	./phys2bids/tests/*
 	versioneer.py
-ignore = E126, E402, W503, E226
-max-line-length = 99
+ignore = E126, E402, W503, E226, F401, F811
+max-line-length = 88
+extend-ignore = E203, E501
+extend-select = B950
 per-file-ignores = 
-	*/__init__.py:F401
+	workflow.py:D401
+
+[isort]
+profile = black
+skip_gitignore = true
+extend_skip = 
+	.autorc
+	.coverage*
+	.readthedocs.yml
+	.zenodo.json
+	codecov.yml
+	setup.py
+	versioneer.py
+	phys2bids/_version.py
+skip_glob = 
+	docs/*
 
 [pydocstyle]
 convention = numpy
 match = 
 	nigsp/*.py
 match_dir = nigsp/[^tests,^heuristics]*
```


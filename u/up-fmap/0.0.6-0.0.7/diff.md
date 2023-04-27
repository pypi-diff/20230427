# Comparing `tmp/up_fmap-0.0.6.tar.gz` & `tmp/up_fmap-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_fmap-0.0.6.tar", last modified: Wed Apr 19 23:40:58 2023, max compression
+gzip compressed data, was "up_fmap-0.0.7.tar", last modified: Thu Apr 27 18:50:47 2023, max compression
```

## Comparing `up_fmap-0.0.6.tar` & `up_fmap-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:40:47.000000 up_fmap-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:40:58.371481 up_fmap-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-19 23:40:47.000000 up_fmap-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:40:58.371481 up_fmap-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-19 23:40:47.000000 up_fmap-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-19 23:40:47.000000 up_fmap-0.0.6/test/test_up_fmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/up_fmap/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:40:47.000000 up_fmap-0.0.6/up_fmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-04-19 23:40:47.000000 up_fmap-0.0.6/up_fmap/fmap_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/up_fmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:50:47.007117 up_fmap-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 18:50:32.000000 up_fmap-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 18:50:47.007117 up_fmap-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-27 18:50:32.000000 up_fmap-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:50:47.007117 up_fmap-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-27 18:50:32.000000 up_fmap-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:50:47.003117 up_fmap-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-27 18:50:32.000000 up_fmap-0.0.7/test/test_up_fmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:50:47.003117 up_fmap-0.0.7/up_fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 18:50:32.000000 up_fmap-0.0.7/up_fmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-27 18:50:32.000000 up_fmap-0.0.7/up_fmap/fmap_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:50:47.007117 up_fmap-0.0.7/up_fmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 18:50:46.000000 up_fmap-0.0.7/up_fmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 18:50:46.000000 up_fmap-0.0.7/up_fmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:50:46.000000 up_fmap-0.0.7/up_fmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 18:50:46.000000 up_fmap-0.0.7/up_fmap.egg-info/top_level.txt
```

### Comparing `up_fmap-0.0.6/LICENSE` & `up_fmap-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.6/README.md` & `up_fmap-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.6/setup.py` & `up_fmap-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def run(self):
         install_FMAP()
         develop.run(self)
 
 
 setup(
     name="up_fmap",
-    version="0.0.6",
+    version="0.0.7",
     description="up_fmap",
     author="Alejandro Torreño, Eva Onaindia and Oscar Sapena",
     author_email="onaindia@dsic.upv.es",
     packages=["up_fmap"],
     package_data={"": ["FMAP/FMAP.jar"]},
     cmdclass={"build_py": InstallFMAP, "develop": InstallFMAPdevelop},
     license="APACHE",
```

### Comparing `up_fmap-0.0.6/test/test_up_fmap.py` & `up_fmap-0.0.7/test/test_up_fmap.py`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.6/up_fmap/fmap_planner.py` & `up_fmap-0.0.7/up_fmap/fmap_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     ) -> "up.engines.results.PlanGenerationResult":
         assert isinstance(problem, up.model.Problem) or isinstance(
             problem, up.model.multi_agent.MultiAgentProblem
         )
         plan = None
         logs: List["up.engines.results.LogMessage"] = []
         with tempfile.TemporaryDirectory() as tempdir:
-            w = MAPDDLWriter(problem)
+            w = MAPDDLWriter(problem, explicit_false_initial_states=True)
             domain_filename = os.path.join(tempdir, "domain_pddl/")
             problem_filename = os.path.join(tempdir, "problem_pddl/")
             plan_filename = os.path.join(tempdir, "plan.txt")
             plan_filename = "ma_pddl_" + plan_filename
             w.write_ma_domain(domain_filename)
             w.write_ma_problem(problem_filename)
             cmd = self._get_cmd_ma(problem, domain_filename, problem_filename)
```


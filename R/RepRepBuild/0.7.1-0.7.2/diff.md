# Comparing `tmp/RepRepBuild-0.7.1.tar.gz` & `tmp/RepRepBuild-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.7.1.tar", last modified: Wed Apr 19 14:05:26 2023, max compression
+gzip compressed data, was "RepRepBuild-0.7.2.tar", last modified: Thu Apr 27 13:55:20 2023, max compression
```

## Comparing `RepRepBuild-0.7.1.tar` & `RepRepBuild-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.1/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.1/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-19 14:04:50.000000 RepRepBuild-0.7.1/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.318328 RepRepBuild-0.7.1/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.319328 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.329328 RepRepBuild-0.7.1/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.1/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)    11114 2023-04-19 14:01:26.000000 RepRepBuild-0.7.1/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.1/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.1/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.1/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4530 2023-04-19 14:02:59.000000 RepRepBuild-0.7.1/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.1/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4119 2023-04-19 09:59:27.000000 RepRepBuild-0.7.1/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.1/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.7.1/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.1/src/reprepbuild/zip.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.466222 RepRepBuild-0.7.2/
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.2/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-27 13:55:20.465222 RepRepBuild-0.7.2/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.2/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-27 13:54:45.000000 RepRepBuild-0.7.2/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-27 13:55:20.466222 RepRepBuild-0.7.2/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.448222 RepRepBuild-0.7.2/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.449222 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.464222 RepRepBuild-0.7.2/src/reprepbuild/
+-rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.2/src/reprepbuild/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)    11425 2023-04-27 13:39:02.000000 RepRepBuild-0.7.2/src/reprepbuild/__main__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.2/src/reprepbuild/articlezip.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.2/src/reprepbuild/bibtex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.2/src/reprepbuild/latex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4530 2023-04-19 14:02:59.000000 RepRepBuild-0.7.2/src/reprepbuild/latexdep.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.2/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4119 2023-04-19 09:59:27.000000 RepRepBuild-0.7.2/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.2/src/reprepbuild/repeat.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5130 2023-04-19 15:07:08.000000 RepRepBuild-0.7.2/src/reprepbuild/utils.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.2/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.7.1/COPYING` & `RepRepBuild-0.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/PKG-INFO` & `RepRepBuild-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.1
+Version: 0.7.2
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.1/README.md` & `RepRepBuild-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/pyproject.toml` & `RepRepBuild-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
```

### Comparing `RepRepBuild-0.7.1/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.7.2/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.1
+Version: 0.7.2
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.1/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.7.2/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/__init__.py` & `RepRepBuild-0.7.2/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/__main__.py` & `RepRepBuild-0.7.2/src/reprepbuild/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,44 +179,49 @@
         "pool": "console",
         "default": True,
     }
 
 
 def svg_pattern(path):
     """Make ninja build commands to convert SVG to PDF files."""
-    result = re.match(r"(?P<name>[a-z0-9/-]+).svg$", path)
+    result = re.match(r"(?P<name>[a-z][a-z0-9-]*/[a-zA-Z0-9/_-]+).svg$", path)
     if not result:
         return
     name = result.group("name")
     yield {
         "outputs": f"{name}.pdf",
         "rule": "svgtopdf",
         "inputs": f"{name}.svg",
         "default": True,
     }
 
 
 def python_script_pattern(path):
     """Make ninja build commands for python scripts."""
     # for any valid python file
-    if not re.match(r"(?P<name>([a-z0-9_-]+/)*[a-z][a-z0-9_-]*).py$", path):
+    if not re.match(r"(?P<name>results-[a-z0-9-]*/[a-zA-Z0-9/_-]*).py$", path):
         return
 
     # Call reprepbuild_info as if the script is running in its own directory.
     orig_workdir = os.getcwd()
     workdir, fn_py = os.path.split(path)
     prefix = fn_py[:-3]
     try:
         # Load the script in its own directory
         os.chdir(workdir)
         pythonscript = import_python_path(fn_py)
 
+        # Ignore script if the import failed.
+        if pythonscript is None:
+            yield "Skipped: import failed"
+            return
         # Get the relevant functions
         reprepbuild_info = getattr(pythonscript, "reprepbuild_info", None)
         if reprepbuild_info is None:
+            yield "Skipped: missing reprepbuild_info"
             return
         reprepbuild_cases = getattr(pythonscript, "reprepbuild_cases", None)
         if reprepbuild_cases is None:
             build_cases = [[]]
         else:
             build_cases = reprepbuild_cases()
 
@@ -264,42 +269,41 @@
                 r"For example, use '.itex' instead and update the \input commands accordingly."
             )
 
 
 def write_ninja(patterns, rules):
     """Search through the source for patterns that can be translated into ninja build commands."""
     # Loop over all files and create rules and builds for them
-    rule_names = set()
-    builds = []
-    defaults = []
-    for path in glob("**", recursive=True):
-        for pattern in patterns:
-            for build in pattern(path):
-                if build.get("default", False):
-                    defaults.append(build["outputs"])
-                    del build["default"]
-                check_tex_outputs(build.get("outputs", None))
-                check_tex_outputs(build.get("implicit_outputs", None))
-                rule_names.add(build["rule"])
-                builds.append(build)
-
-    # Sanity check
-    if len(builds) == 0:
-        print("Nothing to build. Wrong current directory?")
-        sys.exit(-1)
-
-    # Format rules and builds
     with open("build.ninja", "w") as f:
         writer = Writer(f, 100)
-        for rule_name in rule_names:
-            writer.rule(name=rule_name, **rules[rule_name])
-        for build in builds:
-            writer.build(**build)
-        for default in defaults:
-            writer.default(default)
+
+        # Write all rules, even if some are not used.
+        writer.comment("All rules")
+        for name, rule in rules.items():
+            writer.rule(name=name, **rule)
+        writer.newline()
+
+        # Write all build lines and comments
+        for path in glob("**", recursive=True):
+            builds = []
+            for pattern in patterns:
+                builds.extend(pattern(path))
+            if len(builds) > 0:
+                writer.comment(path)
+                for build in builds:
+                    if isinstance(build, str):
+                        writer.comment(build)
+                    else:
+                        default = build.pop("default", False)
+                        check_tex_outputs(build.get("outputs", None))
+                        check_tex_outputs(build.get("implicit_outputs", None))
+                        writer.build(**build)
+                        if default:
+                            writer.default(build["outputs"])
+                writer.newline()
 
 
 DEFAULT_PATTERNS = [
     latex_pattern,
     latexdiff_pattern,
     dataset_pattern,
     svg_pattern,
```

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/articlezip.py` & `RepRepBuild-0.7.2/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/bibtex.py` & `RepRepBuild-0.7.2/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/latex.py` & `RepRepBuild-0.7.2/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/latexdep.py` & `RepRepBuild-0.7.2/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.7.2/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.7.2/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/repeat.py` & `RepRepBuild-0.7.2/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/utils.py` & `RepRepBuild-0.7.2/src/reprepbuild/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,19 @@
         f.write("\n")
 
 
 def import_python_path(path):
     """Return a module by importing a Python file at a given path."""
     spec = importlib.util.spec_from_file_location("<pythonscript>", path)
     module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
+    try:
+        spec.loader.exec_module(module)
+    except Exception as e:
+        # Ignore the script if it cannot be imported correctly.
+        return None
     return module
 
 
 def check_script_args(script_args):
     for script_arg in script_args:
         if isinstance(script_arg, str):
             if not re.match(r"^[a-zA-Z0-9_-]*$", script_arg):
```

### Comparing `RepRepBuild-0.7.1/src/reprepbuild/zip.py` & `RepRepBuild-0.7.2/src/reprepbuild/zip.py`

 * *Files identical despite different names*


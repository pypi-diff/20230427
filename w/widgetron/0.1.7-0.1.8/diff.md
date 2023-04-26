# Comparing `tmp/widgetron-0.1.7.tar.gz` & `tmp/widgetron-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgetron-0.1.7.tar", last modified: Fri Apr 14 17:06:40 2023, max compression
+gzip compressed data, was "widgetron-0.1.8.tar", last modified: Wed Apr 26 20:30:27 2023, max compression
```

## Comparing `widgetron-0.1.7.tar` & `widgetron-0.1.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 17:04:51.000000 widgetron-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 17:06:40.900309 widgetron-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-14 17:04:51.000000 widgetron-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 17:06:40.900309 widgetron-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 17:04:51.000000 widgetron-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.892310 widgetron-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/args.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.icns
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.ico
--rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.png
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/jinja_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.892310 widgetron-0.1.7/src/widgetron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/templates/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/constructor/construct.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/constructor/post_install.sh_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/electron/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/index.html_template
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/main.js_template
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/package.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/bld.bat_template
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/meta.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/widgetron_shortcut.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/setup.cfg_template
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/setup.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/__init__.py_template
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/cli.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 20:28:38.000000 widgetron-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 20:30:27.380339 widgetron-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-26 20:28:38.000000 widgetron-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-26 20:30:27.380339 widgetron-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 20:28:38.000000 widgetron-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/args.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.icns
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/jinja_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/constructor/construct.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/constructor/post_install.sh_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/electron/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/index.html_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/main.js_template
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/package.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/bld.bat_template
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/meta.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/widgetron_shortcut.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/setup.cfg_template
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/setup.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/__init__.py_template
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/cli.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/top_level.txt
```

### Comparing `widgetron-0.1.7/LICENSE` & `widgetron-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/PKG-INFO` & `widgetron-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgetron
-Version: 0.1.7
+Version: 0.1.8
 Summary: Application builder for ipython notebooks
 Author: Joel Stansbury
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: Markdown
 License-File: LICENSE
```

### Comparing `widgetron-0.1.7/README.md` & `widgetron-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/setup.cfg` & `widgetron-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/__main__.py` & `widgetron-0.1.8/src/widgetron/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import platform
 import re
 import shutil
 import sys
 import zipfile
 from pathlib import Path
-from subprocess import call
+from subprocess import check_call
 
 import yaml
 
 from .parse_args import CONFIG
 
 
 def zipdir(path, ziph):
@@ -84,25 +84,37 @@
             "sbom",
             "-t=CONDA",
             f"-f={kwargs['explicit_lock']}",
             "--output-format=json",
             f"-o={Path(kwargs['outdir'])/'conda-sbom.json'}"
         ]
         print(cmd)
-        call(cmd)
+        check_call(cmd)
     elif "environment_yaml" in kwargs:
         with open(kwargs["environment_yaml"], "r") as f:
             _env = yaml.safe_load(f)
         kwargs["dependencies"] += _env["dependencies"]
         kwargs["channels"] +=  _env["channels"]
 
     kwargs["server_command"] = kwargs.get("server_command", DEFAULT_SERVER_COMMAND)
     if isinstance(kwargs["server_command"], str):
         kwargs["server_command"]=kwargs["server_command"].strip().split()
 
+    # cli.py template requires executable and cli args to be separated.
+    if kwargs["server_command"][0] == "jupyter":  # "jupyter lab"
+        kwargs["server_executable"] = '-'.join(kwargs["server_command"][:2])
+        kwargs["server_command_args"] = kwargs["server_command"][2:]
+    elif 'jupyter-' in kwargs["server_command"][0]:  # "jupyter-lab"
+        kwargs["server_executable"] = kwargs["server_command"][0]
+        kwargs["server_command_args"] = kwargs["server_command"][1:]
+    else:
+        raise ValueError(
+            "server command did not follow expected syntax ('jupyter-cmd' or 'jupyter cmd')"
+        )
+
     kwargs["url_whitelist"] = kwargs.get("url_whitelist", [])
     if isinstance(kwargs["url_whitelist"], str):
         kwargs["url_whitelist"]=kwargs["url_whitelist"].strip().split()
 
     kwargs["domain_whitelist"] = kwargs.get("domain_whitelist", [])
     if isinstance(kwargs["domain_whitelist"], str):
         kwargs["domain_whitelist"]=kwargs["domain_whitelist"].strip().split()
@@ -167,24 +179,24 @@
     cwd = Path().absolute()
 
     os.chdir(str(kwargs["temp_files"] / "electron"))
     os.mkdir("build")
     # assert icon.suffix.lower() == ".png", "WIP: only png currently supported"
     shutil.copy(str(icon), f"build/icon{icon.suffix}")
 
-    call("npm install .", shell=True)
+    check_call("npm install .", shell=True)
     sbom = Path(kwargs['outdir']) / 'npm-sbom.json'
     cmd = [
         "npm", "run", "lock", "--",
         "--output-format", "json",
         "--output-file", f"{sbom}"
     ]
     print(cmd)
-    call(cmd, shell=True)
-    call(
+    check_call(cmd, shell=True)
+    check_call(
         "npm run build",
         shell=True,
     )
     if OSX or LINUX:
         dist = "dist"
     elif WIN:
         dist = "dist/win-unpacked"
@@ -210,20 +222,20 @@
     icon = Path(kwargs["icon"])
     shutil.copy(str(icon), kwargs["temp_files"] / f"recipe/{icon.name}")
     kwargs["icon"] = icon.name
 
 
 def build_conda_package(kwargs):
     dir = kwargs["temp_files"] / "recipe"
-    call(CONDA_BUILD.format(dir), shell=True)
+    check_call(CONDA_BUILD.format(dir), shell=True)
 
 
 def build_installer(kwargs):
     dir = kwargs["temp_files"] / "constructor"
-    call(f"constructor {dir} --output-dir {kwargs['outdir']}", shell=True)
+    check_call(f"constructor {dir} --output-dir {kwargs['outdir']}", shell=True)
 
 
 def cli():
     kwargs = parse_arguments()
 
     render_templates(**kwargs)
     package_electron_app(kwargs)
```

### Comparing `widgetron-0.1.7/src/widgetron/args.yml` & `widgetron-0.1.8/src/widgetron/args.yml`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/icons/widgetron.icns` & `widgetron-0.1.8/src/widgetron/icons/widgetron.icns`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/icons/widgetron.ico` & `widgetron-0.1.8/src/widgetron/icons/widgetron.ico`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/icons/widgetron.png` & `widgetron-0.1.8/src/widgetron/icons/widgetron.png`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/jinja_functions.py` & `widgetron-0.1.8/src/widgetron/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/parse_args.py` & `widgetron-0.1.8/src/widgetron/parse_args.py`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/templates/electron/main.js_template` & `widgetron-0.1.8/src/widgetron/templates/electron/main.js_template`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/templates/electron/package.json_template` & `widgetron-0.1.8/src/widgetron/templates/electron/package.json_template`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb` & `widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.7/src/widgetron.egg-info/PKG-INFO` & `widgetron-0.1.8/src/widgetron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgetron
-Version: 0.1.7
+Version: 0.1.8
 Summary: Application builder for ipython notebooks
 Author: Joel Stansbury
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: Markdown
 License-File: LICENSE
```

### Comparing `widgetron-0.1.7/src/widgetron.egg-info/SOURCES.txt` & `widgetron-0.1.8/src/widgetron.egg-info/SOURCES.txt`

 * *Files identical despite different names*


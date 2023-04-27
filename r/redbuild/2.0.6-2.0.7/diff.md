# Comparing `tmp/redbuild-2.0.6.tar.gz` & `tmp/redbuild-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.6.tar", max compression
+gzip compressed data, was "redbuild-2.0.7.tar", max compression
```

## Comparing `redbuild-2.0.6.tar` & `redbuild-2.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.6/LICENSE
--rw-r--r--   0        0        0     2408 2023-04-17 00:28:40.042586 redbuild-2.0.6/README.md
--rw-r--r--   0        0        0      604 2023-04-17 01:34:09.601405 redbuild-2.0.6/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.6/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.6/redbuild/__main__.py
--rw-r--r--   0        0        0     8906 2023-04-17 01:33:20.815068 redbuild-2.0.6/redbuild/cli.py
--rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.6/redbuild/engine.py
--rw-r--r--   0        0        0       41 2023-04-15 17:00:28.562653 redbuild-2.0.6/redbuild/models.py
--rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.6/redbuild/res.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.6/redbuild/util.py
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 redbuild-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.7/LICENSE
+-rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.0.7/README.md
+-rw-r--r--   0        0        0      604 2023-04-17 01:56:51.840957 redbuild-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.7/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.7/redbuild/__main__.py
+-rw-r--r--   0        0        0    10678 2023-04-17 01:56:34.767608 redbuild-2.0.7/redbuild/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.0.7/redbuild/composer.py
+-rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.7/redbuild/engine.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.7/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.7/redbuild/util.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.0.7/PKG-INFO
```

### Comparing `redbuild-2.0.6/LICENSE` & `redbuild-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.6/README.md` & `redbuild-2.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
 ## install stable version from pypi
 
 ```sh
+# with pipx (recommended)
+pipx install redbuild
+# with vanilla pip
 pip install redbuild
 ```
 
 ## build from source
 
 To build redbuild2, we will use the redbuild1 shell script to bootstrap the build environment and build redbuild2.
```

### Comparing `redbuild-2.0.6/pyproject.toml` & `redbuild-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.0.6"
+version = "2.0.7"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = {extras = ["rich"], version = "^0.7.0"}
```

### Comparing `redbuild-2.0.6/redbuild/cli.py` & `redbuild-2.0.7/redbuild/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from . import __version__
 from .engine import (
     ContainerEngine,
     detect_container_engine,
     get_container_engine_command,
 )
 from .util import get_builder_image_name, parse_secondary_args
-from .res import DEFAULT_BUILDENV_DOCKERFILE
+from .composer import BuildEnv, compose_dockerfile, DEFAULT_BUILDENV
 
 APP_NAME = "redbuild"
 app = typer.Typer(
     name=APP_NAME,
     help=f"{APP_NAME}: a tool for easy magic containerized builds",
     no_args_is_help=True,
 )
@@ -264,29 +264,80 @@
     ),
     cwd: str = typer.Option(
         ".", "--cwd", "-C", help="Directory to use as the build context"
     ),
     force: bool = typer.Option(
         False, "--force", "-f", help="Force initialization even if Dockerfile exists"
     ),
+    quiet: bool = typer.Option(
+        False, "--quiet", "-q", help="Suppress output and use default buildenv"
+    ),
+    wizard: bool = typer.Option(
+        False, "--wizard", "-w", help="Run interactive buildenv configuration wizard"
+    ),
 ):
     # first, ensure that no build environment already exists
     dockerfile_path = os.path.join(cwd, dockerfile)
     if os.path.exists(dockerfile_path) and not force:
         # logger.error(f"{dockerfile} already exists in {cwd}")
         print(
             f"Failed to initialize build environment dockerfile: [{dockerfile}] already exists in [{cwd}]."
         )
         raise typer.Exit(1)
 
-    # write out a default Dockerfile
+    # create the dockerfile
     with open(dockerfile_path, "w") as f:
-        f.write(DEFAULT_BUILDENV_DOCKERFILE)
-
-    print(f"Initialized build environment dockerfile: Created [{dockerfile_path}].")
+        buildenv = DEFAULT_BUILDENV
+        if wizard:
+            # buildenv configuration wizard
+            print("Interactive buildenv configuration:")
+
+            # 1. base image selection
+            custom_base_image = typer.prompt(
+                "  Base image",
+                default=buildenv.base_image,
+            )
+
+            # 2. package selection
+            custom_packages = (
+                typer.prompt(
+                    "  Packages",
+                    default=" ".join(buildenv.additional_packages),
+                )
+                .strip()
+                .replace(",", " ")
+                .split(" ")
+            )
+
+            # 3. additional steps (multi-line), terminated by empty line
+            custom_steps = []
+            print("  Additional steps (terminate with empty line):")
+            while True:
+                step = typer.prompt("    ", default="")
+                if step.strip() == "":
+                    break
+                custom_steps.append(step)
+
+            # apply the custom values
+            buildenv.base_image = custom_base_image
+            buildenv.additional_packages = custom_packages
+            buildenv.additional_setup = custom_steps
+        else:
+            # use default buildenv
+            pass
+
+        # write the buildenv contents to the dockerfile
+        f.write(compose_dockerfile(buildenv))
+
+    if not quiet:
+        print(f"Initialized build environment dockerfile: Created [{dockerfile_path}]:")
+        # print out the dockerfile
+        with open(dockerfile_path, "r") as f:
+            for line in f:
+                print(f"  {line}", end="")
 
 
 def version_callback(value: bool):
     if value:
         print(__version__)
         raise typer.Exit()
```

### Comparing `redbuild-2.0.6/redbuild/engine.py` & `redbuild-2.0.7/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.6/redbuild/util.py` & `redbuild-2.0.7/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.6/PKG-INFO` & `redbuild-2.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.6
+Version: 2.0.7
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,14 +29,17 @@
 redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
 ## install stable version from pypi
 
 ```sh
+# with pipx (recommended)
+pipx install redbuild
+# with vanilla pip
 pip install redbuild
 ```
 
 ## build from source
 
 To build redbuild2, we will use the redbuild1 shell script to bootstrap the build environment and build redbuild2.
```


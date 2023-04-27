# Comparing `tmp/cliffy-0.2.5.tar.gz` & `tmp/cliffy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.5.tar", max compression
+gzip compressed data, was "cliffy-0.2.6.tar", max compression
```

## Comparing `cliffy-0.2.5.tar` & `cliffy-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1060 2023-04-17 03:45:28.840986 cliffy-0.2.5/LICENSE
--rw-r--r--   0        0        0     5040 2023-04-17 03:45:28.840986 cliffy-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/__init__.py
--rw-r--r--   0        0        0     4429 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     4010 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      984 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1836 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     1395 2023-04-17 03:45:28.840986 cliffy-0.2.5/cliffy/helper.py
--rw-r--r--   0        0        0     3459 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/homer.py
--rw-r--r--   0        0        0     1354 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/loader.py
--rw-r--r--   0        0        0      297 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7130 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/merger.py
--rw-r--r--   0        0        0     5179 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/parser.py
--rw-r--r--   0        0        0       47 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/run.py
--rw-r--r--   0        0        0     2484 2023-04-17 03:45:28.844986 cliffy-0.2.5/cliffy/transformer.py
--rw-r--r--   0        0        0      919 2023-04-17 03:45:28.844986 cliffy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5866 1970-01-01 00:00:00.000000 cliffy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-27 06:27:19.860110 cliffy-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5214 2023-04-27 06:27:19.860110 cliffy-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/__init__.py
+-rw-r--r--   0        0        0     4429 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     4010 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1832 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     2603 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/helper.py
+-rw-r--r--   0        0        0     3459 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/homer.py
+-rw-r--r--   0        0        0     1354 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/loader.py
+-rw-r--r--   0        0        0      297 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7441 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/merger.py
+-rw-r--r--   0        0        0     5179 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/parser.py
+-rw-r--r--   0        0        0       47 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/run.py
+-rw-r--r--   0        0        0     3406 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/transformer.py
+-rw-r--r--   0        0        0      939 2023-04-27 06:27:19.860110 cliffy-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6080 1970-01-01 00:00:00.000000 cliffy-0.2.6/PKG-INFO
```

### Comparing `cliffy-0.2.5/LICENSE` & `cliffy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/README.md` & `cliffy-0.2.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 * Built-in shell and Python script support
 * Supports Jinja2-templating to create a flexible command flow
 
 ## Install
 `pip install cliffy`
 
 ## Usage
-* `cli init <cli name>`: Generate a template CLI manifest
-* `cli load <manifest>`: Add a new CLI based on the manifest
-* `cli render <manifest>`: Render the YAML manifest into executable code
-* `cli list/ls`: Ouput a list of loaded CLIs 
-* `cli update <cli name>`: Reloads a CLI
-* `cli disable <cli name>`: Disable a CLI
-* `cli enable <cli name>`: Enable a disabled CLI
-* `cli remove/rm <cli name>`: Remove a loaded CLI
+`cli <command>`
+* `init <cli name>`: Generate a template CLI manifest
+* `load <manifest>`: Add a new CLI based on the manifest
+* `render <manifest>`: Render the YAML manifest into executable code
+* `list` or `ls`: Ouput a list of loaded CLIs 
+* `update <cli name>`: Reloads a CLI
+* `disable <cli name>`: Disable a CLI
+* `enable <cli name>`: Enable a disabled CLI
+* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 
-### Example
+### Basic Example
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
 
@@ -40,14 +41,17 @@
 
 2. Load CLI
 ```
 $ cli load hello.yaml
 ```
 
 3. Run CLI directly
+
+`hello -h`
+
 ![hello-demo](docs/images/hello.png)
 
 For more examples, check [examples](examples/) directory.
 
 ## Manifest template
 Generated by `cli init`:
 ```yaml
@@ -59,17 +63,23 @@
 name: cliffy 
 
 # The version of the CLI
 # This should follow the standard semantic versioning format (e.g., 'MAJOR.MINOR.PATCH').
 version: 0.1.0
 
 # List of external CLI manifest paths to include into the main manifest
-# Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest and finally, deep merges the merged manifest with the main manifest.
+# Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest
+# and finally, deep merges the merged manifest with the main manifest.
 includes: []
 
+# List of Python dependencies required for the CLI
+# Validated on CLI load and update
+# Supports basic requirements specifier syntax.
+requires: []
+
 # A mapping defining manifest variables that can be referenced in any other blocks
 # Environments variables can be used in this section with ${some_env_var} for dynamic parsing
 # Supports jinja2 formatted expressions as values
 # Interpolate defined vars in other blocks jinja2-styled {{ var_name }}.
 vars:
     default_mood: happy
```

### Comparing `cliffy-0.2.5/cliffy/cli.py` & `cliffy-0.2.6/cliffy/cli.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/cliffy/commander.py` & `cliffy-0.2.6/cliffy/commander.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/cliffy/commanders/click.py` & `cliffy-0.2.6/cliffy/commanders/click.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 
 class ClickCommander(Commander):
     """Generates commands based on the command config"""
 
     def add_base_imports(self):
         self.cli = f"""## Generated {self.manifest.name} on {datetime.datetime.now()}
-import rich_click as click; import subprocess; CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help']);
+import rich_click as click
+import subprocess
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 """
 
     def add_base_cli(self):
         self.cli += f"""
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.version_option('{self.manifest.version}')
 def cli():
```

### Comparing `cliffy-0.2.5/cliffy/commanders/typer.py` & `cliffy-0.2.6/cliffy/commanders/typer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 
 class TyperCommander(Commander):
     """Generates commands based on the command config"""
 
     def add_base_imports(self):
         self.cli = f"""## Generated {self.manifest.name} on {datetime.datetime.now()}
-import typer; import subprocess; from typing import Optional;
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help']);
+import typer
+import subprocess
+from typing import Optional
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 """
 
     def add_base_cli(self) -> None:
         self.cli += """
 cli = typer.Typer(context_settings=CONTEXT_SETTINGS"""
 
         if self.manifest.cli_options:
```

### Comparing `cliffy-0.2.5/cliffy/homer.py` & `cliffy-0.2.6/cliffy/homer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/cliffy/loader.py` & `cliffy-0.2.6/cliffy/loader.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/cliffy/manifests/v1.py` & `cliffy-0.2.6/cliffy/manifests/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,23 @@
         description="The version of the CLI. "
         "This should follow the standard semantic versioning format (e.g., 'MAJOR.MINOR.PATCH')."
     )
     help: str = Field(
         "",
         description="A brief description of the CLI that is displayed when the user invokes the --help or -h option.",
     )
+    requires: list[str] = Field(
+        [],
+        description="List of Python dependencies required for the CLI. Validated on CLI load and update. "
+        "Supports basic requirements specifier syntax.",
+    )
     includes: list[str] = Field(
         [],
         description="List of external CLI manifest paths to include into the main manifest. "
-        "Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest "
+        "Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest. "
         "and finally, deep merges the merged manifest with the main manifest.",
     )
     vars: dict[str, str] = Field(
         {},
         description="A mapping defining manifest variables that can be referenced in any other blocks. "
         "Environments variables can be used in this section with ${some_env_var} for dynamic parsing. "
         "Supports jinja2 formatted expressions as values. "
@@ -88,14 +93,17 @@
 
 {cls.get_field_description('version', as_comment=True)}
 version: 0.1.0
 
 {cls.get_field_description('includes', as_comment=True)}
 includes: []
 
+{cls.get_field_description('requires', as_comment=True)}
+requires: []
+
 {cls.get_field_description('vars', as_comment=True)}
 vars:
     default_mood: happy
 
 {cls.get_field_description('imports', as_comment=True)}
 imports:
     - import os
@@ -182,14 +190,15 @@
 
     commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = {}
     imports: Union[str, list[str]] = []
     functions: list[str] = []
     args: dict[str, list] = {}
     types: dict[str, str] = {}
     cli_options: dict[str, str] = {}
+    requires: list[str]
 
 
 class CLIMetadata(BaseModel):
     """Metadata model"""
 
     cli_name: str
     runner_path: str
```

### Comparing `cliffy-0.2.5/cliffy/parser.py` & `cliffy-0.2.6/cliffy/parser.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.5/pyproject.toml` & `cliffy-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.2.5"
+version = "0.2.6"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
@@ -13,14 +13,15 @@
 pybash = "^0.2.3"
 pyyaml = "^6.0"
 typer = "^0.7.0"
 shellingham = "^1.5.0.post1"
 pydantic = "^1.10.6"
 deepmerge = "^1.1.0"
 jinja2 = "^3.1.2"
+packaging = "^23.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 autoflake = "^2.0.0"
```

### Comparing `cliffy-0.2.5/PKG-INFO` & `cliffy-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.2.5
+Version: 0.2.6
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pybash (>=0.2.3,<0.3.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
@@ -35,24 +36,25 @@
 * Built-in shell and Python script support
 * Supports Jinja2-templating to create a flexible command flow
 
 ## Install
 `pip install cliffy`
 
 ## Usage
-* `cli init <cli name>`: Generate a template CLI manifest
-* `cli load <manifest>`: Add a new CLI based on the manifest
-* `cli render <manifest>`: Render the YAML manifest into executable code
-* `cli list/ls`: Ouput a list of loaded CLIs 
-* `cli update <cli name>`: Reloads a CLI
-* `cli disable <cli name>`: Disable a CLI
-* `cli enable <cli name>`: Enable a disabled CLI
-* `cli remove/rm <cli name>`: Remove a loaded CLI
+`cli <command>`
+* `init <cli name>`: Generate a template CLI manifest
+* `load <manifest>`: Add a new CLI based on the manifest
+* `render <manifest>`: Render the YAML manifest into executable code
+* `list` or `ls`: Ouput a list of loaded CLIs 
+* `update <cli name>`: Reloads a CLI
+* `disable <cli name>`: Disable a CLI
+* `enable <cli name>`: Enable a disabled CLI
+* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 
-### Example
+### Basic Example
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
 
@@ -63,14 +65,17 @@
 
 2. Load CLI
 ```
 $ cli load hello.yaml
 ```
 
 3. Run CLI directly
+
+`hello -h`
+
 ![hello-demo](docs/images/hello.png)
 
 For more examples, check [examples](examples/) directory.
 
 ## Manifest template
 Generated by `cli init`:
 ```yaml
@@ -82,17 +87,23 @@
 name: cliffy 
 
 # The version of the CLI
 # This should follow the standard semantic versioning format (e.g., 'MAJOR.MINOR.PATCH').
 version: 0.1.0
 
 # List of external CLI manifest paths to include into the main manifest
-# Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest and finally, deep merges the merged manifest with the main manifest.
+# Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest
+# and finally, deep merges the merged manifest with the main manifest.
 includes: []
 
+# List of Python dependencies required for the CLI
+# Validated on CLI load and update
+# Supports basic requirements specifier syntax.
+requires: []
+
 # A mapping defining manifest variables that can be referenced in any other blocks
 # Environments variables can be used in this section with ${some_env_var} for dynamic parsing
 # Supports jinja2 formatted expressions as values
 # Interpolate defined vars in other blocks jinja2-styled {{ var_name }}.
 vars:
     default_mood: happy
```


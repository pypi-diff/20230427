# Comparing `tmp/benchling_cli-0.7.1a0.tar.gz` & `tmp/benchling_cli-0.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchling_cli-0.7.1a0.tar", max compression
+gzip compressed data, was "benchling_cli-0.8.0a0.tar", max compression
```

## Comparing `benchling_cli-0.7.1a0.tar` & `benchling_cli-0.8.0a0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/LICENSE
--rw-r--r--   0        0        0      237 2023-03-03 17:09:41.628237 benchling_cli-0.7.1a0/README.md
--rw-r--r--   0        0        0        0 2023-03-03 17:09:31.608501 benchling_cli-0.7.1a0/benchling_cli/__init__.py
--rw-r--r--   0        0        0       41 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-03-03 17:09:31.608501 benchling_cli-0.7.1a0/benchling_cli/apps/__init__.py
--rw-r--r--   0        0        0     2603 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/cli.py
--rw-r--r--   0        0        0        0 2023-03-03 17:09:31.608501 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/__init__.py
--rw-r--r--   0        0        0     2153 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/generate_dependencies_module.py
--rw-r--r--   0        0        0     4144 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/generate_models.py
--rw-r--r--   0        0        0     3630 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/helpers.py
--rw-r--r--   0        0        0    14501 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2
--rw-r--r--   0        0        0     2124 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2
--rw-r--r--   0        0        0     8395 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2
--rw-r--r--   0        0        0    13835 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2
--rw-r--r--   0        0        0      759 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/cli.py
--rw-r--r--   0        0        0       25 2023-03-03 17:07:29.251729 benchling_cli-0.7.1a0/benchling_cli/py.typed
--rw-r--r--   0        0        0     2316 2023-03-03 17:09:41.588238 benchling_cli-0.7.1a0/pyproject.toml
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 benchling_cli-0.7.1a0/setup.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 benchling_cli-0.7.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/LICENSE
+-rw-r--r--   0        0        0      237 2023-04-27 19:39:14.084632 benchling_cli-0.8.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 19:38:48.974339 benchling_cli-0.8.0a0/benchling_cli/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:38:49.004339 benchling_cli-0.8.0a0/benchling_cli/apps/__init__.py
+-rw-r--r--   0        0        0     2567 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/cli.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:38:49.004339 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/__init__.py
+-rw-r--r--   0        0        0     2257 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_dependencies_module.py
+-rw-r--r--   0        0        0     5465 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_models.py
+-rw-r--r--   0        0        0     4333 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/helpers.py
+-rw-r--r--   0        0        0    14459 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2
+-rw-r--r--   0        0        0     2124 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2
+-rw-r--r--   0        0        0     1167 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/enum_scalar_model.py.jinja2
+-rw-r--r--   0        0        0     8395 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2
+-rw-r--r--   0        0        0    13835 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2
+-rw-r--r--   0        0        0      759 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/cli.py
+-rw-r--r--   0        0        0       25 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/py.typed
+-rw-r--r--   0        0        0     2316 2023-04-27 19:39:14.024631 benchling_cli-0.8.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 benchling_cli-0.8.0a0/setup.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 benchling_cli-0.8.0a0/PKG-INFO
```

### Comparing `benchling_cli-0.7.1a0/LICENSE` & `benchling_cli-0.8.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/cli.py` & `benchling_cli-0.8.0a0/benchling_cli/apps/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,15 @@
         typer.echo(f"Overwriting existing dependency file {dependencies_file_path}")
     else:
         typer.echo(f"Creating new dependency file {dependencies_file_path}")
 
     with open(dependencies_file_path, "w") as f:
         f.write(generate_dependencies_module(manifest))
 
-    # Version is not currently part of the manifest model
-    optional_version = manifest.info.get("version", "")
+    optional_version = manifest.info.version if manifest.info.version else ""
 
     typer.secho(
         f"Success! Generated dependency file for {manifest.info.name} {optional_version} "
         f"at {dependencies_file_path}.",
         fg="green",
     )
```

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/generate_dependencies_module.py` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_dependencies_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     workflow_task_schema_output_from_dependency,
 )
 from jinja2 import Environment, PackageLoader
 
 from benchling_cli.apps.codegen.helpers import (
     dependency_to_pascal_case,
     dependency_to_snake_case,
+    is_manifest_scalar_dependency,
     is_secure_text_dependency,
     reformat_code_str,
 )
 
 
 def generate_dependencies_module(manifest: BenchlingAppManifest) -> str:
     env = Environment(
@@ -27,14 +28,15 @@
         trim_blocks=True,
         lstrip_blocks=True,
     )
     template = env.get_template("dependencies.py.jinja2")
     rendered_template = template.render(
         manifest=manifest,
         is_secure_text_dependency=is_secure_text_dependency,
+        is_manifest_scalar_dependency=is_manifest_scalar_dependency,
         dependency_to_pascal_case=dependency_to_pascal_case,
         dependency_to_snake_case=dependency_to_snake_case,
         field_definitions_from_dependency=field_definitions_from_dependency,
         element_definition_from_dependency=element_definition_from_dependency,
         options_from_dependency=options_from_dependency,
         scalar_type_from_config=scalar_type_from_config,
         workflow_task_schema_output_from_dependency=workflow_task_schema_output_from_dependency,
```

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/helpers.py` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import dataclass
 from keyword import iskeyword
 import re
-from typing import List, Optional, Union
+from typing import get_args, List, Optional, Union
 
 from autoflake import fix_code
 from benchling_api_client.v2.beta.models.base_manifest_config import BaseManifestConfig
 from benchling_api_client.v2.beta.models.dropdown_dependency import DropdownDependency
 from benchling_api_client.v2.beta.models.entity_schema_dependency import EntitySchemaDependency
 from benchling_api_client.v2.beta.models.field_definitions_manifest import FieldDefinitionsManifest
 from benchling_api_client.v2.beta.models.manifest_scalar_config import ManifestScalarConfig
 from benchling_api_client.v2.beta.models.resource_dependency import ResourceDependency
 from benchling_api_client.v2.beta.models.scalar_config_types import ScalarConfigTypes
 from benchling_api_client.v2.beta.models.schema_dependency import SchemaDependency
 from benchling_api_client.v2.beta.models.workflow_task_schema_dependency import WorkflowTaskSchemaDependency
-from benchling_api_client.v2.stable.extensions import NotPresentError
+from benchling_api_client.v2.stable.extensions import NotPresentError, UnknownType
 import black
 
 
 def reformat_code_str(code_str: str) -> str:
     # Use autoflake to remove unused model imports instead of trying to crawl the entire manifest and figure
     # out which ones are being used.
     code_str = fix_code(code_str, remove_all_unused_imports=True)
@@ -61,31 +61,43 @@
 
 
 def to_snake_case(string: str) -> str:
     return _make_valid_identifier("_".join([word.lower() for word in _clean_and_split(string)]))
 
 
 def dependency_to_pascal_case(dependency: DependencyType) -> str:
-    if not hasattr(dependency, "name"):
+    if isinstance(dependency, UnknownType) or not hasattr(dependency, "name"):
         raise UnnamedDependencyError(f"No name available for unknown dependency: {dependency}")
     return to_pascal_case(dependency.name)
 
 
 def dependency_to_snake_case(dependency: DependencyType) -> str:
-    if not hasattr(dependency, "name"):
+    if isinstance(dependency, UnknownType) or not hasattr(dependency, "name"):
         raise UnnamedDependencyError(f"No name available for unknown dependency: {dependency}")
     return to_snake_case(dependency.name)
 
 
 def is_secure_text_dependency(dependency: DependencyType) -> bool:
     return getattr(dependency, "type", None) == ScalarConfigTypes.SECURE_TEXT
 
 
+def is_manifest_scalar_dependency(dependency: DependencyType) -> bool:
+    # Python can't compare isinstance for Union types until Python 3.10 so just do this for now
+    # from: https://github.com/python/typing/discussions/1132#discussioncomment-2560441
+    return isinstance(dependency, get_args(ManifestScalarConfig))
+
+
 def field_type_from_field_definition(field: FieldDefinitionsManifest) -> Optional[str]:
     """Return a scalar definition from a manifest field. Defaults to parsing as text."""
     try:
         if hasattr(field, "type") and field.type:
             return field.type
     # We can't seem to handle this programmatically by checking isinstance() or field truthiness
     except NotPresentError:
         pass
     return None
+
+
+def to_enum_option(enum_value: Union[str, float, int]) -> str:
+    # make all uppercase, remove any symbols, and replace spaces with underscores
+    option_value = "_".join([word.upper() for word in _clean_and_split(str(enum_value))]).replace(".", "_")
+    return option_value
```

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 An instance `dependencies: Dependencies` can be used as follows:
 
 {% macro dependency_doc(dependency, parent="dependencies.") -%}
 {% if dependency.__class__.__name__ == "ManifestArrayConfig" %}
 for element in dependencies.{{ dependency_to_snake_case(dependency) }}:
     element.name
     {% for element in element_definition_from_dependency(dependency) %}{{ dependency_doc(element, parent="element.")|indent(4, True) }}{% endfor %}
-{% elif dependency.__class__.__name__ == "ManifestScalarConfig" %}
+{% elif is_manifest_scalar_dependency(dependency) %}
 {{ parent }}{{ dependency_to_snake_case(dependency) }}.value
 {% else %}
 {{ parent }}{{ dependency_to_snake_case(dependency) }}.id
     {% if field_definitions_from_dependency(dependency) %}
         {% for field in dependency.field_definitions %}
 {{ parent }}{{ dependency_to_snake_case(dependency) }}.fields.{{ dependency_to_snake_case(field) }}.name
         {% endfor %}
@@ -77,15 +77,15 @@
 
     @property
 {% if dependency.__class__.__name__ == "ManifestArrayConfig" %}
     def {{ dependency_to_snake_case(dependency) }}(self) -> Iterable[{{ dependency_to_pascal_case(dependency) }}Dependency]:
 {% else %}
     def {{ dependency_to_snake_case(dependency) }}(self) -> {{ dependency_to_pascal_case(dependency) }}Dependency:
 {% endif %}
-{% if dependency.__class__.__name__ == "ManifestScalarConfig" %}
+{% if is_manifest_scalar_dependency(dependency) %}
   {% if is_secure_text_dependency(dependency) %}
    {% set config_class_name = "SecureTextConfig" %}
   {% else %}
    {% set config_class_name = "ScalarConfig" %}
   {% endif %}
         parent_path = self.full_path() if isinstance(self, BaseConfigNode) else []
         path = parent_path + {{ inner_class_name }}.path
@@ -128,15 +128,15 @@
         {% endif %}
         assert isinstance(config_item, {{ expected_config_type }}), f"Expected {config_item} to be {{ expected_config_type }}"
         return {{ inner_class_name }}(self, config_item)
 {% endif %}
 {%- endmacro -%}
 
 {% macro dependency_class(dependency, parent_class="") -%}
-{% if dependency.__class__.__name__ == "ManifestScalarConfig" %}
+{% if is_manifest_scalar_dependency(dependency) %}
     {% if is_secure_text_dependency(dependency) %}
        {% set dependency_subclass_name = "SecureTextDependency" %}
        {% set required_mixin_name = "RequiredSecureTextDependencyMixin" %}
        {% set optional_mixin_name = "OptionalSecureTextDependencyMixin" %}
     {% else %}
        {% set dependency_subclass_name = "ScalarConfigItem" %}
        {% set scalar_type_instance = scalar_type_from_config(dependency) %}
```

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.7.1a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2` & `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.7.1a0/benchling_cli/cli.py` & `benchling_cli-0.8.0a0/benchling_cli/cli.py`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.7.1a0/pyproject.toml` & `benchling_cli-0.8.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "benchling-cli"
-version = "0.7.1a0"   # NOTE: This version number is ignored and does not correspond to releases (see README)
+version = "0.8.0a0"   # NOTE: This version number is ignored and does not correspond to releases (see README)
 description = "CLI for assistance in developing with the Benchling Platform."
 authors = ["Benchling Support <support@benchling.com>"]
 packages = [{include = "benchling_cli"}]
 include = [
     "LICENSE", "benchling_cli/py.typed"
 ]
 license = "Apache-2.0"
@@ -16,15 +16,15 @@
 testpaths = [
     "tests",
 ]
 
 [tool.poetry.dependencies]
 black = "^22.3.0"
 python = "^3.8"
-benchling_sdk = "^1.6.0"
+benchling_sdk = "^1.6.1"
 typer = "^0.6.1"
 Jinja2 = "^3.1.2"
 autoflake = "^1.7"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.10.1"
 pre-commit = "^2.6.0"
```

### Comparing `benchling_cli-0.7.1a0/setup.py` & `benchling_cli-0.8.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 package_data = \
 {'': ['*'], 'benchling_cli.apps.codegen': ['templates/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'autoflake>=1.7,<2.0',
- 'benchling_sdk>=1.6.0,<2.0.0',
+ 'benchling_sdk>=1.6.1,<2.0.0',
  'black>=22.3.0,<23.0.0',
  'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['benchling-cli = benchling_cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'benchling-cli',
-    'version': '0.7.1a0',
+    'version': '0.8.0a0',
     'description': 'CLI for assistance in developing with the Benchling Platform.',
     'long_description': 'Benchling CLI\n-------------\n\nA Python 3.8+ CLI for the [Benchling](https://www.benchling.com/) platform designed to assist in developing against the\nBenchling platform\n\nTo see all commands available in the CLI, use `benchling-cli --help`',
     'author': 'Benchling Support',
     'author_email': 'support@benchling.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `benchling_cli-0.7.1a0/PKG-INFO` & `benchling_cli-0.8.0a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: benchling-cli
-Version: 0.7.1a0
+Version: 0.8.0a0
 Summary: CLI for assistance in developing with the Benchling Platform.
 License: Apache-2.0
 Author: Benchling Support
 Author-email: support@benchling.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: autoflake (>=1.7,<2.0)
-Requires-Dist: benchling_sdk (>=1.6.0,<2.0.0)
+Requires-Dist: benchling_sdk (>=1.6.1,<2.0.0)
 Requires-Dist: black (>=22.3.0,<23.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Description-Content-Type: text/markdown
 
 Benchling CLI
 -------------
```


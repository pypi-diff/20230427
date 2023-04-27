# Comparing `tmp/kpops-1.1.1.tar.gz` & `tmp/kpops-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.1.1.tar", max compression
+gzip compressed data, was "kpops-1.1.2.tar", max compression
```

## Comparing `kpops-1.1.1.tar` & `kpops-1.1.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     1064 2023-04-17 08:26:24.653158 kpops-1.1.1/LICENSE
--rw-r--r--   0        0        0     2370 2023-04-17 08:26:24.653158 kpops-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/exception.py
--rw-r--r--   0        0        0    11186 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/main.py
--rw-r--r--   0        0        0     4226 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9371 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2161 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     2913 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8202 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      182 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5890 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1470 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      788 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      180 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9588 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6937 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     4552 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    11549 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     4546 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1553 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     1754 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     7401 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      402 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2244 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     4575 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3072 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    10755 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     4407 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      291 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1107 2023-04-17 08:26:24.661158 kpops-1.1.1/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1840 2023-04-17 08:26:43.429217 kpops-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.1/setup.py
--rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-27 14:18:20.378846 kpops-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2370 2023-04-27 14:18:20.378846 kpops-1.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-27 14:19:03.610898 kpops-1.1.2/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11739 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/main.py
+-rw-r--r--   0        0        0     4206 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1711 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     9357 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4373 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8202 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      182 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5890 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1851 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      788 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9588 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6937 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     8321 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     7457 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    16472 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6775 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3272 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0    11398 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1116 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2859 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9097 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     4080 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    10755 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     2589 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     5808 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      594 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     1189 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1892 2023-04-27 14:19:03.590898 kpops-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.2/setup.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.2/PKG-INFO
```

### Comparing `kpops-1.1.1/LICENSE` & `kpops-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/README.md` & `kpops-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/cli/custom_formatter.py` & `kpops-1.1.2/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/cli/main.py` & `kpops-1.1.2/kpops/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterator, Optional
 
 import typer
 
+from kpops import __version__
 from kpops.cli.custom_formatter import CustomFormatter
 from kpops.cli.pipeline_config import ENV_PREFIX, PipelineConfig
 from kpops.cli.registry import Registry
 from kpops.component_handlers import ComponentHandlers
 from kpops.component_handlers.kafka_connect.kafka_connect_handler import (
     KafkaConnectHandler,
 )
@@ -197,23 +198,26 @@
 def schema(
     scope: SchemaScope = typer.Argument(
         ...,
         show_default=False,
         help="""
         Scope of the generated schema
         \n\n\n
-        pipeline: Schema of PipelineComponents. Always includes the built-in kpops components. To include custom components, provide [COMPONENTS_MODULES].
+        pipeline: Schema of PipelineComponents. Includes the built-in kpops components by default. To include custom components, provide [COMPONENTS_MODULES].
         \n\n\n
         config: Schema of PipelineConfig.""",
     ),
     components_module: Optional[str] = COMPONENTS_MODULES,
+    include_stock_components: bool = typer.Option(
+        default=True, help="Include the built-in KPOps components."
+    ),
 ) -> None:
     match scope:
         case SchemaScope.PIPELINE:
-            gen_pipeline_schema(components_module)
+            gen_pipeline_schema(components_module, include_stock_components)
         case SchemaScope.CONFIG:
             gen_config_schema()
 
 
 @app.command(
     help="Enriches pipelines steps with defaults. The output is used as input for the deploy/destroy/... commands."
 )
@@ -341,9 +345,29 @@
     pipeline_steps = reverse_pipeline_steps(pipeline, steps)
     for component in pipeline_steps:
         log_action("Clean", component)
         component.destroy(dry_run)
         component.clean(dry_run)
 
 
+def version_callback(show_version: bool) -> None:
+    if show_version:
+        typer.echo(f"KPOps {__version__}")
+        raise typer.Exit()
+
+
+@app.callback()
+def main(
+    version: bool = typer.Option(
+        False,
+        "--version",
+        "-V",
+        help="Print KPOps version",
+        callback=version_callback,
+        is_eager=True,
+    ),
+):
+    ...
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `kpops-1.1.1/kpops/cli/pipeline_config.py` & `kpops-1.1.2/kpops/cli/pipeline_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 from kpops.component_handlers.helm_wrapper.model import HelmConfig, HelmDiffConfig
 from kpops.utils.yaml_loading import load_yaml_file
 
 ENV_PREFIX = "KPOPS_"
 
 
 class TopicNameConfig(BaseSettings):
-    """
-    Configures topic names.
-    """
+    """Configures topic names."""
 
     default_output_topic_name: str = Field(
         default="${pipeline_name}-${component_name}",
         description="Configures the value for the variable ${output_topic_name}",
     )
     default_error_topic_name: str = Field(
         default="${pipeline_name}-${component_name}-error",
         description="Configures the value for the variable ${error_topic_name}",
     )
 
 
 class PipelineConfig(BaseSettings):
-    """
-    Pipeline configuration unrelated to the components.
-    """
+    """Pipeline configuration unrelated to the components."""
 
     defaults_path: Path = Field(
         default=Path("."),
         example="defaults",
         description="The path to the folder containing the defaults.yaml file and the environment defaults files. "
         "Paths can either be absolute or relative to `config.yaml`",
     )
```

### Comparing `kpops-1.1.1/kpops/cli/registry.py` & `kpops-1.1.2/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/__init__.py` & `kpops-1.1.2/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,15 @@
         release_name: str,
         chart: str,
         dry_run: bool,
         namespace: str,
         values: dict,
         flags: HelmUpgradeInstallFlags = HelmUpgradeInstallFlags(),
     ) -> str:
-        """
-        Prepares and executes the helm upgrade install command
-        """
+        """Prepares and executes the `helm upgrade --install` command"""
         with tempfile.NamedTemporaryFile("w") as values_file:
             yaml.safe_dump(values, values_file)
 
             command = ["helm"]
             command.extend(
                 [
                     "upgrade",
```

### Comparing `kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         self.config: HelmDiffConfig = config
 
     @staticmethod
     def calculate_changes(
         current_release: Iterable[HelmTemplate],
         new_release: Iterable[HelmTemplate],
     ) -> Iterator[Change[dict]]:
-        """
-        Compare 2 releases and generate a Change object for each difference
+        """Compare 2 releases and generate a Change object for each difference
 
         :param current_release: Iterable containing HelmTemplate objects for the current release
         :type current_release: Iterable[HelmTemplate]
         :param new_release: Iterable containing HelmTemplate objects for the new release
         :type new_release: Iterable[HelmTemplate]
         :return: A Generator of Change objects for each difference between the two releases
         :rtype: Iterator[Change[dict]]
```

### Comparing `kpops-1.1.1/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.1.2/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.1.2/kpops/component_handlers/kafka_connect/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from enum import Enum
-from typing import Literal
+from typing import Any, Literal
 
 from pydantic import BaseConfig, BaseModel, Extra
+from typing_extensions import override
 
-from kpops.utils.pydantic import CamelCaseConfig
+from kpops.utils.docstring import describe_object
+from kpops.utils.pydantic import CamelCaseConfig, DescConfig
 
 
 class KafkaConnectorType(str, Enum):
     SINK = "sink"
     SOURCE = "source"
 
 
 class KafkaConnectConfig(BaseModel):
-    class Config(BaseConfig):
+    """Settings specific to Kafka Connectors"""
+
+    class Config(DescConfig):
         extra = Extra.allow
-        schema_extra = {"additionalProperties": {"type": "string"}}
+
+        @override
+        @staticmethod
+        def schema_extra(schema: dict[str, Any], model: type[BaseModel]) -> None:  # type: ignore[override]
+            schema["description"] = describe_object(model.__doc__)
+            schema["additionalProperties"] = {"type": "string"}
 
 
 class ConnectorTask(BaseModel):
     connector: str
     task: int
 
 
@@ -61,9 +70,10 @@
     connector_type: Literal["source", "sink"]
     config: KafkaConnectResetterConfig
     name_override: str
 
     class Config(CamelCaseConfig):
         pass
 
+    @override
     def dict(self, **_) -> dict:
         return super().dict(by_alias=True, exclude_none=True)
```

### Comparing `kpops-1.1.1/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.1.2/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.1.2/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/topic/handler.py` & `kpops-1.1.2/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/topic/model.py` & `kpops-1.1.2/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.1.2/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/topic/utils.py` & `kpops-1.1.2/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/component_handlers/utils/exception.py` & `kpops-1.1.2/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/components/base_components/kafka_connector.py` & `kpops-1.1.2/kpops/components/base_components/kafka_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,70 +23,112 @@
     KafkaConnectResetterConfig,
     KafkaConnectResetterValues,
 )
 from kpops.components.base_components.base_defaults_component import deduplicate
 from kpops.components.base_components.models.from_section import FromTopic
 from kpops.components.base_components.pipeline_component import PipelineComponent
 from kpops.utils.colorify import magentaify
+from kpops.utils.docstring import describe_attr, describe_object
 from kpops.utils.pydantic import CamelCaseConfig
 
 log = logging.getLogger("KafkaConnector")
 
 
 class KafkaConnector(PipelineComponent, ABC):
-    type: str = "kafka-connector"
+    """Base class for all Kafka connectors
+
+    Should only be used to set defaults
+
+    :param type: Component type, defaults to "kafka-connector"
+    :type type: str, optional
+    :param schema_type: Used for schema generation, same as :param:`type`,
+        defaults to "kafka-connector"
+    :type schema_type: Literal["kafka-connector"], optional
+    :param app: Application-specific settings
+    :type app: KafkaAppConfig
+    :param repo_config: Configuration of the Helm chart repo to be used for
+        deploying the component,
+        defaults to HelmRepoConfig(repository_name="bakdata-kafka-connect-resetter", url="https://bakdata.github.io/kafka-connect-resetter/")
+    :type repo_config: HelmRepoConfig, None, optional
+    :param namespace: Namespace in which the component shall be deployed
+    :type namespace: str
+    :param version: Helm chart version, defaults to "1.0.4"
+    :type version: str, optional
+    :param resetter_values: Overriding Kafka Connect Resetter Helm values. E.g. to override the Image Tag etc.,
+        defaults to dict
+    :type resetter_values: dict, optional
+    """
+
+    type: str = Field(default="kafka-connector", description="Component type")
     schema_type: Literal["kafka-connector"] = Field(  # type: ignore[assignment]
-        default="kafka-connector", exclude=True
+        default="kafka-connector",
+        title="Component type",
+        description=describe_object(__doc__),
+        exclude=True,
     )
-    app: KafkaConnectConfig
-
-    repo_config: HelmRepoConfig = HelmRepoConfig(
-        repository_name="bakdata-kafka-connect-resetter",
-        url="https://bakdata.github.io/kafka-connect-resetter/",
+    app: KafkaConnectConfig = Field(
+        default=...,
+        description=describe_attr("app", __doc__),
     )
-    namespace: str
-    version: str = "1.0.4"
+    repo_config: HelmRepoConfig = Field(
+        default=HelmRepoConfig(
+            repository_name="bakdata-kafka-connect-resetter",
+            url="https://bakdata.github.io/kafka-connect-resetter/",
+        ),
+        description=describe_attr("repo_config", __doc__),
+    )
+    namespace: str = Field(
+        default=...,
+        description=describe_attr("namespace", __doc__),
+    )
+    version = Field(default="1.0.4", description="Helm chart version")
     resetter_values: dict = Field(
         default_factory=dict,
-        description="Overriding Kafka Connect Resetter Helm values. E.g. to override the Image Tag etc.",
+        description=describe_attr("resetter_values", __doc__),
     )
 
     class Config(CamelCaseConfig):
         pass
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self.prepare_connector_config()
 
     @cached_property
     def helm(self) -> Helm:
+        """Helm object that contains component-specific config such as repo"""
         helm_repo_config = self.repo_config
         helm = Helm(self.config.helm_config)
         helm.add_repo(
             helm_repo_config.repository_name,
             helm_repo_config.url,
             helm_repo_config.repo_auth_flags,
         )
         return helm
 
     def _get_resetter_helm_chart(self) -> str:
+        """Get reseter Helm chart
+
+        :return: returns the component resetter's helm chart
+        :rtype: str
+        """
         return f"{self.repo_config.repository_name}/kafka-connect-resetter"
 
     @cached_property
     def helm_diff(self) -> HelmDiff:
+        """Helm diff object of last and current release of this component"""
         return HelmDiff(self.config.helm_diff_config)
 
     @property
     def kafka_connect_resetter_chart(self) -> str:
+        """Resetter chart for this component"""
         return f"{self.repo_config.repository_name}/kafka-connect-resetter"
 
     def prepare_connector_config(self) -> None:
-        """
-        Substitute component related variables in config
-        """
+        """Substitute component related variables in config"""
         substituted_config = self.substitute_component_variables(
             json.dumps(self.app.dict())
         )
         out: dict = json.loads(substituted_config)
         self.app = KafkaConnectConfig(**out)
 
     @override
@@ -124,22 +166,28 @@
         self,
         connector_name: str,
         connector_type: KafkaConnectorType,
         dry_run: bool,
         retain_clean_jobs: bool,
         **kwargs,
     ) -> None:
-        """
-        Cleans the connector from the cluster. At first, it deletes the previous cleanup job (connector resetter)
+        """Clean the connector from the cluster
+
+        At first, it deletes the previous cleanup job (connector resetter)
         to make sure that there is no running clean job in the cluster. Then it releases a cleanup job.
         If the retain_clean_jobs flag is set to false the cleanup job will be deleted.
+
         :param connector_name: Name of the connector
+        :type connector_name: str
         :param connector_type: Type of the connector (SINK or SOURCE)
+        :type connector_type: KafkaConnectorType
         :param dry_run: If the cleanup should be run in dry run mode or not
+        :type dry_run: bool
         :param retain_clean_jobs: If the cleanup job should be kept
+        :type retain_clean_jobs: bool
         :param kwargs: Other values for the KafkaConnectResetter
         """
         trimmed_name = self._get_kafka_resetter_release_name(connector_name)
 
         log.info(
             magentaify(
                 f"Connector Cleanup: uninstalling cleanup job Helm release from previous runs for {connector_name}"
@@ -163,27 +211,47 @@
             self.helm_diff.log_helm_diff(log, current_release, new_release)
 
         if not retain_clean_jobs:
             log.info(magentaify("Connector Cleanup: uninstall Kafka Resetter."))
             self.__uninstall_connect_resetter(trimmed_name, dry_run)
 
     def _get_kafka_resetter_release_name(self, connector_name: str) -> str:
+        """Get connector resetter's release name
+
+        :param connector_name: Name of the connector to be reset
+        :type connector_name: str
+        :return: The name of the resetter to be used
+        :rtype: str
+        """
         suffix = "-clean"
         clean_up_release_name = connector_name + suffix
         trimmed_name = trim_release_name(clean_up_release_name, suffix)
         return trimmed_name
 
     def __install_connect_resetter(
         self,
         release_name: str,
         connector_name: str,
         connector_type: KafkaConnectorType,
         dry_run: bool,
         **kwargs,
     ) -> str:
+        """Install connector resetter
+
+        :param release_name: Release name for the resetter
+        :type release_name: str
+        :param connector_name: Name of the connector-to-be-reset
+        :type connector_name: str
+        :param connector_type: Type of the connector
+        :type connector_type: KafkaConnectorType
+        :param dry_run: Whether to dry run the command
+        :type dry_run: bool
+        :return: The output of `helm upgrade --install`
+        :rtype: str
+        """
         return self.helm.upgrade_install(
             release_name=release_name,
             namespace=self.namespace,
             chart=self.kafka_connect_resetter_chart,
             dry_run=dry_run,
             flags=HelmUpgradeInstallFlags(
                 create_namespace=self.config.create_namespace,
@@ -200,41 +268,79 @@
 
     def _get_kafka_connect_resetter_values(
         self,
         connector_name: str,
         connector_type: KafkaConnectorType,
         **kwargs,
     ) -> dict:
+        """Get connector resetter helm chart values
+
+        :param connector_name: Name of the connector
+        :type connector_name: str
+        :param connector_type: Type of the connector
+        :type connector_type: KafkaConnectorType
+        :return: The Helm chart values of the connector resetter
+        :rtype: dict
+        """
         return {
             **KafkaConnectResetterValues(
                 config=KafkaConnectResetterConfig(
                     connector=connector_name,
                     brokers=self.config.broker,
                     **kwargs,
                 ),
                 connector_type=connector_type.value,
                 name_override=connector_name,
             ).dict(),
             **self.resetter_values,
         }
 
     def __uninstall_connect_resetter(self, release_name: str, dry_run: bool) -> None:
+        """Uninstall connector resetter
+
+        :param release_name: Name of the release to be uninstalled
+        :type release_name: str
+        :param dry_run: Whether to do a dry run of the command
+        :type dry_run: bool
+        """
         self.helm.uninstall(
             namespace=self.namespace,
             release_name=release_name,
             dry_run=dry_run,
         )
 
 
 class KafkaSourceConnector(KafkaConnector):
-    type: str = "kafka-source-connector"
+    """Kafka source connector model
+
+    :param type: Component type, defaults to "kafka-source-connector"
+    :type type: str, optional
+    :param schema_type: Used for schema generation, same as :param:`type`,
+        defaults to "kafka-source-connector"
+    :type schema_type: Literal["kafka-source-connector"], optional
+    :param offset_topic: offset.storage.topic,
+        more info: https://kafka.apache.org/documentation/#connect_running,
+        defaults to None
+    :type schema_type: str, None
+    """
+
+    type: str = Field(
+        default="kafka-source-connector",
+        description=describe_attr("type", __doc__),
+    )
     schema_type: Literal["kafka-source-connector"] = Field(  # type: ignore[assignment]
-        default="kafka-source-connector", exclude=True
+        default="kafka-source-connector",
+        title="Component type",
+        description=describe_object(__doc__),
+        exclude=True,
+    )
+    offset_topic: str | None = Field(
+        default=None,
+        description=describe_attr("offset_topic", __doc__),
     )
-    offset_topic: str | None = None
 
     @override
     def apply_from_inputs(self, name: str, topic: FromTopic) -> NoReturn:
         raise NotImplementedError("Kafka source connector doesn't support FromSection")
 
     @override
     def template(
@@ -260,27 +366,47 @@
 
     @override
     def clean(self, dry_run: bool) -> None:
         super().clean(dry_run)
         self.__run_kafka_connect_resetter(dry_run)
 
     def __run_kafka_connect_resetter(self, dry_run: bool) -> None:
+        """Runs the connector resetter
+
+        :param dry_run: Whether to do a dry run of the command
+        :type dry_run: bool
+        """
         self._run_connect_resetter(
             connector_name=self.name,
             connector_type=KafkaConnectorType.SOURCE,
             dry_run=dry_run,
             retain_clean_jobs=self.config.retain_clean_jobs,
             offset_topic=self.offset_topic,
         )
 
 
 class KafkaSinkConnector(KafkaConnector):
-    type: str = "kafka-sink-connector"
+    """Kafka sink connector model
+
+    :param type: Component type, defaults to "kafka-sink-connector"
+    :type type: str, optional
+    :param schema_type: Used for schema generation, same as :param:`type`,
+        defaults to "kafka-sink-connector"
+    :type schema_type: Literal["kafka-sink-connector"], optional
+    """
+
+    type: str = Field(
+        default="kafka-sink-connector",
+        description=describe_attr("type", __doc__),
+    )
     schema_type: Literal["kafka-sink-connector"] = Field(  # type: ignore[assignment]
-        default="kafka-sink-connector", exclude=True
+        default="kafka-sink-connector",
+        title="Component type",
+        description=describe_object(__doc__),
+        exclude=True,
     )
 
     @override
     def add_input_topics(self, topics: list[str]) -> None:
         existing_topics: str | None = getattr(self.app, "topics", None)
         topics = existing_topics.split(",") + topics if existing_topics else topics
         topics = deduplicate(topics)
@@ -318,14 +444,19 @@
     def clean(self, dry_run: bool) -> None:
         super().clean(dry_run)
         self.__run_kafka_connect_resetter(dry_run, delete_consumer_group=True)
 
     def __run_kafka_connect_resetter(
         self, dry_run: bool, delete_consumer_group: bool
     ) -> None:
+        """Runs the connector resetter
+
+        :param dry_run: Whether to do a dry run of the command
+        :type dry_run: bool
+        """
         self._run_connect_resetter(
             connector_name=self.name,
             connector_type=KafkaConnectorType.SINK,
             dry_run=dry_run,
             retain_clean_jobs=self.config.retain_clean_jobs,
             delete_consumer_group=delete_consumer_group,
         )
```

### Comparing `kpops-1.1.1/kpops/components/base_components/kubernetes_app.py` & `kpops-1.1.2/kpops/components/base_components/kubernetes_app.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,61 +13,102 @@
 from kpops.component_handlers.helm_wrapper.model import (
     HelmRepoConfig,
     HelmTemplateFlags,
     HelmUpgradeInstallFlags,
 )
 from kpops.components.base_components.pipeline_component import PipelineComponent
 from kpops.utils.colorify import magentaify
-from kpops.utils.pydantic import CamelCaseConfig
+from kpops.utils.docstring import describe_attr, describe_object
+from kpops.utils.pydantic import CamelCaseConfig, DescConfig
 
 log = logging.getLogger("KubernetesAppComponent")
 
 KUBERNETES_NAME_CHECK_PATTERN = re.compile(
     r"^(?![0-9]+$)(?!.*-$)(?!-)[a-z0-9-.]{1,253}(?<!_)$"
 )
 
 
 class KubernetesAppConfig(BaseModel):
-    class Config(CamelCaseConfig):
+    """Settings specific to Kubernetes Apps"""
+
+    class Config(CamelCaseConfig, DescConfig):
         extra = Extra.allow
 
 
 # TODO: label and annotations
 class KubernetesApp(PipelineComponent):
-    """Base Kubernetes app"""
+    """Base class for all Kubernetes apps.
+
+    All built-in components are Kubernetes apps, except for the Kafka connectors.
 
-    type: str = "kubernetes-app"
+    :param type: Component type, defaults to "kubernetes-app"
+    :type type: str, optional
+    :param schema_type: Used for schema generation, same as :param:`type`,
+        defaults to "kubernetes-app"
+    :type schema_type: Literal["kubernetes-app"], optional
+    :param app: Application-specific settings
+    :type app: KubernetesAppConfig
+    :param repo_config: Configuration of the Helm chart repo to be used for
+        deploying the component, defaults to None
+    :type repo_config: HelmRepoConfig, None, optional
+    :param namespace: Namespace in which the component shall be deployed
+    :type namespace: str
+    :param version: Helm chart version, defaults to None
+    :type version: str, None, optional
+    """
+
+    type: str = Field(
+        default="kubernetes-app",
+        description=describe_attr("type", __doc__),
+    )
     schema_type: Literal["kubernetes-app"] = Field(  # type: ignore[assignment]
-        default="kubernetes-app", exclude=True
+        default="kubernetes-app",
+        title="Component type",
+        description=describe_object(__doc__),
+        exclude=True,
+    )
+    app: KubernetesAppConfig = Field(
+        default=...,
+        description=describe_attr("app", __doc__),
+    )
+    repo_config: HelmRepoConfig | None = Field(
+        default=None,
+        description=describe_attr("repo_config", __doc__),
+    )
+    namespace: str = Field(
+        default=...,
+        description=describe_attr("namespace", __doc__),
+    )
+    version: str | None = Field(
+        default=None,
+        description=describe_attr("version", __doc__),
     )
-    app: KubernetesAppConfig
-    repo_config: HelmRepoConfig | None = None
-    namespace: str
-    version: str | None = None
 
-    class Config(CamelCaseConfig):
+    class Config(CamelCaseConfig, DescConfig):
         pass
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.__check_compatible_name()
 
     @cached_property
     def helm(self) -> Helm:
+        """Helm object that contains component-specific config such as repo"""
         helm = Helm(self.config.helm_config)
         if self.repo_config is not None:
             helm.add_repo(
                 self.repo_config.repository_name,
                 self.repo_config.url,
                 self.repo_config.repo_auth_flags,
             )
         return helm
 
     @cached_property
     def helm_diff(self) -> HelmDiff:
+        """Helm diff object of last and current release of this component"""
         return HelmDiff(self.config.helm_diff_config)
 
     @property
     def helm_release_name(self) -> str:
         """The name for the Helm release. Can be overridden."""
         return self.name
 
@@ -104,38 +145,55 @@
             dry_run,
         )
 
         if stdout:
             log.info(magentaify(stdout))
 
     def to_helm_values(self) -> dict:
+        """Generate a dictionary of values readable by Helm from `self.app`
+
+        :returns: Thte values to be used by Helm
+        :rtype: dict
+        """
         return self.app.dict(by_alias=True, exclude_none=True, exclude_unset=True)
 
     def print_helm_diff(self, stdout: str) -> None:
+        """Print the diff of the last and current release of this component
+
+        :param stdout: The output of a Helm command that installs or upgrades the release
+        :type stdout: str
+        """
         current_release = list(
             self.helm.get_manifest(self.helm_release_name, self.namespace)
         )
         if current_release:
             log.info(f"Helm release {self.helm_release_name} already exists")
         else:
             log.info(f"Helm release {self.helm_release_name} does not exist")
         new_release = Helm.load_manifest(stdout)
         self.helm_diff.log_helm_diff(log, current_release, new_release)
 
     def get_helm_chart(self) -> str:
+        """Return component's helm chart
+
+        :return: Helm chart of this component
+        :rtype: str
+        """
         raise NotImplementedError(
             f"Please implement the get_helm_chart() method of the {self.__module__} module."
         )
 
     def __check_compatible_name(self) -> None:
+        """Check if the component's name `self.name` is valid for Kubernetes"""
         if not bool(KUBERNETES_NAME_CHECK_PATTERN.match(self.name)):  # TODO: SMARTER
             raise ValueError(
                 f"The component name {self.name} is invalid for Kubernetes."
             )
 
+    @override
     def dict(self, *, exclude=None, **kwargs) -> dict[str, Any]:
         # HACK: workaround for Pydantic to exclude cached properties during model export
         if exclude is None:
             exclude = set()
         exclude.add("helm")
         exclude.add("helm_diff")
         return super().dict(exclude=exclude, **kwargs)
```

### Comparing `kpops-1.1.1/kpops/components/base_components/models/to_section.py` & `kpops-1.1.2/kpops/components/base_components/models/to_section.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,97 @@
 from enum import Enum
 from typing import Any
 
-from pydantic import BaseConfig, BaseModel, Extra, Field, root_validator
+from pydantic import BaseModel, Extra, Field, root_validator
+
+from kpops.utils.docstring import describe_attr
+from kpops.utils.pydantic import DescConfig
 
 
 class OutputTopicTypes(str, Enum):
-    """Types of output topic.
-    error (error topic), output (output topic), and extra topics. Every extra topic must have a role.
+    """Types of output topic
+
+    Error (error topic), output (output topic), and extra topics. Every extra topic must have a role.
     """
 
     ERROR = "error"
     OUTPUT = "output"
     EXTRA = "extra"
 
 
 class TopicConfig(BaseModel):
-    """Configures a topic"""
+    """Configure an output topic
+
+    :param type: Topic type
+    :type type: InputTopicTypes
+    :param key_schema: Key schema class name
+    :type key_schema: str | None
+    :param partitions_count: Number of partitions into which the topic is divided
+    :type partitions_count: int | None
+    :param replication_factor: Replication topic of the topic
+    :type replication_factor: int | None
+    :param configs: Topic configs
+    :type configs: dict[str, str | int]
+    :param role: Custom identifier belonging to one or multiple topics, provide only if `type` is `extra`
+    :type role: str | None
+    """
 
-    type: OutputTopicTypes = Field(...)
-    key_schema: str | None = Field(default=None, alias="keySchema")
-    value_schema: str | None = Field(default=None, alias="valueSchema")
-    partitions_count: int | None = None
-    replication_factor: int | None = None
-    configs: dict[str, str] = {}
-    role: str | None = None
+    type: OutputTopicTypes = Field(..., description="Topic type")
+    key_schema: str | None = Field(
+        default=None, alias="keySchema", description="Key schema class name"
+    )
+    value_schema: str | None = Field(
+        default=None, alias="valueSchema", description="Value schema class name"
+    )
+    partitions_count: int | None = Field(
+        default=None, description="Number of partitions into which the topic is divided"
+    )
+    replication_factor: int | None = Field(
+        default=None, description="Replication topic of the topic"
+    )
+    configs: dict[str, str | int] = Field(default={}, description="Topic configs")
+    role: str | None = Field(
+        default=None,
+        description="Custom identifier belonging to one or multiple topics, provide only if `type` is `extra`",
+    )
 
-    class Config(BaseConfig):
+    class Config(DescConfig):
         extra = Extra.forbid
         allow_population_by_field_name = True
         use_enum_values = True
 
     @root_validator
     def extra_topic_role(cls, values):
+        """Ensure that cls.role is used correctly"""
         is_extra_topic: bool = values["type"] == OutputTopicTypes.EXTRA
         if is_extra_topic and not values.get("role"):
             raise ValueError(
                 "If you define an extra output topic, you have to define a role."
             )
         if not is_extra_topic and values.get("role"):
             raise ValueError(
                 "If you do not define a output topic, the role is unnecessary. (This topic is either an output topic "
                 "without a role or an error topic)"
             )
         return values
 
 
 class ToSection(BaseModel):
-    models: dict[
-        str, Any
-    ] = (
-        {}
-    )  # any because snapshot versions must be supported  # TODO: really multiple models?
-    topics: dict[str, TopicConfig]
+    """Holds multiple output topics
+
+    :param models: Data models
+    :type models: dict[str, Any]
+    :param topics: Output topics
+    :type topics: dict[str, TopicConfig]
+    """
+
+    # TODO: really multiple models?
+    # any because snapshot versions must be supported
+    models: dict[str, Any] = Field(
+        default={}, description=describe_attr("models", __doc__)
+    )
+    topics: dict[str, TopicConfig] = Field(
+        ..., description=describe_attr("topics", __doc__)
+    )
 
-    class Config(BaseConfig):
+    class Config(DescConfig):
         extra = Extra.allow
```

### Comparing `kpops-1.1.1/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.1.2/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,40 +2,56 @@
 
 from typing import Literal
 
 from pydantic import BaseConfig, Extra, Field
 from typing_extensions import override
 
 from kpops.components.base_components.kafka_app import KafkaApp
-from kpops.components.base_components.models.from_section import FromSection
 from kpops.components.base_components.models.to_section import (
     OutputTopicTypes,
     TopicConfig,
 )
 from kpops.components.streams_bootstrap.app_type import AppType
 from kpops.components.streams_bootstrap.producer.model import ProducerValues
+from kpops.utils.docstring import describe_attr, describe_object
 
 
 class ProducerApp(KafkaApp):
-    """
-    Producer component
+    """Producer component
+
+    This producer holds configuration to use as values for the streams bootstrap
+    producer helm chart.
 
-    This producer holds configuration to use as values for the streams bootstrap produce helm chart.
+    :param type: Component type, defaults to "producer"
+    :type type: str, optional
+    :param schema_type: Used for schema generation, same as :param:`type`,
+        defaults to "producer"
+    :type schema_type: Literal["producer"], optional
+    :param app: Application-specific settings
+    :type app: ProducerValues
+    :param from_: Producer doesn't support FromSection, defaults to None
+    :type from_: None, optional
     """
 
-    type: str = "producer"
+    type: str = Field(default="producer", description="Component type")
     schema_type: Literal["producer"] = Field(  # type: ignore[assignment]
-        default="producer", exclude=True
+        default="producer",
+        title="Component type",
+        description=describe_object(__doc__),
+        exclude=True,
+    )
+    app: ProducerValues = Field(
+        default=...,
+        description=describe_attr("app", __doc__),
     )
-    app: ProducerValues
     from_: None = Field(
         default=None,
         alias="from",
         title="From",
-        description=f"Producer doesn't support {FromSection.__name__}",
+        description=describe_attr("from_", __doc__),
     )
 
     class Config(BaseConfig):
         extra = Extra.allow
 
     @override
     def apply_to_outputs(self, name: str, topic: TopicConfig) -> None:
```

### Comparing `kpops-1.1.1/kpops/pipeline_generator/pipeline.py` & `kpops-1.1.2/kpops/pipeline_generator/pipeline.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/utils/dict_differ.py` & `kpops-1.1.2/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.1/kpops/utils/yaml_loading.py` & `kpops-1.1.2/kpops/utils/yaml_loading.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,16 +19,19 @@
     file_path: Path, *, substitution: dict | None = None
 ) -> dict | list[dict]:
     with open(file_path) as yaml_file:
         return yaml.load(substitute(yaml_file.read(), substitution), Loader=yaml.Loader)
 
 
 def substitute(input: str, substitution: Mapping[str, Any] | None = None) -> str:
-    """
-    Substitute $-placeholders in input using template string.
+    """Substitute $-placeholders in input using template string.
+
     :param input: The raw input containing $-placeholders
+    :type input: str
     :param substitution: The key-value mapping containing substitutions
+    :type substitution: Mapping[str, Any] | None
     :return: Substituted input string
+    :rtype: str
     """
     if not substitution:
         return input
     return Template(input).safe_substitute(**substitution)
```

### Comparing `kpops-1.1.1/pyproject.toml` & `kpops-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.1.1"
+version = "1.1.2"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
@@ -44,23 +44,25 @@
 snapshottest = "^0.6.0"
 responses = "^0.22.0"
 pre-commit = "^2.19.0"
 mypy = "^0.990"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 isort = "^5.12.0"
+typer-cli = "^0.0.13"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-material = "^9.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material-extensions = "^1.1.1"
 mkdocs-glightbox = "^0.3.1"
 mike = "^1.1.2"
-typer-cli = "^0.0.13"
+
+[tool.poetry_bumpversion.file."kpops/__init__.py"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kpops-1.1.1/setup.py` & `kpops-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['kpops = kpops.cli.main:app']}
 
 setup_kwargs = {
     'name': 'kpops',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'KPOps is a tool to deploy Kafka pipelines to Kubernetes',
     'long_description': '# KPOps\n\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)\n[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)\n[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
     'author': 'bakdata',
     'author_email': 'opensource@bakdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/kpops',
```

### Comparing `kpops-1.1.1/PKG-INFO` & `kpops-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.1.1
+Version: 1.1.2
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
```


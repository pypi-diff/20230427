# Comparing `tmp/garden_ai-0.3.1.tar.gz` & `tmp/garden_ai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.3.1.tar", max compression
+gzip compressed data, was "garden_ai-0.4.0.tar", max compression
```

## Comparing `garden_ai-0.3.1.tar` & `garden_ai-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,32 @@
--rw-r--r--   0        0        0      797 2023-03-15 21:12:48.950873 garden_ai-0.3.1/README.md
--rw-r--r--   0        0        0      345 2023-03-15 21:12:48.950873 garden_ai-0.3.1/garden_ai/__init__.py
--rw-r--r--   0        0        0       51 2023-03-15 21:12:48.950873 garden_ai-0.3.1/garden_ai/__main__.py
--rw-r--r--   0        0        0        0 2023-03-15 21:12:48.950873 garden_ai-0.3.1/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     5212 2023-03-15 21:12:48.950873 garden_ai-0.3.1/garden_ai/app/garden.py
--rw-r--r--   0        0        0      484 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/app/main.py
--rw-r--r--   0        0        0     1653 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/app/model.py
--rw-r--r--   0        0        0     6352 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0    17790 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/client.py
--rw-r--r--   0        0        0     9398 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/datacite.py
--rw-r--r--   0        0        0     9416 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/mlflow_bandaid/__init__.py
--rw-r--r--   0        0        0     1064 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/mlflow_bandaid/binary_header_provider.py
--rw-r--r--   0        0        0     3885 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/mlmodel.py
--rw-r--r--   0        0        0     5137 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10527 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/steps.py
--rw-r--r--   0        0        0     1806 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/templates/pipeline
--rw-r--r--   0        0        0     6333 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/utils.py
--rw-r--r--   0        0        0      136 2023-03-15 21:12:48.954873 garden_ai-0.3.1/garden_ai/version.py
--rw-r--r--   0        0        0     1397 2023-03-15 21:12:58.230994 garden_ai-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 garden_ai-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-27 18:43:36.665809 garden_ai-0.4.0/LICENSE
+-rw-r--r--   0        0        0      797 2023-04-27 18:43:36.665809 garden_ai-0.4.0/README.md
+-rw-r--r--   0        0        0      391 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/console.py
+-rw-r--r--   0        0        0     9616 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      484 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/main.py
+-rw-r--r--   0        0        0     1881 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/model.py
+-rw-r--r--   0        0        0     7757 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0    15473 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/client.py
+-rw-r--r--   0        0        0     9398 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/datacite.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/funcx_bandaid/__init__.py
+-rw-r--r--   0        0        0     1247 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/funcx_bandaid/serialization_patch.py
+-rw-r--r--   0        0        0     9691 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2803 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1451 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      801 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0     6244 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/local_data.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/mlflow_bandaid/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/mlflow_bandaid/binary_header_provider.py
+-rw-r--r--   0        0        0     7053 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0    13740 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    11675 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/steps.py
+-rw-r--r--   0        0        0     2016 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     1160 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0    10634 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0      136 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/version.py
+-rw-r--r--   0        0        0     2429 2023-04-27 18:43:53.589881 garden_ai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 garden_ai-0.4.0/PKG-INFO
```

### Comparing `garden_ai-0.3.1/README.md` & `garden_ai-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.3.1/garden_ai/app/model.py` & `garden_ai-0.4.0/garden_ai/app/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,40 +21,45 @@
 def register(
     name: str = typer.Argument(
         ...,
         help=("The name of your model"),
     ),
     model_path: Path = typer.Argument(
         ...,
-        dir_okay=False,
+        exists=True,
+        dir_okay=True,
         file_okay=True,
         writable=True,
         readable=True,
         resolve_path=True,
         help=("The path to your model on your filesystem"),
     ),
     flavor: str = typer.Argument(
         "sklearn",
         help=(
             "What ML library did you make the model with? "
-            "Currently we just support sklearn."
+            "Currently we support the following flavors 'sklearn', 'tensorflow', and 'pytorch'."
         ),
     ),
     extra_pip_requirements: Optional[List[str]] = typer.Option(
         None,
         "--extra-pip-requirements",
         "-r",
         help=(
             "Additonal package requirmeents. Add multiple like "
-            '--extra_pip_requirements "torch=1.3.1" --extra_pip_requirements "pandas<=1.5.0"'
+            '--extra-pip-requirements "torch=1.3.1" --extra-pip-requirements "pandas<=1.5.0"'
         ),
     ),
 ):
     """Register a model in Garden. Outputs a full model identifier that you can reference in a Pipeline."""
-    if flavor != "sklearn":
-        rich.print("Sorry jk, we only support sklearn.")
+    if flavor not in ["sklearn", "tensorflow", "pytorch"]:
+        raise typer.BadParameter(
+            f"Sorry, we only support 'sklearn', 'tensorflow', and 'pytorch'. The {flavor} flavor is not yet supported."
+        )
 
     client = GardenClient()
-    full_model_name = client.log_model(str(model_path), name, extra_pip_requirements)
+    full_model_name = client.log_model(
+        str(model_path), name, flavor, extra_pip_requirements
+    )
     rich.print(
         f"Successfully uploaded your model! The full name to include in your pipeline is '{full_model_name}'"
     )
```

### Comparing `garden_ai-0.3.1/garden_ai/app/pipeline.py` & `garden_ai-0.4.0/garden_ai/app/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 import re
 from datetime import datetime
 from keyword import iskeyword
 from pathlib import Path
 from typing import List, Optional
 
 import jinja2
-import rich
 import typer
-from garden_ai import GardenClient, Pipeline, step
 from rich import print
 from rich.prompt import Prompt
 
+from garden_ai import GardenClient, Pipeline, step
+from garden_ai.app.console import console
+
+from garden_ai.utils.filesystem import (
+    load_pipeline_from_python_file,
+    PipelineLoadException,
+)
+
 logger = logging.getLogger()
 
 pipeline_app = typer.Typer(name="pipeline", no_args_is_help=True)
 
 
 def clean_identifier(name: str) -> str:
     """Clean the name provided for use as a pipeline's python identifier."""
@@ -195,15 +201,49 @@
         raise typer.Exit(code=1)
     else:
         out_dir.mkdir(parents=True)
         out_file = out_dir / "pipeline.py"
         contents = template_pipeline(shortname, pipeline)
         with open(out_file, "w") as f:
             f.write(contents)
-        print(f"Wrote to {out_file}.")
+        with open(out_dir / "requirements.txt", "w") as f:
+            f.write("## Please specify all pipeline dependencies here\n")
 
-    if verbose:
-        client.put_local_pipeline(pipeline)
-        metadata = client.get_local_pipeline(pipeline.uuid)
-        rich.print_json(metadata)
+        print(f"Generated pipeline scaffolding in {out_dir}.")
 
     return
+
+
+@pipeline_app.command(no_args_is_help=True)
+def register(
+    pipeline_file: Path = typer.Argument(
+        None,
+        dir_okay=False,
+        file_okay=True,
+        resolve_path=True,
+        help=("Path to a Python file containing your pipeline implementation."),
+    ),
+):
+    client = GardenClient()
+    if (
+        not pipeline_file.exists()
+        or not pipeline_file.is_file()
+        or pipeline_file.suffix != ".py"
+    ):
+        console.log(
+            f"{pipeline_file} is not a valid Python file. Please provide a valid Python file (.py)."
+        )
+        raise typer.Exit(code=1)
+    try:
+        user_pipeline = load_pipeline_from_python_file(pipeline_file)
+    except PipelineLoadException as e:
+        console.log(f"Could not parse {pipeline_file} as a Garden pipeline. " + str(e))
+        raise typer.Exit(code=1) from e
+
+    with console.status(
+        "[bold green]Building container. This operation times out after 30 minutes."
+    ):
+        container_uuid = client.build_container(user_pipeline)
+    console.print(f"Created container {container_uuid}")
+    func_uuid = client.register_pipeline(user_pipeline, container_uuid)
+    console.print(f"Created function {func_uuid}")
+    console.print("Done! Pipeline is registered.")
```

### Comparing `garden_ai-0.3.1/garden_ai/client.py` & `garden_ai-0.4.0/garden_ai/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,54 @@
+# mypy: disable-error-code="import"
 import json
 import logging
 import os
 import time
 from pathlib import Path
-from typing import Dict, List, Union, Optional
+from typing import List, Optional, Union
 from uuid import UUID
 
 import requests
 import typer
+from globus_compute_sdk import Client
 from globus_sdk import (
     AuthAPIError,
     AuthClient,
     GroupsClient,
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
 )
-from globus_sdk.scopes import ScopeBuilder
+from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
-from pydantic import ValidationError
+from mlflow.tracking.request_header.registry import _request_header_provider_registry
 from rich import print
 from rich.prompt import Prompt
 
-from garden_ai.gardens import Garden
-from garden_ai.pipelines import Pipeline
-from garden_ai.utils import JSON, extract_email_from_globus_jwt
-from garden_ai.mlmodel import upload_model
-
+import garden_ai.funcx_bandaid.serialization_patch  # type: ignore # noqa: F401
+from garden_ai import local_data
+from garden_ai.gardens import Garden, PipelineNotFoundException
+from garden_ai.globus_compute.containers import build_container
+from garden_ai.globus_compute.login_manager import ComputeLoginManager
+from garden_ai.globus_compute.remote_functions import register_pipeline
 from garden_ai.mlflow_bandaid.binary_header_provider import (
     BinaryContentTypeHeaderProvider,
 )
-from mlflow.tracking.request_header.registry import _request_header_provider_registry  # type: ignore
+from garden_ai.mlmodel import upload_model
+from garden_ai.pipelines import Pipeline, RegisteredPipeline
+from garden_ai.utils.misc import extract_email_from_globus_jwt
 
 # garden-dev index
 GARDEN_INDEX_UUID = "58e4df29-4492-4e7d-9317-b27eba62a911"
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
 
-LOCAL_STORAGE = Path("~/.garden").expanduser()
-LOCAL_STORAGE.mkdir(parents=True, exist_ok=True)
+COMPUTE_RESOURCE_SERVER_NAME = "funcx_service"
 
 logger = logging.getLogger()
 
 
 class AuthException(Exception):
     pass
 
@@ -80,45 +84,60 @@
         self.client_id = os.environ.get(
             "GARDEN_CLIENT_ID", "cf9f8938-fb72-439c-a70b-85addf1b8539"
         )
 
         self.auth_client = (
             NativeAppAuthClient(self.client_id) if not auth_client else auth_client
         )
-
+        self.openid_authorizer = self._create_authorizer(
+            AuthClient.scopes.resource_server
+        )
         self.groups_authorizer = self._create_authorizer(
             GroupsClient.scopes.resource_server
         )
         self.search_authorizer = self._create_authorizer(
             SearchClient.scopes.resource_server
         )
+        self.compute_authorizer = self._create_authorizer(COMPUTE_RESOURCE_SERVER_NAME)
         self.search_client = (
             SearchClient(authorizer=self.search_authorizer)
             if not search_client
             else search_client
         )
         self.garden_authorizer = self._create_authorizer(
             GardenClient.scopes.resource_server
         )
 
+        self.compute_client = self._make_compute_client()
         self._set_up_mlflow_env()
 
     def _set_up_mlflow_env(self):
         os.environ["MLFLOW_TRACKING_TOKEN"] = self.garden_authorizer.access_token
         os.environ["MLFLOW_TRACKING_URI"] = GARDEN_ENDPOINT + "/mlflow"
         _request_header_provider_registry.register(BinaryContentTypeHeaderProvider)
 
+    def _make_compute_client(self):
+        scope_to_authorizer = {
+            AuthScopes.openid: self.openid_authorizer,
+            SearchScopes.all: self.search_authorizer,
+            Client.FUNCX_SCOPE: self.compute_authorizer,
+        }
+        compute_login_manager = ComputeLoginManager(scope_to_authorizer)
+        return Client(login_manager=compute_login_manager, do_version_check=False)
+
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
                 AuthClient.scopes.openid,
                 AuthClient.scopes.email,
                 GroupsClient.scopes.view_my_groups_and_memberships,
                 SearchClient.scopes.ingest,
+                SearchClient.scopes.search,
                 GardenClient.scopes.action_all,
+                Client.FUNCX_SCOPE,
             ],
             refresh_tokens=True,
         )
         authorize_url = self.auth_client.oauth2_get_authorize_url()
 
         print(
             f"Authenticating with Globus in your default web browser: \n\n{authorize_url}"
@@ -144,15 +163,15 @@
                 raise AuthException
 
             # now store the tokens and pull out the Groups tokens
             self.auth_key_store.store(response)
             tokens = response.by_resource_server[resource_server]
 
             email = extract_email_from_globus_jwt(response.data["id_token"])
-            self._store_user_email(email)
+            local_data._store_user_email(email)
         else:
             # otherwise, we already did login; load the tokens from that file
             tokens = self.auth_key_store.get_token_data(resource_server)
         # construct the RefreshTokenAuthorizer which writes back to storage on refresh
         authorizer = RefreshTokenAuthorizer(
             tokens["refresh_token"],
             self.auth_client,
@@ -213,27 +232,50 @@
         if title:
             data["title"] = title
         return Garden(**data)
 
     def create_pipeline(
         self, authors: Optional[List[str]] = None, title: Optional[str] = None, **kwargs
     ) -> Pipeline:
+        """Initialize and return a pipeline object.
+
+        If this pipeline's UUID has been used before to register a function for
+        remote execution, reuse the (funcx/globus compute) ID for consistency.
+
+        NOTE: this means that local modifications to a pipeline will not be
+        reflected when executing remotely until the pipeline is re-registered.
+        """
         data = dict(kwargs)
         if authors:
             data["authors"] = authors
         if title:
             data["title"] = title
-        return Pipeline(**data)
+
+        pipeline = Pipeline(**data)
+        record = local_data.get_local_pipeline_by_uuid(pipeline.uuid)
+        if record:
+            logger.info("Found pre-registered pipeline. Reusing DOI.")
+            pipeline.doi = record.doi
+
+        return pipeline
 
     def log_model(
-        self, model_path: str, model_name: str, extra_pip_requirements: List[str] = None
+        self,
+        model_path: str,
+        model_name: str,
+        flavor: str,
+        extra_pip_requirements: List[str] = None,
     ) -> str:
-        email = self._get_user_email()
+        email = local_data._get_user_email()
         full_model_name = upload_model(
-            model_path, model_name, email, extra_pip_requirements=extra_pip_requirements
+            model_path,
+            model_name,
+            email,
+            flavor,
+            extra_pip_requirements=extra_pip_requirements,
         )
         return full_model_name
 
     def _mint_doi(
         self, obj: Union[Garden, Pipeline], force: bool = False, test: bool = True
     ) -> str:
         """Register a new "findable" doi with DataCite via Garden backend.
@@ -254,21 +296,35 @@
 
         Raises
         ------
         NotImplementedError
             see `test`
 
         """
+
         if not test:
             raise NotImplementedError
-        elif obj.doi and not force:
+
+        def get_existing_doi() -> Optional[str]:
+            # check for existing doi, either on object or in db
+            registered_obj: Optional[Union[Garden, RegisteredPipeline]]
+            if isinstance(obj, Garden):
+                registered_obj = local_data.get_local_garden_by_uuid(obj.uuid)
+            else:
+                registered_obj = local_data.get_local_pipeline_by_uuid(obj.uuid)
+
+            return registered_obj.doi if registered_obj else None
+
+        existing_doi = obj.doi or get_existing_doi()
+
+        if existing_doi and not force:
             logger.info(
                 "existing DOI found, not requesting new DOI. Pass `force=true` to override this behavior."
             )
-            return obj.doi
+            return existing_doi
 
         logger.info("Requesting DOI")
         url = f"{GARDEN_ENDPOINT}/doi"
 
         header = {
             "Content-Type": "application/vnd.api+json",
             "Authorization": self.garden_authorizer.get_authorization_header(),
@@ -286,218 +342,85 @@
             doi = r.json()["doi"]
         except requests.HTTPError:
             logger.error(f"{r.text}")
             raise
         else:
             return doi
 
-    def register_metadata(self, garden: Garden, out_dir=None):
-        """
-        NOTE: this is mostly vestigial until we're at the point of implementing
-        ``$ garden-ai {garden, pipeline, model(?)} register`` and know what should be
-        here instead.
-
-        Make a `Garden` object's metadata (and any pipelines' metadata)
-        discoverable; mint DOIs via DataCite.
-
-        This will perform validation on the metadata fields and (if successful)
-        write all of the Garden's (including its pipelines) metadata to a
-        `"metadata.json"` file.
+    def build_container(self, pipeline: Pipeline) -> str:
+        built_container_uuid = build_container(self.compute_client, pipeline)
+        return built_container_uuid
+
+    def register_pipeline(self, pipeline: Pipeline, container_uuid: str) -> str:
+        func_uuid = register_pipeline(self.compute_client, pipeline, container_uuid)
+        pipeline.func_uuid = UUID(func_uuid)
+        pipeline.doi = self._mint_doi(pipeline)
+        registered = RegisteredPipeline.from_pipeline(pipeline)
+        local_data.put_local_pipeline(registered)
+        return func_uuid
+
+    def get_registered_pipeline(
+        self, identifier: Union[UUID, str]
+    ) -> RegisteredPipeline:
+        """Return a callable ``RegisteredPipeline`` corresponding to the given uuid/doi.
 
         Parameters
         ----------
-        garden : Garden
-            A Garden object with user's ready-to-publish metadata. See `Garden`
-            docstring for explanation of fields.
-
-        out_dir : Union[PathLike, str]
-            Directory in which a copy of the Garden's metadata is written on
-            successful registration. Defaults to current working directory.
-
-        Raises
-        ------
-        ValidationError
-
-        """
-        out_dir = Path(out_dir) if out_dir else Path.cwd()
-        try:
-            for p in garden.pipelines:
-                p.doi = self._mint_doi(p)
-            garden.doi = self._mint_doi(garden)
-            garden.validate()
-        except ValidationError as e:
-            logger.error(e)
-            raise
-        else:
-            with open(out_dir / f"{garden.uuid}.json", "w+") as f:
-                f.write(garden.json())
-
-    def _read_local_db(self) -> Dict:
-        """Helper: load JSON contents of local storage and return as a dict."""
-        data = {}
-        # read existing entries into memory, if any
-        if (LOCAL_STORAGE / "data.json").exists():
-            with open(LOCAL_STORAGE / "data.json", "r+") as f:
-                raw_data = f.read()
-                if raw_data:
-                    data = json.loads(raw_data)
-        return data
-
-    def _write_local_db(self, data: Dict) -> None:
-        """Helper: JSON-serialize and write ``contents`` to ~/.garden/data.json."""
-        contents = json.dumps(data)
-        with open(LOCAL_STORAGE / "data.json", "w+") as f:
-            f.write(contents)
-        return
-
-    def _store_user_email(self, email: str) -> None:
-        data = self._read_local_db()
-        data["user_email"] = email
-        self._write_local_db(data)
-
-    def _get_user_email(self) -> str:
-        data = self._read_local_db()
-        maybe_email = data.get("user_email")
-        return str(maybe_email) if maybe_email else "unknown"
-
-    def put_local_garden(self, garden: Garden) -> None:
-        """Helper: write a record to 'local database' for a given Garden
-
-        Overwrites any existing entry with the same uuid in ~/.garden/data.json.
-
-        Parameters
-        ----------
-        garden : Garden
-            The object to json-serialize and write/update in the local database.
-            a TypeError will be raised if not a Garden.
-
-        """
-        if not isinstance(garden, Garden):
-            raise TypeError(f"Expected Garden object, got: {type(garden)}.")
-        data = self._read_local_db()
-
-        key, val = str(garden.uuid), json.loads(garden.json())
-        local_gardens = data.get("gardens", {})
-        local_gardens[key] = val
-        data["gardens"] = local_gardens
-
-        self._write_local_db(data)
-        return
-
-    def get_local_garden(self, uuid: Union[UUID, str]) -> Optional[JSON]:
-        """Helper: fetch a record from 'local database'
-
-        Find entry with key matching ``uuid`` and return the associated metadata
-        extracted from ``~/.garden/db/data.json``
-
-        Parameters
-        ----------
-        uuid : UUID
-            The uuid corresponding to the desired Garden or Pipeline.
+        identifier : Union[UUID, str]
+            The previously registered pipeline's DOI or UUID. Raises an
+            exception if not found.
 
         Returns
         -------
-        Optional[JSON]
-            If successful, the JSON string corresponding to the metadata of the
-            object with the given uuid.
-        """
-        data = self._read_local_db()
-
-        uuid = str(uuid)
-        local_gardens = data.get("gardens", {})
-        if local_gardens and uuid in local_gardens:
-            return json.dumps(local_gardens[uuid])
-        else:
-            logger.error(f"No garden found locally with uuid: {uuid}.")
-            return None
-
-    def put_local_pipeline(self, pipeline: Pipeline) -> None:
-        """Helper: write a record to 'local database' for a given Pipeline.
-
-        Overwrites any existing entry with the same ``uuid``.
-
-        Parameters
-        ----------
-        pipeline : Pipeline
-            The object to json-serialize and write/update in the local database.
-            a TypeError will be raised if not a Pipeline.
+        RegisteredPipeline
+            Instance of ``RegisteredPipeline``, which can be run on
+            a specified remote Globus Compute endpoint (and knows how to
+            set the appropriate MLFlow environment variables).
 
+        Raises
+        ------
+        PipelineNotFoundException
+            Raised when no known pipeline exists with the given identifier.
         """
-        if not isinstance(pipeline, Pipeline):
-            raise TypeError(f"Expected pipeline object, got: {type(pipeline)}.")
-        data = {}
-        # read existing entries into memory, if any
-        if (LOCAL_STORAGE / "data.json").exists():
-            with open(LOCAL_STORAGE / "data.json", "r+") as f:
-                raw_data = f.read()
-                if raw_data:
-                    data = json.loads(raw_data)
-
-        # update data['pipelines'], leaving data['gardens'] etc unmodified
-        pipelines = data.get("pipelines", {})
-        key, val = str(pipeline.uuid), pipeline.json()
-        pipelines[key] = json.loads(val)
-        data["pipelines"] = pipelines
-        contents = json.dumps(data)
-
-        with open(LOCAL_STORAGE / "data.json", "w+") as f:
-            f.write(contents)
-        return
-
-    def get_local_pipeline(self, uuid: Union[UUID, str]) -> Optional[JSON]:
-        """Helper: fetch a pipeline record from 'local database', if one exists.
-
-        Find entry with key matching ``uuid`` and return the associated metadata
-        extracted from ``~/.garden/db/data.json``
+        is_doi = "/" in str(identifier)
+        if is_doi:
+            registered = local_data.get_local_pipeline_by_doi(str(identifier))
+        else:
+            registered = local_data.get_local_pipeline_by_uuid(identifier)
 
-        Parameters
-        ----------
-        uuid : UUID
-            The uuid corresponding to the desired Pipeline.
+        if registered is None:
+            raise PipelineNotFoundException(
+                f"Could not find any pipelines with identifier {identifier}."
+            )
 
-        Returns
-        -------
-        Optional[JSON]
-            If successful, the JSON string corresponding to the metadata of the
-            object with the given uuid.
-        """
-        uuid = str(uuid)
-        with open(LOCAL_STORAGE / "data.json", "r+") as f:
-            raw_contents = f.read()
-            if raw_contents:
-                data: Dict[str, Dict] = json.loads(raw_contents)
-            else:
-                logger.error("Local storage is empty; could not find by uuid.")
-                return None
+        self._set_up_mlflow_env()
+        registered._env_vars = {
+            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
+            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
+        }
 
-        if "pipelines" in data and uuid in data["pipelines"]:
-            result = data["pipelines"][uuid]
-            return json.dumps(result)
-        else:
-            logger.error(f"No pipeline found locally with uuid: {uuid}.")
-            return None
+        return registered
 
-    def publish_garden(self, garden=None, visibility="Public"):
-        # Takes a garden_id UUID as a subject, and a garden_doc dict, and
-        # publishes to the GARDEN_INDEX_UUID index.  Polls to discover status,
-        # and returns the Task document:
+    def publish_garden_metadata(self, garden: Garden):
+        # Takes a garden, and publishes to the GARDEN_INDEX_UUID index.  Polls
+        # to discover status, and returns the Task document:
         # https://docs.globus.org/api/search/reference/get_task/#task
-
-        # Sanity check visibility--if it is a string, make it a list of strings
-        if isinstance(visibility, str):
-            visibility = [visibility]
-
+        garden_meta = json.loads(garden.expanded_json())
         gmeta_ingest = {
-            "subject": str(garden.uuid),
-            "visible_to": visibility,
-            "content": json.loads(garden.json()),
+            "subject": garden_meta["uuid"],
+            "visible_to": ["all_authenticated_users"],
+            "content": garden_meta,
         }
 
         publish_result = self.search_client.create_entry(
             GARDEN_INDEX_UUID, gmeta_ingest
         )
 
         task_result = self.search_client.get_task(publish_result["task_id"])
         while not task_result["state"] in {"FAILED", "SUCCESS"}:
             time.sleep(5)
             task_result = self.search_client.get_task(publish_result["task_id"])
         return task_result
+
+    def search(self, query: str) -> str:
+        res = self.search_client.search(GARDEN_INDEX_UUID, query, advanced=True)
+        return res.text
```

### Comparing `garden_ai-0.3.1/garden_ai/datacite.py` & `garden_ai-0.4.0/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.3.1/garden_ai/gardens.py` & `garden_ai-0.4.0/garden_ai/gardens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from __future__ import annotations
 
+import json
 import logging
 from datetime import datetime
-from typing import List, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field, ValidationError, validator
 
+from garden_ai.utils.misc import JSON, garden_json_encoder
+
 from .datacite import (
     Contributor,
     Creator,
     DataciteSchema,
     Description,
     RelatedIdentifier,
     Title,
     Types,
 )
-from .pipelines import Pipeline
-from .steps import Step
-from .utils import JSON, garden_json_encoder
+from .pipelines import RegisteredPipeline
 
 logger = logging.getLogger()
 
 
+class PipelineNotFoundException(KeyError):
+    """Exception raised when a Garden references an unknown pipeline uuid"""
+
+
 class Garden(BaseModel):
     """Object representation of a Garden™.
 
     Required Attributes
     --------------------
     authors: List[str]
         The main researchers involved in producing the Garden. At least one
@@ -80,61 +85,94 @@
         gc.register(pea_garden)
 
     Notes
     --------
     Mendel's work was ignored by the scientific community during his lifetime,
     presumably due to the lack of a working DOI.
     To remedy this, if the `doi` field is unset when registering the garden, we
-    build one for the user with the datacite api (see the `request_doi()`
-    method).
+    build one for the user with the datacite api.
     """
 
     class Config:
         """
         Configure pydantic per-model settings.
 
         We disable validate_all so that pydantic ignores temporarily-illegal defaults
         We enable validate_assignment to make validation occur naturally even after object construction
         """
 
         validate_all = False  # (this is the default)
         validate_assignment = True  # validators invoked on assignment
         underscore_attrs_are_private = True
 
+    title: str = cast(str, Field(default_factory=lambda: None))
     authors: List[str] = Field(default_factory=list, min_items=1, unique_items=True)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
-    # note: default_factory=lambda:None allows us to have fields which are None by
-    # default, but not automatically considered optional by pydantic
-    title: str = cast(str, Field(default_factory=lambda: None))
-    doi: str = cast(str, Field(default_factory=lambda: None))
-    # ^ casts here to appease mypy
+    doi: Optional[str] = Field(default=None)
     description: Optional[str] = Field(None)
     publisher: str = "Garden"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     language: str = "en"
     tags: List[str] = Field(default_factory=list, unique_items=True)
-    version: str = "0.0.1"  # TODO: enforce semver for this?
-    pipelines: List[Pipeline] = Field(default_factory=list)
+    version: str = "0.0.1"
     uuid: UUID = Field(default_factory=uuid4, allow_mutation=False)
+    pipeline_ids: List[UUID] = Field(default_factory=list)
 
     @validator("year")
     def valid_year(cls, year):
         if len(str(year)) != 4:
             raise ValueError("year must be formatted `YYYY`")
         return str(year)
 
-    def json(self, **kwargs):
-        def pipeline_id_only_encoder(obj):
-            if isinstance(obj, Pipeline):
-                return {"uuid": str(obj.uuid), "doi": obj.doi}
-            else:
-                return garden_json_encoder(obj)
+    def collect_pipelines(self) -> List[RegisteredPipeline]:
+        """Collect the full ``RegisteredPipeline`` objects referred to by this garden's pipeline_ids."""
+        from .local_data import get_local_pipeline_by_uuid
+
+        pipelines = []
+        for uuid in self.pipeline_ids:
+            pipeline = get_local_pipeline_by_uuid(uuid)
+            if pipeline is None:
+                raise PipelineNotFoundException(
+                    f"Could not find registered pipeline with id {uuid}."
+                )
+            pipelines += [pipeline]
+        return pipelines
 
-        kwargs.update(encoder=pipeline_id_only_encoder)
-        return super().json(**kwargs)
+    def expanded_metadata(self) -> Dict[str, Any]:
+        """Helper: build the "complete" metadata dict with nested ``Pipeline`` and ``step`` metadata.
+
+        Notes
+        ------
+        When serializing normally with ``garden.{dict(), json()}``, only the
+        uuids of the pipelines in the garden are included.
+
+        This returns a superset of ``garden.dict()``, so that the following holds:
+
+            valid_garden == Garden(**valid_garden.expanded_metadata()) == Garden(**valid_garden.dict())
+
+        Returns
+        -------
+        Dict[str, Any]  ``Garden`` metadata dict augmented with a list of ``RegisteredPipeline`` metadata
+
+        Raises
+        ------
+        PipelineNotFoundException  if ``garden.pipeline_ids`` references an unknown pipeline id.
+        """
+
+        data = self.dict()
+        data["pipelines"] = [p.dict() for p in self.collect_pipelines()]
+        return data
+
+    def expanded_json(self) -> JSON:
+        """Helper: return the expanded garden metadata as JSON.
+
+        See: ``Garden.expanded_metadata`` method
+        """
+        data = self.expanded_metadata()
+        return json.dumps(data, default=garden_json_encoder)
 
     def datacite_json(self) -> JSON:
         """Parse this `Garden`s metadata into a DataCite-schema-compliant JSON string.
 
         Leverages a pydantic class `DataCiteSchema`, which was automatically generated from:
         https://github.com/datacite/schema/blob/master/source/json/kernel-4.3/datacite_4.3_schema.json
 
@@ -154,16 +192,15 @@
             language=self.language,
             relatedIdentifiers=[
                 RelatedIdentifier(
                     relatedIdentifier=p.doi,
                     relatedIdentifierType="DOI",
                     relationType="HasPart",
                 )
-                for p in self.pipelines
-                if p.doi
+                for p in self.collect_pipelines()
             ],
             version=self.version,
             descriptions=[
                 Description(description=self.description, descriptionType="Other")
             ]
             if self.description
             else None,
@@ -197,56 +234,28 @@
         pea_garden.validate()
         # ...
         # ValidationError: 1 validation error for Garden
         # authors -> 1
         #   none is not an allowed value (type=type_error.none.not_allowed)
         """
         try:
-            self._sync_author_metadata()
-            _ = self.__init__(**self.dict())
+            _ = self.__class__(**self.dict())
         except ValidationError as err:
             logger.error(err)
             raise
 
     def _sync_author_metadata(self):
         """helper: authors and contributors of steps and Pipelines also appear as contributors in their respective Pipeline and Garden's metadata.
 
         We'll probably want to tweak the behavior of this at some point once we
         tease out what we really want `contributor` to entail, but for now this
         seems like a sane default.
         """
         known_contributors = set(self.contributors)
         # garden contributors don't need to duplicate garden authors unless they've been explicitly added
         known_authors = set(self.authors) - known_contributors
-        for pipe in self.pipelines:
-            pipe._sync_author_metadata()
+        for pipe in self.collect_pipelines():
             new_contributors = set(pipe.authors) | set(pipe.contributors)
             known_contributors |= new_contributors - known_authors
 
         self.contributors = list(known_contributors)
         return
-
-    def add_new_pipeline(
-        self, title: str, steps: List[Step], authors: List[str] = None, **kwargs
-    ):
-        """Create a new Pipeline object and add it to this Garden's list of pipelines.
-
-        Arguments (along with any further `kwargs`, e.g. `description`) have the
-        same meaning as in `Pipeline` constructor.
-
-        If not provided, the `authors` field of the pipeline will be set to this
-        garden's `authors` attribute.
-
-        """
-        kwargs.update(
-            authors=authors if authors else self.authors,
-            title=title,
-            steps=tuple(steps),
-        )
-        pipe = Pipeline(**kwargs)
-        self.pipelines += [pipe]
-        return
-
-    def remove_pipeline(self, to_remove: Pipeline):
-        """Removes a given Pipeline object from this Garden, if present."""
-        self.pipelines = [p for p in self.pipelines if p.uuid != to_remove.uuid]
-        return
```

### Comparing `garden_ai-0.3.1/garden_ai/mlflow_bandaid/binary_header_provider.py` & `garden_ai-0.4.0/garden_ai/mlflow_bandaid/binary_header_provider.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.3.1/garden_ai/steps.py` & `garden_ai-0.4.0/garden_ai/steps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
+import json
 import logging
 import typing
 from functools import update_wrapper, wraps
 from inspect import Parameter, Signature, signature
-from typing import Callable, Dict, List, Optional
-from uuid import UUID, uuid4
+from typing import Any, Callable, Dict, List, Optional
 
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
 from typing_extensions import get_type_hints
 
-from garden_ai.mlmodel import Model
+from garden_ai.mlmodel import Model, _Model
+from garden_ai.utils.misc import JSON, garden_json_encoder
 
 logger = logging.getLogger()
 
 
 class DataclassConfig:
     # pydantic dataclasses read their config via decorator argument, not as
     # nested class (like BaseModels do)
     validate_assignment = True
-    underscore_attrs_are_private = True
 
 
 @dataclass(config=DataclassConfig)
 class Step:
     """The ``Step`` class (via the ``@step`` decorator) wraps a callable for use as a single step in a ``Pipeline``.
 
     **IMPORTANT**: When included in a ``Pipeline``, all ``Step``s will be checked
@@ -117,15 +117,17 @@
     func: Callable
     authors: List[str] = Field(default_factory=list)
     contributors: List[str] = Field(default_factory=list)
     title: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     input_info: Optional[str] = Field(None)
     output_info: Optional[str] = Field(None)
-    uuid: UUID = Field(default_factory=uuid4)
+    conda_dependencies: List[str] = Field(default_factory=list)
+    pip_dependencies: List[str] = Field(default_factory=list)
+    python_version: Optional[str] = Field(None)
 
     def __post_init_post_parse__(self):
         # like __post_init__, but called after pydantic validation
         # copies e.g. __doc__ and __name__ from
         # the underlying callable to this object
         # (also handy for signature/annotations)
         update_wrapper(self, self.func)
@@ -134,27 +136,44 @@
         self.__signature__ = signature(self.func)
         input_hints: Dict = get_type_hints(self.func, include_extras=True)
         return_hint = input_hints.pop("return")
         if self.input_info is None:
             self.input_info = str(input_hints)
         if self.output_info is None:
             self.output_info = f"return: {return_hint}"
+        self._infer_model_deps()
         return
 
     def __call__(self, *args, **kwargs):
         # keep it simple: just pass input the underlying callable.
         return self.func(*args, **kwargs)
 
+    def _infer_model_deps(self):
+        """
+        If this step's function has a Model as a default argument, like
+        ``func(*args, model=Model(...))``, extract the dependencies for that model
+        and track them as step-level dependencies.
+        """
+
+        sig = signature(self.func)
+        for param in sig.parameters.values():
+            if isinstance(param.default, _Model):
+                model = param.default
+                self.python_version = model.python_version
+                self.conda_dependencies += model.conda_dependencies
+                self.pip_dependencies += model.pip_dependencies
+        return
+
     @validator("func")
     def has_annotations(cls, f: Callable):
         sig = signature(f)
         # check that any positional arguments have annotations
         for p in sig.parameters.values():
             if p.annotation is Parameter.empty is p.default:
-                # fine to skip annotation if there's a default we can use to infer type
+                # fine to skip annotation only if there's a default we can use to infer type
                 raise TypeError(
                     f"Parameter {p} is missing an annotation in {f.__name__}'s definition. "
                     "Please double check that the argument list is fully annotated.\n"
                     "See also: https://peps.python.org/pep-0484/#type-definition-syntax"
                 )
         # check that return value has annotation
         if sig.return_annotation in {Signature.empty, None}:
@@ -185,14 +204,24 @@
                 "before being published as a Pipeline. Please try again with a more descriptive type hint.\n"
                 "We use `beartype` to resolve type hints -- for a full list of supported annotations \n "
                 "(including 3rd party type hints, like `numpy.typing`), see:\n "
                 "https://github.com/beartype/beartype#compliance"
             )
         return f
 
+    def json(self) -> JSON:
+        return json.dumps(self, default=garden_json_encoder)
+
+    def dict(self) -> Dict[str, Any]:
+        d = {}
+        for key in self.__dataclass_fields__:
+            val = getattr(self, key)
+            d[key] = val
+        return d
+
 
 def step(func: Callable = None, **kwargs):
     """Helper: provide ``@step(...)`` decorator for creation of ``Step``s."""
     # note:
     # The ``Step`` class itself could also technically be used as a decorator,
     # but would run into trouble as soon as you tried passing any arguments:
     # this definition means ``@step`` and ``@step(...)`` are equivalent decorators,
@@ -213,29 +242,30 @@
 
 
 def inference_step(model_uri: str, **kwargs):
     """Helper: provide ``@inference_step(...)`` decorator for creation of ``Step``s.
 
     Example:
     --------
-    ```python
-    @inference_step(model_uri="models:/my-model/my-version")
-    def my_step(data: pd.DataFrame) -> MyResultType:
-        pass  # NOTE: leave the function body empty
-
-    ## equivalent to:
-
-    def my_step(data: MyDataType) -> MyResultType:
-        model = garden_ai.Model("models:/my-model/my-version")
-        return model.predict(data)
-    ```
+        ```python
+        @inference_step(model_uri="me@uni.edu-my-model/version")
+        def my_step(data: pd.DataFrame) -> MyResultType:
+            pass  # NOTE: leave the function body empty
+
+        ## equivalent to:
+        @step
+        def my_step(
+            data: MyDataType,
+            model=garden_ai.Model("me@uni.edu-my-model/version"),
+        ) -> MyResultType:
+            return model.predict(data)
+        ```
     """
 
     def wrapper(f: Callable):
         @wraps(f)  # make sure we aren't losing signature info
-        def boilerplate(*args, **_kwargs):
-            model = Model(model_uri)
+        def boilerplate(*args, model=Model(model_uri), **_kwargs):
             return model.predict(*args)
 
         return step(boilerplate)
 
     return wrapper
```

### Comparing `garden_ai-0.3.1/garden_ai/templates/pipeline` & `garden_ai-0.4.0/garden_ai/templates/pipeline`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 ## THIS FILE WAS AUTOMATICALLY GENERATED ##
-from garden_ai import Pipeline, step, Model
+from garden_ai import GardenClient, Model, Pipeline, step
 import typing
 
+client = GardenClient()
 ##################################### STEPS #####################################
 """
 Brief notes on steps (see docs for more detail):
 
-    - any python callable can be made into a step by decorating it with `@step`.
-    - the callable MUST have valid type-hints for all arguments and return type.
-    - these type-hints are used to verify that the steps can be composed in a pipeline.
-    - steps also extract metadata from the callable, like `description` or
-        `output_info` from the callable's docstring or return annotation,
-        respectively.
-    - don't use `Any` or `None` in step annotations. If a step is indeed general enough to
-        accept or return any python object, prefer `object` as the annotation.
+    - you may define your pipeline using as many or as few @steps as you like.
+
+    - Any python function or callable can be made into a step by decorating it
+        with `@step`, like below.
+
+    - these functions will be composed in the pipeline (i.e. calling the pipeline
+        is equivalent to calling each step in order).
+
+    - the steps MUST have valid type-hints for all positional arguments and
+        return types.
+      - don't use `Any` or `None` in step annotations
+      - these type-hints are used to verify that steps are compatible when
+          composing (no checking at runtime)
 """
 
 # example step using the decorator:
 @step
 def preprocessing_step(input_data: object) -> object:
     """ """
     # TODO
     pass
 
 
-# metadata can also be manually specified with kwargs
-@step(input_info=..., authors=...)
+@step()
 def another_step(data: object) -> object:
     # TODO
     pass
 
 
 @step
-def run_inference(arg: object, model = Model("YOUR MODEL's URI HERE")) -> object:
+def run_inference(
+    input_arg: object,
+    model=Model("YOUR MODEL's NAME HERE"),
+) -> object:
     pass
 
-# steps will be composed in order by the pipeline below
+# the step functions will be composed in order by the pipeline:
 ALL_STEPS = (
     preprocessing_step,
     another_step,
     run_inference,
 )
 
+REQUIREMENTS_FILE = None  # to specify additional dependencies, replace `None`
+                          # with an "/absolute/path/to/requirements.txt"
+
 ################################### PIPELINE ####################################
 
-{{ shortname }} = Pipeline(
+{{ shortname }}: Pipeline = client.create_pipeline(
     title="{{ pipeline.title }}",
     steps=ALL_STEPS,
+    requirements_file=REQUIREMENTS_FILE,
     authors={{ pipeline.authors }},
     contributors={{ pipeline.contributors }},
     description="{{ pipeline.description }}",
     version="{{ pipeline.version }}",
     year={{ pipeline.year }},
-    tags= {{ pipeline.tags }},
+    tags={{ pipeline.tags }},
     uuid="{{ pipeline.uuid }}",  # WARNING: DO NOT EDIT UUID
 )
```

### Comparing `garden_ai-0.3.1/PKG-INFO` & `garden_ai-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.3.1
+Version: 0.4.0
 Summary: Garden: tools to simplify access to scientific AI advances.
 License: Apache-2.0
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: flavors
+Provides-Extra: tensorflow
+Provides-Extra: torch
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: boto3 (>=1.26.77,<2.0.0)
+Requires-Dist: dparse[conda] (>=0.6.2,<0.7.0)
+Requires-Dist: globus-compute-sdk (>=2.0.0,<3.0.0)
 Requires-Dist: globus-sdk (>=3.12.0,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mlflow (==2.2.1)
 Requires-Dist: numba (>=0.56,<0.57)
+Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
+Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "flavors")
+Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "flavors"
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Garden
 
 [![NSF-2209892](https://img.shields.io/badge/NSF-2209892-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209892&HistoricalAwards=false)
 [![PyPI](https://badge.fury.io/py/garden-ai.svg)](https://badge.fury.io/py/garden-ai)
```


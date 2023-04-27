# Comparing `tmp/GitLabCICli-0.2.2.tar.gz` & `tmp/gitlabcicli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GitLabCICli-0.2.2.tar", max compression
+gzip compressed data, was "gitlabcicli-0.2.3.tar", max compression
```

## Comparing `GitLabCICli-0.2.2.tar` & `gitlabcicli-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 GitLabCICli-0.2.2/LICENSE
--rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 GitLabCICli-0.2.2/gitlabcicli/__init__.py
--rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 GitLabCICli-0.2.2/gitlabcicli/__main__.py
--rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 GitLabCICli-0.2.2/gitlabcicli/api/__init__.py
--rw-r--r--   0        0        0     2182 2020-12-08 14:07:42.259276 GitLabCICli-0.2.2/gitlabcicli/api/gitlab_api_driver.py
--rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 GitLabCICli-0.2.2/gitlabcicli/api/models/__init__.py
--rw-r--r--   0        0        0     1498 2020-12-08 14:07:42.219276 GitLabCICli-0.2.2/gitlabcicli/api/models/pipeline.py
--rw-r--r--   0        0        0     3950 2020-12-08 14:07:42.339276 GitLabCICli-0.2.2/gitlabcicli/api/models/project.py
--rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 GitLabCICli-0.2.2/gitlabcicli/gitlabapiwrapper.py
--rwxr-xr-x   0        0        0    19568 2022-02-04 13:05:04.027149 GitLabCICli-0.2.2/gitlabcicli/gitlabcicli.py
--rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 GitLabCICli-0.2.2/gitlabcicli/gitwrapper.py
--rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 GitLabCICli-0.2.2/gitlabcicli/managerlib/__init__.py
--rw-r--r--   0        0        0     4657 2020-12-08 14:07:42.339276 GitLabCICli-0.2.2/gitlabcicli/managerlib/api_driver.py
--rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 GitLabCICli-0.2.2/gitlabcicli/managerlib/errors.py
--rw-r--r--   0        0        0     7296 2020-12-08 14:07:42.429276 GitLabCICli-0.2.2/gitlabcicli/managerlib/fields.py
--rw-r--r--   0        0        0     3887 2020-12-08 14:07:42.349276 GitLabCICli-0.2.2/gitlabcicli/managerlib/model.py
--rw-r--r--   0        0        0      698 2020-05-04 21:50:57.300409 GitLabCICli-0.2.2/gitlabcicli/managerlib/utils.py
--rw-r--r--   0        0        0     1004 2020-11-13 21:40:57.960798 GitLabCICli-0.2.2/gitlabcicli/script_helpers.py
--rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 GitLabCICli-0.2.2/gitlabcicli/utils.py
--rw-r--r--   0        0        0      686 2022-02-04 13:06:38.047634 GitLabCICli-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1031 2022-02-04 13:08:23.208718 GitLabCICli-0.2.2/setup.py
--rw-r--r--   0        0        0      862 2022-02-04 13:08:23.208950 GitLabCICli-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.3/LICENSE
+-rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.3/gitlabcicli/__init__.py
+-rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.3/gitlabcicli/__main__.py
+-rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.3/gitlabcicli/api/__init__.py
+-rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.3/gitlabcicli/api/gitlab_api_driver.py
+-rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.3/gitlabcicli/api/models/__init__.py
+-rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.3/gitlabcicli/api/models/pipeline.py
+-rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.3/gitlabcicli/api/models/project.py
+-rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.3/gitlabcicli/gitlabapiwrapper.py
+-rwxr-xr-x   0        0        0    19468 2023-04-27 09:33:06.459609 gitlabcicli-0.2.3/gitlabcicli/gitlabcicli.py
+-rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.3/gitlabcicli/gitwrapper.py
+-rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.3/gitlabcicli/managerlib/__init__.py
+-rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.3/gitlabcicli/managerlib/api_driver.py
+-rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.3/gitlabcicli/managerlib/errors.py
+-rw-r--r--   0        0        0     7252 2023-04-27 09:33:46.186499 gitlabcicli-0.2.3/gitlabcicli/managerlib/fields.py
+-rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.3/gitlabcicli/managerlib/model.py
+-rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.3/gitlabcicli/managerlib/utils.py
+-rw-r--r--   0        0        0     1004 2020-11-13 21:40:57.960798 gitlabcicli-0.2.3/gitlabcicli/script_helpers.py
+-rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.3/gitlabcicli/utils.py
+-rw-r--r--   0        0        0      727 2023-04-27 09:27:37.697756 gitlabcicli-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 gitlabcicli-0.2.3/PKG-INFO
```

### Comparing `GitLabCICli-0.2.2/LICENSE` & `gitlabcicli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GitLabCICli-0.2.2/gitlabcicli/api/gitlab_api_driver.py` & `gitlabcicli-0.2.3/gitlabcicli/api/gitlab_api_driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 
 class GitLabAPIDriver(SimpleReadOnlyRESTAPIDriver):
     """The API driver for GitLab API."""
 
     API_PATH = "/api/v4"
 
-    def __init__(self, host: str, private_token: typing.Optional[str] = None):
+    def __init__(self, host: str, private_token: str | None = None):
         super().__init__(host)
 
         if private_token:
             self.session.headers["PRIVATE-TOKEN"] = private_token
 
     def create_filter_params(
         self,
         **filter,
-    ) -> typing.Dict[str, typing.Union[str, int, bool]]:
+    ) -> dict[str, str | int | bool]:
         self._check_model_set()
 
         if self._model is Pipeline:
             # TODO
 
             return filter
         elif self._model is Project:
@@ -47,15 +47,15 @@
             return query
         else:
             raise OperationalError(f"Unknown model configured: {self._model}")
 
     def create_order_params(
         self,
         *properties,
-    ) -> typing.Dict[str, typing.Union[str, int, bool]]:
+    ) -> dict[str, str | int | bool]:
         self._check_model_set()
 
         if self._model is Pipeline:
             # TODO
 
             return {}
         elif self._model is Project:
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/api/models/pipeline.py` & `gitlabcicli-0.2.3/gitlabcicli/api/models/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     StrField,
     StrIntField,
 )
 
 
 class Pipeline(Model):
     #  The ID or URL-encoded path of the project owned by the authenticated user
-    id: typing.Union[int, str] = StrIntField()
+    id: int | str = StrIntField()
     # The scope of pipelines, one of: running, pending, finished, branches, tags
     scope: str = StrField()
     # The status of pipelines, one of: running, pending, success, failed, canceled, skipped, created, manual
     status: str = StrField()
     # The ref of pipelines
     ref: str = StrField()
     # The SHA of pipelines
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/api/models/project.py` & `gitlabcicli-0.2.3/gitlabcicli/api/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description: str = StrField()
     default_branch: str = StrField(default="master", nullable=True)
     visibility = StrField(choices=ProjectVisibility)
     ssh_url_to_repo: str = StrField(readonly=True)
     http_url_to_repo: str = StrField(readonly=True)
     web_url: str = StrField(readonly=True)
     readme_url: str = StrField(readonly=True, nullable=True)
-    tag_list: typing.List[str] = ListField([StrField()], readonly=True)
+    tag_list: list[str] = ListField([StrField()], readonly=True)
     #  "owner": {
     #      "id": 3,
     #      "name": "Diaspora",
     #      "created_at": "2013-09-30T13:46:02Z"
     #  },
     name: str = StrField()
     name_with_namespace: str = StrField()
@@ -72,15 +72,15 @@
     avatar_url: str = StrField(nullable=True, readonly=True)
     shared_runners_enabled: bool = BoolField()
     forks_count: int = PositiveIntField(readonly=True)
     star_count: int = PositiveIntField(readonly=True)
     runners_token: str = StrField()
     ci_default_git_depth: int = PositiveIntField(nullable=True)
     public_jobs: bool = BoolField()
-    shared_with_groups: typing.List = ListField([StrIntField()], readonly=True)
+    shared_with_groups: list = ListField([StrIntField()], readonly=True)
     only_allow_merge_if_pipeline_succeeds: bool = BoolField(default=False)
     only_allow_merge_if_all_discussions_are_resolved: bool = BoolField(default=False)
     remove_source_branch_after_merge: bool = BoolField(default=False, nullable=True)
     request_access_enabled: bool = BoolField()
     merge_method: str = StrField(default="merge")
     autoclose_referenced_issues: bool = BoolField(default=True)
     suggestion_commit_message: str = StrField(nullable=True, default=None)
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/gitlabapiwrapper.py` & `gitlabcicli-0.2.3/gitlabcicli/gitlabapiwrapper.py`

 * *Files identical despite different names*

### Comparing `GitLabCICli-0.2.2/gitlabcicli/gitlabcicli.py` & `gitlabcicli-0.2.3/gitlabcicli/gitlabcicli.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,17 +80,17 @@
 
 
 COMMANDS = dict[str, Command]()
 
 
 def register_command(
     *,
-    name: typing.Optional[str] = None,
+    name: str | None = None,
     aliases: set[str] = frozenset[str](),
-    doc: typing.Optional[str] = None,
+    doc: str | None = None,
 ) -> typing.Callable:
     """Decorator to register a command"""
 
     def inner(func: typing.Callable) -> typing.Callable:
         cmd_name = name or func.__name__.replace("_", "-")
         COMMANDS[cmd_name] = Command(
             name=cmd_name,
@@ -120,15 +120,15 @@
     return [
         fn
         for fn in files
         if (os.path.isdir(fn) or ".gitlab-ci.yml".startswith(fn.split("/")[-1]))
     ]
 
 
-def get_token_from_keyring(server_url: str) -> typing.Optional[str]:
+def get_token_from_keyring(server_url: str) -> str | None:
     """Retreive the token for current server from keyring."""
 
     try:
         return keyring.get_password(KEYRING_SERVICE_NAME, server_url)
     except Exception as exc:
         error(
             "No token found in wallet. Please use --ask-for-token to specify your token."
@@ -247,21 +247,21 @@
     print(tabulate(table_jobs, headers=table_headers, disable_numparse=True))
 
 
 class GitLabCiCli(object):
     """A Cli class."""
 
     def __init__(self, **kwargs):
-        self._api_client: typing.Optional[GitLabApiClient] = None
-        self._server_url: typing.Optional[str] = kwargs.get("server_url", None)
-        self._project_id: typing.Optional[int] = kwargs.get("project_id", None)
-        self._project_path: typing.Optional[str] = kwargs.get("project_path", None)
-        self._project: typing.Optional[str] = kwargs.get("project", None)
-        self._token: typing.Optional[str] = kwargs.get("token", None)
-        self._commit_hash: typing.Optional[str] = kwargs.get("commit_hash", None)
+        self._api_client: GitLabApiClient | None = None
+        self._server_url: str | None = kwargs.get("server_url", None)
+        self._project_id: int | None = kwargs.get("project_id", None)
+        self._project_path: str | None = kwargs.get("project_path", None)
+        self._project: str | None = kwargs.get("project", None)
+        self._token: str | None = kwargs.get("token", None)
+        self._commit_hash: str | None = kwargs.get("commit_hash", None)
         self.args = kwargs
 
     def stop(self):
         """Shutdown."""
 
         if self._token:
             keyring.set_password(KEYRING_SERVICE_NAME, self.server_url, self._token)
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/gitwrapper.py` & `gitlabcicli-0.2.3/gitlabcicli/gitwrapper.py`

 * *Files identical despite different names*

### Comparing `GitLabCICli-0.2.2/gitlabcicli/managerlib/api_driver.py` & `gitlabcicli-0.2.3/gitlabcicli/managerlib/api_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     The abstract class all API implementations must inherit from.
 
     It follows more or less the CRUD design.
     """
 
     def __init__(self):
-        self._model: typing.Optional[typing.Type[Model]] = None
+        self._model: typing.Type[Model] | None = None
 
     def use(self, model: typing.Type[Model]) -> APIDriver:
         """
         Configure the api driver to use a specific model for the next operation(s).
         """
         self._model = model
 
@@ -47,23 +47,23 @@
 
     def create(self, instance: Model) -> Model:
         """Create an instance of ``instance`` on the server side."""
         self._check_model_set()
         instance.validate()
         raise NotImplementedError()
 
-    def get(self, **filter) -> typing.Optional[Model]:
+    def get(self, **filter) -> Model | None:
         """Get a single instance for a given ``filter``."""
         self._check_model_set()
         raise NotImplementedError()
 
     def list(
         self,
-        filter: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        order_by: typing.Optional[typing.List[str]] = None,
+        filter: dict[str, typing.Any] | None = None,
+        order_by: list[str] | None = None,
     ) -> typing.Iterable[Model]:
         """Get all matching instances for a given ``filter``."""
         self._check_model_set()
         raise NotImplementedError()
 
     def update(self) -> Model:
         """Update a ressource."""
@@ -104,16 +104,16 @@
     def get(self, **filter):
         matching_instances = self.list(**filter)
 
         return check_single_result(matching_instances)
 
     def list(
         self,
-        filter: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        order_by: typing.Optional[typing.List[str]] = None,
+        filter: dict[str, typing.Any] | None = None,
+        order_by: list[str] | None = None,
     ) -> typing.Iterable[Model]:
         self._check_model_set()
 
         response = self.session.get(
             self.resource_url,
             params={
                 **(self.create_filter_params(**filter) if filter else {}),
@@ -140,22 +140,22 @@
 
         return results
 
     @abstractmethod
     def create_filter_params(
         self,
         **filter,
-    ) -> typing.Dict[str, typing.Union[str, int, bool]]:
+    ) -> dict[str, str | int | bool]:
         """Create the GET-parameters for a given ``filter``."""
 
     @abstractmethod
     def create_order_params(
         self,
         *properties,
-    ) -> typing.Dict[str, typing.Union[str, int, bool]]:
+    ) -> dict[str, str | int | bool]:
         """
         Create the GET-parameters for sorting the results.
 
         :param properties: Property names of the model in this notation `-id`, `+name`, `date_created`.
         """
 
     def __str__(self):
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/managerlib/fields.py` & `gitlabcicli-0.2.3/gitlabcicli/managerlib/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     def __init__(
         self,
         description: str = "",
         default: typing.Any = EmptyParameter,
         nullable: bool = False,
         choices: "Enum" = None,
         readonly: bool = False,
-        validators: typing.List[typing.Callable[[typing.Any], None]] = [],
+        validators: list[typing.Callable[[typing.Any], None]] = [],
         is_id_field: bool = False,
     ):
         self.description = description
         self.default = default
         self.nullable = nullable
         self.choices = choices
         self.readonly = readonly
         self.required = default == EmptyParameter
         self.validators = validators
         self.is_id_field = is_id_field
 
-    def clean(self, value: typing.Any, _field_name: typing.Optional[str] = None):
+    def clean(self, value: typing.Any, _field_name: str | None = None):
         """Validate and clean the value."""
 
         if value is None:
             if self.nullable:
                 return None
             else:
                 raise ValidationError(
@@ -104,15 +104,15 @@
 
         value = super().clean(value, **kwargs)
 
         return value
 
 
 class PositiveIntField(IntField):
-    def clean(self, value, _field_name: typing.Optional[str] = None):
+    def clean(self, value, _field_name: str | None = None):
         value: int = super().clean(value, _field_name=_field_name)
 
         if value is not None and value < 0:
             raise ValidationError(
                 f"Value must not be smaller than zero in field '{_field_name}'."
                 if _field_name
                 else "Value must not be smaller than zero."
@@ -182,15 +182,15 @@
 
         raise ValidationError(errs)
 
 
 class ListField(Field):
     def __init__(
         self,
-        child_fields: typing.List[Field],
+        child_fields: list[Field],
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.child_fields = child_fields
         # inherit arguments to child fields:
 
         for child_field in child_fields:
@@ -198,15 +198,15 @@
                 child_field.default = self.default
 
             if child_field.choices is None:
                 child_field.choices = self.choices
             child_field.readonly |= self.readonly
             child_field.validators.extend(self.validators)
 
-    def clean(self, value, _field_name: typing.Optional[str] = None):
+    def clean(self, value, _field_name: str | None = None):
         if not isinstance(value, Iterable):
             raise ValidationError(
                 f"Value for field '{_field_name}' is not iterable."
                 if _field_name
                 else "Value is not iterable."
             )
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/managerlib/model.py` & `gitlabcicli-0.2.3/gitlabcicli/managerlib/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 # not required, use default value
                 setattr(self, name, description.default)
 
         if missing_args:
             raise ValueError(f'Missing argument for {", ".join(missing_args)}')
 
     @classmethod
-    def from_api(cls, data: typing.Dict[typing.Any, typing.Any]) -> Model:
+    def from_api(cls, data: dict[typing.Any, typing.Any]) -> Model:
         """
         Create an instance from values fetched from the remote API.
 
         We do not expect to get all values.
         Additional data will be ignored.
         """
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/managerlib/utils.py` & `gitlabcicli-0.2.3/gitlabcicli/managerlib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, func):
         self.func = func
 
     def __get__(self, obj, owner):
         return self.func(owner)
 
 
-def check_single_result(results: typing.List[Model]) -> Model:
+def check_single_result(results: list[Model]) -> Model:
     """
     Check if there is only one result in the results list and return it. Raise exceptions otherwise.
     """
 
     if len(results) == 1:
         return results[0]
```

### Comparing `GitLabCICli-0.2.2/gitlabcicli/script_helpers.py` & `gitlabcicli-0.2.3/gitlabcicli/script_helpers.py`

 * *Files identical despite different names*

### Comparing `GitLabCICli-0.2.2/PKG-INFO` & `gitlabcicli-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gitlabcicli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command line interface for GitLab CI
 Home-page: https://gitlab.com/sedrubal/gitlabcicli.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: GitPython (>=3.1.11,<4.0.0)
-Requires-Dist: argcomplete (>=1.12.2,<2.0.0)
-Requires-Dist: dbus-python (>=1.2.16,<2.0.0)
-Requires-Dist: keyring (>=21.5.0,<22.0.0)
-Requires-Dist: requests (>=2.25.0,<3.0.0)
-Requires-Dist: tabulate (>=0.8.7,<0.9.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: GitPython (>=3.1.31,<4.0.0)
+Requires-Dist: argcomplete (>=1.12.3,<2.0.0)
+Requires-Dist: dbus-python (>=1.3.2,<2.0.0)
+Requires-Dist: keyring (>=21.8.0,<22.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: tabulate (>=0.8.10,<0.9.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/sedrubal/gitlabcicli.git
```


# Comparing `tmp/falcon_toolkit-3.1.1.tar.gz` & `tmp/falcon_toolkit-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_toolkit-3.1.1.tar", max compression
+gzip compressed data, was "falcon_toolkit-3.1.2.tar", max compression
```

## Comparing `falcon_toolkit-3.1.1.tar` & `falcon_toolkit-3.1.2.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/LICENSE.md
--rw-r--r--   0        0        0    20600 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/README.md
--rw-r--r--   0        0        0      188 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/__init__.py
--rw-r--r--   0        0        0      174 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/__init__.py
--rw-r--r--   0        0        0     1847 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth.py
--rw-r--r--   0        0        0      191 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/__init__.py
--rw-r--r--   0        0        0      449 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/default.py
--rw-r--r--   0        0        0     6069 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/public_mssp.py
--rw-r--r--   0        0        0     4020 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/public_single_cid.py
--rw-r--r--   0        0        0     2709 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/utils.py
--rw-r--r--   0        0        0     1831 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/cli.py
--rw-r--r--   0        0        0     7974 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/config.py
--rw-r--r--   0        0        0      962 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/console_utils.py
--rw-r--r--   0        0        0      385 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/constants.py
--rw-r--r--   0        0        0     2767 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/logging_config.py
--rw-r--r--   0        0        0      340 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/meta.py
--rw-r--r--   0        0        0     1599 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/namespace.py
--rw-r--r--   0        0        0     1944 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/common/utils.py
--rwxr-xr-x   0        0        0     7553 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/falcon.py
--rw-r--r--   0        0        0      116 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/hosts/__init__.py
--rw-r--r--   0        0        0     1016 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/hosts/cli.py
--rw-r--r--   0        0        0      941 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/hosts/host_search.py
--rw-r--r--   0        0        0      120 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/policies/__init__.py
--rw-r--r--   0        0        0     5058 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/policies/cli.py
--rw-r--r--   0        0        0     1049 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/policies/constants.py
--rw-r--r--   0        0        0     3354 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/policies/container.py
--rw-r--r--   0        0        0     3659 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/policies/describe.py
--rw-r--r--   0        0        0      160 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/__init__.py
--rw-r--r--   0        0        0     6397 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/cli.py
--rw-r--r--   0        0        0      219 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/cmd_generators/__init__.py
--rw-r--r--   0        0        0      335 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/cmd_generators/common.py
--rw-r--r--   0        0        0     2583 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/cmd_generators/reg.py
--rw-r--r--   0        0        0    19009 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/parsers.py
--rw-r--r--   0        0        0    40345 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/prompt.py
--rw-r--r--   0        0        0     1880 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/refresh.py
--rw-r--r--   0        0        0      681 2023-02-13 21:53:10.249379 falcon_toolkit-3.1.1/falcon_toolkit/shell/utils.py
--rw-r--r--   0        0        0     2075 2023-02-13 21:53:10.253379 falcon_toolkit-3.1.1/pyproject.toml
--rw-r--r--   0        0        0    22244 1970-01-01 00:00:00.000000 falcon_toolkit-3.1.1/setup.py
--rw-r--r--   0        0        0    22027 1970-01-01 00:00:00.000000 falcon_toolkit-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/LICENSE.md
+-rw-r--r--   0        0        0    20600 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/README.md
+-rw-r--r--   0        0        0      188 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/__init__.py
+-rw-r--r--   0        0        0     1847 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth.py
+-rw-r--r--   0        0        0      191 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/__init__.py
+-rw-r--r--   0        0        0      449 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/default.py
+-rw-r--r--   0        0        0     6069 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_mssp.py
+-rw-r--r--   0        0        0     4087 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_single_cid.py
+-rw-r--r--   0        0        0     2709 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/utils.py
+-rw-r--r--   0        0        0     1831 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/cli.py
+-rw-r--r--   0        0        0     7974 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/config.py
+-rw-r--r--   0        0        0      962 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/console_utils.py
+-rw-r--r--   0        0        0      385 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/constants.py
+-rw-r--r--   0        0        0     2767 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/logging_config.py
+-rw-r--r--   0        0        0      340 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/meta.py
+-rw-r--r--   0        0        0     1599 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/namespace.py
+-rw-r--r--   0        0        0     1944 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/utils.py
+-rwxr-xr-x   0        0        0     7553 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/falcon.py
+-rw-r--r--   0        0        0      116 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/__init__.py
+-rw-r--r--   0        0        0     1016 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/cli.py
+-rw-r--r--   0        0        0      941 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/host_search.py
+-rw-r--r--   0        0        0      120 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/__init__.py
+-rw-r--r--   0        0        0     5058 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/cli.py
+-rw-r--r--   0        0        0     1049 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/constants.py
+-rw-r--r--   0        0        0     3354 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/container.py
+-rw-r--r--   0        0        0     3659 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/describe.py
+-rw-r--r--   0        0        0      160 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/__init__.py
+-rw-r--r--   0        0        0     6397 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cli.py
+-rw-r--r--   0        0        0      219 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/common.py
+-rw-r--r--   0        0        0     2583 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/reg.py
+-rw-r--r--   0        0        0    18855 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/parsers.py
+-rw-r--r--   0        0        0    40348 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/prompt.py
+-rw-r--r--   0        0        0     1880 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/refresh.py
+-rw-r--r--   0        0        0      681 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/utils.py
+-rw-r--r--   0        0        0     2075 2023-04-27 18:21:51.779285 falcon_toolkit-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0    22027 1970-01-01 00:00:00.000000 falcon_toolkit-3.1.2/PKG-INFO
```

### Comparing `falcon_toolkit-3.1.1/LICENSE.md` & `falcon_toolkit-3.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/README.md` & `falcon_toolkit-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/auth.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/auth.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/public_mssp.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_mssp.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             _client_secret = fancy_input("Client Secret: ")
             self.client_secret = _client_secret
 
         return _client_secret
 
     @client_secret.setter
     def client_secret(self, _client_secret: str):
-        """Store the client secret to the system secrets store."""
+        """Store the client secret in the system secrets store."""
         keyring.set_password(
             service_name=KEYRING_SERVICE_NAME,
             username=self.client_id,
             password=_client_secret,
         )
 
     def dump_config(self) -> Dict[str, object]:
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/public_single_cid.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_single_cid.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             _client_secret = fancy_input("Client Secret: ")
             self.client_secret = _client_secret
 
         return _client_secret
 
     @client_secret.setter
     def client_secret(self, _client_secret: str):
+        """Store the client secret in the system secrets store."""
         keyring.set_password(
             service_name=KEYRING_SERVICE_NAME,
             username=self.client_id,
             password=_client_secret,
         )
 
     def dump_config(self) -> Dict[str, object]:
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/auth_backends/utils.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/cli.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/config.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/console_utils.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/console_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/logging_config.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/logging_config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/namespace.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/namespace.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/common/utils.py` & `falcon_toolkit-3.1.2/falcon_toolkit/common/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/falcon.py` & `falcon_toolkit-3.1.2/falcon_toolkit/falcon.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/hosts/cli.py` & `falcon_toolkit-3.1.2/falcon_toolkit/hosts/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/hosts/host_search.py` & `falcon_toolkit-3.1.2/falcon_toolkit/hosts/host_search.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/policies/cli.py` & `falcon_toolkit-3.1.2/falcon_toolkit/policies/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from click_option_group import (
     optgroup,
     RequiredMutuallyExclusiveOptionGroup,
 )
 
 from falcon_toolkit.common.cli import get_instance
-from falcon_toolkit.policies.constants import PoliciesAPIModule
+from falcon_toolkit.policies.constants import PoliciesApiModule
 from falcon_toolkit.policies.describe import pretty_print_policies
 from falcon_toolkit.policies.container import PolicyContainer
 
 
 @click.group(
     name='policies',
     help='Manage Falcon Prevention and Response policies',
@@ -71,30 +71,30 @@
 @click.command(
     name='describe',
     help='List and describe the policies within the Falcon tenant.'
 )
 @click.pass_context
 def policies_describe(ctx: click.Context):
     """List and describe the Prevention or Response policies within the Falcon tenant."""
-    policies_api: PoliciesAPIModule = ctx.obj['policies_api']
+    policies_api: PoliciesApiModule = ctx.obj['policies_api']
     policies_type: str = ctx.obj['policies_type']
     click.echo(click.style(f"Describing all {policies_type} policies", fg='green', bold=True))
     policies = policies_api.describe_policies()
     pretty_print_policies(policies)
 
 
 @click.command(
     name='export',
     help='Export a Prevention or Response policy to disk.',
 )
 @click.pass_context
 def policies_export(ctx: click.Context):
     """Allow a user to choose a Prevention or Response policy to export to disk."""
     # pylint: disable=too-many-locals
-    policies_api: PoliciesAPIModule = ctx.obj['policies_api']
+    policies_api: PoliciesApiModule = ctx.obj['policies_api']
     policies_type: str = ctx.obj['policies_type']
     click.echo("Loading policies...")
     policies = policies_api.describe_policies()
 
     options: List[pick.Option] = []
     for policy in policies:
         option_text = f"{policy.name} [{policy.platform_name}]"
@@ -138,15 +138,15 @@
     type=click.STRING,
 )
 def policies_import(
     ctx: click.Context,
     filename: str,
 ):
     """Import a Prevention or Response policy from the JSON file named FILENAME."""
-    policies_api: PoliciesAPIModule = ctx.obj['policies_api']
+    policies_api: PoliciesApiModule = ctx.obj['policies_api']
 
     click.echo(f"Loading policy in the file: {filename}")
 
     with open(filename, 'rt', encoding='utf-8') as policy_file_handle:
         policy_str = str(policy_file_handle.read())
 
     policy_container = PolicyContainer.loads(policy_str)
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/policies/constants.py` & `falcon_toolkit-3.1.2/falcon_toolkit/policies/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 POLICY_TYPES = [
     "prevention",
     "response",
 ]
 
 # Union type of all types of all Caracara modules providing policy data
 # They all expose a common API, so can be assumed to be one type where convenient
-PoliciesAPIModule = Union[
+PoliciesApiModule = Union[
     PreventionPoliciesApiModule,
     ResponsePoliciesApiModule,
 ]
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/policies/container.py` & `falcon_toolkit-3.1.2/falcon_toolkit/policies/container.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/policies/describe.py` & `falcon_toolkit-3.1.2/falcon_toolkit/policies/describe.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/cli.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/cmd_generators/reg.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/reg.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/parsers.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,14 @@
     Cmd2ArgumentParser,
 )
 from falcon_toolkit.common.namespace import FalconRecursiveNamespace
 
 CLOUD_SCRIPT_CHOICES = []
 PUT_FILE_CHOICES = []
 
-# For all commands that take no arguments at all,
-# we can reuse this blank argparser to avoid instantiating
-# lots of empty/blank argparsers objects
-blank_argparser = Cmd2ArgumentParser()
 
 cat_argparser = Cmd2ArgumentParser()
 cat_argparser.add_argument(
     'file',
     help="File to read the contents of",
 )
 
@@ -667,38 +663,38 @@
 )
 
 _PARSERS = {
     "cat": cat_argparser,
     "cd": cd_argparser,
     "cloud_scripts": cloud_scripts_argparser,
     "cp": cp_argparser,
-    "csrutil": blank_argparser,
-    "cswindiag": blank_argparser,
+    "csrutil": Cmd2ArgumentParser(),
+    "cswindiag": Cmd2ArgumentParser(),
     "download": download_argparser,
     "encrypt": encrypt_argparser,
     "env": env_argparser,
     "eventlog": eventlog_argparser,
     "ls": ls_argparser,
     "filehash": filehash_argparser,
     "get": get_argparser,
     "get_status": get_status_argparser,
-    "getsid": blank_argparser,
-    "ifconfig": blank_argparser,
-    "ipconfig": blank_argparser,
+    "getsid": Cmd2ArgumentParser(),
+    "ifconfig": Cmd2ArgumentParser(),
+    "ipconfig": Cmd2ArgumentParser(),
     "kill": kill_argparser,
     "map": map_argparser,
     "memdump": memdump_argparser,
     "mkdir": mkdir_argparser,
     "mount": mount_argparser,
     "mv": mv_argparser,
     "netstat": netstat_argparser,
-    "ps": blank_argparser,
+    "ps": Cmd2ArgumentParser(),
     "put": put_argparser,
     "put_and_run": put_and_run_argparser,
-    "put_files": blank_argparser,
+    "put_files": Cmd2ArgumentParser(),
     "reg": reg_argparser,
     "restart": restart_argparser,
     "rm": rm_argparser,
     "run": run_argparser,
     "runscript": runscript_argparser,
     "shutdown": shutdown_argparser,
     "tar": tar_argparser,
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/prompt.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
         """[Windows] Download and immediately execute a file from the CrowdStrike Cloud."""
         command = f'put-and-run {args.file}'
         self.send_generic_command(command)
 
     @with_argparser(PARSERS.put_files, preserve_quotes=False)
     def do_put_files(self, args):
         """List the PUT files available in the Falcon instance."""
-        put_files = self.client.rtr.query_put_files()
+        put_files = self.client.rtr.describe_put_files()
         sorted_put_files = sorted(
             put_files.items(),
             key=lambda x: x[1]['name'],
         )
         # Since we've made this API call, we might as well update the
         # choices for the parser, too.
         PUT_FILE_CHOICES.clear()
```

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/refresh.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/refresh.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/falcon_toolkit/shell/utils.py` & `falcon_toolkit-3.1.2/falcon_toolkit/shell/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.1/pyproject.toml` & `falcon_toolkit-3.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "falcon-toolkit"
-version = "3.1.1"
+version = "3.1.2"
 description = "Toolkit to interface with CrowdStrike Falcon via the API"
 license = "MIT"
 authors = [
     "Chris Hammond <chris.hammond@crowdstrike.com>",
 ]
 repository = "http://github.com/CrowdStrike/Falcon-Toolkit"
 readme = "README.md"
```

### Comparing `falcon_toolkit-3.1.1/setup.py` & `falcon_toolkit-3.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,446 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: falcon-toolkit
+Version: 3.1.2
+Summary: Toolkit to interface with CrowdStrike Falcon via the API
+Home-page: http://github.com/CrowdStrike/Falcon-Toolkit
+License: MIT
+Keywords: automation,cli,crowdstrike,endpoint-protection,falcon,falcon-platform
+Author: Chris Hammond
+Author-email: chris.hammond@crowdstrike.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Requires-Dist: caracara (>=0.2.2,<0.3.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
+Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
+Requires-Dist: cmd2 (>=2.4,<3.0)
+Requires-Dist: colorama (>=0.4.5,<0.5.0)
+Requires-Dist: keyring (>=23,<24)
+Requires-Dist: pick (>=2.0.2,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Project-URL: Repository, http://github.com/CrowdStrike/Falcon-Toolkit
+Description-Content-Type: text/markdown
 
-packages = \
-['falcon_toolkit',
- 'falcon_toolkit.common',
- 'falcon_toolkit.common.auth_backends',
- 'falcon_toolkit.hosts',
- 'falcon_toolkit.policies',
- 'falcon_toolkit.shell',
- 'falcon_toolkit.shell.cmd_generators']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['caracara>=0.2.2,<0.3.0',
- 'click-option-group>=0.5.3,<0.6.0',
- 'click-spinner>=0.1.10,<0.2.0',
- 'click>=8.1.3,<9.0.0',
- 'cmd2>=2.4,<3.0',
- 'colorama>=0.4.5,<0.5.0',
- 'keyring>=23,<24',
- 'pick>=2.0.2,<3.0.0',
- 'tabulate>=0.9.0,<0.10.0']
-
-entry_points = \
-{'console_scripts': ['falcon = falcon_toolkit.falcon:cli']}
-
-setup_kwargs = {
-    'name': 'falcon-toolkit',
-    'version': '3.1.1',
-    'description': 'Toolkit to interface with CrowdStrike Falcon via the API',
-    'long_description': '<!--markdownlint-disable MD033-->\n# Falcon Toolkit\n\n![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)\n\n[![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)\n![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CrowdStrike/Falcon-Toolkit/Publish%20Python%20Package?label=build%20and%20deploy)\n[![PyPI](https://img.shields.io/pypi/v/Falcon-Toolkit)](https://pypi.org/project/Falcon-Toolkit)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Falcon-Toolkit)\n![OSS Lifecycle](https://img.shields.io/osslifecycle/CrowdStrike/Falcon-Toolkit)\n\n***automate all the things...remotely!***\n\n## What Is This?\n\n*Falcon Toolkit* is an all in one toolkit designed to make your Falcon life much easier. It is built on top of [Caracara](https://github.com/CrowdStrike/caracara).\n\nThe toolkit provides:\n\n- Host searching, with filter support.\n- Multiple profile support, including support for MSSP / Falcon Flight Control configurations.\n- A shell allowing you to interface with many hosts via RTR at once, and get the output via CSV.\n- Scriptability! You can program the shell by providing pre-written routines via a file on disk, and a full Python extensibility API is provided.\n- Prevention policy import and export\n- Response policy import and export\n- More functionality is coming soon! Want more functionality? Open an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new)!\n\nSince this is built on top of Caracara, you get a bunch of great functionality and flexibility free, including the ability to filter hosts using dynamically generated FQL queries, full debug logging where desired, Falcon Flight Control integration, and more! Plus, the tool is lightning quick as it leverages Caracara\'s parallelisation tricks to pull more information quickly.\n\n## Getting Started\n\nThere are two supported methods to install Falcon Toolkit.\n\n<details>\n<summary>\n<h3>Recommended for Most Users: <code>pipx</code></h3>\n</summary>\n\n### Installing Falcon Toolkit with `pipx`\n\n[`pipx`](https://pypa.github.io/pipx/) is a tool published the Python Packaging Authority to ease the install of Python tools. It will automatically configure you a virtual environment and make a link the `falcon` command that your shell can work with.\n\nFollow the instructions to install `pipx` and add its `bin` folder to your `PATH` variable. Then, use `pipx` to install the `falcon-toolkit` PyPI package. Your output should look like this:\n\n```shell\n$ pipx install falcon-toolkit\ninstalled package falcon-toolkit 3.0.1, installed using Python 3.11.0\n  These apps are now globally available\n    - falcon\n```\n\nOnce installed, run the `falcon` command to test it.\n\n#### Configuring `readline` when installed via `pipx`\n\nIf you see a message like this, read on...\n\n```shell\n$ falcon\nReadline features including tab completion have been disabled because\nno supported version of readline was found. To resolve this, install\npyreadline3 on Windows or gnureadline on Linux/Mac.\n```\n\nThis is caused by Python installations compiled against a non-supported `readline` library, such as `libedit` on macOS. To fix it, run the following command to install a supported readline library.\n\nWindows:\n\n```shell\n> pipx inject falcon-toolkit pyreadline3\ninjected package pyreadline3 into venv falcon-toolkit\ndone! ✨ 🌟 ✨\n```\n\nLinux or macOS:\n\n```shell\n$ pipx inject falcon-toolkit gnureadline\ninjected package gnureadline into venv falcon-toolkit\ndone! ✨ 🌟 ✨\n```\n\n#### Upgrading Falcon Toolkit when installed via `pipx`\n\nWhen installed via `pipx`, you can upgrade Falcon Toolkit by simply running:\n\n```shell\n$ pipx upgrade falcon-toolkit\nfalcon-toolkit is already at latest version 3.0.1\n```\n\n</details>\n\n<details>\n<summary>\n<h3>Installing via Poetry (Recommended for Developers and Maintainers)</h3>\n</summary>\n\nThis tool is built using [Poetry](https://python-poetry.org) and Python 3. Therefore, you must first ensure that you have both Poetry and Python 3.9+ installed to make use of this tool. Ensure you pay attention to Step 3 of the [Poetry installation instructions](https://python-poetry.org/docs/master/#installing-with-the-official-installer) so that you get Poetry added to your shell\'s `PATH` variable.\n\nOnce Poetry is installed and loaded in your shell, simply clone this repository from GitHub and run `poetry install` within the `Falcon-Toolkit` directory to get all the necessary requirements set up in a virtual environment.\n\nNext, run  `poetry shell` to enter the virtual environment.\n\nFinally, run the `falcon` command to get started! If this succeeds and you get some help output, you\'re ready to go.\n\nIf you close your shell, simply run `poetry shell` to get back in to the virtual environment. This will bring back the `falcon` command.\n\n#### Configuring `readline` when installed via Poetry\n\nIf you see a message like this, read on...\n\n```shell\n$ falcon\nReadline features including tab completion have been disabled because\nno supported version of readline was found. To resolve this, install\npyreadline3 on Windows or gnureadline on Linux/Mac.\n```\n\nThis is caused by Python installations compiled against a non-supported `readline` library, such as `libedit` on macOS. To fix it, run the following commands to install a supported readline library.\n\nWindows:\n\n```shell\n# Enter the Poetry virtual environment\n> poetry shell\n\n# Install pyreadline3 in the virtual environment\n> pip install pyreadline3\n```\n\nLinux or macOS:\n\n```shell\n# Enter the Poetry virtual environment\n$ poetry shell\n\n# Install gnureadline in the virtual environment\n$ pip install gnureadline\n```\n\n#### Upgrading Falcon Toolkit when installed via Poetry\n\nWhen installed via Poetry, you have to follow two steps to upgrade the tool. First update your local copy of the Git repository, then install the updated dependencies.\n\n```shell\n# Update the code\n$ git pull\n\n# Update the requirements\n$ poetry install\n\n# Enter the virtual environment if you are not already in it\n$ poetry shell\n\n# Run Falcon Toolkit\n$ falcon\n```\n\n</details>\n\n## Profile Management\n\nFalcon Toolkit requires you to pre-configure profiles, consisting of:\n\n- A name (such as for a client or Falcon tenant);\n- An optional description;\n- A Falcon API client ID;\n- A corresponding Falcon API client secret; and\n- Optionally, the desired cloud, although this can be automatically figured out based on magic provided by [FalconPy](https://falconpy.io) provided you are not a GovCloud customer.\n\nOnce these options are configured, you do not need to specify a client ID/secret again for communicating with that client. The configurations are saved in the file `~/FalconToolkit/FalconToolkit.json`, and the client secret for each corresponding client ID is stored in your host\'s local secure storage environment (e.g., via DPAPI on Windows, the Keychain on macOS, or Gnome\'s secret store on Linux). This keeps your client secrets secure and encrypted using your logon password.\n\n### Creating a New Profile\n\nThe command\xa0`falcon profiles new` will guide you through creating a new configuration. Note that:\n\n- The name you specify will be the one you use to start a shell, so if you put a space in it remember that you\'ll need to wrap it in quotes later. Therefore, we do not recommend using a space here.\n- The client ID and secret you specify must have full RTR admin and host querying permissions enabled; otherwise, this tool will not be able to execute any commands.\n\nTwo types of configuration backends are provided out of the box: the default, which is for an API keypair associated with a standard Falcon tenant, and a Falcon Flight Control backend. Use the Flight Control backend when authenticating to a Parent CID, as you will be able to specify the desired child CID on execution.\n\nYour API keys should have the following scopes enabled in the Falcon dashboard:\n\n| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  |\n|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|\n| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* |\n| **Hosts: Read**                      |       X       |    X    |                            |                           |\n| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |\n| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |\n| **Real Time Response: Read**         |               |    X    |                            |                           |\n| **Real Time Response: Write**        |               |    X    |                            |                           |\n| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |\n| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |\n| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |\n\n### Showing Your Profiles\n\nThe command `falcon profiles list` will show you all configurations (if any) you have created using the `new` command above, listed by the name you specified.\n\nExample output:\n\n```shell\n$ falcon profiles list\nFalcon Toolkit\nConfiguration Directory: /Users/username/FalconToolkit\nFalcon Instance Configurations\nServicesTest\n    Test instance for Services\n```\n\n### Deleting a Profile\n\nThe command `falcon profiles delete [Profile Name]` will delete a configuration for you. Use the name you defined when you created the profile via `falcon profiles new`.\n\n### Selecting a Profile\n\nIf you have configured one profile, Falcon Toolkit will use it by default. If you have multiple profiles, you must select one using `-p`, like this:\n\n```shell\n$ falcon -p Profile2 <command> <command-specific params>\nFalcon Toolkit\n...\n```\n\n## Listing Filters\n\nA key part of this tool (as we\'ll see later) is filter support. To see what filters are supported by the Falcon Toolkit and FalconPy, run `falcon filters`. Each filter is listed and explained with examples.\n\n## Host Search\n\nBefore jumping into an RTR shell, you may wish to see which hosts you would connect to if you used the `shell` command (covered below). To do so, use the `falcon host_search` command.\n\nAs with the `shell` command, you must specify a profile (the name of a configuration you created using the `new` command above) if you have created more than one, and you can then optionally provide as many filters as you want using succesive `-f` switches. Some examples:\n\nList all Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.\n\n```shell\nfalcon host_search -f OS=Windows -f Site__NOT=London\n```\n\nList all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, wihtin the `MyCompany` Falcon tenant.\n\n```shell\nfalcon -p MyCompany host_search -f OS=Windows -f GroupID__NOT=075e03f5e5c04d83b4831374e7dc01c3\n```\n\nList all `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`\n\n```shell\nfalcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected\n```\n\nList all `MyOtherCompany` Windows Workstations that have checked in to Falcon within the past 30 minutes\n\n```shell\nfalcon -p MyOtherCompany host_search -f OS=Windows -f Role=Workstation -f LastSeen__GTE=-30m\n```\n\n## Jump into an RTR Shell\n\nNow that you know how to filter, you know how to jump into a shell! To get into a batch shell with no special options, just do the same as for a `host_search` but use the `shell` command instead. For example, to launch an RTR shell with all Windows hosts last seen within the past 30 minutes within the `MyCompany` Falcon instance, use this command:\n\n```shell\nfalcon -p MyCompany shell -f OS=Windows -f LastSeen__GTE=-30m\n```\n\nYou can also specify an initial timeout to use for all RTR commands. By default, the timeout is 30 seconds, but you can change this to, e.g., 60 seconds, like this:\n\n```shell\nfalcon -p MyCompany shell -f OS=Windows -t 60\n```\n\nOnce you are within an RTR shell, you can run any command that you can run within standard RTR, with full usage, tab completion and examples. However, note that some commands (such as `reg` and `runscript`) have been slightly adjusted in their usage to match standard Unix command patterns. There are technical reasons for this; reach out to us if you need support. Furthermore, some commands have been augmented or added, such as `runscript -WorkstationPath` which allows you to run a local script without making it a cloud file first, `get_status` to check on file uploads, and `download` to pull files retrieved via `get` down to your local system.\n\nYou can run `help` at any time within the shell to get a list of commands. Every command also supports the `-h` switch to find out how it works. Run `quit` at any time to get back to your command line.\n\nAll outputs are written to a log file, as well as a CSV alongside it showing the output from every host. If you run this tool against many hosts, you will see the output from the first in the list on screen. However, every host\'s output (from `stdout` and `stderr`) is written to the accompanying CSV.\n\nAll logs and CSVs are written to the `logs` folder within your configuration directory (default: `~/FalconToolkit`).\n\n### Specifying Hosts by ID\n\nAlthough Falcon Toolkit provides you with plenty of filtering options, sometimes you may wish to connect to hosts by Agent ID (AID) / Device ID. You can do this using two command line options.\n\n#### Specifying Device IDs at the Command Line: The `-d` Option\n\nTo specify Device IDs at the command line, simply provide the `--device-id-list` / `-d` option and a comma-delimited list of IDs. For example, to connect to two hosts with the AIDs `abcdef12345` and `ghijkl67890`, you could use the following command:\n\n```shell\nfalcon -p ProfileName shell -d abcdef12345,ghijkl67890\n```\n\n#### Specifying a File Containing Device IDs: The `-df` Option\n\nSometimes it is not practical to provide a list of Device IDs at the command line, often because the length of the string containing all the IDs would exceed the maximum command length allowable within your shell. To get around this, Falcon Toolkit provides another parameter (`--device-id-file` / `-df`), which allows you to provide a path to a file containing a list of AIDs, one per line. For example, let\'s say you wanted to connect to two devices with the AIDs `abcdef12345` and `ghijkl67890`, you may have a file named `device_ids.txt` with the following contents:\n\n```text\nabcdef12345\nghijkl67890\n```\n\nThen, you could jump into a shell with these devices via this Falcon Toolkit command:\n\n```shell\nfalcon -p ProfileName shell -df device_ids.txt\n```\n\n### Real Time Response (RTR) Scripting\n\nThe RTR shell is fully scriptable. There are two different scripting methods supported:\n\n- Command replay scripts that simulate a human typing commands into the shell; and\n- Python scripts that can interact with the shell programmatically at runtime.\n\n<details>\n<summary>\n<h4>Command Replay Script</h4>\n</summary>\n\nIf you have a file on disk with all shell commands you wish to run, you can specify it as a command line switch:\n\n```shell\nfalcon shell -f OS=Windows -s script.rtr\n```\n\nThis would run a script from disk called `script.rtr`. Scripts should end in the `quit` command if you do not wish to run further commands after your script has run (and therefore return to the shell).\n\nNote that scripts contain a list of shell commands, *not* a list of zsh/PowerShell commands. Therefore, if you need to run a raw script command, write a script containing content like this:\n\n```shell\nrunscript -Raw "Get-ChildItem"\nquit\n```\n\n</details>\n\n<details>\n<summary>\n<h4>Python Scripting API</h4>\n</summary>\n\nThis tool is build on top of the excellent [Cmd2](https://cmd2.readthedocs.io/) Python library, which brings with it copious extensibility. It is possible to write Python scripts that run within the context of the Toolkit\'s shell with programmatic logic applied. This feature is very much in beta, and we are actively seeking feedback on which state data should be made available globally to aid in programmatic scripting of the shell.\n\nInformation on Cmd2\'s scripting backend is provided [here](https://cmd2.readthedocs.io/en/stable/features/scripting.html#python-scripts). The backend is configured as follows:\n\n- The RTR Shell\'s application [bridge name](https://cmd2.readthedocs.io/en/stable/features/scripting.html#basics) is `rtr`, so `rtr("runscript -Raw \\"Get-ChildItem\\"")` would execute the `Get-ChildItem` PowerShell command against all connected systems from within a custom PyScript.\n- The `self` functionality is enabled, enabling developers to introspect data stored within the RTR Shell itself. In this context, `self` will refer to the instantiated `RTRPrompt` object defined in `falcon_toolkit/shell/prompt.py`.\n\nSome example usages of this functionality are as follows:\n\n- Execute a batch `get` command and then cache the contents of `self.last_batch_get_successful_requests` to find out how many systems had the file on disk. Then, the script could wait `x` seconds in a loop up to a maximum amount of time, running `get_status` each time. On each iteration, the script may query `self.last_batch_get_completed_uploads` to determine whether a minimum threshold of systems have uploaded the requested file, and then once complete execute `download -e /some/output/folder` to pull those completed uploads down to a folder of choice (then extract them automatically).\n- Execute a series of commands that differ by target OS, using the contents of `self.connected_devices` to make decisions dynamically.\n- Execute `self.send_generic_command` directly, then use the returned `(stdout, stderr)` tuple to make decisions about which command to execute next (best suited to single system connections).\n\n</details>\n\n## Policy Manipulation\n\nYou can `describe`, `import` and `export` two types of policies: Prevention and Response. The three verbs are applied to the `falcon policies` command to specify what you would like to do with policies, and a command line switch is used to specify the policy type to work with. Exported policies are written to disk as JSON with some Falcon Toolkit-specific data needed to import a policy back again.\n\n### Examples\n\nShow all Prevention policies within the `MyCompany` Falcon profile:\n\n```shell\n$ falcon -p MyCompany policies -p describe\nplatform_default (Platform: Windows)\n    Platform default policy\n...\n```\n\nShow all Response policies when only one profile is configured:\n\n```shell\n$ falcon policies -r describe\nplatform_default (Platform: Windows)\n    Platform default policy\n...\n```\n\nExport a Response policy from the `MyCompany` tenant to disk:\n\n```shell\n$ falcon -p MyCompany policies -r export\nPlease choose a policy to export\n\n * My Response Policy [Windows]\n   My Other Response Policy [Linux]\n...\n```\n\nImport a Prevention policy to the one configured Falcon tenant:\n\n```shell\n$ falcon policies -p import MyExportedPolicy.json\n...\n```\n\n## Support & Community Forums\n\nFalcon Toolkit is an open source project, and not a formal CrowdStrike product, designed to assist users with managing their Falcon tenants and executing commands at scale. As such, it carries no formal support, express or implied. This project originated out of the CrowdStrike Services Incident Response (IR) team\'s need to execute commands across Falcon tenants quickly, at scale, and with auditing, and is maintained by [Chris Hammond](mailto:Chris.Hammond@crowdstrike.com).\n\nIs something going wrong? GitHub Issues are used to report bugs. Submit an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new/choose) and let us know what is happening.\n\nFurthermore, GitHub Discussions provide the community with means to communicate.\n\n*Security issues should be raised to our [Security team](mailto:security@crowdstrike.com) and [Chris Hammond](mailto:Chris.Hammond@crowdstrike.com).*\n\nThank you for using the Falcon Toolkit! We hope it is as useful to the Falcon user community as it is to us.\n',
-    'author': 'Chris Hammond',
-    'author_email': 'chris.hammond@crowdstrike.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'http://github.com/CrowdStrike/Falcon-Toolkit',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+<!--markdownlint-disable MD033-->
+# Falcon Toolkit
 
+![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)
+
+[![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CrowdStrike/Falcon-Toolkit/Publish%20Python%20Package?label=build%20and%20deploy)
+[![PyPI](https://img.shields.io/pypi/v/Falcon-Toolkit)](https://pypi.org/project/Falcon-Toolkit)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Falcon-Toolkit)
+![OSS Lifecycle](https://img.shields.io/osslifecycle/CrowdStrike/Falcon-Toolkit)
+
+***automate all the things...remotely!***
+
+## What Is This?
+
+*Falcon Toolkit* is an all in one toolkit designed to make your Falcon life much easier. It is built on top of [Caracara](https://github.com/CrowdStrike/caracara).
+
+The toolkit provides:
+
+- Host searching, with filter support.
+- Multiple profile support, including support for MSSP / Falcon Flight Control configurations.
+- A shell allowing you to interface with many hosts via RTR at once, and get the output via CSV.
+- Scriptability! You can program the shell by providing pre-written routines via a file on disk, and a full Python extensibility API is provided.
+- Prevention policy import and export
+- Response policy import and export
+- More functionality is coming soon! Want more functionality? Open an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new)!
+
+Since this is built on top of Caracara, you get a bunch of great functionality and flexibility free, including the ability to filter hosts using dynamically generated FQL queries, full debug logging where desired, Falcon Flight Control integration, and more! Plus, the tool is lightning quick as it leverages Caracara's parallelisation tricks to pull more information quickly.
+
+## Getting Started
+
+There are two supported methods to install Falcon Toolkit.
+
+<details>
+<summary>
+<h3>Recommended for Most Users: <code>pipx</code></h3>
+</summary>
+
+### Installing Falcon Toolkit with `pipx`
+
+[`pipx`](https://pypa.github.io/pipx/) is a tool published the Python Packaging Authority to ease the install of Python tools. It will automatically configure you a virtual environment and make a link the `falcon` command that your shell can work with.
+
+Follow the instructions to install `pipx` and add its `bin` folder to your `PATH` variable. Then, use `pipx` to install the `falcon-toolkit` PyPI package. Your output should look like this:
+
+```shell
+$ pipx install falcon-toolkit
+installed package falcon-toolkit 3.0.1, installed using Python 3.11.0
+  These apps are now globally available
+    - falcon
+```
+
+Once installed, run the `falcon` command to test it.
+
+#### Configuring `readline` when installed via `pipx`
+
+If you see a message like this, read on...
+
+```shell
+$ falcon
+Readline features including tab completion have been disabled because
+no supported version of readline was found. To resolve this, install
+pyreadline3 on Windows or gnureadline on Linux/Mac.
+```
+
+This is caused by Python installations compiled against a non-supported `readline` library, such as `libedit` on macOS. To fix it, run the following command to install a supported readline library.
+
+Windows:
+
+```shell
+> pipx inject falcon-toolkit pyreadline3
+injected package pyreadline3 into venv falcon-toolkit
+done! ✨ 🌟 ✨
+```
+
+Linux or macOS:
+
+```shell
+$ pipx inject falcon-toolkit gnureadline
+injected package gnureadline into venv falcon-toolkit
+done! ✨ 🌟 ✨
+```
+
+#### Upgrading Falcon Toolkit when installed via `pipx`
+
+When installed via `pipx`, you can upgrade Falcon Toolkit by simply running:
+
+```shell
+$ pipx upgrade falcon-toolkit
+falcon-toolkit is already at latest version 3.0.1
+```
+
+</details>
+
+<details>
+<summary>
+<h3>Installing via Poetry (Recommended for Developers and Maintainers)</h3>
+</summary>
+
+This tool is built using [Poetry](https://python-poetry.org) and Python 3. Therefore, you must first ensure that you have both Poetry and Python 3.9+ installed to make use of this tool. Ensure you pay attention to Step 3 of the [Poetry installation instructions](https://python-poetry.org/docs/master/#installing-with-the-official-installer) so that you get Poetry added to your shell's `PATH` variable.
+
+Once Poetry is installed and loaded in your shell, simply clone this repository from GitHub and run `poetry install` within the `Falcon-Toolkit` directory to get all the necessary requirements set up in a virtual environment.
+
+Next, run  `poetry shell` to enter the virtual environment.
+
+Finally, run the `falcon` command to get started! If this succeeds and you get some help output, you're ready to go.
+
+If you close your shell, simply run `poetry shell` to get back in to the virtual environment. This will bring back the `falcon` command.
+
+#### Configuring `readline` when installed via Poetry
+
+If you see a message like this, read on...
+
+```shell
+$ falcon
+Readline features including tab completion have been disabled because
+no supported version of readline was found. To resolve this, install
+pyreadline3 on Windows or gnureadline on Linux/Mac.
+```
+
+This is caused by Python installations compiled against a non-supported `readline` library, such as `libedit` on macOS. To fix it, run the following commands to install a supported readline library.
+
+Windows:
+
+```shell
+# Enter the Poetry virtual environment
+> poetry shell
+
+# Install pyreadline3 in the virtual environment
+> pip install pyreadline3
+```
+
+Linux or macOS:
+
+```shell
+# Enter the Poetry virtual environment
+$ poetry shell
+
+# Install gnureadline in the virtual environment
+$ pip install gnureadline
+```
+
+#### Upgrading Falcon Toolkit when installed via Poetry
+
+When installed via Poetry, you have to follow two steps to upgrade the tool. First update your local copy of the Git repository, then install the updated dependencies.
+
+```shell
+# Update the code
+$ git pull
+
+# Update the requirements
+$ poetry install
+
+# Enter the virtual environment if you are not already in it
+$ poetry shell
+
+# Run Falcon Toolkit
+$ falcon
+```
+
+</details>
+
+## Profile Management
+
+Falcon Toolkit requires you to pre-configure profiles, consisting of:
+
+- A name (such as for a client or Falcon tenant);
+- An optional description;
+- A Falcon API client ID;
+- A corresponding Falcon API client secret; and
+- Optionally, the desired cloud, although this can be automatically figured out based on magic provided by [FalconPy](https://falconpy.io) provided you are not a GovCloud customer.
+
+Once these options are configured, you do not need to specify a client ID/secret again for communicating with that client. The configurations are saved in the file `~/FalconToolkit/FalconToolkit.json`, and the client secret for each corresponding client ID is stored in your host's local secure storage environment (e.g., via DPAPI on Windows, the Keychain on macOS, or Gnome's secret store on Linux). This keeps your client secrets secure and encrypted using your logon password.
+
+### Creating a New Profile
+
+The command `falcon profiles new` will guide you through creating a new configuration. Note that:
+
+- The name you specify will be the one you use to start a shell, so if you put a space in it remember that you'll need to wrap it in quotes later. Therefore, we do not recommend using a space here.
+- The client ID and secret you specify must have full RTR admin and host querying permissions enabled; otherwise, this tool will not be able to execute any commands.
+
+Two types of configuration backends are provided out of the box: the default, which is for an API keypair associated with a standard Falcon tenant, and a Falcon Flight Control backend. Use the Flight Control backend when authenticating to a Parent CID, as you will be able to specify the desired child CID on execution.
+
+Your API keys should have the following scopes enabled in the Falcon dashboard:
+
+| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  |
+|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|
+| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* |
+| **Hosts: Read**                      |       X       |    X    |                            |                           |
+| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |
+| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |
+| **Real Time Response: Read**         |               |    X    |                            |                           |
+| **Real Time Response: Write**        |               |    X    |                            |                           |
+| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |
+| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |
+| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |
+
+### Showing Your Profiles
+
+The command `falcon profiles list` will show you all configurations (if any) you have created using the `new` command above, listed by the name you specified.
+
+Example output:
+
+```shell
+$ falcon profiles list
+Falcon Toolkit
+Configuration Directory: /Users/username/FalconToolkit
+Falcon Instance Configurations
+ServicesTest
+    Test instance for Services
+```
+
+### Deleting a Profile
+
+The command `falcon profiles delete [Profile Name]` will delete a configuration for you. Use the name you defined when you created the profile via `falcon profiles new`.
+
+### Selecting a Profile
+
+If you have configured one profile, Falcon Toolkit will use it by default. If you have multiple profiles, you must select one using `-p`, like this:
+
+```shell
+$ falcon -p Profile2 <command> <command-specific params>
+Falcon Toolkit
+...
+```
+
+## Listing Filters
+
+A key part of this tool (as we'll see later) is filter support. To see what filters are supported by the Falcon Toolkit and FalconPy, run `falcon filters`. Each filter is listed and explained with examples.
+
+## Host Search
+
+Before jumping into an RTR shell, you may wish to see which hosts you would connect to if you used the `shell` command (covered below). To do so, use the `falcon host_search` command.
+
+As with the `shell` command, you must specify a profile (the name of a configuration you created using the `new` command above) if you have created more than one, and you can then optionally provide as many filters as you want using succesive `-f` switches. Some examples:
+
+List all Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.
+
+```shell
+falcon host_search -f OS=Windows -f Site__NOT=London
+```
+
+List all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, wihtin the `MyCompany` Falcon tenant.
+
+```shell
+falcon -p MyCompany host_search -f OS=Windows -f GroupID__NOT=075e03f5e5c04d83b4831374e7dc01c3
+```
+
+List all `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`
+
+```shell
+falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected
+```
+
+List all `MyOtherCompany` Windows Workstations that have checked in to Falcon within the past 30 minutes
+
+```shell
+falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Workstation -f LastSeen__GTE=-30m
+```
+
+## Jump into an RTR Shell
+
+Now that you know how to filter, you know how to jump into a shell! To get into a batch shell with no special options, just do the same as for a `host_search` but use the `shell` command instead. For example, to launch an RTR shell with all Windows hosts last seen within the past 30 minutes within the `MyCompany` Falcon instance, use this command:
+
+```shell
+falcon -p MyCompany shell -f OS=Windows -f LastSeen__GTE=-30m
+```
+
+You can also specify an initial timeout to use for all RTR commands. By default, the timeout is 30 seconds, but you can change this to, e.g., 60 seconds, like this:
+
+```shell
+falcon -p MyCompany shell -f OS=Windows -t 60
+```
+
+Once you are within an RTR shell, you can run any command that you can run within standard RTR, with full usage, tab completion and examples. However, note that some commands (such as `reg` and `runscript`) have been slightly adjusted in their usage to match standard Unix command patterns. There are technical reasons for this; reach out to us if you need support. Furthermore, some commands have been augmented or added, such as `runscript -WorkstationPath` which allows you to run a local script without making it a cloud file first, `get_status` to check on file uploads, and `download` to pull files retrieved via `get` down to your local system.
+
+You can run `help` at any time within the shell to get a list of commands. Every command also supports the `-h` switch to find out how it works. Run `quit` at any time to get back to your command line.
+
+All outputs are written to a log file, as well as a CSV alongside it showing the output from every host. If you run this tool against many hosts, you will see the output from the first in the list on screen. However, every host's output (from `stdout` and `stderr`) is written to the accompanying CSV.
+
+All logs and CSVs are written to the `logs` folder within your configuration directory (default: `~/FalconToolkit`).
+
+### Specifying Hosts by ID
+
+Although Falcon Toolkit provides you with plenty of filtering options, sometimes you may wish to connect to hosts by Agent ID (AID) / Device ID. You can do this using two command line options.
+
+#### Specifying Device IDs at the Command Line: The `-d` Option
+
+To specify Device IDs at the command line, simply provide the `--device-id-list` / `-d` option and a comma-delimited list of IDs. For example, to connect to two hosts with the AIDs `abcdef12345` and `ghijkl67890`, you could use the following command:
+
+```shell
+falcon -p ProfileName shell -d abcdef12345,ghijkl67890
+```
+
+#### Specifying a File Containing Device IDs: The `-df` Option
+
+Sometimes it is not practical to provide a list of Device IDs at the command line, often because the length of the string containing all the IDs would exceed the maximum command length allowable within your shell. To get around this, Falcon Toolkit provides another parameter (`--device-id-file` / `-df`), which allows you to provide a path to a file containing a list of AIDs, one per line. For example, let's say you wanted to connect to two devices with the AIDs `abcdef12345` and `ghijkl67890`, you may have a file named `device_ids.txt` with the following contents:
+
+```text
+abcdef12345
+ghijkl67890
+```
+
+Then, you could jump into a shell with these devices via this Falcon Toolkit command:
+
+```shell
+falcon -p ProfileName shell -df device_ids.txt
+```
+
+### Real Time Response (RTR) Scripting
+
+The RTR shell is fully scriptable. There are two different scripting methods supported:
+
+- Command replay scripts that simulate a human typing commands into the shell; and
+- Python scripts that can interact with the shell programmatically at runtime.
+
+<details>
+<summary>
+<h4>Command Replay Script</h4>
+</summary>
+
+If you have a file on disk with all shell commands you wish to run, you can specify it as a command line switch:
+
+```shell
+falcon shell -f OS=Windows -s script.rtr
+```
+
+This would run a script from disk called `script.rtr`. Scripts should end in the `quit` command if you do not wish to run further commands after your script has run (and therefore return to the shell).
+
+Note that scripts contain a list of shell commands, *not* a list of zsh/PowerShell commands. Therefore, if you need to run a raw script command, write a script containing content like this:
+
+```shell
+runscript -Raw "Get-ChildItem"
+quit
+```
+
+</details>
+
+<details>
+<summary>
+<h4>Python Scripting API</h4>
+</summary>
+
+This tool is build on top of the excellent [Cmd2](https://cmd2.readthedocs.io/) Python library, which brings with it copious extensibility. It is possible to write Python scripts that run within the context of the Toolkit's shell with programmatic logic applied. This feature is very much in beta, and we are actively seeking feedback on which state data should be made available globally to aid in programmatic scripting of the shell.
+
+Information on Cmd2's scripting backend is provided [here](https://cmd2.readthedocs.io/en/stable/features/scripting.html#python-scripts). The backend is configured as follows:
+
+- The RTR Shell's application [bridge name](https://cmd2.readthedocs.io/en/stable/features/scripting.html#basics) is `rtr`, so `rtr("runscript -Raw \"Get-ChildItem\"")` would execute the `Get-ChildItem` PowerShell command against all connected systems from within a custom PyScript.
+- The `self` functionality is enabled, enabling developers to introspect data stored within the RTR Shell itself. In this context, `self` will refer to the instantiated `RTRPrompt` object defined in `falcon_toolkit/shell/prompt.py`.
+
+Some example usages of this functionality are as follows:
+
+- Execute a batch `get` command and then cache the contents of `self.last_batch_get_successful_requests` to find out how many systems had the file on disk. Then, the script could wait `x` seconds in a loop up to a maximum amount of time, running `get_status` each time. On each iteration, the script may query `self.last_batch_get_completed_uploads` to determine whether a minimum threshold of systems have uploaded the requested file, and then once complete execute `download -e /some/output/folder` to pull those completed uploads down to a folder of choice (then extract them automatically).
+- Execute a series of commands that differ by target OS, using the contents of `self.connected_devices` to make decisions dynamically.
+- Execute `self.send_generic_command` directly, then use the returned `(stdout, stderr)` tuple to make decisions about which command to execute next (best suited to single system connections).
+
+</details>
+
+## Policy Manipulation
+
+You can `describe`, `import` and `export` two types of policies: Prevention and Response. The three verbs are applied to the `falcon policies` command to specify what you would like to do with policies, and a command line switch is used to specify the policy type to work with. Exported policies are written to disk as JSON with some Falcon Toolkit-specific data needed to import a policy back again.
+
+### Examples
+
+Show all Prevention policies within the `MyCompany` Falcon profile:
+
+```shell
+$ falcon -p MyCompany policies -p describe
+platform_default (Platform: Windows)
+    Platform default policy
+...
+```
+
+Show all Response policies when only one profile is configured:
+
+```shell
+$ falcon policies -r describe
+platform_default (Platform: Windows)
+    Platform default policy
+...
+```
+
+Export a Response policy from the `MyCompany` tenant to disk:
+
+```shell
+$ falcon -p MyCompany policies -r export
+Please choose a policy to export
+
+ * My Response Policy [Windows]
+   My Other Response Policy [Linux]
+...
+```
+
+Import a Prevention policy to the one configured Falcon tenant:
+
+```shell
+$ falcon policies -p import MyExportedPolicy.json
+...
+```
+
+## Support & Community Forums
+
+Falcon Toolkit is an open source project, and not a formal CrowdStrike product, designed to assist users with managing their Falcon tenants and executing commands at scale. As such, it carries no formal support, express or implied. This project originated out of the CrowdStrike Services Incident Response (IR) team's need to execute commands across Falcon tenants quickly, at scale, and with auditing, and is maintained by [Chris Hammond](mailto:Chris.Hammond@crowdstrike.com).
+
+Is something going wrong? GitHub Issues are used to report bugs. Submit an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new/choose) and let us know what is happening.
+
+Furthermore, GitHub Discussions provide the community with means to communicate.
+
+*Security issues should be raised to our [Security team](mailto:security@crowdstrike.com) and [Chris Hammond](mailto:Chris.Hammond@crowdstrike.com).*
+
+Thank you for using the Falcon Toolkit! We hope it is as useful to the Falcon user community as it is to us.
 
-setup(**setup_kwargs)
```


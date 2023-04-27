# Comparing `tmp/pyiaacsync-0.4.tar.gz` & `tmp/pyiaacsync-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiaacsync-0.4.tar", last modified: Tue Mar 21 13:37:23 2023, max compression
+gzip compressed data, was "dist/pyiaacsync-0.5.tar", last modified: Thu Apr 27 00:30:14 2023, max compression
```

## Comparing `pyiaacsync-0.4.tar` & `pyiaacsync-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-03-21 13:37:23.000000 pyiaacsync-0.4/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     5059 2023-03-21 13:37:23.000000 pyiaacsync-0.4/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)     4004 2023-03-21 13:34:45.000000 pyiaacsync-0.4/README.md
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync/
--rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.4/pyiaacsync/__init__.py
--rw-r--r--   0 manasbellani   (501) wheel        (0)    13408 2023-03-21 13:20:32.000000 pyiaacsync-0.4/pyiaacsync/pyiaacsync.py
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     5059 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)      235 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/SOURCES.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/dependency_links.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/requires.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2023-03-21 13:37:23.000000 pyiaacsync-0.4/pyiaacsync.egg-info/top_level.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2023-03-21 13:37:23.000000 pyiaacsync-0.4/setup.cfg
--rw-r--r--   0 manasbellani   (501) wheel        (0)      864 2023-03-21 13:37:17.000000 pyiaacsync-0.4/setup.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-04-27 00:30:14.000000 pyiaacsync-0.5/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5688 2023-04-27 00:30:14.000000 pyiaacsync-0.5/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     4585 2023-04-26 04:33:24.000000 pyiaacsync-0.5/README.md
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.5/pyiaacsync/__init__.py
+-rw-r--r--   0 manasbellani   (501) wheel        (0)    13875 2023-04-27 00:29:31.000000 pyiaacsync-0.5/pyiaacsync/pyiaacsync.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5688 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      235 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/requires.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2023-04-27 00:30:14.000000 pyiaacsync-0.5/pyiaacsync.egg-info/top_level.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2023-04-27 00:30:14.000000 pyiaacsync-0.5/setup.cfg
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      864 2023-04-26 04:34:15.000000 pyiaacsync-0.5/setup.py
```

### Comparing `pyiaacsync-0.4/PKG-INFO` & `pyiaacsync-0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pyiaacsync
-Version: 0.4
+Version: 0.5
 Summary: Deploy infrastructure as code via polling
 Home-page: https://github.com/manasmbellani/pyiaacsync
 License: UNKNOWN
 Description: # PyIAACSync
         
         ## Introduction
-        infrastructure-as-code tools such as Terraform and Palumi gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
+        infrastructure-as-code tools such as Terraform and Palumi are gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
         
         However, there are a couple of disadvantages in existing tools in the market:
         - Terraform requires knowledge of golang to be able to sync assets
-        - Both Terraform and Paulmi can be quite complex for beginners to manage and maintain
+        - Both Terraform and Palumi plugins can be quite complex for beginners to manage and maintain - As in 2023, Terraform plugins require modules to be built in golang
+        - In a shared environment, where some assets are being built manually while others are being built using automation, tools like Terraform Automation can fail if assets managed by automation are deleted
         
-        PyIAACSync provides a framework which allows software engineering getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that 
+        PyIAACSync provides a framework which allows software engineering teams getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue components can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that can be:
+            a. described in YAML files, and 
+            b. can be read, created or deleted via API calls
         
-        Software engineers need to create the following:
+        Software engineers need to create the following to leverage `pyiaacsync`:
         1. A folder (`iaac_sync_folder`) that contains the specs/configs for the infrastructure to create
         2. A simple asset python file that contains a class describing the asset with the following `static` functions:
            - validate: to validate whether the spec/config that has been supplied in the 
            - create: to create the asset via the supplied spec/config
            - delete: to delete that has been supplied via the spec/config
            - check: to check whether the asset that has been deployed matches the spec/config aka `integrity check`. If not, the asset will be re-created
         
@@ -101,10 +104,13 @@
         To delete all existing assets (in this case, all files) and remove the assets from the state file:
         ```
         python3 example.py -a delete_assets
         ```
         
         ## TODO
         - Add unit testing
+        - Fix the comments for create asset
+        - Fix the bug in deleteasset
+        - Add an assumption: Assuming that the API works ok - every action performed once (no retry)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyiaacsync-0.4/README.md` & `pyiaacsync-0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # PyIAACSync
 
 ## Introduction
-infrastructure-as-code tools such as Terraform and Palumi gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
+infrastructure-as-code tools such as Terraform and Palumi are gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
 
 However, there are a couple of disadvantages in existing tools in the market:
 - Terraform requires knowledge of golang to be able to sync assets
-- Both Terraform and Paulmi can be quite complex for beginners to manage and maintain
+- Both Terraform and Palumi plugins can be quite complex for beginners to manage and maintain - As in 2023, Terraform plugins require modules to be built in golang
+- In a shared environment, where some assets are being built manually while others are being built using automation, tools like Terraform Automation can fail if assets managed by automation are deleted
 
-PyIAACSync provides a framework which allows software engineering getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that 
+PyIAACSync provides a framework which allows software engineering teams getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue components can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that can be:
+    a. described in YAML files, and 
+    b. can be read, created or deleted via API calls
 
-Software engineers need to create the following:
+Software engineers need to create the following to leverage `pyiaacsync`:
 1. A folder (`iaac_sync_folder`) that contains the specs/configs for the infrastructure to create
 2. A simple asset python file that contains a class describing the asset with the following `static` functions:
    - validate: to validate whether the spec/config that has been supplied in the 
    - create: to create the asset via the supplied spec/config
    - delete: to delete that has been supplied via the spec/config
    - check: to check whether the asset that has been deployed matches the spec/config aka `integrity check`. If not, the asset will be re-created
 
@@ -95,7 +98,10 @@
 To delete all existing assets (in this case, all files) and remove the assets from the state file:
 ```
 python3 example.py -a delete_assets
 ```
 
 ## TODO
 - Add unit testing
+- Fix the comments for create asset
+- Fix the bug in deleteasset
+- Add an assumption: Assuming that the API works ok - every action performed once (no retry)
```

### Comparing `pyiaacsync-0.4/pyiaacsync/pyiaacsync.py` & `pyiaacsync-0.5/pyiaacsync/pyiaacsync.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             asset (object): A class that represents the asset to sync. The asset is an class which defines the validate, check, 
                 create, delete methods
             conf_file_extensions (list, optional): List of extensions in iaac_sync_folder. Defaults to CONFIG_FILE_EXTENSIONS.
             init (bool, optional): Initialize the state file only. Defaults to False.
             init_state_file (str, optional): An optional initial state file to use when performing initialize. Defaults to None.
             init_force (bool, optional): Force initialization even if init file exists. Defaults to False.
             delete_all_only (bool, optional): Delete all the assets that have been created and clean the state file. Defaults to `False`.
-            validate_configs_only (bool, optional): _description_. Defaults to False.
+            validate_configs_only (bool, optional): Whether to only validate the configs (not execute any syncing). Defaults to False.
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
         """
         self.iaac_sync_folder = iaac_sync_folder
         self.state_file = state_file
         self.asset = asset
         self.conf_file_extensions = conf_file_extensions
         self.state = {}
@@ -112,22 +112,28 @@
     def __delete_assets(self, **args):
         """Delete all the assets that have been previously created, and update state file
 
         Args:
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
         """
         if self.read_state():
-            if self.state:
-                state_config_paths = list(self.state.keys())
-                for config_path in state_config_paths:
-                    asset_id = self.state[config_path].get('asset_id', None)
-                    if self.asset.delete(asset_id, **args):
-                        # Remove the asset tracking from the state since it is no longer being tracked in git
-                        del self.state[config_path]
-                        
+            try:
+                if self.state:
+                    state_config_paths = list(self.state.keys())
+                    for config_path in state_config_paths:
+                        asset_id = self.state[config_path].get('asset_id', None)
+                        if self.asset.delete(asset_id, **args):
+                            # Remove the asset tracking from the state since it is no longer being tracked in git
+                            del self.state[config_path]
+            except Exception as e:
+                # Ensure that the current state is written back irrespective of exception that occurs
+                self.write_state()
+                # Re-raise the error
+                raise
+                
             self.write_state()
 
     def __validate_configs(self, **args):
         """Simply validate ALL configurations that exist in config files in IAAC Sync folder
 
         Args:
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
@@ -162,86 +168,103 @@
         Raises:
             FileNotFoundException: When the state file is not found
             ConfigFileInvalidSyntax: If config spec file's content is deemed invalid
         """
         all_config_files = []
         
         if self.read_state():
-            
-            # Loop through each config fie in the IAAC Sync folder
-            for dir_path, _, files in os.walk(self.iaac_sync_folder):
-
-                for f in files:
-                    
-                    # Work only with the conf files
-                    if any([f.endswith(ext) for ext in self.conf_file_extensions]):
-                        
-                        config_path = os.path.join(dir_path, f)
-
-                        # Keep track of ALL the asset config files
-                        all_config_files.append(config_path)
+            try:
+                # Loop through each config fie in the IAAC Sync folder
+                for dir_path, _, files in os.walk(self.iaac_sync_folder):
 
-                        # Calculate the hash for config which will be checked to see if they have changed
-                        config_hash = self.__calculate_hash(config_path)
-                        state_conf = self.state.get(config_path, None)
+                    for f in files:
                         
-                        # Get the hash of existing assets. If it doesn't exist then 
-                        state_hash = ''
-                        asset_id = ''
-                        if state_conf:
-                            state_hash = state_conf['hash']
-                            asset_id = state_conf['asset_id']
-                        else:
-                            self.state[config_path] = {
-                                'asset_id': '',
-                                'hash': '',
-                            }
-
-                        # Read the config from file
-                        config = ''
-                        try:
-                            with open(config_path, "r") as f:
-                                config = yaml.safe_load(f)
-                        except Exception as e:
-                            raise ConfigFileInvalidSyntax(f"Config file: {config_path} syntax invalid. Error: {e.__class__}, {e}")
-
-                        # Validate whether the config is correctly provided before syncing
-                        if config:
-                            if self.asset.validate(config, **args):
-                                
-                                # Checking if the asset that currently exists matches the config in 'git'
-                                is_asset_in_sync = True
-                                if asset_id:
-                                    is_asset_in_sync = self.asset.check(asset_id, config, **args)
+                        # Work only with the conf files
+                        if any([f.endswith(ext) for ext in self.conf_file_extensions]):
+                            
+                            config_path = os.path.join(dir_path, f)
+
+                            # Keep track of ALL the asset config files
+                            all_config_files.append(config_path)
+
+                            # Calculate the hash for config which will be checked to see if they have changed
+                            config_hash = self.__calculate_hash(config_path)
+                            state_conf = self.state.get(config_path, None)
+                            
+                            # Get the hash of existing assets. If it doesn't exist then 
+                            state_hash = ''
+                            asset_id = ''
+                            if state_conf:
+                                state_hash = state_conf['hash']
+                                asset_id = state_conf['asset_id']
+                            else:
+                                self.state[config_path] = {
+                                    'asset_id': '',
+                                    'hash': '',
+                                }
+
+                            # Read the config from file
+                            config = ''
+                            try:
+                                with open(config_path, "r") as f:
+                                    config = yaml.safe_load(f)
+                            except Exception as e:
+                                self.write_state()
+                                raise ConfigFileInvalidSyntax(f"Config file: {config_path} syntax invalid. Error: {e.__class__}, {e}")
+
+                            # Validate whether the config is correctly provided before syncing
+                            if config:
+                                if self.asset.validate(config, **args):
+                                    
+                                    # Checking if the asset that currently exists matches the config in 'git'
+                                    is_asset_in_sync = True
+                                    if asset_id:
+                                        is_asset_in_sync = self.asset.check(asset_id, config, **args)
 
-                                # If the spec file has changed OR is brand new, then create the asset again
-                                if (not state_hash) or (state_hash != config_hash) or not is_asset_in_sync:
+                                    # If the spec file has changed OR is brand new, then re-create the asset (delete, then create)
+                                    if (not state_hash) or (state_hash != config_hash) or not is_asset_in_sync:
 
-                                    # Recreate the asset
-                                    asset_id =  self.__recreate_asset(config_path, asset_id, config, **args)
+                                        # Recreate the asset by first attempting to delete it
+                                        if asset_id:
+                                            if self.asset.delete(asset_id, **args):
+                                                if config_path in self.state:
+                                                    # Update the state file that asset has been deleted
+                                                    del self.state[config_path]
+                                            else:
+                                                raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
+                                            
+                                        # Try to create the asset again now
+                                        asset_id = self.asset.create(config, **args)
+                                        if asset_id:
+                                            if config_path not in self.state:
+                                                self.state[config_path] = {}
+                                            # Update the state file with the hash and the new asset ID created
+                                            self.state[config_path]['hash'] = config_hash
+                                            self.state[config_path]['asset_id'] = asset_id
 
-                                    if asset_id:
-                                        # Update the state file with the hash and the new asset ID created
-                                        self.state[config_path]['hash'] = config_hash
-                                        self.state[config_path]['asset_id'] = asset_id 
-
-            # Delete any assets which are not in the config spec (git)
-            if self.state:
-
-                # Read all the config spec keys and loop through them
-                state_config_paths = list(self.state.keys())
-                for config_path in state_config_paths:
+                                        if not asset_id:
+                                            raise AssetNotCreatedException(f"Asset with config in file {config_path} could not be created")
+            
+                # Delete any assets which are not in the config spec (git)
+                if self.state:
 
-                    # Check if any are not in the config specs
-                    if config_path not in all_config_files:
-                        asset_id = self.state[config_path].get('asset_id', None)
-                        if asset_id:
-                            if self.asset.delete(asset_id, **args):
-                                # Remove the asset tracking from the state since it is no longer being tracked in git
-                                del self.state[config_path]
+                    # Read all the config spec keys and loop through them
+                    state_config_paths = list(self.state.keys())
+                    for config_path in state_config_paths:
+
+                        # Check if any are not in the config specs
+                        if config_path not in all_config_files:
+                            asset_id = self.state[config_path].get('asset_id', None)
+                            if asset_id:
+                                if self.asset.delete(asset_id, **args):
+                                    # Remove the asset tracking from the state since it is no longer being tracked in git
+                                    del self.state[config_path]
+            except Exception as e:
+                self.write_state()
+                raise
 
             self.write_state()
 
         else:
             raise FileNotFoundException(f"State file: {self.state_file} not found. Was file init or state file not copied")
 
     def __calculate_hash(self, file_path):
@@ -260,41 +283,8 @@
         if os.path.isfile(file_path):
             with open(file_path,"rb") as f:
                 bytes = f.read()
                 readable_hash = hashlib.sha256(bytes).hexdigest()
         else:
             raise FileNotFoundException(f"File: {file_path} not found")
 
-        return readable_hash
-
-    def __recreate_asset(self, file_path, existing_asset_id, config, **args):
-        """Recreate (delete and create) an asset based on the 
-
-        Args:
-            file_path (str): File path to the config file (to be used when printing error messages)
-            existing_asset_id (str): Existing asset ID to delete
-            config (str): Config  representing the object
-            args (dict): Any additional optional args which would get passed to the methods defined in the asset class
-
-        Returns:
-            str: ID of the asset that was created successfully, otherwise None.
-
-        Raises:
-            AssetNotCreatedException: If the asset could not be created
-            AssetNotDeletedException: If the asset could not be deleted
-        """
-        asset_id = None
-
-        if existing_asset_id:
-            if self.asset.delete(existing_asset_id, **args):
-                asset_id = self.asset.create(config, **args)
-            else:
-                raise AssetNotDeletedException(f"Asset with config in file {file_path} could not be deleted")
-            
-        else:
-            asset_id = self.asset.create(config, **args)
-
-            if not asset_id:
-                raise AssetNotCreatedException(f"Asset with config in file {file_path} could not be created")
-            
-        return asset_id
-
+        return readable_hash
```

### Comparing `pyiaacsync-0.4/pyiaacsync.egg-info/PKG-INFO` & `pyiaacsync-0.5/pyiaacsync.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pyiaacsync
-Version: 0.4
+Version: 0.5
 Summary: Deploy infrastructure as code via polling
 Home-page: https://github.com/manasmbellani/pyiaacsync
 License: UNKNOWN
 Description: # PyIAACSync
         
         ## Introduction
-        infrastructure-as-code tools such as Terraform and Palumi gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
+        infrastructure-as-code tools such as Terraform and Palumi are gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
         
         However, there are a couple of disadvantages in existing tools in the market:
         - Terraform requires knowledge of golang to be able to sync assets
-        - Both Terraform and Paulmi can be quite complex for beginners to manage and maintain
+        - Both Terraform and Palumi plugins can be quite complex for beginners to manage and maintain - As in 2023, Terraform plugins require modules to be built in golang
+        - In a shared environment, where some assets are being built manually while others are being built using automation, tools like Terraform Automation can fail if assets managed by automation are deleted
         
-        PyIAACSync provides a framework which allows software engineering getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that 
+        PyIAACSync provides a framework which allows software engineering teams getting into infrastructure-as-code to easily create and sync assets which they have defined in YAML spec files, in a polled manner (non-event driven). The infrastructue components can be `anything` (AWS asset, GCP asset, any SIEM detection rule) that can be:
+            a. described in YAML files, and 
+            b. can be read, created or deleted via API calls
         
-        Software engineers need to create the following:
+        Software engineers need to create the following to leverage `pyiaacsync`:
         1. A folder (`iaac_sync_folder`) that contains the specs/configs for the infrastructure to create
         2. A simple asset python file that contains a class describing the asset with the following `static` functions:
            - validate: to validate whether the spec/config that has been supplied in the 
            - create: to create the asset via the supplied spec/config
            - delete: to delete that has been supplied via the spec/config
            - check: to check whether the asset that has been deployed matches the spec/config aka `integrity check`. If not, the asset will be re-created
         
@@ -101,10 +104,13 @@
         To delete all existing assets (in this case, all files) and remove the assets from the state file:
         ```
         python3 example.py -a delete_assets
         ```
         
         ## TODO
         - Add unit testing
+        - Fix the comments for create asset
+        - Fix the bug in deleteasset
+        - Add an assumption: Assuming that the API works ok - every action performed once (no retry)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyiaacsync-0.4/setup.py` & `pyiaacsync-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Read the description from the markdown file
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name="pyiaacsync",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     install_requires=requirements,
     description=project_description,
     long_description=description,
     long_description_content_type="text/markdown",
     url=get_git_remote_url()
 )
```


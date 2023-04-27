# Comparing `tmp/redshift-user-manager-0.1.2.tar.gz` & `tmp/redshift-user-manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift-user-manager-0.1.2.tar", last modified: Thu Apr 27 16:26:31 2023, max compression
+gzip compressed data, was "redshift-user-manager-0.1.3.tar", last modified: Thu Apr 27 17:17:55 2023, max compression
```

## Comparing `redshift-user-manager-0.1.2.tar` & `redshift-user-manager-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 16:26:31.922719 redshift-user-manager-0.1.2/
--rw-r--r--   0 henryjones   (501) staff       (20)    35147 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/LICENSE
--rw-r--r--   0 henryjones   (501) staff       (20)     6096 2023-04-27 16:26:31.922352 redshift-user-manager-0.1.2/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)     5300 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/README.md
--rw-r--r--   0 henryjones   (501) staff       (20)     1035 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/pyproject.toml
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 16:26:31.919489 redshift-user-manager-0.1.2/redshift_user_manager/
--rw-r--r--   0 henryjones   (501) staff       (20)      112 2023-04-27 16:13:34.000000 redshift-user-manager-0.1.2/redshift_user_manager/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)    11125 2023-04-27 16:24:56.000000 redshift-user-manager-0.1.2/redshift_user_manager/cli.py
--rw-r--r--   0 henryjones   (501) staff       (20)      249 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/redshift_user_manager/constants.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1480 2023-04-27 14:20:50.000000 redshift-user-manager-0.1.2/redshift_user_manager/exceptions.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/redshift_user_manager/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)    20976 2023-04-27 16:25:47.000000 redshift-user-manager-0.1.2/redshift_user_manager/redshift_user_manager.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 16:26:31.921539 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)     6096 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      525 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       61 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       45 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       22 2023-04-27 16:26:31.000000 redshift-user-manager-0.1.2/redshift_user_manager.egg-info/top_level.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-04-27 16:26:31.922840 redshift-user-manager-0.1.2/setup.cfg
--rw-r--r--   0 henryjones   (501) staff       (20)      711 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.2/setup.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 17:17:55.121128 redshift-user-manager-0.1.3/
+-rw-r--r--   0 henryjones   (501) staff       (20)    35147 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/LICENSE
+-rw-r--r--   0 henryjones   (501) staff       (20)     6096 2023-04-27 17:17:55.120810 redshift-user-manager-0.1.3/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)     5300 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/README.md
+-rw-r--r--   0 henryjones   (501) staff       (20)     1035 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/pyproject.toml
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 17:17:55.117998 redshift-user-manager-0.1.3/redshift_user_manager/
+-rw-r--r--   0 henryjones   (501) staff       (20)      112 2023-04-27 16:57:34.000000 redshift-user-manager-0.1.3/redshift_user_manager/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    11369 2023-04-27 16:43:46.000000 redshift-user-manager-0.1.3/redshift_user_manager/cli.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      249 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/redshift_user_manager/constants.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1480 2023-04-27 14:20:50.000000 redshift-user-manager-0.1.3/redshift_user_manager/exceptions.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/redshift_user_manager/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)    21103 2023-04-27 17:04:42.000000 redshift-user-manager-0.1.3/redshift_user_manager/redshift_user_manager.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-04-27 17:17:55.120356 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)     6096 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      525 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       61 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       45 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       22 2023-04-27 17:17:55.000000 redshift-user-manager-0.1.3/redshift_user_manager.egg-info/top_level.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-04-27 17:17:55.121267 redshift-user-manager-0.1.3/setup.cfg
+-rw-r--r--   0 henryjones   (501) staff       (20)      711 2023-04-27 14:19:51.000000 redshift-user-manager-0.1.3/setup.py
```

### Comparing `redshift-user-manager-0.1.2/LICENSE` & `redshift-user-manager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redshift-user-manager-0.1.2/PKG-INFO` & `redshift-user-manager-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redshift-user-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A user management CLI tool for AWS Redshift.
 Home-page: https://github.com/henryivesjones/redshift-user-manager
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: sql,redshift,user,managment
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `redshift-user-manager-0.1.2/README.md` & `redshift-user-manager-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `redshift-user-manager-0.1.2/pyproject.toml` & `redshift-user-manager-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redshift-user-manager-0.1.2/redshift_user_manager/cli.py` & `redshift-user-manager-0.1.3/redshift_user_manager/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             try:
                 password = await rum.create_user(
                     user_name=user_name, roles=list(role), password=password
                 )
             except exceptions.UserAlreadyExists:
                 raise click.ClickException(
@@ -132,14 +133,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=20,
         ) as rum:
             try:
                 await rum.delete_user(user_name=user_name)
             except exceptions.UserDoesntExist:
                 raise click.ClickException(
                     f"No user with the username: '{user_name}' exists."
                 )
@@ -165,14 +167,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             try:
                 p = await rum.update_user_password(user_name, password)
                 click.echo(p)
             except exceptions.UserDoesntExist:
                 raise click.ClickException(
                     f"No user with the username: '{user_name}' exists."
@@ -199,14 +202,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             if len(role) == 0:
                 return
             try:
                 await rum.grant_user_roles(user_name=user_name, roles=list(role))
             except exceptions.UserDoesntExist:
                 raise click.ClickException(
@@ -238,14 +242,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             if len(role) == 0:
                 return
             try:
                 await rum.revoke_user_roles(user_name=user_name, roles=list(role))
             except exceptions.UserDoesntExist:
                 raise click.ClickException(
@@ -279,14 +284,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             try:
                 await rum.refresh_user_roles(user_name, only_grant=only_grant)
             except exceptions.UserDoesntExist:
                 raise click.ClickException(
                     f"No user with the username: '{user_name}' exists."
                 )
@@ -308,14 +314,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             for user in rum.state.users:
                 click.echo(f"{user.user_name} - ({', '.join(user.roles)})")
     except exceptions.RedshiftUserManagerException as e:
         raise click.ClickException(f"{type(e).__name__} {e}")
 
 
@@ -335,14 +342,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             for user in rum.state.users:
                 click.echo(f"Refreshing {user.user_name}.")
                 await rum.refresh_user_roles(user.user_name, only_grant=only_grant)
     except exceptions.RedshiftUserManagerException as e:
         raise click.ClickException(f"{type(e).__name__} {e}")
 
@@ -363,14 +371,15 @@
     """
     try:
         async with RedshiftUserManager(
             config_yaml_file=config_file,
             state_yaml_file=state_file,
             username=sys_username,
             password=sys_password,
+            concurrency=1,
         ) as rum:
             user = rum.state.get_user(user_name)
             if user is None:
                 raise click.ClickException(f"User {user_name} doesn't exist.")
             for permission in rum._get_permissions(user.roles):
                 entity = (
                     permission.entities
```

### Comparing `redshift-user-manager-0.1.2/redshift_user_manager/exceptions.py` & `redshift-user-manager-0.1.3/redshift_user_manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `redshift-user-manager-0.1.2/redshift_user_manager/redshift_user_manager.py` & `redshift-user-manager-0.1.3/redshift_user_manager/redshift_user_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,43 +150,47 @@
 
 
 class RedshiftUserManager:
     """
     A class for orchestrating user creation/deletion and role granting/revoking.
     """
 
+    concurrency: int
     username: str
     password: str
     config: RedshiftUserManagerConfig
     state: RedshiftUserManagerState
     state_yaml_file: str
     config_yaml_file: str
     pool: asyncpg.Pool
 
     def __init__(
         self,
         config_yaml_file: str,
         username: str,
         password: str,
         state_yaml_file: str,
+        concurrency: int = 1
     ):
+        self.concurrency = concurrency
         self.config = RedshiftUserManager.parse_config_yaml(config_yaml_file)
         self.state_yaml_file = state_yaml_file
         self.state = RedshiftUserManager.parse_state_yaml(state_yaml_file)
         self.username = username
         self.password = password
 
     async def __aenter__(self):
         self.pool = await asyncpg.create_pool(
             host=self.config.host,
             port=self.config.port,
             user=self.username,
             password=self.password,
             database=self.config.database,
-            max_size=20,
+            max_size=self.concurrency,
+            min_size=1,
         )
         return self
 
     async def __aexit__(self, _, __, ___):
         self._persist_state()
         await self.pool.close()
```

### Comparing `redshift-user-manager-0.1.2/redshift_user_manager.egg-info/PKG-INFO` & `redshift-user-manager-0.1.3/redshift_user_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redshift-user-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A user management CLI tool for AWS Redshift.
 Home-page: https://github.com/henryivesjones/redshift-user-manager
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: sql,redshift,user,managment
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `redshift-user-manager-0.1.2/redshift_user_manager.egg-info/SOURCES.txt` & `redshift-user-manager-0.1.3/redshift_user_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redshift-user-manager-0.1.2/setup.py` & `redshift-user-manager-0.1.3/setup.py`

 * *Files identical despite different names*


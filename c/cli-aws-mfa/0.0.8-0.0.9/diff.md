# Comparing `tmp/cli-aws-mfa-0.0.8.tar.gz` & `tmp/cli-aws-mfa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-aws-mfa-0.0.8.tar", last modified: Thu Apr 20 05:52:07 2023, max compression
+gzip compressed data, was "cli-aws-mfa-0.0.9.tar", last modified: Thu Apr 27 06:59:53 2023, max compression
```

## Comparing `cli-aws-mfa-0.0.8.tar` & `cli-aws-mfa-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/MFA/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/MFA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/MFA/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/setup.py
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-27 06:59:53.431543 cli-aws-mfa-0.0.9/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1068 2023-04-19 11:40:57.000000 cli-aws-mfa-0.0.9/LICENSE
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-27 06:59:53.430392 cli-aws-mfa-0.0.9/MFA/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.9/MFA/__init__.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     3922 2023-04-27 06:57:52.000000 cli-aws-mfa-0.0.9/MFA/mfa.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1396 2023-04-27 06:59:53.431338 cli-aws-mfa-0.0.9/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1122 2023-04-19 11:32:09.000000 cli-aws-mfa-0.0.9/README.md
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1658 2023-04-19 11:27:22.000000 cli-aws-mfa-0.0.9/cli.py
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-27 06:59:53.431159 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1396 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      272 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       40 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/requires.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        8 2023-04-27 06:59:53.000000 cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/top_level.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-27 06:59:53.431582 cli-aws-mfa-0.0.9/setup.cfg
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      953 2023-04-27 06:58:09.000000 cli-aws-mfa-0.0.9/setup.py
```

### Comparing `cli-aws-mfa-0.0.8/LICENSE` & `cli-aws-mfa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.8/MFA/mfa.py` & `cli-aws-mfa-0.0.9/MFA/mfa.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,21 @@
         aws_config_dir = os.path.join(os.path.expanduser("~"), ".aws")
         if not os.path.exists(aws_config_dir):
             os.makedirs(aws_config_dir)
         credentials_path = os.path.join(aws_config_dir, "credentials")
         config.read(credentials_path)
 
         if self.profile_name in config.sections():
-            config.set(self.profile_name, "aws_access_key_id", aws_access_key_id)
+            config.set(self.profile_name,
+                       "aws_access_key_id", aws_access_key_id)
             config.set(
                 self.profile_name, "aws_secret_access_key", aws_secret_access_key
             )
-            config.set(self.profile_name, "aws_session_token", aws_session_token)
+            config.set(self.profile_name,
+                       "aws_session_token", aws_session_token)
             with open(credentials_path, "w") as f:
                 config.write(f)
         else:
             with open(credentials_path, "a") as f:
                 f.write(f"\n[{self.profile_name}]\n")
                 f.write(f"aws_access_key_id = {aws_access_key_id}\n")
                 f.write(f"aws_secret_access_key = {aws_secret_access_key}\n")
@@ -88,30 +90,14 @@
         if self.check_mfa_profile_file:
             aws_config_dir = os.path.join(os.path.expanduser("~"), ".aws")
             mfa_profile_file = os.path.join(aws_config_dir, ".profile")
             self.profile_name = open(mfa_profile_file, "r").read().strip()
 
         return self.profile_name
 
-    def set_credtiona(self):
-        config = configparser.ConfigParser()
-
-        config.read(creds_path)
-
-        if "profilename" in config.sections():
-            print("Profile already exists")
-        else:
-            # Add the new profile to the credentials file
-            config["profilename"] = new_profile
-
-            with open(creds_path, "w") as configfile:
-                config.write(configfile)
-
-            print("Profile added successfully")
-
     def validate_session(self):
         session = boto3.Session(profile_name=self.profile_name)
         if session.get_credentials().access_key is None:
             print("Error: AWS access key is not set")
         elif session.get_credentials().secret_key is None:
             print("Error: AWS secret key is not set")
         elif session.get_credentials().token is None:
```

### Comparing `cli-aws-mfa-0.0.8/PKG-INFO` & `cli-aws-mfa-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CLI MFA - Easily Manage Session Token
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cli-aws-mfa-0.0.8/README.md` & `cli-aws-mfa-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.8/cli.py` & `cli-aws-mfa-0.0.9/cli.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/PKG-INFO` & `cli-aws-mfa-0.0.9/cli_aws_mfa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.8
+Version: 0.0.9
 Summary: AWS CLI MFA - Easily Manage Session Token
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cli-aws-mfa-0.0.8/setup.py` & `cli-aws-mfa-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "AWS CLI MFA - Easily Manage Session Token"
 LONG_DESCRIPTION = "Use MFA to increase the security of your AWS environment. Signing in with MFA requires an authentication code from an MFA device."
 
 # Setting up
 setup(
     name="cli-aws-mfa",
     version=VERSION,
```


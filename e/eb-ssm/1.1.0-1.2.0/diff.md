# Comparing `tmp/eb-ssm-1.1.0.tar.gz` & `tmp/eb-ssm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eb-ssm-1.1.0.tar", last modified: Mon Jan 10 21:29:36 2022, max compression
+gzip compressed data, was "eb-ssm-1.2.0.tar", last modified: Thu Apr 27 20:29:26 2023, max compression
```

## Comparing `eb-ssm-1.1.0.tar` & `eb-ssm-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-01-10 21:29:36.210699 eb-ssm-1.1.0/
--rw-r--r--   0 zags      (1000) zags      (1000)     4851 2022-01-10 21:29:36.210699 eb-ssm-1.1.0/PKG-INFO
--rw-r--r--   0 zags      (1000) zags      (1000)     3732 2021-03-18 21:21:24.000000 eb-ssm-1.1.0/README.md
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-01-10 21:29:36.200699 eb-ssm-1.1.0/eb_ssm/
--rw-r--r--   0 zags      (1000) zags      (1000)        0 2020-10-21 22:26:07.000000 eb-ssm-1.1.0/eb_ssm/__init__.py
--rw-r--r--   0 zags      (1000) zags      (1000)     3537 2022-01-10 21:28:24.000000 eb-ssm-1.1.0/eb_ssm/eb_ssm.py
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-01-10 21:29:36.200699 eb-ssm-1.1.0/eb_ssm.egg-info/
--rw-r--r--   0 zags      (1000) zags      (1000)     4851 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/PKG-INFO
--rw-r--r--   0 zags      (1000) zags      (1000)      236 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 zags      (1000) zags      (1000)        1 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       47 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/entry_points.txt
--rw-r--r--   0 zags      (1000) zags      (1000)        9 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/requires.txt
--rw-r--r--   0 zags      (1000) zags      (1000)        7 2022-01-10 21:29:36.000000 eb-ssm-1.1.0/eb_ssm.egg-info/top_level.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       38 2022-01-10 21:29:36.210699 eb-ssm-1.1.0/setup.cfg
--rw-r--r--   0 zags      (1000) zags      (1000)      916 2022-01-10 21:23:16.000000 eb-ssm-1.1.0/setup.py
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-04-27 20:29:26.679813 eb-ssm-1.2.0/
+-rw-r--r--   0 zags      (1000) zags      (1000)     1080 2020-10-22 01:35:55.000000 eb-ssm-1.2.0/LICENSE
+-rw-r--r--   0 zags      (1000) zags      (1000)     4266 2023-04-27 20:29:26.679813 eb-ssm-1.2.0/PKG-INFO
+-rw-r--r--   0 zags      (1000) zags      (1000)     3732 2021-03-18 21:21:24.000000 eb-ssm-1.2.0/README.md
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-04-27 20:29:26.679813 eb-ssm-1.2.0/eb_ssm/
+-rw-r--r--   0 zags      (1000) zags      (1000)        0 2020-10-21 22:26:07.000000 eb-ssm-1.2.0/eb_ssm/__init__.py
+-rw-r--r--   0 zags      (1000) zags      (1000)     4308 2023-04-27 20:24:25.000000 eb-ssm-1.2.0/eb_ssm/eb_ssm.py
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-04-27 20:29:26.679813 eb-ssm-1.2.0/eb_ssm.egg-info/
+-rw-r--r--   0 zags      (1000) zags      (1000)     4266 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 zags      (1000) zags      (1000)      244 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)        1 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       46 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)        9 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/requires.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)        7 2023-04-27 20:29:26.000000 eb-ssm-1.2.0/eb_ssm.egg-info/top_level.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       38 2023-04-27 20:29:26.679813 eb-ssm-1.2.0/setup.cfg
+-rw-r--r--   0 zags      (1000) zags      (1000)      916 2023-04-27 20:23:24.000000 eb-ssm-1.2.0/setup.py
```

### Comparing `eb-ssm-1.1.0/PKG-INFO` & `eb-ssm-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 Metadata-Version: 2.1
 Name: eb-ssm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple tool to SSH into an Elastic Beanstalk server using AWS SSM.
 Home-page: https://github.com/zagaran/eb-ssm
 Author: Zagaran, Inc.
 Author-email: info@zagaran.com
 License: MIT
-Description: # EB SSM
-        
-        This simple script helps you SSH into an Elastic Beanstalk server using AWS SSM.
-        
-        eb-ssm is desinged to combine tools from the EB CLI and the AWS CLI to provide a better alternaitve to `eb ssh`.
-        
-        It's a pip library, installed by `pip install eb-ssm`.
-        
-        Once it's set up, you can SSH into your Elastic Beanstalk servers with `eb-ssm [ENVIRONMENT_NAME]`.
-        
-        
-        ## Why you should use it
-        
-        While `eb ssh` exists, it requires each individual user to have the EC2 instance private keys locally. This is unideal
-        from both an information security and access management standpoint. If you've configured SSM, users will no longer need
-        SSH keys to SSH into Elastic Beanstalk instances and instead have their access managed via IAM.
-        
-        The main advantages of eb-ssm are the following:
-        
-        1. **Server SSH access is managed through IAM.**  Normally, you have to manage SSH access to Elastic Beanstalk environments yourself.  IAM is where AWS manages user access for everything else, and with eb-ssm, you can manage server SSH access for EB environments there as well.
-        
-        2. **No shared SSH keys.**  Sharing, tracking, and rotating SSH keys is a pain.  Using eb-ssm, you there are no SSH keys, so these problems go away.
-        
-        3. **No mucking around with port 22.**  The EB CLI is supposed to open port 22 just for the SSH session but it doesn't close it in the event of non-graceful termination of the SSH session.  eb-ssm does one better by never opening port 22 in the first place.
-        
-        4. **Audit log of SSH sessions.**  AWS SSM keeps a log of SSH sessions.  This is one more benefit that comes from using it over native SSH.
-        
-        5. **Ability to access non-public servers.**  If you have servers in a privative subnet, you can use eb-ssm to SSH into them without needing a bastion host.
-        
-        
-        ## Prerequisites
-        
-        ### Set up your Elastic Beanstalk Environment to allow SSH via AWS SSM
-        
-        The following steps need to be done once per environment.
-        
-        1. Go to Elastic Beanstalk > ENVIRONEMNT_NAME > Configuration > Security and find the "IAM instance profile" (by default, this is "aws-elasticbeanstalk-ec2-role").  This is ROLE_NAME in step 2.
-        
-        2. Go to IAM > Roles > ROLE_NAME.  Under permissions, add "AmazonSSMManagedInstanceCore".
-        
-        3. Go to Systems Manager > Session Manager > Preferences > Edit.  Enable "Run As Support" and set the "Run As Defualt User" to be "ec2-user" (or whatever the default user for your Elastic Beanstalk servers is).
-        
-        Note that it may take some time (~10 minutes) for the IAM changes to propagate.  If you have completed the AWS setup and get a "TargetNotConnected" error, wait 10-15 minutes and try again.
-        
-        ### Configure your local computer
-        
-        The following steps need to be done once per computer.
-        
-        1. Install the AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
-        
-        2. Install the Session Manager Plugin: https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
-        
-        ## Using EB SSM
-        
-        Install eb-ssm via `pip install eb-ssm`.
-        
-        Once it is installed, all you need to do is run `eb-ssm` from your repository and it will automatically hook into your repository's EB configuration (in .elasticbeanstalk/config.yml).
-        
-        To ssh into a specific environment, use `eb-ssm ENVIRONMENT_NAME`.
-        
-        You can also optionally pass other parameters, such as an AWS CLI profile or a region to eb-ssm.  See `eb-ssm --help` for a full list of options.
-        
-        ## Config
-        
-        eb-ssm uses the EB CLI configuration files.  If you have not used the EB CLI to set up a project, here is the minimal configruation needed by eb-ssm; this configraution lives in `.elasticbeanstalk/config.yml`:
-        
-        ```
-        global:
-          application_name: EB_APPLICATION_NAME
-          default_region: REGION_NAME
-          profile: PROFILE_NAME
-        ```
-        
 Keywords: aws eb ssm elastic beanstalk systems manager agent ssh
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EB SSM
+
+This simple script helps you SSH into an Elastic Beanstalk server using AWS SSM.
+
+eb-ssm is desinged to combine tools from the EB CLI and the AWS CLI to provide a better alternaitve to `eb ssh`.
+
+It's a pip library, installed by `pip install eb-ssm`.
+
+Once it's set up, you can SSH into your Elastic Beanstalk servers with `eb-ssm [ENVIRONMENT_NAME]`.
+
+
+## Why you should use it
+
+While `eb ssh` exists, it requires each individual user to have the EC2 instance private keys locally. This is unideal
+from both an information security and access management standpoint. If you've configured SSM, users will no longer need
+SSH keys to SSH into Elastic Beanstalk instances and instead have their access managed via IAM.
+
+The main advantages of eb-ssm are the following:
+
+1. **Server SSH access is managed through IAM.**  Normally, you have to manage SSH access to Elastic Beanstalk environments yourself.  IAM is where AWS manages user access for everything else, and with eb-ssm, you can manage server SSH access for EB environments there as well.
+
+2. **No shared SSH keys.**  Sharing, tracking, and rotating SSH keys is a pain.  Using eb-ssm, you there are no SSH keys, so these problems go away.
+
+3. **No mucking around with port 22.**  The EB CLI is supposed to open port 22 just for the SSH session but it doesn't close it in the event of non-graceful termination of the SSH session.  eb-ssm does one better by never opening port 22 in the first place.
+
+4. **Audit log of SSH sessions.**  AWS SSM keeps a log of SSH sessions.  This is one more benefit that comes from using it over native SSH.
+
+5. **Ability to access non-public servers.**  If you have servers in a privative subnet, you can use eb-ssm to SSH into them without needing a bastion host.
+
+
+## Prerequisites
+
+### Set up your Elastic Beanstalk Environment to allow SSH via AWS SSM
+
+The following steps need to be done once per environment.
+
+1. Go to Elastic Beanstalk > ENVIRONEMNT_NAME > Configuration > Security and find the "IAM instance profile" (by default, this is "aws-elasticbeanstalk-ec2-role").  This is ROLE_NAME in step 2.
+
+2. Go to IAM > Roles > ROLE_NAME.  Under permissions, add "AmazonSSMManagedInstanceCore".
+
+3. Go to Systems Manager > Session Manager > Preferences > Edit.  Enable "Run As Support" and set the "Run As Defualt User" to be "ec2-user" (or whatever the default user for your Elastic Beanstalk servers is).
+
+Note that it may take some time (~10 minutes) for the IAM changes to propagate.  If you have completed the AWS setup and get a "TargetNotConnected" error, wait 10-15 minutes and try again.
+
+### Configure your local computer
+
+The following steps need to be done once per computer.
+
+1. Install the AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
+
+2. Install the Session Manager Plugin: https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
+
+## Using EB SSM
+
+Install eb-ssm via `pip install eb-ssm`.
+
+Once it is installed, all you need to do is run `eb-ssm` from your repository and it will automatically hook into your repository's EB configuration (in .elasticbeanstalk/config.yml).
+
+To ssh into a specific environment, use `eb-ssm ENVIRONMENT_NAME`.
+
+You can also optionally pass other parameters, such as an AWS CLI profile or a region to eb-ssm.  See `eb-ssm --help` for a full list of options.
+
+## Config
+
+eb-ssm uses the EB CLI configuration files.  If you have not used the EB CLI to set up a project, here is the minimal configruation needed by eb-ssm; this configraution lives in `.elasticbeanstalk/config.yml`:
+
+```
+global:
+  application_name: EB_APPLICATION_NAME
+  default_region: REGION_NAME
+  profile: PROFILE_NAME
+```
```

### Comparing `eb-ssm-1.1.0/README.md` & `eb-ssm-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eb-ssm-1.1.0/eb_ssm.egg-info/PKG-INFO` & `eb-ssm-1.2.0/eb_ssm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 Metadata-Version: 2.1
 Name: eb-ssm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple tool to SSH into an Elastic Beanstalk server using AWS SSM.
 Home-page: https://github.com/zagaran/eb-ssm
 Author: Zagaran, Inc.
 Author-email: info@zagaran.com
 License: MIT
-Description: # EB SSM
-        
-        This simple script helps you SSH into an Elastic Beanstalk server using AWS SSM.
-        
-        eb-ssm is desinged to combine tools from the EB CLI and the AWS CLI to provide a better alternaitve to `eb ssh`.
-        
-        It's a pip library, installed by `pip install eb-ssm`.
-        
-        Once it's set up, you can SSH into your Elastic Beanstalk servers with `eb-ssm [ENVIRONMENT_NAME]`.
-        
-        
-        ## Why you should use it
-        
-        While `eb ssh` exists, it requires each individual user to have the EC2 instance private keys locally. This is unideal
-        from both an information security and access management standpoint. If you've configured SSM, users will no longer need
-        SSH keys to SSH into Elastic Beanstalk instances and instead have their access managed via IAM.
-        
-        The main advantages of eb-ssm are the following:
-        
-        1. **Server SSH access is managed through IAM.**  Normally, you have to manage SSH access to Elastic Beanstalk environments yourself.  IAM is where AWS manages user access for everything else, and with eb-ssm, you can manage server SSH access for EB environments there as well.
-        
-        2. **No shared SSH keys.**  Sharing, tracking, and rotating SSH keys is a pain.  Using eb-ssm, you there are no SSH keys, so these problems go away.
-        
-        3. **No mucking around with port 22.**  The EB CLI is supposed to open port 22 just for the SSH session but it doesn't close it in the event of non-graceful termination of the SSH session.  eb-ssm does one better by never opening port 22 in the first place.
-        
-        4. **Audit log of SSH sessions.**  AWS SSM keeps a log of SSH sessions.  This is one more benefit that comes from using it over native SSH.
-        
-        5. **Ability to access non-public servers.**  If you have servers in a privative subnet, you can use eb-ssm to SSH into them without needing a bastion host.
-        
-        
-        ## Prerequisites
-        
-        ### Set up your Elastic Beanstalk Environment to allow SSH via AWS SSM
-        
-        The following steps need to be done once per environment.
-        
-        1. Go to Elastic Beanstalk > ENVIRONEMNT_NAME > Configuration > Security and find the "IAM instance profile" (by default, this is "aws-elasticbeanstalk-ec2-role").  This is ROLE_NAME in step 2.
-        
-        2. Go to IAM > Roles > ROLE_NAME.  Under permissions, add "AmazonSSMManagedInstanceCore".
-        
-        3. Go to Systems Manager > Session Manager > Preferences > Edit.  Enable "Run As Support" and set the "Run As Defualt User" to be "ec2-user" (or whatever the default user for your Elastic Beanstalk servers is).
-        
-        Note that it may take some time (~10 minutes) for the IAM changes to propagate.  If you have completed the AWS setup and get a "TargetNotConnected" error, wait 10-15 minutes and try again.
-        
-        ### Configure your local computer
-        
-        The following steps need to be done once per computer.
-        
-        1. Install the AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
-        
-        2. Install the Session Manager Plugin: https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
-        
-        ## Using EB SSM
-        
-        Install eb-ssm via `pip install eb-ssm`.
-        
-        Once it is installed, all you need to do is run `eb-ssm` from your repository and it will automatically hook into your repository's EB configuration (in .elasticbeanstalk/config.yml).
-        
-        To ssh into a specific environment, use `eb-ssm ENVIRONMENT_NAME`.
-        
-        You can also optionally pass other parameters, such as an AWS CLI profile or a region to eb-ssm.  See `eb-ssm --help` for a full list of options.
-        
-        ## Config
-        
-        eb-ssm uses the EB CLI configuration files.  If you have not used the EB CLI to set up a project, here is the minimal configruation needed by eb-ssm; this configraution lives in `.elasticbeanstalk/config.yml`:
-        
-        ```
-        global:
-          application_name: EB_APPLICATION_NAME
-          default_region: REGION_NAME
-          profile: PROFILE_NAME
-        ```
-        
 Keywords: aws eb ssm elastic beanstalk systems manager agent ssh
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EB SSM
+
+This simple script helps you SSH into an Elastic Beanstalk server using AWS SSM.
+
+eb-ssm is desinged to combine tools from the EB CLI and the AWS CLI to provide a better alternaitve to `eb ssh`.
+
+It's a pip library, installed by `pip install eb-ssm`.
+
+Once it's set up, you can SSH into your Elastic Beanstalk servers with `eb-ssm [ENVIRONMENT_NAME]`.
+
+
+## Why you should use it
+
+While `eb ssh` exists, it requires each individual user to have the EC2 instance private keys locally. This is unideal
+from both an information security and access management standpoint. If you've configured SSM, users will no longer need
+SSH keys to SSH into Elastic Beanstalk instances and instead have their access managed via IAM.
+
+The main advantages of eb-ssm are the following:
+
+1. **Server SSH access is managed through IAM.**  Normally, you have to manage SSH access to Elastic Beanstalk environments yourself.  IAM is where AWS manages user access for everything else, and with eb-ssm, you can manage server SSH access for EB environments there as well.
+
+2. **No shared SSH keys.**  Sharing, tracking, and rotating SSH keys is a pain.  Using eb-ssm, you there are no SSH keys, so these problems go away.
+
+3. **No mucking around with port 22.**  The EB CLI is supposed to open port 22 just for the SSH session but it doesn't close it in the event of non-graceful termination of the SSH session.  eb-ssm does one better by never opening port 22 in the first place.
+
+4. **Audit log of SSH sessions.**  AWS SSM keeps a log of SSH sessions.  This is one more benefit that comes from using it over native SSH.
+
+5. **Ability to access non-public servers.**  If you have servers in a privative subnet, you can use eb-ssm to SSH into them without needing a bastion host.
+
+
+## Prerequisites
+
+### Set up your Elastic Beanstalk Environment to allow SSH via AWS SSM
+
+The following steps need to be done once per environment.
+
+1. Go to Elastic Beanstalk > ENVIRONEMNT_NAME > Configuration > Security and find the "IAM instance profile" (by default, this is "aws-elasticbeanstalk-ec2-role").  This is ROLE_NAME in step 2.
+
+2. Go to IAM > Roles > ROLE_NAME.  Under permissions, add "AmazonSSMManagedInstanceCore".
+
+3. Go to Systems Manager > Session Manager > Preferences > Edit.  Enable "Run As Support" and set the "Run As Defualt User" to be "ec2-user" (or whatever the default user for your Elastic Beanstalk servers is).
+
+Note that it may take some time (~10 minutes) for the IAM changes to propagate.  If you have completed the AWS setup and get a "TargetNotConnected" error, wait 10-15 minutes and try again.
+
+### Configure your local computer
+
+The following steps need to be done once per computer.
+
+1. Install the AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
+
+2. Install the Session Manager Plugin: https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
+
+## Using EB SSM
+
+Install eb-ssm via `pip install eb-ssm`.
+
+Once it is installed, all you need to do is run `eb-ssm` from your repository and it will automatically hook into your repository's EB configuration (in .elasticbeanstalk/config.yml).
+
+To ssh into a specific environment, use `eb-ssm ENVIRONMENT_NAME`.
+
+You can also optionally pass other parameters, such as an AWS CLI profile or a region to eb-ssm.  See `eb-ssm --help` for a full list of options.
+
+## Config
+
+eb-ssm uses the EB CLI configuration files.  If you have not used the EB CLI to set up a project, here is the minimal configruation needed by eb-ssm; this configraution lives in `.elasticbeanstalk/config.yml`:
+
+```
+global:
+  application_name: EB_APPLICATION_NAME
+  default_region: REGION_NAME
+  profile: PROFILE_NAME
+```
```

### Comparing `eb-ssm-1.1.0/setup.py` & `eb-ssm-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     license="MIT",
     long_description=README,
     long_description_content_type="text/markdown",
     name="eb-ssm",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     url="https://github.com/zagaran/eb-ssm",
-    version="1.1.0",
+    version="1.2.0",
 )
```


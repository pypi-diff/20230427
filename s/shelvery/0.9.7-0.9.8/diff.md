# Comparing `tmp/shelvery-0.9.7.tar.gz` & `tmp/shelvery-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shelvery-0.9.7.tar", last modified: Wed Jul 27 06:37:37 2022, max compression
+gzip compressed data, was "shelvery-0.9.8.tar", last modified: Thu Apr 27 02:51:51 2023, max compression
```

## Comparing `shelvery-0.9.7.tar` & `shelvery-0.9.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2022-07-27 06:37:37.316055 shelvery-0.9.7/
--rw-r--r--   0 gus        (501) staff       (20)     1057 2021-10-12 01:55:23.000000 shelvery-0.9.7/LICENSE.txt
--rw-r--r--   0 gus        (501) staff       (20)      667 2022-07-27 06:37:37.315543 shelvery-0.9.7/PKG-INFO
--rw-r--r--   0 gus        (501) staff       (20)    20790 2021-10-12 01:55:23.000000 shelvery-0.9.7/README.md
--rw-r--r--   0 gus        (501) staff       (20)       38 2022-07-27 06:37:37.316481 shelvery-0.9.7/setup.cfg
--rw-r--r--   0 gus        (501) staff       (20)      933 2022-07-26 04:13:19.000000 shelvery-0.9.7/setup.py
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2022-07-27 06:37:37.299876 shelvery-0.9.7/shelvery/
--rw-r--r--   0 gus        (501) staff       (20)      153 2022-07-26 04:13:19.000000 shelvery-0.9.7/shelvery/__init__.py
--rw-r--r--   0 gus        (501) staff       (20)     4209 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/aws_helper.py
--rw-r--r--   0 gus        (501) staff       (20)     8835 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/backup_resource.py
--rw-r--r--   0 gus        (501) staff       (20)    15628 2022-07-26 04:11:30.000000 shelvery-0.9.7/shelvery/documentdb_backup.py
--rw-r--r--   0 gus        (501) staff       (20)     8222 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/ebs_backup.py
--rw-r--r--   0 gus        (501) staff       (20)     1750 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/ec2_backup.py
--rw-r--r--   0 gus        (501) staff       (20)    10747 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/ec2ami_backup.py
--rw-r--r--   0 gus        (501) staff       (20)    38030 2022-07-26 04:11:30.000000 shelvery-0.9.7/shelvery/engine.py
--rw-r--r--   0 gus        (501) staff       (20)      610 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/entity_resource.py
--rw-r--r--   0 gus        (501) staff       (20)      943 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/factory.py
--rw-r--r--   0 gus        (501) staff       (20)      941 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/notifications.py
--rw-r--r--   0 gus        (501) staff       (20)     1151 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/queue.py
--rw-r--r--   0 gus        (501) staff       (20)    14511 2022-07-26 04:11:30.000000 shelvery-0.9.7/shelvery/rds_backup.py
--rw-r--r--   0 gus        (501) staff       (20)    14651 2022-07-11 01:20:49.000000 shelvery-0.9.7/shelvery/rds_cluster_backup.py
--rw-r--r--   0 gus        (501) staff       (20)    11496 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/redshift_backup.py
--rw-r--r--   0 gus        (501) staff       (20)    14453 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/runtime_config.py
--rw-r--r--   0 gus        (501) staff       (20)     2542 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery/shelvery_invoker.py
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2022-07-27 06:37:37.310262 shelvery-0.9.7/shelvery.egg-info/
--rw-r--r--   0 gus        (501) staff       (20)      667 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/PKG-INFO
--rw-r--r--   0 gus        (501) staff       (20)      792 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/SOURCES.txt
--rw-r--r--   0 gus        (501) staff       (20)        1 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/dependency_links.txt
--rw-r--r--   0 gus        (501) staff       (20)       57 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/entry_points.txt
--rw-r--r--   0 gus        (501) staff       (20)       29 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/requires.txt
--rw-r--r--   0 gus        (501) staff       (20)       38 2022-07-27 06:37:37.000000 shelvery-0.9.7/shelvery.egg-info/top_level.txt
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2022-07-27 06:37:37.313265 shelvery-0.9.7/shelvery_cli/
--rw-r--r--   0 gus        (501) staff       (20)        0 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery_cli/__init__.py
--rw-r--r--   0 gus        (501) staff       (20)     1149 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery_cli/__main__.py
--rw-r--r--   0 gus        (501) staff       (20)      453 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery_cli/shelver_cli_main.py
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2022-07-27 06:37:37.314731 shelvery-0.9.7/shelvery_lambda/
--rw-r--r--   0 gus        (501) staff       (20)        0 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery_lambda/__init__.py
--rw-r--r--   0 gus        (501) staff       (20)     1234 2021-10-12 01:55:23.000000 shelvery-0.9.7/shelvery_lambda/lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 02:51:35.000000 shelvery-0.9.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 02:51:51.363486 shelvery-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21023 2023-04-27 02:51:35.000000 shelvery-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 02:51:51.363486 shelvery-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-27 02:51:35.000000 shelvery-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/aws_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/documentdb_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ebs_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ec2_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ec2ami_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40843 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/entity_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/rds_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/rds_cluster_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/redshift_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/runtime_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/shelvery_invoker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/shelver_cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_lambda/lambda_handler.py
```

### Comparing `shelvery-0.9.7/LICENSE.txt` & `shelvery-0.9.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/PKG-INFO` & `shelvery-0.9.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: shelvery
-Version: 0.9.7
+Version: 0.9.8
 Summary: Backup manager for AWS EBS and AWS RDS services
 Home-page: http://github.com/base2Services/shelvery-aws-backups
 Author: Base2Services R&D
 Author-email: itsupport@base2services.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: aws backup lambda ebs rds ami
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Archiving :: Backup
 Requires-Python: >=3.6
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `shelvery-0.9.7/README.md` & `shelvery-0.9.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,17 @@
 - `shelvery_encrypt_copy` - [boolean] when copying a shared unencrypted snapshot, encrypt the shapshot. 
                             when enabled 'shelvery_copy_kms_key_id' must also be set.
 
 - `shelvery_copy_kms_key_id` - when copying a shared snapshot, you can specify a different kms key used to encrypt the original snapshot.
                                Note that when copying to a new key, the shelvery requires access to both the new key and the original key.
                                The full KMS key ARN should be supplied.
 
+- `shelvery_reencrypt_kms_key_id`  - when it is required to re-encrypt a RDS instance or cluster snapshot with a different KMS key 
+                                than that of the existing resource. Specify the ARN of the KMS Key.
+
 ### Configuration Priority 0: Sensible defaults
 
 ```text
 shelvery_keep_daily_backups=14
 shelvery_keep_weekly_backups=8
 shelvery_keep_monthly_backups=12
 shelvery_keep_yearly_backups=10
```

### Comparing `shelvery-0.9.7/setup.py` & `shelvery-0.9.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-setup(name='shelvery', version='0.9.7', author='Base2Services R&D',
+setup(name='shelvery', version='0.9.8', author='Base2Services R&D',
       author_email='itsupport@base2services.com',
       url='http://github.com/base2Services/shelvery-aws-backups',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Programming Language :: Python :: 3.6',
           'Intended Audience :: System Administrators',
           'Intended Audience :: Information Technology',
```

### Comparing `shelvery-0.9.7/shelvery/aws_helper.py` & `shelvery-0.9.8/shelvery/aws_helper.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/backup_resource.py` & `shelvery-0.9.8/shelvery/backup_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         else:
             obj.account_id = AwsHelper.local_account_id()
 
         return obj
 
     def entity_resource_tags(self):
         return self.entity_resource.tags if self.entity_resource is not None else {}
-
+    
     def calculate_expire_date(self, engine, custom_retention_types=None):
         """Determine expire date, based on 'retention_type' tag"""
         if self.retention_type == BackupResource.RETENTION_DAILY:
             expire_date = self.date_created + timedelta(
                 days=RuntimeConfig.get_keep_daily(self.entity_resource_tags(), engine))
         elif self.retention_type == BackupResource.RETENTION_WEEKLY:
             expire_date = self.date_created + relativedelta(
@@ -193,19 +193,20 @@
         return self.__region
 
     @region.setter
     def region(self, region: str):
         self.__region = region
 
     def set_retention_type(self, retention_type: str):
+        self.retention_type = retention_type
         self.name = '-'.join(self.name.split('-')[0:-1]) + f"-{retention_type}"
         self.tags[f"{self.tags['shelvery:tag_name']}:name"] = self.name
         self.tags['Name'] = self.name
         self.tags[f"{self.tags['shelvery:tag_name']}:retention_type"] = retention_type
-
+    
     @property
     def boto3_tags(self):
         tags = self.tags
         return list(map(lambda k: {'Key': k, 'Value': tags[k]}, tags))
 
     @staticmethod
     def dict_from_boto3_tags(boot3_tags):
```

### Comparing `shelvery-0.9.7/shelvery/documentdb_backup.py` & `shelvery-0.9.8/shelvery/documentdb_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/ebs_backup.py` & `shelvery-0.9.8/shelvery/ebs_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/ec2_backup.py` & `shelvery-0.9.8/shelvery/ec2_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/ec2ami_backup.py` & `shelvery-0.9.8/shelvery/ec2ami_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/engine.py` & `shelvery-0.9.8/shelvery/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 import logging
 import time
 import sys
+from unittest import skip
 
 import botocore
 import yaml
 import boto3
 from botocore.exceptions import ClientError
 from datetime import datetime
 
@@ -30,14 +31,21 @@
 
     __metaclass__ = abc.ABCMeta
 
     DEFAULT_KEEP_DAILY = 14
     DEFAULT_KEEP_WEEKLY = 8
     DEFAULT_KEEP_MONTHLY = 12
     DEFAULT_KEEP_YEARLY = 10
+    
+    RETENTION_TYPE_PRECEDENCE = {
+        BackupResource.RETENTION_YEARLY : BackupResource.RETENTION_MONTHLY,
+        BackupResource.RETENTION_MONTHLY : BackupResource.RETENTION_WEEKLY,
+        BackupResource.RETENTION_WEEKLY :  BackupResource.RETENTION_DAILY,
+        BackupResource.RETENTION_DAILY : None
+    }
 
     BACKUP_RESOURCE_TAG = 'create_backup'
 
     def __init__(self):
         # system logger
         FORMAT = "%(asctime)s %(process)s %(thread)s: %(message)s"
         logging.basicConfig(format=FORMAT)
@@ -169,25 +177,37 @@
         bucket.put_object(
             Body=yaml.dump(backup, default_flow_style=False),
             Key=s3key
         )
         self.logger.info(f"Wrote meta for backup {backup.name} of type {self.get_engine_type()} to" +
                          f" s3://{bucket.name}/{s3key}")
 
+    def _verify_retention(self,backup_resource: BackupResource) -> bool:
+        if backup_resource.retention_type == backup_resource.RETENTION_DAILY:
+            return RuntimeConfig.get_keep_daily(backup_resource.entity_resource_tags(),self) != 0
+        elif backup_resource.retention_type == backup_resource.RETENTION_WEEKLY:
+            return RuntimeConfig.get_keep_weekly(backup_resource.entity_resource_tags(),self) != 0
+        elif backup_resource.retention_type == backup_resource.RETENTION_MONTHLY:
+            return RuntimeConfig.get_keep_monthly(backup_resource.entity_resource_tags(),self) != 0
+        elif backup_resource.retention_type == backup_resource.RETENTION_YEARLY:
+            return RuntimeConfig.get_keep_yearly(backup_resource.entity_resource_tags(),self) != 0
+        
+        # fail open
+        return True         
 
     ### Top level methods, invoked externally ####
     def create_backups(self) -> List[BackupResource]:
         """Create backups from all collected entities marked for backup by using specific tag"""
 
         # collect resources to be backed up
         resource_type = self.get_resource_type()
         self.logger.info(f"Collecting entities of type {resource_type} tagged with "
                          f"{RuntimeConfig.get_tag_prefix()}:{self.BACKUP_RESOURCE_TAG}")
         resources = self.get_entities_to_backup(f"{RuntimeConfig.get_tag_prefix()}:{self.BACKUP_RESOURCE_TAG}")
-
+        
         # allows user to select single entity to be backed up
         if RuntimeConfig.get_shelvery_select_entity(self) is not None:
             entity_id = RuntimeConfig.get_shelvery_select_entity(self)
             self.logger.info(f"Creating backups only for entity {entity_id}")
             resources = list(
                 filter(
                     lambda x: x.resource_id == entity_id,
@@ -202,17 +222,41 @@
         for r in resources:
             backup_resource = BackupResource(
                 tag_prefix=RuntimeConfig.get_tag_prefix(),
                 entity_resource=r,
                 copy_resource_tags=RuntimeConfig.copy_resource_tags(self),
                 exluded_resource_tag_keys=RuntimeConfig.get_exluded_resource_tag_keys(self)
             )
+            
             # if retention is explicitly given by runtime environment
             if current_retention_type is not None:
                 backup_resource.set_retention_type(current_retention_type)
+                        
+            # Check whether current retention is allowed, if not try next retention type by precedence
+            skip_backup = False
+
+            # skip validation if custom retention type
+            if backup_resource.retention_type in self.RETENTION_TYPE_PRECEDENCE:
+                # Check whether current retention is allowed, if not try next retention type by precedence
+                while not self._verify_retention(backup_resource):
+                    self.logger.info(f"Retention Type: {backup_resource.retention_type} disabled")
+                    new_retention_type = self.RETENTION_TYPE_PRECEDENCE[backup_resource.retention_type]
+                    self.logger.info(f"Checking whether retention type: {new_retention_type} is permitted")
+                    if new_retention_type:
+                        backup_resource.set_retention_type(new_retention_type)
+                    else:
+                        #Set skip backup to true as daily is set to 0
+                        skip_backup = True
+                        break 
+            else:
+                self.logger.info(f"Skipping retention check as custom retention type {backup_resource.retention_type} was detected")
+
+            # Skip current backup
+            if skip_backup:
+                continue
 
             dr_regions = RuntimeConfig.get_dr_regions(backup_resource.entity_resource.tags, self)
             backup_resource.tags[f"{RuntimeConfig.get_tag_prefix()}:dr_regions"] = ','.join(dr_regions)
             self.logger.info(f"Processing {resource_type} with id {r.resource_id}")
             self.logger.info(f"Creating backup {backup_resource.name}")
 
             try:
@@ -627,15 +671,18 @@
                                               backup_id=backup_id,
                                               lambda_method='do_share_backup',
                                               lambda_args=kwargs):
                 return
 
         self.logger.info(f"Do share backup {backup_id} ({backup_region}) with {destination_account_id}")
         try:
-            self.share_backup_with_account(backup_region, backup_id, destination_account_id)
+            new_backup_id = self.share_backup_with_account(backup_region, backup_id, destination_account_id)
+            #assign new backup id if new snapshot is created (eg: re-encrypted rds snapshot)
+            backup_id = new_backup_id if new_backup_id else backup_id
+            self.logger.info(f"Shared backup {backup_id} ({backup_region}) with {destination_account_id}")
             backup_resource = self.get_backup_resource(backup_region, backup_id)
             self._write_backup_data(
                 backup_resource,
                 self._get_data_bucket(backup_region),
                 destination_account_id
             )
             self.snspublisher.notify({
```

### Comparing `shelvery-0.9.7/shelvery/entity_resource.py` & `shelvery-0.9.8/shelvery/entity_resource.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/factory.py` & `shelvery-0.9.8/shelvery/factory.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/notifications.py` & `shelvery-0.9.8/shelvery/notifications.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/queue.py` & `shelvery-0.9.8/shelvery/queue.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/rds_backup.py` & `shelvery-0.9.8/shelvery/rds_backup.py`

 * *Files 22% similar despite different names*

```diff
@@ -91,33 +91,85 @@
         # filter ones backed up with shelvery
         all_backups = self.get_shelvery_backups_only(all_snapshots, backup_tag_prefix, rds_client)
 
         return all_backups
 
     def share_backup_with_account(self, backup_region: str, backup_id: str, aws_account_id: str):
         rds_client = AwsHelper.boto3_client('rds', region_name=backup_region, arn=self.role_arn, external_id=self.role_external_id)
+        backup_resource = self.get_backup_resource(backup_region, backup_id)
+        kms_key = RuntimeConfig.get_reencrypt_kms_key_id(backup_resource.tags, self)
+        
+        # if a re-encrypt key is provided, create new re-encrypted snapshot and share that instead
+        if kms_key:
+            self.logger.info(f"Re-encrypt KMS Key found, creating new backup with {kms_key}")
+            # create re-encrypted backup
+            backup_id = self.copy_backup_to_region(backup_id, backup_region)
+            self.logger.info(f"Creating new encrypted backup {backup_id}")
+            # wait till new snapshot is available
+            if not self.wait_backup_available(backup_region=backup_region,
+                backup_id=backup_id,
+                lambda_method='do_share_backup',
+                lambda_args={}):
+                return
+            self.logger.info(f"New encrypted backup {backup_id} created")
+            
+            #Get new snapshot ARN
+            snapshots = rds_client.describe_db_snapshots(DBSnapshotIdentifier=backup_id)
+            snapshot_arn = snapshots['DBSnapshots'][0]['DBSnapshotArn']
+            
+            #Update tags with '-re-encrypted' suffix
+            self.logger.info(f"Updating tags for new snapshot - {backup_id}")
+            tags = self.get_backup_resource(backup_region, backup_id).tags
+            tags.update({'Name': backup_id, 'shelvery:name': backup_id})
+            tag_list = [{'Key': key, 'Value': value} for key, value in tags.items()]
+            rds_client.add_tags_to_resource(
+                ResourceName=snapshot_arn,
+                Tags=tag_list
+            )
+            created_new_encrypted_snapshot = True
+        else:
+            self.logger.info(f"No re-encrypt key detected")
+            created_new_encrypted_snapshot = False 
+        
         rds_client.modify_db_snapshot_attribute(
             DBSnapshotIdentifier=backup_id,
             AttributeName='restore',
             ValuesToAdd=[aws_account_id]
         )
+        # if re-encryption occured, clean up old snapshot
+        if created_new_encrypted_snapshot:
+            # delete old snapshot
+            self.delete_backup(backup_resource)
+            self.logger.info(f"Cleaning up un-encrypted backup: {backup_resource.backup_id}")
+
+        return backup_id
 
     def copy_backup_to_region(self, backup_id: str, region: str) -> str:
         local_region = boto3.session.Session().region_name
         client_local = AwsHelper.boto3_client('rds', arn=self.role_arn, external_id=self.role_external_id)
         rds_client = AwsHelper.boto3_client('rds', region_name=region, arn=self.role_arn, external_id=self.role_external_id)
         snapshots = client_local.describe_db_snapshots(DBSnapshotIdentifier=backup_id)
         snapshot = snapshots['DBSnapshots'][0]
-        rds_client.copy_db_snapshot(
-            SourceDBSnapshotIdentifier=snapshot['DBSnapshotArn'],
-            TargetDBSnapshotIdentifier=backup_id,
-            SourceRegion=local_region,
+        backup_resource = self.get_backup_resource(local_region, backup_id)
+        kms_key = RuntimeConfig.get_reencrypt_kms_key_id(backup_resource.tags, self)
+        rds_client_params = {
+            'SourceDBSnapshotIdentifier': snapshot['DBSnapshotArn'],
+            'TargetDBSnapshotIdentifier': backup_id,
+            'SourceRegion': local_region,
             # tags are created explicitly
-            CopyTags=False
-        )
+            'CopyTags': False
+        }
+         # add kms key params if reencrypt key is defined
+        if kms_key is not None:
+            backup_id = f'{backup_id}-re-encrypted'
+            rds_client_params['KmsKeyId'] = kms_key
+            rds_client_params['CopyTags'] = True
+            rds_client_params['TargetDBSnapshotIdentifier'] = backup_id
+            
+        rds_client.copy_db_snapshot(**rds_client_params)
         return backup_id
 
     def get_backup_resource(self, backup_region: str, backup_id: str) -> BackupResource:
         rds_client = AwsHelper.boto3_client('rds', region_name=backup_region, arn=self.role_arn, external_id=self.role_external_id)
         snapshots = rds_client.describe_db_snapshots(DBSnapshotIdentifier=backup_id)
         snapshot = snapshots['DBSnapshots'][0]
         tags = snapshot['TagList']
```

### Comparing `shelvery-0.9.7/shelvery/rds_cluster_backup.py` & `shelvery-0.9.8/shelvery/rds_cluster_backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from tracemalloc import Snapshot
 import boto3
 
 from shelvery.runtime_config import RuntimeConfig
 from shelvery.backup_resource import BackupResource
 from shelvery.engine import ShelveryEngine, SHELVERY_DO_BACKUP_TAGS
 from shelvery.entity_resource import EntityResource
 
@@ -92,33 +93,84 @@
         # filter ones backed up with shelvery
         all_backups = self.get_shelvery_backups_only(all_snapshots, backup_tag_prefix, rds_client)
 
         return all_backups
 
     def share_backup_with_account(self, backup_region: str, backup_id: str, aws_account_id: str):
         rds_client = AwsHelper.boto3_client('rds', region_name=backup_region, arn=self.role_arn, external_id=self.role_external_id)
+        backup_resource = self.get_backup_resource(backup_region, backup_id)
+        kms_key = RuntimeConfig.get_reencrypt_kms_key_id(backup_resource.tags, self)
+        
+        # if a re-encrypt key is provided, create new re-encrypted snapshot and share that instead
+        if kms_key:
+            self.logger.info(f"Re-encrypt KMS Key found, creating new backup with {kms_key}")
+            # create re-encrypted backup
+            backup_id = self.copy_backup_to_region(backup_id, backup_region)
+            self.logger.info(f"Creating new encrypted backup {backup_id}")
+            # wait till new snapshot is available
+            if not self.wait_backup_available(backup_region=backup_region,
+                backup_id=backup_id,
+                lambda_method='do_share_backup',
+                lambda_args={}):
+                return
+            self.logger.info(f"New encrypted backup {backup_id} created")
+            
+            #Get new snapshot ARN 
+            snapshots = rds_client.describe_db_cluster_snapshots(DBClusterSnapshotIdentifier=backup_id)
+            snapshot_arn = snapshots['DBClusterSnapshots'][0]['DBClusterSnapshotArn']
+           
+            #Update tags with '-re-encrypted' suffix
+            self.logger.info(f"Updating tags for new snapshot - {backup_id}")
+            tags = self.get_backup_resource(backup_region, backup_id).tags
+            tags.update({'Name': backup_id, 'shelvery:name': backup_id})
+            tag_list = [{'Key': key, 'Value': value} for key, value in tags.items()]
+            rds_client.add_tags_to_resource(
+                ResourceName=snapshot_arn,
+                Tags=tag_list
+            )
+            created_new_encrypted_snapshot = True
+        else:
+            self.logger.info(f"No re-encrypt key detected")
+            created_new_encrypted_snapshot = False 
+            
         rds_client.modify_db_cluster_snapshot_attribute(
             DBClusterSnapshotIdentifier=backup_id,
             AttributeName='restore',
             ValuesToAdd=[aws_account_id]
         )
+        # if re-encryption occured, clean up old snapshot
+        if created_new_encrypted_snapshot:
+            # delete old snapshot
+            self.delete_backup(backup_resource)
+            self.logger.info(f"Cleaning up un-encrypted backup: {backup_resource.backup_id}")
+        
+        return backup_id
 
     def copy_backup_to_region(self, backup_id: str, region: str) -> str:
         local_region = boto3.session.Session().region_name
         client_local = AwsHelper.boto3_client('rds', arn=self.role_arn, external_id=self.role_external_id)
         rds_client = AwsHelper.boto3_client('rds', region_name=region)
         snapshots = client_local.describe_db_cluster_snapshots(DBClusterSnapshotIdentifier=backup_id)
         snapshot = snapshots['DBClusterSnapshots'][0]
-        rds_client.copy_db_cluster_snapshot(
-            SourceDBClusterSnapshotIdentifier=snapshot['DBClusterSnapshotArn'],
-            TargetDBClusterSnapshotIdentifier=backup_id,
-            SourceRegion=local_region,
-            # tags are created explicitly
-            CopyTags=False
-        )
+        backup_resource = self.get_backup_resource(local_region, backup_id)
+        kms_key = RuntimeConfig.get_reencrypt_kms_key_id(backup_resource.tags, self)
+        rds_client_params = {
+            'SourceDBClusterSnapshotIdentifier': snapshot['DBClusterSnapshotArn'],
+            'TargetDBClusterSnapshotIdentifier': backup_id,
+            'SourceRegion': local_region,
+            'CopyTags': False
+        }
+        # add kms key params if re-encrypt key is defined
+        if kms_key is not None:
+            backup_id = f'{backup_id}-re-encrypted'
+            rds_client_params['KmsKeyId'] = kms_key
+            rds_client_params['CopyTags'] = True
+            rds_client_params['TargetDBClusterSnapshotIdentifier'] = backup_id
+                       
+        rds_client.copy_db_cluster_snapshot(**rds_client_params)
         return backup_id
 
     def copy_shared_backup(self, source_account: str, source_backup: BackupResource):
         rds_client = AwsHelper.boto3_client('rds', arn=self.role_arn, external_id=self.role_external_id)
         # copying of tags happens outside this method
         source_arn = f"arn:aws:rds:{source_backup.region}:{source_backup.account_id}:cluster-snapshot:{source_backup.backup_id}"
 
@@ -199,20 +251,22 @@
         :param rds_client: boto3 rds service
         :return: all RDS instances within region for given boto3 client
         """
         # list of resource models
         db_clusters = []
         # temporary list of api models, as calls are batched
         temp_clusters = rds_client.describe_db_clusters()
+        
         db_clusters.extend(temp_clusters['DBClusters'])
         # collect database instances
         while 'Marker' in temp_clusters:
             temp_clusters = rds_client.describe_db_clusters(Marker=temp_clusters['Marker'])
             db_clusters.extend(temp_clusters['DBClusters'])
 
+        db_clusters = [cluster for cluster in db_clusters if cluster.get('Engine') != 'docdb']
         return db_clusters
 
     def get_shelvery_backups_only(self, all_snapshots, backup_tag_prefix, rds_client):
         """
         :param all_snapshots: all snapshots within region
         :param backup_tag_prefix:  prefix of shelvery backup system
         :param rds_client:  amazon boto3 rds client
@@ -246,14 +300,16 @@
         tmp_snapshots = rds_client.describe_db_cluster_snapshots(SnapshotType='manual')
         all_snapshots.extend(tmp_snapshots['DBClusterSnapshots'])
 
         while 'Marker' in tmp_snapshots:
             self.logger.info(f"Collected {len(tmp_snapshots['DBClusterSnapshots'])} manual snapshots. Continuing collection...")
             tmp_snapshots = rds_client.describe_db_cluster_snapshots(SnapshotType='manual', Marker=tmp_snapshots['Marker'])
             all_snapshots.extend(tmp_snapshots['DBClusterSnapshots'])
+            
+        all_snapshots = [snapshot for snapshot in all_snapshots if snapshot.get('Engine') != 'docdb']
 
         self.logger.info(f"Collected {len(all_snapshots)} manual snapshots.")
         self.populate_snap_entity_resource(all_snapshots)
 
         return all_snapshots
 
     def populate_snap_entity_resource(self, all_snapshots):
```

### Comparing `shelvery-0.9.7/shelvery/redshift_backup.py` & `shelvery-0.9.8/shelvery/redshift_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery/runtime_config.py` & `shelvery-0.9.8/shelvery/runtime_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     shelvery_ignore_invalid_resource_state - ignore exceptions due to the resource being in a unavailable state,
                                              such as shutdown, rebooting.
                                              
     shelvery_encrypt_copy - when copying a shared unencrypted snapshot, encrypt the shapshot. 
                             when enabled 'shelvery_copy_kms_key_id' must also be set.
     shelvery_copy_kms_key_id - when copying a shared snapshot, you can specify a different kms key used to encrypt the original snapshot.
                                Note that when copying to a new key, the shelvery requires access to both the new key and the original key.
+    shelvery_reencrypt_kms_key_id - when re-encrypting a snapshot with a new KMS key before sharing it to a new account.               
     """
 
     DEFAULT_KEEP_DAILY = 14
     DEFAULT_KEEP_WEEKLY = 8
     DEFAULT_KEEP_MONTHLY = 12
     DEFAULT_KEEP_YEARLY = 10
 
@@ -98,15 +99,16 @@
         'role_external_id': None,
         'shelvery_copy_resource_tags': True,
         'shelvery_exluded_resource_tag_keys': None,
         'shelvery_sqs_queue_url': None,
         'shelvery_sqs_queue_wait_period': 0,
         'shelvery_ignore_invalid_resource_state': False,
         'shelvery_encrypt_copy': False,
-        'shelvery_copy_kms_key_id': None
+        'shelvery_copy_kms_key_id': None,
+        'shelvery_reencrypt_kms_key_id': None
     }
 
     @classmethod
     def get_conf_value(cls, key: str, resource_tags=None, lambda_payload=None):
         # priority 3 are resource tags
         if resource_tags is not None:
             tag_key = f"shelvery:config:{key}"
@@ -330,8 +332,12 @@
     
     @classmethod
     def get_encrypt_copy(cls, resource_tags, engine):
         return cls.get_conf_value('shelvery_encrypt_copy', resource_tags, engine.lambda_payload)
     
     @classmethod
     def get_copy_kms_key_id(cls, resource_tags, engine):
-        return cls.get_conf_value('shelvery_copy_kms_key_id', resource_tags, engine.lambda_payload)
+        return cls.get_conf_value('shelvery_copy_kms_key_id', resource_tags, engine.lambda_payload)
+    
+    @classmethod
+    def get_reencrypt_kms_key_id(cls, resource_tags, engine):
+        return cls.get_conf_value('shelvery_reencrypt_kms_key_id', resource_tags, engine.lambda_payload)
```

### Comparing `shelvery-0.9.7/shelvery/shelvery_invoker.py` & `shelvery-0.9.8/shelvery/shelvery_invoker.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery.egg-info/PKG-INFO` & `shelvery-0.9.8/shelvery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: shelvery
-Version: 0.9.7
+Version: 0.9.8
 Summary: Backup manager for AWS EBS and AWS RDS services
 Home-page: http://github.com/base2Services/shelvery-aws-backups
 Author: Base2Services R&D
 Author-email: itsupport@base2services.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: aws backup lambda ebs rds ami
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Archiving :: Backup
 Requires-Python: >=3.6
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `shelvery-0.9.7/shelvery.egg-info/SOURCES.txt` & `shelvery-0.9.8/shelvery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery_cli/__main__.py` & `shelvery-0.9.8/shelvery_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.7/shelvery_lambda/lambda_handler.py` & `shelvery-0.9.8/shelvery_lambda/lambda_handler.py`

 * *Files identical despite different names*


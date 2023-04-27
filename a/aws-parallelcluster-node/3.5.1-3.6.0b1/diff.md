# Comparing `tmp/aws-parallelcluster-node-3.5.1.tar.gz` & `tmp/aws-parallelcluster-node-3.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-node-3.5.1.tar", last modified: Tue Mar 28 16:54:15 2023, max compression
+gzip compressed data, was "aws-parallelcluster-node-3.6.0b1.tar", last modified: Thu Apr 27 20:57:52 2023, max compression
```

## Comparing `aws-parallelcluster-node-3.5.1.tar` & `aws-parallelcluster-node-3.6.0b1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.669905 aws-parallelcluster-node-3.5.1/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11358 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/LICENSE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      102 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/NOTICE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      732 2023-03-28 16:54:15.665905 aws-parallelcluster-node-3.5.1/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      748 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/README.md
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-03-28 16:54:15.669905 aws-parallelcluster-node-3.5.1/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2298 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.661905 aws-parallelcluster-node-3.5.1/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.661905 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      732 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1270 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      257 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       30 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       20 2023-03-28 16:54:15.000000 aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.665905 aws-parallelcluster-node-3.5.1/src/common/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/common/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.665905 aws-parallelcluster-node-3.5.1/src/common/schedulers/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/common/schedulers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16398 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/common/schedulers/slurm_commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      733 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/common/time_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11793 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/common/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.665905 aws-parallelcluster-node-3.5.1/src/slurm_plugin/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    62690 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/clustermgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5071 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9891 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/computemgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3675 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/console_logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17448 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/fleet_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6564 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    22094 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/instance_manager.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 16:54:15.665905 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      777 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      343 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      382 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      368 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      369 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10640 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/resume.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    22507 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/slurm_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3658 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/suspend.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2711 2023-03-28 14:46:25.000000 aws-parallelcluster-node-3.5.1/src/slurm_plugin/task_executor.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11358 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/LICENSE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      102 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/NOTICE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      734 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      748 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/README.md
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2300 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.432629 aws-parallelcluster-node-3.6.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      734 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1338 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      257 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       30 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       20 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/common/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1284 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/ec2_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16552 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/slurm_commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      733 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/time_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11793 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    31273 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/cluster_event_publisher.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    63899 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/clustermgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5071 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9891 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/computemgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4232 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/console_logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17504 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6565 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    22150 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/instance_manager.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1117 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      343 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      382 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      710 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      369 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11351 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/resume.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25616 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/slurm_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3658 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/suspend.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3268 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/task_executor.py
```

### Comparing `aws-parallelcluster-node-3.5.1/LICENSE.txt` & `aws-parallelcluster-node-3.6.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/PKG-INFO` & `aws-parallelcluster-node-3.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.5.1
+Version: 3.6.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.5.1/README.md` & `aws-parallelcluster-node-3.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/setup.py` & `aws-parallelcluster-node-3.6.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 console_scripts = [
     "slurm_resume = slurm_plugin.resume:main",
     "slurm_suspend = slurm_plugin.suspend:main",
     "slurm_fleet_status_manager = slurm_plugin.fleet_status_manager:main",
     "clustermgtd = slurm_plugin.clustermgtd:main",
     "computemgtd = slurm_plugin.computemgtd:main",
 ]
-version = "3.5.1"
+version = "3.6.0b1"
 requires = ["boto3>=1.7.55", "retrying>=1.3.3"]
 
 setup(
     name="aws-parallelcluster-node",
     version=version,
     author="Amazon Web Services",
     description="aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.",
```

### Comparing `aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/PKG-INFO` & `aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.5.1
+Version: 3.6.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.5.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt` & `aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 src/aws_parallelcluster_node.egg-info/SOURCES.txt
 src/aws_parallelcluster_node.egg-info/dependency_links.txt
 src/aws_parallelcluster_node.egg-info/entry_points.txt
 src/aws_parallelcluster_node.egg-info/not-zip-safe
 src/aws_parallelcluster_node.egg-info/requires.txt
 src/aws_parallelcluster_node.egg-info/top_level.txt
 src/common/__init__.py
+src/common/ec2_utils.py
 src/common/time_utils.py
 src/common/utils.py
 src/common/schedulers/__init__.py
 src/common/schedulers/slurm_commands.py
 src/slurm_plugin/__init__.py
+src/slurm_plugin/cluster_event_publisher.py
 src/slurm_plugin/clustermgtd.py
 src/slurm_plugin/common.py
 src/slurm_plugin/computemgtd.py
 src/slurm_plugin/console_logger.py
 src/slurm_plugin/fleet_manager.py
 src/slurm_plugin/fleet_status_manager.py
 src/slurm_plugin/instance_manager.py
```

### Comparing `aws-parallelcluster-node-3.5.1/src/common/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/common/schedulers/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/common/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/common/schedulers/slurm_commands.py` & `aws-parallelcluster-node-3.6.0b1/src/common/schedulers/slurm_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 SLURM_BINARIES_DIR = os.environ.get("SLURM_BINARIES_DIR", "/opt/slurm/bin")
 SCONTROL = f"sudo {SLURM_BINARIES_DIR}/scontrol"
 SINFO = f"{SLURM_BINARIES_DIR}/sinfo"
 
 SCONTROL_OUTPUT_AWK_PARSER = (
     'awk \'BEGIN{{RS="\\n\\n" ; ORS="######\\n";}} {{print}}\' | '
     + "grep -oP '^(NodeName=\\S+)|(NodeAddr=\\S+)|(NodeHostName=\\S+)|(?<!Next)(State=\\S+)|"
-    + "(Partitions=\\S+)|(SlurmdStartTime=\\S+)|(Reason=.*)|(######)'"
+    + "(Partitions=\\S+)|(SlurmdStartTime=\\S+)|(LastBusyTime=\\S+)|(Reason=.*)|(######)'"
 )
 
 # Set default timeouts for running different slurm commands.
 # These timeouts might be needed when running on large scale
 DEFAULT_GET_INFO_COMMAND_TIMEOUT = 30
 DEFAULT_UPDATE_COMMAND_TIMEOUT = 60
 
@@ -329,15 +329,16 @@
     return ",".join(nodes)
 
 
 def _parse_nodes_info(slurm_node_info: str) -> List[SlurmNode]:
     """Parse slurm node info into SlurmNode objects."""
     # [ec2-user@ip-10-0-0-58 ~]$ /opt/slurm/bin/scontrol show nodes compute-dy-c5xlarge-[1-3],compute-dy-c5xlarge-50001\
     # | awk 'BEGIN{{RS="\n\n" ; ORS="######\n";}} {{print}}' | grep -oP "^(NodeName=\S+)|(NodeAddr=\S+)
-    # |(NodeHostName=\S+)|(?<!Next)(State=\S+)|(Partitions=\S+)|(SlurmdStartTime=\S+)|(Reason=.*)|(######)"
+    # |(NodeHostName=\S+)|(?<!Next)(State=\S+)|(Partitions=\S+)|(SlurmdStartTime=\S+)|(LastBusyTime=\\S+)|(Reason=.*)\
+    # |(######)"
     # NodeName=compute-dy-c5xlarge-1
     # NodeAddr=1.2.3.4
     # NodeHostName=compute-dy-c5xlarge-1
     # State=IDLE+CLOUD+POWER
     # Partitions=compute,compute2
     # SlurmdStartTime=2023-01-26T09:57:15
     # Reason=some reason
@@ -368,25 +369,28 @@
         "NodeName": "name",
         "NodeAddr": "nodeaddr",
         "NodeHostName": "nodehostname",
         "State": "state",
         "Partitions": "partitions",
         "Reason": "reason",
         "SlurmdStartTime": "slurmdstarttime",
+        "LastBusyTime": "lastbusytime",
     }
 
+    date_fields = ["SlurmdStartTime", "LastBusyTime"]
+
     node_info = slurm_node_info.split("######\n")
     slurm_nodes = []
     for node in node_info:
         lines = node.splitlines()
         kwargs = {}
         for line in lines:
             key, value = line.split("=")
-            if key == "SlurmdStartTime":
-                if value != "None":
+            if key in date_fields:
+                if value not in ["None", "Unknown"]:
                     value = datetime.strptime(value, "%Y-%m-%dT%H:%M:%S").astimezone(tz=timezone.utc)
                 else:
                     value = None
             kwargs[map_slurm_key_to_arg[key]] = value
         if lines:
             try:
                 if is_static_node(kwargs["name"]):
```

### Comparing `aws-parallelcluster-node-3.5.1/src/common/time_utils.py` & `aws-parallelcluster-node-3.6.0b1/src/common/time_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/common/utils.py` & `aws-parallelcluster-node-3.6.0b1/src/common/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/clustermgtd.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/clustermgtd.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     set_nodes_power_down,
     update_all_partitions,
     update_partitions,
 )
 from common.time_utils import seconds
 from common.utils import check_command_output, read_json, sleep_remaining_loop_time, time_is_up, wait_remaining_time
 from retrying import retry
+from slurm_plugin.cluster_event_publisher import ClusterEventPublisher
 from slurm_plugin.common import TIMESTAMP_FORMAT, log_exception, print_with_count
 from slurm_plugin.console_logger import ConsoleLogger
 from slurm_plugin.instance_manager import InstanceManager
 from slurm_plugin.slurm_resources import (
     CONFIG_FILE_DIR,
     ComputeResourceFailureEvent,
     DynamicNode,
@@ -55,14 +56,15 @@
 from slurm_plugin.task_executor import TaskExecutor
 
 LOOP_TIME = 60
 CONSOLE_OUTPUT_WAIT_TIME = 5 * 60
 MAXIMUM_TASK_BACKLOG = 100
 log = logging.getLogger(__name__)
 compute_logger = log.getChild("console_output")
+event_logger = log.getChild("events")
 
 
 class ComputeFleetStatus(Enum):
     """Represents the status of the cluster compute fleet."""
 
     STOPPED = "STOPPED"  # Fleet is stopped, partitions are inactive.
     RUNNING = "RUNNING"  # Fleet is running, partitions are active.
@@ -189,14 +191,15 @@
     def _get_basic_config(self, config):
         """Get basic config options."""
         self.region = config.get("clustermgtd", "region")
         self.cluster_name = config.get("clustermgtd", "cluster_name")
         self.dynamodb_table = config.get("clustermgtd", "dynamodb_table")
         self.head_node_private_ip = config.get("clustermgtd", "head_node_private_ip")
         self.head_node_hostname = config.get("clustermgtd", "head_node_hostname")
+        self.head_node_instance_id = config.get("clustermgtd", "instance_id", fallback="unknown")
 
         # Configure boto3 to retry 1 times by default
         self._boto3_retry = config.getint("clustermgtd", "boto3_retry", fallback=self.DEFAULTS.get("max_retry"))
         self._boto3_config = {"retries": {"max_attempts": self._boto3_retry, "mode": "standard"}}
         self.loop_time = config.getint("clustermgtd", "loop_time", fallback=self.DEFAULTS.get("loop_time"))
         self.disable_all_cluster_management = config.getboolean(
             "clustermgtd",
@@ -372,14 +375,15 @@
         self._compute_fleet_status = ComputeFleetStatus.RUNNING
         self._current_time = None
         self._config = None
         self._compute_fleet_status_manager = None
         self._instance_manager = None
         self._task_executor = None
         self._console_logger = None
+        self._event_publisher = None
         self.set_config(config)
 
     def set_config(self, config: ClustermgtdConfig):
         if self._config != config:
             log.info("Applying new clustermgtd config: %s", config)
 
             # If a new task executor is needed, the old one will be shutdown.
@@ -390,14 +394,17 @@
             # can be queried to determine how the task exited.
             # The shutdown on the task_executor is by default, non-blocking, so
             # it is possible for some tasks to continue executing even after the
             # shutdown request has returned.
             self._task_executor = self._initialize_executor(config)
 
             self._config = config
+            self._event_publisher = ClusterEventPublisher.create_with_default_publisher(
+                event_logger, config.cluster_name, "HeadNode", "clustermgtd", config.head_node_instance_id
+            )
             self._compute_fleet_status_manager = ComputeFleetStatusManager()
             self._instance_manager = self._initialize_instance_manager(config)
             self._console_logger = self._initialize_console_logger(config)
 
     def shutdown(self):
         if self._task_executor:
             self._task_executor.shutdown()
@@ -506,14 +513,15 @@
                     cluster_instances = self._get_ec2_instances()
                 except ClusterManager.EC2InstancesInfoUnavailable:
                     log.error("Unable to get instances info from EC2, no other action can be performed. Sleeping...")
                     return
                 log.debug("Current cluster instances in EC2: %s", cluster_instances)
                 partitions = list(partitions_name_map.values())
                 self._update_slurm_nodes_with_ec2_info(nodes, cluster_instances)
+                self._event_publisher.publish_compute_node_events(nodes, cluster_instances)
                 # Handle inactive partition and terminate backing instances
                 self._clean_up_inactive_partition(partitions)
                 # Perform health check actions
                 if not self._config.disable_all_health_checks:
                     self._perform_health_check_actions(partitions)
                 # Maintain slurm nodes
                 self._maintain_nodes(partitions_name_map, compute_resource_nodes_map)
@@ -703,24 +711,28 @@
 
         Check and return slurm nodes with unhealthy and healthy scheduler state, grouping unhealthy nodes
         by node type (static/dynamic).
         """
         unhealthy_static_nodes = []
         unhealthy_dynamic_nodes = []
         ice_compute_resources_and_nodes_map = {}
+        all_unhealthy_nodes = []
         for node in slurm_nodes:
             if not node.is_healthy(self._config.terminate_drain_nodes, self._config.terminate_down_nodes):
+                all_unhealthy_nodes.append(node)
+
                 if isinstance(node, StaticNode):
                     unhealthy_static_nodes.append(node)
                 elif self._config.disable_nodes_on_insufficient_capacity and node.is_ice():
                     ice_compute_resources_and_nodes_map.setdefault(node.queue_name, {}).setdefault(
                         node.compute_resource_name, []
                     ).append(node)
                 else:
                     unhealthy_dynamic_nodes.append(node)
+        self._event_publisher.publish_unhealthy_node_events(all_unhealthy_nodes)
         return (
             unhealthy_dynamic_nodes,
             unhealthy_static_nodes,
             ice_compute_resources_and_nodes_map,
         )
 
     def _increase_partitions_protected_failure_count(self, bootstrap_failure_nodes):
@@ -812,25 +824,34 @@
         if instances_to_terminate:
             log.info("Terminating instances backing unhealthy static nodes")
             self._instance_manager.delete_instances(
                 instances_to_terminate, terminate_batch_size=self._config.terminate_max_batch_size
             )
         log.info("Launching new instances for unhealthy static nodes")
         self._instance_manager.add_instances_for_nodes(
-            node_list, self._config.launch_max_batch_size, self._config.update_node_address
+            node_list,
+            self._config.launch_max_batch_size,
+            self._config.update_node_address,
         )
         # Add launched nodes to list of nodes being replaced, excluding any nodes that failed to launch
         failed_nodes = set().union(*self._instance_manager.failed_nodes.values())
         launched_nodes = set(node_list) - failed_nodes
         self._static_nodes_in_replacement |= launched_nodes
         log.info(
             "After node maintenance, following nodes are currently in replacement: %s",
             print_with_count(self._static_nodes_in_replacement),
         )
 
+        self._event_publisher.publish_unhealthy_static_node_events(
+            unhealthy_static_nodes,
+            self._static_nodes_in_replacement,
+            launched_nodes,
+            self._instance_manager.failed_nodes,
+        )
+
     @log_exception(log, "maintaining slurm nodes", catch_exception=Exception, raise_on_error=False)
     def _maintain_nodes(self, partitions_name_map, compute_resource_nodes_map):
         """
         Call functions to maintain unhealthy nodes.
 
         This function needs to handle the case that 2 slurm nodes have the same IP/nodeaddr.
         A list of slurm nodes is passed in and slurm node map with IP/nodeaddr as key should be avoided.
@@ -907,14 +928,15 @@
         # Find bootstrap failure nodes in unhealthy nodes
         bootstrap_failure_nodes = self._find_bootstrap_failure_nodes(active_nodes)
         # Find bootstrap failure nodes failing health check
         if bootstrap_failure_nodes:
             log.warning("Found the following bootstrap failure nodes: %s", print_with_count(bootstrap_failure_nodes))
             # Increase the partition failure count and add failed nodes to the set of bootstrap failure nodes.
             self._increase_partitions_protected_failure_count(bootstrap_failure_nodes)
+        self._event_publisher.publish_bootstrap_failure_events(bootstrap_failure_nodes)
 
     def _is_protected_mode_enabled(self):
         """When protected_failure_count is set to -1, disable protected mode."""
         if self._config.protected_failure_count <= 0:
             return False
         return True
 
@@ -963,17 +985,17 @@
                 "Cluster is in protected mode due to failures detected in node provisioning. "
                 "Please investigate the issue and then use 'pcluster update-compute-fleet --status START_REQUESTED' "
                 "command to re-enable the fleet."
             )
 
     def _handle_nodes_failing_health_check(self, nodes_failing_health_check: List[SlurmNode], health_check_type: str):
         # Place unhealthy node into drain, this operation is idempotent
+        nodes_name_failing_health_check = set()
+        nodes_name_recently_rebooted = set()
         if nodes_failing_health_check:
-            nodes_name_failing_health_check = set()
-            nodes_name_recently_rebooted = set()
             for node in nodes_failing_health_check:
                 # Do not consider nodes failing health checks as unhealthy if:
                 # 1. the node is still rebooting, OR
                 # 2. slurmd was recently restarted (less than health_check_timeout_after_slurmdstarttime seconds ago).
                 # In the implementation the logic is reversed to exploit the `and` in the if clause
                 if not node.is_reboot_issued() and time_is_up(
                     node.slurmdstarttime, self._current_time, self._config.health_check_timeout_after_slurmdstarttime
@@ -989,14 +1011,17 @@
                 )
                 set_nodes_drain(nodes_name_failing_health_check, reason=f"Node failing {health_check_type}")
             if len(nodes_name_recently_rebooted) > 0:
                 log.info(
                     "Ignoring health check failure due to reboot for nodes: %s",
                     nodes_name_recently_rebooted,
                 )
+        self._event_publisher.publish_nodes_failing_health_check_events(
+            health_check_type, nodes_name_failing_health_check
+        )
 
     def _handle_failed_health_check_nodes_in_replacement(self, active_nodes):
         failed_health_check_nodes_in_replacement = []
         for node in active_nodes:
             if node.is_static_nodes_in_replacement and node.is_failing_health_check:
                 failed_health_check_nodes_in_replacement.append(node.name)
 
@@ -1175,15 +1200,16 @@
                 for node in nodes:
                     if node.is_power() and not node.is_nodeaddr_set():
                         error_code = event.error_code
                         nodes_to_down.setdefault(error_code, []).append(node.name)
         if nodes_to_down:
             for error_code, node_list in nodes_to_down.items():
                 set_nodes_down(
-                    node_list, reason=f"(Code:{error_code})Temporarily disabling node due to insufficient capacity"
+                    node_list,
+                    reason=f"(Code:{error_code})Temporarily disabling node due to insufficient capacity",
                 )
 
     def _find_insufficient_capacity_timeout_expired_compute_resources(
         self,
     ) -> Dict[str, Dict[str, ComputeResourceFailureEvent]]:
         """Find compute resources which insufficient_capacity_timeout expired."""
         timeout_expired_cr = dict()
@@ -1195,15 +1221,15 @@
                     if not self._insufficient_capacity_compute_resources.get(queue_name):
                         self._insufficient_capacity_compute_resources.pop(queue_name)
         return timeout_expired_cr
 
     def _reset_insufficient_capacity_timeout_expired_nodes(
         self,
         timeout_expired_cr: Dict[str, Dict[str, ComputeResourceFailureEvent]],
-        ice_compute_resources_and_nodes_map: Dict[str, Dict[str, ComputeResourceFailureEvent]],
+        ice_compute_resources_and_nodes_map: Dict[str, Dict[str, List[SlurmNode]]],
     ):
         """Reset nodes in the compute resource which insufficient_capacity_timeout expired."""
         logging.info(
             "Reset the following compute resources because insufficient capacity timeout expired: %s",
             timeout_expired_cr,
         )
         nodes_to_power_down = []
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/common.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/computemgtd.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/computemgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/console_logger.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/console_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Copyright 2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License").
+# You may not use this file except in compliance with the
+# License. A copy of the License is located at
+#
+# http://aws.amazon.com/apache2.0/
+#
+# or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
+# OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
+# limitations under the License.
+
 import logging
 import re
 from typing import Any, Callable, Iterable
 
 import boto3
 from slurm_plugin.common import ComputeInstanceDescriptor, TaskController
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/fleet_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import copy
 import logging
 import time
 from abc import ABC, abstractmethod
 
 import boto3
 from botocore.exceptions import ClientError
+from common.ec2_utils import get_private_ip_address
 
 logger = logging.getLogger(__name__)
 
 
 class EC2Instance:
     def __init__(self, id, private_ip, hostname, launch_time):
         """Initialize slurm node with attributes."""
@@ -45,15 +46,15 @@
         return hash(self.id)
 
     @staticmethod
     def from_describe_instance_data(instance_info):
         try:
             return EC2Instance(
                 instance_info["InstanceId"],
-                instance_info["PrivateIpAddress"],
+                get_private_ip_address(instance_info),
                 instance_info["PrivateDnsName"].split(".")[0],
                 instance_info["LaunchTime"],
             )
         except KeyError as e:
             logger.error("Unable to retrieve EC2 instance info: %s", e)
             raise e
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/fleet_status_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_status_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             self._boto3_config["proxies"] = {"https": proxy}
         self.boto3_config = Config(**self._boto3_config)
 
         self.logging_config = config.get(
             "slurm_fleet_status_manager", "logging_config", fallback=self.DEFAULTS.get("logging_config")
         )
 
-        log.info(self.__repr__())
+        log.debug(self.__repr__())
 
 
 def _manage_fleet_status_transition(config, computefleet_status_data_path):
     computefleet_status = _get_computefleet_status(computefleet_status_data_path)
 
     if ComputeFleetStatus.is_stop_requested(computefleet_status):
         _stop_partitions(config)
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/instance_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/instance_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # In this file the input of the module subprocess is trusted.
 import subprocess  # nosec B404
 from typing import Iterable
 
 import boto3
 from botocore.config import Config
 from botocore.exceptions import ClientError
+from common.ec2_utils import get_private_ip_address
 from common.schedulers.slurm_commands import update_nodes
 from common.utils import grouper
 from slurm_plugin.common import ComputeInstanceDescriptor, log_exception, print_with_count
 from slurm_plugin.fleet_manager import EC2Instance, FleetManagerFactory
 from slurm_plugin.slurm_resources import (
     EC2_HEALTH_STATUS_UNHEALTHY_STATES,
     EC2_INSTANCE_ALIVE_STATES,
@@ -338,15 +339,15 @@
 
         instances = []
         for instance_info in filtered_iterator:
             try:
                 instances.append(
                     EC2Instance(
                         instance_info["InstanceId"],
-                        instance_info["PrivateIpAddress"],
+                        get_private_ip_address(instance_info),
                         instance_info["PrivateDnsName"].split(".")[0],
                         instance_info["LaunchTime"],
                     )
                 )
             except Exception as e:
                 logger.warning(
                     "Ignoring instance %s because not all EC2 info are available, exception: %s, message: %s",
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [loggers]
-keys=root,computeConsole
+keys=root,events
 
 [handlers]
-keys=streamHandler,computeConsoleHandler
+keys=fileHandler,eventsHandler
 
 [formatters]
-keys=defaultFormatter,computeConsoleFormatter
+keys=defaultFormatter,eventsFormatter
 
 [logger_root]
 level=INFO
-handlers=streamHandler
+handlers=fileHandler
 
 [formatter_defaultFormatter]
 format=%(asctime)s - [%(name)s:%(funcName)s] - %(levelname)s - %(message)s
 
-[handler_streamHandler]
-class=StreamHandler
+[handler_fileHandler]
+class=FileHandler
 level=INFO
 formatter=defaultFormatter
-args=(sys.stdout,)
+args=("/var/log/parallelcluster/slurm_resume.log",)
 
-[logger_computeConsole]
-level=INFO
-handlers=computeConsoleHandler
+[logger_events]
+level=WARNING
+handlers=eventsHandler
 propagate=0
-qualname=slurm_plugin.clustermgtd.console_output
+qualname=slurm_plugin.resume.events
 
-[formatter_computeConsoleFormatter]
-format=%(asctime)s - %(message)s
+[formatter_eventsFormatter]
+format=%(message)s
 
-[handler_computeConsoleHandler]
+[handler_eventsHandler]
 class=FileHandler
-level=INFO
-formatter=computeConsoleFormatter
-args=('/var/log/parallelcluster/compute_console_output.log', 'a', None, False)
+level=WARNING
+formatter=eventsFormatter
+args=('/var/log/parallelcluster/slurm_resume.events', 'a', None, False)
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/resume.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/resume.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from configparser import ConfigParser
 from datetime import datetime, timezone
 from logging.config import fileConfig
 
 from botocore.config import Config
 from common.schedulers.slurm_commands import get_nodes_info, set_nodes_down
 from common.utils import read_json
+from slurm_plugin.cluster_event_publisher import ClusterEventPublisher
 from slurm_plugin.common import is_clustermgtd_heartbeat_valid, print_with_count
 from slurm_plugin.instance_manager import InstanceManager
 from slurm_plugin.slurm_resources import CONFIG_FILE_DIR
 
 log = logging.getLogger(__name__)
+event_logger = log.getChild("events")
 
 
 class SlurmResumeConfig:
     DEFAULTS = {
         "max_retry": 1,
         "max_batch_size": 500,
         "update_node_address": True,
@@ -116,16 +118,17 @@
         self._boto3_retry = config.getint("slurm_resume", "boto3_retry", fallback=self.DEFAULTS.get("max_retry"))
         self._boto3_config = {"retries": {"max_attempts": self._boto3_retry, "mode": "standard"}}
         proxy = config.get("slurm_resume", "proxy", fallback=self.DEFAULTS.get("proxy"))
         if proxy != "NONE":
             self._boto3_config["proxies"] = {"https": proxy}
         self.boto3_config = Config(**self._boto3_config)
         self.logging_config = config.get("slurm_resume", "logging_config", fallback=self.DEFAULTS.get("logging_config"))
+        self.head_node_instance_id = config.get("slurm_resume", "instance_id", fallback="unknown")
 
-        log.info(self.__repr__())
+        log.debug(self.__repr__())
 
 
 def _handle_failed_nodes(node_list, reason="Failure when resuming nodes"):
     """
     Fall back mechanism to handle failure when launching instances.
 
     When encountering a failure, want slurm to deallocate current nodes,
@@ -157,16 +160,20 @@
             "Please check clustermgtd log for error.\n"
             "Not launching nodes %s",
             arg_nodes,
         )
         _handle_failed_nodes(arg_nodes)
         return
     log.info("Launching EC2 instances for the following Slurm nodes: %s", arg_nodes)
-    node_list = [node.name for node in get_nodes_info(arg_nodes)]
-    log.debug("Retrieved nodelist: %s", node_list)
+    node_list = []
+    node_list_with_status = []
+    for node in get_nodes_info(arg_nodes):
+        node_list.append(node.name)
+        node_list_with_status.append((node.name, node.state_string))
+    log.info("Current state of Slurm nodes to resume: %s", node_list_with_status)
 
     instance_manager = InstanceManager(
         resume_config.region,
         resume_config.cluster_name,
         resume_config.boto3_config,
         table_name=resume_config.dynamodb_table,
         hosted_zone=resume_config.hosted_zone,
@@ -192,14 +199,23 @@
         log.error(
             "Failed to launch following nodes, setting nodes to down: %s",
             print_with_count(failed_nodes),
         )
         for error_code, node_list in instance_manager.failed_nodes.items():
             _handle_failed_nodes(node_list, reason=f"(Code:{error_code})Failure when resuming nodes")
 
+        event_publisher = ClusterEventPublisher.create_with_default_publisher(
+            event_logger,
+            resume_config.cluster_name,
+            "HeadNode",
+            "slurm-resume",
+            resume_config.head_node_instance_id,
+        )
+        event_publisher.publish_node_launch_events(instance_manager.failed_nodes)
+
 
 def main():
     default_log_file = "/var/log/parallelcluster/slurm_resume.log"
     logging.basicConfig(
         filename=default_log_file,
         level=logging.INFO,
         format="%(asctime)s - [%(name)s:%(funcName)s] - %(levelname)s - %(message)s",
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/slurm_resources.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/slurm_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,18 +90,22 @@
     SLURM_SCONTROL_POWERING_DOWN_STATE = "POWERING_DOWN"
     SLURM_SCONTROL_POWER_DOWN_STATE = "POWER_DOWN"
     SLURM_SCONTROL_POWERED_DOWN_STATE = "POWERED_DOWN"
     SLURM_SCONTROL_POWER_UP_STATE = "POWERING_UP"
     SLURM_SCONTROL_ONLINE_STATES = {"IDLE+CLOUD", "MIXED+CLOUD", "ALLOCATED+CLOUD", "COMPLETING+CLOUD"}
     SLURM_SCONTROL_POWER_WITH_JOB_STATE = {"MIXED", "CLOUD", "POWERED_DOWN"}
     SLURM_SCONTROL_RESUME_FAILED_STATE = {"DOWN", "CLOUD", "POWERED_DOWN", "NOT_RESPONDING"}
+    SLURM_SCONTROL_NODE_DOWN_NOT_RESPONDING_STATE = {"DOWN", "CLOUD", "NOT_RESPONDING"}
     # Due to a bug in Slurm a powered down node can enter IDLE+CLOUD+POWER_DOWN+POWERED_DOWN state
     SLURM_SCONTROL_POWER_STATES = [{"IDLE", "CLOUD", "POWERED_DOWN"}, {"IDLE", "CLOUD", "POWERED_DOWN", "POWER_DOWN"}]
     SLURM_SCONTROL_REBOOT_REQUESTED_STATE = "REBOOT_REQUESTED"
     SLURM_SCONTROL_REBOOT_ISSUED_STATE = "REBOOT_ISSUED"
+    SLURM_SCONTROL_INVALID_REGISTRATION_STATE = "INVALID_REG"
+
+    SLURM_SCONTROL_NODE_DOWN_NOT_RESPONDING_REASON = re.compile(r"Not responding \[slurm@.+\]")
 
     EC2_ICE_ERROR_CODES = {
         "InsufficientInstanceCapacity",
         "InsufficientHostCapacity",
         "InsufficientReservedInstanceCapacity",
         "MaxSpotInstanceCountExceeded",
         "Unsupported",
@@ -114,25 +118,27 @@
         nodeaddr,
         nodehostname,
         state,
         partitions=None,
         reason=None,
         instance=None,
         slurmdstarttime: datetime = None,
+        lastbusytime: datetime = None,
     ):
         """Initialize slurm node with attributes."""
         self.name = name
         self.nodeaddr = nodeaddr
         self.nodehostname = nodehostname
         self.state_string = state
         self.states = set(state.split("+"))
         self.partitions = partitions.strip().split(",") if partitions else None
         self.reason = reason
         self.instance = instance
         self.slurmdstarttime = slurmdstarttime
+        self.lastbusytime = lastbusytime
         self.is_static_nodes_in_replacement = False
         self.is_being_replaced = False
         self._is_replacement_timeout = False
         self.is_failing_health_check = False
         self.error_code = self._parse_error_code()
         self.queue_name, self._node_type, self.compute_resource_name = parse_nodename(name)
 
@@ -172,14 +178,22 @@
         """Check if slurm node is in powering down state."""
         return self.SLURM_SCONTROL_POWERING_DOWN_STATE in self.states
 
     def is_powered_down(self):
         """Check if slurm node is in powered down state."""
         return self.SLURM_SCONTROL_POWERED_DOWN_STATE in self.states
 
+    def is_idle(self):
+        """
+        Determine if node as idle.
+
+        A node is idle if it has a backing instance, LastBusyTime has a value from scontrol, and is in IDLE state.
+        """
+        return self.instance and self.lastbusytime and self.SLURM_SCONTROL_IDLE_STATE in self.states
+
     def is_power(self):
         """Check if slurm node is in power state."""
         return self.states in self.SLURM_SCONTROL_POWER_STATES
 
     def is_down(self):
         """Check if slurm node is in a down state."""
         return (
@@ -212,15 +226,24 @@
         """Check if slurm node is running a job but not in configuring job state."""
         return not self.is_powering_up() and self.has_job() and not self.is_power_with_job()
 
     def is_resume_failed(self):
         """Check if node resume timeout expires."""
         return self.states == self.SLURM_SCONTROL_RESUME_FAILED_STATE
 
-    def is_poweing_up_idle(self):
+    def is_down_not_responding(self):
+        """Check if node was set to down by Slurm because it was not responding."""
+        return (
+            self.states == self.SLURM_SCONTROL_NODE_DOWN_NOT_RESPONDING_STATE
+            and self.SLURM_SCONTROL_NODE_DOWN_NOT_RESPONDING_REASON.match(self.reason)
+            if self.reason
+            else False
+        )
+
+    def is_powering_up_idle(self):
         """Check if node is in IDLE# state."""
         return self.SLURM_SCONTROL_IDLE_STATE in self.states and self.is_powering_up()
 
     def is_ice(self):
         return self.error_code in self.EC2_ICE_ERROR_CODES
 
     def is_reboot_requested(self):
@@ -241,14 +264,18 @@
                 "Node state check: node %s is currently rebooting, ignoring, node state: %s",
                 self,
                 self.state_string,
             )
             cond = True
         return cond
 
+    def is_invalid_slurm_registration(self):
+        """Check if a slurm node has failed registration with the Slurm management daemon."""
+        return self.SLURM_SCONTROL_INVALID_REGISTRATION_STATE in self.states
+
     @abstractmethod
     def is_state_healthy(self, terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=True):
         """Check if a slurm node's scheduler state is considered healthy."""
         pass
 
     @abstractmethod
     def is_bootstrap_failure(self):
@@ -258,14 +285,19 @@
         Here's the cases of bootstrap error we are checking:
         Bootstrap error that causes instance to self terminate.
         Bootstrap error that prevents instance from joining cluster but does not cause self termination.
         """
         pass
 
     @abstractmethod
+    def is_bootstrap_timeout(self):
+        """Check if slurm node timed out while waiting for backing instance to bootstrap."""
+        pass
+
+    @abstractmethod
     def is_healthy(self, terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=True):
         """Check if a slurm node is considered healthy."""
         pass
 
     def is_powering_down_with_nodeaddr(self):
         """Check if a slurm node is a powering down node with instance backing."""
         # Node in POWERED_DOWN with nodeaddr still set, may have not been seen during the POWERING_DOWN transition
@@ -286,14 +318,17 @@
         return True
 
     @abstractmethod
     def needs_reset_when_inactive(self):
         """Check if the node need to be reset if node is inactive."""
         pass
 
+    def idle_time(self, current_time: datetime) -> float:
+        return (current_time - self.lastbusytime).total_seconds() if self.lastbusytime else 0
+
     def _parse_error_code(self):
         """Parse RunInstance error code from node reason."""
         if self.reason and self.reason.startswith("(Code:"):
             index_of_bracket = self.reason.find(")")
             error_code = self.reason[len("(Code:") : index_of_bracket]  # noqa E203: whitespace before ':'
             return error_code
         return None
@@ -313,23 +348,42 @@
 
     def __hash__(self):
         return hash(self.name)
 
 
 class StaticNode(SlurmNode):
     def __init__(
-        self, name, nodeaddr, nodehostname, state, partitions=None, reason=None, instance=None, slurmdstarttime=None
+        self,
+        name,
+        nodeaddr,
+        nodehostname,
+        state,
+        partitions=None,
+        reason=None,
+        instance=None,
+        slurmdstarttime=None,
+        lastbusytime=None,
     ):
         """Initialize slurm node with attributes."""
-        super().__init__(name, nodeaddr, nodehostname, state, partitions, reason, instance, slurmdstarttime)
+        super().__init__(
+            name,
+            nodeaddr,
+            nodehostname,
+            state,
+            partitions,
+            reason,
+            instance,
+            slurmdstarttime,
+            lastbusytime=lastbusytime,
+        )
 
     def is_healthy(self, terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=True):
         """Check if a slurm node is considered healthy."""
         return (
-            self._is_static_node_configuration_valid(log_warn_if_unhealthy=log_warn_if_unhealthy)
+            self._is_static_node_ip_configuration_valid(log_warn_if_unhealthy=log_warn_if_unhealthy)
             and self.is_backing_instance_valid(log_warn_if_unhealthy=log_warn_if_unhealthy)
             and self.is_state_healthy(
                 terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=log_warn_if_unhealthy
             )
         )
 
     def is_state_healthy(self, terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=True):
@@ -361,15 +415,15 @@
                 return True
             else:
                 if log_warn_if_unhealthy:
                     logger.warning("Node state check: node %s in DOWN, node state: %s", self, self.state_string)
                 return False
         return True
 
-    def _is_static_node_configuration_valid(self, log_warn_if_unhealthy=True):
+    def _is_static_node_ip_configuration_valid(self, log_warn_if_unhealthy=True):
         """Check if static node is configured with a private IP."""
         if not self.is_nodeaddr_set():
             if log_warn_if_unhealthy:
                 logger.warning(
                     "Node state check: static node without nodeaddr set, node %s, node state %s:",
                     self,
                     self.state_string,
@@ -384,15 +438,15 @@
             logger.warning(
                 "Node bootstrap error: Node %s is currently in replacement and no backing instance, node state %s:",
                 self,
                 self.state_string,
             )
             return True
             # Replacement timeout expires for node in replacement
-        elif self._is_replacement_timeout:
+        elif self.is_bootstrap_timeout():
             logger.warning(
                 "Node bootstrap error: Replacement timeout expires for node %s in replacement, node state %s:",
                 self,
                 self.state_string,
             )
             return True
         elif self.is_failing_health_check and self.is_static_nodes_in_replacement:
@@ -400,25 +454,48 @@
                 "Node bootstrap error: Node %s failed during bootstrap when performing health check, node state %s:",
                 self,
                 self.state_string,
             )
             return True
         return False
 
+    def is_bootstrap_timeout(self):
+        """Check if slurm node timed out waiting for backing instance to bootstrap."""
+        return self._is_replacement_timeout
+
     def needs_reset_when_inactive(self):
         """Check if the node need to be reset if node is inactive."""
         return self.is_nodeaddr_set()
 
 
 class DynamicNode(SlurmNode):
     def __init__(
-        self, name, nodeaddr, nodehostname, state, partitions=None, reason=None, instance=None, slurmdstarttime=None
+        self,
+        name,
+        nodeaddr,
+        nodehostname,
+        state,
+        partitions=None,
+        reason=None,
+        instance=None,
+        slurmdstarttime=None,
+        lastbusytime=None,
     ):
         """Initialize slurm node with attributes."""
-        super().__init__(name, nodeaddr, nodehostname, state, partitions, reason, instance, slurmdstarttime)
+        super().__init__(
+            name,
+            nodeaddr,
+            nodehostname,
+            state,
+            partitions,
+            reason,
+            instance,
+            slurmdstarttime,
+            lastbusytime=lastbusytime,
+        )
 
     def is_state_healthy(self, terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=True):
         """Check if a slurm node's scheduler state is considered healthy."""
         # Check if node is rebooting: if so, the node is healthy
         if self.is_rebooting():
             return True
         # Check to see if node is in DRAINED, ignoring any node currently being replaced or in POWER_DOWN
@@ -442,40 +519,55 @@
         return self.is_backing_instance_valid(log_warn_if_unhealthy=log_warn_if_unhealthy) and self.is_state_healthy(
             terminate_drain_nodes, terminate_down_nodes, log_warn_if_unhealthy=log_warn_if_unhealthy
         )
 
     def is_bootstrap_failure(self):
         """Check if a slurm node has boostrap failure."""
         # no backing instance + [working state]# in node state
-        if (self.is_configuring_job() or self.is_poweing_up_idle()) and not self.is_backing_instance_valid(
+        if (self.is_configuring_job() or self.is_powering_up_idle()) and not self.is_backing_instance_valid(
             log_warn_if_unhealthy=False
         ):
             logger.warning(
                 "Node bootstrap error: Node %s is in power up state without valid backing instance, node state: %s",
                 self,
                 self.state_string,
             )
             return True
         # Dynamic node in DOWN+CLOUD+POWERED_DOWN+NOT_RESPONDING state
-        elif self.is_resume_failed() and self.is_nodeaddr_set():
+        elif self.is_bootstrap_timeout():
             # We need to check if nodeaddr is set to avoid counting powering up nodes as bootstrap failure nodes during
             # cluster start/stop.
             logger.warning(
                 "Node bootstrap error: Resume timeout expires for node %s, node state: %s", self, self.state_string
             )
             return True
         elif self.is_failing_health_check and self.is_powering_up():
             logger.warning(
                 "Node bootstrap error: Node %s failed during bootstrap when performing health check, node state: %s",
                 self,
                 self.state_string,
             )
             return True
+        # Consider the invalid registration as a bootstrap failure event, but only the first time it is registered.
+        # After this, clustermgtd will mark the node as unhealthy and power it down.
+        # This does not clear the INVALID_REG flag immediately: this will happen only when the node is fully powered
+        # down. Therefore we exclude the nodes that are still pending powering down from this check.
+        elif self.is_invalid_slurm_registration() and not (self.is_power_down() or self.is_powering_down()):
+            logger.warning(
+                "Node bootstrap error: Node %s failed to register to the Slurm management daemon, node state: %s",
+                self,
+                self.state_string,
+            )
+            return True
         return False
 
+    def is_bootstrap_timeout(self):
+        """Check if slurm node timed out waiting for backing instance to bootstrap."""
+        return self.is_resume_failed() and self.is_nodeaddr_set()
+
     def needs_reset_when_inactive(self):
         """Check if the node need to be reset if node is inactive."""
         return self.is_nodeaddr_set() or (not (self.is_power() or self.is_powering_down() or self.is_down()))
 
 
 class EC2InstanceHealthState:
     def __init__(self, id, state, instance_status, system_status, scheduled_events):
```

### Comparing `aws-parallelcluster-node-3.5.1/src/slurm_plugin/suspend.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/suspend.py`

 * *Files identical despite different names*


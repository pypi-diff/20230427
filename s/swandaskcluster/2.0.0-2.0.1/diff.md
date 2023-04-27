# Comparing `tmp/swandaskcluster-2.0.0.tar.gz` & `tmp/swandaskcluster-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swandaskcluster-2.0.0.tar", last modified: Tue Mar 21 14:28:42 2023, max compression
+gzip compressed data, was "swandaskcluster-2.0.1.tar", last modified: Thu Apr 27 14:47:01 2023, max compression
```

## Comparing `swandaskcluster-2.0.0.tar` & `swandaskcluster-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:28:42.766460 swandaskcluster-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-21 14:28:42.766460 swandaskcluster-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 14:28:42.766460 swandaskcluster-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:28:42.766460 swandaskcluster-2.0.0/swandaskcluster/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/jobqueue-swan.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-21 14:28:27.000000 swandaskcluster-2.0.0/swandaskcluster/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:28:42.766460 swandaskcluster-2.0.0/swandaskcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-21 14:28:42.000000 swandaskcluster-2.0.0/swandaskcluster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:47:01.310405 swandaskcluster-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-27 14:47:01.310405 swandaskcluster-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:47:01.310405 swandaskcluster-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:47:01.306404 swandaskcluster-2.0.1/swandaskcluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/jobqueue-swan.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-27 14:46:46.000000 swandaskcluster-2.0.1/swandaskcluster/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:47:01.310405 swandaskcluster-2.0.1/swandaskcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 14:47:01.000000 swandaskcluster-2.0.1/swandaskcluster.egg-info/top_level.txt
```

### Comparing `swandaskcluster-2.0.0/LICENSE` & `swandaskcluster-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swandaskcluster-2.0.0/setup.py` & `swandaskcluster-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `swandaskcluster-2.0.0/swandaskcluster/cluster.py` & `swandaskcluster-2.0.1/swandaskcluster/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,36 +53,40 @@
     Class that configures an HTCondorCluster to be used from SWAN.
     '''
 
     config_name = 'swan'
     job_cls = SwanHTCondorJob
 
     def __init__(self,
-                 worker_image = None,
                  job_extra = {},
                  scheduler_options = {},
                  **base_class_kwargs):
         '''
         Configures the Dask workers to be used by SWAN clients and dynamically
         obtains the necessary addresses for a Dask scheduler that runs in a
         SWAN user session.
         '''
 
         # Worker configuration
-        worker_image = worker_image or \
-                       dask.config.get(
+        worker_image = dask.config.get(
                            f'jobqueue.{self.config_name}.worker-image')
+        tag = os.getenv('VERSION_DOCKER_IMAGE', None)
+        if tag is None:
+            raise SwanDaskClusterException(
+                'Error when creating a SwanHTCondorCluster: could not '
+                'find the tag to be used for the worker image')
+        worker_image += f':{tag}'
 
         config_job_extra = dask.config.get(
                                f'jobqueue.{self.config_name}.job-extra')
 
         # TODO: set a value for 'log_directory'
 
         # Security
-        security = self._get_security()
+        security = self.security()
         if security is None:
             raise SwanDaskClusterException(
                 'Error when creating a SwanHTCondorCluster: could not '
                 'configure TLS')
         tls_job_extra = self._get_tls_job_extra(security)
         protocol = 'tls'
 
@@ -125,15 +129,16 @@
             self._scheduler_config.release_port()
             raise SwanDaskClusterException(
                 'Error when creating a SwanHTCondorCluster') from e
 
         # The scheduler was successfully created, we can keep the port
         self._scheduler_config.reserve_port()
 
-    def _get_security(self):
+    @classmethod
+    def security(cls):
         '''
         Constructs and returns a Dask Security object if a directory with
         pregenerated certificates is found. Otherwise it logs an error and
         returns None.
         The certificates should have been generated during user session
         startup, if the user selected to work with an HTCondor cluster.
         Client, scheduler and workers share the same certificate, signed by the
```

### Comparing `swandaskcluster-2.0.0/swandaskcluster/utils.py` & `swandaskcluster-2.0.1/swandaskcluster/utils.py`

 * *Files identical despite different names*


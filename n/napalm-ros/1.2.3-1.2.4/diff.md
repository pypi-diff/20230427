# Comparing `tmp/napalm-ros-1.2.3.tar.gz` & `tmp/napalm-ros-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/napalm-ros/napalm-ros/dist/.tmp-h1broeim/napalm-ros-1.2.3.tar", last modified: Wed Mar 15 14:44:53 2023, max compression
+gzip compressed data, was "/home/runner/work/napalm-ros/napalm-ros/dist/.tmp-9aqok8s0/napalm-ros-1.2.4.tar", last modified: Thu Apr 27 15:25:19 2023, max compression
```

## Comparing `napalm-ros-1.2.3.tar` & `napalm-ros-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/napalm_ros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/napalm_ros/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    23916 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/napalm_ros/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/napalm_ros/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/napalm_ros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 14:44:11.000000 napalm-ros-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 14:44:53.000000 napalm-ros-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/napalm_ros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/napalm_ros/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24124 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/napalm_ros/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/napalm_ros/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/napalm_ros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 15:24:37.000000 napalm-ros-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:25:19.000000 napalm-ros-1.2.4/setup.cfg
```

### Comparing `napalm-ros-1.2.3/PKG-INFO` & `napalm-ros-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-ros
-Version: 1.2.3
+Version: 1.2.4
 Summary: Network Automation and Programmability Abstraction Layer driver for Mikrotik ROS
 Author-email: Łukasz Kostka <lukasz.g.kostka@gmail.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-ros
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-ros/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `napalm-ros-1.2.3/README.md` & `napalm-ros-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `napalm-ros-1.2.3/napalm_ros/query.py` & `napalm-ros-1.2.4/napalm_ros/query.py`

 * *Files identical despite different names*

### Comparing `napalm-ros-1.2.3/napalm_ros/ros.py` & `napalm-ros-1.2.4/napalm_ros/ros.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
                 ctx.check_hostname = self.optional_args.get('check_hostname', True)
 
             self.optional_args['ssl_wrapper'] = ctx.wrap_socket
 
         self.ssl_wrapper = self.optional_args.get('ssl_wrapper', librouteros.DEFAULTS['ssl_wrapper'])
         self.port = self.optional_args.get('port', 8729 if 'ssl_wrapper' in self.optional_args else 8728)
         self.ssh_port = self.optional_args.get('ssh_port', 22)
+        self.paramiko_look_for_keys = self.optional_args.get('paramiko_look_for_keys', False)
         self.api = None
         self.ssh = None
 
     def close(self):
         self.api.close()
 
     def is_alive(self):
@@ -366,15 +367,21 @@
         version = version_parse(version['installed-version'])
         if full:
             command.append("verbose")
         if version.major >= 7 and not sanitized:
             command.append("show-sensitive")
         if version.major <= 6 and sanitized:
             command.append("hide-sensitive")
-        self.ssh.connect(self.hostname, port=self.ssh_port, username=self.username, password=self.password)
+        self.ssh.connect(
+            self.hostname,
+            port=self.ssh_port,
+            username=self.username,
+            password=self.password,
+            look_for_keys=self.paramiko_look_for_keys,
+        )
         _, stdout, _ = self.ssh.exec_command(" ".join(command))
         config = stdout.read().decode().strip()
         # remove date/time in 1st line
         config = re.sub(r"^# \S+ \S+ by (.+)$", r'# by \1', config, flags=re.MULTILINE)
         if retrieve in ("running", "all"):
             configs['running'] = config
         return configs
```

### Comparing `napalm-ros-1.2.3/napalm_ros/utils.py` & `napalm-ros-1.2.4/napalm_ros/utils.py`

 * *Files identical despite different names*

### Comparing `napalm-ros-1.2.3/napalm_ros.egg-info/PKG-INFO` & `napalm-ros-1.2.4/napalm_ros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-ros
-Version: 1.2.3
+Version: 1.2.4
 Summary: Network Automation and Programmability Abstraction Layer driver for Mikrotik ROS
 Author-email: Łukasz Kostka <lukasz.g.kostka@gmail.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-ros
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-ros/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `napalm-ros-1.2.3/pyproject.toml` & `napalm-ros-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=56.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napalm-ros"
-version="1.2.3"
+version="1.2.4"
 description="Network Automation and Programmability Abstraction Layer driver for Mikrotik ROS"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   { name="Łukasz Kostka", email="lukasz.g.kostka@gmail.com" },
 ]
```


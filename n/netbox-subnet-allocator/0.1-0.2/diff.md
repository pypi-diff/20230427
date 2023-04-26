# Comparing `tmp/netbox-subnet-allocator-0.1.tar.gz` & `tmp/netbox-subnet-allocator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-subnet-allocator-0.1.tar", last modified: Wed Apr 26 21:37:20 2023, max compression
+gzip compressed data, was "netbox-subnet-allocator-0.2.tar", last modified: Wed Apr 26 22:00:16 2023, max compression
```

## Comparing `netbox-subnet-allocator-0.1.tar` & `netbox-subnet-allocator-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 21:37:20.180210 netbox-subnet-allocator-0.1/
--rw-r--r--   0 aaron.finney   (503) staff       (20)     1069 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.1/LICENSE
--rw-r--r--   0 aaron.finney   (503) staff       (20)      215 2023-04-26 21:37:20.180366 netbox-subnet-allocator-0.1/PKG-INFO
--rw-r--r--   0 aaron.finney   (503) staff       (20)      116 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.1/README.md
-drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 21:37:20.178518 netbox-subnet-allocator-0.1/netbox_subnet_allocator/
--rw-r--r--   0 aaron.finney   (503) staff       (20)      335 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator/__init__.py
--rw-r--r--   0 aaron.finney   (503) staff       (20)     1426 2023-04-26 21:03:48.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator/models.py
-drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 21:37:20.179926 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/
--rw-r--r--   0 aaron.finney   (503) staff       (20)      215 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/PKG-INFO
--rw-r--r--   0 aaron.finney   (503) staff       (20)      340 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/SOURCES.txt
--rw-r--r--   0 aaron.finney   (503) staff       (20)        1 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/dependency_links.txt
--rw-r--r--   0 aaron.finney   (503) staff       (20)        1 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/not-zip-safe
--rw-r--r--   0 aaron.finney   (503) staff       (20)       24 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.1/netbox_subnet_allocator.egg-info/top_level.txt
--rw-r--r--   0 aaron.finney   (503) staff       (20)      103 2023-04-26 21:37:20.180832 netbox-subnet-allocator-0.1/setup.cfg
--rw-r--r--   0 aaron.finney   (503) staff       (20)      290 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.1/setup.py
+drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 22:00:16.008969 netbox-subnet-allocator-0.2/
+-rw-r--r--   0 aaron.finney   (503) staff       (20)     1069 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.2/LICENSE
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      215 2023-04-26 22:00:16.009034 netbox-subnet-allocator-0.2/PKG-INFO
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      116 2023-04-26 18:19:58.000000 netbox-subnet-allocator-0.2/README.md
+drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 22:00:16.004286 netbox-subnet-allocator-0.2/netbox_subnet_allocator/
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      348 2023-04-26 21:58:15.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator/__init__.py
+-rw-r--r--   0 aaron.finney   (503) staff       (20)     1426 2023-04-26 21:03:48.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator/models.py
+drwxr-xr-x   0 aaron.finney   (503) staff       (20)        0 2023-04-26 22:00:16.008804 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      215 2023-04-26 22:00:15.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/PKG-INFO
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      340 2023-04-26 22:00:16.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron.finney   (503) staff       (20)        1 2023-04-26 22:00:15.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron.finney   (503) staff       (20)        1 2023-04-26 21:37:20.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/not-zip-safe
+-rw-r--r--   0 aaron.finney   (503) staff       (20)       24 2023-04-26 22:00:15.000000 netbox-subnet-allocator-0.2/netbox_subnet_allocator.egg-info/top_level.txt
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      103 2023-04-26 22:00:16.009283 netbox-subnet-allocator-0.2/setup.cfg
+-rw-r--r--   0 aaron.finney   (503) staff       (20)      290 2023-04-26 22:00:12.000000 netbox-subnet-allocator-0.2/setup.py
```

### Comparing `netbox-subnet-allocator-0.1/LICENSE` & `netbox-subnet-allocator-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-subnet-allocator-0.1/netbox_subnet_allocator/models.py` & `netbox-subnet-allocator-0.2/netbox_subnet_allocator/models.py`

 * *Files identical despite different names*


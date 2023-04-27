# Comparing `tmp/simpledi-0.3.tar.gz` & `tmp/simpledi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpledi-0.3.tar", last modified: Mon Oct 12 07:15:30 2015, max compression
+gzip compressed data, was "simpledi-0.4.1.tar", last modified: Thu Apr 27 11:11:27 2023, max compression
```

## Comparing `simpledi-0.3.tar` & `simpledi-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 costache   (501) staff       (20)        0 2015-10-12 07:15:30.000000 simpledi-0.3/
--rw-r--r--   0 costache   (501) staff       (20)      268 2015-10-12 07:15:30.000000 simpledi-0.3/PKG-INFO
--rw-r--r--   0 costache   (501) staff       (20)       59 2015-10-12 07:15:30.000000 simpledi-0.3/setup.cfg
--rw-r--r--   0 costache   (501) staff       (20)      332 2015-10-12 07:12:24.000000 simpledi-0.3/setup.py
-drwxr-xr-x   0 costache   (501) staff       (20)        0 2015-10-12 07:15:30.000000 simpledi-0.3/src/
-drwxr-xr-x   0 costache   (501) staff       (20)        0 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi/
--rw-r--r--   0 costache   (501) staff       (20)     3553 2015-10-12 07:14:30.000000 simpledi-0.3/src/simpledi/__init__.py
-drwxr-xr-x   0 costache   (501) staff       (20)        0 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi.egg-info/
--rw-r--r--   0 costache   (501) staff       (20)        1 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi.egg-info/dependency_links.txt
--rw-r--r--   0 costache   (501) staff       (20)      268 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi.egg-info/PKG-INFO
--rw-r--r--   0 costache   (501) staff       (20)      177 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi.egg-info/SOURCES.txt
--rw-r--r--   0 costache   (501) staff       (20)        9 2015-10-12 07:15:30.000000 simpledi-0.3/src/simpledi.egg-info/top_level.txt
+drwxr-xr-x   0 dcoman     (502) staff       (20)        0 2023-04-27 11:11:27.866575 simpledi-0.4.1/
+-rw-r--r--   0 dcoman     (502) staff       (20)    11335 2021-08-18 13:36:07.000000 simpledi-0.4.1/LICENSE
+-rw-r--r--   0 dcoman     (502) staff       (20)      236 2023-04-27 11:11:27.866201 simpledi-0.4.1/PKG-INFO
+-rw-r--r--   0 dcoman     (502) staff       (20)     3306 2023-04-27 08:44:52.000000 simpledi-0.4.1/README.md
+-rw-r--r--   0 dcoman     (502) staff       (20)       38 2023-04-27 11:11:27.866672 simpledi-0.4.1/setup.cfg
+-rw-r--r--   0 dcoman     (502) staff       (20)      334 2023-04-27 11:10:44.000000 simpledi-0.4.1/setup.py
+drwxr-xr-x   0 dcoman     (502) staff       (20)        0 2023-04-27 11:11:27.861548 simpledi-0.4.1/src/
+drwxr-xr-x   0 dcoman     (502) staff       (20)        0 2023-04-27 11:11:27.863998 simpledi-0.4.1/src/simpledi/
+-rw-r--r--   0 dcoman     (502) staff       (20)     3567 2023-04-27 08:29:49.000000 simpledi-0.4.1/src/simpledi/__init__.py
+drwxr-xr-x   0 dcoman     (502) staff       (20)        0 2023-04-27 11:11:27.865806 simpledi-0.4.1/src/simpledi.egg-info/
+-rw-r--r--   0 dcoman     (502) staff       (20)      236 2023-04-27 11:11:27.000000 simpledi-0.4.1/src/simpledi.egg-info/PKG-INFO
+-rw-r--r--   0 dcoman     (502) staff       (20)      195 2023-04-27 11:11:27.000000 simpledi-0.4.1/src/simpledi.egg-info/SOURCES.txt
+-rw-r--r--   0 dcoman     (502) staff       (20)        1 2023-04-27 11:11:27.000000 simpledi-0.4.1/src/simpledi.egg-info/dependency_links.txt
+-rw-r--r--   0 dcoman     (502) staff       (20)        9 2023-04-27 11:11:27.000000 simpledi-0.4.1/src/simpledi.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simpledi-0.3/src/simpledi/__init__.py` & `simpledi-0.4.1/src/simpledi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from inspect import getargspec
+from inspect import getfullargspec
 
 """
 A basic implementation of a dependency injection container
 
 Basic usage:
 
     class Foo(object):
@@ -51,30 +51,30 @@
     def __init__(self, clz):
         self.clz = clz
 
     def __call__(self, container):
         if '__init__' not in self.clz.__dict__:
             return self.clz()
 
-        argspec = getargspec(self.clz.__init__)
+        argspec = getfullargspec(self.clz.__init__)
         # ignore self
         dependencies = argspec.args[1:]
 
         return self.clz(*[container.get_instance(dependency) for dependency in dependencies])
 
 
 class ListInstanceProvider(Provider):
     def __init__(self, *providers):
         self._providers = list(providers)
 
     def add(self, *providers):
         self._providers.extend(providers)
 
     def __call__(self, container):
-        return map(lambda provider: provider(container), self._providers)
+        return list(map(lambda provider: provider(container), self._providers))
 
 
 class CacheInstanceProvider(Provider):
     def __init__(self, provider):
         self.provider = provider
         self.cache = None
```


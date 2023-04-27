# Comparing `tmp/function-cooldowns-1.7.0.tar.gz` & `tmp/function-cooldowns-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-cooldowns-1.7.0.tar", last modified: Tue Feb 14 11:35:11 2023, max compression
+gzip compressed data, was "function-cooldowns-1.7.1.tar", last modified: Thu Apr 27 10:17:41 2023, max compression
```

## Comparing `function-cooldowns-1.7.0.tar` & `function-cooldowns-1.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1211 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/LICENSE
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/PKG-INFO
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/cooldowns/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1415 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/__init__.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/cooldowns/buckets/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      182 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/cooldowns/buckets/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2154 2022-10-30 10:38:23.000000 function-cooldowns-1.7.0/cooldowns/buckets/hashable_arguments.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      911 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/cooldowns/buckets/main.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1134 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/cooldowns/buckets/slash.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    13914 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/cooldown.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3640 2023-02-14 11:29:20.000000 function-cooldowns-1.7.0/cooldowns/cooldown_times_per.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2202 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/exceptions.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2675 2022-07-19 09:36:03.000000 function-cooldowns-1.7.0/cooldowns/persistence.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/cooldowns/protocols/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       82 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/cooldowns/protocols/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      359 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/cooldowns/protocols/bucket.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6139 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/static_cooldown.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2273 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/static_times_per.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     9214 2023-02-14 11:31:54.000000 function-cooldowns-1.7.0/cooldowns/utils.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/function_cooldowns.egg-info/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-02-14 11:35:11.000000 function-cooldowns-1.7.0/function_cooldowns.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      572 2023-02-14 11:35:11.000000 function-cooldowns-1.7.0/function_cooldowns.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-02-14 11:35:11.000000 function-cooldowns-1.7.0/function_cooldowns.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       10 2023-02-14 11:35:11.000000 function-cooldowns-1.7.0/function_cooldowns.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-02-14 11:35:11.497067 function-cooldowns-1.7.0/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1496 2022-06-02 07:37:26.000000 function-cooldowns-1.7.0/setup.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1211 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/LICENSE
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/PKG-INFO
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1415 2023-04-27 10:17:31.000000 function-cooldowns-1.7.1/cooldowns/__init__.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/buckets/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      182 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2154 2022-10-30 10:38:23.000000 function-cooldowns-1.7.1/cooldowns/buckets/hashable_arguments.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      911 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/main.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1134 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/slash.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    13914 2023-04-27 09:26:19.000000 function-cooldowns-1.7.1/cooldowns/cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3640 2023-04-27 10:13:38.000000 function-cooldowns-1.7.1/cooldowns/cooldown_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2202 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/exceptions.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2905 2023-04-27 10:17:31.000000 function-cooldowns-1.7.1/cooldowns/persistence.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/protocols/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       82 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/protocols/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      359 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/protocols/bucket.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6139 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/static_cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2273 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/static_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     9214 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/utils.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/function_cooldowns.egg-info/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-04-27 10:17:40.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      572 2023-04-27 10:17:41.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/SOURCES.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-04-27 10:17:40.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/dependency_links.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       10 2023-04-27 10:17:41.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/top_level.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/setup.cfg
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1496 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/setup.py
```

### Comparing `function-cooldowns-1.7.0/LICENSE` & `function-cooldowns-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/PKG-INFO` & `function-cooldowns-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-cooldowns
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simplistic decorator based approach to rate limiting function calls.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
 License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/Skelmis/Function-Cooldowns/issues
 Project-URL: Documentation, https://function-cooldowns.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/Skelmis/Function-Cooldowns
```

### Comparing `function-cooldowns-1.7.0/cooldowns/__init__.py` & `function-cooldowns-1.7.1/cooldowns/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     "get_shared_cooldown",
     "StaticTimesPer",
     "StaticCooldown",
     "static_cooldown",
     "define_shared_static_cooldown",
 )
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 VersionInfo = namedtuple("VersionInfo", "major minor micro releaselevel serial")
-version_info = VersionInfo(major=1, minor=7, micro=0, releaselevel="final", serial=0)
+version_info = VersionInfo(major=1, minor=7, micro=1, releaselevel="final", serial=0)
```

### Comparing `function-cooldowns-1.7.0/cooldowns/buckets/hashable_arguments.py` & `function-cooldowns-1.7.1/cooldowns/buckets/hashable_arguments.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/buckets/main.py` & `function-cooldowns-1.7.1/cooldowns/buckets/main.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/buckets/slash.py` & `function-cooldowns-1.7.1/cooldowns/buckets/slash.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/cooldown.py` & `function-cooldowns-1.7.1/cooldowns/cooldown.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/cooldown_times_per.py` & `function-cooldowns-1.7.1/cooldowns/cooldown_times_per.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/exceptions.py` & `function-cooldowns-1.7.1/cooldowns/exceptions.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/persistence.py` & `function-cooldowns-1.7.1/cooldowns/persistence.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,25 @@
             limit=v["limit"],
             time_period=v["time_period"],
             _cooldown=cooldown,
         )
         cooldown_times_per.current = v["current"]
 
         for epoch in v["next_reset"]:
-            epoch_time = datetime.datetime.fromtimestamp(
+            epoch_time = datetime.datetime.utcfromtimestamp(
                 epoch,  # tz=datetime.timezone.utc
             )
             if _check_expired(epoch_time):
                 # No longer relevant
                 cooldown_times_per.current += 1
                 continue
 
+            current_time = datetime.datetime.utcnow()
             cooldown_times_per._next_reset.put_nowait(epoch_time)
+            cooldown_times_per.loop.call_later(
+                (epoch_time - current_time).total_seconds(),
+                cooldown_times_per._reset_invoke,
+            )
 
         cache[hashable_arguments] = cooldown_times_per
 
     cooldown._cache = cache
```

### Comparing `function-cooldowns-1.7.0/cooldowns/static_cooldown.py` & `function-cooldowns-1.7.1/cooldowns/static_cooldown.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/static_times_per.py` & `function-cooldowns-1.7.1/cooldowns/static_times_per.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/cooldowns/utils.py` & `function-cooldowns-1.7.1/cooldowns/utils.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/function_cooldowns.egg-info/PKG-INFO` & `function-cooldowns-1.7.1/function_cooldowns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-cooldowns
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simplistic decorator based approach to rate limiting function calls.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
 License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/Skelmis/Function-Cooldowns/issues
 Project-URL: Documentation, https://function-cooldowns.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/Skelmis/Function-Cooldowns
```

### Comparing `function-cooldowns-1.7.0/function_cooldowns.egg-info/SOURCES.txt` & `function-cooldowns-1.7.1/function_cooldowns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.0/setup.py` & `function-cooldowns-1.7.1/setup.py`

 * *Files identical despite different names*


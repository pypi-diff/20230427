# Comparing `tmp/m-caching-0.1.8.tar.gz` & `tmp/m-caching-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m-caching-0.1.8.tar", last modified: Mon Sep  7 04:33:27 2020, max compression
+gzip compressed data, was "m-caching-0.1.9.tar", last modified: Fri Mar 24 10:02:25 2023, max compression
```

## Comparing `m-caching-0.1.8.tar` & `m-caching-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 locnguyen   (501) staff       (20)        0 2020-09-07 04:33:27.000000 m-caching-0.1.8/
--rw-r--r--   0 locnguyen   (501) staff       (20)     1983 2020-09-07 04:33:27.000000 m-caching-0.1.8/PKG-INFO
--rw-r--r--   0 locnguyen   (501) staff       (20)     1275 2019-12-11 07:48:43.000000 m-caching-0.1.8/README.md
-drwxr-xr-x   0 locnguyen   (501) staff       (20)        0 2020-09-07 04:33:27.000000 m-caching-0.1.8/m_caching.egg-info/
--rw-r--r--   0 locnguyen   (501) staff       (20)     1983 2020-09-07 04:33:26.000000 m-caching-0.1.8/m_caching.egg-info/PKG-INFO
--rw-r--r--   0 locnguyen   (501) staff       (20)      213 2020-09-07 04:33:26.000000 m-caching-0.1.8/m_caching.egg-info/SOURCES.txt
--rw-r--r--   0 locnguyen   (501) staff       (20)        1 2020-09-07 04:33:26.000000 m-caching-0.1.8/m_caching.egg-info/dependency_links.txt
--rw-r--r--   0 locnguyen   (501) staff       (20)        6 2020-09-07 04:33:26.000000 m-caching-0.1.8/m_caching.egg-info/requires.txt
--rw-r--r--   0 locnguyen   (501) staff       (20)       19 2020-09-07 04:33:26.000000 m-caching-0.1.8/m_caching.egg-info/top_level.txt
-drwxr-xr-x   0 locnguyen   (501) staff       (20)        0 2020-09-07 04:33:27.000000 m-caching-0.1.8/mobio/
-drwxr-xr-x   0 locnguyen   (501) staff       (20)        0 2020-09-07 04:33:27.000000 m-caching-0.1.8/mobio/libs/
-drwxr-xr-x   0 locnguyen   (501) staff       (20)        0 2020-09-07 04:33:27.000000 m-caching-0.1.8/mobio/libs/caching/
--rw-r--r--   0 locnguyen   (501) staff       (20)    22599 2020-09-07 04:32:26.000000 m-caching-0.1.8/mobio/libs/caching/__init__.py
--rw-r--r--   0 locnguyen   (501) staff       (20)       38 2020-09-07 04:33:27.000000 m-caching-0.1.8/setup.cfg
--rw-r--r--   0 locnguyen   (501) staff       (20)      646 2020-09-07 04:32:59.000000 m-caching-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 10:02:25.889963 m-caching-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-03-24 10:02:25.888963 m-caching-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-03-24 10:01:08.000000 m-caching-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 10:02:25.886963 m-caching-0.1.9/m_caching.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-03-24 10:02:25.000000 m-caching-0.1.9/m_caching.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      213 2023-03-24 10:02:25.000000 m-caching-0.1.9/m_caching.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 10:02:25.000000 m-caching-0.1.9/m_caching.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-03-24 10:02:25.000000 m-caching-0.1.9/m_caching.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-03-24 10:02:25.000000 m-caching-0.1.9/m_caching.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 10:02:25.877963 m-caching-0.1.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 10:02:25.877963 m-caching-0.1.9/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 10:02:25.887963 m-caching-0.1.9/mobio/libs/caching/
+-rw-r--r--   0 root         (0) root         (0)    22747 2023-03-24 10:01:08.000000 m-caching-0.1.9/mobio/libs/caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 10:02:25.889963 m-caching-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      686 2023-03-24 10:02:24.000000 m-caching-0.1.9/setup.py
```

### Comparing `m-caching-0.1.8/PKG-INFO` & `m-caching-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: m-caching
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setup normal class to mobio lru cache
-Home-page: https://github.com/mobiovn
+Home-page: UNKNOWN
 Author: MOBIO
-Author-email: contact@mobio.vn
+Author-email: contact@mobio.io
 License: MIT
 Description: # <h2 id="title">LRU Cache</h2>
         Thư viện caching của MOBIO. Hỗ trợ cache trên memory hoặc Redis.
         
         #### Cài đặt:
         `pip3 install m-caching`
         
@@ -58,9 +58,12 @@
         ```
         [REDIS]
         host=redis-server
         port=6379
         cache_prefix=test_cache
         ```
         
+        #### Changedlog:
+        ##### v1.0.9:
+        - Thêm try...except: khi set item vao redis.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `m-caching-0.1.8/README.md` & `m-caching-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,7 +49,11 @@
 #### Example config
 ```
 [REDIS]
 host=redis-server
 port=6379
 cache_prefix=test_cache
 ```
+
+#### Changedlog:
+##### v1.0.9:
+- Thêm try...except: khi set item vao redis.
```

### Comparing `m-caching-0.1.8/m_caching.egg-info/PKG-INFO` & `m-caching-0.1.9/m_caching.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: m-caching
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setup normal class to mobio lru cache
-Home-page: https://github.com/mobiovn
+Home-page: UNKNOWN
 Author: MOBIO
-Author-email: contact@mobio.vn
+Author-email: contact@mobio.io
 License: MIT
 Description: # <h2 id="title">LRU Cache</h2>
         Thư viện caching của MOBIO. Hỗ trợ cache trên memory hoặc Redis.
         
         #### Cài đặt:
         `pip3 install m-caching`
         
@@ -58,9 +58,12 @@
         ```
         [REDIS]
         host=redis-server
         port=6379
         cache_prefix=test_cache
         ```
         
+        #### Changedlog:
+        ##### v1.0.9:
+        - Thêm try...except: khi set item vao redis.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `m-caching-0.1.8/mobio/libs/caching/__init__.py` & `m-caching-0.1.9/mobio/libs/caching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,17 +551,23 @@
             if accept_none is not None:
                 if not value and not accept_none:
                     print("value is None => ignore")
                     return
 
             _key = self.norm_key(key)
             if expiration == EXPIRATION_NEVER:
-                self._redis.set(_key, json.dumps(value), None)
+                try:
+                    self._redis.set(_key, json.dumps(value), None)
+                except:
+                    pass
             else:
-                self._redis.set(_key, json.dumps(value), expiration)
+                try:
+                    self._redis.set(_key, json.dumps(value), expiration)
+                except:
+                    pass
             self.cleanup()
         else:
             print("REDIS not ready for cache")
 
     @_lock_decorator
     def __getitem__(self, key):
         if self.is_redis_ready:
```


# Comparing `tmp/leocli-3.4.1.tar.gz` & `tmp/leocli-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leocli-3.4.1.tar", max compression
+gzip compressed data, was "leocli-3.4.2.tar", max compression
```

## Comparing `leocli-3.4.1.tar` & `leocli-3.4.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      265 2020-06-27 16:29:17.968091 leocli-3.4.1/leocli/__init__.py
--rw-r--r--   0        0        0     3154 2022-07-30 17:43:55.313178 leocli-3.4.1/leocli/cache.py
--rw-r--r--   0        0        0     2939 2022-07-30 18:05:19.634248 leocli-3.4.1/leocli/conf.py
--rw-r--r--   0        0        0     1036 2022-07-30 18:36:49.671999 leocli-3.4.1/leocli/consts.py
--rwxr-xr-x   0        0        0     9205 2022-07-30 18:37:03.103844 leocli-3.4.1/leocli/leo.py
--rw-r--r--   0        0        0      670 2022-07-30 18:50:19.811908 leocli-3.4.1/pyproject.toml
--rw-r--r--   0        0        0      920 2022-07-30 18:50:50.574817 leocli-3.4.1/setup.py
--rw-r--r--   0        0        0      683 2022-07-30 18:50:50.575054 leocli-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-06-27 16:29:17.968091 leocli-3.4.2/leocli/__init__.py
+-rw-r--r--   0        0        0     3195 2022-07-30 18:52:24.042936 leocli-3.4.2/leocli/cache.py
+-rw-r--r--   0        0        0     2939 2022-07-30 18:05:19.634248 leocli-3.4.2/leocli/conf.py
+-rw-r--r--   0        0        0     1036 2022-07-30 18:36:49.671999 leocli-3.4.2/leocli/consts.py
+-rwxr-xr-x   0        0        0     9205 2022-07-30 18:37:03.103844 leocli-3.4.2/leocli/leo.py
+-rw-r--r--   0        0        0      724 2023-04-27 07:06:54.166769 leocli-3.4.2/pyproject.toml
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 leocli-3.4.2/PKG-INFO
```

### Comparing `leocli-3.4.1/leocli/cache.py` & `leocli-3.4.2/leocli/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         lang1: str,
         lang2: str,
         data: list[APISection],
     ):
         cache_path = self._get_cache_path(search=search, lang1=lang1, lang2=lang2)
         cache_path.parent.mkdir(parents=True, exist_ok=True)
 
+        # TODO max cache size & cleanup
+
         cache_entry = {
             "last_used": int(datetime.now().timestamp()),
             "num_used": 1,
             "cache_format": "v1",
             "data": [],
         }
```

### Comparing `leocli-3.4.1/leocli/conf.py` & `leocli-3.4.2/leocli/conf.py`

 * *Files identical despite different names*

### Comparing `leocli-3.4.1/leocli/consts.py` & `leocli-3.4.2/leocli/consts.py`

 * *Files identical despite different names*

### Comparing `leocli-3.4.1/leocli/leo.py` & `leocli-3.4.2/leocli/leo.py`

 * *Files identical despite different names*


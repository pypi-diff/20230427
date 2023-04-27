# Comparing `tmp/recon_lw-2.0.0.dev4808598137.tar.gz` & `tmp/recon_lw-2.0.0.dev4816988331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4808598137.tar", last modified: Wed Apr 26 12:22:56 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4816988331.tar", last modified: Thu Apr 27 07:08:13 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4808598137.tar` & `recon_lw-2.0.0.dev4816988331.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-26 12:22:35.000000 recon_lw-2.0.0.dev4808598137/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2757 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    19709 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-27 07:07:52.000000 recon_lw-2.0.0.dev4816988331/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20312 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 07:08:13.000000 recon_lw-2.0.0.dev4816988331/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-27 07:07:44.000000 recon_lw-2.0.0.dev4816988331/setup.py
```

### Comparing `recon_lw-2.0.0.dev4808598137/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4816988331/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4808598137/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4816988331/recon_lw/TimeCacheMatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
             ts, key1, key2 = self._get_timestamp_key1_key2(o, self._custom_settings)
             log_event =  self._create_event ("MatcherLog" + str(self._custom_settings),
                                              "MatcherLog",
                                              False,
                                              {"ts": ts,
                                               "key1": key1,
                                               "key2": key2,
-                                              "sourceEventId": o["eventId"]})
+                                              "sourceEvent": o})
             self._send_events([log_event])
             if ts is None:
                 continue
             stream_time = ts
             if key1 is not None:
                 if key1 not in self._match_index:
                     self._match_index[key1] = [o, None]
                     self._time_index.add([ts, key1])
                 else:
                     self._match_index[key1][0] = o
-            elif key2 is None:
+            elif key2 is not None:
                 if key2 not in self._match_index:
                     self._match_index[key2] = [None, o]
                     self._time_index.add([ts, key2])
                 else:
                     self._match_index[key2][1] = o
 
         if stream_time is not None:
```

### Comparing `recon_lw-2.0.0.dev4808598137/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4816988331/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4816988331/recon_lw/recon_ob.py`

 * *Files 4% similar despite different names*

```diff
@@ -436,14 +436,35 @@
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
+def ob_top_clean_book(order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+
+    order_book["ask_price"] = 0
+    order_book["ask_real_qty"] = 0
+    order_book["ask_impl_qty"] = 0
+    order_book["ask_real_n_orders"] = 0
+    order_book["ask_impl_n_orders"] = 0
+    order_book["bid_price"] = 0
+    order_book["bid_real_qty"] = 0
+    order_book["bid_impl_qty"] = 0
+    order_book["bid_real_n_orders"] = 0
+    order_book["bid_impl_n_orders"] = 0
+
+    order_book["aggr_seq"]["top_delta"] = 1
+    order_book["aggr_seq"]["top_v"] += 1
+
+    return {}, [copy.deepcopy(order_book)]
+
+
 def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
                   bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
                   order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
```

### Comparing `recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4816988331/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4808598137/setup.py` & `recon_lw-2.0.0.dev4816988331/setup.py`

 * *Files identical despite different names*


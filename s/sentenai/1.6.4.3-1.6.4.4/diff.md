# Comparing `tmp/sentenai-1.6.4.3.tar.gz` & `tmp/sentenai-1.6.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentenai-1.6.4.3.tar", last modified: Thu Apr 20 15:55:32 2023, max compression
+gzip compressed data, was "sentenai-1.6.4.4.tar", last modified: Thu Apr 27 15:20:31 2023, max compression
```

## Comparing `sentenai-1.6.4.3.tar` & `sentenai-1.6.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.683889 sentenai-1.6.4.3/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.3/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-20 15:55:32.683968 sentenai-1.6.4.3/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.3/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.682102 sentenai-1.6.4.3/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9052 2023-04-20 15:49:21.000000 sentenai-1.6.4.3/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.3/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.683723 sentenai-1.6.4.3/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.3/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.3/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.3/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24211 2023-04-20 15:49:17.000000 sentenai-1.6.4.3/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.682738 sentenai-1.6.4.3/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-20 15:55:32.684202 sentenai-1.6.4.3/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-20 15:49:43.000000 sentenai-1.6.4.3/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.803426 sentenai-1.6.4.4/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.4/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-27 15:20:31.803482 sentenai-1.6.4.4/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.4/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.801980 sentenai-1.6.4.4/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9160 2023-04-27 15:19:47.000000 sentenai-1.6.4.4/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.4/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.803315 sentenai-1.6.4.4/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.4/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.4/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.4/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24090 2023-04-27 15:19:50.000000 sentenai-1.6.4.4/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.802581 sentenai-1.6.4.4/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-27 15:20:31.803689 sentenai-1.6.4.4/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-27 15:20:11.000000 sentenai-1.6.4.4/setup.py
```

### Comparing `sentenai-1.6.4.3/LICENSE` & `sentenai-1.6.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.3/PKG-INFO` & `sentenai-1.6.4.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.3
+Version: 1.6.4.4
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.3/README.md` & `sentenai-1.6.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.3/sentenai/__init__.py` & `sentenai-1.6.4.4/sentenai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,19 @@
             return {'start': dt64(self._info['start']), 'end': dt64(self._info['end'])}
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
             return self.range
 
     @property
     def origin(self):
-        return dt64(self._post("debug", json=self._tspl['value']).json().get('origin'))
+        if self._info:
+            return dt64(self._info.get('origin'))
+        else:
+            self._info = self._post("range", json=self._tspl['value']).json()
+            return self.origin
 
     @property
     def type(self):
         if self._info:
             return self._info.get('type')
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
```

### Comparing `sentenai-1.6.4.3/sentenai/api.py` & `sentenai-1.6.4.4/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.3/sentenai/stream/events.py` & `sentenai-1.6.4.4/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.3/sentenai/stream/metadata.py` & `sentenai-1.6.4.4/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.3/sentenai/stream/streams.py` & `sentenai-1.6.4.4/sentenai/stream/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,39 +348,39 @@
                             dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
                         elif 'end' in row:
                             dur = (row['end'] - row['start']) // np.timedelta64(1, 'ns')
                         else:
                             dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
                     except IndexError:
                         dur = 1
-                    else:
-                        if dur <= 0: continue
-                        for col, val in dict(row).items():
-                            if col == 'start' and 'start' in dmap:
-                                dmap[col].append((ts, dur))
-                            elif type(val) == float and math.isnan(val): # skip nans
-                                pass
-                            elif val is pd.NaT or val is None:
-                                pass
-                            elif col not in tmap:
-                                pass
-                            elif tmap[col] == 'point3':
-                                dmap[col].append((ts, dur, (val.x, val.y, val.z)))
-                            elif tmap[col] == 'point':
-                                dmap[col].append((ts, dur, (val.x, val.y)))
-                            elif tmap[col] == 'date':
-                                dmap[col].append((ts, dur, val.isoformat()))
-                            elif tmap[col] == 'time':
-                                dmap[col].append((ts, dur, val.isoformat()))
-                            elif tmap[col] == 'datetime':
-                                dmap[col].append((ts, dur, iso8601(val)))
-                            elif tmap[col] == 'timedelta':
-                                dmap[col].append((ts, dur, val // np.timedelta64(1, 'ns')))
-                            else:
-                                dmap[col].append((ts, dur, val))
+
+                    if dur <= 0: continue
+                    for col, val in dict(row).items():
+                        if col == 'start' and 'start' in dmap:
+                            dmap[col].append((ts, dur))
+                        elif type(val) == float and math.isnan(val): # skip nans
+                            pass
+                        elif val is pd.NaT or val is None:
+                            pass
+                        elif col not in tmap:
+                            pass
+                        elif tmap[col] == 'point3':
+                            dmap[col].append((ts, dur, (val.x, val.y, val.z)))
+                        elif tmap[col] == 'point':
+                            dmap[col].append((ts, dur, (val.x, val.y)))
+                        elif tmap[col] == 'date':
+                            dmap[col].append((ts, dur, val.isoformat()))
+                        elif tmap[col] == 'time':
+                            dmap[col].append((ts, dur, val.isoformat()))
+                        elif tmap[col] == 'datetime':
+                            dmap[col].append((ts, dur, iso8601(val)))
+                        elif tmap[col] == 'timedelta':
+                            dmap[col].append((ts, dur, val // np.timedelta64(1, 'ns')))
+                        else:
+                            dmap[col].append((ts, dur, val))
 
                     if 'start' in dmap and len(dmap['start']) >= 4096:
                         list(res) # force result
                         res = pool.map(index_data, [(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
                         for k, v in dmap.items():
                             dmap[k] = []
                     elif len(list(dmap.values())[0]) >= 4096:
```

### Comparing `sentenai-1.6.4.3/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.4/sentenai.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.3
+Version: 1.6.4.4
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.3/setup.py` & `sentenai-1.6.4.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.3',
+    version='1.6.4.4',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```


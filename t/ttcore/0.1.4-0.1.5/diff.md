# Comparing `tmp/ttcore-0.1.4.tar.gz` & `tmp/ttcore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttcore-0.1.4.tar", last modified: Tue Apr 25 12:51:20 2023, max compression
+gzip compressed data, was "ttcore-0.1.5.tar", last modified: Thu Apr 27 11:58:48 2023, max compression
```

## Comparing `ttcore-0.1.4.tar` & `ttcore-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-25 12:51:20.299203 ttcore-0.1.4/
--rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.4/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      633 2023-04-25 12:51:20.299203 ttcore-0.1.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.4/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-04-25 12:51:20.299203 ttcore-0.1.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      871 2023-04-25 12:51:07.000000 ttcore-0.1.4/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-25 12:51:20.297203 ttcore-0.1.4/ttcore/
--rw-r--r--   0 user      (1000) user      (1000)    11508 2023-04-21 18:26:51.000000 ttcore-0.1.4/ttcore/bottle.py
--rw-r--r--   0 user      (1000) user      (1000)     3713 2023-04-21 18:26:51.000000 ttcore-0.1.4/ttcore/docs.html
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.4/ttcore/ip.py
--rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.4/ttcore/mailers.py
--rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.4/ttcore/messages.py
--rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.4/ttcore/peewee.py
--rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.4/ttcore/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-25 12:51:20.299203 ttcore-0.1.4/ttcore.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      633 2023-04-25 12:51:20.000000 ttcore-0.1.4/ttcore.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      331 2023-04-25 12:51:20.000000 ttcore-0.1.4/ttcore.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-25 12:51:20.000000 ttcore-0.1.4/ttcore.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-25 12:51:20.000000 ttcore-0.1.4/ttcore.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-04-25 12:51:20.000000 ttcore-0.1.4/ttcore.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.4/ttcore.egg-info/zip-safe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 11:58:48.055600 ttcore-0.1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.5/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)      633 2023-04-27 11:58:48.055600 ttcore-0.1.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.5/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-04-27 11:58:48.056600 ttcore-0.1.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      871 2023-04-27 11:58:33.000000 ttcore-0.1.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 11:58:48.051600 ttcore-0.1.5/ttcore/
+-rw-r--r--   0 user      (1000) user      (1000)    11749 2023-04-27 11:58:33.000000 ttcore-0.1.5/ttcore/bottle.py
+-rw-r--r--   0 user      (1000) user      (1000)     3713 2023-04-21 18:26:51.000000 ttcore-0.1.5/ttcore/docs.html
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.5/ttcore/ip.py
+-rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.5/ttcore/mailers.py
+-rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.5/ttcore/messages.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.5/ttcore/peewee.py
+-rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.5/ttcore/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 11:58:48.054600 ttcore-0.1.5/ttcore.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      633 2023-04-27 11:58:47.000000 ttcore-0.1.5/ttcore.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      331 2023-04-27 11:58:48.000000 ttcore-0.1.5/ttcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-27 11:58:47.000000 ttcore-0.1.5/ttcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-27 11:58:47.000000 ttcore-0.1.5/ttcore.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-04-27 11:58:47.000000 ttcore-0.1.5/ttcore.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.5/ttcore.egg-info/zip-safe
```

### Comparing `ttcore-0.1.4/LICENSE.txt` & `ttcore-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/PKG-INFO` & `ttcore-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ttcore-0.1.4/setup.py` & `ttcore-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ttcore",
-    version="0.1.4",
+    version="0.1.5",
     author="Martin F",
     author_email="pypi.org@tigerteamx.com",
     description="Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tigerteamx/ttcore",
     packages=['ttcore'],
```

### Comparing `ttcore-0.1.4/ttcore/bottle.py` & `ttcore-0.1.5/ttcore/bottle.py`

 * *Files 6% similar despite different names*

```diff
@@ -261,14 +261,18 @@
     def handle(self, callback):
         def wrapper(*args, **kwargs):
             try:
                 body = callback(*args, **kwargs)
                 return body
             except NotFound404 as e:
                 return dict(msg=e.args[0])
+            except HTTPResponse as e:
+                response.status = getattr(e, "status", None)
+                response.headers.update(getattr(e, "headers", {}))
+                return getattr(e, "body", {"msg": "Something went wrong"})
             except:  # noqa
                 msg = f"{self.on_error()}\n\n{format_exc()}"
                 print(msg)
                 self.on_msg(msg)
                 self._recent_msgs.append(datetime.now())
                 return {"msg": "Internal Error"}
```

### Comparing `ttcore-0.1.4/ttcore/docs.html` & `ttcore-0.1.5/ttcore/docs.html`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/ttcore/mailers.py` & `ttcore-0.1.5/ttcore/mailers.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/ttcore/messages.py` & `ttcore-0.1.5/ttcore/messages.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/ttcore/peewee.py` & `ttcore-0.1.5/ttcore/peewee.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/ttcore/utils.py` & `ttcore-0.1.5/ttcore/utils.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.4/ttcore.egg-info/PKG-INFO` & `ttcore-0.1.5/ttcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


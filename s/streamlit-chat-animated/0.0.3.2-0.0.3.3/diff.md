# Comparing `tmp/streamlit-chat-animated-0.0.3.2.tar.gz` & `tmp/streamlit-chat-animated-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-animated-0.0.3.2.tar", last modified: Thu Apr 27 19:27:51 2023, max compression
+gzip compressed data, was "streamlit-chat-animated-0.0.3.3.tar", last modified: Thu Apr 27 19:40:02 2023, max compression
```

## Comparing `streamlit-chat-animated-0.0.3.2.tar` & `streamlit-chat-animated-0.0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.533987 streamlit-chat-animated-0.0.3.2/
--rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.2/LICENSE
--rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.2/MANIFEST.in
--rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:27:51.533730 streamlit-chat-animated-0.0.3.2/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.2/README.md
--rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-27 19:27:51.534075 streamlit-chat-animated-0.0.3.2/setup.cfg
--rw-r--r--   0 systemd    (501) staff       (20)      897 2023-04-27 19:26:50.000000 streamlit-chat-animated-0.0.3.2/setup.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.524665 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/
--rw-r--r--   0 systemd    (501) staff       (20)     7096 2023-04-27 19:16:00.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/__init__.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.522570 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.529010 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/
--rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/asset-manifest.json
--rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-27 19:27:21.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css
--rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-27 19:27:21.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/index.html
--rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js
--rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/service-worker.js
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.522840 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.533345 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/
--rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
--rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     3286 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     9397 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.526301 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/
--rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/SOURCES.txt
--rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/dependency_links.txt
--rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/requires.txt
--rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/top_level.txt
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.823557 streamlit-chat-animated-0.0.3.3/
+-rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.3/LICENSE
+-rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.3/MANIFEST.in
+-rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:40:02.823113 streamlit-chat-animated-0.0.3.3/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.3/README.md
+-rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-27 19:40:02.823676 streamlit-chat-animated-0.0.3.3/setup.cfg
+-rw-r--r--   0 systemd    (501) staff       (20)      897 2023-04-27 19:38:10.000000 streamlit-chat-animated-0.0.3.3/setup.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.798375 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/
+-rw-r--r--   0 systemd    (501) staff       (20)     7095 2023-04-27 19:37:11.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/__init__.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.796534 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.806095 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/
+-rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/asset-manifest.json
+-rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-27 19:39:53.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/bootstrap.min.css
+-rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-27 19:39:53.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/index.html
+-rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/service-worker.js
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.796800 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.814352 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/
+-rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
+-rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     3286 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     9397 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-27 19:39:57.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:40:02.800827 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/
+-rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:40:02.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-27 19:40:02.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/SOURCES.txt
+-rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-27 19:40:02.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/dependency_links.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-27 19:40:02.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/requires.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-27 19:40:02.000000 streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/top_level.txt
```

### Comparing `streamlit-chat-animated-0.0.3.2/LICENSE` & `streamlit-chat-animated-0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/PKG-INFO` & `streamlit-chat-animated-0.0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A streamlit component, to make chatbots with text
 Home-page: UNKNOWN
 Author: Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.3.2/README.md` & `streamlit-chat-animated-0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/setup.py` & `streamlit-chat-animated-0.0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-animated",
-    version="0.0.3.2",
+    version="0.0.3.3",
     author="Darin Manley",
     author_email="darin.j.manley@gmail.com",
     description="A streamlit component, to make chatbots with text",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/__init__.py` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 
-_RELEASE = False
+_RELEASE = True
 COMPONENT_NAME = "streamlit_chat_animated"
 
 if _RELEASE:  # use the build instead of development if release is true
     root_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(root_dir, "frontend/build")
 
     _streamlit_chat = components.declare_component(
```

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/asset-manifest.json` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css.map` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/index.html` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/service-worker.js` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/PKG-INFO` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A streamlit component, to make chatbots with text
 Home-page: UNKNOWN
 Author: Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/SOURCES.txt` & `streamlit-chat-animated-0.0.3.3/streamlit_chat_animated.egg-info/SOURCES.txt`

 * *Files identical despite different names*


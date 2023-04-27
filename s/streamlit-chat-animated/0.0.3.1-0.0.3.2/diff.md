# Comparing `tmp/streamlit-chat-animated-0.0.3.1.tar.gz` & `tmp/streamlit-chat-animated-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-animated-0.0.3.1.tar", last modified: Tue Apr 18 03:39:26 2023, max compression
+gzip compressed data, was "streamlit-chat-animated-0.0.3.2.tar", last modified: Thu Apr 27 19:27:51 2023, max compression
```

## Comparing `streamlit-chat-animated-0.0.3.1.tar` & `streamlit-chat-animated-0.0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.801768 streamlit-chat-animated-0.0.3.1/
--rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.1/LICENSE
--rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.1/MANIFEST.in
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:39:26.801478 streamlit-chat-animated-0.0.3.1/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.1/README.md
--rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-18 03:39:26.801874 streamlit-chat-animated-0.0.3.1/setup.cfg
--rw-r--r--   0 systemd    (501) staff       (20)      945 2023-04-18 03:39:12.000000 streamlit-chat-animated-0.0.3.1/setup.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.790342 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/
--rw-r--r--   0 systemd    (501) staff       (20)     7095 2023-04-18 03:38:04.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/__init__.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.788615 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.795562 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/
--rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/asset-manifest.json
--rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-18 03:38:14.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css
--rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-18 03:38:14.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/index.html
--rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js
--rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/service-worker.js
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.788890 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.800998 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/
--rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
--rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     3315 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     9426 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-18 03:38:18.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-18 03:39:26.791879 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/SOURCES.txt
--rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/dependency_links.txt
--rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/requires.txt
--rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-18 03:39:26.000000 streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/top_level.txt
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.533987 streamlit-chat-animated-0.0.3.2/
+-rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.3.2/LICENSE
+-rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.3.2/MANIFEST.in
+-rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:27:51.533730 streamlit-chat-animated-0.0.3.2/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.3.2/README.md
+-rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-27 19:27:51.534075 streamlit-chat-animated-0.0.3.2/setup.cfg
+-rw-r--r--   0 systemd    (501) staff       (20)      897 2023-04-27 19:26:50.000000 streamlit-chat-animated-0.0.3.2/setup.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.524665 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/
+-rw-r--r--   0 systemd    (501) staff       (20)     7096 2023-04-27 19:16:00.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/__init__.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.522570 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.529010 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/
+-rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/asset-manifest.json
+-rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-27 19:27:21.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css
+-rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-27 19:27:21.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/index.html
+-rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/service-worker.js
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.522840 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.533345 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/
+-rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
+-rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     3286 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     9397 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-27 19:27:26.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-27 19:27:51.526301 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/
+-rw-r--r--   0 systemd    (501) staff       (20)     1213 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/SOURCES.txt
+-rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/dependency_links.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/requires.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-27 19:27:51.000000 streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/top_level.txt
```

### Comparing `streamlit-chat-animated-0.0.3.1/LICENSE` & `streamlit-chat-animated-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/PKG-INFO` & `streamlit-chat-animated-0.0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.1
-Summary: A streamlit component, to make chatbots with animated text
+Version: 0.0.3.2
+Summary: A streamlit component, to make chatbots with text
 Home-page: UNKNOWN
-Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
+Author: Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamlit-chat-animated-0.0.3.1/README.md` & `streamlit-chat-animated-0.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/setup.py` & `streamlit-chat-animated-0.0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-animated",
-    version="0.0.3.1",
-    author="Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley",
+    version="0.0.3.2",
+    author="Darin Manley",
     author_email="darin.j.manley@gmail.com",
-    description="A streamlit component, to make chatbots with animated text",
+    description="A streamlit component, to make chatbots with text",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/__init__.py` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 
-_RELEASE = True
+_RELEASE = False
 COMPONENT_NAME = "streamlit_chat_animated"
 
 if _RELEASE:  # use the build instead of development if release is true
     root_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(root_dir, "frontend/build")
 
     _streamlit_chat = components.declare_component(
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/asset-manifest.json` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/asset-manifest.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.24daa2e9.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.24daa2e9.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.24daa2e9.chunk.js.map', "*

 * *            "'precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js': "*

 * *            "'./precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js', delete: "*

 * *            "['precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/js/2.c8026899.chunk.js",
-        "static/js/main.6ecc478f.chunk.js"
+        "static/js/main.24daa2e9.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.6ecc478f.chunk.js",
-        "main.js.map": "./static/js/main.6ecc478f.chunk.js.map",
-        "precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js": "./precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js",
+        "main.js": "./static/js/main.24daa2e9.chunk.js",
+        "main.js.map": "./static/js/main.24daa2e9.chunk.js.map",
+        "precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js": "./precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.c8026899.chunk.js": "./static/js/2.c8026899.chunk.js",
         "static/js/2.c8026899.chunk.js.LICENSE.txt": "./static/js/2.c8026899.chunk.js.LICENSE.txt",
         "static/js/2.c8026899.chunk.js.map": "./static/js/2.c8026899.chunk.js.map"
     }
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/bootstrap.min.css.map` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/index.html` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.c8026899.chunk.js"></script><script src="./static/js/main.6ecc478f.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.c8026899.chunk.js"></script><script src="./static/js/main.24daa2e9.chunk.js"></script></body></html>
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/service-worker.js` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/service-worker.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js"
+    "./precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,61 +1,61 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
-        31: function(e, t, a) {
-            e.exports = a(39)
+        31: function(e, t, r) {
+            e.exports = r(39)
         },
-        39: function(e, t, a) {
+        39: function(e, t, r) {
             "use strict";
-            a.r(t);
-            var r, n, i, c, s = a(5),
-                o = a.n(s),
-                l = a(30),
-                d = a.n(l),
-                u = a(0),
-                p = a(1),
-                m = a(2),
-                b = a(3),
-                h = a(14),
-                g = a(15),
-                f = a(22),
-                v = a(7),
-                x = a(12),
+            r.r(t);
+            var a, n, i, c, o = r(5),
+                s = r.n(o),
+                l = r(30),
+                d = r.n(l),
+                u = r(0),
+                p = r(1),
+                m = r(2),
+                g = r(3),
+                h = r(14),
+                b = r(15),
+                f = r(22),
+                x = r(7),
+                v = r(12),
                 j = function(e) {
                     var t = e.text,
-                        a = e.onComplete,
-                        r = e.onHeightChange,
+                        r = e.onComplete,
+                        a = e.onHeightChange,
                         n = e.args,
-                        i = Object(s.useState)(""),
-                        c = Object(v.a)(i, 2),
+                        i = Object(o.useState)(""),
+                        c = Object(x.a)(i, 2),
                         l = c[0],
                         d = c[1],
-                        u = Object(s.useRef)(null),
-                        p = Object(s.useState)(!1),
-                        m = Object(v.a)(p, 2),
-                        b = m[0],
+                        u = Object(o.useRef)(null),
+                        p = Object(o.useState)(!1),
+                        m = Object(x.a)(p, 2),
+                        g = m[0],
                         h = m[1];
-                    return Object(s.useEffect)((function() {
-                        if (!b) {
+                    return Object(o.useEffect)((function() {
+                        if (!g) {
                             var e = 0,
                                 n = setInterval((function() {
                                     if (e < t.length) {
-                                        if (d((function(a) {
-                                                return a + t[e]
+                                        if (d((function(r) {
+                                                return r + t[e]
                                             })), u.current) {
                                             var i = u.current.getBoundingClientRect().height;
-                                            r(i)
+                                            a(i)
                                         }
                                         e++
-                                    } else clearInterval(n), a(), h(!0)
+                                    } else clearInterval(n), r(), h(!0)
                                 }), 10);
                             return function() {
                                 return clearInterval(n)
                             }
                         }
-                    }), [t, a, r, b]), o.a.createElement("div", {
+                    }), [t, r, a, g]), s.a.createElement("div", {
                         style: {
                             background: n.theme.secondaryBackgroundColor,
                             border: "1px solid transparent",
                             borderRadius: "10px",
                             padding: "10px 14px",
                             margin: "5px 20px",
                             maxWidth: "80%",
@@ -64,99 +64,99 @@
                             display: "flex"
                         },
                         ref: u
                     }, l)
                 },
                 O = function(e) {
                     var t = e.args,
-                        a = t.isUser,
+                        r = t.isUser,
                         l = t.message,
-                        d = (t.animated, t.key, Object(s.useState)(!1)),
-                        u = Object(v.a)(d, 2),
-                        p = (u[0], u[1], Object(s.useRef)(0)),
+                        d = (t.animated, t.key, Object(o.useState)(!1)),
+                        u = Object(x.a)(d, 2),
+                        p = (u[0], u[1], Object(o.useRef)(0)),
                         m = "";
-                    m = a ? "https://api.dicebear.com/6.x/shapes/svg?backgroundType=gradientLinear,solid" : "https://api.dicebear.com/6.x/avataaars/svg?seed=Felix&facialHair=beardMajestic&facialHairColor=2c1b18&eyes=happy&hairColor=4a312c&skinColor=d08b5b&style=circle&clothing=shirtVNeck&clothesColor=ffffff&top=curvy";
-                    Object(g.a)(j)({
+                    m = r ? "https://api.dicebear.com/6.x/shapes/svg?shape1Color=6941EB&shape2Color=00C8BC&shape3Color=ffa532&backgroundColor=ffffff&backgroundType=gradientLinear,solid" : "https://user-images.githubusercontent.com/6371329/234966848-c28e98de-221c-433d-bd33-eea5f04414fe.png";
+                    Object(b.a)(j)({
                         background: t.theme.secondaryBackgroundColor
                     });
-                    var b = g.a.img({
+                    var g = b.a.img({
                             border: "1px solid transparent",
                             borderRadius: "50%",
                             height: "5rem",
                             width: "5rem",
                             margin: 0
                         }, (function(e) {
-                            return e.isUser ? Object(x.a)(r || (r = Object(f.a)(["\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        "]))) : Object(x.a)(n || (n = Object(f.a)([""])))
+                            return e.isUser ? Object(v.a)(a || (a = Object(f.a)(["\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        "]))) : Object(v.a)(n || (n = Object(f.a)([""])))
                         })),
-                        h = g.a.div({
+                        h = b.a.div({
                             display: "inline-block",
                             background: t.theme.secondaryBackgroundColor,
                             border: "1px solid transparent",
                             borderRadius: "10px",
                             padding: "10px 14px",
                             margin: "5px 20px",
                             height: "auto",
                             maxWidth: "70%",
                             whiteSpace: "pre-line"
                         }),
-                        O = g.a.div({
+                        O = b.a.div({
                             display: "flex",
                             flex: 1,
                             maxWidth: "100vw",
                             height: "auto",
                             overflow: "auto"
                         }, (function(e) {
-                            return e.isUser ? Object(x.a)(i || (i = Object(f.a)(["\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      "]))) : Object(x.a)(c || (c = Object(f.a)([""])))
+                            return e.isUser ? Object(v.a)(i || (i = Object(f.a)(["\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      "]))) : Object(v.a)(c || (c = Object(f.a)([""])))
                         }));
-                    return o.a.createElement("div", {
+                    return s.a.createElement("div", {
                         style: {
                             height: "".concat(p.current, "px")
                         }
-                    }, o.a.createElement(O, {
-                        isUser: a
-                    }, o.a.createElement(b, {
-                        isUser: a,
+                    }, s.a.createElement(O, {
+                        isUser: r
+                    }, s.a.createElement(g, {
+                        isUser: r,
                         src: m,
                         alt: "profile",
                         draggable: "false"
-                    }), o.a.createElement(h, null, l)))
+                    }), s.a.createElement(h, null, l)))
                 },
-                y = function(e) {
-                    Object(m.a)(a, e);
-                    var t = Object(b.a)(a);
+                k = function(e) {
+                    Object(m.a)(r, e);
+                    var t = Object(g.a)(r);
 
-                    function a() {
+                    function r() {
                         var e;
-                        Object(p.a)(this, a);
-                        for (var r = arguments.length, n = new Array(r), i = 0; i < r; i++) n[i] = arguments[i];
+                        Object(p.a)(this, r);
+                        for (var a = arguments.length, n = new Array(a), i = 0; i < a; i++) n[i] = arguments[i];
                         return (e = t.call.apply(t, [this].concat(n))).render = function() {
                             h.a.setFrameHeight(window.innerHeight);
                             var t = e.props.args,
-                                a = t.isUser,
-                                r = t.message,
+                                r = t.isUser,
+                                a = t.message,
                                 n = t.animated,
                                 i = t.key,
                                 c = e.props.theme;
-                            if (!c) return o.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
-                            var s = Object(g.a)(O)({});
-                            return o.a.createElement(s, {
+                            if (!c) return s.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
+                            var o = Object(b.a)(O)({});
+                            return s.a.createElement(o, {
                                 args: {
-                                    isUser: a,
-                                    message: r,
+                                    isUser: r,
+                                    message: a,
                                     theme: c,
                                     animated: n,
                                     key: i
                                 }
                             })
                         }, e
                     }
-                    return Object(u.a)(a)
+                    return Object(u.a)(r)
                 }(h.b),
-                k = Object(h.c)(y);
-            d.a.render(o.a.createElement(o.a.StrictMode, null, o.a.createElement(k, null)), document.getElementById("root"))
+                y = Object(h.c)(k);
+            d.a.render(s.a.createElement(s.a.StrictMode, null, s.a.createElement(y, null)), document.getElementById("root"))
         }
     },
     [
         [31, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.6ecc478f.chunk.js.map
+//# sourceMappingURL=main.24daa2e9.chunk.js.map
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'static/js/main.24daa2e9.chunk.js'",*

 * * "'mappings'": "'wSA4DeA,EAlDmC,SAAC,GAAgD,IAA9CC,EAA6C,EAA7CA,KAAMC,EAAuC,EAAvCA,WAAYC,EAA2B,EAA3BA,eAAgBC,EAAW,EAAXA,KACrF,EAAsCC,mBAAS,IAA/C,mBAAOC,EAAP,KAAoBC,EAApB,KACMC,EAAUC,iBAAuB,MACvC,EAAkCJ,oBAAS,GAA3C,mBAAOK,EAAP,KAAkBC,EAAlB,KA2BA,OAzBAC,qBAAU,WACR,IAAIF,EAAJ,CAEA,IAAIG,EAAQ,EAENC,EAAWC,aAAY,WAC3B,GAAIF,EAAQZ,EAAKe,OAAQ,CAGvB,GAFAT,GAAe,SAACU,GAAD,OAAcA,EAAWhB,EAAKY,MAEzCL,EAAQU,QAAS,CACnB,IAAQC,EAAWX,EAAQU,QAAQE,wBAA3BD,OACRhB,EAAegB,GAGjBN,SAEA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.6ecc478f.chunk.js",
-    "mappings": "wSA4DeA,EAlDmC,SAAC,GAAgD,IAA9CC,EAA6C,EAA7CA,KAAMC,EAAuC,EAAvCA,WAAYC,EAA2B,EAA3BA,eAAgBC,EAAW,EAAXA,KACrF,EAAsCC,mBAAS,IAA/C,mBAAOC,EAAP,KAAoBC,EAApB,KACMC,EAAUC,iBAAuB,MACvC,EAAkCJ,oBAAS,GAA3C,mBAAOK,EAAP,KAAkBC,EAAlB,KA2BA,OAzBAC,qBAAU,WACR,IAAIF,EAAJ,CAEA,IAAIG,EAAQ,EAENC,EAAWC,aAAY,WAC3B,GAAIF,EAAQZ,EAAKe,OAAQ,CAGvB,GAFAT,GAAe,SAACU,GAAD,OAAcA,EAAWhB,EAAKY,MAEzCL,EAAQU,QAAS,CACnB,IAAQC,EAAWX,EAAQU,QAAQE,wBAA3BD,OACRhB,EAAegB,GAGjBN,SAEAQ,cAAcP,GACdZ,IACAS,GAAa,KAEd,IAEH,OAAO,kBAAMU,cAAcP,OAC1B,CAACb,EAAMC,EAAYC,EAAgBO,IAGpC,yBACEY,MAAO,CACLC,WAAYnB,EAAKoB,MAAMC,yBACvBC,OAAQ,wBACRC,aAAc,OACdC,QAAS,YACTC,OAAQ,WACRC,SAAU,MACVC,SAAU,OACVC,KAAM,EACNC,QAAS,QAEXC,IAAK1B,GAEJF,IC8EQ6B,EA5G4B,SAAC,GAAc,IAAZ/B,EAAW,EAAXA,KACpCgC,EAAmChC,EAAnCgC,OAAQC,EAA2BjC,EAA3BiC,QAChB,GAD2CjC,EAAlBkC,SAAkBlC,EAARmC,IACmBlC,oBAAS,IAA/D,mBACMmC,GADN,UAC2B/B,iBAAO,IAO9BgC,EAAY,GAIdA,EAHGL,EAGM,8EAFA,oNAMSM,YAAO1C,EAAP0C,CAAqB,CACvCnB,WAAYnB,EAAKoB,MAAMC,2BADzB,IAKMkB,EAASD,IAAOE,IACpB,CACElB,OAAO,wBACPC,aAAc,MACdR,OAAQ,OACR0B,MAAO,OACPhB,OAAQ,IAEV,SAACiB,GAEC,OAAIA,EAAMV,OACDW,YAAP,2GAMKA,YAAP,6BAKEC,EAAUN,IAAOO,IAAI,CACzBhB,QAAS,eACTV,WAAYnB,EAAKoB,MAAMC,yBACvBC,OAAQ,wBACRC,aAAc,OACdC,QAAS,YACTC,OAAQ,WACRV,OAAQ,OACRW,SAAU,MACVoB,WAAY,aAIRC,EAAOT,IAAOO,IAClB,CACEhB,QAAS,OACTD,KAAM,EACNF,SAAU,QACVX,OAAQ,OACRiC,SAAU,SAEZ,SAACN,GAEC,OAAIA,EAAMV,OACDW,YAAP,qIAOKA,YAAP,6BAsBJ,OACE,yBAAKzB,MAAO,CAAEH,OAAO,GAAD,OAAKqB,EAAmBtB,QAAxB,QAClB,kBAACiC,EAAD,CAAMf,OAAQA,GACZ,kBAACO,EAAD,CAAQP,OAAQA,EAAQiB,IAAKZ,EAAWa,IAAI,UAAUC,UAAU,UAC9D,kBAACP,EAAD,KAAUX,MCrHdc,E,4MAEGK,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAA2C,EAAKd,MAAM1C,KAA9CgC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,QAASC,EAAzB,EAAyBA,SAAUC,EAAnC,EAAmCA,IAK3Bf,EAAU,EAAKsB,MAAftB,MAIR,IAAKA,EACH,OAAO,oFAGX,IAAMqC,EAAsBnB,YAAOP,EAAPO,CAAsB,IAEhD,OACI,kBAACmB,EAAD,CAAqBzD,KAAM,CAAEgC,OAAQA,EAAQC,QAASA,EAASb,MAAOA,EAAOc,SAAUA,EAAUC,IAAKA,M,yBApB3FuB,KA0BJC,cAAwBZ,GChCvCa,IAASR,OACP,kBAAC,IAAMS,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
+    "file": "static/js/main.24daa2e9.chunk.js",
+    "mappings": "wSA4DeA,EAlDmC,SAAC,GAAgD,IAA9CC,EAA6C,EAA7CA,KAAMC,EAAuC,EAAvCA,WAAYC,EAA2B,EAA3BA,eAAgBC,EAAW,EAAXA,KACrF,EAAsCC,mBAAS,IAA/C,mBAAOC,EAAP,KAAoBC,EAApB,KACMC,EAAUC,iBAAuB,MACvC,EAAkCJ,oBAAS,GAA3C,mBAAOK,EAAP,KAAkBC,EAAlB,KA2BA,OAzBAC,qBAAU,WACR,IAAIF,EAAJ,CAEA,IAAIG,EAAQ,EAENC,EAAWC,aAAY,WAC3B,GAAIF,EAAQZ,EAAKe,OAAQ,CAGvB,GAFAT,GAAe,SAACU,GAAD,OAAcA,EAAWhB,EAAKY,MAEzCL,EAAQU,QAAS,CACnB,IAAQC,EAAWX,EAAQU,QAAQE,wBAA3BD,OACRhB,EAAegB,GAGjBN,SAEAQ,cAAcP,GACdZ,IACAS,GAAa,KAEd,IAEH,OAAO,kBAAMU,cAAcP,OAC1B,CAACb,EAAMC,EAAYC,EAAgBO,IAGpC,yBACEY,MAAO,CACLC,WAAYnB,EAAKoB,MAAMC,yBACvBC,OAAQ,wBACRC,aAAc,OACdC,QAAS,YACTC,OAAQ,WACRC,SAAU,MACVC,SAAU,OACVC,KAAM,EACNC,QAAS,QAEXC,IAAK1B,GAEJF,IC8EQ6B,EA5G4B,SAAC,GAAc,IAAZ/B,EAAW,EAAXA,KACpCgC,EAAmChC,EAAnCgC,OAAQC,EAA2BjC,EAA3BiC,QAChB,GAD2CjC,EAAlBkC,SAAkBlC,EAARmC,IACmBlC,oBAAS,IAA/D,mBACMmC,GADN,UAC2B/B,iBAAO,IAO9BgC,EAAY,GAIdA,EAHGL,EAGM,8JAFA,uGAMSM,YAAO1C,EAAP0C,CAAqB,CACvCnB,WAAYnB,EAAKoB,MAAMC,2BADzB,IAKMkB,EAASD,IAAOE,IACpB,CACElB,OAAO,wBACPC,aAAc,MACdR,OAAQ,OACR0B,MAAO,OACPhB,OAAQ,IAEV,SAACiB,GAEC,OAAIA,EAAMV,OACDW,YAAP,2GAMKA,YAAP,6BAKEC,EAAUN,IAAOO,IAAI,CACzBhB,QAAS,eACTV,WAAYnB,EAAKoB,MAAMC,yBACvBC,OAAQ,wBACRC,aAAc,OACdC,QAAS,YACTC,OAAQ,WACRV,OAAQ,OACRW,SAAU,MACVoB,WAAY,aAIRC,EAAOT,IAAOO,IAClB,CACEhB,QAAS,OACTD,KAAM,EACNF,SAAU,QACVX,OAAQ,OACRiC,SAAU,SAEZ,SAACN,GAEC,OAAIA,EAAMV,OACDW,YAAP,qIAOKA,YAAP,6BAsBJ,OACE,yBAAKzB,MAAO,CAAEH,OAAO,GAAD,OAAKqB,EAAmBtB,QAAxB,QAClB,kBAACiC,EAAD,CAAMf,OAAQA,GACZ,kBAACO,EAAD,CAAQP,OAAQA,EAAQiB,IAAKZ,EAAWa,IAAI,UAAUC,UAAU,UAC9D,kBAACP,EAAD,KAAUX,MCrHdc,E,4MAEGK,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAA2C,EAAKd,MAAM1C,KAA9CgC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,QAASC,EAAzB,EAAyBA,SAAUC,EAAnC,EAAmCA,IAK3Bf,EAAU,EAAKsB,MAAftB,MAIR,IAAKA,EACH,OAAO,oFAGX,IAAMqC,EAAsBnB,YAAOP,EAAPO,CAAsB,IAEhD,OACI,kBAACmB,EAAD,CAAqBzD,KAAM,CAAEgC,OAAQA,EAAQC,QAASA,EAASb,MAAOA,EAAOc,SAAUA,EAAUC,IAAKA,M,yBApB3FuB,KA0BJC,cAAwBZ,GChCvCa,IAASR,OACP,kBAAC,IAAMS,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
     "names": [
         "AnimatedText",
         "text",
         "onComplete",
         "onHeightChange",
         "args",
         "useState",
@@ -76,13 +76,13 @@
         "AnimatedText.tsx",
         "chatContainer.tsx",
         "stChat.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "import { randomInt } from 'crypto';\nimport React, { useState, useEffect, useRef } from 'react';\n\ninterface AnimatedTextProps {\n    text: string;\n    onComplete: () => void;\n    onHeightChange: (height: number) => void;\n    args: any;\n}\n\nconst AnimatedText: React.FC<AnimatedTextProps> = ({ text, onComplete, onHeightChange, args }) => {\n  const [visibleText, setVisibleText] = useState('');\n  const textRef = useRef<HTMLDivElement>(null);\n  const [completed, setCompleted] = useState(false);\n\n  useEffect(() => {\n    if (completed) return;\n\n    let index = 0;\n\n    const interval = setInterval(() => {\n      if (index < text.length) {\n        setVisibleText((prevText) => prevText + text[index]);\n\n        if (textRef.current) {\n          const { height } = textRef.current.getBoundingClientRect();\n          onHeightChange(height);\n        }\n\n        index++;\n      } else {\n        clearInterval(interval);\n        onComplete();\n        setCompleted(true);\n      }\n    }, 10); // Adjust the typing speed here\n\n    return () => clearInterval(interval);\n  }, [text, onComplete, onHeightChange, completed]);\n\n  return (\n    <div\n      style={{\n        background: args.theme.secondaryBackgroundColor,\n        border: '1px solid transparent',\n        borderRadius: '10px',\n        padding: '10px 14px',\n        margin: '5px 20px',\n        maxWidth: '80%',\n        fontSize: '1rem',\n        flex: 1,\n        display: 'flex',\n      }}\n      ref={textRef}\n    >\n      {visibleText}\n    </div>\n  );\n};\n\nexport default AnimatedText;\n",
-        "import React, { useEffect, useRef, useState } from \"react\";\nimport styled from \"@emotion/styled\";\nimport { css } from \"@emotion/react\";\nimport AnimatedText from './AnimatedText'; // Assuming both files are in the same folder\nimport { Streamlit } from \"streamlit-component-lib\";\n\ninterface ChatProps {\n  args: {\n    isUser: boolean;\n    message: string;\n    animated: boolean;\n    key: any;\n    theme: any;\n  \n  };\n}\n\ninterface AvatarProps {\n  isUser: boolean;\n}\n\ninterface ChatContainerProps {\n  isUser: boolean;\n}\n\nconst ChatContainer: React.FC<ChatProps> = ({ args }) => {\n  const { isUser, message, animated, key } = args;\n  const [isAnimationCompleted, setAnimationCompleted] = useState(false);\n  const containerHeightRef = useRef(0);\n\n  // Streamlit.setComponentValue(args); // Send the value back to Streamlit\n \n  \n\n\n  let avatarUrl = \"\";\n  if (!isUser) {\n    avatarUrl = `https://api.dicebear.com/6.x/avataaars/svg?seed=Felix&facialHair=beardMajestic&facialHairColor=2c1b18&eyes=happy&hairColor=4a312c&skinColor=d08b5b&style=circle&clothing=shirtVNeck&clothesColor=ffffff&top=curvy`;\n  } else {\n    avatarUrl = `https://api.dicebear.com/6.x/shapes/svg?backgroundType=gradientLinear,solid`;\n  }\n\n  // Styles for the Typing component\n  const TypingStyle = styled(AnimatedText)({\n    background: args.theme.secondaryBackgroundColor,\n  });\n\n  // styles for the avatar image\n  const Avatar = styled.img<AvatarProps>(\n    {\n      border: `1px solid transparent`,\n      borderRadius: \"50%\",\n      height: \"5rem\",\n      width: \"5rem\",\n      margin: 0,\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        `;\n      }\n      return css``;\n    }\n  );\n\n  // styles for the message box\n  const Message = styled.div({\n    display: \"inline-block\",\n    background: args.theme.secondaryBackgroundColor,\n    border: \"1px solid transparent\",\n    borderRadius: \"10px\",\n    padding: \"10px 14px\",\n    margin: \"5px 20px\",\n    height: \"auto\",\n    maxWidth: \"70%\",\n    whiteSpace: \"pre-line\",\n  });\n\n  // styles for the container\n  const Chat = styled.div<ChatContainerProps>(\n    {\n      display: \"flex\",\n      flex: 1,\n      maxWidth: \"100vw\",\n      height: \"auto\",\n      overflow: \"auto\",\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      `;\n      }\n      return css``;\n    }\n  );\n\n  const handleAnimationComplete = () => {\n    setAnimationCompleted(true);\n    args.animated=true\n    \n  };\n\n  const updateHeight = (height: number) => {\n    containerHeightRef.current = height;\n    //console.log(containerHeightRef.current)\n    if (height < 80){\n      Streamlit.setFrameHeight(80);\n    }else{\n      Streamlit.setFrameHeight(height);\n    }\n      \n\n  };\n\n  return (\n    <div style={{ height: `${containerHeightRef.current}px` }}>\n      <Chat isUser={isUser}>\n        <Avatar isUser={isUser} src={avatarUrl} alt=\"profile\" draggable=\"false\" />\n          <Message>{message}</Message>\n      </Chat>\n    </div>\n  );\n}\n\nexport default ChatContainer",
+        "import React, { useEffect, useRef, useState } from \"react\";\nimport styled from \"@emotion/styled\";\nimport { css } from \"@emotion/react\";\nimport AnimatedText from './AnimatedText'; // Assuming both files are in the same folder\nimport { Streamlit } from \"streamlit-component-lib\";\n\ninterface ChatProps {\n  args: {\n    isUser: boolean;\n    message: string;\n    animated: boolean;\n    key: any;\n    theme: any;\n  \n  };\n}\n\ninterface AvatarProps {\n  isUser: boolean;\n}\n\ninterface ChatContainerProps {\n  isUser: boolean;\n}\n\nconst ChatContainer: React.FC<ChatProps> = ({ args }) => {\n  const { isUser, message, animated, key } = args;\n  const [isAnimationCompleted, setAnimationCompleted] = useState(false);\n  const containerHeightRef = useRef(0);\n\n  // Streamlit.setComponentValue(args); // Send the value back to Streamlit\n \n  \n\n\n  let avatarUrl = \"\";\n  if (!isUser) {\n    avatarUrl = `https://user-images.githubusercontent.com/6371329/234966848-c28e98de-221c-433d-bd33-eea5f04414fe.png`;\n  } else {\n    avatarUrl = `https://api.dicebear.com/6.x/shapes/svg?shape1Color=6941EB&shape2Color=00C8BC&shape3Color=ffa532&backgroundColor=ffffff&backgroundType=gradientLinear,solid`;\n  }\n\n  // Styles for the Typing component\n  const TypingStyle = styled(AnimatedText)({\n    background: args.theme.secondaryBackgroundColor,\n  });\n\n  // styles for the avatar image\n  const Avatar = styled.img<AvatarProps>(\n    {\n      border: `1px solid transparent`,\n      borderRadius: \"50%\",\n      height: \"5rem\",\n      width: \"5rem\",\n      margin: 0,\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        `;\n      }\n      return css``;\n    }\n  );\n\n  // styles for the message box\n  const Message = styled.div({\n    display: \"inline-block\",\n    background: args.theme.secondaryBackgroundColor,\n    border: \"1px solid transparent\",\n    borderRadius: \"10px\",\n    padding: \"10px 14px\",\n    margin: \"5px 20px\",\n    height: \"auto\",\n    maxWidth: \"70%\",\n    whiteSpace: \"pre-line\",\n  });\n\n  // styles for the container\n  const Chat = styled.div<ChatContainerProps>(\n    {\n      display: \"flex\",\n      flex: 1,\n      maxWidth: \"100vw\",\n      height: \"auto\",\n      overflow: \"auto\",\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      `;\n      }\n      return css``;\n    }\n  );\n\n  const handleAnimationComplete = () => {\n    setAnimationCompleted(true);\n    args.animated=true\n    \n  };\n\n  const updateHeight = (height: number) => {\n    containerHeightRef.current = height;\n    //console.log(containerHeightRef.current)\n    if (height < 80){\n      Streamlit.setFrameHeight(80);\n    }else{\n      Streamlit.setFrameHeight(height);\n    }\n      \n\n  };\n\n  return (\n    <div style={{ height: `${containerHeightRef.current}px` }}>\n      <Chat isUser={isUser}>\n        <Avatar isUser={isUser} src={avatarUrl} alt=\"profile\" draggable=\"false\" />\n          <Message>{message}</Message>\n      </Chat>\n    </div>\n  );\n}\n\nexport default ChatContainer",
         "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from \"@emotion/styled\";\nimport ChatContainer from './chatContainer'\n\nclass Chat extends StreamlitComponentBase {\n\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, message, animated, key } = this.props.args;\n    // consrole.log(this.props.args)\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    // Styles for the Typing component\n  const StyledChatContainer = styled(ChatContainer)({\n  });\n    return (\n        <StyledChatContainer args={{ isUser: isUser, message: message, theme: theme, animated: animated, key: key}}/>\n\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Chat from \"./stChat\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Chat />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/PKG-INFO` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.3.1
-Summary: A streamlit component, to make chatbots with animated text
+Version: 0.0.3.2
+Summary: A streamlit component, to make chatbots with text
 Home-page: UNKNOWN
-Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
+Author: Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamlit-chat-animated-0.0.3.1/streamlit_chat_animated.egg-info/SOURCES.txt` & `streamlit-chat-animated-0.0.3.2/streamlit_chat_animated.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 streamlit_chat_animated.egg-info/dependency_links.txt
 streamlit_chat_animated.egg-info/requires.txt
 streamlit_chat_animated.egg-info/top_level.txt
 streamlit_chat_animated/frontend/build/asset-manifest.json
 streamlit_chat_animated/frontend/build/bootstrap.min.css
 streamlit_chat_animated/frontend/build/bootstrap.min.css.map
 streamlit_chat_animated/frontend/build/index.html
-streamlit_chat_animated/frontend/build/precache-manifest.230db9bd95594a43c51ef55435bd1bb4.js
+streamlit_chat_animated/frontend/build/precache-manifest.0c02e5679f95ab531f5daa41cbcc3366.js
 streamlit_chat_animated/frontend/build/service-worker.js
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
-streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js
-streamlit_chat_animated/frontend/build/static/js/main.6ecc478f.chunk.js.map
+streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js
+streamlit_chat_animated/frontend/build/static/js/main.24daa2e9.chunk.js.map
 streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
 streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
```


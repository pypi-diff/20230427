# Comparing `tmp/zendron-1.1.2.tar.gz` & `tmp/zendron-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.2.tar", last modified: Thu Apr 27 08:24:07 2023, max compression
+gzip compressed data, was "zendron-1.1.3.tar", last modified: Thu Apr 27 08:30:24 2023, max compression
```

## Comparing `zendron-1.1.2.tar` & `zendron-1.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.091717 zendron-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 08:23:53.000000 zendron-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 08:23:53.000000 zendron-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-27 08:24:07.091717 zendron-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-27 08:23:53.000000 zendron-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:23:53.000000 zendron-1.1.2/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 08:23:53.000000 zendron-1.1.2/conf/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 08:23:53.000000 zendron-1.1.2/conf/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-27 08:23:53.000000 zendron-1.1.2/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:23:53.000000 zendron-1.1.2/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 08:23:53.000000 zendron-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:24:07.091717 zendron-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.091717 zendron-1.1.2/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.091717 zendron-1.1.2/src/zendron/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/conf/default_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.087717 zendron-1.1.2/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.091717 zendron-1.1.2/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-27 08:23:53.000000 zendron-1.1.2/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:07.091717 zendron-1.1.2/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:24:07.000000 zendron-1.1.2/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 08:30:11.000000 zendron-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 08:30:11.000000 zendron-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-27 08:30:24.893953 zendron-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-27 08:30:11.000000 zendron-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-27 08:30:11.000000 zendron-1.1.3/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:30:11.000000 zendron-1.1.3/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 08:30:11.000000 zendron-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:30:24.893953 zendron-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.2/LICENSE` & `zendron-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/PKG-INFO` & `zendron-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.2
+Version: 1.1.3
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.1.2
+Version: 1.1.3
+[zendron Github](https://github.com/Mjvolk3/Zendron)
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
@@ -49,17 +50,26 @@
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
-- We recommend setting up you Zotero API key with the following settings to allow for full functionality. This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+- We recommend setting up you Zotero API key with the following settings to allow for full functionality.
+  - Personal Library
+    - [x] Allow library access.
+    - [x] Allow notes access.
+    - [x] Allow write access.
+  - Default Gropu Permissions
+    - [x] Read/Write
+
 ![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
+- This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
```

### Comparing `zendron-1.1.2/README.md` & `zendron-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Zendron
 
-Version: 1.1.2
+Version: 1.1.3
+[zendron Github](https://github.com/Mjvolk3/Zendron)
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
@@ -13,17 +14,26 @@
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
-- We recommend setting up you Zotero API key with the following settings to allow for full functionality. This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+- We recommend setting up you Zotero API key with the following settings to allow for full functionality.
+  - Personal Library
+    - [x] Allow library access.
+    - [x] Allow notes access.
+    - [x] Allow write access.
+  - Default Gropu Permissions
+    - [x] Read/Write
+
 ![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
+- This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
```

### Comparing `zendron-1.1.2/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.3/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/pods/dendron.markdown/config.import.yml` & `zendron-1.1.3/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/pyproject.toml` & `zendron-1.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.2"
+version = "1.1.3"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zendron-1.1.2/src/zendron/__main__.py` & `zendron-1.1.3/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/annotations.py` & `zendron-1.1.3/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/bibtex.py` & `zendron-1.1.3/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/cache.py` & `zendron-1.1.3/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/cache_deprecated.py` & `zendron-1.1.3/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/comments.py` & `zendron-1.1.3/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/comments_deprecated.py` & `zendron-1.1.3/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/conf/config_template.yaml` & `zendron-1.1.3/src/zendron/conf/config_template.yaml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/config.py` & `zendron-1.1.3/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/front.py` & `zendron-1.1.3/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/init.py` & `zendron-1.1.3/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/items.py` & `zendron-1.1.3/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/load.py` & `zendron-1.1.3/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/metadata.py` & `zendron-1.1.3/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/pods/dendron.markdown/config.import.yml` & `zendron-1.1.3/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/read_md.py` & `zendron-1.1.3/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/remove.py` & `zendron-1.1.3/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/scratch.py` & `zendron-1.1.3/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/sync.py` & `zendron-1.1.3/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron/user_citation_key.py` & `zendron-1.1.3/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.2/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.3/src/zendron.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.2
+Version: 1.1.3
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.1.2
+Version: 1.1.3
+[zendron Github](https://github.com/Mjvolk3/Zendron)
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
@@ -49,17 +50,26 @@
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
-- We recommend setting up you Zotero API key with the following settings to allow for full functionality. This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+- We recommend setting up you Zotero API key with the following settings to allow for full functionality.
+  - Personal Library
+    - [x] Allow library access.
+    - [x] Allow notes access.
+    - [x] Allow write access.
+  - Default Gropu Permissions
+    - [x] Read/Write
+
 ![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
+- This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
```

### Comparing `zendron-1.1.2/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.3/src/zendron.egg-info/SOURCES.txt`

 * *Files identical despite different names*


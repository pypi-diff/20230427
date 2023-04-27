# Comparing `tmp/zendron-1.0.9.tar.gz` & `tmp/zendron-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.0.9.tar", last modified: Wed Apr 26 08:29:22 2023, max compression
+gzip compressed data, was "zendron-1.1.0.tar", last modified: Thu Apr 27 08:18:51 2023, max compression
```

## Comparing `zendron-1.0.9.tar` & `zendron-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.953232 zendron-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 08:28:56.000000 zendron-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 08:28:56.000000 zendron-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:29:22.953232 zendron-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-26 08:28:56.000000 zendron-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 08:28:56.000000 zendron-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:29:22.953232 zendron-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/comments_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.953232 zendron-1.0.9/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.490342 zendron-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 08:18:35.000000 zendron-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 08:18:35.000000 zendron-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-27 08:18:51.490342 zendron-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-27 08:18:35.000000 zendron-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.486342 zendron-1.1.0/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:35.000000 zendron-1.1.0/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 08:18:35.000000 zendron-1.1.0/conf/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 08:18:35.000000 zendron-1.1.0/conf/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.486342 zendron-1.1.0/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.486342 zendron-1.1.0/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:18:35.000000 zendron-1.1.0/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 08:18:35.000000 zendron-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:18:51.490342 zendron-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.486342 zendron-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.490342 zendron-1.1.0/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.490342 zendron-1.1.0/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.486342 zendron-1.1.0/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.490342 zendron-1.1.0/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-27 08:18:35.000000 zendron-1.1.0/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:18:51.490342 zendron-1.1.0/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:18:51.000000 zendron-1.1.0/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.0.9/LICENSE` & `zendron-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/PKG-INFO` & `zendron-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.0.9
+Version: 1.1.0
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,58 +21,76 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
-Keywords: Zotero,Dendron
+Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.0.9
+Version: 1.1.0
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
 - It is recommended to build a [conda env](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for installation.
 - Install [Dendron CLI](https://wiki.dendron.so/notes/RjBkTbGuKCXJNuE4dyV6G/).
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
+## Zotero API key
+
+- [Zotero API key](https://www.zotero.org/settings/keys)
+- We recommend setting up you Zotero API key with the following settings to allow for full functionality. This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
 api_key : FoCauOvWMlNdYmpYuY5JplTw # Zotero API key
 collection: null # Name of Zotero Collection, null for entire library
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
 local_image_path: /Users/<username>/Zotero/cache # Local path for importing annotated images
 dendron_limb: zendron.import # Dendron import limb e.g. zendron.import.paper-title.annotations.md
 zotero_comment_title: zendron comment # fixed for now... needed for eventual 2-way sync.
-pod_path: zotero_pod # Name of dendron pod, removed
+pod_path: zotero_pod # Name of dendron pod, removed after completion of import. We will later add configuration for this to remain. This will allow for non Dendron users to import markdown Zotero notes in a strucutred hierarchy.
 ```
 
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
-  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Addition notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
+  - This command should only be run in the root directory of the workspace.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml` according the Zotero library specifications and the Zotero API.
+  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
 - `zendron remove=true`
   - This command removes all imported notes and associated links. We run a `createMissingLinkedNotes` following the deletion of Dendron notes to repopulate `tags` and `users` that will be removed on running `zendron-remove`.
-  - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to `str`.
+  - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
+
+## Miscellaneous
+
+- The `zendron_cache` is not currenlty in use. We do an entire relaod each time, so for large libraries performance will be poor.
+  - You an feel free to delete the cache as you please.
+- If there are run that fail, sometimes a `.hydra` with the given configuraiton will be generated in the root dir. This isn't an issue but it contains the API information and should therefore be added to the `.gitignore` as a safeguard. In addition these files can be used to inspect the reason for the faiure.
+- `__main__.log` is generated after running a `zendron`, this can also be deleted as you please. It is also useful for inspecting an failures to import.
+
+## Troubleshooting
+
+- If you are having trouble with startup you can use this [Zendron-Test](https://github.com/Mjvolk3/Zendron-Test) template and try to reproduce your issues here. Simply click on `Use this template`, clone the repo and try to run `zendron` here. This will allow for us to catch things we overlooked for different user workspace configuration etc. Once you have tried to reproduce issues here please submit an issue on [Zendron](https://github.com/Mjvolk3/Zendron).
```

### Comparing `zendron-1.0.9/pyproject.toml` & `zendron-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 # pyproject.toml
 
 [build-system]
-requires      = ["setuptools>=65.5.1", "wheel"]
+requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.0.9"
+version = "1.1.0"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["Zotero", "Dendron"]
+keywords = ["Zotero", "Dendron", "Markdown", "Notes", "Annotations", "VSCode"]
 dependencies = [
     "hydra-core >= 1.3.1",
     "tqdm >= 4.64.1",
     "pyzotero >= 1.5.5",
     "tomli >= 2.0.1",
     "python-frontmatter >= 1.0.0",
     "html2text >= 2020.1.16",
     "Markdown >= 3.4.1",
-    "markdownify >= 0.11.6"
+    "markdownify >= 0.11.6",
+    "importlib-metadata >= 6.6.0"
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Mjvolk3/Zendron"
 
 [project.scripts]
 zendron = "zendron.__main__:main"
+
+[options]
+packages = "find:"
+
+[options.package_data]
+zendron = ["*.yaml", "*.yml"]
```

### Comparing `zendron-1.0.9/src/zendron/__main__.py` & `zendron-1.1.0/src/zendron/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,21 +7,28 @@
 import hydra
 from omegaconf import DictConfig
 
 from zendron import init, load
 
 log = logging.getLogger(__name__)
 
+global USER_CONFIGURE
+USER_CONFIGURE = False
+
+if init.user_configure():
+    USER_CONFIGURE = True
+
 
 @hydra.main(
     version_base=None, config_path=osp.join(os.getcwd(), "conf"), config_name="config"
 )
 def main(cfg: DictConfig) -> None:
-    init.main()
-    if cfg.remove:
+    if USER_CONFIGURE:
+        return
+    elif cfg.remove:
         from zendron import remove
 
         log.info("Remove Starting")
 
         remove.main(cfg)
     else:
         log.info("Sync Starting")
```

### Comparing `zendron-1.0.9/src/zendron/annotations.py` & `zendron-1.1.0/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/bibtex.py` & `zendron-1.1.0/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/cache.py` & `zendron-1.1.0/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/cache_deprecated.py` & `zendron-1.1.0/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/comments.py` & `zendron-1.1.0/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/comments_deprecated.py` & `zendron-1.1.0/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/config.py` & `zendron-1.1.0/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/front.py` & `zendron-1.1.0/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/init.py` & `zendron-1.1.0/src/zendron/init.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,58 +11,77 @@
 
 from omegaconf import OmegaConf
 
 
 def load_default_config():
     workspace_root = os.getcwd()
     default_config_path = osp.join(workspace_root, "conf", "default.yaml")
+    if not osp.exists(default_config_path):
+        return False
     return OmegaConf.load(default_config_path)
 
 
 def is_initialized() -> bool:
-    default_config = load_default_config()
-    return default_config.initialized
+    try:
+        is_zendron_initialized = load_default_config().initialized
+    except:
+        is_zendron_initialized = False
+    return is_zendron_initialized
 
 
 def set_initialized():
     default_config = load_default_config()
     default_config.initialized = True
     workspace_root = os.getcwd()
     default_config_path = osp.join(workspace_root, "conf", "default.yaml")
     OmegaConf.save(default_config, default_config_path)
 
+    # Update config.import.yml with desired values
+    config_path = osp.join(
+        workspace_root, "pods", "dendron.markdown", "config.import.yml"
+    )
+    config = OmegaConf.load(config_path)
+    config.vaultName = workspace_root.split("/")[-1]
+    OmegaConf.save(config, config_path)
+
 
-def main():
+def user_configure() -> None:
     if not is_initialized():
         package_root = osp.dirname(osp.abspath(zendron.__file__))
-
+        # package_root = "/".join(package_root.split("/")[:-2])
         # List all the config files and their paths within the package
         config_files = [
             "conf/__init__.py",
-            "conf/config.yaml",
-            "conf/default.yaml",
+            "conf/default_template.yaml",
             "conf/config_template.yaml",
-            "pods/custom/dendron.markdown/config.import.yml",
+            "pods/dendron.markdown/config.import.yml",
         ]
 
         # Copy each config file to the user's workspace root directory
         for file_path in config_files:
             src_path = osp.join(package_root, file_path)
-            dest_path = osp.join(os.getcwd(), file_path)
+            dest_base_path, file_ext = osp.splitext(file_path)
+            dest_base_path = dest_base_path.replace("_template", "")
+            dest_path = osp.join(os.getcwd(), dest_base_path + file_ext)
 
             # Ensure the destination folder exists
             dest_folder = osp.dirname(dest_path)
             os.makedirs(dest_folder, exist_ok=True)
 
             if not osp.exists(dest_path):
                 shutil.copy2(src_path, dest_path)
                 print(f"{file_path} has been copied to the workspace root directory.")
             else:
                 print(f"{file_path} already exists in the workspace root directory.")
-            set_initialized()
-            log.info("Initialization complete.")
+        set_initialized()
+        print("Initialization complete.")
+        print(
+            "Manually set the STARTER CONFIG in './conf/config.yaml' for quickstart and rerun zendron. All other configs are optional."
+        )
+        return True
     else:
-        log.info(f"Zendron has already been initialized.")
+        print("Zendron has already been initialized.")
+        return False
 
 
 if __name__ == "__main__":
-    main()
+    user_configure()
```

### Comparing `zendron-1.0.9/src/zendron/items.py` & `zendron-1.1.0/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/load.py` & `zendron-1.1.0/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/metadata.py` & `zendron-1.1.0/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/read_md.py` & `zendron-1.1.0/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/remove.py` & `zendron-1.1.0/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/scratch.py` & `zendron-1.1.0/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/sync.py` & `zendron-1.1.0/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron/user_citation_key.py` & `zendron-1.1.0/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.9/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.0/src/zendron.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.0.9
+Version: 1.1.0
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,58 +21,76 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
-Keywords: Zotero,Dendron
+Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.0.9
+Version: 1.1.0
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
 - It is recommended to build a [conda env](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for installation.
 - Install [Dendron CLI](https://wiki.dendron.so/notes/RjBkTbGuKCXJNuE4dyV6G/).
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
+## Zotero API key
+
+- [Zotero API key](https://www.zotero.org/settings/keys)
+- We recommend setting up you Zotero API key with the following settings to allow for full functionality. This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
+![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
 api_key : FoCauOvWMlNdYmpYuY5JplTw # Zotero API key
 collection: null # Name of Zotero Collection, null for entire library
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
 local_image_path: /Users/<username>/Zotero/cache # Local path for importing annotated images
 dendron_limb: zendron.import # Dendron import limb e.g. zendron.import.paper-title.annotations.md
 zotero_comment_title: zendron comment # fixed for now... needed for eventual 2-way sync.
-pod_path: zotero_pod # Name of dendron pod, removed
+pod_path: zotero_pod # Name of dendron pod, removed after completion of import. We will later add configuration for this to remain. This will allow for non Dendron users to import markdown Zotero notes in a strucutred hierarchy.
 ```
 
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
-  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Addition notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
+  - This command should only be run in the root directory of the workspace.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml` according the Zotero library specifications and the Zotero API.
+  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
 - `zendron remove=true`
   - This command removes all imported notes and associated links. We run a `createMissingLinkedNotes` following the deletion of Dendron notes to repopulate `tags` and `users` that will be removed on running `zendron-remove`.
-  - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to `str`.
+  - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
+
+## Miscellaneous
+
+- The `zendron_cache` is not currenlty in use. We do an entire relaod each time, so for large libraries performance will be poor.
+  - You an feel free to delete the cache as you please.
+- If there are run that fail, sometimes a `.hydra` with the given configuraiton will be generated in the root dir. This isn't an issue but it contains the API information and should therefore be added to the `.gitignore` as a safeguard. In addition these files can be used to inspect the reason for the faiure.
+- `__main__.log` is generated after running a `zendron`, this can also be deleted as you please. It is also useful for inspecting an failures to import.
+
+## Troubleshooting
+
+- If you are having trouble with startup you can use this [Zendron-Test](https://github.com/Mjvolk3/Zendron-Test) template and try to reproduce your issues here. Simply click on `Use this template`, clone the repo and try to run `zendron` here. This will allow for us to catch things we overlooked for different user workspace configuration etc. Once you have tried to reproduce issues here please submit an issue on [Zendron](https://github.com/Mjvolk3/Zendron).
```

### Comparing `zendron-1.0.9/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.0/src/zendron.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 conf/__init__.py
 conf/config.yaml
-conf/config_template.yaml
 conf/default.yaml
+src/../conf/config.yaml
+src/../conf/default.yaml
+src/../pods/dendron.markdown/config.import.yml
 src/zendron/__init__.py
 src/zendron/__main__.py
 src/zendron/annotations.py
 src/zendron/bibtex.py
 src/zendron/cache.py
 src/zendron/cache_deprecated.py
 src/zendron/comments.py
@@ -27,8 +29,12 @@
 src/zendron/sync.py
 src/zendron/user_citation_key.py
 src/zendron.egg-info/PKG-INFO
 src/zendron.egg-info/SOURCES.txt
 src/zendron.egg-info/dependency_links.txt
 src/zendron.egg-info/entry_points.txt
 src/zendron.egg-info/requires.txt
-src/zendron.egg-info/top_level.txt
+src/zendron.egg-info/top_level.txt
+src/zendron/conf/__init__.py
+src/zendron/conf/config_template.yaml
+src/zendron/conf/default_template.yaml
+src/zendron/pods/dendron.markdown/config.import.yml
```


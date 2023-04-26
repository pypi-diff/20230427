# Comparing `tmp/cochleogram-0.2.0.tar.gz` & `tmp/cochleogram-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.2.0.tar", last modified: Wed Apr 26 22:17:08 2023, max compression
+gzip compressed data, was "cochleogram-0.2.1.tar", last modified: Wed Apr 26 22:26:37 2023, max compression
```

## Comparing `cochleogram-0.2.0.tar` & `cochleogram-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.818884 cochleogram-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.810883 cochleogram-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-26 22:16:53.000000 cochleogram-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-26 22:16:53.000000 cochleogram-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:17:08.814884 cochleogram-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26638 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 22:16:53.000000 cochleogram-0.2.0/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 22:16:53.000000 cochleogram-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-26 22:16:53.000000 cochleogram-0.2.0/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:17:08.818884 cochleogram-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.646900 cochleogram-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.642900 cochleogram-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.646900 cochleogram-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-26 22:26:23.000000 cochleogram-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-26 22:26:23.000000 cochleogram-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:26:37.646900 cochleogram-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.646900 cochleogram-0.2.1/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.646900 cochleogram-0.2.1/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26638 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-26 22:26:23.000000 cochleogram-0.2.1/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:26:37.646900 cochleogram-0.2.1/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 22:26:37.000000 cochleogram-0.2.1/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 22:26:23.000000 cochleogram-0.2.1/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 22:26:23.000000 cochleogram-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-26 22:26:23.000000 cochleogram-0.2.1/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:26:37.646900 cochleogram-0.2.1/setup.cfg
```

### Comparing `cochleogram-0.2.0/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/.gitignore` & `cochleogram-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/PKG-INFO` & `cochleogram-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.0
+Version: 0.2.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.0/cochleogram/gui.enaml` & `cochleogram-0.2.1/cochleogram/gui.enaml`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
     if path:
-        print('loading')
         load_processed_dataset(path, window, reader.LIFReader)
 
 
 def load_processed_dataset(path, window, reader_class):
     workspace = window.find('dock_area')
     # Remove existing cochlea
     for p in window.presenters:
@@ -89,15 +88,15 @@
     item = MPLDockItem(dock_area, name=f'dock_piece_{presenter.piece}', presenter=presenter)
     op = InsertTab(item=item.name, target=target)
     dock_area.update_layout(op)
     return item.name
 
 
 def remove_dock_item(dock_area, presenter):
-    op = RemoveItem(item=f'dock_piece_{presenter.piece.name}')
+    op = RemoveItem(item=f'dock_piece_{presenter.piece}')
     dock_area.update_layout(op)
 
 
 def save_state(parent, presenters):
     q = 'Your previous analysis will be overwritten. Are you sure?'
     button = question(parent, 'Confirm action', q)
     if button is not None and button.text == 'Yes':
```

### Comparing `cochleogram-0.2.0/cochleogram/icons/cells.png` & `cochleogram-0.2.1/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/icons/exclude.png` & `cochleogram-0.2.1/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/icons/main-icon.png` & `cochleogram-0.2.1/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/icons/make_icons.py` & `cochleogram-0.2.1/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/icons/spiral.png` & `cochleogram-0.2.1/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/icons/tile.png` & `cochleogram-0.2.1/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/instructions.html` & `cochleogram-0.2.1/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/main.py` & `cochleogram-0.2.1/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/model.py` & `cochleogram-0.2.1/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/plot.py` & `cochleogram-0.2.1/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/presenter.py` & `cochleogram-0.2.1/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram/reader.py` & `cochleogram-0.2.1/cochleogram/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         raise NotImplementedError
 
     def state_filename(self, piece):
         raise NotImplementedError
 
     def load_state(self, piece):
         state_filename = self.state_filename(piece)
-        print(state_filename)
         if not state_filename.exists():
             raise IOError('No saved analysis found')
         return json.loads(state_filename.read_text())
 
     def save_state(self, piece, state):
         state_filename = self.state_filename(piece)
         state_filename.parent.mkdir(exist_ok=True)
```

### Comparing `cochleogram-0.2.0/cochleogram/util.py` & `cochleogram-0.2.1/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.2.1/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.0
+Version: 0.2.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.0/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.2.1/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/pyproject.toml` & `cochleogram-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.0/readme.rst` & `cochleogram-0.2.1/readme.rst`

 * *Files identical despite different names*


# Comparing `tmp/cochleogram-0.1.8.tar.gz` & `tmp/cochleogram-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.1.8.tar", last modified: Mon Apr 24 22:16:13 2023, max compression
+gzip compressed data, was "cochleogram-0.2.0.tar", last modified: Wed Apr 26 22:17:08 2023, max compression
```

## Comparing `cochleogram-0.1.8.tar` & `cochleogram-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-24 22:16:02.000000 cochleogram-0.1.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-24 22:16:02.000000 cochleogram-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-24 22:16:13.679224 cochleogram-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26816 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 22:16:02.000000 cochleogram-0.1.8/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-24 22:16:02.000000 cochleogram-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-24 22:16:02.000000 cochleogram-0.1.8/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:16:13.679224 cochleogram-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.818884 cochleogram-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.810883 cochleogram-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-26 22:16:53.000000 cochleogram-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-26 22:16:53.000000 cochleogram-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:17:08.814884 cochleogram-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26638 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-26 22:16:53.000000 cochleogram-0.2.0/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:17:08.814884 cochleogram-0.2.0/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 22:17:08.000000 cochleogram-0.2.0/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 22:16:53.000000 cochleogram-0.2.0/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 22:16:53.000000 cochleogram-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-26 22:16:53.000000 cochleogram-0.2.0/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:17:08.818884 cochleogram-0.2.0/setup.cfg
```

### Comparing `cochleogram-0.1.8/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/.gitignore` & `cochleogram-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/PKG-INFO` & `cochleogram-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.8
+Version: 0.2.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.8/cochleogram/gui.enaml` & `cochleogram-0.2.0/cochleogram/gui.enaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
                                HGroup, Html, Label, MainWindow, Menu, MenuBar,
                                MPLCanvas, ObjectCombo, ProgressBar, PushButton,
                                Slider, Window)
 
 from cochleogram import plot, util
 from cochleogram.model import Cochlea
 from cochleogram.presenter import Presenter
+from cochleogram import reader
 
 
 def load_icon(name):
     data = resources.files('cochleogram.icons').joinpath(f'{name}.png').read_bytes()
     img = Image(data=data)
     icg = IconImage(image=img)
     return Icon(images=[icg])
@@ -43,38 +44,53 @@
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_existing_directory(window, current_path=window.current_path)
     if path:
-        load_processed_dataset(path, window)
+        load_processed_dataset(path, window, reader.ProcessedReader)
 
 
-def load_processed_dataset(path, window):
+def open_20x_lif_file(window):
+    # Check for unsaved changes
+    if any(p.unsaved_changes for p in window.presenters):
+        q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
+        button = question(None, 'Confirm action', q)
+        if button is None or button.text == 'No':
+            return
+
+    path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
+    if path:
+        print('loading')
+        load_processed_dataset(path, window, reader.LIFReader)
+
+
+def load_processed_dataset(path, window, reader_class):
     workspace = window.find('dock_area')
     # Remove existing cochlea
     for p in window.presenters:
         remove_dock_item(workspace, p)
 
+    iface = reader_class(path)
     # Now, load new cochlea
     window.current_path = path
-    window.cochlea = Cochlea.from_path(path)
-    window.presenters = [Presenter(p) for p in window.cochlea.pieces]
+    window.cochlea = iface.load_cochlea()
+    window.presenters = [Presenter(p, iface) for p in window.cochlea.pieces]
     target = 'help'
     for p in window.presenters:
         try:
             p.load_state()
         except IOError:
             pass
         target = add_dock_item(workspace, p, target)
 
 
 def add_dock_item(dock_area, presenter, target):
-    item = MPLDockItem(dock_area, name=f'dock_piece_{presenter.piece.name}', presenter=presenter)
+    item = MPLDockItem(dock_area, name=f'dock_piece_{presenter.piece}', presenter=presenter)
     op = InsertTab(item=item.name, target=target)
     dock_area.update_layout(op)
     return item.name
 
 
 def remove_dock_item(dock_area, presenter):
     op = RemoveItem(item=f'dock_piece_{presenter.piece.name}')
@@ -451,19 +467,27 @@
     attr presenters = []
     attr current_path = ''
 
     MenuBar:
         Menu:
             title = '&File'
             Action:
-                text = 'Open processed dataset\tCtrl+O'
+                text = 'Open processed dataset'
                 triggered ::
                     open_processed_dataset(window)
 
             Action:
+                text = 'Open 20x LIF file'
+                triggered ::
+                    open_20x_lif_file(window)
+
+            Action:
+                separator = True
+
+            Action:
                 text = 'Process 20x LIF file\tCtrl+P'
                 triggered ::
                     path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
                     if path:
                         pp = ProgressWindow()
                         pp.show()
                         cb = lambda x, pp=pp: setattr(pp, 'progress', x)
```

### Comparing `cochleogram-0.1.8/cochleogram/icons/cells.png` & `cochleogram-0.2.0/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/icons/exclude.png` & `cochleogram-0.2.0/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/icons/main-icon.png` & `cochleogram-0.2.0/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/icons/make_icons.py` & `cochleogram-0.2.0/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/icons/spiral.png` & `cochleogram-0.2.0/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/icons/tile.png` & `cochleogram-0.2.0/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/instructions.html` & `cochleogram-0.2.0/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/main.py` & `cochleogram-0.2.0/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/model.py` & `cochleogram-0.2.0/cochleogram/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import logging
 log = logging.getLogger(__name__)
 
-import json
-from pathlib import Path
-import pickle
-import re
-
-from atom.api import Atom, Dict, Event, Float, Int, List, Typed
+from atom.api import Atom, Dict, Event, Float, Int, List, Str, Typed
 from matplotlib import colors
 from matplotlib import transforms as T
 import numpy as np
 import pandas as pd
 
 from psiaudio.util import octave_space
 from scipy import interpolate
@@ -142,14 +137,17 @@
         i = np.argmin(d)
         if d[i] < hit_threshold:
             return i
         raise ValueError(f'No node within hit threshold of {hit_threshold}')
 
     def remove_node(self, x, y, hit_threshold=25):
         i = self.find_node(x, y, hit_threshold)
+        log.info('Removing node %d. Origin is %d.', i, self.origin)
+        if self.origin > i:
+            self.origin -= 1
         self.x.pop(i)
         self.y.pop(i)
         self.update_exclude()
         self.updated = True
 
     def set_origin(self, x, y, hit_threshold=25):
         self.origin = int(self.find_node(x, y, hit_threshold))
@@ -228,15 +226,15 @@
         self.updated = True
 
 
 class Tile(Atom):
 
     info = Dict()
     image = Typed(np.ndarray)
-    source = Typed(Path)
+    source = Str()
     extent = List()
     n_channels = Int()
 
     def __init__(self, info, image, source):
         self.info = info
         self.image = image
         self.source = source
@@ -253,20 +251,14 @@
         self.n_channels = self.image.shape[-1]
 
     def contains(self, x, y):
         contains_x = self.extent[0] <= x <= self.extent[1]
         contains_y = self.extent[2] <= y <= self.extent[3]
         return contains_x and contains_y
 
-    @classmethod
-    def from_filename(cls, img_filename):
-        image = np.load(img_filename)
-        info = json.loads(img_filename.with_suffix('.json').read_text())
-        return cls(info, image, img_filename)
-
     def to_coords(self, x, y, z=None):
         lower = self.info["lower"]
         voxel_size = self.info["voxel_size"]
         if z is None:
             indices = np.c_[x, y, np.full_like(x, lower[-1])]
         else:
             indices = np.c_[x, y, z]
@@ -416,58 +408,26 @@
         extent = np.array(self.extent)
         width, height = extent[1:4:2] - extent[:4:2]
         self.extent = [dx, dx + width, dy, dy + height] + extent[4:]
 
 
 class Piece:
 
-    def __init__(self, tiles, path, piece):
+    def __init__(self, tiles, piece):
         self.tiles = tiles
-        self.path = path
-        self.name = f'{path.stem}_piece_{piece}'
         self.piece = piece
         keys = 'IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra'
         self.spirals = {k: Points() for k in keys}
         self.cells = {k: Points() for k in keys}
 
     @property
     def channel_names(self):
         # We assume that each tile has the same set of channels
         return [c['name'] for c in self.tiles[0].info['channels']]
 
-    @classmethod
-    def from_path(cls, path, piece=None):
-        path = Path(path)
-        tile_filenames = sorted(path.glob(f"*piece_{piece}*.npy"))
-        log.info('Found tiles: %r', [t.stem for t in tile_filenames])
-        tiles = [Tile.from_filename(f) for f in tile_filenames]
-
-        # This pads the z-axis so that we have empty slices above/below stacks
-        # such that they should align properly in z-space. This simplifies a
-        # few downstream operations.
-        slice_n = np.array([t.image.shape[2] for t in tiles])
-        slice_lb = np.array([t.extent[4] for t in tiles])
-        slice_ub = np.array([t.extent[5] for t in tiles])
-        slice_scale = np.array([t.info['voxel_size'][2] for t in tiles])
-
-        z_scale = slice_scale[0]
-        z_min = min(slice_lb)
-        z_max = max(slice_ub)
-        z_n = int(np.ceil((z_max - z_min) / z_scale))
-
-        pad_bottom = np.round((slice_lb - z_min) / z_scale).astype('i')
-        pad_top = (z_n - pad_bottom - slice_n).astype('i')
-
-        for (t, pb, pt) in zip(tiles, pad_bottom, pad_top):
-            padding = [(0, 0), (0, 0), (pb, pt), (0, 0)]
-            t.image = np.pad(t.image, padding)
-            t.extent[4:] = [z_min, z_max]
-
-        return cls(tiles, path, piece)
-
     def get_image_extent(self):
         extents = np.vstack([tile.get_image_extent() for tile in self.tiles])
         xmin = extents[:, 0].min()
         xmax = extents[:, 1].max()
         ymin = extents[:, 2].min()
         ymax = extents[:, 3].max()
         return [xmin, xmax, ymin, ymax]
@@ -507,30 +467,30 @@
         t_base = self.tiles[0]
         extra_keys = set(t_base.info.keys()) - set(('lower', 'voxel_size', 'rotation'))
         for k in extra_keys:
             for t in self.tiles[1:]:
                 if t_base.info[k] != t.info[k]:
                     raise ValueError(f'Cannot merge tiles. {k} differs.')
             info[k] = t_base.info[k]
-        return Tile(info, merged_image, self.path)
+        return Tile(info, merged_image, f'piece_{self.piece}_merged')
 
     def get_state(self):
         return {
-            'tiles': {t.source.stem: t.get_state() for t in self.tiles},
+            'tiles': {t.source: t.get_state() for t in self.tiles},
             'spirals': {k: v.get_state() for k, v in self.spirals.items()},
             'cells': {k: v.get_state() for k, v in self.cells.items()},
         }
 
     def set_state(self, state):
         for k, v in self.spirals.items():
             v.set_state(state['spirals'][k])
         for k, v in self.cells.items():
             v.set_state(state['cells'][k])
         for tile in self.tiles:
-            tile.set_state(state['tiles'][tile.source.stem])
+            tile.set_state(state['tiles'][tile.source])
 
     def guess_cells(self, cell_type, width, spacing, channel):
         log.info('Finding %s assuming within %f um of spiral and spaced %f microns on channel %s',
                  cell_type, width, spacing, channel)
         tile = self.merge_tiles()
         x, y = self.spirals[cell_type].interpolate(resolution=0.0001)
         i = tile.map(x, y, channel, width=width)
@@ -560,25 +520,16 @@
 freq_fn = {
     'mouse': lambda d: (10**((1-d)*0.92) - 0.680) * 9.8,
 }
 
 
 class Cochlea:
 
-    def __init__(self, pieces, path):
+    def __init__(self, pieces):
         self.pieces = pieces
-        self.path = path
-        self.name = path.stem
-
-    @classmethod
-    def from_path(cls, path):
-        log.info('Loading cochlea from %s', path)
-        path = Path(path)
-        pieces = [Piece.from_path(path, p) for p in util.list_pieces(path)]
-        return cls(pieces, path)
 
     @property
     def channel_names(self):
         # We assume that each tile has the same set of channels
         names = set()
         for piece in self.pieces:
             names.update(piece.channel_names)
@@ -598,15 +549,15 @@
         # First, we need to merge the spirals
         xo, yo = 0, 0
         results = []
         for piece in self.pieces:
             s = piece.spirals[spiral]
             x, y = s.interpolate(resolution=0.001)
             if len(x) == 0:
-                raise ValueError(f'Please check the {spiral} spiral on piece {piece.name} and try again.')
+                raise ValueError(f'Please check the {spiral} spiral on piece {piece.piece} and try again.')
             x_norm = x - (x[0] - xo)
             y_norm = y - (y[0] - yo)
             xo = x_norm[-1]
             yo = y_norm[-1]
             i = np.arange(len(x)) / len(x)
             result = pd.DataFrame({
                 'direction': s.direction(),
```

### Comparing `cochleogram-0.1.8/cochleogram/plot.py` & `cochleogram-0.2.0/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/cochleogram/presenter.py` & `cochleogram-0.2.0/cochleogram/presenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,17 @@
 
     def contains(self, x, y):
         return self.tile.contains(x, y)
 
 
 class Presenter(Atom):
 
+    # Interface to help read data
+    reader = Value()
+
     # Tile artists
     tile_artists = Dict()
     current_artist_index = Value()
     current_artist = Value()
 
     # For spirals and cells
     point_artists = Dict()
@@ -367,19 +370,20 @@
 
     def _get_z_min(self):
         return min(a.z_slice_min for a in self.tile_artists.values())
 
     def _get_z_max(self):
         return min(a.z_slice_max for a in self.tile_artists.values())
 
-    def __init__(self, piece, *args, **kwargs):
+    def __init__(self, piece, reader, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.piece = piece
+        self.reader = reader
         self.tile_artists = {
-            t.source.name: ImagePlot(self.axes, t) for t in self.piece.tiles
+            t.source: ImagePlot(self.axes, t) for t in self.piece.tiles
         }
         for artist in self.tile_artists.values():
             artist.observe('updated', self.update)
         self.current_artist_index = None
         for key in ('IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra'):
             cells = PointPlot(self.axes, self.piece.cells[key], name=key)
             spiral = LinePlot(self.axes, self.piece.spirals[key], name=key)
@@ -740,25 +744,21 @@
     def get_full_state(self):
         return deepcopy({
             "data": self.piece.get_state(),
             "view": self.get_state(),
         })
 
     def save_state(self):
-        state_filename = self.piece.path / f"{self.piece.name}_analysis.json"
         state = self.get_full_state()
-        state_filename.write_text(json.dumps(state, indent=4))
+        self.reader.save_state(self.piece, state)
         self.saved_state = state
         self.update()
 
     def load_state(self):
-        state_filename = self.piece.path / f"{self.piece.name}_analysis.json"
-        if not state_filename.exists():
-            raise IOError('No saved analysis found')
-        state = json.loads(state_filename.read_text())
+        state = self.reader.load_state(self.piece)
         self.piece.set_state(state['data'])
         self.saved_state = state
         self.update()
 
     def redraw(self):
         self.figure.canvas.draw()
```

### Comparing `cochleogram-0.1.8/cochleogram/util.py` & `cochleogram-0.2.0/cochleogram/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,27 +106,16 @@
 
 def list_lif_stacks(filename):
     from readlif.reader import LifFile
     fh = LifFile(filename)
     return [stack.name for stack in fh.get_iter_image()]
 
 
-def load_lif(filename, piece, max_xy=512, dtype='uint8', reprocess=False):
+def load_lif(filename, piece, max_xy=4096, dtype='uint8'):
     filename = Path(filename)
-    cache_filename = (
-        filename.parent
-        / filename.stem
-        / (filename.stem + f'_{piece}')
-    )
-    info_filename = cache_filename.with_suffix('.json')
-    img_filename = cache_filename.with_suffix('.npy')
-    if not reprocess and info_filename.exists() and img_filename.exists():
-        info = json.loads(info_filename.read_text())
-        img = np.load(img_filename)
-        return info, img
 
     from readlif.reader import LifFile
     from readlif.utilities import get_xml
     fh = LifFile(filename)
     for stack in fh.get_iter_image():
         if stack.name == piece:
             break
@@ -150,22 +139,27 @@
     system_type = node.find('.//ScannerSettingRecord[@Identifier="SystemType"]').attrib['Variant']
     system = f'{system_type} {system_number}'
 
     pixels = np.array(stack.dims[:3])
     voxel_size = 1 / np.array(stack.scale[:3])
     lower = np.array([x_pos, y_pos, z_pos]) * 1e6
 
-    zoom = max_xy / max(pixels[:2])
+    zoom = min(1, max_xy / max(pixels[:2]))
     voxel_size[:2] /= zoom
 
-    shape = [max_xy, max_xy, stack.dims[2], stack.channels]
+    n = min(max_xy, max(pixels[:2]))
+
+    shape = [n, n, stack.dims[2], stack.channels]
     img = np.empty(shape, dtype=np.float32)
     for c in range(stack.channels):
         for z, s in enumerate(stack.get_iter_z(c=c)):
-            img[:, :, z, c] = ndimage.zoom(s, (zoom, zoom))
+            if zoom != 1:
+                img[:, :, z, c] = ndimage.zoom(s, (zoom, zoom))
+            else:
+                img[:, :, z, c] = s
 
     # Z-step was negative. Flip stack to fix this so that we always have a
     # positive Z-step.
     if voxel_size[2] < 0:
         img = img[:, :, ::-1]
         voxel_size[2] = -voxel_size[2]
 
@@ -204,32 +198,47 @@
 
     # Coerce to dtype, reorder so that tile origin is in lower corner of image
     # (makes it easer to reconcile with plotting), and swap axes from YX to XY.
     # Final axes ordering should be XYZC where C is channel and origin of XY
     # should be in lower corner of screen.
     img = img.astype(dtype)[::-1].swapaxes(0, 1)
 
-    cache_filename.parent.mkdir(exist_ok=True, parents=True)
-    info_filename.write_text(json.dumps(info, indent=2))
-    np.save(img_filename, img, allow_pickle=False)
     return info, img
 
 
 def process_lif(filename, reprocess, cb=None):
     pieces = list_lif_stacks(filename)
     n_pieces = len(pieces)
     if cb is None:
         cb = lambda x: x
     for p, piece in enumerate(pieces):
-        _ = load_lif(filename, piece, reprocess=reprocess)
+        # Check if already cached
+        cache_filename = (
+            filename.parent
+            / filename.stem
+            / (filename.stem + f'_{piece}')
+        )
+        info_filename = cache_filename.with_suffix('.json')
+        img_filename = cache_filename.with_suffix('.npy')
+        if cache and not reprocess and info_filename.exists() and img_filename.exists():
+            info = json.loads(info_filename.read_text())
+            img = np.load(img_filename)
+            continue
+
+        # Generate and cache
+        info, img = load_lif(filename, piece, reprocess=reprocess)
+        cache_filename.parent.mkdir(exist_ok=True, parents=True)
+        info_filename.write_text(json.dumps(info, indent=2))
+        np.save(img_filename, img, allow_pickle=False)
+
         progress = int((p + 1) / n_pieces * 100)
         cb(progress)
 
 
-def load_czi(filename, max_xy=512, dtype='uint8', reload=False):
+def load_czi(filename, max_xy=1024, dtype='uint8', reload=False):
     raise NotImplementedError
     # Note, this needs to be updated since I made some modifications to support
     # Leica LIF format and that includes changing imshow origin from lower to
     # upper since I was using the Leica viewer to make sure I got the extents
     # aligned properly.
 
     filename = Path(filename)
```

### Comparing `cochleogram-0.1.8/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.2.0/cochleogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.8
+Version: 0.2.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.8/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.2.0/cochleogram.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 cochleogram/__init__.py
 cochleogram/gui.enaml
 cochleogram/instructions.html
 cochleogram/main.py
 cochleogram/model.py
 cochleogram/plot.py
 cochleogram/presenter.py
+cochleogram/reader.py
 cochleogram/util.py
 cochleogram/version.py
 cochleogram.egg-info/PKG-INFO
 cochleogram.egg-info/SOURCES.txt
 cochleogram.egg-info/dependency_links.txt
 cochleogram.egg-info/entry_points.txt
 cochleogram.egg-info/requires.txt
```

### Comparing `cochleogram-0.1.8/pyproject.toml` & `cochleogram-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.8/readme.rst` & `cochleogram-0.2.0/readme.rst`

 * *Files identical despite different names*


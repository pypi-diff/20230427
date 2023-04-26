# Comparing `tmp/pygame-json-ui-0.0.0.3.tar.gz` & `tmp/pygame-json-ui-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-json-ui-0.0.0.3.tar", last modified: Mon Apr 24 17:37:37 2023, max compression
+gzip compressed data, was "pygame-json-ui-0.0.0.4.tar", last modified: Wed Apr 26 23:33:15 2023, max compression
```

## Comparing `pygame-json-ui-0.0.0.3.tar` & `pygame-json-ui-0.0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/
--rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9186 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8593 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/README.md
--rw-rw-rw-   0        0        0      671 2023-04-24 17:36:24.000000 pygame-json-ui-0.0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.604939 pygame-json-ui-0.0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.652539 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/
--rw-rw-rw-   0        0        0     9186 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/src/pygame_ui/
--rw-rw-rw-   0        0        0      711 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/__init__.py
--rw-rw-rw-   0        0        0     4566 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/base.py
--rw-rw-rw-   0        0        0      404 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/constants.py
--rw-rw-rw-   0        0        0     5765 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/elements.py
+drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.094774 pygame-json-ui-0.0.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     9225 2023-04-26 23:33:15.092769 pygame-json-ui-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8632 2023-04-26 23:30:32.000000 pygame-json-ui-0.0.0.4/README.md
+-rw-rw-rw-   0        0        0      713 2023-04-26 23:23:42.000000 pygame-json-ui-0.0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 23:33:15.094774 pygame-json-ui-0.0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.004381 pygame-json-ui-0.0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.064578 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/
+-rw-rw-rw-   0        0        0     9225 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.091072 pygame-json-ui-0.0.0.4/src/pygame_ui/
+-rw-rw-rw-   0        0        0      711 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/__init__.py
+-rw-rw-rw-   0        0        0     4592 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/base.py
+-rw-rw-rw-   0        0        0      404 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/constants.py
+-rw-rw-rw-   0        0        0     5791 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/elements.py
```

### Comparing `pygame-json-ui-0.0.0.3/LICENSE` & `pygame-json-ui-0.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame-json-ui-0.0.0.3/PKG-INFO` & `pygame-json-ui-0.0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-json-ui
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
 Author-email: Xander de Haan <sissydeslang@gmail.com>
 Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
 Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,16 +106,16 @@
 ```
 
 #### JSON File
 MUST be named `Interface.json` and in the same folder as python file for loading the json file automatically!
 
 ```json
 {
-   "label": {
-      "name": "test_label",
+   "test_label": {
+      "type": "label",
       "position": [200,100],
       "size": [120,80],
       "background_color": [200,0,0],
       "text": "IT WORKS!",
       "font_size": 20,
       "auto_size": true
    }
@@ -129,18 +129,18 @@
 - Label
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
-- `attribute: type` description (default value).
+- `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
-- `name: str` REQUIRED, used to access the element in python.
+- `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
@@ -204,27 +204,27 @@
 ### Frame Path
 
 A frame path is a string representation of the route to a certain frame.
 
 Say we have the following json file
 ```json
 {
-   "frame": {
-      "name": "Arthur"
+   "Arthur": {
+      "type": "frame"
       "contents": {
-         "frame": {
-            "name": "Bertha"
+         "Bertha": {
+            "type": "frame"
             "contents": {
-               "frame": {
-                  "name": "Pippinpaddleopsicopolis"
+               "Pippinpaddleopsicopolis": {
+                  "type": "frame"
                }
             }
          },
-         "frame": {
-            "name": "Cedric"
+         "Cedric": {
+            "type": "frame"
          }
       }
    }
 }
 ```
 
 and i wanted to access `Pippinpaddleopsicopolis`
@@ -238,22 +238,22 @@
 
 All examples use [this](#python-file) python file as base.
 
 ### A button
 
 ```json
 {
-   "button": {
-      "name": "harry the button",
+   "harry the button": {
+      "type": "button",
       "position": [250,120],
       "size": [200,200],
       "background_color": [100,0,0],
       "contents": {
-         "label": {
-            "name": "jonathan the label",
+         "jonathan the label": {
+            "type": "label",
             "position": [260,150],
             "font_size": 30,
             "auto_size": true
          }
       }
    }
 }
@@ -329,16 +329,16 @@
    pygame.display.flip()
    clock.tick(60)
 ```
 
 #### JSON
 ```json
 {
-   "frame": {
-      "name": "frame0",
+   "frame0": {
+      "type": "frame",
       "contents": {}
    }
 }
 ```
 
 ## FAQ
```

### Comparing `pygame-json-ui-0.0.0.3/README.md` & `pygame-json-ui-0.0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -92,16 +92,16 @@
 ```
 
 #### JSON File
 MUST be named `Interface.json` and in the same folder as python file for loading the json file automatically!
 
 ```json
 {
-   "label": {
-      "name": "test_label",
+   "test_label": {
+      "type": "label",
       "position": [200,100],
       "size": [120,80],
       "background_color": [200,0,0],
       "text": "IT WORKS!",
       "font_size": 20,
       "auto_size": true
    }
@@ -115,18 +115,18 @@
 - Label
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
-- `attribute: type` description (default value).
+- `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
-- `name: str` REQUIRED, used to access the element in python.
+- `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
@@ -190,27 +190,27 @@
 ### Frame Path
 
 A frame path is a string representation of the route to a certain frame.
 
 Say we have the following json file
 ```json
 {
-   "frame": {
-      "name": "Arthur"
+   "Arthur": {
+      "type": "frame"
       "contents": {
-         "frame": {
-            "name": "Bertha"
+         "Bertha": {
+            "type": "frame"
             "contents": {
-               "frame": {
-                  "name": "Pippinpaddleopsicopolis"
+               "Pippinpaddleopsicopolis": {
+                  "type": "frame"
                }
             }
          },
-         "frame": {
-            "name": "Cedric"
+         "Cedric": {
+            "type": "frame"
          }
       }
    }
 }
 ```
 
 and i wanted to access `Pippinpaddleopsicopolis`
@@ -224,22 +224,22 @@
 
 All examples use [this](#python-file) python file as base.
 
 ### A button
 
 ```json
 {
-   "button": {
-      "name": "harry the button",
+   "harry the button": {
+      "type": "button",
       "position": [250,120],
       "size": [200,200],
       "background_color": [100,0,0],
       "contents": {
-         "label": {
-            "name": "jonathan the label",
+         "jonathan the label": {
+            "type": "label",
             "position": [260,150],
             "font_size": 30,
             "auto_size": true
          }
       }
    }
 }
@@ -315,16 +315,16 @@
    pygame.display.flip()
    clock.tick(60)
 ```
 
 #### JSON
 ```json
 {
-   "frame": {
-      "name": "frame0",
+   "frame0": {
+      "type": "frame",
       "contents": {}
    }
 }
 ```
 
 ## FAQ
```

### Comparing `pygame-json-ui-0.0.0.3/pyproject.toml` & `pygame-json-ui-0.0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygame-json-ui"
-version = "0.0.0.3"
+version = "0.0.0.4"
 authors = [
   { name="Xander de Haan", email="sissydeslang@gmail.com" },
 ]
 description = "Pygame UI is a package for building user interfaces for pygame in a JSON Format."
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+	"pygame >= 2.3.0",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/PKG-INFO` & `pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-json-ui
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
 Author-email: Xander de Haan <sissydeslang@gmail.com>
 Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
 Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,16 +106,16 @@
 ```
 
 #### JSON File
 MUST be named `Interface.json` and in the same folder as python file for loading the json file automatically!
 
 ```json
 {
-   "label": {
-      "name": "test_label",
+   "test_label": {
+      "type": "label",
       "position": [200,100],
       "size": [120,80],
       "background_color": [200,0,0],
       "text": "IT WORKS!",
       "font_size": 20,
       "auto_size": true
    }
@@ -129,18 +129,18 @@
 - Label
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
-- `attribute: type` description (default value).
+- `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
-- `name: str` REQUIRED, used to access the element in python.
+- `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
@@ -204,27 +204,27 @@
 ### Frame Path
 
 A frame path is a string representation of the route to a certain frame.
 
 Say we have the following json file
 ```json
 {
-   "frame": {
-      "name": "Arthur"
+   "Arthur": {
+      "type": "frame"
       "contents": {
-         "frame": {
-            "name": "Bertha"
+         "Bertha": {
+            "type": "frame"
             "contents": {
-               "frame": {
-                  "name": "Pippinpaddleopsicopolis"
+               "Pippinpaddleopsicopolis": {
+                  "type": "frame"
                }
             }
          },
-         "frame": {
-            "name": "Cedric"
+         "Cedric": {
+            "type": "frame"
          }
       }
    }
 }
 ```
 
 and i wanted to access `Pippinpaddleopsicopolis`
@@ -238,22 +238,22 @@
 
 All examples use [this](#python-file) python file as base.
 
 ### A button
 
 ```json
 {
-   "button": {
-      "name": "harry the button",
+   "harry the button": {
+      "type": "button",
       "position": [250,120],
       "size": [200,200],
       "background_color": [100,0,0],
       "contents": {
-         "label": {
-            "name": "jonathan the label",
+         "jonathan the label": {
+            "type": "label",
             "position": [260,150],
             "font_size": 30,
             "auto_size": true
          }
       }
    }
 }
@@ -329,16 +329,16 @@
    pygame.display.flip()
    clock.tick(60)
 ```
 
 #### JSON
 ```json
 {
-   "frame": {
-      "name": "frame0",
+   "frame0": {
+      "type": "frame",
       "contents": {}
    }
 }
 ```
 
 ## FAQ
```

### Comparing `pygame-json-ui-0.0.0.3/src/pygame_ui/__init__.py` & `pygame-json-ui-0.0.0.4/src/pygame_ui/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Make sure you read the ``Getting started`` section of the documentation in the library folder.
 """
 
 from pygame_ui.base import *
 from pygame_ui.elements import *
 
 # release, year, month, session
-__version__ = '0.0.0.3'
+__version__ = '0.0.0.4'
 
 #print('Pygame UI ' + __version__)
 
 def test():
 	try:
 		import pygame_ui.base
 		import pygame_ui.constants
```

### Comparing `pygame-json-ui-0.0.0.3/src/pygame_ui/base.py` & `pygame-json-ui-0.0.0.4/src/pygame_ui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 	Calling this manually is deprecated.
 	"""
 
 	elements = {}
 	interactive_elements = []
 
 	def __init__(self, objects:dict):
-		for item_type, data in objects.items():
-			self.elements[data['name']] = getattr(pygame_ui.elements, item_type)(data)
+		for name, data in objects.items():
+			element_type = data.pop('type')
+			self.elements[name] = getattr(pygame_ui.elements, element_type)(data)
 
 	def get_frame(self, frame_path:str=''):
 		"""
 		Returns the frame of given path.
 		"""
 		
 		frame = self
```

### Comparing `pygame-json-ui-0.0.0.3/src/pygame_ui/elements.py` & `pygame-json-ui-0.0.0.4/src/pygame_ui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,17 @@
 	"""
 	
 	contents = {}
 
 	def __init__(self, *initial_data, **kwargs):
 		self.elements = {}
 		super().__init__(initial_data, kwargs)
-		for item_type, data in self.contents.items():
-			self.elements[data['name']] = globals()[item_type](data)
+		for name, data in self.contents.items():
+			element_type = data.pop('type')
+			self.elements[name] = globals()[element_type](data)
 	
 	def get_interactive_elements(self):
 		interactives = []
 		for name, element in self.elements.items():
 			if element.is_visible:
 				if isinstance(element, frame) and not isinstance(element, button):
 					interactives.extend(element.get_interactive_elements())
```


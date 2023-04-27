# Comparing `tmp/viser-0.0.6.tar.gz` & `tmp/viser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viser-0.0.6.tar", max compression
+gzip compressed data, was "viser-0.0.7.tar", max compression
```

## Comparing `viser-0.0.6.tar` & `viser-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,61 @@
--rw-r--r--   0        0        0     2348 2023-04-24 08:51:38.097792 viser-0.0.6/README.md
--rw-r--r--   0        0        0      655 2023-04-24 08:51:38.101792 viser-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      565 2023-04-24 08:51:38.101792 viser-0.0.6/viser/__init__.py
--rw-r--r--   0        0        0     7452 2023-04-24 08:51:38.101792 viser-0.0.6/viser/_gui.py
--rw-r--r--   0        0        0    21495 2023-04-24 08:51:38.101792 viser-0.0.6/viser/_message_api.py
--rw-r--r--   0        0        0     6913 2023-04-24 08:51:38.101792 viser-0.0.6/viser/_messages.py
--rw-r--r--   0        0        0     3226 2023-04-24 08:51:38.101792 viser-0.0.6/viser/_scene_handle.py
--rw-r--r--   0        0        0     8236 2023-04-24 08:51:38.101792 viser-0.0.6/viser/_viser.py
--rw-r--r--   0        0        0     1115 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/.eslintrc.js
--rw-r--r--   0        0        0      289 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/.gitignore
--rw-r--r--   0        0        0     2117 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/README.md
--rw-r--r--   0        0        0      369 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/asset-manifest.json
--rw-r--r--   0        0        0     1675 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/favicon.svg
--rw-r--r--   0        0        0      640 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/index.html
--rw-r--r--   0        0        0      286 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/manifest.json
--rw-r--r--   0        0        0       67 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/robots.txt
--rw-r--r--   0        0        0      441 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/static/css/main.992126cd.css
--rw-r--r--   0        0        0      843 2023-04-24 08:51:38.101792 viser-0.0.6/viser/client/build/static/css/main.992126cd.css.map
--rw-r--r--   0        0        0  1512219 2023-04-24 08:51:38.109793 viser-0.0.6/viser/client/build/static/js/main.3ff88750.js
--rw-r--r--   0        0        0     4434 2023-04-24 08:51:38.109793 viser-0.0.6/viser/client/build/static/js/main.3ff88750.js.LICENSE.txt
--rw-r--r--   0        0        0  5169245 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/build/static/js/main.3ff88750.js.map
--rw-r--r--   0        0        0     1910 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/package.json
--rw-r--r--   0        0        0     1675 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/public/favicon.svg
--rw-r--r--   0        0        0     1717 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/public/index.html
--rw-r--r--   0        0        0      286 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/public/manifest.json
--rw-r--r--   0        0        0       67 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/public/robots.txt
--rw-r--r--   0        0        0     7047 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/CameraControls.tsx
--rw-r--r--   0        0        0    10847 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ControlPanel/ControlPanel.tsx
--rw-r--r--   0        0        0     5793 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ControlPanel/Generated.tsx
--rw-r--r--   0        0        0     2308 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ControlPanel/GuiState.tsx
--rw-r--r--   0        0        0     3802 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ControlPanel/SceneTreeUI.tsx
--rw-r--r--   0        0        0     2101 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ControlPanel/Server.tsx
--rw-r--r--   0        0        0     1151 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/LabelRenderer.tsx
--rw-r--r--   0        0        0     8085 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/SceneTree.tsx
--rw-r--r--   0        0        0     1678 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/SearchParamsUtils.tsx
--rw-r--r--   0        0        0     3840 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/ThreeAssets.tsx
--rw-r--r--   0        0        0    18893 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/WebsocketInterface.tsx
--rw-r--r--   0        0        0     4221 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/WebsocketMessages.tsx
--rw-r--r--   0        0        0      509 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/index.css
--rw-r--r--   0        0        0     6257 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/src/react-app-env.d.ts
--rw-r--r--   0        0        0      503 2023-04-24 08:51:38.137795 viser-0.0.6/viser/client/tsconfig.json
--rw-r--r--   0        0        0   495759 2023-04-24 08:51:38.141795 viser-0.0.6/viser/client/yarn.lock
--rw-r--r--   0        0        0      160 2023-04-24 08:51:38.141795 viser-0.0.6/viser/extras/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-24 08:51:38.141795 viser-0.0.6/viser/extras/_record3d.py
--rw-r--r--   0        0        0      898 2023-04-24 08:51:38.141795 viser-0.0.6/viser/infra/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-24 08:51:38.141795 viser-0.0.6/viser/infra/_async_message_buffer.py
--rw-r--r--   0        0        0    11095 2023-04-24 08:51:38.141795 viser-0.0.6/viser/infra/_infra.py
--rw-r--r--   0        0        0     4429 2023-04-24 08:51:38.141795 viser-0.0.6/viser/infra/_messages.py
--rw-r--r--   0        0        0     3110 2023-04-24 08:51:38.141795 viser-0.0.6/viser/infra/_typescript_interface_gen.py
--rw-r--r--   0        0        0        0 2023-04-24 08:51:38.141795 viser-0.0.6/viser/py.typed
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 viser-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2348 2023-04-26 22:15:09.563548 viser-0.0.7/README.md
+-rw-r--r--   0        0        0      680 2023-04-26 22:15:09.567548 viser-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-04-26 22:15:09.567548 viser-0.0.7/viser/__init__.py
+-rw-r--r--   0        0        0     7442 2023-04-26 22:15:09.567548 viser-0.0.7/viser/_gui.py
+-rw-r--r--   0        0        0    22195 2023-04-26 22:15:09.567548 viser-0.0.7/viser/_message_api.py
+-rw-r--r--   0        0        0     7171 2023-04-26 22:15:09.567548 viser-0.0.7/viser/_messages.py
+-rw-r--r--   0        0        0     3115 2023-04-26 22:15:09.567548 viser-0.0.7/viser/_scene_handle.py
+-rw-r--r--   0        0        0    10535 2023-04-26 22:15:09.567548 viser-0.0.7/viser/_viser.py
+-rw-r--r--   0        0        0     1115 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/.eslintrc.js
+-rw-r--r--   0        0        0      289 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/.gitignore
+-rw-r--r--   0        0        0     2117 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/README.md
+-rw-r--r--   0        0        0      369 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/asset-manifest.json
+-rw-r--r--   0        0        0     1675 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/favicon.svg
+-rw-r--r--   0        0        0      640 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/index.html
+-rw-r--r--   0        0        0      286 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/robots.txt
+-rw-r--r--   0        0        0      441 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/static/css/main.992126cd.css
+-rw-r--r--   0        0        0      843 2023-04-26 22:15:09.567548 viser-0.0.7/viser/client/build/static/css/main.992126cd.css.map
+-rw-r--r--   0        0        0  1512411 2023-04-26 22:15:09.575548 viser-0.0.7/viser/client/build/static/js/main.36f6c191.js
+-rw-r--r--   0        0        0     4434 2023-04-26 22:15:09.575548 viser-0.0.7/viser/client/build/static/js/main.36f6c191.js.LICENSE.txt
+-rw-r--r--   0        0        0  5169188 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/build/static/js/main.36f6c191.js.map
+-rw-r--r--   0        0        0     1910 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/package.json
+-rw-r--r--   0        0        0     1675 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/public/favicon.svg
+-rw-r--r--   0        0        0     1717 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/public/index.html
+-rw-r--r--   0        0        0      286 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/public/robots.txt
+-rw-r--r--   0        0        0     7533 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/CameraControls.tsx
+-rw-r--r--   0        0        0    10847 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ControlPanel/ControlPanel.tsx
+-rw-r--r--   0        0        0     5793 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ControlPanel/Generated.tsx
+-rw-r--r--   0        0        0     2308 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ControlPanel/GuiState.tsx
+-rw-r--r--   0        0        0     3802 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ControlPanel/SceneTreeUI.tsx
+-rw-r--r--   0        0        0     2202 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ControlPanel/Server.tsx
+-rw-r--r--   0        0        0     1151 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/LabelRenderer.tsx
+-rw-r--r--   0        0        0     8085 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/SceneTree.tsx
+-rw-r--r--   0        0        0     1678 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/SearchParamsUtils.tsx
+-rw-r--r--   0        0        0     3840 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/ThreeAssets.tsx
+-rw-r--r--   0        0        0    17922 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/WebsocketInterface.tsx
+-rw-r--r--   0        0        0     4431 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/WebsocketMessages.tsx
+-rw-r--r--   0        0        0      509 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/index.css
+-rw-r--r--   0        0        0     6508 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      503 2023-04-26 22:15:09.603548 viser-0.0.7/viser/client/tsconfig.json
+-rw-r--r--   0        0        0   495759 2023-04-26 22:15:09.607548 viser-0.0.7/viser/client/yarn.lock
+-rw-r--r--   0        0        0      160 2023-04-26 22:15:09.607548 viser-0.0.7/viser/extras/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-26 22:15:09.607548 viser-0.0.7/viser/extras/_record3d.py
+-rw-r--r--   0        0        0      898 2023-04-26 22:15:09.607548 viser-0.0.7/viser/infra/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-26 22:15:09.607548 viser-0.0.7/viser/infra/_async_message_buffer.py
+-rw-r--r--   0        0        0    11299 2023-04-26 22:15:09.607548 viser-0.0.7/viser/infra/_infra.py
+-rw-r--r--   0        0        0     4429 2023-04-26 22:15:09.607548 viser-0.0.7/viser/infra/_messages.py
+-rw-r--r--   0        0        0     3110 2023-04-26 22:15:09.607548 viser-0.0.7/viser/infra/_typescript_interface_gen.py
+-rw-r--r--   0        0        0        0 2023-04-26 22:15:09.607548 viser-0.0.7/viser/py.typed
+-rw-r--r--   0        0        0      491 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/__init__.py
+-rw-r--r--   0        0        0     7955 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/_base.py
+-rw-r--r--   0        0        0     6532 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/_se2.py
+-rw-r--r--   0        0        0     6623 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/_se3.py
+-rw-r--r--   0        0        0     3378 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/_so2.py
+-rw-r--r--   0        0        0    12708 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/_so3.py
+-rw-r--r--   0        0        0      469 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/hints/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-26 22:15:09.607548 viser-0.0.7/viser/transforms/utils/_utils.py
+-rw-r--r--   0        0        0     3161 1970-01-01 00:00:00.000000 viser-0.0.7/PKG-INFO
```

### Comparing `viser-0.0.6/README.md` & `viser-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/pyproject.toml` & `viser-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "viser"
-version = "0.0.6"
+version = "0.0.7"
 description = "3D visualization helper"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.7,<3.11"
 websockets = ">=10.4"
 numpy = ">=1.0.0"
 msgpack = ">=1.0.0"
 imageio = ">=2.0.0"
 pyliblzfse = ">=0.4.1"
 scikit-image = ">=0.18.0"
+scipy = ">=1.7.3"
 tqdm = ">=4.0.0"
 tyro = ">=0.2.0"
 gdown = ">=4.6.6"
 rich = ">=13.3.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `viser-0.0.6/viser/__init__.py` & `viser-0.0.7/viser/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# `viser.infra` should be imported explicitly.
+# `viser.infra` and `viser.transforms` should be imported explicitly.
 # from . import infra as infra
+# from . import transforms as transforms
 from . import extras as extras
 from ._message_api import GuiButtonHandle as GuiButtonHandle
 from ._message_api import GuiHandle as GuiHandle
 from ._message_api import GuiSelectHandle as GuiSelectHandle
 from ._scene_handle import SceneNodeHandle as SceneNodeHandle
 from ._scene_handle import TransformControlsHandle as TransformControlsHandle
 from ._viser import CameraHandle as CameraHandle
```

### Comparing `viser-0.0.6/viser/_gui.py` & `viser-0.0.7/viser/_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Dict,
     Generic,
     List,
     Optional,
     Type,
     TypeVar,
     Union,
-    cast,
 )
 
 import numpy as onp
 
 from ._messages import (
     GuiRemoveMessage,
     GuiSetLevaConfMessage,
```

### Comparing `viser-0.0.6/viser/_message_api.py` & `viser-0.0.7/viser/_message_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,19 @@
                 fov=fov,
                 aspect=aspect,
                 scale=scale,
                 # (255, 255, 255) => 0xffffff, etc
                 color=_encode_rgb(color),
             )
         )
-        return SceneNodeHandle(_SceneNodeHandleState(name, self))
+        return SceneNodeHandle(
+            _SceneNodeHandleState(
+                name, self, wxyz=onp.array([1.0, 0.0, 0.0, 0.0]), position=onp.zeros(3)
+            )
+        )
 
     def add_frame(
         self,
         name: str,
         wxyz: Tuple[float, float, float, float] | onp.ndarray = (1.0, 0.0, 0.0, 0.0),
         position: Tuple[float, float, float] | onp.ndarray = (0.0, 0.0, 0.0),
         show_axes: bool = True,
@@ -380,15 +384,17 @@
                 position=position_tup,
                 show_axes=show_axes,
                 axes_length=axes_length,
                 axes_radius=axes_radius,
             )
         )
         return SceneNodeHandle(
-            _SceneNodeHandleState(name, self, wxyz=wxyz_tup, position=position_tup)
+            _SceneNodeHandleState(
+                name, self, wxyz=onp.asarray(wxyz), position=onp.asarray(position)
+            )
         )
 
     def add_point_cloud(
         self,
         name: str,
         position: onp.ndarray,
         color: onp.ndarray,
@@ -399,15 +405,19 @@
             _messages.PointCloudMessage(
                 name=name,
                 position=position.astype(onp.float32),
                 color=_colors_to_uint8(color),
                 point_size=point_size,
             )
         )
-        return SceneNodeHandle(_SceneNodeHandleState(name, self))
+        return SceneNodeHandle(
+            _SceneNodeHandleState(
+                name, self, wxyz=onp.array([1.0, 0.0, 0.0, 0.0]), position=onp.zeros(3)
+            )
+        )
 
     def add_mesh(
         self,
         name: str,
         vertices: onp.ndarray,
         faces: onp.ndarray,
         color: Tuple[int, int, int]
@@ -422,15 +432,19 @@
                 vertices.astype(onp.float32),
                 faces.astype(onp.uint32),
                 # (255, 255, 255) => 0xffffff, etc
                 color=_encode_rgb(color),
                 wireframe=wireframe,
             )
         )
-        return SceneNodeHandle(_SceneNodeHandleState(name, self))
+        return SceneNodeHandle(
+            _SceneNodeHandleState(
+                name, self, wxyz=onp.array([1.0, 0.0, 0.0, 0.0]), position=onp.zeros(3)
+            )
+        )
 
     def set_background_image(
         self,
         image: onp.ndarray,
         format: Literal["png", "jpeg"] = "jpeg",
         quality: Optional[int] = None,
     ) -> None:
@@ -458,15 +472,19 @@
                 name=name,
                 media_type=media_type,
                 base64_data=base64_data,
                 render_width=render_width,
                 render_height=render_height,
             )
         )
-        return SceneNodeHandle(_SceneNodeHandleState(name, self))
+        return SceneNodeHandle(
+            _SceneNodeHandleState(
+                name, self, wxyz=onp.array([1.0, 0.0, 0.0, 0.0]), position=onp.zeros(3)
+            )
+        )
 
     def add_transform_controls(
         self,
         name: str,
         scale: float = 1.0,
         line_width: float = 2.5,
         fixed: bool = False,
@@ -502,30 +520,32 @@
                 depth_test=depth_test,
                 opacity=opacity,
             )
         )
 
         def sync_cb(client_id: ClientId, state: TransformControlsHandle) -> None:
             message_orientation = _messages.SetOrientationMessage(
-                name=name, wxyz=state._impl.wxyz
+                name=name,
+                wxyz=tuple(map(float, state._impl.wxyz)),  # type: ignore
             )
             message_orientation.excluded_self_client = client_id
             self._queue(message_orientation)
 
             message_position = _messages.SetPositionMessage(
-                name=name, position=state._impl.position
+                name=name,
+                position=tuple(map(float, state._impl.position)),  # type: ignore
             )
             message_position.excluded_self_client = client_id
             self._queue(message_position)
 
         state = _SceneNodeHandleState(
             name=name,
             api=self,
-            wxyz=(1.0, 0.0, 0.0, 0.0),
-            position=(0.0, 0.0, 0.0),
+            wxyz=onp.array([1.0, 0.0, 0.0, 0.0]),
+            position=onp.array([0.0, 0.0, 0.0]),
         )
         state_aux = _TransformControlsState(
             last_updated=time.time(),
             update_cb=[],
             sync_cb=sync_cb,
         )
         handle = TransformControlsHandle(state, state_aux)
@@ -571,16 +591,16 @@
     ) -> None:
         """Callback for handling transform gizmo messages."""
         handle = self._handle_from_transform_controls_name.get(message.name, None)
         if handle is None:
             return
 
         # Update state.
-        handle._impl.wxyz = message.wxyz
-        handle._impl.position = message.position
+        handle._impl.wxyz = onp.array(message.wxyz)
+        handle._impl.position = onp.array(message.position)
         handle._impl_aux.last_updated = time.time()
 
         # Trigger callbacks.
         for cb in handle._impl_aux.update_cb:
             cb(handle)
         if handle._impl_aux.sync_cb is not None:
             handle._impl_aux.sync_cb(client_id, handle)
@@ -640,12 +660,15 @@
         - All outgoing messages are grouped and applied by clients atomically.
         - No incoming messages, like camera or GUI state updates, are processed.
 
         This can be helpful for things like animations, or when we want position and
         orientation updates to happen synchronously.
         """
         # Lock is needed for thread-safety.
-        self._atomic_lock.acquire()
+        got_lock = self._atomic_lock.acquire(blocking=False)
+
         self._queue(_messages.MessageGroupStart())
         yield
         self._queue(_messages.MessageGroupEnd())
-        self._atomic_lock.release()
+
+        if got_lock:
+            self._atomic_lock.release()
```

### Comparing `viser-0.0.6/viser/_messages.py` & `viser-0.0.7/viser/_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     """Message for a posed viewer camera.
     Pose is in the form T_world_camera, OpenCV convention, +Z forward."""
 
     wxyz: Tuple[float, float, float, float]
     position: Tuple[float, float, float]
     fov: float
     aspect: float
+    look_at: Tuple[float, float, float]
+    up_direction: Tuple[float, float, float]
 
 
 @dataclasses.dataclass
 class CameraFrustumMessage(Message):
     """Variant of CameraMessage used for visualizing camera frustums.
 
     OpenCV convention, +Z forward."""
@@ -133,28 +135,35 @@
         Tuple[float, float], Tuple[float, float], Tuple[float, float]
     ]
     depth_test: bool
     opacity: float
 
 
 @dataclasses.dataclass
-class SetCameraOrientationMessage(Message):
-    """Server -> client message to set the camera's orientation."""
+class SetCameraPositionMessage(Message):
+    """Server -> client message to set the camera's position."""
 
-    wxyz: Tuple[float, float, float, float]
+    position: Tuple[float, float, float]
 
 
 @dataclasses.dataclass
-class SetCameraPositionMessage(Message):
-    """Server -> client message to set the camera's position."""
+class SetCameraUpDirectionMessage(Message):
+    """Server -> client message to set the camera's up direction."""
 
     position: Tuple[float, float, float]
 
 
 @dataclasses.dataclass
+class SetCameraLookAtMessage(Message):
+    """Server -> client message to set the camera's look-at point."""
+
+    look_at: Tuple[float, float, float]
+
+
+@dataclasses.dataclass
 class SetCameraFovMessage(Message):
     """Server -> client message to set the camera's field of view."""
 
     fov: float
 
 
 @dataclasses.dataclass
```

### Comparing `viser-0.0.6/viser/_scene_handle.py` & `viser-0.0.7/viser/_scene_handle.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,57 +11,57 @@
     from ._message_api import ClientId, MessageApi
 
 
 @dataclasses.dataclass
 class _SceneNodeHandleState:
     name: str
     api: MessageApi
-    wxyz: Tuple[float, float, float, float] = (1.0, 0.0, 0.0, 0.0)
-    position: Tuple[float, float, float] = (0.0, 0.0, 0.0)
+    wxyz: onp.ndarray
+    position: onp.ndarray
     visible: bool = True
 
 
 @dataclasses.dataclass
 class SceneNodeHandle:
     """Handle for interacting with scene nodes."""
 
     _impl: _SceneNodeHandleState
 
     @property
-    def wxyz(self) -> Tuple[float, float, float, float]:
+    def wxyz(self) -> onp.ndarray:
         """Orientation of the scene node. This is the quaternion representation of the R
         in `p_parent = [R | t] p_local`. Synchronized to clients automatically when assigned.
         """
         return self._impl.wxyz
 
     @wxyz.setter
     def wxyz(self, wxyz: Tuple[float, float, float, float] | onp.ndarray) -> None:
         from ._message_api import cast_vector
 
         wxyz_cast = cast_vector(wxyz, 4)
-        self._impl.wxyz = wxyz_cast
+        self._impl.wxyz = onp.asarray(wxyz)
         self._impl.api._queue(
-            _messages.SetOrientationMessage(self._impl.name, self._impl.wxyz)
+            _messages.SetOrientationMessage(self._impl.name, wxyz_cast)
         )
 
     @property
-    def position(self) -> Tuple[float, float, float]:
+    def position(self) -> onp.ndarray:
         """Position of the scene node. This is equivalent to the t in
         `p_parent = [R | t] p_local`. Synchronized to clients automatically when assigned.
         """
         return self._impl.position
 
     @position.setter
     def position(self, position: Tuple[float, float, float] | onp.ndarray) -> None:
         from ._message_api import cast_vector
 
         position_cast = cast_vector(position, 3)
-        self._impl.position = position_cast
+        self._impl.position = onp.asarray(position)
         self._impl.api._queue(
-            _messages.SetPositionMessage(self._impl.name, self._impl.position)
+            _messages.SetPositionMessage(self._impl.name, position_cast)
         )
 
     @property
     def visible(self) -> bool:
         """Whether the scene node is visible or not. Synchronized to clients automatically when assigned."""
         return self._impl.visible
```

### Comparing `viser-0.0.6/viser/_viser.py` & `viser-0.0.7/viser/_viser.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,72 +3,91 @@
 import dataclasses
 import threading
 import time
 from pathlib import Path
 from typing import Callable, Dict, List, Tuple
 
 import numpy as onp
+import numpy.typing as npt
 from typing_extensions import override
 
 from . import infra
+from . import transforms as tf
 from ._message_api import MessageApi, cast_vector
 from ._messages import (
     SetCameraFovMessage,
-    SetCameraOrientationMessage,
+    SetCameraLookAtMessage,
     SetCameraPositionMessage,
+    SetCameraUpDirectionMessage,
     ViewerCameraMessage,
 )
 from ._scene_handle import SceneNodeHandle, _SceneNodeHandleState
 
 
 @dataclasses.dataclass
 class _CameraHandleState:
     """Information about a client's camera state."""
 
     connection: infra.ClientConnection
-    wxyz: Tuple[float, float, float, float]
-    position: Tuple[float, float, float]
+    wxyz: npt.NDArray[onp.float64]
+    position: npt.NDArray[onp.float64]
     fov: float
     aspect: float
+    look_at: npt.NDArray[onp.float64]
+    up_direction: npt.NDArray[onp.float64]
     update_timestamp: float
     camera_cb: List[Callable[[ClientHandle], None]]
 
 
 @dataclasses.dataclass
 class CameraHandle:
     _state: _CameraHandleState
 
     @property
-    def wxyz(self) -> Tuple[float, float, float, float]:
+    def wxyz(self) -> npt.NDArray[onp.float64]:
         """Corresponds to the R in `P_world = [R | t] p_camera`. Synchronized
         automatically when assigned."""
         assert self._state.update_timestamp != 0.0
         return self._state.wxyz
 
     # Note: asymmetric properties are supported in Pyright, but not yet in mypy.
     # - https://github.com/python/mypy/issues/3004
     # - https://github.com/python/mypy/pull/11643
     @wxyz.setter
     def wxyz(self, wxyz: Tuple[float, float, float, float] | onp.ndarray) -> None:
-        wxyz_cast = cast_vector(wxyz, 4)
-        self._state.wxyz = wxyz_cast
-        self._state.update_timestamp = time.time()
-        self._state.connection.send(SetCameraOrientationMessage(wxyz_cast))
+        R_world_camera = tf.SO3(onp.asarray(wxyz))
+        look_at = onp.array(
+            [
+                0.0,
+                0.0,
+                onp.linalg.norm(self.look_at - self.position),
+            ]
+        )
+        new_look_at = (R_world_camera @ look_at) + self.position
+        self.look_at = new_look_at
+
+        up_direction = R_world_camera @ onp.array([0.0, -1.0, 0.0])
+        self.up_direction = up_direction
+        self._state.wxyz = onp.asarray(wxyz)
 
     @property
-    def position(self) -> Tuple[float, float, float]:
+    def position(self) -> npt.NDArray[onp.float64]:
         """Corresponds to the t in `P_world = [R | t] p_camera`. Synchronized
         automatically when assigned."""
         assert self._state.update_timestamp != 0.0
         return self._state.position
 
     @position.setter
     def position(self, position: Tuple[float, float, float] | onp.ndarray) -> None:
+        offset = onp.asarray(position) - onp.array(self.position)  # type: ignore
+
         position_cast = cast_vector(position, 3)
-        self._state.position = position_cast
+
+        self._state.position = onp.asarray(position)
+        self.look_at = onp.array(self._state.look_at) + offset
         self._state.update_timestamp = time.time()
         self._state.connection.send(SetCameraPositionMessage(position_cast))
 
     @property
     def fov(self) -> float:
         """Vertical field of view of the camera, in radians. Synchronized automatically
         when assigned."""
@@ -88,14 +107,42 @@
         return self._state.aspect
 
     @property
     def update_timestamp(self) -> float:
         assert self._state.update_timestamp != 0.0
         return self._state.update_timestamp
 
+    @property
+    def look_at(self) -> npt.NDArray[onp.float64]:
+        """Look at point for the camera. Synchronized automatically when set."""
+        assert self._state.update_timestamp != 0.0
+        return self._state.look_at
+
+    @look_at.setter
+    def look_at(self, look_at: Tuple[float, float, float] | onp.ndarray) -> None:
+        look_at_cast = cast_vector(look_at, 3)
+        self._state.look_at = onp.asarray(look_at)
+        self._state.update_timestamp = time.time()
+        self._state.connection.send(SetCameraLookAtMessage(look_at_cast))
+
+    @property
+    def up_direction(self) -> npt.NDArray[onp.float64]:
+        """Up direction for the camera. Synchronized automatically when set."""
+        assert self._state.update_timestamp != 0.0
+        return self._state.up_direction
+
+    @up_direction.setter
+    def up_direction(
+        self, up_direction: Tuple[float, float, float] | onp.ndarray
+    ) -> None:
+        up_direction_cast = cast_vector(up_direction, 3)
+        self._state.up_direction = onp.asarray(up_direction)
+        self._state.update_timestamp = time.time()
+        self._state.connection.send(SetCameraUpDirectionMessage(up_direction_cast))
+
     def on_update(
         self, callback: Callable[[ClientHandle], None]
     ) -> Callable[[ClientHandle], None]:
         """Attach a callback to run when a new camera message is received."""
         self._state.camera_cb.append(callback)
         return callback
 
@@ -104,15 +151,15 @@
 class _ClientHandleState:
     connection: infra.ClientConnection
 
 
 @dataclasses.dataclass
 class ClientHandle(MessageApi):
     """Handle for interacting with a specific client. Can be used to send messages to
-    individual clients, read camera information, etc."""
+    individual clients and read/write camera information."""
 
     client_id: int
     camera: CameraHandle
     _state: _ClientHandleState
 
     def __post_init__(self):
         super().__init__(self._state.connection)
@@ -127,15 +174,19 @@
 class _ViserServerState:
     connection: infra.Server
     connected_clients: Dict[int, ClientHandle]
     client_lock: threading.Lock
 
 
 class ViserServer(MessageApi):
-    """Viser server class. The primary interface for functionality in `viser`."""
+    """Viser server class. The primary interface for functionality in `viser`.
+
+    Commands on a server object (`add_frame`, `add_gui_*`, ...) will be sent to all
+    clients, including new clients that connect after a command is called.
+    """
 
     world_axes: SceneNodeHandle
     """Handle for manipulating the world frame axes (/WorldAxes), which is instantiated
     and then hidden by default."""
 
     def __init__(self, host: str = "127.0.0.1", port: int = 8080):
         server = infra.Server(
@@ -153,44 +204,48 @@
         # For new clients, register and add a handler for camera messages.
         @server.on_client_connect
         def _(conn: infra.ClientConnection) -> None:
             camera = CameraHandle(
                 _CameraHandleState(
                     # TODO: values are initially not valid.
                     conn,
-                    wxyz=(1.0, 0.0, 0.0, 0.0),
-                    position=(0.0, 0.0, 0.0),
+                    wxyz=onp.zeros(4),
+                    position=onp.zeros(3),
                     fov=0.0,
                     aspect=0.0,
+                    look_at=onp.zeros(3),
+                    up_direction=onp.zeros(3),
                     update_timestamp=0.0,
                     camera_cb=[],
                 )
             )
             client = ClientHandle(conn.client_id, camera, _ClientHandleState(conn))
             first = True
 
             def handle_camera_message(
                 client_id: infra.ClientId, message: ViewerCameraMessage
             ) -> None:
-                assert client_id == client.client_id
+                nonlocal first
 
+                assert client_id == client.client_id
                 with self._atomic_lock:
                     client.camera._state = _CameraHandleState(
                         conn,
-                        message.wxyz,
-                        message.position,
+                        onp.array(message.wxyz),
+                        onp.array(message.position),
                         message.fov,
                         message.aspect,
+                        onp.array(message.look_at),
+                        onp.array(message.up_direction),
                         time.time(),
                         camera_cb=client.camera._state.camera_cb,
                     )
 
                 # We consider a client to be connected after the first camera message is
                 # received.
-                nonlocal first
                 if first:
                     with self._state.client_lock:
                         state.connected_clients[conn.client_id] = client
                     for cb in self._client_connect_cb:
                         cb(client)
                     first = False
 
@@ -207,15 +262,22 @@
 
             for cb in self._client_disconnect_cb:
                 cb(handle)
 
         # Start the server.
         server.start()
         self.reset_scene()
-        self.world_axes = SceneNodeHandle(_SceneNodeHandleState("/WorldAxes", self))
+        self.world_axes = SceneNodeHandle(
+            _SceneNodeHandleState(
+                "/WorldAxes",
+                self,
+                wxyz=onp.array([1.0, 0.0, 0.0, 0.0]),
+                position=onp.zeros(3),
+            )
+        )
         self.world_axes.visible = False
 
     def get_clients(self) -> Dict[int, ClientHandle]:
         """Creates and returns a copy of the mapping from connected client IDs to
         handles."""
         with self._state.client_lock:
             return self._state.connected_clients.copy()
```

### Comparing `viser-0.0.6/viser/client/.eslintrc.js` & `viser-0.0.7/viser/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/viser/client/README.md` & `viser-0.0.7/viser/client/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/viser/client/build/favicon.svg` & `viser-0.0.7/viser/client/build/favicon.svg`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/viser/client/build/index.html` & `viser-0.0.7/viser/client/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.svg"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>Viser</title><script defer="defer" src="/static/js/main.3ff88750.js"></script><link href="/static/css/main.992126cd.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.svg"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>Viser</title><script defer="defer" src="/static/js/main.36f6c191.js"></script><link href="/static/css/main.992126cd.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `viser-0.0.6/viser/client/build/static/css/main.992126cd.css.map` & `viser-0.0.7/viser/client/build/static/css/main.992126cd.css.map`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/viser/client/build/static/js/main.3ff88750.js` & `viser-0.0.7/viser/client/build/static/js/main.36f6c191.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.3ff88750.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.36f6c191.js.LICENSE.txt */ ! function() {
     var e = {
             7823: function(e) {
                 "use strict";
                 e.exports = function(e, t) {
                     if (null === e || "undefined" === typeof e) throw new TypeError("expected first argument to be an object.");
                     if ("undefined" === typeof t || "undefined" === typeof Symbol) return e;
                     if ("function" !== typeof Object.getOwnPropertySymbols) return e;
@@ -12410,14 +12410,17 @@
                 value: !0
             })
         }, n.nc = void 0;
     var r = {};
     ! function() {
         "use strict";
         n.d(r, {
+            x: function() {
+                return qj
+            },
             Z: function() {
                 return $j
             }
         });
         var e = {};
 
         function t(e) {
@@ -39297,15 +39300,15 @@
                 }), [a, S]), p.createElement("primitive", m({
                     ref: n,
                     object: S
                 }, c))
             }));
         try {
             Ub = new TextDecoder
-        } catch (Kj) {}
+        } catch (Zj) {}
         var Yb, Kb, Zb, Jb, Qb, ex = 0,
             tx = [],
             nx = tx,
             rx = 0,
             ix = {},
             ax = 0,
             ox = 0,
@@ -39319,15 +39322,15 @@
             })),
             cx = new ux;
         cx.name = "MessagePack 0xC1";
         var fx, dx, hx, px = !1,
             vx = 2;
         try {
             new Function("")
-        } catch (Kj) {
+        } catch (Zj) {
             vx = 1 / 0
         }
         var mx = function() {
             function e(t) {
                 et(this, e), t && (!1 === t.useRecords && void 0 === t.mapsAsObjects && (t.mapsAsObjects = !0), t.sequential && !1 !== t.trusted && (t.trusted = !0, t.structures || 0 == t.useRecords || (t.structures = [], t.maxSharedStructures || (t.maxSharedStructures = 0))), t.structures ? t.structures.sharedLength = t.structures.length : t.getStructures && ((t.structures = []).uninitialized = !0, t.structures.sharedLength = 0), t.int64AsNumber && (t.int64AsType = "number")), Object.assign(this, t)
             }
             return nt(e, [{
@@ -39336,16 +39339,16 @@
                     var r = this;
                     if (Fb) return Hx((function() {
                         return Vx(), r ? r.unpack(t, n) : e.prototype.unpack.call(lx, t, n)
                     }));
                     "object" === typeof n ? (Bb = n.end || t.length, ex = n.start || 0) : (ex = 0, Bb = n > -1 ? n : t.length), rx = 0, ox = 0, Kb = null, nx = tx, Zb = null, Fb = t;
                     try {
                         Qb = t.dataView || (t.dataView = new DataView(t.buffer, t.byteOffset, t.byteLength))
-                    } catch (Kj) {
-                        if (Fb = null, t instanceof Uint8Array) throw Kj;
+                    } catch (Zj) {
+                        if (Fb = null, t instanceof Uint8Array) throw Zj;
                         throw new Error("Source must be a Uint8Array or Buffer but was a " + (t && "object" == typeof t ? t.constructor.name : typeof t))
                     }
                     if (this instanceof e) {
                         if (ix = this, this.structures) return Yb = this.structures, gx(n);
                         (!Yb || Yb.length > 0) && (Yb = [])
                     } else ix = lx, (!Yb || Yb.length > 0) && (Yb = []);
                     return gx(n)
@@ -39361,16 +39364,16 @@
                         if (!t) {
                             for (n = [a]; ex < i;) r = ex, n.push(gx());
                             return n
                         }
                         if (!1 === t(a)) return;
                         for (; ex < i;)
                             if (r = ex, !1 === t(gx())) return
-                    } catch (Kj) {
-                        throw Kj.lastPosition = r, Kj.values = n, Kj
+                    } catch (Zj) {
+                        throw Zj.lastPosition = r, Zj.values = n, Zj
                     } finally {
                         px = !1, Vx()
                     }
                 }
             }, {
                 key: "_mergeStructures",
                 value: function(e, t) {
@@ -39405,16 +39408,16 @@
                 var n;
                 if (ix.randomAccessStructure && Fb[ex] < 64 && Fb[ex] >= 32 && fx ? (n = fx(Fb, ex, Bb, ix), Fb = null, e && e.lazy || !n || (n = n.toJSON()), ex = Bb) : n = bx(), Zb && (ex = Zb.postBundlePosition, Zb = null), ex == Bb) Yb && Yb.restoreStructures && yx(), Yb = null, Fb = null, Jb && (Jb = null);
                 else {
                     if (ex > Bb) throw new Error("Unexpected end of MessagePack data");
                     if (!px) throw new Error("Data read, but end of buffer not reached " + JSON.stringify(n).slice(0, 100))
                 }
                 return n
-            } catch (Kj) {
-                throw Yb && Yb.restoreStructures && yx(), Vx(), (Kj instanceof RangeError || Kj.message.startsWith("Unexpected end of buffer") || ex > Bb) && (Kj.incomplete = !0), Kj
+            } catch (Zj) {
+                throw Yb && Yb.restoreStructures && yx(), Vx(), (Zj instanceof RangeError || Zj.message.startsWith("Unexpected end of buffer") || ex > Bb) && (Zj.incomplete = !0), Zj
             }
         }
 
         function yx() {
             for (var e in Yb.restoreStructures) Yb[e] = Yb.restoreStructures[e];
             Yb.restoreStructures = null
         }
@@ -39847,15 +39850,15 @@
                 useRecords: !1
             }),
             Kx = Yx.unpack,
             Zx = (Yx.unpackMultiple, Yx.unpack, new Float32Array(1));
         new Uint8Array(Zx.buffer, 0, 4);
         try {
             $x = new TextEncoder
-        } catch (Kj) {}
+        } catch (Zj) {}
         var Jx, Qx, e_, t_, n_, r_ = "undefined" !== typeof Buffer,
             i_ = r_ ? function(e) {
                 return Buffer.allocUnsafeSlow(e)
             } : Uint8Array,
             a_ = r_ ? Buffer : Uint8Array,
             o_ = r_ ? 4294967296 : 2144337920,
             s_ = 0,
@@ -42905,104 +42908,101 @@
                                                 wxyz: [t.w, t.x, t.y, t.z],
                                                 position: n.toArray()
                                             })
                                         }
                                     })
                                 })));
                                 break;
-                            case "SetCameraOrientationMessage":
-                                var b = e.globalCameras.current.cameras[e.panelKey],
-                                    x = e.globalCameras.current.cameraControlRefs[e.panelKey].current,
-                                    _ = new _a(i.wxyz[1], i.wxyz[2], i.wxyz[3], i.wxyz[0]),
-                                    w = new _a,
-                                    S = new _a;
-                                w.setFromEuler(new lo(-Math.PI, 0, 0)), S.setFromEuler(new lo(-Math.PI / 2, 0, 0));
-                                var M = S.clone().multiply(_).multiply(w),
-                                    E = x.getPosition(new wa),
-                                    k = x.getTarget(new wa).sub(E).length(),
-                                    T = new wa(0, 0, -k).applyQuaternion(M).add(E),
-                                    C = 1e-7,
-                                    A = T.clone().sub(E).setY(C).normalize(),
-                                    P = new wa(C, 1, C).projectOnPlane(A).normalize();
-                                b.up.set(P.x, P.y, P.z), x.setLookAt(E.x, E.y, E.z, T.x, T.y, T.z);
+                            case "SetCameraLookAtMessage":
+                                var b = e.globalCameras.current.cameraControlRefs[e.panelKey].current,
+                                    x = new _a;
+                                x.setFromEuler(new lo(-Math.PI / 2, 0, 0));
+                                var _ = new wa(i.look_at[0], i.look_at[1], i.look_at[2]);
+                                _.applyQuaternion(x), b.setTarget(_.x, _.y, _.z);
+                                break;
+                            case "SetCameraUpDirectionMessage":
+                                var w = e.globalCameras.current.cameras[e.panelKey],
+                                    S = e.globalCameras.current.cameraControlRefs[e.panelKey].current,
+                                    M = new _a;
+                                M.setFromEuler(new lo(-Math.PI / 2, 0, 0));
+                                var E = new wa(i.position[0], i.position[1], i.position[2]).applyQuaternion(M);
+                                w.up.set(E.x, E.y, E.z), S.updateCameraUp();
                                 break;
                             case "SetCameraPositionMessage":
-                                var R = e.globalCameras.current.cameraControlRefs[e.panelKey].current,
-                                    O = new wa;
-                                R.getPosition(O);
-                                var L = new wa(i.position[0], i.position[1], i.position[2]),
-                                    I = new _a;
-                                I.setFromEuler(new lo(-Math.PI / 2, 0, 0)), L.applyQuaternion(I);
-                                var z = R.getTarget(new wa).add(L).sub(O);
-                                R.setLookAt(L.x, L.y, L.z, z.x, z.y, z.z);
+                                var k = e.globalCameras.current.cameraControlRefs[e.panelKey].current,
+                                    T = new wa(i.position[0], i.position[1], i.position[2]),
+                                    C = new _a;
+                                C.setFromEuler(new lo(-Math.PI / 2, 0, 0)), T.applyQuaternion(C), k.setPosition(T.x, T.y, T.z);
                                 break;
                             case "SetCameraFovMessage":
-                                var D = e.globalCameras.current.cameras[e.panelKey];
-                                D.setFocalLength(.5 * D.getFilmHeight() / Math.tan(i.fov / 2));
+                                var A = e.globalCameras.current.cameras[e.panelKey];
+                                A.setFocalLength(.5 * A.getFilmHeight() / Math.tan(i.fov / 2));
                                 break;
                             case "SetOrientationMessage":
                                 u(i.name, new _a(i.wxyz[1], i.wxyz[2], i.wxyz[3], i.wxyz[0]));
                                 break;
                             case "SetPositionMessage":
                                 c(i.name, new wa(i.position[0], i.position[1], i.position[2]));
                                 break;
                             case "BackgroundImageMessage":
-                                var N = t.background,
-                                    U = (new fp).load("data:".concat(i.media_type, ";base64,").concat(i.base64_data));
-                                t.background = U, t.background.encoding = Kr, AM(N) && N.dispose();
+                                var P = t.background,
+                                    R = (new fp).load("data:".concat(i.media_type, ";base64,").concat(i.base64_data));
+                                t.background = R, t.background.encoding = Kr, AM(P) && P.dispose(), e.useGui.setState({
+                                    backgroundAvailable: !0
+                                });
                                 break;
                             case "ImageMessage":
-                                var F = (new fp).load("data:".concat(i.media_type, ";base64,").concat(i.base64_data));
+                                var O = (new fp).load("data:".concat(i.media_type, ";base64,").concat(i.base64_data));
                                 d(new Ww(i.name, (function(e) {
                                     return (0, P_.jsxs)("mesh", {
                                         ref: e,
                                         children: [(0, P_.jsx)("planeGeometry", {
                                             attach: "geometry",
                                             args: [i.render_width, i.render_height]
                                         }), (0, P_.jsx)("meshBasicMaterial", {
                                             attach: "material",
                                             transparent: !0,
                                             side: Pt,
-                                            map: F
+                                            map: O
                                         })]
                                     })
                                 })));
                                 break;
                             case "RemoveSceneNodeMessage":
                                 console.log("Removing scene node:", i.name), n(i.name);
                                 break;
                             case "SetSceneNodeVisibilityMessage":
                                 f(i.name, i.visible);
                                 break;
                             case "ResetSceneMessage":
                                 r();
-                                var B = t.background;
-                                t.background = null, AM(B) && B.dispose(), e.useGui.setState({
+                                var L = t.background;
+                                t.background = null, AM(L) && L.dispose(), e.useGui.setState({
                                     backgroundAvailable: !1
                                 });
                                 break;
                             case "GuiAddMessage":
                                 a(i.name, {
                                     levaConf: i.leva_conf,
                                     folderLabels: i.folder_labels,
                                     visible: !0
                                 });
                                 break;
                             case "GuiSetValueMessage":
                                 l(i.name, i.value);
                                 break;
                             case "GuiSetVisibleMessage":
-                                var j = e.useGui.getState().guiConfigFromName[i.name];
-                                void 0 !== j && a(i.name, s(s({}, j), {}, {
+                                var I = e.useGui.getState().guiConfigFromName[i.name];
+                                void 0 !== I && a(i.name, s(s({}, I), {}, {
                                     visible: i.visible
                                 }));
                                 break;
                             case "GuiSetLevaConfMessage":
-                                var H = e.useGui.getState().guiConfigFromName[i.name];
-                                void 0 !== H && a(i.name, s(s({}, H), {}, {
+                                var z = e.useGui.getState().guiConfigFromName[i.name];
+                                void 0 !== z && a(i.name, s(s({}, z), {}, {
                                     levaConf: i.leva_conf
                                 }));
                                 break;
                             case "GuiRemoveMessage":
                                 o(i.name);
                                 break;
                             default:
@@ -43089,25 +43089,32 @@
                 t = jg((function(e) {
                     return e.camera
                 })),
                 n = p.useRef(null),
                 r = CM(e.websocketRef, 20),
                 i = p.useCallback((function() {
                     var e = t,
-                        n = new _a,
-                        i = new _a;
-                    n.setFromEuler(new lo(Math.PI, 0, 0)), i.setFromEuler(new lo(Math.PI / 2, 0, 0));
-                    var a = i.clone().multiply(e.quaternion).multiply(n);
-                    r({
-                        type: "ViewerCameraMessage",
-                        wxyz: [a.w, a.x, a.y, a.z],
-                        position: e.position.clone().applyQuaternion(i).toArray(),
-                        aspect: e.aspect,
-                        fov: e.fov * Math.PI / 180
-                    })
+                        a = n.current;
+                    if (null !== a) {
+                        var o = new _a,
+                            s = new _a;
+                        o.setFromEuler(new lo(Math.PI, 0, 0)), s.setFromEuler(new lo(Math.PI / 2, 0, 0));
+                        var l = s.clone().multiply(e.quaternion).multiply(o),
+                            u = a.getTarget(new wa).applyQuaternion(s),
+                            c = e.up.clone().applyQuaternion(s);
+                        r({
+                            type: "ViewerCameraMessage",
+                            wxyz: [l.w, l.x, l.y, l.z],
+                            position: e.position.clone().applyQuaternion(s).toArray(),
+                            aspect: e.aspect,
+                            fov: e.fov * Math.PI / 180,
+                            look_at: [u.x, u.y, u.z],
+                            up_direction: [c.x, c.y, c.z]
+                        })
+                    } else setTimeout(i, 10)
                 }), [t, r]);
             i();
             var a = p.useCallback((function() {
                     i();
                     var t = e.globalCameras.current;
                     t.synchronize && (t.synchronize = !1, t.cameraControlRefs.forEach((function(e) {
                         if (n !== e) {
@@ -45762,15 +45769,15 @@
             "hidden" === this.visibilityState && qT && ($T = !0)
         }
 
         function JT(e) {
             var t = e.target;
             try {
                 return t.matches(":focus-visible")
-            } catch (Kj) {}
+            } catch (Zj) {}
             return $T || function(e) {
                 var t = e.type,
                     n = e.tagName;
                 return !("INPUT" !== n || !XT[t] || e.readOnly) || "TEXTAREA" === n && !e.readOnly || !!e.isContentEditable
             }(t)
         }
         var QT = function() {
@@ -52210,18 +52217,18 @@
             u.current = r;
             var c = (0, p.useCallback)((function(e) {
                     return s(LL(n, e, u.current))
                 }), [n]),
                 f = (0, p.useCallback)((function(e) {
                     try {
                         i(e)
-                    } catch (Kj) {
-                        var t = Kj.type,
-                            n = Kj.previousValue;
-                        if ("LEVA_ERROR" !== t) throw Kj;
+                    } catch (Zj) {
+                        var t = Zj.type,
+                            n = Zj.previousValue;
+                        if ("LEVA_ERROR" !== t) throw Zj;
                         c(n)
                     }
                 }), [c, i]);
             return (0, p.useEffect)((function() {
                 LA(t, l.current) || c(t), l.current = t
             }), [t, c]), {
                 displayValue: o,
@@ -53776,17 +53783,17 @@
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, i, a = n.call(e),
                 o = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = a.next()).done;) o.push(r.value)
-            } catch (Kj) {
+            } catch (Zj) {
                 i = {
-                    error: Kj
+                    error: Zj
                 }
             } finally {
                 try {
                     r && !r.done && (n = a.return) && n.call(a)
                 } finally {
                     if (i) throw i.error
                 }
@@ -55770,15 +55777,15 @@
                                 var v = (0, p.useRef)(o);
                                 cU((function() {
                                     var e = function() {
                                             try {
                                                 var e = t.getState(),
                                                     n = l.current(e);
                                                 u.current(f.current, n) || (s.current = e, f.current = n, a())
-                                            } catch (Kj) {
+                                            } catch (Zj) {
                                                 c.current = !0, a()
                                             }
                                         },
                                         n = t.subscribe(e);
                                     return t.getState() !== v.current && e(), n
                                 }), []);
                                 var m = h ? e : f.current;
@@ -57308,55 +57315,55 @@
                     store: l,
                     hideCopyButton: !0
                 })
             })
         }
 
         function XF(e) {
-            var t = e.useGui((function(e) {
+            var t = (0, p.useContext)(qj),
+                n = e.useGui((function(e) {
                     return e.server
                 })),
-                n = e.useGui((function(e) {
+                r = e.useGui((function(e) {
                     return e.label
                 })),
-                r = e.useGui((function(e) {
+                i = e.useGui((function(e) {
                     return e.backgroundAvailable
                 })),
-                i = iF();
+                a = iF();
             return WF({
                 Label: {
-                    value: n,
+                    value: r,
                     onChange: function(t) {
                         return e.useGui.setState({
                             label: t
                         })
                     }
                 },
                 Websocket: {
-                    value: t,
+                    value: n,
                     onChange: function(t) {
                         return e.useGui.setState({
                             server: t
                         })
                     }
                 },
                 "Download Background": lF((function() {
-                    var t = e.wrapperRef.current;
-                    if (null !== t)
-                        if (t.style.backgroundImage.startsWith("url(")) {
-                            var n = t.style.backgroundImage.split('"')[1],
+                    if (null !== e.wrapperRef.current)
+                        if (AM(t.background)) {
+                            var n = t.background.image,
                                 r = document.createElement("a");
                             r.download = "background", r.href = n, document.body.appendChild(r), r.click(), document.body.removeChild(r)
                         } else alert("No background to download!")
                 }), {
-                    disabled: !r
+                    disabled: !i
                 })
             }, {
-                store: i
-            }, [r]), (0, P_.jsx)(sA, {
+                store: a
+            }, [i]), (0, P_.jsx)(sA, {
                 component: "div",
                 sx: {
                     "& label": {
                         color: "#777"
                     },
                     "& input[type='checkbox']~label svg path": {
                         stroke: "#fff !important"
@@ -57367,15 +57374,15 @@
                     }
                 },
                 children: (0, P_.jsx)(VF, {
                     fill: !0,
                     flat: !0,
                     titleBar: !1,
                     theme: $F,
-                    store: i,
+                    store: a,
                     hideCopyButton: !0
                 })
             })
         }
         var YF = !1,
             KF = "unmounted",
             ZF = "exited",
@@ -59574,15 +59581,16 @@
                             }))
                         }
                     })
                 })))
             }))[0]
         }
         var $j = p.createContext(null),
-            qj = p.memo((function(e) {
+            qj = p.createContext(null),
+            Xj = p.memo((function(e) {
                 var t = Ye(sA)(Oj || (Oj = h(["\n    width: 100%;\n    height: 100%;\n    position: relative;\n  "]))),
                     n = Ye($y)(Lj || (Lj = h(["\n    position: relative;\n    z-index: 0;\n\n    width: 100%;\n    height: 100%;\n  "])));
                 var r = new URLSearchParams(window.location.search).getAll(Zw),
                     i = e.panelKey < r.length ? r[e.panelKey] : function() {
                         var e = window.location.href;
                         return (e = (e = e.replace("http://", "ws://")).split("?")[0]).endsWith("/") && (e = e.slice(0, -1)), e
                     }(),
@@ -59654,36 +59662,41 @@
                                 })
                             })))
                         }))[0],
                         useGui: Gj(i),
                         websocketRef: p.useRef(null),
                         wrapperRef: p.useRef(null),
                         globalCameras: e.globalCameras
-                    };
+                    },
+                    o = new Fc;
                 return (0, P_.jsx)($j.Provider, {
                     value: a,
-                    children: (0, P_.jsxs)(t, {
-                        ref: a.wrapperRef,
-                        children: [(0, P_.jsx)(WB, {}), (0, P_.jsxs)(n, {
-                            camera: {
-                                position: [3, 3, -3]
-                            },
-                            children: [(0, P_.jsx)(PM, {}), (0, P_.jsx)(XB, {}), (0, P_.jsx)(RM, {}), (0, P_.jsx)(Yw, {
-                                name: "",
-                                useSceneTree: a.useSceneTree
-                            }), (0, P_.jsx)(gy, {
-                                preset: "city",
-                                blur: 1
+                    children: (0, P_.jsx)(qj.Provider, {
+                        value: o,
+                        children: (0, P_.jsxs)(t, {
+                            ref: a.wrapperRef,
+                            children: [(0, P_.jsx)(WB, {}), (0, P_.jsxs)(n, {
+                                camera: {
+                                    position: [3, 3, -3]
+                                },
+                                scene: o,
+                                children: [(0, P_.jsx)(PM, {}), (0, P_.jsx)(XB, {}), (0, P_.jsx)(RM, {}), (0, P_.jsx)(Yw, {
+                                    name: "",
+                                    useSceneTree: a.useSceneTree
+                                }), (0, P_.jsx)(gy, {
+                                    preset: "city",
+                                    blur: 1
+                                })]
                             })]
-                        })]
+                        })
                     })
                 })
             }));
 
-        function Xj() {
+        function Yj() {
             var e = (0, p.useRef)({
                     synchronize: !1,
                     cameras: [],
                     cameraControlRefs: []
                 }),
                 t = d((0, p.useState)(Math.max(1, Jw().length)), 2),
                 n = t[0],
@@ -59713,15 +59726,15 @@
                 sx: {
                     width: "100%",
                     height: "100%",
                     position: "relative",
                     boxSizing: "border-box",
                     paddingBottom: "2.5em"
                 },
-                children: [(0, P_.jsx)(Yj, {
+                children: [(0, P_.jsx)(Kj, {
                     panelCount: n,
                     setPanelCount: r,
                     globalCameras: e
                 }), Array.from({
                     length: n
                 }, (function(t, r) {
                     return (0, P_.jsx)(sA, {
@@ -59738,24 +59751,24 @@
                             position: "relative",
                             "&:not(:last-child)": {
                                 borderRight: i ? null : "1px solid",
                                 borderBottom: i ? "1px solid" : null,
                                 borderColor: "divider"
                             }
                         }),
-                        children: (0, P_.jsx)(qj, {
+                        children: (0, P_.jsx)(Xj, {
                             panelKey: r,
                             globalCameras: e
                         })
                     }, "box-" + r.toString())
                 }))]
             })
         }
 
-        function Yj(e) {
+        function Kj(e) {
             return (0, P_.jsx)(sA, {
                 component: "div",
                 sx: {
                     position: "fixed",
                     bottom: "0",
                     width: "100%",
                     height: "2.5em",
@@ -59790,11 +59803,11 @@
                         sx: {
                             pl: 1
                         },
                         disabled: 1 === e.panelCount
                     })]
                 })
             })
-        }(0, kS.s)(document.getElementById("root")).render((0, P_.jsx)(Xj, {}))
+        }(0, kS.s)(document.getElementById("root")).render((0, P_.jsx)(Yj, {}))
     }()
 }();
-//# sourceMappingURL=main.3ff88750.js.map
+//# sourceMappingURL=main.36f6c191.js.map
```

### Comparing `viser-0.0.6/viser/client/build/static/js/main.3ff88750.js.LICENSE.txt` & `viser-0.0.7/viser/client/build/static/js/main.36f6c191.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `viser-0.0.6/viser/client/build/static/js/main.3ff88750.js.map` & `viser-0.0.7/viser/client/build/static/js/main.36f6c191.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8555363581484496%*

 * *Differences: {"'file'": "'static/js/main.36f6c191.js'",*

 * * "'mappings'": "';iDASAA,EAAOC,QAAU,SAASC,EAAUC,GAClC,GAAiB,OAAbD,GAAyC,qBAAbA,EAC9B,MAAM,IAAIE,UAAU,4CAGtB,GAAuB,qBAAZD,GAA6C,qBAAXE,OAC3C,OAAOH,EAGT,GAA4C,oBAAjCI,OAAOC,sBAChB,OAAOL,EAOT,IAJA,IAAIM,EAAeF,OAAOG,UAAUC,qBAChCC,EAASL,OAAOJ,GAChBU,EAAMC,UAAUC,OAAQC,EAAI,IAEvBA,EAAIH,GAIX,IAHA,IAAII,EAAWV,OAAOO,UAAUE,IAC5BE,EAAQX,OAAOC,sBAAsBS,GAEhCE,EAAI,EAAGA,EAAID,EAAMH,OAAQI,IAAK,CACrC,IAAIC,EAAMF,EAAMC,GAEZV,EAAaY,KAAKJ,EAAUG,KAC9BR,EAAOQ,GAAOH,EAASG,GAE3B,CAEF,OA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.3ff88750.js",
+    "file": "static/js/main.36f6c191.js",
     "names": [
         "module",
         "exports",
         "receiver",
         "objects",
         "TypeError",
         "Symbol",
@@ -8403,36 +8403,32 @@
         "active_axes",
         "disable_axes",
         "disable_sliders",
         "disable_rotations",
         "translation_limits",
         "rotation_limits",
         "depth_test",
-        "globalCameras",
-        "panelKey",
         "cameraControls",
+        "globalCameras",
         "cameraControlRefs",
-        "R_world_camera",
-        "R_cam_threecam",
+        "panelKey",
         "R_threeworld_world",
-        "R_threeworld_threecamera",
-        "currentTargetDist",
-        "facePlane",
-        "projectOnPlane",
-        "position_cur",
+        "look_at",
+        "setTarget",
+        "updir",
         "position_cmd",
         "R_worldthree_world",
         "setFocalLength",
         "oldBackground",
         "media_type",
         "base64_data",
+        "backgroundAvailable",
         "colorMap",
         "render_width",
         "render_height",
-        "backgroundAvailable",
         "levaConf",
         "leva_conf",
         "folderLabels",
         "folder_labels",
         "currentConf",
         "guiConfigFromName",
         "useMessageHandler",
@@ -8458,16 +8454,19 @@
         "release",
         "acquired",
         "SynchronizedCameraControls",
         "cameraControlRef",
         "sendCameraThrottled",
         "sendCamera",
         "three_camera",
+        "camera_control",
         "R_threecam_cam",
         "R_world_threeworld",
+        "R_world_camera",
+        "up_direction",
         "cameraChangedCallback",
         "synchronize",
         "ours",
         "KEYCODE",
         "wKey",
         "holdEvent",
         "aKey",
@@ -11088,16 +11087,16 @@
         "getFolderContainer",
         "sendUpdate",
         "_propName",
         "guiSetQueue",
         "applyGuiSetQueue",
         "timeouts",
         "ServerControls",
+        "SceneContext",
         "Websocket",
-        "wrapper",
         "download",
         "alert",
         "UNMOUNTED",
         "EXITED",
         "ENTERING",
         "ENTERED",
         "EXITING",
@@ -11139,14 +11138,15 @@
         "_props$style",
         "transitionTimingFunction",
         "getCollapseUtilityClass",
         "CollapseRoot",
         "entered",
         "collapsedSize",
         "CollapseWrapper",
+        "wrapper",
         "CollapseWrapperInner",
         "wrapperInner",
         "Collapse",
         "_props$collapsedSize",
         "collapsedSizeProp",
         "_props$timeout",
         "_props$TransitionComp",
@@ -11970,16 +11970,16 @@
         "import _extends from '@babel/runtime/helpers/esm/extends';\nimport * as React from 'react';\nimport { Vector3, Vector2, Color } from 'three';\nimport { useThree } from '@react-three/fiber';\nimport { LineSegments2, Line2, LineMaterial, LineSegmentsGeometry, LineGeometry } from 'three-stdlib';\n\nconst Line = /*#__PURE__*/React.forwardRef(function Line({\n  points,\n  color = 'black',\n  vertexColors,\n  linewidth,\n  lineWidth,\n  segments,\n  dashed,\n  ...rest\n}, ref) {\n  const size = useThree(state => state.size);\n  const line2 = React.useMemo(() => segments ? new LineSegments2() : new Line2(), [segments]);\n  const [lineMaterial] = React.useState(() => new LineMaterial());\n  const lineGeom = React.useMemo(() => {\n    const geom = segments ? new LineSegmentsGeometry() : new LineGeometry();\n    const pValues = points.map(p => {\n      const isArray = Array.isArray(p);\n      return p instanceof Vector3 ? [p.x, p.y, p.z] : p instanceof Vector2 ? [p.x, p.y, 0] : isArray && p.length === 3 ? [p[0], p[1], p[2]] : isArray && p.length === 2 ? [p[0], p[1], 0] : p;\n    });\n    geom.setPositions(pValues.flat());\n\n    if (vertexColors) {\n      const cValues = vertexColors.map(c => c instanceof Color ? c.toArray() : c);\n      geom.setColors(cValues.flat());\n    }\n\n    return geom;\n  }, [points, segments, vertexColors]);\n  React.useLayoutEffect(() => {\n    line2.computeLineDistances();\n  }, [points, line2]);\n  React.useLayoutEffect(() => {\n    if (dashed) {\n      lineMaterial.defines.USE_DASH = '';\n    } else {\n      // Setting lineMaterial.defines.USE_DASH to undefined is apparently not sufficient.\n      delete lineMaterial.defines.USE_DASH;\n    }\n\n    lineMaterial.needsUpdate = true;\n  }, [dashed, lineMaterial]);\n  React.useEffect(() => {\n    return () => lineGeom.dispose();\n  }, [lineGeom]);\n  return /*#__PURE__*/React.createElement(\"primitive\", _extends({\n    object: line2,\n    ref: ref\n  }, rest), /*#__PURE__*/React.createElement(\"primitive\", {\n    object: lineGeom,\n    attach: \"geometry\"\n  }), /*#__PURE__*/React.createElement(\"primitive\", _extends({\n    object: lineMaterial,\n    attach: \"material\",\n    color: color,\n    vertexColors: Boolean(vertexColors),\n    resolution: [size.width, size.height],\n    linewidth: linewidth !== null && linewidth !== void 0 ? linewidth : lineWidth,\n    dashed: dashed\n  }, rest)));\n});\n\nexport { Line };\n",
         "import _extends from '@babel/runtime/helpers/esm/extends';\nimport * as React from 'react';\nimport * as ReactDOM from 'react-dom/client';\nimport { Vector3, DoubleSide, OrthographicCamera, PerspectiveCamera } from 'three';\nimport { useThree, useFrame } from '@react-three/fiber';\n\nconst v1 = new Vector3();\nconst v2 = new Vector3();\nconst v3 = new Vector3();\n\nfunction defaultCalculatePosition(el, camera, size) {\n  const objectPos = v1.setFromMatrixPosition(el.matrixWorld);\n  objectPos.project(camera);\n  const widthHalf = size.width / 2;\n  const heightHalf = size.height / 2;\n  return [objectPos.x * widthHalf + widthHalf, -(objectPos.y * heightHalf) + heightHalf];\n}\n\nfunction isObjectBehindCamera(el, camera) {\n  const objectPos = v1.setFromMatrixPosition(el.matrixWorld);\n  const cameraPos = v2.setFromMatrixPosition(camera.matrixWorld);\n  const deltaCamObj = objectPos.sub(cameraPos);\n  const camDir = camera.getWorldDirection(v3);\n  return deltaCamObj.angleTo(camDir) > Math.PI / 2;\n}\n\nfunction isObjectVisible(el, camera, raycaster, occlude) {\n  const elPos = v1.setFromMatrixPosition(el.matrixWorld);\n  const screenPos = elPos.clone();\n  screenPos.project(camera);\n  raycaster.setFromCamera(screenPos, camera);\n  const intersects = raycaster.intersectObjects(occlude, true);\n\n  if (intersects.length) {\n    const intersectionDistance = intersects[0].distance;\n    const pointDistance = elPos.distanceTo(raycaster.ray.origin);\n    return pointDistance < intersectionDistance;\n  }\n\n  return true;\n}\n\nfunction objectScale(el, camera) {\n  if (camera instanceof OrthographicCamera) {\n    return camera.zoom;\n  } else if (camera instanceof PerspectiveCamera) {\n    const objectPos = v1.setFromMatrixPosition(el.matrixWorld);\n    const cameraPos = v2.setFromMatrixPosition(camera.matrixWorld);\n    const vFOV = camera.fov * Math.PI / 180;\n    const dist = objectPos.distanceTo(cameraPos);\n    const scaleFOV = 2 * Math.tan(vFOV / 2) * dist;\n    return 1 / scaleFOV;\n  } else {\n    return 1;\n  }\n}\n\nfunction objectZIndex(el, camera, zIndexRange) {\n  if (camera instanceof PerspectiveCamera || camera instanceof OrthographicCamera) {\n    const objectPos = v1.setFromMatrixPosition(el.matrixWorld);\n    const cameraPos = v2.setFromMatrixPosition(camera.matrixWorld);\n    const dist = objectPos.distanceTo(cameraPos);\n    const A = (zIndexRange[1] - zIndexRange[0]) / (camera.far - camera.near);\n    const B = zIndexRange[1] - A * camera.far;\n    return Math.round(A * dist + B);\n  }\n\n  return undefined;\n}\n\nconst epsilon = value => Math.abs(value) < 1e-10 ? 0 : value;\n\nfunction getCSSMatrix(matrix, multipliers, prepend = '') {\n  let matrix3d = 'matrix3d(';\n\n  for (let i = 0; i !== 16; i++) {\n    matrix3d += epsilon(multipliers[i] * matrix.elements[i]) + (i !== 15 ? ',' : ')');\n  }\n\n  return prepend + matrix3d;\n}\n\nconst getCameraCSSMatrix = (multipliers => {\n  return matrix => getCSSMatrix(matrix, multipliers);\n})([1, -1, 1, 1, 1, -1, 1, 1, 1, -1, 1, 1, 1, -1, 1, 1]);\n\nconst getObjectCSSMatrix = (scaleMultipliers => {\n  return (matrix, factor) => getCSSMatrix(matrix, scaleMultipliers(factor), 'translate(-50%,-50%)');\n})(f => [1 / f, 1 / f, 1 / f, 1, -1 / f, -1 / f, -1 / f, -1, 1 / f, 1 / f, 1 / f, 1, 1, 1, 1, 1]);\n\nfunction isRefObject(ref) {\n  return ref && typeof ref === 'object' && 'current' in ref;\n}\n\nconst Html = /*#__PURE__*/React.forwardRef(({\n  children,\n  eps = 0.001,\n  style,\n  className,\n  prepend,\n  center,\n  fullscreen,\n  portal,\n  distanceFactor,\n  sprite = false,\n  transform = false,\n  occlude,\n  onOcclude,\n  castShadow,\n  receiveShadow,\n  material,\n  geometry,\n  zIndexRange = [16777271, 0],\n  calculatePosition = defaultCalculatePosition,\n  as = 'div',\n  wrapperClass,\n  pointerEvents = 'auto',\n  ...props\n}, ref) => {\n  const {\n    gl,\n    camera,\n    scene,\n    size,\n    raycaster,\n    events,\n    viewport\n  } = useThree();\n  const [el] = React.useState(() => document.createElement(as));\n  const root = React.useRef();\n  const group = React.useRef(null);\n  const oldZoom = React.useRef(0);\n  const oldPosition = React.useRef([0, 0]);\n  const transformOuterRef = React.useRef(null);\n  const transformInnerRef = React.useRef(null); // Append to the connected element, which makes HTML work with views\n\n  const target = (portal == null ? void 0 : portal.current) || events.connected || gl.domElement.parentNode;\n  const occlusionMeshRef = React.useRef(null);\n  const isMeshSizeSet = React.useRef(false);\n  const isRayCastOcclusion = React.useMemo(() => {\n    return occlude && occlude !== 'blending' || Array.isArray(occlude) && occlude.length && isRefObject(occlude[0]);\n  }, [occlude]);\n  React.useLayoutEffect(() => {\n    const el = gl.domElement;\n\n    if (occlude && occlude === 'blending') {\n      el.style.zIndex = `${Math.floor(zIndexRange[0] / 2)}`;\n      el.style.position = 'absolute';\n      el.style.pointerEvents = 'none';\n    } else {\n      el.style.zIndex = null;\n      el.style.position = null;\n      el.style.pointerEvents = null;\n    }\n  }, [occlude]);\n  React.useLayoutEffect(() => {\n    if (group.current) {\n      const currentRoot = root.current = ReactDOM.createRoot(el);\n      scene.updateMatrixWorld();\n\n      if (transform) {\n        el.style.cssText = `position:absolute;top:0;left:0;pointer-events:none;overflow:hidden;`;\n      } else {\n        const vec = calculatePosition(group.current, camera, size);\n        el.style.cssText = `position:absolute;top:0;left:0;transform:translate3d(${vec[0]}px,${vec[1]}px,0);transform-origin:0 0;`;\n      }\n\n      if (target) {\n        if (prepend) target.prepend(el);else target.appendChild(el);\n      }\n\n      return () => {\n        if (target) target.removeChild(el);\n        currentRoot.unmount();\n      };\n    }\n  }, [target, transform]);\n  React.useLayoutEffect(() => {\n    if (wrapperClass) el.className = wrapperClass;\n  }, [wrapperClass]);\n  const styles = React.useMemo(() => {\n    if (transform) {\n      return {\n        position: 'absolute',\n        top: 0,\n        left: 0,\n        width: size.width,\n        height: size.height,\n        transformStyle: 'preserve-3d',\n        pointerEvents: 'none'\n      };\n    } else {\n      return {\n        position: 'absolute',\n        transform: center ? 'translate3d(-50%,-50%,0)' : 'none',\n        ...(fullscreen && {\n          top: -size.height / 2,\n          left: -size.width / 2,\n          width: size.width,\n          height: size.height\n        }),\n        ...style\n      };\n    }\n  }, [style, center, fullscreen, size, transform]);\n  const transformInnerStyles = React.useMemo(() => ({\n    position: 'absolute',\n    pointerEvents\n  }), [pointerEvents]);\n  React.useLayoutEffect(() => {\n    isMeshSizeSet.current = false;\n\n    if (transform) {\n      var _root$current;\n\n      (_root$current = root.current) == null ? void 0 : _root$current.render( /*#__PURE__*/React.createElement(\"div\", {\n        ref: transformOuterRef,\n        style: styles\n      }, /*#__PURE__*/React.createElement(\"div\", {\n        ref: transformInnerRef,\n        style: transformInnerStyles\n      }, /*#__PURE__*/React.createElement(\"div\", {\n        ref: ref,\n        className: className,\n        style: style,\n        children: children\n      }))));\n    } else {\n      var _root$current2;\n\n      (_root$current2 = root.current) == null ? void 0 : _root$current2.render( /*#__PURE__*/React.createElement(\"div\", {\n        ref: ref,\n        style: styles,\n        className: className,\n        children: children\n      }));\n    }\n  });\n  const visible = React.useRef(true);\n  useFrame(gl => {\n    if (group.current) {\n      camera.updateMatrixWorld();\n      group.current.updateWorldMatrix(true, false);\n      const vec = transform ? oldPosition.current : calculatePosition(group.current, camera, size);\n\n      if (transform || Math.abs(oldZoom.current - camera.zoom) > eps || Math.abs(oldPosition.current[0] - vec[0]) > eps || Math.abs(oldPosition.current[1] - vec[1]) > eps) {\n        const isBehindCamera = isObjectBehindCamera(group.current, camera);\n        let raytraceTarget = false;\n\n        if (isRayCastOcclusion) {\n          if (occlude !== 'blending') {\n            raytraceTarget = [scene];\n          } else if (Array.isArray(occlude)) {\n            raytraceTarget = occlude.map(item => item.current);\n          }\n        }\n\n        const previouslyVisible = visible.current;\n\n        if (raytraceTarget) {\n          const isvisible = isObjectVisible(group.current, camera, raycaster, raytraceTarget);\n          visible.current = isvisible && !isBehindCamera;\n        } else {\n          visible.current = !isBehindCamera;\n        }\n\n        if (previouslyVisible !== visible.current) {\n          if (onOcclude) onOcclude(!visible.current);else el.style.display = visible.current ? 'block' : 'none';\n        }\n\n        const halfRange = Math.floor(zIndexRange[0] / 2);\n        const zRange = occlude ? isRayCastOcclusion //\n        ? [zIndexRange[0], halfRange] : [halfRange - 1, 0] : zIndexRange;\n        el.style.zIndex = `${objectZIndex(group.current, camera, zRange)}`;\n\n        if (transform) {\n          const [widthHalf, heightHalf] = [size.width / 2, size.height / 2];\n          const fov = camera.projectionMatrix.elements[5] * heightHalf;\n          const {\n            isOrthographicCamera,\n            top,\n            left,\n            bottom,\n            right\n          } = camera;\n          const cameraMatrix = getCameraCSSMatrix(camera.matrixWorldInverse);\n          const cameraTransform = isOrthographicCamera ? `scale(${fov})translate(${epsilon(-(right + left) / 2)}px,${epsilon((top + bottom) / 2)}px)` : `translateZ(${fov}px)`;\n          let matrix = group.current.matrixWorld;\n\n          if (sprite) {\n            matrix = camera.matrixWorldInverse.clone().transpose().copyPosition(matrix).scale(group.current.scale);\n            matrix.elements[3] = matrix.elements[7] = matrix.elements[11] = 0;\n            matrix.elements[15] = 1;\n          }\n\n          el.style.width = size.width + 'px';\n          el.style.height = size.height + 'px';\n          el.style.perspective = isOrthographicCamera ? '' : `${fov}px`;\n\n          if (transformOuterRef.current && transformInnerRef.current) {\n            transformOuterRef.current.style.transform = `${cameraTransform}${cameraMatrix}translate(${widthHalf}px,${heightHalf}px)`;\n            transformInnerRef.current.style.transform = getObjectCSSMatrix(matrix, 1 / ((distanceFactor || 10) / 400));\n          }\n        } else {\n          const scale = distanceFactor === undefined ? 1 : objectScale(group.current, camera) * distanceFactor;\n          el.style.transform = `translate3d(${vec[0]}px,${vec[1]}px,0) scale(${scale})`;\n        }\n\n        oldPosition.current = vec;\n        oldZoom.current = camera.zoom;\n      }\n    }\n\n    if (!isRayCastOcclusion && occlusionMeshRef.current && !isMeshSizeSet.current) {\n      if (transform) {\n        if (transformOuterRef.current) {\n          const el = transformOuterRef.current.children[0];\n\n          if (el != null && el.clientWidth && el != null && el.clientHeight) {\n            const {\n              isOrthographicCamera\n            } = camera;\n\n            if (isOrthographicCamera || geometry) {\n              if (props.scale) {\n                if (!Array.isArray(props.scale)) {\n                  occlusionMeshRef.current.scale.setScalar(1 / props.scale);\n                } else if (props.scale instanceof Vector3) {\n                  occlusionMeshRef.current.scale.copy(props.scale.clone().divideScalar(1));\n                } else {\n                  occlusionMeshRef.current.scale.set(1 / props.scale[0], 1 / props.scale[1], 1 / props.scale[2]);\n                }\n              }\n            } else {\n              const ratio = (distanceFactor || 10) / 400;\n              const w = el.clientWidth * ratio;\n              const h = el.clientHeight * ratio;\n              occlusionMeshRef.current.scale.set(w, h, 1);\n            }\n\n            isMeshSizeSet.current = true;\n          }\n        }\n      } else {\n        const ele = el.children[0];\n\n        if (ele != null && ele.clientWidth && ele != null && ele.clientHeight) {\n          const ratio = 1 / viewport.factor;\n          const w = ele.clientWidth * ratio;\n          const h = ele.clientHeight * ratio;\n          occlusionMeshRef.current.scale.set(w, h, 1);\n          isMeshSizeSet.current = true;\n        }\n\n        occlusionMeshRef.current.lookAt(gl.camera.position);\n      }\n    }\n  });\n  const shaders = React.useMemo(() => ({\n    vertexShader: !transform ?\n    /* glsl */\n    `\n          /*\n            This shader is from the THREE's SpriteMaterial.\n            We need to turn the backing plane into a Sprite\n            (make it always face the camera) if \"transfrom\" \n            is false. \n          */\n          #include <common>\n\n          void main() {\n            vec2 center = vec2(0., 1.);\n            float rotation = 0.0;\n            \n            // This is somewhat arbitrary, but it seems to work well\n            // Need to figure out how to derive this dynamically if it even matters\n            float size = 0.03;\n\n            vec4 mvPosition = modelViewMatrix * vec4( 0.0, 0.0, 0.0, 1.0 );\n            vec2 scale;\n            scale.x = length( vec3( modelMatrix[ 0 ].x, modelMatrix[ 0 ].y, modelMatrix[ 0 ].z ) );\n            scale.y = length( vec3( modelMatrix[ 1 ].x, modelMatrix[ 1 ].y, modelMatrix[ 1 ].z ) );\n\n            bool isPerspective = isPerspectiveMatrix( projectionMatrix );\n            if ( isPerspective ) scale *= - mvPosition.z;\n\n            vec2 alignedPosition = ( position.xy - ( center - vec2( 0.5 ) ) ) * scale * size;\n            vec2 rotatedPosition;\n            rotatedPosition.x = cos( rotation ) * alignedPosition.x - sin( rotation ) * alignedPosition.y;\n            rotatedPosition.y = sin( rotation ) * alignedPosition.x + cos( rotation ) * alignedPosition.y;\n            mvPosition.xy += rotatedPosition;\n\n            gl_Position = projectionMatrix * mvPosition;\n          }\n      ` : undefined,\n    fragmentShader:\n    /* glsl */\n    `\n        void main() {\n          gl_FragColor = vec4(0.0, 0.0, 0.0, 0.0);\n        }\n      `\n  }), [transform]);\n  return /*#__PURE__*/React.createElement(\"group\", _extends({}, props, {\n    ref: group\n  }), occlude && !isRayCastOcclusion && /*#__PURE__*/React.createElement(\"mesh\", {\n    castShadow: castShadow,\n    receiveShadow: receiveShadow,\n    ref: occlusionMeshRef\n  }, geometry || /*#__PURE__*/React.createElement(\"planeGeometry\", null), material || /*#__PURE__*/React.createElement(\"shaderMaterial\", {\n    side: DoubleSide,\n    vertexShader: shaders.vertexShader,\n    fragmentShader: shaders.fragmentShader\n  })));\n});\n\nexport { Html };\n",
         "import * as React from 'react';\n\nconst context = /*#__PURE__*/React.createContext(null);\n\nexport { context };\n",
         "import * as React from 'react';\nimport * as THREE from 'three';\nimport { useThree } from '@react-three/fiber';\nimport { Line } from '../../core/Line.js';\nimport { Html } from '../Html.js';\nimport { context } from './context.js';\n\nconst vec1 = new THREE.Vector3();\nconst vec2 = new THREE.Vector3();\nconst calculateOffset = (clickPoint, normal, rayStart, rayDir) => {\n  const e1 = normal.dot(normal);\n  const e2 = normal.dot(clickPoint) - normal.dot(rayStart);\n  const e3 = normal.dot(rayDir);\n\n  if (e3 === 0) {\n    return -e2 / e1;\n  }\n\n  vec1.copy(rayDir).multiplyScalar(e1 / e3).sub(normal);\n  vec2.copy(rayDir).multiplyScalar(e2 / e3).add(rayStart).sub(clickPoint);\n  const offset = -vec1.dot(vec2) / vec1.dot(vec1);\n  return offset;\n};\nconst upV = new THREE.Vector3(0, 1, 0);\nconst offsetMatrix = new THREE.Matrix4();\nconst AxisArrow = ({\n  direction,\n  axis\n}) => {\n  const {\n    translation,\n    translationLimits,\n    annotations,\n    annotationsClass,\n    depthTest,\n    scale,\n    lineWidth,\n    fixed,\n    axisColors,\n    hoveredColor,\n    opacity,\n    onDragStart,\n    onDrag,\n    onDragEnd,\n    userData\n  } = React.useContext(context); // @ts-expect-error new in @react-three/fiber@7.0.5\n\n  const camControls = useThree(state => state.controls);\n  const divRef = React.useRef(null);\n  const objRef = React.useRef(null);\n  const clickInfo = React.useRef(null);\n  const offset0 = React.useRef(0);\n  const [isHovered, setIsHovered] = React.useState(false);\n  const onPointerDown = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.innerText = `${translation.current[axis].toFixed(2)}`;\n      divRef.current.style.display = 'block';\n    }\n\n    e.stopPropagation();\n    const rotation = new THREE.Matrix4().extractRotation(objRef.current.matrixWorld);\n    const clickPoint = e.point.clone();\n    const origin = new THREE.Vector3().setFromMatrixPosition(objRef.current.matrixWorld);\n    const dir = direction.clone().applyMatrix4(rotation).normalize();\n    clickInfo.current = {\n      clickPoint,\n      dir\n    };\n    offset0.current = translation.current[axis];\n    onDragStart({\n      component: 'Arrow',\n      axis,\n      origin,\n      directions: [dir]\n    });\n    camControls && (camControls.enabled = false); // @ts-ignore - setPointerCapture is not in the type definition\n\n    e.target.setPointerCapture(e.pointerId);\n  }, [annotations, direction, camControls, onDragStart, translation, axis]);\n  const onPointerMove = React.useCallback(e => {\n    e.stopPropagation();\n    if (!isHovered) setIsHovered(true);\n\n    if (clickInfo.current) {\n      const {\n        clickPoint,\n        dir\n      } = clickInfo.current;\n      const [min, max] = (translationLimits == null ? void 0 : translationLimits[axis]) || [undefined, undefined];\n      let offset = calculateOffset(clickPoint, dir, e.ray.origin, e.ray.direction);\n\n      if (min !== undefined) {\n        offset = Math.max(offset, min - offset0.current);\n      }\n\n      if (max !== undefined) {\n        offset = Math.min(offset, max - offset0.current);\n      }\n\n      translation.current[axis] = offset0.current + offset;\n\n      if (annotations) {\n        divRef.current.innerText = `${translation.current[axis].toFixed(2)}`;\n      }\n\n      offsetMatrix.makeTranslation(dir.x * offset, dir.y * offset, dir.z * offset);\n      onDrag(offsetMatrix);\n    }\n  }, [annotations, onDrag, isHovered, translation, translationLimits, axis]);\n  const onPointerUp = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.style.display = 'none';\n    }\n\n    e.stopPropagation();\n    clickInfo.current = null;\n    onDragEnd();\n    camControls && (camControls.enabled = true); // @ts-ignore - releasePointerCapture & PointerEvent#pointerId is not in the type definition\n\n    e.target.releasePointerCapture(e.pointerId);\n  }, [annotations, camControls, onDragEnd]);\n  const onPointerOut = React.useCallback(e => {\n    e.stopPropagation();\n    setIsHovered(false);\n  }, []);\n  const {\n    cylinderLength,\n    coneWidth,\n    coneLength,\n    matrixL\n  } = React.useMemo(() => {\n    const coneWidth = fixed ? lineWidth / scale * 1.6 : scale / 20;\n    const coneLength = fixed ? 0.2 : scale / 5;\n    const cylinderLength = fixed ? 1 - coneLength : scale - coneLength;\n    const quaternion = new THREE.Quaternion().setFromUnitVectors(upV, direction.clone().normalize());\n    const matrixL = new THREE.Matrix4().makeRotationFromQuaternion(quaternion);\n    return {\n      cylinderLength,\n      coneWidth,\n      coneLength,\n      matrixL\n    };\n  }, [direction, scale, lineWidth, fixed]);\n  const color_ = isHovered ? hoveredColor : axisColors[axis];\n  return /*#__PURE__*/React.createElement(\"group\", {\n    ref: objRef\n  }, /*#__PURE__*/React.createElement(\"group\", {\n    matrix: matrixL,\n    matrixAutoUpdate: false,\n    onPointerDown: onPointerDown,\n    onPointerMove: onPointerMove,\n    onPointerUp: onPointerUp,\n    onPointerOut: onPointerOut\n  }, annotations && /*#__PURE__*/React.createElement(Html, {\n    position: [0, -coneLength, 0]\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    style: {\n      display: 'none',\n      background: '#151520',\n      color: 'white',\n      padding: '6px 8px',\n      borderRadius: 7,\n      whiteSpace: 'nowrap'\n    },\n    className: annotationsClass,\n    ref: divRef\n  })), /*#__PURE__*/React.createElement(\"mesh\", {\n    visible: false,\n    position: [0, (cylinderLength + coneLength) / 2.0, 0],\n    userData: userData\n  }, /*#__PURE__*/React.createElement(\"cylinderGeometry\", {\n    args: [coneWidth * 1.4, coneWidth * 1.4, cylinderLength + coneLength, 8, 1]\n  })), /*#__PURE__*/React.createElement(Line, {\n    transparent: true,\n    raycast: () => null,\n    depthTest: depthTest,\n    points: [0, 0, 0, 0, cylinderLength, 0],\n    lineWidth: lineWidth,\n    color: color_,\n    opacity: opacity,\n    polygonOffset: true,\n    renderOrder: 1,\n    polygonOffsetFactor: -10\n  }), /*#__PURE__*/React.createElement(\"mesh\", {\n    raycast: () => null,\n    position: [0, cylinderLength + coneLength / 2.0, 0],\n    renderOrder: 500\n  }, /*#__PURE__*/React.createElement(\"coneGeometry\", {\n    args: [coneWidth, coneLength, 24, 1]\n  }), /*#__PURE__*/React.createElement(\"meshBasicMaterial\", {\n    transparent: true,\n    depthTest: depthTest,\n    color: color_,\n    opacity: opacity,\n    polygonOffset: true,\n    polygonOffsetFactor: -10\n  }))));\n};\n\nexport { AxisArrow, calculateOffset };\n",
         "import * as React from 'react';\nimport * as THREE from 'three';\nimport { useThree } from '@react-three/fiber';\nimport { Line } from '../../core/Line.js';\nimport { Html } from '../Html.js';\nimport { context } from './context.js';\n\nconst decomposeIntoBasis = (e1, e2, offset) => {\n  const i1 = Math.abs(e1.x) >= Math.abs(e1.y) && Math.abs(e1.x) >= Math.abs(e1.z) ? 0 : Math.abs(e1.y) >= Math.abs(e1.x) && Math.abs(e1.y) >= Math.abs(e1.z) ? 1 : 2;\n  const e2DegrowthOrder = [0, 1, 2].sort((a, b) => Math.abs(e2.getComponent(b)) - Math.abs(e2.getComponent(a)));\n  const i2 = i1 === e2DegrowthOrder[0] ? e2DegrowthOrder[1] : e2DegrowthOrder[0];\n  const a1 = e1.getComponent(i1);\n  const a2 = e1.getComponent(i2);\n  const b1 = e2.getComponent(i1);\n  const b2 = e2.getComponent(i2);\n  const c1 = offset.getComponent(i1);\n  const c2 = offset.getComponent(i2);\n  const y = (c2 - c1 * (a2 / a1)) / (b2 - b1 * (a2 / a1));\n  const x = (c1 - y * b1) / a1;\n  return [x, y];\n};\n\nconst ray = new THREE.Ray();\nconst intersection = new THREE.Vector3();\nconst offsetMatrix = new THREE.Matrix4();\nconst PlaneSlider = ({\n  dir1,\n  dir2,\n  axis\n}) => {\n  const {\n    translation,\n    translationLimits,\n    annotations,\n    annotationsClass,\n    depthTest,\n    scale,\n    lineWidth,\n    fixed,\n    axisColors,\n    hoveredColor,\n    opacity,\n    onDragStart,\n    onDrag,\n    onDragEnd,\n    userData\n  } = React.useContext(context); // @ts-expect-error new in @react-three/fiber@7.0.5\n\n  const camControls = useThree(state => state.controls);\n  const divRef = React.useRef(null);\n  const objRef = React.useRef(null);\n  const clickInfo = React.useRef(null);\n  const offsetX0 = React.useRef(0);\n  const offsetY0 = React.useRef(0);\n  const [isHovered, setIsHovered] = React.useState(false);\n  const onPointerDown = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.innerText = `${translation.current[(axis + 1) % 3].toFixed(2)}, ${translation.current[(axis + 2) % 3].toFixed(2)}`;\n      divRef.current.style.display = 'block';\n    }\n\n    e.stopPropagation();\n    const clickPoint = e.point.clone();\n    const origin = new THREE.Vector3().setFromMatrixPosition(objRef.current.matrixWorld);\n    const e1 = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 0).normalize();\n    const e2 = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 1).normalize();\n    const normal = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 2).normalize();\n    const plane = new THREE.Plane().setFromNormalAndCoplanarPoint(normal, origin);\n    clickInfo.current = {\n      clickPoint,\n      e1,\n      e2,\n      plane\n    };\n    offsetX0.current = translation.current[(axis + 1) % 3];\n    offsetY0.current = translation.current[(axis + 2) % 3];\n    onDragStart({\n      component: 'Slider',\n      axis,\n      origin,\n      directions: [e1, e2, normal]\n    });\n    camControls && (camControls.enabled = false); // @ts-ignore\n\n    e.target.setPointerCapture(e.pointerId);\n  }, [annotations, camControls, onDragStart, axis]);\n  const onPointerMove = React.useCallback(e => {\n    e.stopPropagation();\n    if (!isHovered) setIsHovered(true);\n\n    if (clickInfo.current) {\n      const {\n        clickPoint,\n        e1,\n        e2,\n        plane\n      } = clickInfo.current;\n      const [minX, maxX] = (translationLimits == null ? void 0 : translationLimits[(axis + 1) % 3]) || [undefined, undefined];\n      const [minY, maxY] = (translationLimits == null ? void 0 : translationLimits[(axis + 2) % 3]) || [undefined, undefined];\n      ray.copy(e.ray);\n      ray.intersectPlane(plane, intersection);\n      ray.direction.negate();\n      ray.intersectPlane(plane, intersection);\n      intersection.sub(clickPoint);\n      let [offsetX, offsetY] = decomposeIntoBasis(e1, e2, intersection);\n      /* let offsetY = (intersection.y - (intersection.x * e1.y) / e1.x) / (e2.y - (e2.x * e1.y) / e1.x)\n      let offsetX = (intersection.x - offsetY * e2.x) / e1.x */\n\n      if (minX !== undefined) {\n        offsetX = Math.max(offsetX, minX - offsetX0.current);\n      }\n\n      if (maxX !== undefined) {\n        offsetX = Math.min(offsetX, maxX - offsetX0.current);\n      }\n\n      if (minY !== undefined) {\n        offsetY = Math.max(offsetY, minY - offsetY0.current);\n      }\n\n      if (maxY !== undefined) {\n        offsetY = Math.min(offsetY, maxY - offsetY0.current);\n      }\n\n      translation.current[(axis + 1) % 3] = offsetX0.current + offsetX;\n      translation.current[(axis + 2) % 3] = offsetY0.current + offsetY;\n\n      if (annotations) {\n        divRef.current.innerText = `${translation.current[(axis + 1) % 3].toFixed(2)}, ${translation.current[(axis + 2) % 3].toFixed(2)}`;\n      }\n\n      offsetMatrix.makeTranslation(offsetX * e1.x + offsetY * e2.x, offsetX * e1.y + offsetY * e2.y, offsetX * e1.z + offsetY * e2.z);\n      onDrag(offsetMatrix);\n    }\n  }, [annotations, onDrag, isHovered, translation, translationLimits, axis]);\n  const onPointerUp = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.style.display = 'none';\n    }\n\n    e.stopPropagation();\n    clickInfo.current = null;\n    onDragEnd();\n    camControls && (camControls.enabled = true); // @ts-ignore\n\n    e.target.releasePointerCapture(e.pointerId);\n  }, [annotations, camControls, onDragEnd]);\n  const onPointerOut = React.useCallback(e => {\n    e.stopPropagation();\n    setIsHovered(false);\n  }, []);\n  const matrixL = React.useMemo(() => {\n    const dir1N = dir1.clone().normalize();\n    const dir2N = dir2.clone().normalize();\n    return new THREE.Matrix4().makeBasis(dir1N, dir2N, dir1N.clone().cross(dir2N));\n  }, [dir1, dir2]);\n  const pos1 = fixed ? 1 / 7 : scale / 7;\n  const length = fixed ? 0.225 : scale * 0.225;\n  const color = isHovered ? hoveredColor : axisColors[axis];\n  const points = React.useMemo(() => [new THREE.Vector3(0, 0, 0), new THREE.Vector3(0, length, 0), new THREE.Vector3(length, length, 0), new THREE.Vector3(length, 0, 0), new THREE.Vector3(0, 0, 0)], [length]);\n  return /*#__PURE__*/React.createElement(\"group\", {\n    ref: objRef,\n    matrix: matrixL,\n    matrixAutoUpdate: false\n  }, annotations && /*#__PURE__*/React.createElement(Html, {\n    position: [0, 0, 0]\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    style: {\n      display: 'none',\n      background: '#151520',\n      color: 'white',\n      padding: '6px 8px',\n      borderRadius: 7,\n      whiteSpace: 'nowrap'\n    },\n    className: annotationsClass,\n    ref: divRef\n  })), /*#__PURE__*/React.createElement(\"group\", {\n    position: [pos1 * 1.7, pos1 * 1.7, 0]\n  }, /*#__PURE__*/React.createElement(\"mesh\", {\n    visible: true,\n    onPointerDown: onPointerDown,\n    onPointerMove: onPointerMove,\n    onPointerUp: onPointerUp,\n    onPointerOut: onPointerOut,\n    scale: length,\n    userData: userData\n  }, /*#__PURE__*/React.createElement(\"planeGeometry\", null), /*#__PURE__*/React.createElement(\"meshBasicMaterial\", {\n    transparent: true,\n    depthTest: depthTest,\n    color: color,\n    polygonOffset: true,\n    polygonOffsetFactor: -10,\n    side: THREE.DoubleSide\n  })), /*#__PURE__*/React.createElement(Line, {\n    position: [-length / 2, -length / 2, 0],\n    transparent: true,\n    depthTest: depthTest,\n    points: points,\n    lineWidth: lineWidth,\n    color: color,\n    opacity: opacity,\n    polygonOffset: true,\n    polygonOffsetFactor: -10,\n    userData: userData\n  })));\n};\n\nexport { PlaneSlider };\n",
         "import * as React from 'react';\nimport * as THREE from 'three';\nimport { useThree } from '@react-three/fiber';\nimport { Line } from '../../core/Line.js';\nimport { Html } from '../Html.js';\nimport clamp from 'lodash.clamp';\nimport { context } from './context.js';\n\nconst clickDir = new THREE.Vector3();\nconst intersectionDir = new THREE.Vector3();\n\nconst toDegrees = radians => radians * 180 / Math.PI;\n\nconst toRadians = degrees => degrees * Math.PI / 180;\n\nconst calculateAngle = (clickPoint, intersectionPoint, origin, e1, e2) => {\n  clickDir.copy(clickPoint).sub(origin);\n  intersectionDir.copy(intersectionPoint).sub(origin);\n  const dote1e1 = e1.dot(e1);\n  const dote2e2 = e2.dot(e2);\n  const uClick = clickDir.dot(e1) / dote1e1;\n  const vClick = clickDir.dot(e2) / dote2e2;\n  const uIntersection = intersectionDir.dot(e1) / dote1e1;\n  const vIntersection = intersectionDir.dot(e2) / dote2e2;\n  const angleClick = Math.atan2(vClick, uClick);\n  const angleIntersection = Math.atan2(vIntersection, uIntersection);\n  return angleIntersection - angleClick;\n};\n\nconst fmod = (num, denom) => {\n  let k = Math.floor(num / denom);\n  k = k < 0 ? k + 1 : k;\n  return num - k * denom;\n};\n\nconst minimizeAngle = angle => {\n  let result = fmod(angle, 2 * Math.PI);\n\n  if (Math.abs(result) < 1e-6) {\n    return 0.0;\n  }\n\n  if (result < 0.0) {\n    result += 2 * Math.PI;\n  }\n\n  return result;\n};\n\nconst rotMatrix = new THREE.Matrix4();\nconst posNew = new THREE.Vector3();\nconst ray = new THREE.Ray();\nconst intersection = new THREE.Vector3();\nconst AxisRotator = ({\n  dir1,\n  dir2,\n  axis\n}) => {\n  const {\n    rotationLimits,\n    annotations,\n    annotationsClass,\n    depthTest,\n    scale,\n    lineWidth,\n    fixed,\n    axisColors,\n    hoveredColor,\n    opacity,\n    onDragStart,\n    onDrag,\n    onDragEnd,\n    userData\n  } = React.useContext(context); // @ts-expect-error new in @react-three/fiber@7.0.5\n\n  const camControls = useThree(state => state.controls);\n  const divRef = React.useRef(null);\n  const objRef = React.useRef(null);\n  const angle0 = React.useRef(0);\n  const angle = React.useRef(0);\n  const clickInfo = React.useRef(null);\n  const [isHovered, setIsHovered] = React.useState(false);\n  const onPointerDown = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.innerText = `${toDegrees(angle.current).toFixed(0)}\u00ba`;\n      divRef.current.style.display = 'block';\n    }\n\n    e.stopPropagation();\n    const clickPoint = e.point.clone();\n    const origin = new THREE.Vector3().setFromMatrixPosition(objRef.current.matrixWorld);\n    const e1 = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 0).normalize();\n    const e2 = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 1).normalize();\n    const normal = new THREE.Vector3().setFromMatrixColumn(objRef.current.matrixWorld, 2).normalize();\n    const plane = new THREE.Plane().setFromNormalAndCoplanarPoint(normal, origin);\n    clickInfo.current = {\n      clickPoint,\n      origin,\n      e1,\n      e2,\n      normal,\n      plane\n    };\n    onDragStart({\n      component: 'Rotator',\n      axis,\n      origin,\n      directions: [e1, e2, normal]\n    });\n    camControls && (camControls.enabled = false); // @ts-ignore\n\n    e.target.setPointerCapture(e.pointerId);\n  }, [annotations, camControls, onDragStart, axis]);\n  const onPointerMove = React.useCallback(e => {\n    e.stopPropagation();\n    if (!isHovered) setIsHovered(true);\n\n    if (clickInfo.current) {\n      const {\n        clickPoint,\n        origin,\n        e1,\n        e2,\n        normal,\n        plane\n      } = clickInfo.current;\n      const [min, max] = (rotationLimits == null ? void 0 : rotationLimits[axis]) || [undefined, undefined];\n      ray.copy(e.ray);\n      ray.intersectPlane(plane, intersection);\n      ray.direction.negate();\n      ray.intersectPlane(plane, intersection);\n      let deltaAngle = calculateAngle(clickPoint, intersection, origin, e1, e2);\n      let degrees = toDegrees(deltaAngle); // @ts-ignore\n\n      if (e.shiftKey) {\n        degrees = Math.round(degrees / 10) * 10;\n        deltaAngle = toRadians(degrees);\n      }\n\n      if (min !== undefined && max !== undefined && max - min < 2 * Math.PI) {\n        deltaAngle = minimizeAngle(deltaAngle);\n        deltaAngle = deltaAngle > Math.PI ? deltaAngle - 2 * Math.PI : deltaAngle;\n        deltaAngle = clamp(deltaAngle, min - angle0.current, max - angle0.current);\n        angle.current = angle0.current + deltaAngle;\n      } else {\n        angle.current = minimizeAngle(angle0.current + deltaAngle);\n        angle.current = angle.current > Math.PI ? angle.current - 2 * Math.PI : angle.current;\n      }\n\n      if (annotations) {\n        degrees = toDegrees(angle.current);\n        divRef.current.innerText = `${degrees.toFixed(0)}\u00ba`;\n      }\n\n      rotMatrix.makeRotationAxis(normal, deltaAngle);\n      posNew.copy(origin).applyMatrix4(rotMatrix).sub(origin).negate();\n      rotMatrix.setPosition(posNew);\n      onDrag(rotMatrix);\n    }\n  }, [annotations, onDrag, isHovered, rotationLimits, axis]);\n  const onPointerUp = React.useCallback(e => {\n    if (annotations) {\n      divRef.current.style.display = 'none';\n    }\n\n    e.stopPropagation();\n    angle0.current = angle.current;\n    clickInfo.current = null;\n    onDragEnd();\n    camControls && (camControls.enabled = true); // @ts-ignore\n\n    e.target.releasePointerCapture(e.pointerId);\n  }, [annotations, camControls, onDragEnd]);\n  const onPointerOut = React.useCallback(e => {\n    e.stopPropagation();\n    setIsHovered(false);\n  }, []);\n  const matrixL = React.useMemo(() => {\n    const dir1N = dir1.clone().normalize();\n    const dir2N = dir2.clone().normalize();\n    return new THREE.Matrix4().makeBasis(dir1N, dir2N, dir1N.clone().cross(dir2N));\n  }, [dir1, dir2]);\n  const r = fixed ? 0.65 : scale * 0.65;\n  const arc = React.useMemo(() => {\n    const segments = 32;\n    const points = [];\n\n    for (let j = 0; j <= segments; j++) {\n      const angle = j * (Math.PI / 2) / segments;\n      points.push(new THREE.Vector3(Math.cos(angle) * r, Math.sin(angle) * r, 0));\n    }\n\n    return points;\n  }, [r]);\n  return /*#__PURE__*/React.createElement(\"group\", {\n    ref: objRef,\n    onPointerDown: onPointerDown,\n    onPointerMove: onPointerMove,\n    onPointerUp: onPointerUp,\n    onPointerOut: onPointerOut,\n    matrix: matrixL,\n    matrixAutoUpdate: false\n  }, annotations && /*#__PURE__*/React.createElement(Html, {\n    position: [r, r, 0]\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    style: {\n      display: 'none',\n      background: '#151520',\n      color: 'white',\n      padding: '6px 8px',\n      borderRadius: 7,\n      whiteSpace: 'nowrap'\n    },\n    className: annotationsClass,\n    ref: divRef\n  })), /*#__PURE__*/React.createElement(Line, {\n    points: arc,\n    lineWidth: lineWidth * 4,\n    visible: false,\n    userData: userData\n  }), /*#__PURE__*/React.createElement(Line, {\n    transparent: true,\n    raycast: () => null,\n    depthTest: depthTest,\n    points: arc,\n    lineWidth: lineWidth,\n    color: isHovered ? hoveredColor : axisColors[axis],\n    opacity: opacity,\n    polygonOffset: true,\n    polygonOffsetFactor: -10\n  }));\n};\n\nexport { AxisRotator };\n",
         "import _extends from '@babel/runtime/helpers/esm/extends';\nimport * as THREE from 'three';\nimport * as React from 'react';\nimport { useThree, useFrame } from '@react-three/fiber';\nimport { AxisArrow } from './AxisArrow.js';\nimport { PlaneSlider } from './PlaneSlider.js';\nimport { AxisRotator } from './AxisRotator.js';\nimport { context } from './context.js';\n\nconst tV0 = new THREE.Vector3();\nconst tV1 = new THREE.Vector3();\nconst tV2 = new THREE.Vector3();\n\nconst getPoint2 = (point3, camera, size) => {\n  const widthHalf = size.width / 2;\n  const heightHalf = size.height / 2;\n  camera.updateMatrixWorld(false);\n  const vector = point3.project(camera);\n  vector.x = vector.x * widthHalf + widthHalf;\n  vector.y = -(vector.y * heightHalf) + heightHalf;\n  return vector;\n};\n\nconst getPoint3 = (point2, camera, size, zValue = 1) => {\n  const vector = tV0.set(point2.x / size.width * 2 - 1, -(point2.y / size.height) * 2 + 1, zValue);\n  vector.unproject(camera);\n  return vector;\n};\n\nconst calculateScaleFactor = (point3, radiusPx, camera, size) => {\n  const point2 = getPoint2(tV2.copy(point3), camera, size);\n  let scale = 0;\n\n  for (let i = 0; i < 2; ++i) {\n    const point2off = tV1.copy(point2).setComponent(i, point2.getComponent(i) + radiusPx);\n    const point3off = getPoint3(point2off, camera, size, point2off.z);\n    scale = Math.max(scale, point3.distanceTo(point3off));\n  }\n\n  return scale;\n};\nconst mL0 = new THREE.Matrix4();\nconst mW0 = new THREE.Matrix4();\nconst mP = new THREE.Matrix4();\nconst mPInv = new THREE.Matrix4();\nconst mW = new THREE.Matrix4();\nconst mL = new THREE.Matrix4();\nconst mL0Inv = new THREE.Matrix4();\nconst mdL = new THREE.Matrix4();\nconst bb = new THREE.Box3();\nconst bbObj = new THREE.Box3();\nconst vCenter = new THREE.Vector3();\nconst vSize = new THREE.Vector3();\nconst vAnchorOffset = new THREE.Vector3();\nconst vPosition = new THREE.Vector3();\nconst xDir = new THREE.Vector3(1, 0, 0);\nconst yDir = new THREE.Vector3(0, 1, 0);\nconst zDir = new THREE.Vector3(0, 0, 1);\nconst PivotControls = /*#__PURE__*/React.forwardRef(({\n  matrix,\n  onDragStart,\n  onDrag,\n  onDragEnd,\n  autoTransform = true,\n  anchor,\n  disableAxes = false,\n  disableSliders = false,\n  disableRotations = false,\n  activeAxes = [true, true, true],\n  offset = [0, 0, 0],\n  rotation = [0, 0, 0],\n  scale = 1,\n  lineWidth = 4,\n  fixed = false,\n  translationLimits,\n  rotationLimits,\n  depthTest = true,\n  axisColors = ['#ff2060', '#20df80', '#2080ff'],\n  hoveredColor = '#ffff40',\n  annotations = false,\n  annotationsClass,\n  opacity = 1,\n  visible = true,\n  userData,\n  children,\n  ...props\n}, fRef) => {\n  const invalidate = useThree(state => state.invalidate);\n  const parentRef = React.useRef(null);\n  const ref = React.useRef(null);\n  const gizmoRef = React.useRef(null);\n  const childrenRef = React.useRef(null);\n  const translation = React.useRef([0, 0, 0]);\n  React.useLayoutEffect(() => {\n    if (!anchor) return;\n    childrenRef.current.updateWorldMatrix(true, true);\n    mPInv.copy(childrenRef.current.matrixWorld).invert();\n    bb.makeEmpty();\n    childrenRef.current.traverse(obj => {\n      if (!obj.geometry) return;\n      if (!obj.geometry.boundingBox) obj.geometry.computeBoundingBox();\n      mL.copy(obj.matrixWorld).premultiply(mPInv);\n      bbObj.copy(obj.geometry.boundingBox);\n      bbObj.applyMatrix4(mL);\n      bb.union(bbObj);\n    });\n    vCenter.copy(bb.max).add(bb.min).multiplyScalar(0.5);\n    vSize.copy(bb.max).sub(bb.min).multiplyScalar(0.5);\n    vAnchorOffset.copy(vSize).multiply(new THREE.Vector3(...anchor)).add(vCenter);\n    vPosition.set(...offset).add(vAnchorOffset);\n    gizmoRef.current.position.copy(vPosition);\n    invalidate();\n  });\n  const config = React.useMemo(() => ({\n    onDragStart: props => {\n      mL0.copy(ref.current.matrix);\n      mW0.copy(ref.current.matrixWorld);\n      onDragStart && onDragStart(props);\n      invalidate();\n    },\n    onDrag: mdW => {\n      mP.copy(parentRef.current.matrixWorld);\n      mPInv.copy(mP).invert(); // After applying the delta\n\n      mW.copy(mW0).premultiply(mdW);\n      mL.copy(mW).premultiply(mPInv);\n      mL0Inv.copy(mL0).invert();\n      mdL.copy(mL).multiply(mL0Inv);\n      if (autoTransform) ref.current.matrix.copy(mL);\n      onDrag && onDrag(mL, mdL, mW, mdW);\n      invalidate();\n    },\n    onDragEnd: () => {\n      if (onDragEnd) onDragEnd();\n      invalidate();\n    },\n    translation,\n    translationLimits,\n    rotationLimits,\n    axisColors,\n    hoveredColor,\n    opacity,\n    scale,\n    lineWidth,\n    fixed,\n    depthTest,\n    userData,\n    annotations,\n    annotationsClass\n  }), [onDragStart, onDrag, onDragEnd, translation, translationLimits, rotationLimits, depthTest, scale, lineWidth, fixed, ...axisColors, hoveredColor, opacity, userData, autoTransform, annotations, annotationsClass]);\n  const vec = new THREE.Vector3();\n  useFrame(state => {\n    if (fixed) {\n      const sf = calculateScaleFactor(gizmoRef.current.getWorldPosition(vec), scale, state.camera, state.size);\n\n      if (gizmoRef.current) {\n        var _gizmoRef$current, _gizmoRef$current2, _gizmoRef$current3;\n\n        if (((_gizmoRef$current = gizmoRef.current) == null ? void 0 : _gizmoRef$current.scale.x) !== sf || ((_gizmoRef$current2 = gizmoRef.current) == null ? void 0 : _gizmoRef$current2.scale.y) !== sf || ((_gizmoRef$current3 = gizmoRef.current) == null ? void 0 : _gizmoRef$current3.scale.z) !== sf) {\n          gizmoRef.current.scale.setScalar(sf);\n          state.invalidate();\n        }\n      }\n    }\n  });\n  React.useImperativeHandle(fRef, () => ref.current, []);\n  React.useLayoutEffect(() => {\n    // If the matrix is a real matrix4 it means that the user wants to control the gizmo\n    // In that case it should just be set, as a bare prop update would merely copy it\n    if (matrix && matrix instanceof THREE.Matrix4) ref.current.matrix = matrix;\n  }, [matrix]);\n  return /*#__PURE__*/React.createElement(context.Provider, {\n    value: config\n  }, /*#__PURE__*/React.createElement(\"group\", {\n    ref: parentRef\n  }, /*#__PURE__*/React.createElement(\"group\", _extends({\n    ref: ref,\n    matrix: matrix,\n    matrixAutoUpdate: false\n  }, props), /*#__PURE__*/React.createElement(\"group\", {\n    visible: visible,\n    ref: gizmoRef,\n    position: offset,\n    rotation: rotation\n  }, !disableAxes && activeAxes[0] && /*#__PURE__*/React.createElement(AxisArrow, {\n    axis: 0,\n    direction: xDir\n  }), !disableAxes && activeAxes[1] && /*#__PURE__*/React.createElement(AxisArrow, {\n    axis: 1,\n    direction: yDir\n  }), !disableAxes && activeAxes[2] && /*#__PURE__*/React.createElement(AxisArrow, {\n    axis: 2,\n    direction: zDir\n  }), !disableSliders && activeAxes[0] && activeAxes[1] && /*#__PURE__*/React.createElement(PlaneSlider, {\n    axis: 2,\n    dir1: xDir,\n    dir2: yDir\n  }), !disableSliders && activeAxes[0] && activeAxes[2] && /*#__PURE__*/React.createElement(PlaneSlider, {\n    axis: 1,\n    dir1: zDir,\n    dir2: xDir\n  }), !disableSliders && activeAxes[2] && activeAxes[1] && /*#__PURE__*/React.createElement(PlaneSlider, {\n    axis: 0,\n    dir1: yDir,\n    dir2: zDir\n  }), !disableRotations && activeAxes[0] && activeAxes[1] && /*#__PURE__*/React.createElement(AxisRotator, {\n    axis: 2,\n    dir1: xDir,\n    dir2: yDir\n  }), !disableRotations && activeAxes[0] && activeAxes[2] && /*#__PURE__*/React.createElement(AxisRotator, {\n    axis: 1,\n    dir1: zDir,\n    dir2: xDir\n  }), !disableRotations && activeAxes[2] && activeAxes[1] && /*#__PURE__*/React.createElement(AxisRotator, {\n    axis: 0,\n    dir1: yDir,\n    dir2: zDir\n  })), /*#__PURE__*/React.createElement(\"group\", {\n    ref: childrenRef\n  }, children))));\n});\n\nexport { PivotControls, calculateScaleFactor };\n",
-        "import { pack, unpack } from \"msgpackr\";\nimport React, { MutableRefObject, useContext } from \"react\";\nimport * as THREE from \"three\";\nimport AwaitLock from \"await-lock\";\nimport { TextureLoader } from \"three\";\n\nimport { SceneNode } from \"./SceneTree\";\nimport { CoordinateFrame, CameraFrustum } from \"./ThreeAssets\";\nimport { Message } from \"./WebsocketMessages\";\nimport { syncSearchParamServer } from \"./SearchParamsUtils\";\nimport { PivotControls } from \"@react-three/drei\";\nimport { ViewerContext } from \".\";\nimport { useThree } from \"@react-three/fiber\";\n\n/** Send message over websocket. */\nexport function sendWebsocketMessage(\n  websocketRef: MutableRefObject<WebSocket | null>,\n  message: Message\n) {\n  if (websocketRef.current === null) return;\n  websocketRef.current.send(pack(message));\n}\n\n/** Returns a function for sending messages, with automatic throttling. */\nexport function makeThrottledMessageSender(\n  websocketRef: MutableRefObject<WebSocket | null>,\n  throttleMilliseconds: number\n) {\n  let readyToSend = true;\n  let stale = false;\n  let latestMessage: Message | null = null;\n\n  function send(message: Message) {\n    if (websocketRef.current === null) return;\n    latestMessage = message;\n    if (readyToSend) {\n      websocketRef.current.send(pack(message));\n      stale = false;\n      readyToSend = false;\n\n      setTimeout(() => {\n        readyToSend = true;\n        if (!stale) return;\n        latestMessage && send(latestMessage);\n      }, throttleMilliseconds);\n    } else {\n      stale = true;\n    }\n  }\n  return send;\n}\n\n/** Type guard for threejs textures. Meant to be used with `scene.background`. */\nfunction isTexture(\n  background: THREE.Color | THREE.Texture | THREE.CubeTexture | null\n): background is THREE.Texture {\n  return (\n    background !== null && (background as THREE.Texture).isTexture !== undefined\n  );\n}\n\n/** Returns a handler for all incoming messages. */\nfunction useMessageHandler() {\n  const viewer = useContext(ViewerContext)!;\n  const scene = useThree((state) => state.scene);\n\n  const removeSceneNode = viewer.useSceneTree((state) => state.removeSceneNode);\n  const resetScene = viewer.useSceneTree((state) => state.resetScene);\n  const addSceneNode = viewer.useSceneTree((state) => state.addSceneNode);\n  const addGui = viewer.useGui((state) => state.addGui);\n  const removeGui = viewer.useGui((state) => state.removeGui);\n  const guiSet = viewer.useGui((state) => state.guiSet);\n  const setOrientation = viewer.useSceneTree((state) => state.setOrientation);\n  const setPosition = viewer.useSceneTree((state) => state.setPosition);\n  const setVisibility = viewer.useSceneTree((state) => state.setVisibility);\n\n  // Same as addSceneNode, but make a parent in the form of a dummy coordinate\n  // frame if it doesn't exist yet.\n  function addSceneNodeMakeParents(node: SceneNode) {\n    const nodeFromName = viewer.useSceneTree.getState().nodeFromName;\n    const parent_name = node.name.split(\"/\").slice(0, -1).join(\"/\");\n    if (!(parent_name in nodeFromName)) {\n      addSceneNodeMakeParents(\n        new SceneNode(parent_name, (ref) => (\n          <CoordinateFrame ref={ref} show_axes={false} />\n        ))\n      );\n    }\n    addSceneNode(node);\n  }\n\n  // Return message handler.\n  return (message: Message) => {\n    switch (message.type) {\n      // Add a coordinate frame.\n      case \"FrameMessage\": {\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <CoordinateFrame\n              ref={ref}\n              position={new THREE.Vector3().fromArray(message.position)}\n              quaternion={\n                new THREE.Quaternion(\n                  message.wxyz[1],\n                  message.wxyz[2],\n                  message.wxyz[3],\n                  message.wxyz[0]\n                )\n              }\n              show_axes={message.show_axes}\n              axes_length={message.axes_length}\n              axes_radius={message.axes_radius}\n            />\n          ))\n        );\n        break;\n      }\n      // Add a point cloud.\n      case \"PointCloudMessage\": {\n        const geometry = new THREE.BufferGeometry();\n        const pointCloudMaterial = new THREE.PointsMaterial({\n          size: message.point_size,\n          vertexColors: true,\n        });\n\n        // Reinterpret cast: uint8 buffer => float32 for positions.\n        geometry.setAttribute(\n          \"position\",\n          new THREE.Float32BufferAttribute(\n            new Float32Array(\n              message.position.buffer.slice(\n                message.position.byteOffset,\n                message.position.byteOffset + message.position.byteLength\n              )\n            ),\n            3\n          )\n        );\n        geometry.computeBoundingSphere();\n\n        // Wrap uint8 buffer for colors. Note that we need to set normalized=true.\n        geometry.setAttribute(\n          \"color\",\n          new THREE.Uint8BufferAttribute(message.color, 3, true)\n        );\n\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <points\n              ref={ref}\n              geometry={geometry}\n              material={pointCloudMaterial}\n            />\n          ))\n        );\n        break;\n      }\n      // Add mesh\n      case \"MeshMessage\": {\n        const geometry = new THREE.BufferGeometry();\n        // TODO(hangg): Should expose color as well.\n        const material = new THREE.MeshStandardMaterial({\n          color: message.color,\n          wireframe: message.wireframe,\n        });\n        geometry.setAttribute(\n          \"position\",\n          new THREE.Float32BufferAttribute(\n            new Float32Array(\n              message.vertices.buffer.slice(\n                message.vertices.byteOffset,\n                message.vertices.byteOffset + message.vertices.byteLength\n              )\n            ),\n            3\n          )\n        );\n        geometry.setIndex(\n          new THREE.Uint32BufferAttribute(\n            new Uint32Array(\n              message.faces.buffer.slice(\n                message.faces.byteOffset,\n                message.faces.byteOffset + message.faces.byteLength\n              )\n            ),\n            1\n          )\n        );\n        geometry.computeVertexNormals();\n        geometry.computeBoundingSphere();\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <mesh ref={ref} geometry={geometry} material={material} />\n          ))\n        );\n        break;\n      }\n      // Add a camera frustum.\n      case \"CameraFrustumMessage\": {\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <CameraFrustum\n              ref={ref}\n              fov={message.fov}\n              aspect={message.aspect}\n              scale={message.scale}\n              color={message.color}\n            ></CameraFrustum>\n          ))\n        );\n        break;\n      }\n      case \"TransformControlsMessage\": {\n        const name = message.name;\n        const sendDragMessage = makeThrottledMessageSender(\n          viewer.websocketRef,\n          25\n        );\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <PivotControls\n              ref={ref}\n              scale={message.scale}\n              lineWidth={message.line_width}\n              fixed={message.fixed}\n              autoTransform={message.auto_transform}\n              activeAxes={message.active_axes}\n              disableAxes={message.disable_axes}\n              disableSliders={message.disable_sliders}\n              disableRotations={message.disable_rotations}\n              translationLimits={message.translation_limits}\n              rotationLimits={message.rotation_limits}\n              depthTest={message.depth_test}\n              opacity={message.opacity}\n              onDrag={(l) => {\n                const wxyz = new THREE.Quaternion();\n                wxyz.setFromRotationMatrix(l);\n                const position = new THREE.Vector3().setFromMatrixPosition(l);\n                sendDragMessage({\n                  type: \"TransformControlsUpdateMessage\",\n                  name: name,\n                  wxyz: [wxyz.w, wxyz.x, wxyz.y, wxyz.z],\n                  position: position.toArray(),\n                });\n              }}\n            />\n          ))\n        );\n        break;\n      }\n      case \"SetCameraOrientationMessage\": {\n        const camera = viewer.globalCameras.current!.cameras[viewer.panelKey];\n        const cameraControls =\n          viewer.globalCameras.current!.cameraControlRefs[viewer.panelKey]\n            .current!;\n\n        const R_world_camera = new THREE.Quaternion(\n          message.wxyz[1],\n          message.wxyz[2],\n          message.wxyz[3],\n          message.wxyz[0]\n        );\n\n        const R_cam_threecam = new THREE.Quaternion();\n        const R_threeworld_world = new THREE.Quaternion();\n        R_cam_threecam.setFromEuler(new THREE.Euler(-Math.PI, 0.0, 0.0));\n        R_threeworld_world.setFromEuler(\n          new THREE.Euler(-Math.PI / 2.0, 0.0, 0.0)\n        );\n        const R_threeworld_threecamera = R_threeworld_world.clone()\n          .multiply(R_world_camera)\n          .multiply(R_cam_threecam);\n\n        // Compute a look-at point, while holding the orbit distance constant.\n        const position = cameraControls.getPosition(new THREE.Vector3());\n        const currentTargetDist = cameraControls\n          .getTarget(new THREE.Vector3())\n          .sub(position)\n          .length();\n        const target = new THREE.Vector3(0.0, 0.0, -currentTargetDist)\n          .applyQuaternion(R_threeworld_threecamera)\n          .add(position);\n\n        // Compute and apply a new up direction.\n        // The goal here is simple: set the up direction s.t. the camera roll is correct,\n        // but keep the up direction as close to a world-frame vertical as possible.\n        const eps = 1e-7;\n        const facePlane = target.clone().sub(position).setY(eps).normalize();\n        const up = new THREE.Vector3(eps, 1.0, eps)\n          .projectOnPlane(facePlane)\n          .normalize();\n        camera.up.set(up.x, up.y, up.z);\n\n        cameraControls.setLookAt(\n          position.x,\n          position.y,\n          position.z,\n          target.x,\n          target.y,\n          target.z\n        );\n        break;\n      }\n      case \"SetCameraPositionMessage\": {\n        const cameraControls =\n          viewer.globalCameras.current!.cameraControlRefs[viewer.panelKey]\n            .current!;\n\n        // When setting camera position, we're going to shift the look-at point by the same amount as the position.\n        // This will hold the camera orientation constant.\n        const position_cur = new THREE.Vector3();\n        cameraControls.getPosition(position_cur);\n\n        const position_cmd = new THREE.Vector3(\n          message.position[0],\n          message.position[1],\n          message.position[2]\n        );\n        const R_worldthree_world = new THREE.Quaternion();\n        R_worldthree_world.setFromEuler(\n          new THREE.Euler(-Math.PI / 2.0, 0.0, 0.0)\n        );\n        position_cmd.applyQuaternion(R_worldthree_world);\n\n        const target = cameraControls\n          .getTarget(new THREE.Vector3())\n          .add(position_cmd)\n          .sub(position_cur);\n\n        cameraControls.setLookAt(\n          position_cmd.x,\n          position_cmd.y,\n          position_cmd.z,\n          target.x,\n          target.y,\n          target.z\n        );\n        break;\n      }\n      case \"SetCameraFovMessage\": {\n        const camera = viewer.globalCameras.current!.cameras[viewer.panelKey];\n        // tan(fov / 2.0) = 0.5 * film height / focal length\n        // focal length = 0.5 * film height / tan(fov / 2.0)\n        camera.setFocalLength(\n          (0.5 * camera.getFilmHeight()) / Math.tan(message.fov / 2.0)\n        );\n        break;\n      }\n      case \"SetOrientationMessage\": {\n        setOrientation(\n          message.name,\n          new THREE.Quaternion(\n            message.wxyz[1],\n            message.wxyz[2],\n            message.wxyz[3],\n            message.wxyz[0]\n          )\n        );\n        break;\n      }\n      case \"SetPositionMessage\": {\n        setPosition(\n          message.name,\n          new THREE.Vector3(\n            message.position[0],\n            message.position[1],\n            message.position[2]\n          )\n        );\n        break;\n      }\n      // Add a background image.\n      case \"BackgroundImageMessage\": {\n        const oldBackground = scene.background;\n        const texture = new TextureLoader().load(\n          `data:${message.media_type};base64,${message.base64_data}`\n        );\n        scene.background = texture;\n        scene.background.encoding = THREE.sRGBEncoding;\n\n        if (isTexture(oldBackground)) oldBackground.dispose();\n        break;\n      }\n      // Add an image.\n      case \"ImageMessage\": {\n        // It's important that we load the texture outside of the node\n        // construction callback; this prevents flickering by ensuring that the\n        // texture is ready before the scene tree updates.\n        const colorMap = new TextureLoader().load(\n          `data:${message.media_type};base64,${message.base64_data}`\n        );\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => {\n            return (\n              <mesh ref={ref}>\n                <planeGeometry\n                  attach=\"geometry\"\n                  args={[message.render_width, message.render_height]}\n                />\n                <meshBasicMaterial\n                  attach=\"material\"\n                  transparent={true}\n                  side={THREE.DoubleSide}\n                  map={colorMap}\n                />\n              </mesh>\n            );\n          })\n        );\n        break;\n      }\n      // Remove a scene node by name.\n      case \"RemoveSceneNodeMessage\": {\n        console.log(\"Removing scene node:\", message.name);\n        removeSceneNode(message.name);\n        break;\n      }\n      // Set the visibility of a particular scene node.\n      case \"SetSceneNodeVisibilityMessage\": {\n        setVisibility(message.name, message.visible);\n        break;\n      }\n      // Reset the entire scene, removing all scene nodes.\n      case \"ResetSceneMessage\": {\n        resetScene();\n\n        const oldBackground = scene.background;\n        scene.background = null;\n        if (isTexture(oldBackground)) oldBackground.dispose();\n\n        viewer.useGui.setState({ backgroundAvailable: false });\n        break;\n      }\n      // Add a GUI input.\n      case \"GuiAddMessage\": {\n        addGui(message.name, {\n          levaConf: message.leva_conf,\n          folderLabels: message.folder_labels,\n          visible: true,\n        });\n        break;\n      }\n      // Set the value of a GUI input.\n      case \"GuiSetValueMessage\": {\n        guiSet(message.name, message.value);\n        break;\n      }\n      // Set the hidden state of a GUI input.\n      case \"GuiSetVisibleMessage\": {\n        const currentConf =\n          viewer.useGui.getState().guiConfigFromName[message.name];\n        if (currentConf !== undefined) {\n          addGui(message.name, {\n            ...currentConf,\n            visible: message.visible,\n          });\n        }\n        break;\n      }\n      // Add a GUI input.\n      case \"GuiSetLevaConfMessage\": {\n        const currentConf =\n          viewer.useGui.getState().guiConfigFromName[message.name];\n        if (currentConf !== undefined) {\n          addGui(message.name, {\n            ...currentConf,\n            levaConf: message.leva_conf,\n          });\n        }\n        break;\n      }\n      // Remove a GUI input.\n      case \"GuiRemoveMessage\": {\n        removeGui(message.name);\n        break;\n      }\n      default: {\n        console.log(\"Received message did not match any known types:\", message);\n        break;\n      }\n    }\n  };\n}\n\n/** Component for handling websocket connections. */\nexport default function WebsocketInterface() {\n  const viewer = useContext(ViewerContext)!;\n  const handleMessage = useMessageHandler();\n\n  const server = viewer.useGui((state) => state.server);\n  const resetGui = viewer.useGui((state) => state.resetGui);\n\n  syncSearchParamServer(viewer.panelKey, server);\n\n  React.useEffect(() => {\n    // Lock for making sure messages are handled in order.\n    const orderLock = new AwaitLock();\n\n    let ws: null | WebSocket = null;\n    let done = false;\n\n    function tryConnect(): void {\n      if (done) return;\n\n      ws = new WebSocket(server);\n\n      ws.onopen = () => {\n        console.log(\"Connected!\" + server);\n        viewer.websocketRef.current = ws;\n        viewer.useGui.setState({ websocketConnected: true });\n      };\n\n      ws.onclose = () => {\n        console.log(\"Disconnected! \" + server);\n        viewer.websocketRef.current = null;\n        viewer.useGui.setState({ websocketConnected: false });\n        if (viewer.useGui.getState().guiNames.length > 0) resetGui();\n\n        // Try to reconnect.\n        timeout = setTimeout(tryConnect, 1000);\n      };\n\n      const messageQueue: Message[] = [];\n      const messageGroup: Message[] = [];\n      let grouping = false;\n\n      // Handle batches of messages at 200Hz. This helps prevent some React errors from interrupting renders.\n      setInterval(() => {\n        const numMessages = messageQueue.length;\n        const processBatch = messageQueue.slice(0, numMessages);\n        messageQueue.splice(0, numMessages);\n        processBatch.forEach(handleMessage);\n      }, 5);\n\n      ws.onmessage = async (event) => {\n        // Reduce websocket backpressure.\n        const messagePromise = new Promise<Message>((resolve) => {\n          (event.data.arrayBuffer() as Promise<ArrayBuffer>).then((buffer) => {\n            resolve(unpack(new Uint8Array(buffer)) as Message);\n          });\n        });\n\n        // Try our best to handle messages in order. If this takes more than 1 second, we give up. :)\n        await orderLock.acquireAsync({ timeout: 1000 }).catch(() => {\n          console.log(\"Order lock timed out.\");\n          orderLock.release();\n        });\n        try {\n          const message = await messagePromise;\n          if (message.type === \"MessageGroupStart\") grouping = true;\n          else if (message.type === \"MessageGroupEnd\") {\n            messageQueue.push(...messageGroup);\n            messageGroup.length = 0;\n            grouping = false;\n          } else if (grouping) {\n            messageGroup.push(message);\n          } else {\n            messageQueue.push(message);\n          }\n        } finally {\n          orderLock.acquired && orderLock.release();\n        }\n      };\n    }\n\n    let timeout = setTimeout(tryConnect, 500);\n    return () => {\n      done = true;\n      clearTimeout(timeout);\n      viewer.useGui.setState({ websocketConnected: false });\n      ws && ws.close();\n      clearTimeout(timeout);\n    };\n  }, [server, handleMessage, resetGui]);\n\n  return <></>;\n}\n",
-        "import React, { RefObject, useContext } from \"react\";\nimport { PerspectiveCamera } from \"three\";\nimport * as holdEvent from \"hold-event\";\nimport { CameraControls } from \"@react-three/drei\";\nimport { makeThrottledMessageSender } from \"./WebsocketInterface\";\nimport { useThree } from \"@react-three/fiber\";\nimport * as THREE from \"three\";\nimport { ViewerContext } from \".\";\n\nexport interface CameraPrimitives {\n  synchronize: boolean;\n  cameras: PerspectiveCamera[];\n  cameraControlRefs: RefObject<CameraControls>[];\n}\n\n/** OrbitControls, but synchronized with the server and other panels. */\nexport function SynchronizedCameraControls() {\n  const viewer = useContext(ViewerContext)!;\n  const camera = useThree((state) => state.camera as PerspectiveCamera);\n  const cameraControlRef = React.useRef<CameraControls>(null);\n\n  const sendCameraThrottled = makeThrottledMessageSender(\n    viewer.websocketRef,\n    20\n  );\n\n  // Callback for sending cameras.\n  const sendCamera = React.useCallback(() => {\n    const three_camera = camera;\n\n    // We put Z up to match the scene tree, and convert threejs camera convention\n    // to the OpenCV one.\n    const R_threecam_cam = new THREE.Quaternion();\n    const R_world_threeworld = new THREE.Quaternion();\n    R_threecam_cam.setFromEuler(new THREE.Euler(Math.PI, 0.0, 0.0));\n    R_world_threeworld.setFromEuler(new THREE.Euler(Math.PI / 2.0, 0.0, 0.0));\n    const R_world_camera = R_world_threeworld.clone()\n      .multiply(three_camera.quaternion)\n      .multiply(R_threecam_cam);\n\n    sendCameraThrottled({\n      type: \"ViewerCameraMessage\",\n      wxyz: [\n        R_world_camera.w,\n        R_world_camera.x,\n        R_world_camera.y,\n        R_world_camera.z,\n      ],\n      position: three_camera.position\n        .clone()\n        .applyQuaternion(R_world_threeworld)\n        .toArray(),\n      aspect: three_camera.aspect,\n      fov: (three_camera.fov * Math.PI) / 180.0,\n    });\n  }, [camera, sendCameraThrottled]);\n\n  // What do we need to when the camera moves?\n  sendCamera();\n  const cameraChangedCallback = React.useCallback(() => {\n    // If desired, send our camera via websocket.\n    sendCamera();\n\n    // Match all cameras.\n    const globalCameras = viewer.globalCameras.current;\n    if (globalCameras.synchronize) {\n      globalCameras.synchronize = false;\n\n      globalCameras.cameraControlRefs.forEach((other) => {\n        if (cameraControlRef === other) return;\n        const position = new THREE.Vector3();\n        const target = new THREE.Vector3();\n        cameraControlRef.current!.getPosition(position);\n        cameraControlRef.current!.getTarget(target);\n        other.current!.setLookAt(\n          position.x,\n          position.y,\n          position.z,\n          target.x,\n          target.y,\n          target.z\n        );\n      });\n\n      // Hack to prevent the cameraChangedCallback() functions of other camera controls from firing.\n      setTimeout(() => (globalCameras.synchronize = true), 1);\n    }\n  }, [viewer.globalCameras, camera, sendCamera]);\n\n  // Send camera for new connections.\n  // We add a small delay to give the server time to add a callback.\n  const connected = viewer.useGui((state) => state.websocketConnected);\n  React.useEffect(() => {\n    if (!connected) return;\n    setTimeout(() => cameraChangedCallback(), 50);\n  }, [connected, cameraChangedCallback]);\n\n  React.useEffect(() => {\n    const globalCameras = viewer.globalCameras.current;\n\n    if (globalCameras.synchronize && globalCameras.cameras.length > 0) {\n      const ours = cameraControlRef.current!;\n      const other = globalCameras.cameraControlRefs[0].current!;\n      const position = new THREE.Vector3();\n      const target = new THREE.Vector3();\n      other.getPosition(position);\n      other.getTarget(target);\n      ours.setLookAt(\n        position.x,\n        position.y,\n        position.z,\n        target.x,\n        target.y,\n        target.z\n      );\n    }\n\n    globalCameras.cameras.push(camera);\n    globalCameras.cameraControlRefs.push(cameraControlRef);\n\n    window.addEventListener(\"resize\", cameraChangedCallback);\n\n    return () => {\n      window.removeEventListener(\"resize\", cameraChangedCallback);\n\n      // Remove ourself from camera list. Since we always add/remove panels\n      // from the end, a pop() would actually work as well here in constant\n      // time.\n      globalCameras.cameras.splice(globalCameras.cameras.indexOf(camera), 1);\n      globalCameras.cameraControlRefs.splice(\n        globalCameras.cameraControlRefs.indexOf(cameraControlRef),\n        1\n      );\n    };\n  }, [cameraChangedCallback, camera, viewer.globalCameras]);\n\n  // Keyboard controls.\n  React.useEffect(() => {\n    const KEYCODE = {\n      W: 87,\n      A: 65,\n      S: 83,\n      D: 68,\n      ARROW_LEFT: 37,\n      ARROW_UP: 38,\n      ARROW_RIGHT: 39,\n      ARROW_DOWN: 40,\n    };\n    const cameraControls = cameraControlRef.current!;\n\n    const wKey = new holdEvent.KeyboardKeyHold(KEYCODE.W, 20);\n    const aKey = new holdEvent.KeyboardKeyHold(KEYCODE.A, 20);\n    const sKey = new holdEvent.KeyboardKeyHold(KEYCODE.S, 20);\n    const dKey = new holdEvent.KeyboardKeyHold(KEYCODE.D, 20);\n    aKey.addEventListener(\"holding\", (event) => {\n      cameraControls.truck(-0.01 * event!.deltaTime, 0, false);\n    });\n    dKey.addEventListener(\"holding\", (event) => {\n      cameraControls.truck(0.01 * event!.deltaTime, 0, false);\n    });\n    wKey.addEventListener(\"holding\", (event) => {\n      cameraControls.forward(0.01 * event!.deltaTime, false);\n    });\n    sKey.addEventListener(\"holding\", (event) => {\n      cameraControls.forward(-0.01 * event!.deltaTime, false);\n    });\n\n    const leftKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_LEFT, 20);\n    const rightKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_RIGHT, 20);\n    const upKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_UP, 20);\n    const downKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_DOWN, 20);\n    leftKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        -0.1 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        0,\n        true\n      );\n    });\n    rightKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0.1 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        0,\n        true\n      );\n    });\n    upKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0,\n        -0.05 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        true\n      );\n    });\n    downKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0,\n        0.05 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        true\n      );\n    });\n\n    // It seems like we should be disposing some event listeners, but we don't get errors despite not doing this. Worth revisiting.\n  });\n\n  return (\n    <CameraControls\n      ref={cameraControlRef}\n      minDistance={0.5}\n      maxDistance={200.0}\n      dollySpeed={0.3}\n      smoothTime={0.0}\n      draggingSmoothTime={0.0}\n      onChange={cameraChangedCallback}\n      makeDefault\n    />\n  );\n}\n",
+        "import { pack, unpack } from \"msgpackr\";\nimport React, { MutableRefObject, useContext } from \"react\";\nimport * as THREE from \"three\";\nimport AwaitLock from \"await-lock\";\nimport { TextureLoader } from \"three\";\n\nimport { SceneNode } from \"./SceneTree\";\nimport { CoordinateFrame, CameraFrustum } from \"./ThreeAssets\";\nimport { Message } from \"./WebsocketMessages\";\nimport { syncSearchParamServer } from \"./SearchParamsUtils\";\nimport { PivotControls } from \"@react-three/drei\";\nimport { ViewerContext } from \".\";\nimport { useThree } from \"@react-three/fiber\";\n\n/** Send message over websocket. */\nexport function sendWebsocketMessage(\n  websocketRef: MutableRefObject<WebSocket | null>,\n  message: Message\n) {\n  if (websocketRef.current === null) return;\n  websocketRef.current.send(pack(message));\n}\n\n/** Returns a function for sending messages, with automatic throttling. */\nexport function makeThrottledMessageSender(\n  websocketRef: MutableRefObject<WebSocket | null>,\n  throttleMilliseconds: number\n) {\n  let readyToSend = true;\n  let stale = false;\n  let latestMessage: Message | null = null;\n\n  function send(message: Message) {\n    if (websocketRef.current === null) return;\n    latestMessage = message;\n    if (readyToSend) {\n      websocketRef.current.send(pack(message));\n      stale = false;\n      readyToSend = false;\n\n      setTimeout(() => {\n        readyToSend = true;\n        if (!stale) return;\n        latestMessage && send(latestMessage);\n      }, throttleMilliseconds);\n    } else {\n      stale = true;\n    }\n  }\n  return send;\n}\n\n/** Type guard for threejs textures. Meant to be used with `scene.background`. */\nexport function isTexture(\n  background: THREE.Color | THREE.Texture | THREE.CubeTexture | null\n): background is THREE.Texture {\n  return (\n    background !== null && (background as THREE.Texture).isTexture !== undefined\n  );\n}\n\n/** Returns a handler for all incoming messages. */\nfunction useMessageHandler() {\n  const viewer = useContext(ViewerContext)!;\n  const scene = useThree((state) => state.scene);\n\n  const removeSceneNode = viewer.useSceneTree((state) => state.removeSceneNode);\n  const resetScene = viewer.useSceneTree((state) => state.resetScene);\n  const addSceneNode = viewer.useSceneTree((state) => state.addSceneNode);\n  const addGui = viewer.useGui((state) => state.addGui);\n  const removeGui = viewer.useGui((state) => state.removeGui);\n  const guiSet = viewer.useGui((state) => state.guiSet);\n  const setOrientation = viewer.useSceneTree((state) => state.setOrientation);\n  const setPosition = viewer.useSceneTree((state) => state.setPosition);\n  const setVisibility = viewer.useSceneTree((state) => state.setVisibility);\n\n  // Same as addSceneNode, but make a parent in the form of a dummy coordinate\n  // frame if it doesn't exist yet.\n  function addSceneNodeMakeParents(node: SceneNode) {\n    const nodeFromName = viewer.useSceneTree.getState().nodeFromName;\n    const parent_name = node.name.split(\"/\").slice(0, -1).join(\"/\");\n    if (!(parent_name in nodeFromName)) {\n      addSceneNodeMakeParents(\n        new SceneNode(parent_name, (ref) => (\n          <CoordinateFrame ref={ref} show_axes={false} />\n        ))\n      );\n    }\n    addSceneNode(node);\n  }\n\n  // Return message handler.\n  return (message: Message) => {\n    switch (message.type) {\n      // Add a coordinate frame.\n      case \"FrameMessage\": {\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <CoordinateFrame\n              ref={ref}\n              position={new THREE.Vector3().fromArray(message.position)}\n              quaternion={\n                new THREE.Quaternion(\n                  message.wxyz[1],\n                  message.wxyz[2],\n                  message.wxyz[3],\n                  message.wxyz[0]\n                )\n              }\n              show_axes={message.show_axes}\n              axes_length={message.axes_length}\n              axes_radius={message.axes_radius}\n            />\n          ))\n        );\n        break;\n      }\n      // Add a point cloud.\n      case \"PointCloudMessage\": {\n        const geometry = new THREE.BufferGeometry();\n        const pointCloudMaterial = new THREE.PointsMaterial({\n          size: message.point_size,\n          vertexColors: true,\n        });\n\n        // Reinterpret cast: uint8 buffer => float32 for positions.\n        geometry.setAttribute(\n          \"position\",\n          new THREE.Float32BufferAttribute(\n            new Float32Array(\n              message.position.buffer.slice(\n                message.position.byteOffset,\n                message.position.byteOffset + message.position.byteLength\n              )\n            ),\n            3\n          )\n        );\n        geometry.computeBoundingSphere();\n\n        // Wrap uint8 buffer for colors. Note that we need to set normalized=true.\n        geometry.setAttribute(\n          \"color\",\n          new THREE.Uint8BufferAttribute(message.color, 3, true)\n        );\n\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <points\n              ref={ref}\n              geometry={geometry}\n              material={pointCloudMaterial}\n            />\n          ))\n        );\n        break;\n      }\n      // Add mesh\n      case \"MeshMessage\": {\n        const geometry = new THREE.BufferGeometry();\n        // TODO(hangg): Should expose color as well.\n        const material = new THREE.MeshStandardMaterial({\n          color: message.color,\n          wireframe: message.wireframe,\n        });\n        geometry.setAttribute(\n          \"position\",\n          new THREE.Float32BufferAttribute(\n            new Float32Array(\n              message.vertices.buffer.slice(\n                message.vertices.byteOffset,\n                message.vertices.byteOffset + message.vertices.byteLength\n              )\n            ),\n            3\n          )\n        );\n        geometry.setIndex(\n          new THREE.Uint32BufferAttribute(\n            new Uint32Array(\n              message.faces.buffer.slice(\n                message.faces.byteOffset,\n                message.faces.byteOffset + message.faces.byteLength\n              )\n            ),\n            1\n          )\n        );\n        geometry.computeVertexNormals();\n        geometry.computeBoundingSphere();\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <mesh ref={ref} geometry={geometry} material={material} />\n          ))\n        );\n        break;\n      }\n      // Add a camera frustum.\n      case \"CameraFrustumMessage\": {\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <CameraFrustum\n              ref={ref}\n              fov={message.fov}\n              aspect={message.aspect}\n              scale={message.scale}\n              color={message.color}\n            ></CameraFrustum>\n          ))\n        );\n        break;\n      }\n      case \"TransformControlsMessage\": {\n        const name = message.name;\n        const sendDragMessage = makeThrottledMessageSender(\n          viewer.websocketRef,\n          25\n        );\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => (\n            <PivotControls\n              ref={ref}\n              scale={message.scale}\n              lineWidth={message.line_width}\n              fixed={message.fixed}\n              autoTransform={message.auto_transform}\n              activeAxes={message.active_axes}\n              disableAxes={message.disable_axes}\n              disableSliders={message.disable_sliders}\n              disableRotations={message.disable_rotations}\n              translationLimits={message.translation_limits}\n              rotationLimits={message.rotation_limits}\n              depthTest={message.depth_test}\n              opacity={message.opacity}\n              onDrag={(l) => {\n                const wxyz = new THREE.Quaternion();\n                wxyz.setFromRotationMatrix(l);\n                const position = new THREE.Vector3().setFromMatrixPosition(l);\n                sendDragMessage({\n                  type: \"TransformControlsUpdateMessage\",\n                  name: name,\n                  wxyz: [wxyz.w, wxyz.x, wxyz.y, wxyz.z],\n                  position: position.toArray(),\n                });\n              }}\n            />\n          ))\n        );\n        break;\n      }\n      case \"SetCameraLookAtMessage\": {\n        const cameraControls =\n          viewer.globalCameras.current!.cameraControlRefs[viewer.panelKey]\n            .current!;\n\n        const R_threeworld_world = new THREE.Quaternion();\n        R_threeworld_world.setFromEuler(\n          new THREE.Euler(-Math.PI / 2.0, 0.0, 0.0)\n        );\n        const target = new THREE.Vector3(\n          message.look_at[0],\n          message.look_at[1],\n          message.look_at[2]\n        );\n        target.applyQuaternion(R_threeworld_world);\n        cameraControls.setTarget(target.x, target.y, target.z);\n        break;\n      }\n      case \"SetCameraUpDirectionMessage\": {\n        const camera = viewer.globalCameras.current!.cameras[viewer.panelKey];\n        const cameraControls =\n          viewer.globalCameras.current!.cameraControlRefs[viewer.panelKey]\n            .current!;\n        const R_threeworld_world = new THREE.Quaternion();\n        R_threeworld_world.setFromEuler(\n          new THREE.Euler(-Math.PI / 2.0, 0.0, 0.0)\n        );\n        const updir = new THREE.Vector3(\n          message.position[0],\n          message.position[1],\n          message.position[2]\n        ).applyQuaternion(R_threeworld_world);\n        camera.up.set(updir.x, updir.y, updir.z);\n        cameraControls.updateCameraUp();\n        break;\n      }\n      case \"SetCameraPositionMessage\": {\n        const cameraControls =\n          viewer.globalCameras.current!.cameraControlRefs[viewer.panelKey]\n            .current!;\n\n        // Set the camera position. Note that this will shift the orientation as-well.\n        const position_cmd = new THREE.Vector3(\n          message.position[0],\n          message.position[1],\n          message.position[2]\n        );\n        const R_worldthree_world = new THREE.Quaternion();\n        R_worldthree_world.setFromEuler(\n          new THREE.Euler(-Math.PI / 2.0, 0.0, 0.0)\n        );\n        position_cmd.applyQuaternion(R_worldthree_world);\n\n        cameraControls.setPosition(\n          position_cmd.x,\n          position_cmd.y,\n          position_cmd.z\n        );\n        break;\n      }\n      case \"SetCameraFovMessage\": {\n        const camera = viewer.globalCameras.current!.cameras[viewer.panelKey];\n        // tan(fov / 2.0) = 0.5 * film height / focal length\n        // focal length = 0.5 * film height / tan(fov / 2.0)\n        camera.setFocalLength(\n          (0.5 * camera.getFilmHeight()) / Math.tan(message.fov / 2.0)\n        );\n        break;\n      }\n      case \"SetOrientationMessage\": {\n        setOrientation(\n          message.name,\n          new THREE.Quaternion(\n            message.wxyz[1],\n            message.wxyz[2],\n            message.wxyz[3],\n            message.wxyz[0]\n          )\n        );\n        break;\n      }\n      case \"SetPositionMessage\": {\n        setPosition(\n          message.name,\n          new THREE.Vector3(\n            message.position[0],\n            message.position[1],\n            message.position[2]\n          )\n        );\n        break;\n      }\n      // Add a background image.\n      case \"BackgroundImageMessage\": {\n        const oldBackground = scene.background;\n        const texture = new TextureLoader().load(\n          `data:${message.media_type};base64,${message.base64_data}`\n        );\n        scene.background = texture;\n        scene.background.encoding = THREE.sRGBEncoding;\n\n        if (isTexture(oldBackground)) oldBackground.dispose();\n        viewer.useGui.setState({ backgroundAvailable: true });\n        break;\n      }\n      // Add an image.\n      case \"ImageMessage\": {\n        // It's important that we load the texture outside of the node\n        // construction callback; this prevents flickering by ensuring that the\n        // texture is ready before the scene tree updates.\n        const colorMap = new TextureLoader().load(\n          `data:${message.media_type};base64,${message.base64_data}`\n        );\n        addSceneNodeMakeParents(\n          new SceneNode(message.name, (ref) => {\n            return (\n              <mesh ref={ref}>\n                <planeGeometry\n                  attach=\"geometry\"\n                  args={[message.render_width, message.render_height]}\n                />\n                <meshBasicMaterial\n                  attach=\"material\"\n                  transparent={true}\n                  side={THREE.DoubleSide}\n                  map={colorMap}\n                />\n              </mesh>\n            );\n          })\n        );\n        break;\n      }\n      // Remove a scene node by name.\n      case \"RemoveSceneNodeMessage\": {\n        console.log(\"Removing scene node:\", message.name);\n        removeSceneNode(message.name);\n        break;\n      }\n      // Set the visibility of a particular scene node.\n      case \"SetSceneNodeVisibilityMessage\": {\n        setVisibility(message.name, message.visible);\n        break;\n      }\n      // Reset the entire scene, removing all scene nodes.\n      case \"ResetSceneMessage\": {\n        resetScene();\n\n        const oldBackground = scene.background;\n        scene.background = null;\n        if (isTexture(oldBackground)) oldBackground.dispose();\n\n        viewer.useGui.setState({ backgroundAvailable: false });\n        break;\n      }\n      // Add a GUI input.\n      case \"GuiAddMessage\": {\n        addGui(message.name, {\n          levaConf: message.leva_conf,\n          folderLabels: message.folder_labels,\n          visible: true,\n        });\n        break;\n      }\n      // Set the value of a GUI input.\n      case \"GuiSetValueMessage\": {\n        guiSet(message.name, message.value);\n        break;\n      }\n      // Set the hidden state of a GUI input.\n      case \"GuiSetVisibleMessage\": {\n        const currentConf =\n          viewer.useGui.getState().guiConfigFromName[message.name];\n        if (currentConf !== undefined) {\n          addGui(message.name, {\n            ...currentConf,\n            visible: message.visible,\n          });\n        }\n        break;\n      }\n      // Add a GUI input.\n      case \"GuiSetLevaConfMessage\": {\n        const currentConf =\n          viewer.useGui.getState().guiConfigFromName[message.name];\n        if (currentConf !== undefined) {\n          addGui(message.name, {\n            ...currentConf,\n            levaConf: message.leva_conf,\n          });\n        }\n        break;\n      }\n      // Remove a GUI input.\n      case \"GuiRemoveMessage\": {\n        removeGui(message.name);\n        break;\n      }\n      default: {\n        console.log(\"Received message did not match any known types:\", message);\n        break;\n      }\n    }\n  };\n}\n\n/** Component for handling websocket connections. */\nexport default function WebsocketInterface() {\n  const viewer = useContext(ViewerContext)!;\n  const handleMessage = useMessageHandler();\n\n  const server = viewer.useGui((state) => state.server);\n  const resetGui = viewer.useGui((state) => state.resetGui);\n\n  syncSearchParamServer(viewer.panelKey, server);\n\n  React.useEffect(() => {\n    // Lock for making sure messages are handled in order.\n    const orderLock = new AwaitLock();\n\n    let ws: null | WebSocket = null;\n    let done = false;\n\n    function tryConnect(): void {\n      if (done) return;\n\n      ws = new WebSocket(server);\n\n      ws.onopen = () => {\n        console.log(\"Connected!\" + server);\n        viewer.websocketRef.current = ws;\n        viewer.useGui.setState({ websocketConnected: true });\n      };\n\n      ws.onclose = () => {\n        console.log(\"Disconnected! \" + server);\n        viewer.websocketRef.current = null;\n        viewer.useGui.setState({ websocketConnected: false });\n        if (viewer.useGui.getState().guiNames.length > 0) resetGui();\n\n        // Try to reconnect.\n        timeout = setTimeout(tryConnect, 1000);\n      };\n\n      const messageQueue: Message[] = [];\n      const messageGroup: Message[] = [];\n      let grouping = false;\n\n      // Handle batches of messages at 200Hz. This helps prevent some React errors from interrupting renders.\n      setInterval(() => {\n        const numMessages = messageQueue.length;\n        const processBatch = messageQueue.slice(0, numMessages);\n        messageQueue.splice(0, numMessages);\n        processBatch.forEach(handleMessage);\n      }, 5);\n\n      ws.onmessage = async (event) => {\n        // Reduce websocket backpressure.\n        const messagePromise = new Promise<Message>((resolve) => {\n          (event.data.arrayBuffer() as Promise<ArrayBuffer>).then((buffer) => {\n            resolve(unpack(new Uint8Array(buffer)) as Message);\n          });\n        });\n\n        // Try our best to handle messages in order. If this takes more than 1 second, we give up. :)\n        await orderLock.acquireAsync({ timeout: 1000 }).catch(() => {\n          console.log(\"Order lock timed out.\");\n          orderLock.release();\n        });\n        try {\n          const message = await messagePromise;\n          if (message.type === \"MessageGroupStart\") grouping = true;\n          else if (message.type === \"MessageGroupEnd\") {\n            messageQueue.push(...messageGroup);\n            messageGroup.length = 0;\n            grouping = false;\n          } else if (grouping) {\n            messageGroup.push(message);\n          } else {\n            messageQueue.push(message);\n          }\n        } finally {\n          orderLock.acquired && orderLock.release();\n        }\n      };\n    }\n\n    let timeout = setTimeout(tryConnect, 500);\n    return () => {\n      done = true;\n      clearTimeout(timeout);\n      viewer.useGui.setState({ websocketConnected: false });\n      ws && ws.close();\n      clearTimeout(timeout);\n    };\n  }, [server, handleMessage, resetGui]);\n\n  return <></>;\n}\n",
+        "import React, { RefObject, useContext } from \"react\";\nimport { PerspectiveCamera } from \"three\";\nimport * as holdEvent from \"hold-event\";\nimport { CameraControls } from \"@react-three/drei\";\nimport { makeThrottledMessageSender } from \"./WebsocketInterface\";\nimport { useThree } from \"@react-three/fiber\";\nimport * as THREE from \"three\";\nimport { ViewerContext } from \".\";\n\nexport interface CameraPrimitives {\n  synchronize: boolean;\n  cameras: PerspectiveCamera[];\n  cameraControlRefs: RefObject<CameraControls>[];\n}\n\n/** OrbitControls, but synchronized with the server and other panels. */\nexport function SynchronizedCameraControls() {\n  const viewer = useContext(ViewerContext)!;\n  const camera = useThree((state) => state.camera as PerspectiveCamera);\n  const cameraControlRef = React.useRef<CameraControls>(null);\n\n  const sendCameraThrottled = makeThrottledMessageSender(\n    viewer.websocketRef,\n    20\n  );\n\n  // Callback for sending cameras.\n  const sendCamera = React.useCallback(() => {\n    const three_camera = camera;\n    const camera_control = cameraControlRef.current;\n\n    if (camera_control === null) {\n      // Camera controls not yet ready, let's re-try later.\n      setTimeout(sendCamera, 10);\n      return;\n    }\n\n    // We put Z up to match the scene tree, and convert threejs camera convention\n    // to the OpenCV one.\n    const R_threecam_cam = new THREE.Quaternion();\n    const R_world_threeworld = new THREE.Quaternion();\n    R_threecam_cam.setFromEuler(new THREE.Euler(Math.PI, 0.0, 0.0));\n    R_world_threeworld.setFromEuler(new THREE.Euler(Math.PI / 2.0, 0.0, 0.0));\n    const R_world_camera = R_world_threeworld.clone()\n      .multiply(three_camera.quaternion)\n      .multiply(R_threecam_cam);\n\n    const look_at = camera_control\n      .getTarget(new THREE.Vector3())\n      .applyQuaternion(R_world_threeworld);\n    const up = three_camera.up.clone().applyQuaternion(R_world_threeworld);\n    sendCameraThrottled({\n      type: \"ViewerCameraMessage\",\n      wxyz: [\n        R_world_camera.w,\n        R_world_camera.x,\n        R_world_camera.y,\n        R_world_camera.z,\n      ],\n      position: three_camera.position\n        .clone()\n        .applyQuaternion(R_world_threeworld)\n        .toArray(),\n      aspect: three_camera.aspect,\n      fov: (three_camera.fov * Math.PI) / 180.0,\n      look_at: [look_at.x, look_at.y, look_at.z],\n      up_direction: [up.x, up.y, up.z],\n    });\n  }, [camera, sendCameraThrottled]);\n\n  // What do we need to when the camera moves?\n  sendCamera();\n  const cameraChangedCallback = React.useCallback(() => {\n    // If desired, send our camera via websocket.\n    sendCamera();\n\n    // Match all cameras.\n    const globalCameras = viewer.globalCameras.current;\n    if (globalCameras.synchronize) {\n      globalCameras.synchronize = false;\n\n      globalCameras.cameraControlRefs.forEach((other) => {\n        if (cameraControlRef === other) return;\n        const position = new THREE.Vector3();\n        const target = new THREE.Vector3();\n        cameraControlRef.current!.getPosition(position);\n        cameraControlRef.current!.getTarget(target);\n        other.current!.setLookAt(\n          position.x,\n          position.y,\n          position.z,\n          target.x,\n          target.y,\n          target.z\n        );\n      });\n\n      // Hack to prevent the cameraChangedCallback() functions of other camera controls from firing.\n      setTimeout(() => (globalCameras.synchronize = true), 1);\n    }\n  }, [viewer.globalCameras, camera, sendCamera]);\n\n  // Send camera for new connections.\n  // We add a small delay to give the server time to add a callback.\n  const connected = viewer.useGui((state) => state.websocketConnected);\n  React.useEffect(() => {\n    if (!connected) return;\n    setTimeout(() => cameraChangedCallback(), 50);\n  }, [connected, cameraChangedCallback]);\n\n  React.useEffect(() => {\n    const globalCameras = viewer.globalCameras.current;\n\n    if (globalCameras.synchronize && globalCameras.cameras.length > 0) {\n      const ours = cameraControlRef.current!;\n      const other = globalCameras.cameraControlRefs[0].current!;\n      const position = new THREE.Vector3();\n      const target = new THREE.Vector3();\n      other.getPosition(position);\n      other.getTarget(target);\n      ours.setLookAt(\n        position.x,\n        position.y,\n        position.z,\n        target.x,\n        target.y,\n        target.z\n      );\n    }\n\n    globalCameras.cameras.push(camera);\n    globalCameras.cameraControlRefs.push(cameraControlRef);\n\n    window.addEventListener(\"resize\", cameraChangedCallback);\n\n    return () => {\n      window.removeEventListener(\"resize\", cameraChangedCallback);\n\n      // Remove ourself from camera list. Since we always add/remove panels\n      // from the end, a pop() would actually work as well here in constant\n      // time.\n      globalCameras.cameras.splice(globalCameras.cameras.indexOf(camera), 1);\n      globalCameras.cameraControlRefs.splice(\n        globalCameras.cameraControlRefs.indexOf(cameraControlRef),\n        1\n      );\n    };\n  }, [cameraChangedCallback, camera, viewer.globalCameras]);\n\n  // Keyboard controls.\n  React.useEffect(() => {\n    const KEYCODE = {\n      W: 87,\n      A: 65,\n      S: 83,\n      D: 68,\n      ARROW_LEFT: 37,\n      ARROW_UP: 38,\n      ARROW_RIGHT: 39,\n      ARROW_DOWN: 40,\n    };\n    const cameraControls = cameraControlRef.current!;\n\n    const wKey = new holdEvent.KeyboardKeyHold(KEYCODE.W, 20);\n    const aKey = new holdEvent.KeyboardKeyHold(KEYCODE.A, 20);\n    const sKey = new holdEvent.KeyboardKeyHold(KEYCODE.S, 20);\n    const dKey = new holdEvent.KeyboardKeyHold(KEYCODE.D, 20);\n    aKey.addEventListener(\"holding\", (event) => {\n      cameraControls.truck(-0.01 * event!.deltaTime, 0, false);\n    });\n    dKey.addEventListener(\"holding\", (event) => {\n      cameraControls.truck(0.01 * event!.deltaTime, 0, false);\n    });\n    wKey.addEventListener(\"holding\", (event) => {\n      cameraControls.forward(0.01 * event!.deltaTime, false);\n    });\n    sKey.addEventListener(\"holding\", (event) => {\n      cameraControls.forward(-0.01 * event!.deltaTime, false);\n    });\n\n    const leftKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_LEFT, 20);\n    const rightKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_RIGHT, 20);\n    const upKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_UP, 20);\n    const downKey = new holdEvent.KeyboardKeyHold(KEYCODE.ARROW_DOWN, 20);\n    leftKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        -0.1 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        0,\n        true\n      );\n    });\n    rightKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0.1 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        0,\n        true\n      );\n    });\n    upKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0,\n        -0.05 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        true\n      );\n    });\n    downKey.addEventListener(\"holding\", (event) => {\n      cameraControls.rotate(\n        0,\n        0.05 * THREE.MathUtils.DEG2RAD * event!.deltaTime,\n        true\n      );\n    });\n\n    // It seems like we should be disposing some event listeners, but we don't get errors despite not doing this. Worth revisiting.\n  });\n\n  return (\n    <CameraControls\n      ref={cameraControlRef}\n      minDistance={0.5}\n      maxDistance={200.0}\n      dollySpeed={0.3}\n      smoothTime={0.0}\n      draggingSmoothTime={0.0}\n      onChange={cameraChangedCallback}\n      makeDefault\n    />\n  );\n}\n",
         "function r(e){var t,f,n=\"\";if(\"string\"==typeof e||\"number\"==typeof e)n+=e;else if(\"object\"==typeof e)if(Array.isArray(e))for(t=0;t<e.length;t++)e[t]&&(f=r(e[t]))&&(n&&(n+=\" \"),n+=f);else for(t in e)e[t]&&(n&&(n+=\" \"),n+=t);return n}export function clsx(){for(var e,t,f=0,n=\"\";f<arguments.length;)(e=arguments[f++])&&(t=r(e))&&(n&&(n+=\" \"),n+=t);return n}export default clsx;",
         "/**\n * @mui/styled-engine v5.11.16\n *\n * @license MIT\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n/* eslint-disable no-underscore-dangle */\nimport emStyled from '@emotion/styled';\nexport default function styled(tag, options) {\n  const stylesFactory = emStyled(tag, options);\n  if (process.env.NODE_ENV !== 'production') {\n    return (...styles) => {\n      const component = typeof tag === 'string' ? `\"${tag}\"` : 'component';\n      if (styles.length === 0) {\n        console.error([`MUI: Seems like you called \\`styled(${component})()\\` without a \\`style\\` argument.`, 'You must provide a `styles` argument: `styled(\"div\")(styleYouForgotToPass)`.'].join('\\n'));\n      } else if (styles.some(style => style === undefined)) {\n        console.error(`MUI: the styled(${component})(...args) API requires all its args to be defined.`);\n      }\n      return stylesFactory(...styles);\n    };\n  }\n  return stylesFactory;\n}\n\n// eslint-disable-next-line @typescript-eslint/naming-convention\nexport const internal_processStyles = (tag, processor) => {\n  // Emotion attaches all the styles as `__emotion_styles`.\n  // Ref: https://github.com/emotion-js/emotion/blob/16d971d0da229596d6bcc39d282ba9753c9ee7cf/packages/styled/src/base.js#L186\n  if (Array.isArray(tag.__emotion_styles)) {\n    tag.__emotion_styles = processor(tag.__emotion_styles);\n  }\n};\nexport { ThemeContext, keyframes, css } from '@emotion/react';\nexport { default as StyledEngineProvider } from './StyledEngineProvider';\nexport { default as GlobalStyles } from './GlobalStyles';",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nexport function isPlainObject(item) {\n  return item !== null && typeof item === 'object' && item.constructor === Object;\n}\nfunction deepClone(source) {\n  if (!isPlainObject(source)) {\n    return source;\n  }\n  const output = {};\n  Object.keys(source).forEach(key => {\n    output[key] = deepClone(source[key]);\n  });\n  return output;\n}\nexport default function deepmerge(target, source, options = {\n  clone: true\n}) {\n  const output = options.clone ? _extends({}, target) : target;\n  if (isPlainObject(target) && isPlainObject(source)) {\n    Object.keys(source).forEach(key => {\n      // Avoid prototype pollution\n      if (key === '__proto__') {\n        return;\n      }\n      if (isPlainObject(source[key]) && key in target && isPlainObject(target[key])) {\n        // Since `output` is a clone of `target` and we have narrowed `target` in this block we can cast to the same type.\n        output[key] = deepmerge(target[key], source[key], options);\n      } else if (options.clone) {\n        output[key] = isPlainObject(source[key]) ? deepClone(source[key]) : source[key];\n      } else {\n        output[key] = source[key];\n      }\n    });\n  }\n  return output;\n}",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"values\", \"unit\", \"step\"];\n// Sorted ASC by size. That's important.\n// It can't be configured as it's used statically for propTypes.\nexport const breakpointKeys = ['xs', 'sm', 'md', 'lg', 'xl'];\nconst sortBreakpointsValues = values => {\n  const breakpointsAsArray = Object.keys(values).map(key => ({\n    key,\n    val: values[key]\n  })) || [];\n  // Sort in ascending order\n  breakpointsAsArray.sort((breakpoint1, breakpoint2) => breakpoint1.val - breakpoint2.val);\n  return breakpointsAsArray.reduce((acc, obj) => {\n    return _extends({}, acc, {\n      [obj.key]: obj.val\n    });\n  }, {});\n};\n\n// Keep in mind that @media is inclusive by the CSS specification.\nexport default function createBreakpoints(breakpoints) {\n  const {\n      // The breakpoint **start** at this value.\n      // For instance with the first breakpoint xs: [xs, sm).\n      values = {\n        xs: 0,\n        // phone\n        sm: 600,\n        // tablet\n        md: 900,\n        // small laptop\n        lg: 1200,\n        // desktop\n        xl: 1536 // large screen\n      },\n\n      unit = 'px',\n      step = 5\n    } = breakpoints,\n    other = _objectWithoutPropertiesLoose(breakpoints, _excluded);\n  const sortedValues = sortBreakpointsValues(values);\n  const keys = Object.keys(sortedValues);\n  function up(key) {\n    const value = typeof values[key] === 'number' ? values[key] : key;\n    return `@media (min-width:${value}${unit})`;\n  }\n  function down(key) {\n    const value = typeof values[key] === 'number' ? values[key] : key;\n    return `@media (max-width:${value - step / 100}${unit})`;\n  }\n  function between(start, end) {\n    const endIndex = keys.indexOf(end);\n    return `@media (min-width:${typeof values[start] === 'number' ? values[start] : start}${unit}) and ` + `(max-width:${(endIndex !== -1 && typeof values[keys[endIndex]] === 'number' ? values[keys[endIndex]] : end) - step / 100}${unit})`;\n  }\n  function only(key) {\n    if (keys.indexOf(key) + 1 < keys.length) {\n      return between(key, keys[keys.indexOf(key) + 1]);\n    }\n    return up(key);\n  }\n  function not(key) {\n    // handle first and last key separately, for better readability\n    const keyIndex = keys.indexOf(key);\n    if (keyIndex === 0) {\n      return up(keys[1]);\n    }\n    if (keyIndex === keys.length - 1) {\n      return down(keys[keyIndex]);\n    }\n    return between(key, keys[keys.indexOf(key) + 1]).replace('@media', '@media not all and');\n  }\n  return _extends({\n    keys,\n    values: sortedValues,\n    up,\n    down,\n    between,\n    only,\n    not,\n    unit\n  }, other);\n}",
         "const shape = {\n  borderRadius: 4\n};\nexport default shape;",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport PropTypes from 'prop-types';\nimport { deepmerge } from '@mui/utils';\nimport merge from './merge';\n\n// The breakpoint **start** at this value.\n// For instance with the first breakpoint xs: [xs, sm[.\nexport const values = {\n  xs: 0,\n  // phone\n  sm: 600,\n  // tablet\n  md: 900,\n  // small laptop\n  lg: 1200,\n  // desktop\n  xl: 1536 // large screen\n};\n\nconst defaultBreakpoints = {\n  // Sorted ASC by size. That's important.\n  // It can't be configured as it's used statically for propTypes.\n  keys: ['xs', 'sm', 'md', 'lg', 'xl'],\n  up: key => `@media (min-width:${values[key]}px)`\n};\nexport function handleBreakpoints(props, propValue, styleFromPropValue) {\n  const theme = props.theme || {};\n  if (Array.isArray(propValue)) {\n    const themeBreakpoints = theme.breakpoints || defaultBreakpoints;\n    return propValue.reduce((acc, item, index) => {\n      acc[themeBreakpoints.up(themeBreakpoints.keys[index])] = styleFromPropValue(propValue[index]);\n      return acc;\n    }, {});\n  }\n  if (typeof propValue === 'object') {\n    const themeBreakpoints = theme.breakpoints || defaultBreakpoints;\n    return Object.keys(propValue).reduce((acc, breakpoint) => {\n      // key is breakpoint\n      if (Object.keys(themeBreakpoints.values || values).indexOf(breakpoint) !== -1) {\n        const mediaKey = themeBreakpoints.up(breakpoint);\n        acc[mediaKey] = styleFromPropValue(propValue[breakpoint], breakpoint);\n      } else {\n        const cssKey = breakpoint;\n        acc[cssKey] = propValue[cssKey];\n      }\n      return acc;\n    }, {});\n  }\n  const output = styleFromPropValue(propValue);\n  return output;\n}\nfunction breakpoints(styleFunction) {\n  // false positive\n  // eslint-disable-next-line react/function-component-definition\n  const newStyleFunction = props => {\n    const theme = props.theme || {};\n    const base = styleFunction(props);\n    const themeBreakpoints = theme.breakpoints || defaultBreakpoints;\n    const extended = themeBreakpoints.keys.reduce((acc, key) => {\n      if (props[key]) {\n        acc = acc || {};\n        acc[themeBreakpoints.up(key)] = styleFunction(_extends({\n          theme\n        }, props[key]));\n      }\n      return acc;\n    }, null);\n    return merge(base, extended);\n  };\n  newStyleFunction.propTypes = process.env.NODE_ENV !== 'production' ? _extends({}, styleFunction.propTypes, {\n    xs: PropTypes.object,\n    sm: PropTypes.object,\n    md: PropTypes.object,\n    lg: PropTypes.object,\n    xl: PropTypes.object\n  }) : {};\n  newStyleFunction.filterProps = ['xs', 'sm', 'md', 'lg', 'xl', ...styleFunction.filterProps];\n  return newStyleFunction;\n}\nexport function createEmptyBreakpointObject(breakpointsInput = {}) {\n  var _breakpointsInput$key;\n  const breakpointsInOrder = (_breakpointsInput$key = breakpointsInput.keys) == null ? void 0 : _breakpointsInput$key.reduce((acc, key) => {\n    const breakpointStyleKey = breakpointsInput.up(key);\n    acc[breakpointStyleKey] = {};\n    return acc;\n  }, {});\n  return breakpointsInOrder || {};\n}\nexport function removeUnusedBreakpoints(breakpointKeys, style) {\n  return breakpointKeys.reduce((acc, key) => {\n    const breakpointOutput = acc[key];\n    const isBreakpointUnused = !breakpointOutput || Object.keys(breakpointOutput).length === 0;\n    if (isBreakpointUnused) {\n      delete acc[key];\n    }\n    return acc;\n  }, style);\n}\nexport function mergeBreakpointsInOrder(breakpointsInput, ...styles) {\n  const emptyBreakpoints = createEmptyBreakpointObject(breakpointsInput);\n  const mergedOutput = [emptyBreakpoints, ...styles].reduce((prev, next) => deepmerge(prev, next), {});\n  return removeUnusedBreakpoints(Object.keys(emptyBreakpoints), mergedOutput);\n}\n\n// compute base for responsive values; e.g.,\n// [1,2,3] => {xs: true, sm: true, md: true}\n// {xs: 1, sm: 2, md: 3} => {xs: true, sm: true, md: true}\nexport function computeBreakpointsBase(breakpointValues, themeBreakpoints) {\n  // fixed value\n  if (typeof breakpointValues !== 'object') {\n    return {};\n  }\n  const base = {};\n  const breakpointsKeys = Object.keys(themeBreakpoints);\n  if (Array.isArray(breakpointValues)) {\n    breakpointsKeys.forEach((breakpoint, i) => {\n      if (i < breakpointValues.length) {\n        base[breakpoint] = true;\n      }\n    });\n  } else {\n    breakpointsKeys.forEach(breakpoint => {\n      if (breakpointValues[breakpoint] != null) {\n        base[breakpoint] = true;\n      }\n    });\n  }\n  return base;\n}\nexport function resolveBreakpointValues({\n  values: breakpointValues,\n  breakpoints: themeBreakpoints,\n  base: customBase\n}) {\n  const base = customBase || computeBreakpointsBase(breakpointValues, themeBreakpoints);\n  const keys = Object.keys(base);\n  if (keys.length === 0) {\n    return breakpointValues;\n  }\n  let previous;\n  return keys.reduce((acc, breakpoint, i) => {\n    if (Array.isArray(breakpointValues)) {\n      acc[breakpoint] = breakpointValues[i] != null ? breakpointValues[i] : breakpointValues[previous];\n      previous = i;\n    } else if (typeof breakpointValues === 'object') {\n      acc[breakpoint] = breakpointValues[breakpoint] != null ? breakpointValues[breakpoint] : breakpointValues[previous];\n      previous = breakpoint;\n    } else {\n      acc[breakpoint] = breakpointValues;\n    }\n    return acc;\n  }, {});\n}\nexport default breakpoints;",
         "/**\n * WARNING: Don't import this directly.\n * Use `MuiError` from `@mui/utils/macros/MuiError.macro` instead.\n * @param {number} code\n */\nexport default function formatMuiErrorMessage(code) {\n  // Apply babel-plugin-transform-template-literals in loose mode\n  // loose mode is safe iff we're concatenating primitives\n  // see https://babeljs.io/docs/en/babel-plugin-transform-template-literals#loose\n  /* eslint-disable prefer-template */\n  let url = 'https://mui.com/production-error/?code=' + code;\n  for (let i = 1; i < arguments.length; i += 1) {\n    // rest params over-transpile for this case\n    // eslint-disable-next-line prefer-rest-params\n    url += '&args[]=' + encodeURIComponent(arguments[i]);\n  }\n  return 'Minified MUI error #' + code + '; visit ' + url + ' for the full message.';\n  /* eslint-enable prefer-template */\n}",
@@ -12150,15 +12150,15 @@
         "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); enumerableOnly && (symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; })), keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = null != arguments[i] ? arguments[i] : {}; i % 2 ? ownKeys(Object(source), !0).forEach(function (key) { _defineProperty(target, key, source[key]); }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)) : ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\nfunction _typeof(obj) { \"@babel/helpers - typeof\"; return _typeof = \"function\" == typeof Symbol && \"symbol\" == typeof Symbol.iterator ? function (obj) { return typeof obj; } : function (obj) { return obj && \"function\" == typeof Symbol && obj.constructor === Symbol && obj !== Symbol.prototype ? \"symbol\" : typeof obj; }, _typeof(obj); }\n\nfunction _slicedToArray(arr, i) { return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest(); }\n\nfunction _nonIterableRest() { throw new TypeError(\"Invalid attempt to destructure non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\"); }\n\nfunction _unsupportedIterableToArray(o, minLen) { if (!o) return; if (typeof o === \"string\") return _arrayLikeToArray(o, minLen); var n = Object.prototype.toString.call(o).slice(8, -1); if (n === \"Object\" && o.constructor) n = o.constructor.name; if (n === \"Map\" || n === \"Set\") return Array.from(o); if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen); }\n\nfunction _arrayLikeToArray(arr, len) { if (len == null || len > arr.length) len = arr.length; for (var i = 0, arr2 = new Array(len); i < len; i++) { arr2[i] = arr[i]; } return arr2; }\n\nfunction _iterableToArrayLimit(arr, i) { var _i = arr == null ? null : typeof Symbol !== \"undefined\" && arr[Symbol.iterator] || arr[\"@@iterator\"]; if (_i == null) return; var _arr = []; var _n = true; var _d = false; var _s, _e; try { for (_i = _i.call(arr); !(_n = (_s = _i.next()).done); _n = true) { _arr.push(_s.value); if (i && _arr.length === i) break; } } catch (err) { _d = true; _e = err; } finally { try { if (!_n && _i[\"return\"] != null) _i[\"return\"](); } finally { if (_d) throw _e; } } return _arr; }\n\nfunction _arrayWithHoles(arr) { if (Array.isArray(arr)) return arr; }\n\nimport accepts from \"attr-accept\"; // Error codes\n\nexport var FILE_INVALID_TYPE = \"file-invalid-type\";\nexport var FILE_TOO_LARGE = \"file-too-large\";\nexport var FILE_TOO_SMALL = \"file-too-small\";\nexport var TOO_MANY_FILES = \"too-many-files\";\nexport var ErrorCode = {\n  FileInvalidType: FILE_INVALID_TYPE,\n  FileTooLarge: FILE_TOO_LARGE,\n  FileTooSmall: FILE_TOO_SMALL,\n  TooManyFiles: TOO_MANY_FILES\n}; // File Errors\n\nexport var getInvalidTypeRejectionErr = function getInvalidTypeRejectionErr(accept) {\n  accept = Array.isArray(accept) && accept.length === 1 ? accept[0] : accept;\n  var messageSuffix = Array.isArray(accept) ? \"one of \".concat(accept.join(\", \")) : accept;\n  return {\n    code: FILE_INVALID_TYPE,\n    message: \"File type must be \".concat(messageSuffix)\n  };\n};\nexport var getTooLargeRejectionErr = function getTooLargeRejectionErr(maxSize) {\n  return {\n    code: FILE_TOO_LARGE,\n    message: \"File is larger than \".concat(maxSize, \" \").concat(maxSize === 1 ? \"byte\" : \"bytes\")\n  };\n};\nexport var getTooSmallRejectionErr = function getTooSmallRejectionErr(minSize) {\n  return {\n    code: FILE_TOO_SMALL,\n    message: \"File is smaller than \".concat(minSize, \" \").concat(minSize === 1 ? \"byte\" : \"bytes\")\n  };\n};\nexport var TOO_MANY_FILES_REJECTION = {\n  code: TOO_MANY_FILES,\n  message: \"Too many files\"\n}; // Firefox versions prior to 53 return a bogus MIME type for every file drag, so dragovers with\n// that MIME type will always be accepted\n\nexport function fileAccepted(file, accept) {\n  var isAcceptable = file.type === \"application/x-moz-file\" || accepts(file, accept);\n  return [isAcceptable, isAcceptable ? null : getInvalidTypeRejectionErr(accept)];\n}\nexport function fileMatchSize(file, minSize, maxSize) {\n  if (isDefined(file.size)) {\n    if (isDefined(minSize) && isDefined(maxSize)) {\n      if (file.size > maxSize) return [false, getTooLargeRejectionErr(maxSize)];\n      if (file.size < minSize) return [false, getTooSmallRejectionErr(minSize)];\n    } else if (isDefined(minSize) && file.size < minSize) return [false, getTooSmallRejectionErr(minSize)];else if (isDefined(maxSize) && file.size > maxSize) return [false, getTooLargeRejectionErr(maxSize)];\n  }\n\n  return [true, null];\n}\n\nfunction isDefined(value) {\n  return value !== undefined && value !== null;\n}\n\nexport function allFilesAccepted(_ref) {\n  var files = _ref.files,\n      accept = _ref.accept,\n      minSize = _ref.minSize,\n      maxSize = _ref.maxSize,\n      multiple = _ref.multiple,\n      maxFiles = _ref.maxFiles;\n\n  if (!multiple && files.length > 1 || multiple && maxFiles >= 1 && files.length > maxFiles) {\n    return false;\n  }\n\n  return files.every(function (file) {\n    var _fileAccepted = fileAccepted(file, accept),\n        _fileAccepted2 = _slicedToArray(_fileAccepted, 1),\n        accepted = _fileAccepted2[0];\n\n    var _fileMatchSize = fileMatchSize(file, minSize, maxSize),\n        _fileMatchSize2 = _slicedToArray(_fileMatchSize, 1),\n        sizeMatch = _fileMatchSize2[0];\n\n    return accepted && sizeMatch;\n  });\n} // React's synthetic events has event.isPropagationStopped,\n// but to remain compatibility with other libs (Preact) fall back\n// to check event.cancelBubble\n\nexport function isPropagationStopped(event) {\n  if (typeof event.isPropagationStopped === \"function\") {\n    return event.isPropagationStopped();\n  } else if (typeof event.cancelBubble !== \"undefined\") {\n    return event.cancelBubble;\n  }\n\n  return false;\n}\nexport function isEvtWithFiles(event) {\n  if (!event.dataTransfer) {\n    return !!event.target && !!event.target.files;\n  } // https://developer.mozilla.org/en-US/docs/Web/API/DataTransfer/types\n  // https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API/Recommended_drag_types#file\n\n\n  return Array.prototype.some.call(event.dataTransfer.types, function (type) {\n    return type === \"Files\" || type === \"application/x-moz-file\";\n  });\n}\nexport function isKindFile(item) {\n  return _typeof(item) === \"object\" && item !== null && item.kind === \"file\";\n} // allow the entire document to be a drag target\n\nexport function onDocumentDragOver(event) {\n  event.preventDefault();\n}\n\nfunction isIe(userAgent) {\n  return userAgent.indexOf(\"MSIE\") !== -1 || userAgent.indexOf(\"Trident/\") !== -1;\n}\n\nfunction isEdge(userAgent) {\n  return userAgent.indexOf(\"Edge/\") !== -1;\n}\n\nexport function isIeOrEdge() {\n  var userAgent = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : window.navigator.userAgent;\n  return isIe(userAgent) || isEdge(userAgent);\n}\n/**\n * This is intended to be used to compose event handlers\n * They are executed in order until one of them calls `event.isPropagationStopped()`.\n * Note that the check is done on the first invoke too,\n * meaning that if propagation was stopped before invoking the fns,\n * no handlers will be executed.\n *\n * @param {Function} fns the event hanlder functions\n * @return {Function} the event handler to add to an element\n */\n\nexport function composeEventHandlers() {\n  for (var _len = arguments.length, fns = new Array(_len), _key = 0; _key < _len; _key++) {\n    fns[_key] = arguments[_key];\n  }\n\n  return function (event) {\n    for (var _len2 = arguments.length, args = new Array(_len2 > 1 ? _len2 - 1 : 0), _key2 = 1; _key2 < _len2; _key2++) {\n      args[_key2 - 1] = arguments[_key2];\n    }\n\n    return fns.some(function (fn) {\n      if (!isPropagationStopped(event) && fn) {\n        fn.apply(void 0, [event].concat(args));\n      }\n\n      return isPropagationStopped(event);\n    });\n  };\n}\n/**\n * canUseFileSystemAccessAPI checks if the [File System Access API](https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API)\n * is supported by the browser.\n * @returns {boolean}\n */\n\nexport function canUseFileSystemAccessAPI() {\n  return \"showOpenFilePicker\" in window;\n}\n/**\n * filePickerOptionsTypes returns the {types} option for https://developer.mozilla.org/en-US/docs/Web/API/window/showOpenFilePicker\n * based on the accept attr (see https://github.com/react-dropzone/attr-accept)\n * E.g: converts ['image/*', 'text/*'] to {'image/*': [], 'text/*': []}\n * @param {string|string[]} accept\n */\n\nexport function filePickerOptionsTypes(accept) {\n  accept = typeof accept === \"string\" ? accept.split(\",\") : accept;\n  return [{\n    description: \"everything\",\n    // TODO: Need to handle filtering more elegantly than this!\n    accept: Array.isArray(accept) ? // Accept just MIME types as per spec\n    // NOTE: accept can be https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#unique_file_type_specifiers\n    accept.filter(function (item) {\n      return item === \"audio/*\" || item === \"video/*\" || item === \"image/*\" || item === \"text/*\" || /\\w+\\/[-+.\\w]+/g.test(item);\n    }).reduce(function (a, b) {\n      return _objectSpread(_objectSpread({}, a), {}, _defineProperty({}, b, []));\n    }, {}) : {}\n  }];\n}\n/**\n * Check if v is an exception caused by aborting a request (e.g window.showOpenFilePicker()).\n *\n * See https://developer.mozilla.org/en-US/docs/Web/API/DOMException.\n * @param {any} v\n * @returns {boolean} True if v is an abort exception.\n */\n\nexport function isAbort(v) {\n  return v instanceof DOMException && (v.name === \"AbortError\" || v.code === v.ABORT_ERR);\n}\n/**\n * Check if v is a security error.\n *\n * See https://developer.mozilla.org/en-US/docs/Web/API/DOMException.\n * @param {any} v\n * @returns {boolean} True if v is a security error.\n */\n\nexport function isSecurityError(v) {\n  return v instanceof DOMException && (v.name === \"SecurityError\" || v.code === v.SECURITY_ERR);\n}",
         "var _excluded = [\"children\"],\n    _excluded2 = [\"open\"],\n    _excluded3 = [\"refKey\", \"role\", \"onKeyDown\", \"onFocus\", \"onBlur\", \"onClick\", \"onDragEnter\", \"onDragOver\", \"onDragLeave\", \"onDrop\"],\n    _excluded4 = [\"refKey\", \"onChange\", \"onClick\"];\n\nfunction _toConsumableArray(arr) { return _arrayWithoutHoles(arr) || _iterableToArray(arr) || _unsupportedIterableToArray(arr) || _nonIterableSpread(); }\n\nfunction _nonIterableSpread() { throw new TypeError(\"Invalid attempt to spread non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\"); }\n\nfunction _iterableToArray(iter) { if (typeof Symbol !== \"undefined\" && iter[Symbol.iterator] != null || iter[\"@@iterator\"] != null) return Array.from(iter); }\n\nfunction _arrayWithoutHoles(arr) { if (Array.isArray(arr)) return _arrayLikeToArray(arr); }\n\nfunction _slicedToArray(arr, i) { return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest(); }\n\nfunction _nonIterableRest() { throw new TypeError(\"Invalid attempt to destructure non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\"); }\n\nfunction _unsupportedIterableToArray(o, minLen) { if (!o) return; if (typeof o === \"string\") return _arrayLikeToArray(o, minLen); var n = Object.prototype.toString.call(o).slice(8, -1); if (n === \"Object\" && o.constructor) n = o.constructor.name; if (n === \"Map\" || n === \"Set\") return Array.from(o); if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen); }\n\nfunction _arrayLikeToArray(arr, len) { if (len == null || len > arr.length) len = arr.length; for (var i = 0, arr2 = new Array(len); i < len; i++) { arr2[i] = arr[i]; } return arr2; }\n\nfunction _iterableToArrayLimit(arr, i) { var _i = arr == null ? null : typeof Symbol !== \"undefined\" && arr[Symbol.iterator] || arr[\"@@iterator\"]; if (_i == null) return; var _arr = []; var _n = true; var _d = false; var _s, _e; try { for (_i = _i.call(arr); !(_n = (_s = _i.next()).done); _n = true) { _arr.push(_s.value); if (i && _arr.length === i) break; } } catch (err) { _d = true; _e = err; } finally { try { if (!_n && _i[\"return\"] != null) _i[\"return\"](); } finally { if (_d) throw _e; } } return _arr; }\n\nfunction _arrayWithHoles(arr) { if (Array.isArray(arr)) return arr; }\n\nfunction ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); enumerableOnly && (symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; })), keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = null != arguments[i] ? arguments[i] : {}; i % 2 ? ownKeys(Object(source), !0).forEach(function (key) { _defineProperty(target, key, source[key]); }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)) : ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\nfunction _objectWithoutProperties(source, excluded) { if (source == null) return {}; var target = _objectWithoutPropertiesLoose(source, excluded); var key, i; if (Object.getOwnPropertySymbols) { var sourceSymbolKeys = Object.getOwnPropertySymbols(source); for (i = 0; i < sourceSymbolKeys.length; i++) { key = sourceSymbolKeys[i]; if (excluded.indexOf(key) >= 0) continue; if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue; target[key] = source[key]; } } return target; }\n\nfunction _objectWithoutPropertiesLoose(source, excluded) { if (source == null) return {}; var target = {}; var sourceKeys = Object.keys(source); var key, i; for (i = 0; i < sourceKeys.length; i++) { key = sourceKeys[i]; if (excluded.indexOf(key) >= 0) continue; target[key] = source[key]; } return target; }\n\n/* eslint prefer-template: 0 */\nimport React, { forwardRef, Fragment, useCallback, useEffect, useImperativeHandle, useMemo, useReducer, useRef } from \"react\";\nimport PropTypes from \"prop-types\";\nimport { fromEvent } from \"file-selector\";\nimport { allFilesAccepted, composeEventHandlers, fileAccepted, fileMatchSize, filePickerOptionsTypes, canUseFileSystemAccessAPI, isAbort, isEvtWithFiles, isIeOrEdge, isPropagationStopped, isSecurityError, onDocumentDragOver, TOO_MANY_FILES_REJECTION } from \"./utils/index\";\n/**\n * Convenience wrapper component for the `useDropzone` hook\n *\n * ```jsx\n * <Dropzone>\n *   {({getRootProps, getInputProps}) => (\n *     <div {...getRootProps()}>\n *       <input {...getInputProps()} />\n *       <p>Drag 'n' drop some files here, or click to select files</p>\n *     </div>\n *   )}\n * </Dropzone>\n * ```\n */\n\nvar Dropzone = /*#__PURE__*/forwardRef(function (_ref, ref) {\n  var children = _ref.children,\n      params = _objectWithoutProperties(_ref, _excluded);\n\n  var _useDropzone = useDropzone(params),\n      open = _useDropzone.open,\n      props = _objectWithoutProperties(_useDropzone, _excluded2);\n\n  useImperativeHandle(ref, function () {\n    return {\n      open: open\n    };\n  }, [open]); // TODO: Figure out why react-styleguidist cannot create docs if we don't return a jsx element\n\n  return /*#__PURE__*/React.createElement(Fragment, null, children(_objectSpread(_objectSpread({}, props), {}, {\n    open: open\n  })));\n});\nDropzone.displayName = \"Dropzone\"; // Add default props for react-docgen\n\nvar defaultProps = {\n  disabled: false,\n  getFilesFromEvent: fromEvent,\n  maxSize: Infinity,\n  minSize: 0,\n  multiple: true,\n  maxFiles: 0,\n  preventDropOnDocument: true,\n  noClick: false,\n  noKeyboard: false,\n  noDrag: false,\n  noDragEventsBubbling: false,\n  validator: null,\n  useFsAccessApi: true\n};\nDropzone.defaultProps = defaultProps;\nDropzone.propTypes = {\n  /**\n   * Render function that exposes the dropzone state and prop getter fns\n   *\n   * @param {object} params\n   * @param {Function} params.getRootProps Returns the props you should apply to the root drop container you render\n   * @param {Function} params.getInputProps Returns the props you should apply to hidden file input you render\n   * @param {Function} params.open Open the native file selection dialog\n   * @param {boolean} params.isFocused Dropzone area is in focus\n   * @param {boolean} params.isFileDialogActive File dialog is opened\n   * @param {boolean} params.isDragActive Active drag is in progress\n   * @param {boolean} params.isDragAccept Dragged files are accepted\n   * @param {boolean} params.isDragReject Some dragged files are rejected\n   * @param {File[]} params.draggedFiles Files in active drag\n   * @param {File[]} params.acceptedFiles Accepted files\n   * @param {FileRejection[]} params.fileRejections Rejected files and why they were rejected\n   */\n  children: PropTypes.func,\n\n  /**\n   * Set accepted file types.\n   * See https://github.com/okonet/attr-accept for more information.\n   * Keep in mind that mime type determination is not reliable across platforms. CSV files,\n   * for example, are reported as text/plain under macOS but as application/vnd.ms-excel under\n   * Windows. In some cases there might not be a mime type set at all.\n   * See: https://github.com/react-dropzone/react-dropzone/issues/276\n   */\n  accept: PropTypes.oneOfType([PropTypes.string, PropTypes.arrayOf(PropTypes.string)]),\n\n  /**\n   * Allow drag 'n' drop (or selection from the file dialog) of multiple files\n   */\n  multiple: PropTypes.bool,\n\n  /**\n   * If false, allow dropped items to take over the current browser window\n   */\n  preventDropOnDocument: PropTypes.bool,\n\n  /**\n   * If true, disables click to open the native file selection dialog\n   */\n  noClick: PropTypes.bool,\n\n  /**\n   * If true, disables SPACE/ENTER to open the native file selection dialog.\n   * Note that it also stops tracking the focus state.\n   */\n  noKeyboard: PropTypes.bool,\n\n  /**\n   * If true, disables drag 'n' drop\n   */\n  noDrag: PropTypes.bool,\n\n  /**\n   * If true, stops drag event propagation to parents\n   */\n  noDragEventsBubbling: PropTypes.bool,\n\n  /**\n   * Minimum file size (in bytes)\n   */\n  minSize: PropTypes.number,\n\n  /**\n   * Maximum file size (in bytes)\n   */\n  maxSize: PropTypes.number,\n\n  /**\n   * Maximum accepted number of files\n   * The default value is 0 which means there is no limitation to how many files are accepted.\n   */\n  maxFiles: PropTypes.number,\n\n  /**\n   * Enable/disable the dropzone\n   */\n  disabled: PropTypes.bool,\n\n  /**\n   * Use this to provide a custom file aggregator\n   *\n   * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n   */\n  getFilesFromEvent: PropTypes.func,\n\n  /**\n   * Cb for when closing the file dialog with no selection\n   */\n  onFileDialogCancel: PropTypes.func,\n\n  /**\n   * Cb for when opening the file dialog\n   */\n  onFileDialogOpen: PropTypes.func,\n\n  /**\n   * Set to true to use the https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API\n   * to open the file picker instead of using an `<input type=\"file\">` click event.\n   */\n  useFsAccessApi: PropTypes.bool,\n\n  /**\n   * Cb for when the `dragenter` event occurs.\n   *\n   * @param {DragEvent} event\n   */\n  onDragEnter: PropTypes.func,\n\n  /**\n   * Cb for when the `dragleave` event occurs\n   *\n   * @param {DragEvent} event\n   */\n  onDragLeave: PropTypes.func,\n\n  /**\n   * Cb for when the `dragover` event occurs\n   *\n   * @param {DragEvent} event\n   */\n  onDragOver: PropTypes.func,\n\n  /**\n   * Cb for when the `drop` event occurs.\n   * Note that this callback is invoked after the `getFilesFromEvent` callback is done.\n   *\n   * Files are accepted or rejected based on the `accept`, `multiple`, `minSize` and `maxSize` props.\n   * `accept` must be a valid [MIME type](http://www.iana.org/assignments/media-types/media-types.xhtml) according to [input element specification](https://www.w3.org/wiki/HTML/Elements/input/file) or a valid file extension.\n   * If `multiple` is set to false and additional files are dropped,\n   * all files besides the first will be rejected.\n   * Any file which does not have a size in the [`minSize`, `maxSize`] range, will be rejected as well.\n   *\n   * Note that the `onDrop` callback will always be invoked regardless if the dropped files were accepted or rejected.\n   * If you'd like to react to a specific scenario, use the `onDropAccepted`/`onDropRejected` props.\n   *\n   * `onDrop` will provide you with an array of [File](https://developer.mozilla.org/en-US/docs/Web/API/File) objects which you can then process and send to a server.\n   * For example, with [SuperAgent](https://github.com/visionmedia/superagent) as a http/ajax library:\n   *\n   * ```js\n   * function onDrop(acceptedFiles) {\n   *   const req = request.post('/upload')\n   *   acceptedFiles.forEach(file => {\n   *     req.attach(file.name, file)\n   *   })\n   *   req.end(callback)\n   * }\n   * ```\n   *\n   * @param {File[]} acceptedFiles\n   * @param {FileRejection[]} fileRejections\n   * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n   */\n  onDrop: PropTypes.func,\n\n  /**\n   * Cb for when the `drop` event occurs.\n   * Note that if no files are accepted, this callback is not invoked.\n   *\n   * @param {File[]} files\n   * @param {(DragEvent|Event)} event\n   */\n  onDropAccepted: PropTypes.func,\n\n  /**\n   * Cb for when the `drop` event occurs.\n   * Note that if no files are rejected, this callback is not invoked.\n   *\n   * @param {FileRejection[]} fileRejections\n   * @param {(DragEvent|Event)} event\n   */\n  onDropRejected: PropTypes.func,\n\n  /**\n   * Custom validation function\n   * @param {File} file\n   * @returns {FileError|FileError[]}\n   */\n  validator: PropTypes.func\n};\nexport default Dropzone;\n/**\n * A function that is invoked for the `dragenter`,\n * `dragover` and `dragleave` events.\n * It is not invoked if the items are not files (such as link, text, etc.).\n *\n * @callback dragCb\n * @param {DragEvent} event\n */\n\n/**\n * A function that is invoked for the `drop` or input change event.\n * It is not invoked if the items are not files (such as link, text, etc.).\n *\n * @callback dropCb\n * @param {File[]} acceptedFiles List of accepted files\n * @param {FileRejection[]} fileRejections List of rejected files and why they were rejected\n * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n */\n\n/**\n * A function that is invoked for the `drop` or input change event.\n * It is not invoked if the items are files (such as link, text, etc.).\n *\n * @callback dropAcceptedCb\n * @param {File[]} files List of accepted files that meet the given criteria\n * (`accept`, `multiple`, `minSize`, `maxSize`)\n * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n */\n\n/**\n * A function that is invoked for the `drop` or input change event.\n *\n * @callback dropRejectedCb\n * @param {File[]} files List of rejected files that do not meet the given criteria\n * (`accept`, `multiple`, `minSize`, `maxSize`)\n * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n */\n\n/**\n * A function that is used aggregate files,\n * in a asynchronous fashion, from drag or input change events.\n *\n * @callback getFilesFromEvent\n * @param {(DragEvent|Event)} event A drag event or input change event (if files were selected via the file dialog)\n * @returns {(File[]|Promise<File[]>)}\n */\n\n/**\n * An object with the current dropzone state and some helper functions.\n *\n * @typedef {object} DropzoneState\n * @property {Function} getRootProps Returns the props you should apply to the root drop container you render\n * @property {Function} getInputProps Returns the props you should apply to hidden file input you render\n * @property {Function} open Open the native file selection dialog\n * @property {boolean} isFocused Dropzone area is in focus\n * @property {boolean} isFileDialogActive File dialog is opened\n * @property {boolean} isDragActive Active drag is in progress\n * @property {boolean} isDragAccept Dragged files are accepted\n * @property {boolean} isDragReject Some dragged files are rejected\n * @property {File[]} draggedFiles Files in active drag\n * @property {File[]} acceptedFiles Accepted files\n * @property {FileRejection[]} fileRejections Rejected files and why they were rejected\n */\n\nvar initialState = {\n  isFocused: false,\n  isFileDialogActive: false,\n  isDragActive: false,\n  isDragAccept: false,\n  isDragReject: false,\n  draggedFiles: [],\n  acceptedFiles: [],\n  fileRejections: []\n};\n/**\n * A React hook that creates a drag 'n' drop area.\n *\n * ```jsx\n * function MyDropzone(props) {\n *   const {getRootProps, getInputProps} = useDropzone({\n *     onDrop: acceptedFiles => {\n *       // do something with the File objects, e.g. upload to some server\n *     }\n *   });\n *   return (\n *     <div {...getRootProps()}>\n *       <input {...getInputProps()} />\n *       <p>Drag and drop some files here, or click to select files</p>\n *     </div>\n *   )\n * }\n * ```\n *\n * @function useDropzone\n *\n * @param {object} props\n * @param {string|string[]} [props.accept] Set accepted file types.\n * See https://github.com/okonet/attr-accept for more information.\n * Keep in mind that mime type determination is not reliable across platforms. CSV files,\n * for example, are reported as text/plain under macOS but as application/vnd.ms-excel under\n * Windows. In some cases there might not be a mime type set at all.\n * See: https://github.com/react-dropzone/react-dropzone/issues/276\n * @param {boolean} [props.multiple=true] Allow drag 'n' drop (or selection from the file dialog) of multiple files\n * @param {boolean} [props.preventDropOnDocument=true] If false, allow dropped items to take over the current browser window\n * @param {boolean} [props.noClick=false] If true, disables click to open the native file selection dialog\n * @param {boolean} [props.noKeyboard=false] If true, disables SPACE/ENTER to open the native file selection dialog.\n * Note that it also stops tracking the focus state.\n * @param {boolean} [props.noDrag=false] If true, disables drag 'n' drop\n * @param {boolean} [props.noDragEventsBubbling=false] If true, stops drag event propagation to parents\n * @param {number} [props.minSize=0] Minimum file size (in bytes)\n * @param {number} [props.maxSize=Infinity] Maximum file size (in bytes)\n * @param {boolean} [props.disabled=false] Enable/disable the dropzone\n * @param {getFilesFromEvent} [props.getFilesFromEvent] Use this to provide a custom file aggregator\n * @param {Function} [props.onFileDialogCancel] Cb for when closing the file dialog with no selection\n * @param {boolean} [props.useFsAccessApi] Set to true to use the https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API\n * to open the file picker instead of using an `<input type=\"file\">` click event.\n * @param {Function} [props.onFileDialogOpen] Cb for when opening the file dialog\n * @param {dragCb} [props.onDragEnter] Cb for when the `dragenter` event occurs.\n * @param {dragCb} [props.onDragLeave] Cb for when the `dragleave` event occurs\n * @param {dragCb} [props.onDragOver] Cb for when the `dragover` event occurs\n * @param {dropCb} [props.onDrop] Cb for when the `drop` event occurs.\n * Note that this callback is invoked after the `getFilesFromEvent` callback is done.\n *\n * Files are accepted or rejected based on the `accept`, `multiple`, `minSize` and `maxSize` props.\n * `accept` must be a valid [MIME type](http://www.iana.org/assignments/media-types/media-types.xhtml) according to [input element specification](https://www.w3.org/wiki/HTML/Elements/input/file) or a valid file extension.\n * If `multiple` is set to false and additional files are dropped,\n * all files besides the first will be rejected.\n * Any file which does not have a size in the [`minSize`, `maxSize`] range, will be rejected as well.\n *\n * Note that the `onDrop` callback will always be invoked regardless if the dropped files were accepted or rejected.\n * If you'd like to react to a specific scenario, use the `onDropAccepted`/`onDropRejected` props.\n *\n * `onDrop` will provide you with an array of [File](https://developer.mozilla.org/en-US/docs/Web/API/File) objects which you can then process and send to a server.\n * For example, with [SuperAgent](https://github.com/visionmedia/superagent) as a http/ajax library:\n *\n * ```js\n * function onDrop(acceptedFiles) {\n *   const req = request.post('/upload')\n *   acceptedFiles.forEach(file => {\n *     req.attach(file.name, file)\n *   })\n *   req.end(callback)\n * }\n * ```\n * @param {dropAcceptedCb} [props.onDropAccepted]\n * @param {dropRejectedCb} [props.onDropRejected]\n *\n * @returns {DropzoneState}\n */\n\nexport function useDropzone() {\n  var options = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};\n\n  var _defaultProps$options = _objectSpread(_objectSpread({}, defaultProps), options),\n      accept = _defaultProps$options.accept,\n      disabled = _defaultProps$options.disabled,\n      getFilesFromEvent = _defaultProps$options.getFilesFromEvent,\n      maxSize = _defaultProps$options.maxSize,\n      minSize = _defaultProps$options.minSize,\n      multiple = _defaultProps$options.multiple,\n      maxFiles = _defaultProps$options.maxFiles,\n      onDragEnter = _defaultProps$options.onDragEnter,\n      onDragLeave = _defaultProps$options.onDragLeave,\n      onDragOver = _defaultProps$options.onDragOver,\n      onDrop = _defaultProps$options.onDrop,\n      onDropAccepted = _defaultProps$options.onDropAccepted,\n      onDropRejected = _defaultProps$options.onDropRejected,\n      onFileDialogCancel = _defaultProps$options.onFileDialogCancel,\n      onFileDialogOpen = _defaultProps$options.onFileDialogOpen,\n      useFsAccessApi = _defaultProps$options.useFsAccessApi,\n      preventDropOnDocument = _defaultProps$options.preventDropOnDocument,\n      noClick = _defaultProps$options.noClick,\n      noKeyboard = _defaultProps$options.noKeyboard,\n      noDrag = _defaultProps$options.noDrag,\n      noDragEventsBubbling = _defaultProps$options.noDragEventsBubbling,\n      validator = _defaultProps$options.validator;\n\n  var onFileDialogOpenCb = useMemo(function () {\n    return typeof onFileDialogOpen === \"function\" ? onFileDialogOpen : noop;\n  }, [onFileDialogOpen]);\n  var onFileDialogCancelCb = useMemo(function () {\n    return typeof onFileDialogCancel === \"function\" ? onFileDialogCancel : noop;\n  }, [onFileDialogCancel]);\n  var rootRef = useRef(null);\n  var inputRef = useRef(null);\n\n  var _useReducer = useReducer(reducer, initialState),\n      _useReducer2 = _slicedToArray(_useReducer, 2),\n      state = _useReducer2[0],\n      dispatch = _useReducer2[1];\n\n  var isFocused = state.isFocused,\n      isFileDialogActive = state.isFileDialogActive,\n      draggedFiles = state.draggedFiles;\n  var fsAccessApiWorksRef = useRef(typeof window !== \"undefined\" && window.isSecureContext && useFsAccessApi && canUseFileSystemAccessAPI()); // Update file dialog active state when the window is focused on\n\n  var onWindowFocus = function onWindowFocus() {\n    // Execute the timeout only if the file dialog is opened in the browser\n    if (!fsAccessApiWorksRef.current && isFileDialogActive) {\n      setTimeout(function () {\n        if (inputRef.current) {\n          var files = inputRef.current.files;\n\n          if (!files.length) {\n            dispatch({\n              type: \"closeDialog\"\n            });\n            onFileDialogCancelCb();\n          }\n        }\n      }, 300);\n    }\n  };\n\n  useEffect(function () {\n    window.addEventListener(\"focus\", onWindowFocus, false);\n    return function () {\n      window.removeEventListener(\"focus\", onWindowFocus, false);\n    };\n  }, [inputRef, isFileDialogActive, onFileDialogCancelCb, fsAccessApiWorksRef]);\n  var dragTargetsRef = useRef([]);\n\n  var onDocumentDrop = function onDocumentDrop(event) {\n    if (rootRef.current && rootRef.current.contains(event.target)) {\n      // If we intercepted an event for our instance, let it propagate down to the instance's onDrop handler\n      return;\n    }\n\n    event.preventDefault();\n    dragTargetsRef.current = [];\n  };\n\n  useEffect(function () {\n    if (preventDropOnDocument) {\n      document.addEventListener(\"dragover\", onDocumentDragOver, false);\n      document.addEventListener(\"drop\", onDocumentDrop, false);\n    }\n\n    return function () {\n      if (preventDropOnDocument) {\n        document.removeEventListener(\"dragover\", onDocumentDragOver);\n        document.removeEventListener(\"drop\", onDocumentDrop);\n      }\n    };\n  }, [rootRef, preventDropOnDocument]);\n  var onDragEnterCb = useCallback(function (event) {\n    event.preventDefault(); // Persist here because we need the event later after getFilesFromEvent() is done\n\n    event.persist();\n    stopPropagation(event);\n    dragTargetsRef.current = [].concat(_toConsumableArray(dragTargetsRef.current), [event.target]);\n\n    if (isEvtWithFiles(event)) {\n      Promise.resolve(getFilesFromEvent(event)).then(function (draggedFiles) {\n        if (isPropagationStopped(event) && !noDragEventsBubbling) {\n          return;\n        }\n\n        dispatch({\n          draggedFiles: draggedFiles,\n          isDragActive: true,\n          type: \"setDraggedFiles\"\n        });\n\n        if (onDragEnter) {\n          onDragEnter(event);\n        }\n      });\n    }\n  }, [getFilesFromEvent, onDragEnter, noDragEventsBubbling]);\n  var onDragOverCb = useCallback(function (event) {\n    event.preventDefault();\n    event.persist();\n    stopPropagation(event);\n    var hasFiles = isEvtWithFiles(event);\n\n    if (hasFiles && event.dataTransfer) {\n      try {\n        event.dataTransfer.dropEffect = \"copy\";\n      } catch (_unused) {}\n      /* eslint-disable-line no-empty */\n\n    }\n\n    if (hasFiles && onDragOver) {\n      onDragOver(event);\n    }\n\n    return false;\n  }, [onDragOver, noDragEventsBubbling]);\n  var onDragLeaveCb = useCallback(function (event) {\n    event.preventDefault();\n    event.persist();\n    stopPropagation(event); // Only deactivate once the dropzone and all children have been left\n\n    var targets = dragTargetsRef.current.filter(function (target) {\n      return rootRef.current && rootRef.current.contains(target);\n    }); // Make sure to remove a target present multiple times only once\n    // (Firefox may fire dragenter/dragleave multiple times on the same element)\n\n    var targetIdx = targets.indexOf(event.target);\n\n    if (targetIdx !== -1) {\n      targets.splice(targetIdx, 1);\n    }\n\n    dragTargetsRef.current = targets;\n\n    if (targets.length > 0) {\n      return;\n    }\n\n    dispatch({\n      isDragActive: false,\n      type: \"setDraggedFiles\",\n      draggedFiles: []\n    });\n\n    if (isEvtWithFiles(event) && onDragLeave) {\n      onDragLeave(event);\n    }\n  }, [rootRef, onDragLeave, noDragEventsBubbling]);\n  var setFiles = useCallback(function (files, event) {\n    var acceptedFiles = [];\n    var fileRejections = [];\n    files.forEach(function (file) {\n      var _fileAccepted = fileAccepted(file, accept),\n          _fileAccepted2 = _slicedToArray(_fileAccepted, 2),\n          accepted = _fileAccepted2[0],\n          acceptError = _fileAccepted2[1];\n\n      var _fileMatchSize = fileMatchSize(file, minSize, maxSize),\n          _fileMatchSize2 = _slicedToArray(_fileMatchSize, 2),\n          sizeMatch = _fileMatchSize2[0],\n          sizeError = _fileMatchSize2[1];\n\n      var customErrors = validator ? validator(file) : null;\n\n      if (accepted && sizeMatch && !customErrors) {\n        acceptedFiles.push(file);\n      } else {\n        var errors = [acceptError, sizeError];\n\n        if (customErrors) {\n          errors = errors.concat(customErrors);\n        }\n\n        fileRejections.push({\n          file: file,\n          errors: errors.filter(function (e) {\n            return e;\n          })\n        });\n      }\n    });\n\n    if (!multiple && acceptedFiles.length > 1 || multiple && maxFiles >= 1 && acceptedFiles.length > maxFiles) {\n      // Reject everything and empty accepted files\n      acceptedFiles.forEach(function (file) {\n        fileRejections.push({\n          file: file,\n          errors: [TOO_MANY_FILES_REJECTION]\n        });\n      });\n      acceptedFiles.splice(0);\n    }\n\n    dispatch({\n      acceptedFiles: acceptedFiles,\n      fileRejections: fileRejections,\n      type: \"setFiles\"\n    });\n\n    if (onDrop) {\n      onDrop(acceptedFiles, fileRejections, event);\n    }\n\n    if (fileRejections.length > 0 && onDropRejected) {\n      onDropRejected(fileRejections, event);\n    }\n\n    if (acceptedFiles.length > 0 && onDropAccepted) {\n      onDropAccepted(acceptedFiles, event);\n    }\n  }, [dispatch, multiple, accept, minSize, maxSize, maxFiles, onDrop, onDropAccepted, onDropRejected, validator]);\n  var onDropCb = useCallback(function (event) {\n    event.preventDefault(); // Persist here because we need the event later after getFilesFromEvent() is done\n\n    event.persist();\n    stopPropagation(event);\n    dragTargetsRef.current = [];\n\n    if (isEvtWithFiles(event)) {\n      Promise.resolve(getFilesFromEvent(event)).then(function (files) {\n        if (isPropagationStopped(event) && !noDragEventsBubbling) {\n          return;\n        }\n\n        setFiles(files, event);\n      });\n    }\n\n    dispatch({\n      type: \"reset\"\n    });\n  }, [getFilesFromEvent, setFiles, noDragEventsBubbling]); // Fn for opening the file dialog programmatically\n\n  var openFileDialog = useCallback(function () {\n    // No point to use FS access APIs if context is not secure\n    // https://developer.mozilla.org/en-US/docs/Web/Security/Secure_Contexts#feature_detection\n    if (fsAccessApiWorksRef.current) {\n      dispatch({\n        type: \"openDialog\"\n      });\n      onFileDialogOpenCb(); // https://developer.mozilla.org/en-US/docs/Web/API/window/showOpenFilePicker\n\n      var opts = {\n        multiple: multiple,\n        types: filePickerOptionsTypes(accept)\n      };\n      window.showOpenFilePicker(opts).then(function (handles) {\n        return getFilesFromEvent(handles);\n      }).then(function (files) {\n        setFiles(files, null);\n        dispatch({\n          type: \"closeDialog\"\n        });\n      }).catch(function (e) {\n        // AbortError means the user canceled\n        if (isAbort(e)) {\n          onFileDialogCancelCb(e);\n          dispatch({\n            type: \"closeDialog\"\n          });\n        } else if (isSecurityError(e)) {\n          fsAccessApiWorksRef.current = false; // CORS, so cannot use this API\n          // Try using the input\n\n          if (inputRef.current) {\n            inputRef.current.value = null;\n            inputRef.current.click();\n          }\n        }\n      });\n      return;\n    }\n\n    if (inputRef.current) {\n      dispatch({\n        type: \"openDialog\"\n      });\n      onFileDialogOpenCb();\n      inputRef.current.value = null;\n      inputRef.current.click();\n    }\n  }, [dispatch, onFileDialogOpenCb, onFileDialogCancelCb, useFsAccessApi, setFiles, accept, multiple]); // Cb to open the file dialog when SPACE/ENTER occurs on the dropzone\n\n  var onKeyDownCb = useCallback(function (event) {\n    // Ignore keyboard events bubbling up the DOM tree\n    if (!rootRef.current || !rootRef.current.isEqualNode(event.target)) {\n      return;\n    }\n\n    if (event.key === \" \" || event.key === \"Enter\" || event.keyCode === 32 || event.keyCode === 13) {\n      event.preventDefault();\n      openFileDialog();\n    }\n  }, [rootRef, openFileDialog]); // Update focus state for the dropzone\n\n  var onFocusCb = useCallback(function () {\n    dispatch({\n      type: \"focus\"\n    });\n  }, []);\n  var onBlurCb = useCallback(function () {\n    dispatch({\n      type: \"blur\"\n    });\n  }, []); // Cb to open the file dialog when click occurs on the dropzone\n\n  var onClickCb = useCallback(function () {\n    if (noClick) {\n      return;\n    } // In IE11/Edge the file-browser dialog is blocking, therefore, use setTimeout()\n    // to ensure React can handle state changes\n    // See: https://github.com/react-dropzone/react-dropzone/issues/450\n\n\n    if (isIeOrEdge()) {\n      setTimeout(openFileDialog, 0);\n    } else {\n      openFileDialog();\n    }\n  }, [noClick, openFileDialog]);\n\n  var composeHandler = function composeHandler(fn) {\n    return disabled ? null : fn;\n  };\n\n  var composeKeyboardHandler = function composeKeyboardHandler(fn) {\n    return noKeyboard ? null : composeHandler(fn);\n  };\n\n  var composeDragHandler = function composeDragHandler(fn) {\n    return noDrag ? null : composeHandler(fn);\n  };\n\n  var stopPropagation = function stopPropagation(event) {\n    if (noDragEventsBubbling) {\n      event.stopPropagation();\n    }\n  };\n\n  var getRootProps = useMemo(function () {\n    return function () {\n      var _ref2 = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {},\n          _ref2$refKey = _ref2.refKey,\n          refKey = _ref2$refKey === void 0 ? \"ref\" : _ref2$refKey,\n          role = _ref2.role,\n          onKeyDown = _ref2.onKeyDown,\n          onFocus = _ref2.onFocus,\n          onBlur = _ref2.onBlur,\n          onClick = _ref2.onClick,\n          onDragEnter = _ref2.onDragEnter,\n          onDragOver = _ref2.onDragOver,\n          onDragLeave = _ref2.onDragLeave,\n          onDrop = _ref2.onDrop,\n          rest = _objectWithoutProperties(_ref2, _excluded3);\n\n      return _objectSpread(_objectSpread(_defineProperty({\n        onKeyDown: composeKeyboardHandler(composeEventHandlers(onKeyDown, onKeyDownCb)),\n        onFocus: composeKeyboardHandler(composeEventHandlers(onFocus, onFocusCb)),\n        onBlur: composeKeyboardHandler(composeEventHandlers(onBlur, onBlurCb)),\n        onClick: composeHandler(composeEventHandlers(onClick, onClickCb)),\n        onDragEnter: composeDragHandler(composeEventHandlers(onDragEnter, onDragEnterCb)),\n        onDragOver: composeDragHandler(composeEventHandlers(onDragOver, onDragOverCb)),\n        onDragLeave: composeDragHandler(composeEventHandlers(onDragLeave, onDragLeaveCb)),\n        onDrop: composeDragHandler(composeEventHandlers(onDrop, onDropCb)),\n        role: typeof role === \"string\" && role !== \"\" ? role : \"button\"\n      }, refKey, rootRef), !disabled && !noKeyboard ? {\n        tabIndex: 0\n      } : {}), rest);\n    };\n  }, [rootRef, onKeyDownCb, onFocusCb, onBlurCb, onClickCb, onDragEnterCb, onDragOverCb, onDragLeaveCb, onDropCb, noKeyboard, noDrag, disabled]);\n  var onInputElementClick = useCallback(function (event) {\n    event.stopPropagation();\n  }, []);\n  var getInputProps = useMemo(function () {\n    return function () {\n      var _ref3 = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {},\n          _ref3$refKey = _ref3.refKey,\n          refKey = _ref3$refKey === void 0 ? \"ref\" : _ref3$refKey,\n          onChange = _ref3.onChange,\n          onClick = _ref3.onClick,\n          rest = _objectWithoutProperties(_ref3, _excluded4);\n\n      var inputProps = _defineProperty({\n        accept: accept,\n        multiple: multiple,\n        type: \"file\",\n        style: {\n          display: \"none\"\n        },\n        onChange: composeHandler(composeEventHandlers(onChange, onDropCb)),\n        onClick: composeHandler(composeEventHandlers(onClick, onInputElementClick)),\n        tabIndex: -1\n      }, refKey, inputRef);\n\n      return _objectSpread(_objectSpread({}, inputProps), rest);\n    };\n  }, [inputRef, accept, multiple, onDropCb, disabled]);\n  var fileCount = draggedFiles.length;\n  var isDragAccept = fileCount > 0 && allFilesAccepted({\n    files: draggedFiles,\n    accept: accept,\n    minSize: minSize,\n    maxSize: maxSize,\n    multiple: multiple,\n    maxFiles: maxFiles\n  });\n  var isDragReject = fileCount > 0 && !isDragAccept;\n  return _objectSpread(_objectSpread({}, state), {}, {\n    isDragAccept: isDragAccept,\n    isDragReject: isDragReject,\n    isFocused: isFocused && !disabled,\n    getRootProps: getRootProps,\n    getInputProps: getInputProps,\n    rootRef: rootRef,\n    inputRef: inputRef,\n    open: composeHandler(openFileDialog)\n  });\n}\n\nfunction reducer(state, action) {\n  /* istanbul ignore next */\n  switch (action.type) {\n    case \"focus\":\n      return _objectSpread(_objectSpread({}, state), {}, {\n        isFocused: true\n      });\n\n    case \"blur\":\n      return _objectSpread(_objectSpread({}, state), {}, {\n        isFocused: false\n      });\n\n    case \"openDialog\":\n      return _objectSpread(_objectSpread({}, initialState), {}, {\n        isFileDialogActive: true\n      });\n\n    case \"closeDialog\":\n      return _objectSpread(_objectSpread({}, state), {}, {\n        isFileDialogActive: false\n      });\n\n    case \"setDraggedFiles\":\n      /* eslint no-case-declarations: 0 */\n      var isDragActive = action.isDragActive,\n          draggedFiles = action.draggedFiles;\n      return _objectSpread(_objectSpread({}, state), {}, {\n        draggedFiles: draggedFiles,\n        isDragActive: isDragActive\n      });\n\n    case \"setFiles\":\n      return _objectSpread(_objectSpread({}, state), {}, {\n        acceptedFiles: action.acceptedFiles,\n        fileRejections: action.fileRejections\n      });\n\n    case \"reset\":\n      return _objectSpread({}, initialState);\n\n    default:\n      return state;\n  }\n}\n\nfunction noop() {}\n\nexport { ErrorCode } from \"./utils\";",
         "import { useReducer, useRef, useDebugValue, useEffect, useLayoutEffect } from 'react';\n\nfunction createStore(createState) {\n  let state;\n  const listeners = /* @__PURE__ */ new Set();\n  const setState = (partial, replace) => {\n    const nextState = typeof partial === \"function\" ? partial(state) : partial;\n    if (nextState !== state) {\n      const previousState = state;\n      state = replace ? nextState : Object.assign({}, state, nextState);\n      listeners.forEach((listener) => listener(state, previousState));\n    }\n  };\n  const getState = () => state;\n  const subscribeWithSelector = (listener, selector = getState, equalityFn = Object.is) => {\n    console.warn(\"[DEPRECATED] Please use `subscribeWithSelector` middleware\");\n    let currentSlice = selector(state);\n    function listenerToAdd() {\n      const nextSlice = selector(state);\n      if (!equalityFn(currentSlice, nextSlice)) {\n        const previousSlice = currentSlice;\n        listener(currentSlice = nextSlice, previousSlice);\n      }\n    }\n    listeners.add(listenerToAdd);\n    return () => listeners.delete(listenerToAdd);\n  };\n  const subscribe = (listener, selector, equalityFn) => {\n    if (selector || equalityFn) {\n      return subscribeWithSelector(listener, selector, equalityFn);\n    }\n    listeners.add(listener);\n    return () => listeners.delete(listener);\n  };\n  const destroy = () => listeners.clear();\n  const api = { setState, getState, subscribe, destroy };\n  state = createState(setState, getState, api);\n  return api;\n}\n\nconst isSSR = typeof window === \"undefined\" || !window.navigator || /ServerSideRendering|^Deno\\//.test(window.navigator.userAgent);\nconst useIsomorphicLayoutEffect = isSSR ? useEffect : useLayoutEffect;\nfunction create(createState) {\n  const api = typeof createState === \"function\" ? createStore(createState) : createState;\n  const useStore = (selector = api.getState, equalityFn = Object.is) => {\n    const [, forceUpdate] = useReducer((c) => c + 1, 0);\n    const state = api.getState();\n    const stateRef = useRef(state);\n    const selectorRef = useRef(selector);\n    const equalityFnRef = useRef(equalityFn);\n    const erroredRef = useRef(false);\n    const currentSliceRef = useRef();\n    if (currentSliceRef.current === void 0) {\n      currentSliceRef.current = selector(state);\n    }\n    let newStateSlice;\n    let hasNewStateSlice = false;\n    if (stateRef.current !== state || selectorRef.current !== selector || equalityFnRef.current !== equalityFn || erroredRef.current) {\n      newStateSlice = selector(state);\n      hasNewStateSlice = !equalityFn(currentSliceRef.current, newStateSlice);\n    }\n    useIsomorphicLayoutEffect(() => {\n      if (hasNewStateSlice) {\n        currentSliceRef.current = newStateSlice;\n      }\n      stateRef.current = state;\n      selectorRef.current = selector;\n      equalityFnRef.current = equalityFn;\n      erroredRef.current = false;\n    });\n    const stateBeforeSubscriptionRef = useRef(state);\n    useIsomorphicLayoutEffect(() => {\n      const listener = () => {\n        try {\n          const nextState = api.getState();\n          const nextStateSlice = selectorRef.current(nextState);\n          if (!equalityFnRef.current(currentSliceRef.current, nextStateSlice)) {\n            stateRef.current = nextState;\n            currentSliceRef.current = nextStateSlice;\n            forceUpdate();\n          }\n        } catch (error) {\n          erroredRef.current = true;\n          forceUpdate();\n        }\n      };\n      const unsubscribe = api.subscribe(listener);\n      if (api.getState() !== stateBeforeSubscriptionRef.current) {\n        listener();\n      }\n      return unsubscribe;\n    }, []);\n    const sliceToReturn = hasNewStateSlice ? newStateSlice : currentSliceRef.current;\n    useDebugValue(sliceToReturn);\n    return sliceToReturn;\n  };\n  Object.assign(useStore, api);\n  useStore[Symbol.iterator] = function() {\n    console.warn(\"[useStore, api] = create() is deprecated and will be removed in v4\");\n    const items = [useStore, api];\n    return {\n      next() {\n        const done = items.length <= 0;\n        return { value: items.shift(), done };\n      }\n    };\n  };\n  return useStore;\n}\n\nexport { create as default };\n",
         "export default function(e,f){var a={white:\"#ffffff\",bisque:\"#ffe4c4\",blue:\"#0000ff\",cadetblue:\"#5f9ea0\",chartreuse:\"#7fff00\",chocolate:\"#d2691e\",coral:\"#ff7f50\",antiquewhite:\"#faebd7\",aqua:\"#00ffff\",azure:\"#f0ffff\",whitesmoke:\"#f5f5f5\",papayawhip:\"#ffefd5\",plum:\"#dda0dd\",blanchedalmond:\"#ffebcd\",black:\"#000000\",gold:\"#ffd700\",goldenrod:\"#daa520\",gainsboro:\"#dcdcdc\",cornsilk:\"#fff8dc\",cornflowerblue:\"#6495ed\",burlywood:\"#deb887\",aquamarine:\"#7fffd4\",beige:\"#f5f5dc\",crimson:\"#dc143c\",cyan:\"#00ffff\",darkblue:\"#00008b\",darkcyan:\"#008b8b\",darkgoldenrod:\"#b8860b\",darkkhaki:\"#bdb76b\",darkgray:\"#a9a9a9\",darkgreen:\"#006400\",darkgrey:\"#a9a9a9\",peachpuff:\"#ffdab9\",darkmagenta:\"#8b008b\",darkred:\"#8b0000\",darkorchid:\"#9932cc\",darkorange:\"#ff8c00\",darkslateblue:\"#483d8b\",gray:\"#808080\",darkslategray:\"#2f4f4f\",darkslategrey:\"#2f4f4f\",deeppink:\"#ff1493\",deepskyblue:\"#00bfff\",wheat:\"#f5deb3\",firebrick:\"#b22222\",floralwhite:\"#fffaf0\",ghostwhite:\"#f8f8ff\",darkviolet:\"#9400d3\",magenta:\"#ff00ff\",green:\"#008000\",dodgerblue:\"#1e90ff\",grey:\"#808080\",honeydew:\"#f0fff0\",hotpink:\"#ff69b4\",blueviolet:\"#8a2be2\",forestgreen:\"#228b22\",lawngreen:\"#7cfc00\",indianred:\"#cd5c5c\",indigo:\"#4b0082\",fuchsia:\"#ff00ff\",brown:\"#a52a2a\",maroon:\"#800000\",mediumblue:\"#0000cd\",lightcoral:\"#f08080\",darkturquoise:\"#00ced1\",lightcyan:\"#e0ffff\",ivory:\"#fffff0\",lightyellow:\"#ffffe0\",lightsalmon:\"#ffa07a\",lightseagreen:\"#20b2aa\",linen:\"#faf0e6\",mediumaquamarine:\"#66cdaa\",lemonchiffon:\"#fffacd\",lime:\"#00ff00\",khaki:\"#f0e68c\",mediumseagreen:\"#3cb371\",limegreen:\"#32cd32\",mediumspringgreen:\"#00fa9a\",lightskyblue:\"#87cefa\",lightblue:\"#add8e6\",midnightblue:\"#191970\",lightpink:\"#ffb6c1\",mistyrose:\"#ffe4e1\",moccasin:\"#ffe4b5\",mintcream:\"#f5fffa\",lightslategray:\"#778899\",lightslategrey:\"#778899\",navajowhite:\"#ffdead\",navy:\"#000080\",mediumvioletred:\"#c71585\",powderblue:\"#b0e0e6\",palegoldenrod:\"#eee8aa\",oldlace:\"#fdf5e6\",paleturquoise:\"#afeeee\",mediumturquoise:\"#48d1cc\",mediumorchid:\"#ba55d3\",rebeccapurple:\"#663399\",lightsteelblue:\"#b0c4de\",mediumslateblue:\"#7b68ee\",thistle:\"#d8bfd8\",tan:\"#d2b48c\",orchid:\"#da70d6\",mediumpurple:\"#9370db\",purple:\"#800080\",pink:\"#ffc0cb\",skyblue:\"#87ceeb\",springgreen:\"#00ff7f\",palegreen:\"#98fb98\",red:\"#ff0000\",yellow:\"#ffff00\",slateblue:\"#6a5acd\",lavenderblush:\"#fff0f5\",peru:\"#cd853f\",palevioletred:\"#db7093\",violet:\"#ee82ee\",teal:\"#008080\",slategray:\"#708090\",slategrey:\"#708090\",aliceblue:\"#f0f8ff\",darkseagreen:\"#8fbc8f\",darkolivegreen:\"#556b2f\",greenyellow:\"#adff2f\",seagreen:\"#2e8b57\",seashell:\"#fff5ee\",tomato:\"#ff6347\",silver:\"#c0c0c0\",sienna:\"#a0522d\",lavender:\"#e6e6fa\",lightgreen:\"#90ee90\",orange:\"#ffa500\",orangered:\"#ff4500\",steelblue:\"#4682b4\",royalblue:\"#4169e1\",turquoise:\"#40e0d0\",yellowgreen:\"#9acd32\",salmon:\"#fa8072\",saddlebrown:\"#8b4513\",sandybrown:\"#f4a460\",rosybrown:\"#bc8f8f\",darksalmon:\"#e9967a\",lightgoldenrodyellow:\"#fafad2\",snow:\"#fffafa\",lightgrey:\"#d3d3d3\",lightgray:\"#d3d3d3\",dimgray:\"#696969\",dimgrey:\"#696969\",olivedrab:\"#6b8e23\",olive:\"#808000\"},r={};for(var d in a)r[a[d]]=d;var l={};e.prototype.toName=function(f){if(!(this.rgba.a||this.rgba.r||this.rgba.g||this.rgba.b))return\"transparent\";var d,i,n=r[this.toHex()];if(n)return n;if(null==f?void 0:f.closest){var o=this.toRgb(),t=1/0,b=\"black\";if(!l.length)for(var c in a)l[c]=new e(a[c]).toRgb();for(var g in a){var u=(d=o,i=l[g],Math.pow(d.r-i.r,2)+Math.pow(d.g-i.g,2)+Math.pow(d.b-i.b,2));u<t&&(t=u,b=g)}return b}};f.string.push([function(f){var r=f.toLowerCase(),d=\"transparent\"===r?\"#0000\":a[r];return d?new e(d).toRgb():null},\"name\"])}\n",
         "export default {\n  disabled: false\n};",
         "export var forceReflow = function forceReflow(node) {\n  return node.scrollTop;\n};",
@@ -12187,11 +12187,11 @@
     ],
 }
```
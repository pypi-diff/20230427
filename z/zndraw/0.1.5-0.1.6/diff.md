# Comparing `tmp/zndraw-0.1.5.tar.gz` & `tmp/zndraw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.5.tar", max compression
+gzip compressed data, was "zndraw-0.1.6.tar", max compression
```

## Comparing `zndraw-0.1.5.tar` & `zndraw-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.5/LICENSE
--rw-r--r--   0        0        0     2020 2023-04-24 08:50:45.092660 zndraw-0.1.5/README.md
--rw-r--r--   0        0        0      834 2023-04-25 07:53:59.807276 zndraw-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      166 2023-04-21 17:52:18.309756 zndraw-0.1.5/zndraw/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-25 07:53:59.817276 zndraw-0.1.5/zndraw/analyse.py
--rw-r--r--   0        0        0     4682 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/app.py
--rw-r--r--   0        0        0     1659 2023-04-23 21:22:34.280010 zndraw-0.1.5/zndraw/cli.py
--rw-r--r--   0        0        0     2695 2023-04-24 08:50:45.102660 zndraw-0.1.5/zndraw/examples/__init__.py
--rw-r--r--   0        0        0     4278 2023-04-24 08:50:45.102660 zndraw-0.1.5/zndraw/globals.py
--rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.5/zndraw/io.py
--rw-r--r--   0        0        0      880 2023-04-21 17:52:18.319756 zndraw-0.1.5/zndraw/main.py
--rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.5/zndraw/static/favion-192x192.png
--rw-r--r--   0        0        0     3521 2023-04-23 21:22:34.290009 zndraw-0.1.5/zndraw/static/main.css
--rw-r--r--   0        0        0    20035 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/main.js
--rw-r--r--   0        0        0     2633 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/modules/data.js
--rw-r--r--   0        0        0     2893 2023-04-24 08:50:45.112660 zndraw-0.1.5/zndraw/static/modules/draw.js
--rw-r--r--   0        0        0     1009 2023-04-24 16:48:30.446942 zndraw-0.1.5/zndraw/static/modules/keypress.js
--rw-r--r--   0        0        0    11582 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/modules/particles.js
--rw-r--r--   0        0        0    15833 2023-04-25 09:20:10.142886 zndraw-0.1.5/zndraw/templates/index.html
--rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 zndraw-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2020 2023-04-24 08:50:45.092660 zndraw-0.1.6/README.md
+-rw-r--r--   0        0        0      834 2023-04-26 14:27:21.725760 zndraw-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-04-21 17:52:18.309756 zndraw-0.1.6/zndraw/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-25 07:53:59.817276 zndraw-0.1.6/zndraw/analyse.py
+-rw-r--r--   0        0        0     4682 2023-04-25 09:20:10.132886 zndraw-0.1.6/zndraw/app.py
+-rw-r--r--   0        0        0     2099 2023-04-26 12:45:50.160180 zndraw-0.1.6/zndraw/cli.py
+-rw-r--r--   0        0        0     2695 2023-04-24 08:50:45.102660 zndraw-0.1.6/zndraw/examples/__init__.py
+-rw-r--r--   0        0        0     4637 2023-04-26 11:24:00.222400 zndraw-0.1.6/zndraw/globals.py
+-rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.6/zndraw/io.py
+-rw-r--r--   0        0        0      880 2023-04-21 17:52:18.319756 zndraw-0.1.6/zndraw/main.py
+-rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.6/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     5011 2023-04-25 18:09:18.446738 zndraw-0.1.6/zndraw/static/main.css
+-rw-r--r--   0        0        0    20776 2023-04-26 13:30:15.711999 zndraw-0.1.6/zndraw/static/main.js
+-rw-r--r--   0        0        0     2980 2023-04-26 13:30:15.711999 zndraw-0.1.6/zndraw/static/modules/data.js
+-rw-r--r--   0        0        0     2893 2023-04-24 08:50:45.112660 zndraw-0.1.6/zndraw/static/modules/draw.js
+-rw-r--r--   0        0        0     1009 2023-04-24 16:48:30.446942 zndraw-0.1.6/zndraw/static/modules/keypress.js
+-rw-r--r--   0        0        0    11591 2023-04-26 13:30:15.711999 zndraw-0.1.6/zndraw/static/modules/particles.js
+-rw-r--r--   0        0        0    16172 2023-04-25 18:09:18.446738 zndraw-0.1.6/zndraw/templates/index.html
+-rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 zndraw-0.1.6/PKG-INFO
```

### Comparing `zndraw-0.1.5/LICENSE` & `zndraw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/README.md` & `zndraw-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/pyproject.toml` & `zndraw-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zndraw-0.1.5/zndraw/analyse.py` & `zndraw-0.1.6/zndraw/analyse.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/app.py` & `zndraw-0.1.6/zndraw/app.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/cli.py` & `zndraw-0.1.6/zndraw/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 @cli.command()
 def main(
     file: str = typer.Argument(..., help="Trajectory File"),
     port: int = typer.Option(None, help="Port to run the server on"),
     browser: bool = typer.Option(True, help="Open the browser automatically."),
     webview: bool = typer.Option(True, help="Use the webview library if available."),
     verbose: bool = typer.Option(False, help="Run the server in verbose mode."),
+    camera: str = typer.Option(
+        "PerspectiveCamera", help="Either PerspectiveCamera or OrthographicCamera"
+    ),
+    export: str = typer.Option(None, help="Export the scene to a file."),
 ):
     """ZnDraw: Visualize Molecules
 
     The ZnDraw CLI. Use 'zndraw version' to get the current version.
     """
     if not verbose:
         import logging
@@ -49,15 +53,21 @@
     if file == "version":
         version_callback()
 
     if not pathlib.Path(file).exists():
         typer.echo(f"File {file} does not exist.")
         raise typer.Exit()
 
-    globals.config = globals.Config(file=file)
+    if pathlib.Path(file).suffix == ".json":
+        globals.config = globals.Config.parse_file(file)
+    else:
+        globals.config = globals.Config(file=file, camera=camera)
+    if export is not None:
+        pathlib.Path(export).write_text(globals.config.json(indent=4))
+        return
     print(globals.config)
 
     if wv is not None and webview:
         wv.create_window("ZnDraw", app)
         with contextlib.suppress(wv.WebViewException):
             wv.start()
             return
```

### Comparing `zndraw-0.1.5/zndraw/examples/__init__.py` & `zndraw-0.1.6/zndraw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/globals.py` & `zndraw-0.1.6/zndraw/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import dataclasses
+import enum
 import importlib
 import pathlib
 import typing
 
 import ase.io
 import pydantic
 import tqdm
 import znh5md
 from pydantic import BaseModel, Field, PrivateAttr
 
 
+class CameraChoices(str, enum.Enum):
+    OrthographicCamera = "OrthographicCamera"
+    PerspectiveCamera = "PerspectiveCamera"
+
+
 class Config(BaseModel):
     file: str = Field(..., description="Trajectory File")
+    camera: CameraChoices = Field(
+        CameraChoices.PerspectiveCamera, description="Camera style"
+    )
     bond_size: float = Field(1.0, description="Bond Size")
     sphere_size: float = Field(1.0, description="Sphere Size")
     resolution: int = Field(10, description="Resolution")
     max_fps: int = Field(100, description="Maximum Frames Per Second")
     frames_per_post: int = Field(100, description="Frames per JS POST request")
     active_update_function: str = Field(None, description="Active Update Function")
     material: str = Field("MeshPhongMaterial", description="Material")
     antialias: bool = Field(True, description="Antialias")
+    continuous_loading: bool = Field(
+        True, description="Continuous Loading of the trajectory"
+    )
 
     _update_functions = PrivateAttr(default_factory=dict)
     _atoms_cache = PrivateAttr(default_factory=dict)
 
     def add_update_function(self, update_function) -> dict:
         """Add an update function to the config.
```

### Comparing `zndraw-0.1.5/zndraw/io.py` & `zndraw-0.1.6/zndraw/io.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/main.py` & `zndraw-0.1.6/zndraw/main.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/static/favion-192x192.png` & `zndraw-0.1.6/zndraw/static/favion-192x192.png`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/static/main.js` & `zndraw-0.1.6/zndraw/static/main.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -13,26 +13,24 @@
 
 
 // some global variables
 let selected_ids = [];
 let animation_frame = 0;
 let displayed_frame = 0;
 let scene_building = false;
-let animation_running = true;
+let animation_running = false;
 let fps = [];
 
 
 /**
  * DOM variables
  */
 
 const div_info = document.getElementById('info');
 const div_loading = document.getElementById('atom-spinner');
-const div_progressBar = document.getElementById('progressBar');
-const div_bufferBar = document.getElementById('bufferBar');
 const div_greyOut = document.getElementById('greyOut');
 const div_lst_selected_ids = document.getElementById('lst_selected_ids');
 const div_FPS = document.getElementById('FPS');
 const div_n_particles = document.getElementById('n_particles');
 const div_n_bonds = document.getElementById('n_bonds');
 
 const o_autoRestart = document.getElementById('autoRestart');
@@ -50,15 +48,29 @@
 
 
 // Helper Functions
 
 await DATA.load_config();
 // THREE JS Setup
 const scene = new THREE.Scene();
-const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
+
+function getCamera() {
+    let width = window.innerWidth;
+    let height = window.innerHeight;
+
+    if (DATA.config.camera == "PerspectiveCamera") {
+        return new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
+    } else {
+        return new THREE.OrthographicCamera(width / -2, width / 2, height / 2, height / -2, 1, 1000);
+    }
+}
+
+const camera = getCamera();
+camera.position.z = 50;
+
 const renderer = new THREE.WebGLRenderer({
     antialias: DATA.config["antialias"],
     alpha: true
 });
 
 const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
 const spotLight = new THREE.SpotLight(0xffffff, 0, 0, Math.PI / 2);
@@ -93,14 +105,15 @@
 // Setup Scene
 
 
 async function build_scene(step) {
     if (scene_building) {
         return;
     }
+    scene_building = true;
     console.log("Updating scene");
 
     div_loading.style.visibility = 'visible';
     div_greyOut.style.visibility = 'visible';
 
     animation_frame = step;
 
@@ -116,15 +129,14 @@
     });
 }
 
 build_scene(0);
 
 // interactions
 
-camera.position.z = 50;
 const controls = new OrbitControls(camera, renderer.domElement);
 
 controls.update();
 
 function onWindowResize() {
     camera.aspect = window.innerWidth / window.innerHeight
     camera.updateProjectionMatrix()
@@ -163,20 +175,20 @@
         } else {
             selected_ids = [mesh.userData["id"]];
         }
     } else {
         if (!selected_ids.includes(mesh.userData["id"])) {
             selected_ids.push(mesh.userData["id"]);
         } else {
-            mesh.material.color.set(mesh.userData["color"]);
             selected_ids.splice(selected_ids.indexOf(mesh.userData["id"]), 1);
         }
     }
     // update colors here for better performance
-    update_color_of_ids(selected_ids);
+    // TODO chain them
+    await update_color_of_ids(selected_ids);
     await update_selection();
 }
 
 /**
  * We update the color of every atom in the scene
  * @param {list[int]} ids, the selected ids
  * @returns 
@@ -220,18 +232,14 @@
         }
         div_lst_selected_ids.innerHTML = response_json["selected_ids"].join(", ");
     });
 
 }
 
 
-if (DATA.config["animate"] === true) {
-    div_info.innerHTML = "Reading file...";
-    DATA.getAnimationFrames();
-}
 if (DATA.config["restart_animation"] === true) {
     o_autoRestart.checked = true;
 }
 
 /**
  * Event listeners
  */
@@ -367,15 +375,15 @@
 function createRadioElement(id, properties) {
 
     let modifierCanvas = document.createElement('div');
     // modifierCanvas.classList.add("mb-3");
     modifierCanvas.classList.add("collapse", "show", "scene-modifier", "border", "border-primary", "rounded", "p-3");
     modifierCanvas.id = "sceneModifier_" + id;
 
-    console.log(properties);
+    console.log("Adding modifier: " + id);
 
     Object.values(properties).forEach((item) => {
         let controller = document.createElement('input');
         if (item["type"] == "integer") {
             controller.type = "range";
             controller.classList.add("form-range");
             controller.step = 1;
@@ -470,23 +478,19 @@
             alert(response_json["error"]);
             stepError(response_json["error"]);
         } else {
             if (document.getElementById("sceneModifier_" + response_json["title"]) != null) {
                 alert("Function already loaded");
                 stepError("Function already loaded");
             };
-
             addModifierModal.hide();
-
-            console.log(response_json);
             DATA.load_config();
         }
         return response_json;
     }).then(function(response_json) {
-        console.log(response_json);
         let modifier = document.createElement("option");
         modifier.value = response_json["title"];
         modifier.innerHTML = response_json["title"];
         addSceneModifier.appendChild(modifier);
         addSceneModifier.value = response_json["title"];
         return response_json;
     }).then(function(response_json) {
@@ -519,15 +523,17 @@
     if (event.isComposing || event.key === "ArrowUp") {
         animation_frame = parseInt(Math.min(DATA.frames.length - 1, animation_frame + (DATA.frames.length / 10)));
     }
     if (event.isComposing || event.key === "ArrowDown") {
         animation_frame = parseInt(Math.max(0, animation_frame - (DATA.frames.length / 10)));
     }
     if (event.isComposing || event.key === "q") {
-        DATA.getAnimationFrames();
+        DATA.resetAnimationFrames();
+        animation_frame = 0;
+        document.getElementById("frame-slider").value = 0;
     }
     if (event.isComposing || event.key === "i") {
         PARTICLES.printIndices(camera);
     };
 });
 
 
@@ -551,20 +557,17 @@
                 "Content-Type": "application/json"
             },
             "body": JSON.stringify({
                 "selected_ids": selected_ids,
                 "step": animation_frame,
                 "points": DRAW.positions
             }),
-        }).then((response) => {
-            if (DATA.frames.length > 0) {
-                DATA.spliceFrames(animation_frame + 1);
-            }
-            DATA.getAnimationFrames();
-        });
+        }).then(function(response) {
+            DATA.resetAnimationFrames(); // use DATA.spliceFrames(animation_frame + 1); ?
+        }).then(DATA.getAnimationFrames);
     }
 });
 
 // Drawing
 
 DRAW.init(camera, renderer, scene, controls)
 
@@ -599,51 +602,72 @@
     if (this.checked) {
         scene.add(PARTICLES.createBox(DATA.frames.box[animation_frame]));
     } else {
         scene.remove(PARTICLES.box);
     }
 };
 
+document.getElementById("continuousLoading").onclick = function() {
+    if (this.checked) {
+        fetch("config", {
+            "method": "POST",
+            "headers": {
+                "Content-Type": "application/json"
+            },
+            "body": JSON.stringify({
+                "continuous_loading": true
+            }),
+        }).then(DATA.load_config).then(DATA.getAnimationFrames);
+    } else {
+        fetch("config", {
+            "method": "POST",
+            "headers": {
+                "Content-Type": "application/json"
+            },
+            "body": JSON.stringify({
+                "continuous_loading": false
+            }),
+        }).then(DATA.load_config);
+    }
+};
+
+document.getElementById("frame-slider").oninput = function() {
+    if (this.value > DATA.frames.length - 1) {
+        this.value = DATA.frames.length - 1;
+    }
+    animation_frame = parseInt(this.value);
+};
 
 let move_atoms_clock = new THREE.Clock();
 
 
 function move_atoms() {
-    if (DATA.frames.length === 0) {
+    if (DATA.frames.length < animation_frame) {
         return;
     }
     if (move_atoms_clock.getElapsedTime() < (1 / o_max_fps.value)) {
         return;
     }
     if (scene_building === true) {
         return;
     }
-    div_progressBar.style.visibility = "hidden";
 
-    if (animation_running === true) {
-        if (animation_frame < DATA.frames.length - 1) {
-            animation_frame += 1;
-        } else if (o_autoRestart.checked === true) {
-            animation_frame = 0;
-        }
-    }
-    if (DATA.frames.length < animation_frame) {
-        // waiting for async call to finish
-        return;
-    }
-    if (DATA.config["total_frames"] > 0) {
-        div_progressBar.style.visibility = "visible";
-        div_progressBar.style.width = ((animation_frame / DATA.config["total_frames"]) * 100).toFixed(2) + "%";
-        div_bufferBar.style.width = (((DATA.frames.length - 1) / DATA.config["total_frames"]) * 100).toFixed(2) + "%";
-    }
-    if (DATA.frames.position[animation_frame].length != PARTICLES.particleGroup.children.length) {
-        // we need to update the scene
-        build_scene(animation_frame);
-        scene_building = true;
-        return; // we need to wait for the scene to be updated
+    document.getElementById("frame-slider").value = animation_frame;
+    document.getElementById("frame-slider").max = DATA.config["total_frames"];
+
+    try {
+        if (DATA.frames.position[animation_frame].length != PARTICLES.particleGroup.children.length) {
+            // we need to update the scene
+            console.log("Particle count changed from " + DATA.frames.position[animation_frame].length + " to " + PARTICLES.particleGroup.children.length + ", rebuilding scene");
+            build_scene(animation_frame);
+            return; // we need to wait for the scene to be updated
+        }
+    } catch (e) {
+        console.log("Scene not ready yet");
+        return; // scene is not ready yet
     }
 
     div_info.innerHTML = "Frame (" + animation_frame + "/" + (DATA.frames.length - 1) + ")";
 
     if (animation_frame != displayed_frame) {
         displayed_frame = animation_frame;
         PARTICLES.updateParticlePositions(DATA.frames.position[animation_frame]);
@@ -660,38 +684,41 @@
     }
     // if (!data_loading) {
     // 	DATA.getAnimationFrames();
     // }
 
     div_FPS.innerHTML = (1 / (fps.reduce((a, b) => a + b, 0) / fps.length)).toFixed(2);
     move_atoms_clock.start();
+    if (animation_running === true) {
+        if (animation_frame < DATA.frames.length - 1) {
+            animation_frame += 1;
+        } else if (o_autoRestart.checked === true) {
+            animation_frame = 0;
+        }
+    }
 }
 
 function centerCamera() {
     if (selected_ids.length === 0) {
         controls.target = PARTICLES.getAtomsCenter([...Array(PARTICLES.particleGroup.children.length).keys()]);
     } else {
         controls.target = PARTICLES.getAtomsCenter(selected_ids);
     }
 }
 
-/**
- * Dynamic indices
- * 
- */
+div_info.innerHTML = "Reading file...";
+DATA.getAnimationFrames();
 
 // scene.add(PARTICLES.arrowGroup);
 function animate() {
 
     renderer.render(scene, camera);
     controls.update();
 
-    if (DATA.frames.length > 0) {
-        move_atoms();
-    }
+    move_atoms();
     if (keydown["c"]) {
         centerCamera();
     }
     if (keydown["l"]) {
         spotLight.position.x = camera.position.x;
         spotLight.position.y = camera.position.y;
         spotLight.position.z = camera.position.z;
```

### Comparing `zndraw-0.1.5/zndraw/static/modules/data.js` & `zndraw-0.1.6/zndraw/static/modules/data.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -61,25 +61,28 @@
             }), // TODO keep configurable
         }).then(response => response.json()).then(function(response_json) {
             load_config();
             return response_json;
         });
 
         console.log("Read " + step + "-" + (frames_per_post + step) + " frames");
-        if (Object.keys(obj).length === 0) {
-            console.log("Animation read finished");
-            break;
+        if (obj["position"].length === 0) {
+            if (!config["continuous_loading"]) {
+                console.log("Animation read finished");
+                break;
+            } else {
+                console.log("Continuous Loading: waiting for new frames");
+            }
         }
         frames.position = frames.position.concat(obj["position"]);
         frames.box = frames.box.concat(obj["box"]);
         // frames.force = frames.force.concat(obj["force"]);
         frames.length = frames.position.length;
 
-        step += frames_per_post;
-        step = Math.min(step, frames.length);
+        step = frames.length;
     }
     data_loading = false;
 }
 
 export async function getRebuildCache(step) {
     let arrayOfResponses = [];
     if (rebuild_cache.hasOwnProperty(step)) {
@@ -94,18 +97,29 @@
                 "Content-Type": "application/json"
             },
             "body": JSON.stringify(step)
         })).json();
         rebuild_cache[step] = arrayOfResponses;
     }
     await load_config();
-    if (step === 0) {
+    if ((step === 0) && (frames.position.length === 0)) {
         let positions = [];
         for (let i = 0; i < arrayOfResponses["nodes"].length; i++) {
             positions.push(arrayOfResponses["nodes"][i]["position"]);
         }
         frames.position = [positions];
         frames.box = [arrayOfResponses["box"]];
         frames.length = frames.position.length;
     }
     return arrayOfResponses;
+}
+
+export function resetAnimationFrames() {
+    console.log("Resetting animation frames")
+    frames.position = [];
+    frames.force = [];
+    frames.length = 0;
+    frames.box = [];
+    rebuild_cache = {};
+    getRebuildCache(0);
+    getAnimationFrames();
 }
```

### Comparing `zndraw-0.1.5/zndraw/static/modules/draw.js` & `zndraw-0.1.6/zndraw/static/modules/draw.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/static/modules/keypress.js` & `zndraw-0.1.6/zndraw/static/modules/keypress.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.5/zndraw/static/modules/particles.js` & `zndraw-0.1.6/zndraw/static/modules/particles.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -216,17 +216,17 @@
     return center;
 }
 
 // TODO rename clean AtomsBonds
 // this does not remove the scene!
 // TODO add setup function that loads the scene inside this module
 export function cleanScene(scene) {
-    speciesMaterialFactoryCache = {};
-    sphereGeometryFactoryCache = {};
-    halfCylinderGeometryFactoryCache = {};
+    // speciesMaterialFactoryCache = {};
+    // sphereGeometryFactoryCache = {};
+    // halfCylinderGeometryFactoryCache = {};
 
     while (particleGroup.children.length > 0) {
         scene.remove(particleGroup.children.shift());
     };
 
     while (arrowGroup.children.length > 0) {
         scene.remove(arrowGroup.children.shift());
```

### Comparing `zndraw-0.1.5/zndraw/templates/index.html` & `zndraw-0.1.6/zndraw/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,21 @@
       <div class="mb-3">
         <input class="form-check-input" type="checkbox" value="" id="autoRestart">
         <label class="form-check-label" for="autoRestart">
           Auto Restart
         </label>
       </div>
       <div class="mb-3">
+        <input class="form-check-input" type="checkbox" value="" id="continuousLoading" {{ "checked" if
+          config['continuous_loading'] }}>
+        <label class="form-check-label" for="continuousLoading">
+          Continuous Loading of new data.
+        </label>
+      </div>
+      <div class="mb-3">
         <input class="form-check-input" type="checkbox" value="" id="showBox">
         <label for="showBox" class="form-label">Show Box (static)</label>
       </div>
       <div class="mb-3">
         <button type="button" class="btn btn-secondary" id="reset">Reset Scene</button>
         <button type="button" class="btn btn-secondary" id="animate" {% if config.update_function %} disabled {% endif
           %}>Load Animation</button>
@@ -341,13 +348,12 @@
         </div>
       </div>
     </div>
   </div>
 
   <!-- Progress Bar -->
   <div id="info"></div>
-  <div id="progressBar"></div>
-  <div id="bufferBar"></div>
+  <input id="frame-slider" class="frame-slider" type="range" value="0" min="0" max="100">
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -32,14 +32,16 @@
 ** Scene **
 Camera light intensity: 1.0 [Unknown INPUT type]
 Spot light intensity: 0.0 [Unknown INPUT type]
 Hemisphere light intensity: 1.0 [Unknown INPUT type]
 Max FPS: {{ config.max_fps }}
  oninput="max_fpsLabel.innerHTML = 'Max FPS: ' + this.value">
 ⁰  Auto Restart
+{ "checked" if config['continuous_loading'] }}>  Continuous Loading of new
+data.
 ⁰ Show Box (static)
 Reset Scene
 % if config.update_function %} disabled {% endif %}>Load Animation
 ** Draw **
 Add anchor point Remove Line
 ** Analyse **
 Get distance
@@ -63,7 +65,8 @@
       keydown shift
   show particle index
       keydown I
 ** Add Scene Modifier **
 Path to modifier class [Unknown INPUT type]
 The input should be module.cls such that from module import cls works.
 Close Load
+[Unknown INPUT type]
```

### Comparing `zndraw-0.1.5/PKG-INFO` & `zndraw-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/balanna-0.5.tar.gz` & `tmp/balanna-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanna-0.5.tar", last modified: Tue Mar 14 09:20:44 2023, max compression
+gzip compressed data, was "balanna-1.0.tar", last modified: Thu Apr 27 13:23:12 2023, max compression
```

## Comparing `balanna-0.5.tar` & `balanna-1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-03-14 09:20:44.632685 balanna-0.5/
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-02-28 12:47:14.000000 balanna-0.5/LICENSE
--rw-r--r--   0 sas      (23222) tumuser  (20909)      223 2023-03-14 09:20:44.632685 balanna-0.5/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      432 2023-03-08 14:07:10.000000 balanna-0.5/README.md
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-03-14 09:20:44.620685 balanna-0.5/balanna/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      163 2023-03-14 09:19:18.000000 balanna-0.5/balanna/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-03-13 13:08:04.000000 balanna-0.5/balanna/camera_trajectories.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    18984 2023-03-14 09:19:18.000000 balanna-0.5/balanna/display_scenes.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-03-13 13:08:04.000000 balanna-0.5/balanna/trimesh.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-03-14 09:20:44.632685 balanna-0.5/balanna/utils/
--rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-02-28 12:47:14.000000 balanna-0.5/balanna/utils/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-02-28 12:47:14.000000 balanna-0.5/balanna/utils/geometry.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-03-14 09:20:44.628685 balanna-0.5/balanna.egg-info/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      223 2023-03-14 09:20:44.000000 balanna-0.5/balanna.egg-info/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      338 2023-03-14 09:20:44.000000 balanna-0.5/balanna.egg-info/SOURCES.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-03-14 09:20:44.000000 balanna-0.5/balanna.egg-info/dependency_links.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-03-14 09:20:44.000000 balanna-0.5/balanna.egg-info/requires.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-03-14 09:20:44.000000 balanna-0.5/balanna.egg-info/top_level.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-03-14 09:20:44.636685 balanna-0.5/setup.cfg
--rw-r--r--   0 sas      (23222) tumuser  (20909)      471 2023-03-14 09:20:34.000000 balanna-0.5/setup.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.097470 balanna-1.0/
+-rw-r--r--   0 sele       (501) staff       (20)     1070 2023-04-27 11:14:03.000000 balanna-1.0/LICENSE
+-rw-r--r--   0 sele       (501) staff       (20)      245 2023-04-27 13:23:12.097623 balanna-1.0/PKG-INFO
+-rw-r--r--   0 sele       (501) staff       (20)      517 2023-04-27 11:17:40.000000 balanna-1.0/README.md
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.092117 balanna-1.0/balanna/
+-rw-r--r--   0 sele       (501) staff       (20)      540 2023-04-27 13:14:38.000000 balanna-1.0/balanna/__init__.py
+-rw-r--r--   0 sele       (501) staff       (20)     1095 2023-04-27 13:14:38.000000 balanna-1.0/balanna/__main__.py
+-rw-r--r--   0 sele       (501) staff       (20)     1581 2023-04-27 11:14:03.000000 balanna-1.0/balanna/camera_trajectories.py
+-rw-r--r--   0 sele       (501) staff       (20)    10078 2023-04-27 11:14:03.000000 balanna-1.0/balanna/trimesh.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.096621 balanna-1.0/balanna/utils/
+-rw-r--r--   0 sele       (501) staff       (20)       30 2023-04-27 11:14:03.000000 balanna-1.0/balanna/utils/__init__.py
+-rw-r--r--   0 sele       (501) staff       (20)      559 2023-04-27 11:14:03.000000 balanna-1.0/balanna/utils/geometry.py
+-rw-r--r--   0 sele       (501) staff       (20)    15330 2023-04-27 12:54:01.000000 balanna-1.0/balanna/window_base.py
+-rw-r--r--   0 sele       (501) staff       (20)     4645 2023-04-27 13:16:24.000000 balanna-1.0/balanna/window_dataset.py
+-rw-r--r--   0 sele       (501) staff       (20)     4593 2023-04-27 12:57:38.000000 balanna-1.0/balanna/window_generator.py
+-rw-r--r--   0 sele       (501) staff       (20)     7265 2023-04-27 12:58:33.000000 balanna-1.0/balanna/window_real_time.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.094874 balanna-1.0/balanna.egg-info/
+-rw-r--r--   0 sele       (501) staff       (20)      245 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/PKG-INFO
+-rw-r--r--   0 sele       (501) staff       (20)      437 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/SOURCES.txt
+-rw-r--r--   0 sele       (501) staff       (20)        1 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/dependency_links.txt
+-rw-r--r--   0 sele       (501) staff       (20)       56 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/requires.txt
+-rw-r--r--   0 sele       (501) staff       (20)        8 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/top_level.txt
+-rw-r--r--   0 sele       (501) staff       (20)      103 2023-04-27 13:23:12.098296 balanna-1.0/setup.cfg
+-rw-r--r--   0 sele       (501) staff       (20)      493 2023-04-27 13:17:06.000000 balanna-1.0/setup.py
```

### Comparing `balanna-0.5/LICENSE` & `balanna-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balanna-0.5/balanna/camera_trajectories.py` & `balanna-1.0/balanna/camera_trajectories.py`

 * *Files identical despite different names*

### Comparing `balanna-0.5/balanna/display_scenes.py` & `balanna-1.0/balanna/window_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,35 +5,40 @@
 import packaging.version
 import pathlib
 import trimesh.path.entities
 import trimesh.visual
 import trimesh.viewer
 import time
 import vedo
+import vtk
+
+import matplotlib
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from matplotlib.backends.backend_qtagg import (
+    FigureCanvasQTAgg as FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 
 from functools import partial
-from PIL import Image, ImageQt
+from PIL import Image
 from PyQt5 import Qt
-from PyQt5.QtCore import QObject, QThread, pyqtSignal
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from vtk.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
-
-
-__all__ = ['display_scenes', 'display_real_time', 'RealTimeNode']
+from vtk.util.numpy_support import numpy_to_vtk
 
 
 SceneDictType = Dict[str, Any]
 
 
 class MainWindow(Qt.QMainWindow):
 
     def __init__(
         self,
         image_keys: List[str],
         scene_keys: List[str],
+        figure_keys: List[str],
         video_directory: Optional[Union[pathlib.Path, str]] = None,
         horizontal: bool = True,
         show_labels: bool = False,
         use_scene_cam: bool = False,
         debug: bool = False,
         parent: Qt.QWidget = None
     ):
@@ -76,31 +81,49 @@
             vp.add_callback('MouseWheelBackward', partial(self.__align_event, align_id=scene_id))
             vp.add_callback('KeyPress', self._on_key)
             vp.show()
             self.vtkWidgets.append(vtk_widget)
             self.vps.append(vp)
         vl.addLayout(vl2)
 
+        vl3 = Qt.QVBoxLayout()
+        self.figure_key_dict = {key: i for i, key in enumerate(figure_keys)}
+        self.figureCanvas = []
+        for _ in figure_keys:
+            figure_canvas = FigureCanvas(Figure())
+            self.figureCanvas.append(figure_canvas)
+            #vl3.addWidget(NavigationToolbar(figure_canvas, self))
+            vl3.addWidget(figure_canvas)
+        vl.addLayout(vl3)
+
         # Set up mouse timer for synchronizing mouse interactions across multiple (3D) widgets.
         # Therefore, the interaction is detected, tracked and transferred to all other 3D widgets.
         self._mouse_timer = Qt.QTimer(self)
         self._mouse_timer.timeout.connect(self.__align_event)  # noqa
         self._current_align_id = None
 
         frame.setLayout(vl)
         self.setCentralWidget(frame)
+        # If image and scene keys are displayed, somehow the scene widgets start with zero width.
+        # Therefore, resize the window before startup by multiplying the current size with the
+        # number of scene widgets.
+        if len(image_keys) > 0 and len(scene_keys) > 0:
+            w = self.size().width() + self.size().width() * len(scene_keys)
+            h = self.size().height()
+            self.resize(w, h)
         self.show()
 
         # Set up video directory for storing screenshots.
         self.video_directory = None
         self.__video_index = 0
         if video_directory is not None:
             self.video_directory = pathlib.Path(video_directory)
             if self.video_directory.exists():
                 print("\033[93m" + "Video directory already exists, overwriting it ..." + "\033[0m")
+            self.video_directory.mkdir(exist_ok=True, parents=True)
 
     def render_(self, scene_dict: SceneDictType, resetcam: bool = False):
         start_time = time.perf_counter()
 
         for key, element in scene_dict.items():
             if isinstance(element, trimesh.Scene) and key in self.scene_key_dict:
                 at = self.scene_key_dict[key]
@@ -110,15 +133,51 @@
                         m_vedo = vedo.trimesh2vedo(m)
                         if m.visual.kind == "vertex":
                             face_colors = trimesh.visual.color.vertex_to_face_color(m.visual.vertex_colors, m.faces)
                             m_vedo.cellIndividualColors(face_colors)
                         meshes_vedo.append(m_vedo)
 
                     elif isinstance(m, trimesh.PointCloud):
-                        m_vedo = vedo.Points(m.vertices, c=m.visual.vertex_colors)
+                        vertices = m.vertices
+                        vertex_colors = m.visual.vertex_colors
+                        n, _ = vertices.shape
+
+                        # vedo.Points uses vtk.vtkPolyData() as backend data storage and thus converts
+                        # the input to this type. However, the vedo conversion is quite inefficient, therefore
+                        # we convert the trimesh.PointCloud before passing it to vedo.
+                        # partially from https://github.com/pyvista/utilities/helpers.py
+                        vtkpts = vtk.vtkPoints()
+                        vtk_arr = numpy_to_vtk(vertices, deep=True)
+                        vtkpts.SetData(vtk_arr)
+                        pd = vtk.vtkPolyData()
+                        pd.SetPoints(vtkpts)
+
+                        # For some reason, vedo requires each vtk.vtkPolyData object to set an internal
+                        # cell array, as it uses the vertices, not the points attribute. As a point cloud
+                        # is unconnected, the offset and connectivity is just the index of the respective point.
+                        carr = vtk.vtkCellArray()
+                        carr.SetData(vedo.numpy2vtk(np.arange(n + 1), dtype="int"),  # offset
+                                     vedo.numpy2vtk(np.arange(n), dtype="int"))  # connectivity
+                        pd.SetVerts(carr)
+
+                        # Set vertex color RGB/RGBA values as active scalar property of the vtk.vtkPolyData.
+                        if vertex_colors.shape[1] == 3:
+                            ucols = numpy_to_vtk(vertex_colors)
+                            ucols.SetName("Points_RGB")
+                            pd.GetPointData().AddArray(ucols)
+                            pd.GetPointData().SetActiveScalars("Points_RGB")
+                        elif vertex_colors.shape[1] == 4:
+                            ucols = numpy_to_vtk(vertex_colors)
+                            ucols.SetName("Points_RGBA")
+                            pd.GetPointData().AddArray(ucols)
+                            pd.GetPointData().SetActiveScalars("Points_RGBA")
+                        else:
+                            print("\033[93m" + f"Invalid point cloud colors, skipping ..." + "\033[0m")
+
+                        m_vedo = vedo.Points(pd)
                         meshes_vedo.append(m_vedo)
 
                     elif isinstance(m, trimesh.path.Path3D):
                         # The trimesh path consists of entities and vertices. The vertices are the 3D points,
                         # that are connected as described in the entities.
                         if not all([isinstance(me, trimesh.path.entities.Line) for me in m.entities]):
                             raise ValueError("Currently only trimesh.path.entities.Line entities are supported")
@@ -152,26 +211,39 @@
                     camera_dict = dict(pos=cam_0, focal_point=cam_1, viewup=view_up)
 
                 self.vps[at].clear()
                 self.vps[at].show(meshes_vedo, bg="white", resetcam=resetcam, camera=camera_dict)
 
             elif isinstance(element, np.ndarray) and key in self.image_widge_dict:
                 if len(element.shape) == 3:
-                    image_mode = "RGB"
-                    element = np.transpose(element, (1, 2, 0))  # (C, H, W) -> (H, W, C)
+                    if element.shape[0] == 3:
+                        element = np.transpose(element, (1, 2, 0))  # (C, H, W) -> (H, W, C)
                 else:
-                    image_mode = "L"
-                img = Image.fromarray(element, mode=image_mode)
-                qt_img = ImageQt.ImageQt(img)
+                    element = np.stack([element] * 3, axis=-1)
+                height, width, _ = element.shape
+                qt_img = Qt.QImage(element.data.tobytes(), width, height, 3 * width, Qt.QImage.Format_RGB888)
                 self.image_widge_dict[key].setPixmap(Qt.QPixmap.fromImage(qt_img))
 
             elif isinstance(element, str):
                 print(f"{key}: {element}")
 
+            elif isinstance(element, Axes) and key in self.figure_key_dict:
+                at = self.figure_key_dict[key]
+                # have to use this width/height to adjust the size of the axis somehow
+                width, height = self.figureCanvas[at].get_width_height()
+                # clear figure
+                self.figureCanvas[at].figure.clf()
+                # set new references of axes element
+                element.figure = self.figureCanvas[at].figure
+                self.figureCanvas[at].figure.add_axes(element)
+                # draw figure to update!
+                self.figureCanvas[at].draw()
+
             else:
+                print("\033[93m" + f"Invalid element in scene dict of type {type(element)}, skipping ..." + "\033[0m")
                 continue
 
         if self.debug:
             dt = int((time.perf_counter() - start_time) * 1000)  # secs -> milliseconds
             print("\033[36m" + f"Rendering time: {dt} ms" + "\033[0m")
 
         if self.video_directory is not None:
@@ -185,14 +257,23 @@
             align_id = self._current_align_id
 
         camera = self.vps[align_id].camera
         for k in range(self.num_scenes):
             self.vps[k].renderer.SetActiveCamera(camera)
             self.vps[k].render()
 
+    def keyPressEvent(self, event):
+        """In case the Qt key callback is called, convert the Qt event to a string key and call the _on_key() method.
+        However, this case will only occur if the window contains no vedo panel. Thus, duplicated calling of
+        the key callback is not an issue.
+        """
+        event_dict = {"keyPressed": chr(event.key()).lower()}
+        self._on_key(event_dict)
+        event.accept()
+
     def _on_key(self, event_dict) -> None:
         key_pressed = event_dict["keyPressed"]
         if key_pressed == "z":
             if self.num_scenes > 0:
                 self.vps[0].render(resetcam=True)
                 self.__align_event(align_id=0)
         elif key_pressed == "k":
@@ -224,15 +305,15 @@
         image_paths = []
 
         # Store the images from the widget's pixmaps, store them and add them to
         # the list of screenshot files.
         for key, widget in self.image_widge_dict.items():
             path = directory / key / f"{prefix}.png"
             path.parent.mkdir(parents=True, exist_ok=True)
-            widget.pixmap().toImage().save(path)
+            widget.pixmap().toImage().save(path.as_posix())
             image_paths.append(path)
 
         # Make screenshots of all trimesh scenes, store them and add them to
         # the list of screenshot files.
         for key, widget in self.scene_key_dict.items():
             path = directory / key / f"{prefix}.png"
             path.parent.mkdir(parents=True, exist_ok=True)
@@ -253,258 +334,7 @@
     @property
     def num_images(self) -> int:
         return len(self.image_widge_dict)
 
     @property
     def num_scenes(self) -> int:
         return len(self.vps)
-
-
-class MainWindowDataset(MainWindow):
-
-    def __init__(
-        self,
-        scene_iterator: Iterable[SceneDictType],
-        fps: float,
-        video_directory: Optional[Union[pathlib.Path, str]] = None,
-        horizontal: bool = True,
-        loop: bool = True,
-        show_labels: bool = False,
-        use_scene_cam: bool = False,
-        debug: bool = False,
-        parent: Qt.QWidget = None
-    ):
-        self.scene_iterator = scene_iterator
-        self.fps = fps
-        scene_dict = self.get_next_scene_dict()
-        if scene_dict is None:
-            return
-
-        image_keys = [key for key, value in scene_dict.items() if isinstance(value, np.ndarray)]
-        scene_keys = [key for key, value in scene_dict.items() if isinstance(value, trimesh.Scene)]
-        super(MainWindowDataset, self).__init__(
-            image_keys=image_keys,
-            scene_keys=scene_keys,
-            video_directory=video_directory,
-            horizontal=horizontal,
-            show_labels=show_labels,
-            use_scene_cam=use_scene_cam,
-            debug=debug,
-            parent=parent
-        )
-
-        self.render_(scene_dict, resetcam=True)
-
-        # Setup looping timer and connect it to render a new scene at every timer callback.
-        # If loop is true, start looping right away.
-        self.timer = Qt.QTimer(self)
-        self.timer.timeout.connect(self.render_next_scene)  # noqa
-        if loop:
-            self.toggle_looping()
-
-    def render_next_scene(self, resetcam: bool = False) -> None:
-        scene_dict = self.get_next_scene_dict()
-        if scene_dict is not None:
-            self.render_(scene_dict, resetcam=resetcam)
-        elif self.timer.isActive():
-            self.timer.stop()
-
-    def _on_key(self, event_dict) -> None:
-        super(MainWindowDataset, self)._on_key(event_dict)
-        key_pressed = event_dict["keyPressed"]
-        if key_pressed == "s":
-            self.toggle_looping()
-        elif key_pressed == "n":
-            self.render_next_scene()
-
-    @staticmethod
-    def print_usage():
-        MainWindow.print_usage()
-        print("\ts: play / pause",
-              "\n\tn: next")
-
-    def get_next_scene_dict(self) -> Optional[SceneDictType]:
-        try:
-            return next(self.scene_iterator)  # noqa
-        except StopIteration:
-            return None
-
-    def toggle_looping(self):
-        if self.timer.isActive():
-            self.timer.stop()
-        else:
-            self.timer.start(int(1 / self.fps * 1000))  # in milliseconds
-
-
-class RealTimeNode(QObject):
-    """Template class for real time rendering.
-
-    Examples:
-        class DemoNode(RealTimeNode):
-
-            def callback(self):
-                scene = trimesh.Scene()
-                box_mesh = trimesh.creation.box(bounds=[(-1, -1, 0), (1, 1, 1)])
-                scene.add_geometry(box_mesh)
-                self.render({"scene": scene})
-
-                if condition:
-                    self.close()
-    """
-    finished = pyqtSignal()
-    running = pyqtSignal()
-    scene_dict_emitter = pyqtSignal(dict)
-
-    def callback(self):
-        raise NotImplementedError
-
-    def run(self):
-        while True:
-            if not self.running:
-                continue
-            self.callback()
-
-    def render(self, scene_dict: SceneDictType):
-        self.scene_dict_emitter.emit(scene_dict)  # noqa
-
-    def close(self):
-        self.finished.emit()  # noqa
-
-
-class MainWindowRealTime(MainWindow):
-
-    def __init__(
-        self,
-        worker: QObject,
-        image_keys: List[str],
-        scene_keys: List[str],
-        video_directory: Optional[Union[pathlib.Path, str]] = None,
-        horizontal: bool = True,
-        show_labels: bool = False,
-        use_scene_cam: bool = False,
-        debug: bool = False,
-        parent: Qt.QWidget = None
-    ):
-        super(MainWindowRealTime, self).__init__(
-            image_keys=image_keys,
-            scene_keys=scene_keys,
-            video_directory=video_directory,
-            horizontal=horizontal,
-            show_labels=show_labels,
-            use_scene_cam=use_scene_cam,
-            debug=debug,
-            parent=parent
-        )
-
-        # Set up multi-processing pipeline.
-        self.thread = QThread()
-        self.worker = worker
-        self.worker.moveToThread(self.thread)
-        self.thread.started.connect(self.worker.run)
-        self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.worker.scene_dict_emitter.connect(self.render_)
-        self.thread.start()
-
-        self.show()
-
-    def _on_key(self, event_dict) -> None:
-        super(MainWindowRealTime, self)._on_key(event_dict)
-        key_pressed = event_dict["keyPressed"]
-        if key_pressed == "s":
-            self.worker.running = not self.worker.running
-
-    @staticmethod
-    def print_usage():
-        MainWindow.print_usage()
-        print("\ts: play / pause")
-
-
-def display_scenes(
-    scene_iterator: Iterable[SceneDictType],
-    horizontal: bool = True,
-    loop: bool = False,
-    fps: float = 30.0,
-    video_directory: Optional[pathlib.Path] = None,
-    show_labels: bool = False,
-    use_scene_cam: bool = False,
-    debug: bool = False
-):
-    """Display scenes stored in scene iterator as PyQt app.
-
-    The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
-    Currently, images (np.array), 3D scenes (trimesh.Scene) and strings (for prinout) are supported.
-
-    Args:
-        scene_iterator: iterator function to get the scene dictionaries.
-        horizontal: window orientation, horizontal or vertical stacking.
-        loop: start looping from beginning.
-        fps: frames (i.e. scenes) per second for looping.
-        video_directory: directory for storing screenshots.
-        show_labels: display the scene dict keys.
-        use_scene_cam: use camera transform from trimesh scenes.
-        debug: printing debug information.
-    """
-    app = Qt.QApplication([])
-    window = MainWindowDataset(
-        scene_iterator=scene_iterator,
-        fps=fps,
-        video_directory=video_directory,
-        horizontal=horizontal,
-        loop=loop,
-        show_labels=show_labels,
-        debug=debug,
-        use_scene_cam=use_scene_cam
-    )
-    app.aboutToQuit.connect(window.on_close)
-    app.exec_()
-
-
-def display_real_time(
-    worker: RealTimeNode,
-    image_keys: Optional[List[str]] = None,
-    scene_keys: Optional[List[str]] = None,
-    horizontal: bool = True,
-    video_directory: Optional[pathlib.Path] = None,
-    show_labels: bool = False,
-    use_scene_cam: bool = False,
-    debug: bool = False
-):
-    """Display scenes from a real-time application, i.e. render in-coming scenes directly.
-
-    The worker is a process that generates each new scene in a separate thread and passes it to the renderer.
-    For a smooth rendering process and for simplification, the image and scene keys have to be known in advances
-    and cannot be changed afterwards.
-
-    Args:
-        worker: generator of new scenes.
-        image_keys: names of images in rendered dictionary.
-        scene_keys: names of 3D scenes in rendered dictionary.
-        horizontal: window orientation, horizontal or vertical stacking.
-        video_directory: directory for storing screenshots.
-        show_labels: display the scene dict keys.
-        use_scene_cam: use camera transform from trimesh scenes.
-        debug: printing debug information.
-    """
-    if image_keys is None and scene_keys is None:
-        raise ValueError("Neither image nor scene keys, provide at least one key!")
-    if not hasattr(worker, 'run'):
-        raise ValueError("Worker must have method run()")
-    if image_keys is None:
-        image_keys = []
-    if scene_keys is None:
-        scene_keys = []
-
-    app = Qt.QApplication([])
-    window = MainWindowRealTime(
-        worker=worker,
-        image_keys=image_keys,
-        scene_keys=scene_keys,
-        video_directory=video_directory,
-        horizontal=horizontal,
-        show_labels=show_labels,
-        use_scene_cam=use_scene_cam,
-        debug=debug
-    )
-    app.aboutToQuit.connect(window.on_close)
-    app.exec_()
```

### Comparing `balanna-0.5/balanna/trimesh.py` & `balanna-1.0/balanna/trimesh.py`

 * *Files identical despite different names*

### Comparing `balanna-0.5/balanna/utils/geometry.py` & `balanna-1.0/balanna/utils/geometry.py`

 * *Files identical despite different names*


# Comparing `tmp/panda_gym-3.0.5.tar.gz` & `tmp/panda_gym-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_gym-3.0.5.tar", last modified: Sat Mar 18 10:27:05 2023, max compression
+gzip compressed data, was "panda_gym-3.0.6.tar", last modified: Thu Apr 27 08:56:10 2023, max compression
```

## Comparing `panda_gym-3.0.5.tar` & `panda_gym-3.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.207322 panda_gym-3.0.5/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     1075 2021-10-12 17:31:44.000000 panda_gym-3.0.5/LICENSE
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3891 2023-03-18 10:27:05.207142 panda_gym-3.0.5/PKG-INFO
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3291 2023-01-02 15:40:01.000000 panda_gym-3.0.5/README.md
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.202715 panda_gym-3.0.5/panda_gym/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     1821 2022-10-19 15:32:25.000000 panda_gym-3.0.5/panda_gym/__init__.py
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.203489 panda_gym-3.0.5/panda_gym/assets/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)      104 2021-11-24 13:21:10.000000 panda_gym-3.0.5/panda_gym/assets/__init__.py
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.204308 panda_gym-3.0.5/panda_gym/envs/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)      162 2023-01-23 15:31:17.000000 panda_gym-3.0.5/panda_gym/envs/__init__.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)    11724 2023-03-18 10:04:26.000000 panda_gym-3.0.5/panda_gym/envs/core.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)    14044 2023-03-18 10:04:26.000000 panda_gym-3.0.5/panda_gym/envs/panda_tasks.py
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.204619 panda_gym-3.0.5/panda_gym/envs/robots/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)        0 2022-01-28 13:40:33.000000 panda_gym-3.0.5/panda_gym/envs/robots/__init__.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     6321 2023-03-18 10:04:26.000000 panda_gym-3.0.5/panda_gym/envs/robots/panda.py
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.206837 panda_gym-3.0.5/panda_gym/envs/tasks/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)        0 2022-01-28 13:40:33.000000 panda_gym-3.0.5/panda_gym/envs/tasks/__init__.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3747 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/flip.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3985 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/pick_and_place.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3904 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/push.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     2302 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/reach.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     4067 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/slide.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     5730 2023-01-02 17:03:24.000000 panda_gym-3.0.5/panda_gym/envs/tasks/stack.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)    26817 2023-03-18 10:04:26.000000 panda_gym-3.0.5/panda_gym/pybullet.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)      800 2022-10-19 15:32:25.000000 panda_gym-3.0.5/panda_gym/utils.py
--rw-r--r--   0 quentingallouedec   (501) staff       (20)        5 2023-03-18 10:15:11.000000 panda_gym-3.0.5/panda_gym/version.txt
-drwxr-xr-x   0 quentingallouedec   (501) staff       (20)        0 2023-03-18 10:27:05.203360 panda_gym-3.0.5/panda_gym.egg-info/
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     3891 2023-03-18 10:27:05.000000 panda_gym-3.0.5/panda_gym.egg-info/PKG-INFO
--rw-r--r--   0 quentingallouedec   (501) staff       (20)      669 2023-03-18 10:27:05.000000 panda_gym-3.0.5/panda_gym.egg-info/SOURCES.txt
--rw-r--r--   0 quentingallouedec   (501) staff       (20)        1 2023-03-18 10:27:05.000000 panda_gym-3.0.5/panda_gym.egg-info/dependency_links.txt
--rw-r--r--   0 quentingallouedec   (501) staff       (20)      102 2023-03-18 10:27:05.000000 panda_gym-3.0.5/panda_gym.egg-info/requires.txt
--rw-r--r--   0 quentingallouedec   (501) staff       (20)       10 2023-03-18 10:27:05.000000 panda_gym-3.0.5/panda_gym.egg-info/top_level.txt
--rw-r--r--   0 quentingallouedec   (501) staff       (20)       38 2023-03-18 10:27:05.207367 panda_gym-3.0.5/setup.cfg
--rw-r--r--   0 quentingallouedec   (501) staff       (20)     1195 2023-03-18 10:04:40.000000 panda_gym-3.0.5/setup.py
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.811579 panda_gym-3.0.6/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1075 2023-04-27 07:54:06.000000 panda_gym-3.0.6/LICENSE
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3928 2023-04-27 08:56:10.807579 panda_gym-3.0.6/PKG-INFO
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3291 2023-04-27 07:54:06.000000 panda_gym-3.0.6/README.md
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1821 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/__init__.py
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/assets/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      104 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/assets/__init__.py
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      162 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/__init__.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    12094 2023-04-27 08:35:37.000000 panda_gym-3.0.6/panda_gym/envs/core.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    14044 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/panda_tasks.py
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/robots/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/robots/__init__.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     6321 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/robots/panda.py
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym/envs/tasks/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/envs/tasks/__init__.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3647 2023-04-27 08:34:57.000000 panda_gym-3.0.6/panda_gym/envs/tasks/flip.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3885 2023-04-27 08:35:00.000000 panda_gym-3.0.6/panda_gym/envs/tasks/pick_and_place.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3804 2023-04-27 08:35:03.000000 panda_gym-3.0.6/panda_gym/envs/tasks/push.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     2202 2023-04-27 08:35:07.000000 panda_gym-3.0.6/panda_gym/envs/tasks/reach.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3967 2023-04-27 08:35:10.000000 panda_gym-3.0.6/panda_gym/envs/tasks/slide.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     5630 2023-04-27 08:35:14.000000 panda_gym-3.0.6/panda_gym/envs/tasks/stack.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)    26817 2023-04-27 08:30:08.000000 panda_gym-3.0.6/panda_gym/pybullet.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      800 2023-04-27 07:54:06.000000 panda_gym-3.0.6/panda_gym/utils.py
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        5 2023-04-27 08:42:08.000000 panda_gym-3.0.6/panda_gym/version.txt
+drwxrwxr-x   0 qgallouedec  (1000) qgallouedec  (1000)        0 2023-04-27 08:56:10.807579 panda_gym-3.0.6/panda_gym.egg-info/
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     3928 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/PKG-INFO
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      669 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/SOURCES.txt
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)        1 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/dependency_links.txt
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)      102 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/requires.txt
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)       10 2023-04-27 08:56:10.000000 panda_gym-3.0.6/panda_gym.egg-info/top_level.txt
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)       38 2023-04-27 08:56:10.811579 panda_gym-3.0.6/setup.cfg
+-rw-rw-r--   0 qgallouedec  (1000) qgallouedec  (1000)     1195 2023-04-27 07:54:06.000000 panda_gym-3.0.6/setup.py
```

### Comparing `panda_gym-3.0.5/LICENSE` & `panda_gym-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/PKG-INFO` & `panda_gym-3.0.6/panda_gym.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: panda_gym
-Version: 3.0.5
+Name: panda-gym
+Version: 3.0.6
 Summary: Set of robotic environments based on PyBullet physics engine and gymnasium.
 Home-page: https://github.com/qgallouedec/panda-gym
 Author: Quentin GALLOUÉDEC
 Author-email: gallouedec.quentin@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -92,7 +94,9 @@
   author       = {Gallou{\'e}dec, Quentin and Cazin, Nicolas and Dellandr{\'e}a, Emmanuel and Chen, Liming},
   year         = 2021,
   journal      = {4th Robot Learning Workshop: Self-Supervised and Lifelong Learning at NeurIPS},
 }
 ```
 
 Environments are widely inspired from [OpenAI Fetch environments](https://openai.com/blog/ingredients-for-robotics-research/). 
+
+
```

### Comparing `panda_gym-3.0.5/README.md` & `panda_gym-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym/__init__.py` & `panda_gym-3.0.6/panda_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym/envs/core.py` & `panda_gym-3.0.6/panda_gym/envs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,19 +243,28 @@
         )
         self.action_space = self.robot.action_space
         self.compute_reward = self.task.compute_reward
         self._saved_goal = dict()  # For state saving and restoring
 
         self.render_width = render_width
         self.render_height = render_height
-        self.render_target_position = render_target_position
+        self.render_target_position = (
+            render_target_position if render_target_position is not None else np.array([0.0, 0.0, 0.0])
+        )
         self.render_distance = render_distance
         self.render_yaw = render_yaw
         self.render_pitch = render_pitch
         self.render_roll = render_roll
+        with self.sim.no_rendering():
+            self.sim.place_visualizer(
+                target_position=self.render_target_position,
+                distance=self.render_distance,
+                yaw=self.render_yaw,
+                pitch=self.render_pitch,
+            )
 
     def _get_obs(self) -> Dict[str, np.ndarray]:
         robot_obs = self.robot.get_obs().astype(np.float32)  # robot state
         task_obs = self.task.get_obs().astype(np.float32)  # object position, velococity, etc...
         observation = np.concatenate([robot_obs, task_obs])
         achieved_goal = self.task.get_achieved_goal().astype(np.float32)
         return {
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/panda_tasks.py` & `panda_gym-3.0.6/panda_gym/envs/panda_tasks.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym/envs/robots/panda.py` & `panda_gym-3.0.6/panda_gym/envs/robots/panda.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/flip.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/flip.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self.reward_type = reward_type
         self.distance_threshold = distance_threshold
         self.object_size = 0.04
         self.obj_range_low = np.array([-obj_xy_range / 2, -obj_xy_range / 2, 0])
         self.obj_range_high = np.array([obj_xy_range / 2, obj_xy_range / 2, 0])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         """Create the scene."""
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.1, width=0.7, height=0.4, x_offset=-0.3)
         self.sim.create_box(
             body_name="object",
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/pick_and_place.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/pick_and_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self.object_size = 0.04
         self.goal_range_low = np.array([-goal_xy_range / 2, -goal_xy_range / 2, 0])
         self.goal_range_high = np.array([goal_xy_range / 2, goal_xy_range / 2, goal_z_range])
         self.obj_range_low = np.array([-obj_xy_range / 2, -obj_xy_range / 2, 0])
         self.obj_range_high = np.array([obj_xy_range / 2, obj_xy_range / 2, 0])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         """Create the scene."""
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.1, width=0.7, height=0.4, x_offset=-0.3)
         self.sim.create_box(
             body_name="object",
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/push.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         self.object_size = 0.04
         self.goal_range_low = np.array([-goal_xy_range / 2, -goal_xy_range / 2, 0])
         self.goal_range_high = np.array([goal_xy_range / 2, goal_xy_range / 2, 0])
         self.obj_range_low = np.array([-obj_xy_range / 2, -obj_xy_range / 2, 0])
         self.obj_range_high = np.array([obj_xy_range / 2, obj_xy_range / 2, 0])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.1, width=0.7, height=0.4, x_offset=-0.3)
         self.sim.create_box(
             body_name="object",
             half_extents=np.ones(3) * self.object_size / 2,
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/reach.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/reach.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.reward_type = reward_type
         self.distance_threshold = distance_threshold
         self.get_ee_position = get_ee_position
         self.goal_range_low = np.array([-goal_range / 2, -goal_range / 2, 0])
         self.goal_range_high = np.array([goal_range / 2, goal_range / 2, goal_range])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.1, width=0.7, height=0.4, x_offset=-0.3)
         self.sim.create_sphere(
             body_name="target",
             radius=0.02,
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/slide.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         self.object_size = 0.06
         self.goal_range_low = np.array([-goal_xy_range / 2 + goal_x_offset, -goal_xy_range / 2, 0])
         self.goal_range_high = np.array([goal_xy_range / 2 + goal_x_offset, goal_xy_range / 2, 0])
         self.obj_range_low = np.array([-obj_xy_range / 2, -obj_xy_range / 2, 0])
         self.obj_range_high = np.array([obj_xy_range / 2, obj_xy_range / 2, 0])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.4, width=0.7, height=0.4, x_offset=-0.1)
         self.sim.create_cylinder(
             body_name="object",
             mass=1.0,
```

### Comparing `panda_gym-3.0.5/panda_gym/envs/tasks/stack.py` & `panda_gym-3.0.6/panda_gym/envs/tasks/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         self.object_size = 0.04
         self.goal_range_low = np.array([-goal_xy_range / 2, -goal_xy_range / 2, 0])
         self.goal_range_high = np.array([goal_xy_range / 2, goal_xy_range / 2, 0])
         self.obj_range_low = np.array([-obj_xy_range / 2, -obj_xy_range / 2, 0])
         self.obj_range_high = np.array([obj_xy_range / 2, obj_xy_range / 2, 0])
         with self.sim.no_rendering():
             self._create_scene()
-            self.sim.place_visualizer(target_position=np.zeros(3), distance=0.9, yaw=45, pitch=-30)
 
     def _create_scene(self) -> None:
         self.sim.create_plane(z_offset=-0.4)
         self.sim.create_table(length=1.1, width=0.7, height=0.4, x_offset=-0.3)
         self.sim.create_box(
             body_name="object1",
             half_extents=np.ones(3) * self.object_size / 2,
```

### Comparing `panda_gym-3.0.5/panda_gym/pybullet.py` & `panda_gym-3.0.6/panda_gym/pybullet.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym/utils.py` & `panda_gym-3.0.6/panda_gym/utils.py`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/panda_gym.egg-info/PKG-INFO` & `panda_gym-3.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: panda-gym
-Version: 3.0.5
+Name: panda_gym
+Version: 3.0.6
 Summary: Set of robotic environments based on PyBullet physics engine and gymnasium.
 Home-page: https://github.com/qgallouedec/panda-gym
 Author: Quentin GALLOUÉDEC
 Author-email: gallouedec.quentin@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -92,7 +94,9 @@
   author       = {Gallou{\'e}dec, Quentin and Cazin, Nicolas and Dellandr{\'e}a, Emmanuel and Chen, Liming},
   year         = 2021,
   journal      = {4th Robot Learning Workshop: Self-Supervised and Lifelong Learning at NeurIPS},
 }
 ```
 
 Environments are widely inspired from [OpenAI Fetch environments](https://openai.com/blog/ingredients-for-robotics-research/). 
+
+
```

### Comparing `panda_gym-3.0.5/panda_gym.egg-info/SOURCES.txt` & `panda_gym-3.0.6/panda_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_gym-3.0.5/setup.py` & `panda_gym-3.0.6/setup.py`

 * *Files identical despite different names*


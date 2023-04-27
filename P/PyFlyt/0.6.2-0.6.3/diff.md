# Comparing `tmp/PyFlyt-0.6.2.tar.gz` & `tmp/PyFlyt-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.6.2.tar", last modified: Mon Apr 24 12:08:52 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.3.tar", last modified: Thu Apr 27 19:27:00 2023, max compression
```

## Comparing `PyFlyt-0.6.2.tar` & `PyFlyt-0.6.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.954846 PyFlyt-0.6.2/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.2/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     8847 2023-04-24 12:08:52.954846 PyFlyt-0.6.2/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.942846 PyFlyt-0.6.2/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.2/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.942846 PyFlyt-0.6.2/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.2/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.946846 PyFlyt-0.6.2/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-23 00:11:20.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4277 2023-04-12 15:03:07.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7239 2023-04-23 20:15:04.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15014 2023-04-12 15:29:07.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.2/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15536 2023-04-23 00:13:01.000000 PyFlyt-0.6.2/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.946846 PyFlyt-0.6.2/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.2/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.2/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    17954 2023-04-12 14:34:19.000000 PyFlyt-0.6.2/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11506 2023-04-12 14:34:51.000000 PyFlyt-0.6.2/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.2/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.946846 PyFlyt-0.6.2/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.946846 PyFlyt-0.6.2/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.946846 PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.2/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.2/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.2/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.2/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.942846 PyFlyt-0.6.2/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.950846 PyFlyt-0.6.2/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.2/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.942846 PyFlyt-0.6.2/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8847 2023-04-24 12:08:52.000000 PyFlyt-0.6.2/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-24 12:08:52.000000 PyFlyt-0.6.2/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-24 12:08:52.000000 PyFlyt-0.6.2/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       36 2023-04-24 12:08:52.000000 PyFlyt-0.6.2/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-24 12:08:52.000000 PyFlyt-0.6.2/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1154 2023-04-24 12:08:47.000000 PyFlyt-0.6.2/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     7030 2023-04-12 17:54:58.000000 PyFlyt-0.6.2/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-24 12:08:52.954846 PyFlyt-0.6.2/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.2/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-24 12:08:52.954846 PyFlyt-0.6.2/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.2/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.2/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.3/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.3/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-23 00:11:20.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4277 2023-04-12 15:03:07.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15014 2023-04-12 15:29:07.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15536 2023-04-23 00:13:01.000000 PyFlyt-0.6.3/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.3/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.3/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11598 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.3/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.3/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.3/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-04-27 19:26:54.000000 PyFlyt-0.6.3/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.3/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.3/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.3/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.6.2/LICENSE.txt` & `PyFlyt-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/gimbals.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,25 +149,30 @@
             gimbal_command <= 1.0
         ), f"`{gimbal_command=} has values out of bounds of -1.0 and 1.0.`"
 
         # model the gimbal using first order ODE, y' = T/tau * (setpoint - y)
         self.gimbal_state += (self.physics_period / self.gimbal_tau) * (
             gimbal_command - self.gimbal_state
         )
+
+        # precompute some things
+        gimbal_angles = np.expand_dims(
+            self.gimbal_state * self.gimbal_range_radians, axis=(-1, -2)
+        )
+        sin_angles = np.sin(gimbal_angles)
+        sin_half_angles = np.sin(gimbal_angles / 2.0)
+
         # start calculating rotation matrices
         # https://math.stackexchange.com/questions/142821/matrix-for-rotation-around-a-vector
-        sin_angles = np.expand_dims(
-            np.sin(self.gimbal_state * self.gimbal_range_radians), axis=(-1, -2)
-        )
         rotation1 = (
             np.eye(3)
             + sin_angles[:, 0, ...] * self.w1
-            + 2 * (sin_angles[:, 0, ...] ** 2) * self.w1_squared
+            + 2 * (sin_half_angles[:, 0, ...] ** 2) * self.w1_squared
         )
         rotation2 = (
             np.eye(3)
             + sin_angles[:, 1, ...] * self.w2
-            + 2 * (sin_angles[:, 1, ...] ** 2) * self.w2_squared
+            + 2 * (sin_half_angles[:, 1, ...] ** 2) * self.w2_squared
         )
 
         # get the final thrust vector
         return rotation1 @ rotation2
```

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.3/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/aviary.py` & `PyFlyt-0.6.3/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.3/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.3/PyFlyt/core/drones/quadx.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,31 +195,32 @@
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.disable_artificial_damping()
         self.motors.reset()
 
     def set_mode(self, mode: int):
         """Sets the current flight mode of the vehicle.
 
-        sets the flight mode:
-           -1 - m1, m2, m3, m4
-            0 - vp, vq, vr, T
-            1 - p, q, r, vz
-            2 - vp, vq, vr, z
-            3 - p, q, r, z
-            4 - u, v, vr, z
-            5 - u, v, vr, vz
-            6 - vx, vy, vr, vz
-            7 - x, y, r, z
+        flight modes:
+            - -1: m1, m2, m3, m4
+            - 0: vp, vq, vr, T
+            - 1: p, q, r, vz
+            - 2: vp, vq, vr, z
+            - 3: p, q, r, z
+            - 4: u, v, vr, z
+            - 5: u, v, vr, vz
+            - 6: vx, vy, vr, vz
+            - 7: x, y, r, z
 
-        vp, vq, vr = angular velocities
-        p, q, r = angular positions
-        u, v, w = local linear velocities
-        x, y, z = linear positions
-        vx, vy, vz = ground linear velocities
-        T = thrust
+        breakdown:
+            - vp, vq, vr = angular velocities
+            - p, q, r = angular positions
+            - u, v, w = local linear velocities
+            - x, y, z = linear positions
+            - vx, vy, vz = ground linear velocities
+            - T = thrust
 
         Args:
             mode (int): flight mode
 
         """
         if (mode < -1 or mode > 7) and mode not in self.registered_controllers.keys():
             raise ValueError(
```

### Comparing `PyFlyt-0.6.2/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.3/PyFlyt/core/drones/rocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,25 @@
 from ..abstractions.boring_bodies import BoringBodies
 from ..abstractions.camera import Camera
 from ..abstractions.gimbals import Gimbals
 from ..abstractions.lifting_surfaces import LiftingSurface, LiftingSurfaces
 
 
 class Rocket(DroneClass):
-    """Rocket instance that handles everything about a thrust vectored rocket with throttleable boosters and controllable finlets."""
+    """Rocket instance that handles everything about a thrust vectored rocket with throttleable boosters and controllable finlets.
+
+    The setpoint for this model has 7 values:
+        - finlet x deflection
+        - finlet y deflection
+        - finlet yaw
+        - ignition
+        - throttle
+        - booster gimbal axis 1
+        - booster gimbal axis 2
+    """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         start_pos: np.ndarray,
         start_orn: np.ndarray,
         control_hz: int = 120,
@@ -32,17 +42,14 @@
         camera_FOV_degrees: int = 90,
         camera_resolution: tuple[int, int] = (128, 128),
         camera_position_offset: np.ndarray = np.array([-1.0, 0.0, 3.0]),
         starting_fuel_ratio: float = 0.05,
     ):
         """Creates a drone in the QuadX configuration and handles all relevant control and physics.
 
-        The setpoint for this model has 7 values:
-            - force_x, force_y, yaw, ignition, throttle, booster gimbal 1, booster gimbal 2
-
         Args:
             p (bullet_client.BulletClient): p
             start_pos (np.ndarray): start_pos
             start_orn (np.ndarray): start_orn
             physics_hz (int): physics_hz
             control_hz (int): control_hz
             drone_model (str): drone_model
```

### Comparing `PyFlyt-0.6.2/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.3/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.3/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.3/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.3/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/pyproject.toml` & `PyFlyt-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["matplotlib", "gymnasium", "numpy", "pybullet"]
-keywords = ["Reinforcement Learning", "UAVs", "drones", "Quadcopter", "AI", "Gym", "PettingZoo"]
+dependencies = ["matplotlib", "gymnasium", "numpy", "pybullet", "pyyaml"]
+keywords = ["Reinforcement Learning", "UAVs", "drones", "Quadcopter", "AI", "RL", "Gymnasium"]
 license = { file="./LICENSE.txt" }
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
```

### Comparing `PyFlyt-0.6.2/tests/test_core.py` & `PyFlyt-0.6.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.2/tests/test_gym_envs.py` & `PyFlyt-0.6.3/tests/test_gym_envs.py`

 * *Files identical despite different names*


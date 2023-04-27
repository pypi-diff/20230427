# Comparing `tmp/rover_arm-1.0.7.tar.gz` & `tmp/rover_arm-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.0.7.tar", last modified: Wed Apr 26 14:28:28 2023, max compression
+gzip compressed data, was "rover_arm-1.0.8.tar", last modified: Thu Apr 27 19:34:05 2023, max compression
```

## Comparing `rover_arm-1.0.7.tar` & `rover_arm-1.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.785897 rover_arm-1.0.7/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-26 05:06:37.000000 rover_arm-1.0.7/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.0.7/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.0.7/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-26 14:28:28.785759 rover_arm-1.0.7/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.0.7/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.762051 rover_arm-1.0.7/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.0.7/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      225 2023-03-30 17:22:48.000000 rover_arm-1.0.7/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.763121 rover_arm-1.0.7/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.763477 rover_arm-1.0.7/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.766573 rover_arm-1.0.7/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.781154 rover_arm-1.0.7/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.0.7/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.785104 rover_arm-1.0.7/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.0.7/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.785547 rover_arm-1.0.7/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.0.7/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     6891 2023-04-26 14:24:56.000000 rover_arm-1.0.7/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    10518 2023-04-26 14:26:29.000000 rover_arm-1.0.7/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.0.7/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11738 2023-03-31 05:58:56.000000 rover_arm-1.0.7/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2371 2023-03-29 22:55:55.000000 rover_arm-1.0.7/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-26 14:28:28.762657 rover_arm-1.0.7/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-26 14:28:28.000000 rover_arm-1.0.7/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-04-26 14:28:28.000000 rover_arm-1.0.7/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-04-26 14:28:28.000000 rover_arm-1.0.7/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-04-26 14:28:28.000000 rover_arm-1.0.7/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-04-26 14:28:28.000000 rover_arm-1.0.7/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-04-26 14:28:28.785955 rover_arm-1.0.7/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-04-26 14:28:12.000000 rover_arm-1.0.7/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.815303 rover_arm-1.0.8/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.0.8/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.0.8/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.0.8/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:34:05.815164 rover_arm-1.0.8/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.0.8/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.802462 rover_arm-1.0.8/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.0.8/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.0.8/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803338 rover_arm-1.0.8/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803532 rover_arm-1.0.8/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.805682 rover_arm-1.0.8/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.813129 rover_arm-1.0.8/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.814723 rover_arm-1.0.8/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.0.8/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.814967 rover_arm-1.0.8/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.0.8/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6933 2023-04-27 19:31:10.000000 rover_arm-1.0.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10582 2023-04-27 19:31:07.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2371 2023-03-29 22:55:55.000000 rover_arm-1.0.8/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803041 rover_arm-1.0.8/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-04-27 19:34:05.815350 rover_arm-1.0.8/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-04-27 19:34:03.000000 rover_arm-1.0.8/setup.py
```

### Comparing `rover_arm-1.0.7/.DS_Store` & `rover_arm-1.0.8/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
 00000050: 0000 0001 0000 1000 0064 496c 6f63 626c  .........dIlocbl
 00000060: 6f62 0000 0000 0000 0000 0000 0000 0000  ob..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,15 +58,15 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 000a 0000 0005  ................
+00000400: 0000 0000 0000 0000 0000 0009 0000 0005  ................
 00000410: 0062 0075 0069 006c 0064 496c 6f63 626c  .b.u.i.l.dIlocbl
 00000420: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
 00000430: ffff ffff 0000 0000 0004 0064 0069 0073  ...........d.i.s
 00000440: 0074 496c 6f63 626c 6f62 0000 0010 0000  .tIlocblob......
 00000450: 0041 0000 002e ffff ffff ffff 0000 0000  .A..............
 00000460: 000b 004d 0041 004e 0049 0046 0045 0053  ...M.A.N.I.F.E.S
 00000470: 0054 002e 0069 006e 496c 6f63 626c 6f62  .T...i.nIlocblob
@@ -95,21 +95,21 @@
 000005e0: 1016 7b7b 3439 2c20 3738 7d2c 207b 3735  ..{{49, 78}, {75
 000005f0: 362c 2038 3636 7d7d 0908 1523 2f3b 525f  6, 866}}...#/;R_
 00000600: 6b6c 6d6e 6f88 0000 0000 0000 0101 0000  klmno...........
 00000610: 0000 0000 000d 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0089 0000 0012 0072 006f 0076  ...........r.o.v
 00000630: 0065 0072 005f 0061 0072 006d 002e 0065  .e.r._.a.r.m...e
 00000640: 0067 0067 002d 0069 006e 0066 006f 7653  .g.g.-.i.n.f.ovS
-00000650: 726e 6c6f 6e67 0000 0001 0000 0009 0073  rnlong.........s
-00000660: 0061 006d 0070 006c 0065 002e 0070 0079  .a.m.p.l.e...p.y
-00000670: 496c 6f63 626c 6f62 0000 0010 0000 011d  Ilocblob........
-00000680: 0000 009e ffff ffff ffff 0000 0000 0008  ................
-00000690: 0073 0065 0074 0075 0070 002e 0070 0079  .s.e.t.u.p...p.y
-000006a0: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
-000006b0: 0000 002e ffff ffff ffff 0000 0000 0000  ................
+00000650: 726e 6c6f 6e67 0000 0001 0000 0008 0073  rnlong.........s
+00000660: 0065 0074 0075 0070 002e 0070 0079 496c  .e.t.u.p...p.yIl
+00000670: 6f63 626c 6f62 0000 0010 0000 01f9 0000  ocblob..........
+00000680: 002e ffff ffff ffff 0000 0000 0000 0000  ................
+00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `rover_arm-1.0.7/PKG-INFO` & `rover_arm-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover_arm
-Version: 1.0.7
+Version: 1.0.8
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.0.7/README.md` & `rover_arm-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/.DS_Store` & `rover_arm-1.0.8/rover_arm/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.0.8/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/panda.urdf` & `rover_arm-1.0.8/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/data/rover_arm.xml` & `rover_arm-1.0.8/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.0.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 26 14:24:32 2023 UTC, .py size: 10518 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-00000000: 610d 0d0a 0000 0000 2034 4964 1629 0000  a....... 4Id.)..
+00000000: 610d 0d0a 0000 0000 7bcd 4a64 5629 0000  a.......{.JdV)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
-00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
-00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 6400  m.Z...d.d.l.Z.d.
-00000060: 6401 6c07 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c0a 5a0a 6400 6401 6c0b 5a0c 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0d 5a0d 6400 6401 6c0e 5a0e 4700  d.l.Z.d.d.l.Z.G.
-00000090: 6404 6405 8400 6405 6500 6a0f 8303 5a10  d.d...d.e.j...Z.
+00000030: 6401 6c00 5a01 6400 6402 6c00 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
+00000060: 6401 6c08 5a09 6400 6401 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6401 6c0b 5a0b 6400 6401 6c0c 5a0d 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6401 6c0e 5a0e 6400 6401 6c0f 5a0f 4700  d.l.Z.d.d.l.Z.G.
+00000090: 6404 6405 8400 6405 6501 6a10 8303 5a11  d.d...d.e.j...Z.
 000000a0: 6401 5300 2906 e900 0000 004e 2903 da05  d.S.)......N)...
 000000b0: 6572 726f 72da 0673 7061 6365 73da 0575  error..spaces..u
 000000c0: 7469 6c73 2901 da07 7365 6564 696e 6763  tils)...seedingc
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0600 0000 4000 0000 735c 0000 0065 005a  ....@...s\...e.Z
 000000f0: 0164 005a 0264 0164 0264 0367 0269 015a  .d.Z.d.d.d.g.i.Z
 00000100: 0364 0364 0464 0565 04a0 05a1 0064 0664  .d.d.d.e.....d.d
 00000110: 0666 0664 0764 0884 015a 0664 0964 0a84  .f.d.d...Z.d.d..
 00000120: 005a 0764 0b64 0c84 005a 0864 1464 0e64  .Z.d.d...Z.d.d.d
 00000130: 0f84 015a 0964 1064 1184 005a 0a64 1264  ...Z.d.d...Z.d.d
 00000140: 1384 005a 0b64 0d53 0029 15da 0b52 6f76  ...Z.d.S.)...Rov
 00000150: 6572 4172 6d45 6e76 7a0c 7265 6e64 6572  erArmEnvz.render
 00000160: 2e6d 6f64 6573 da05 6875 6d61 6eda 0972  .modes..human..r
-00000170: 6762 5f61 7272 6179 6950 c300 0046 e930  gb_arrayiP...F.0
+00000170: 6762 5f61 7272 6179 6910 2700 0046 e930  gb_arrayi.'..F.0
 00000180: 0000 0063 0700 0000 0000 0000 0000 0000  ...c............
 00000190: 0800 0000 0800 0000 4300 0000 7372 0100  ........C...sr..
 000001a0: 007c 017c 005f 007c 037c 005f 0164 017c  .|.|._.|.|._.d.|
 000001b0: 005f 027c 047c 005f 037c 027c 005f 047c  ._.|.|._.|.|._.|
 000001c0: 057c 005f 057c 067c 005f 067c 006a 0064  .|._.|.|._.|.j.d
 000001d0: 026b 0272 6a74 07a0 0874 076a 09a1 017d  .k.rjt...t.j...}
 000001e0: 077c 0764 036b 0072 5474 07a0 0874 076a  .|.d.k.rTt...t.j
@@ -99,333 +99,336 @@
 00000620: 6e69 745f 5f11 0000 0073 3800 0000 0002  nit__....s8.....
 00000630: 0601 0601 0601 0601 0601 0601 0601 0a01  ................
 00000640: 0c01 0801 0c01 1602 0c01 0601 0601 0601  ................
 00000650: 0a02 1a01 3601 0601 5403 0a01 0a02 0602  ....6...T.......
 00000660: 0601 0602 0602 7a14 526f 7665 7241 726d  ......z.RoverArm
 00000670: 456e 762e 5f5f 696e 6974 5f5f 6301 0000  Env.__init__c...
 00000680: 0000 0000 0000 0000 000d 0000 0008 0000  ................
-00000690: 0043 0000 0073 e601 0000 6401 7c00 5f00  .C...s....d.|._.
+00000690: 0043 0000 0073 ea01 0000 6401 7c00 5f00  .C...s....d.|._.
 000006a0: 7401 a002 a100 0100 7401 a003 7401 6a04  t.......t...t.j.
 000006b0: 6401 a102 0100 7401 a005 6401 6401 6402  d.....t...d.d.d.
 000006c0: a103 0100 7401 6a06 7407 6a08 a009 7c00  ....t.j.t.j...|.
 000006d0: 6a0a 6403 a102 6700 6404 a201 6405 8d02  j.d...g.d...d...
 000006e0: 7d01 6700 6406 a201 7d02 740b 6a0c a00d  }.g.d...}.t.j...
 000006f0: 740c a00e 6407 6408 a102 740c a00e 6409  t...d.d...t...d.
 00000700: 640a a102 6702 a101 7d03 740c a00e 6407  d...g...}.t...d.
 00000710: 640b a102 7d04 740f a010 a100 6401 1900  d...}.t.....d...
-00000720: 640c 1700 7d05 7401 6a06 7c05 640d 1700  d...}.t.j.|.d...
-00000730: 7c03 7c04 640e 6703 6405 8d02 7c00 5f11  |.|.d.g.d...|._.
-00000740: 7412 640f 6410 8302 4400 5d1c 7d06 7401  t.d.d...D.].}.t.
-00000750: a013 7c00 6a11 7c06 7c02 7c06 640f 1800  ..|.j.|.|.|.d...
-00000760: 1900 a103 0100 71b0 7401 a013 7c00 6a11  ......q.t...|.j.
-00000770: 6411 6412 a103 0100 7401 a013 7c00 6a11  d.d.....t...|.j.
-00000780: 6413 6412 a103 0100 7401 6a06 7407 6a08  d.d.....t.j.t.j.
-00000790: a009 7c00 6a0a 6414 a102 6700 6415 a201  ..|.j.d...g.d...
-000007a0: 6416 6417 8d03 7d07 7401 6a06 7407 6a08  d.d...}.t.j.t.j.
-000007b0: a009 7c00 6a0a 6418 a102 6700 6419 a201  ..|.j.d...g.d...
-000007c0: 6416 6417 8d03 7d08 740c a00e 641a 6416  d.d...}.t...d.d.
-000007d0: a102 740c a00e 641b 641c a102 641d 6703  ..t...d.d...d.g.
-000007e0: 7d09 7401 6a06 7407 6a08 a009 7c00 6a0a  }.t.j.t.j...|.j.
-000007f0: 641e a102 7c09 641f 6417 8d03 7c00 5f14  d...|.d.d...|._.
-00000800: 7401 a015 7c00 6a11 6401 a102 6401 1900  t...|.j.d...d...
-00000810: 6400 640a 8502 1900 7d0a 7401 a015 7c00  d.d.....}.t...|.
-00000820: 6a11 6420 a102 6401 1900 7d0b 7401 a016  j.d ..d...}.t...
-00000830: 7c00 6a11 6411 a102 6401 1900 7401 a016  |.j.d...d...t...
-00000840: 7c00 6a11 6413 a102 6401 1900 6602 7d0c  |.j.d...d...f.}.
-00000850: 7c0a 7c0b 1700 7c0c 1700 7c00 5f17 7401  |.|...|...|._.t.
-00000860: a003 7401 6a04 6421 a102 0100 740b a018  ..t.j.d!....t...
-00000870: 7c00 6a17 a101 a019 740b 6a1a a101 5300  |.j.....t.j...S.
-00000880: 2922 4e72 0100 0000 69f6 ffff ff7a 0a70  )"Nr....i....z.p
-00000890: 6c61 6e65 2e75 7264 6629 0372 0100 0000  lane.urdf).r....
-000008a0: 7201 0000 00e7 cdcc cccc cccc e4bf 2901  r.............).
-000008b0: da0c 6261 7365 506f 7369 7469 6f6e 2909  ..basePosition).
-000008c0: 7201 0000 0067 85eb 51b8 1e85 cbbf 7201  r....g..Q.....r.
-000008d0: 0000 0067 8fc2 f528 5c8f 04c0 7201 0000  ...g...(\...r...
-000008e0: 00e7 0c02 2b87 16d9 0240 723d 0000 00e7  ....+....@r=....
-000008f0: 7b14 ae47 e17a b43f 723e 0000 0072 0f00  {..G.z.?r>...r..
-00000900: 0000 6733 3333 3333 33d3 bf67 0000 0000  ..g333333..g....
-00000910: 0000 f43f 7216 0000 0067 0000 0000 0000  ...?r....g......
-00000920: 0440 7a10 2f72 6f76 6572 5f61 726d 2f64  .@z./rover_arm/d
-00000930: 6174 612f 7a0d 726f 7665 725f 6172 6d2e  ata/z.rover_arm.
-00000940: 786d 6c67 0000 0000 0000 e0bf e907 0000  xmlg............
-00000950: 00e9 0e00 0000 e910 0000 0072 1500 0000  ...........r....
-00000960: e911 0000 007a 1074 6162 6c65 2f74 6162  .....z.table/tab
-00000970: 6c65 2e75 7264 6629 03e7 0000 0000 0000  le.urdf)........
-00000980: e03f 7201 0000 0072 3b00 0000 7243 0000  .?r....r;...rC..
-00000990: 0029 0272 3c00 0000 5a0d 676c 6f62 616c  .).r<...Z.global
-000009a0: 5363 616c 696e 677a 1174 7261 792f 7472  Scalingz.tray/tr
-000009b0: 6179 626f 782e 7572 6466 2903 67cd cccc  aybox.urdf).g...
-000009c0: cccc ccdc 3f72 0100 0000 6771 3d0a d7a3  ....?r....gq=...
-000009d0: 70d5 bf67 9a99 9999 9999 d93f 679a 9999  p..g.......?g...
-000009e0: 9999 99a9 bfe7 9a99 9999 9999 a93f 720b  .............?r.
-000009f0: 0000 007a 1972 616e 646f 6d5f 7572 6466  ...z.random_urdf
-00000a00: 732f 3030 302f 3030 302e 7572 6466 679a  s/000/000.urdfg.
-00000a10: 9999 9999 99e9 3fe9 1200 0000 7212 0000  ......?.....r...
-00000a20: 0029 1bda 0c73 7465 705f 636f 756e 7465  .)...step_counte
-00000a30: 7272 1e00 0000 da0f 7265 7365 7453 696d  rr......resetSim
-00000a40: 756c 6174 696f 6eda 1863 6f6e 6669 6775  ulation..configu
-00000a50: 7265 4465 6275 6756 6973 7561 6c69 7a65  reDebugVisualize
-00000a60: 72da 1443 4f56 5f45 4e41 424c 455f 5245  r..COV_ENABLE_RE
-00000a70: 4e44 4552 494e 47da 0a73 6574 4772 6176  NDERING..setGrav
-00000a80: 6974 79da 086c 6f61 6455 5244 46da 026f  ity..loadURDF..o
-00000a90: 73da 0470 6174 68da 046a 6f69 6e72 1a00  s..path..joinr..
-00000aa0: 0000 7229 0000 00da 0672 616e 646f 6dda  ..r).....random.
-00000ab0: 0663 686f 6963 65da 0775 6e69 666f 726d  .choice..uniform
-00000ac0: da04 7369 7465 da0f 6765 7473 6974 6570  ..site..getsitep
-00000ad0: 6163 6b61 6765 73da 0b72 6f76 6572 6172  ackages..roverar
-00000ae0: 6d55 6964 da05 7261 6e67 65da 0f72 6573  mUid..range..res
-00000af0: 6574 4a6f 696e 7453 7461 7465 da09 6f62  etJointState..ob
-00000b00: 6a65 6374 5569 64da 0c67 6574 4c69 6e6b  jectUid..getLink
-00000b10: 5374 6174 65da 0d67 6574 4a6f 696e 7453  State..getJointS
-00000b20: 7461 7465 da0b 6f62 7365 7276 6174 696f  tate..observatio
-00000b30: 6e72 2a00 0000 da06 6173 7479 7065 da07  nr*.....astype..
-00000b40: 666c 6f61 7433 3229 0d72 3500 0000 5a08  float32).r5...Z.
-00000b50: 706c 616e 6555 6964 5a0a 7265 7374 5f70  planeUidZ.rest_p
-00000b60: 6f73 6573 5a05 785f 706f 735a 0579 5f70  osesZ.x_posZ.y_p
-00000b70: 6f73 da08 4241 5345 5f44 4952 da01 695a  os..BASE_DIR..iZ
-00000b80: 0874 6162 6c65 5569 645a 0774 7261 7955  .tableUidZ.trayU
-00000b90: 6964 da0c 7374 6174 655f 6f62 6a65 6374  id..state_object
-00000ba0: da0b 7374 6174 655f 726f 7665 72da 0973  ..state_rover..s
-00000bb0: 7461 7465 5f61 726d da0d 7374 6174 655f  tate_arm..state_
-00000bc0: 6669 6e67 6572 7372 3800 0000 7238 0000  fingersr8...r8..
-00000bd0: 0072 3900 0000 da05 7265 7365 7438 0000  .r9.....reset8..
-00000be0: 0073 3000 0000 0001 0601 0801 0e02 0e02  .s0.............
-00000bf0: 1e02 0802 2001 0c02 1001 1a03 0e01 1a01  .... ...........
-00000c00: 1001 1002 2001 2002 1a01 1e02 1a01 1201  .... . .........
-00000c10: 2402 0e02 0e01 7a11 526f 7665 7241 726d  $.....z.RoverArm
-00000c20: 456e 762e 7265 7365 7463 0200 0000 0000  Env.resetc......
-00000c30: 0000 0000 0000 2200 0000 0800 0000 0300  ......".........
-00000c40: 0000 7328 0300 0074 00a0 0164 0174 026a  ..s(...t...d.t.j
-00000c50: 030b 0074 026a 0364 021b 0067 03a1 017d  ...t.j.d...g...}
-00000c60: 0264 0389 0087 0066 0164 0464 0584 087c  .d.....f.d.d...|
-00000c70: 0164 0664 0785 0219 0044 0083 015c 037d  .d.d.....D...\.}
-00000c80: 037d 047d 057c 0164 0719 007d 0674 00a0  .}.}.|.d...}.t..
-00000c90: 0488 016a 0564 08a1 027d 077c 0764 0919  ...j.d...}.|.d..
-00000ca0: 007d 087c 0864 0919 007c 0317 007c 0864  .}.|.d...|...|.d
-00000cb0: 0a19 007c 0417 007c 0864 0619 007c 0517  ...|...|.d...|..
-00000cc0: 0067 037d 0974 00a0 0688 016a 0564 087c  .g.}.t.....j.d.|
-00000cd0: 097c 02a1 047d 0a7c 0a64 0064 0b85 0219  .|...}.|.d.d....
-00000ce0: 007c 0a64 0b64 0c85 0219 0002 007d 0b7d  .|.d.d.......}.}
-00000cf0: 0c74 00a0 0788 016a 0574 0874 0964 0d64  .t.....j.t.t.d.d
-00000d00: 0e83 0283 0164 0f64 1067 0217 0074 006a  .....d.d.g...t.j
-00000d10: 0a74 087c 0c83 0164 067c 0667 0114 0017  .t.|...d.|.g....
-00000d20: 00a1 0401 007c 0164 0064 0685 0219 005c  .....|.d.d.....\
-00000d30: 027d 0d7d 0e74 0b74 0c7c 0d64 1183 0264  .}.}.t.t.|.d...d
-00000d40: 0a83 027d 0d74 0c74 0b7c 0e64 1283 0264  ...}.t.t.|.d...d
-00000d50: 1383 027d 0e74 006a 0788 016a 0588 016a  ...}.t.j...j...j
-00000d60: 0d74 006a 0a7c 0e67 0164 0614 0064 148d  .t.j.|.g.d...d..
-00000d70: 0401 0088 016a 0e0b 0088 016a 0e88 016a  .....j.....j...j
-00000d80: 0f14 0088 016a 1017 0014 007d 0f88 016a  .....j.....}...j
-00000d90: 117c 0d14 007c 0f17 007d 1088 016a 0e64  .|...|...}...j.d
-00000da0: 157c 1014 0017 0088 015f 0e74 0b74 0c88  .|......._.t.t..
-00000db0: 016a 0e88 016a 120b 0083 0288 016a 1283  .j...j.......j..
-00000dc0: 0288 015f 0e74 006a 0788 016a 0588 016a  ..._.t.j...j...j
-00000dd0: 1374 006a 1488 016a 0e67 0164 1614 0064  .t.j...j.g.d...d
-00000de0: 1767 0164 1614 0064 188d 0501 0074 00a0  .g.d...d.....t..
-00000df0: 1588 016a 16a1 015c 027d 117d 1274 00a0  ...j...\.}.}.t..
-00000e00: 17a1 0001 0074 00a0 1588 016a 16a1 015c  .....t.....j...\
-00000e10: 027d 137d 1274 00a0 0488 016a 0564 09a1  .}.}.t.....j.d..
-00000e20: 0264 0919 0064 0064 0685 0219 007d 1474  .d...d.d.....}.t
-00000e30: 00a0 0488 016a 0564 08a1 0264 0919 007d  .....j.d...d...}
-00000e40: 1574 00a0 1888 016a 0564 0fa1 0264 0919  .t.....j.d...d..
-00000e50: 0074 00a0 1888 016a 0564 10a1 0264 0919  .t.....j.d...d..
-00000e60: 0066 027d 1664 195c 027d 177d 187c 1364  .f.}.d.\.}.}.|.d
-00000e70: 0619 0064 096b 0490 0272 3e64 0a7d 1964  ...d.k...r>d.}.d
-00000e80: 1a7d 176e 7474 19a0 1a74 19a0 1b7c 08a1  .}.ntt...t...|..
-00000e90: 0174 19a0 1b7c 11a1 0118 00a1 015c 037d  .t...|.......\.}
-00000ea0: 1a7d 1b7d 1c74 19a0 1a74 19a0 1b7c 15a1  .}.}.t...t...|..
-00000eb0: 0174 19a0 1b7c 13a1 0118 00a1 015c 037d  .t...|.......\.}
-00000ec0: 1d7d 1e7d 1f7c 1a7c 1d18 007c 1b17 007c  .}.}.|.|...|...|
-00000ed0: 1e18 007c 1c17 007c 1f18 007d 1974 1a7c  ...|...|...}.t.|
-00000ee0: 1983 0164 1b6b 0490 0272 ae7c 1964 171b  ...d.k...r.|.d..
-00000ef0: 007d 196e 0464 097d 1988 0104 006a 1c64  .}.n.d.}.....j.d
-00000f00: 0a37 0002 005f 1c87 0166 0164 1c64 1d84  .7..._...f.d.d..
-00000f10: 087d 207c 207c 1483 0190 0273 de64 117d  .} | |.....s.d.}
-00000f20: 1964 1a7d 1788 016a 1c88 016a 1d6b 0490  .d.}...j...j.k..
-00000f30: 0272 f464 097d 1964 1a7d 1864 1e7c 1369  .r.d.}.d.}.d.|.i
-00000f40: 017d 217c 147c 1517 007c 1617 0088 015f  .}!|.|...|....._
-00000f50: 1e74 19a0 1b88 016a 1ea1 01a0 1f74 196a  .t.....j.....t.j
-00000f60: 20a1 017c 197c 177c 187c 2166 0553 0029   ..|.|.|.|!f.S.)
-00000f70: 1f4e 6700 0000 0000 0000 0067 0000 0000  .Ng........g....
-00000f80: 0000 0040 7244 0000 0063 0100 0000 0000  ...@rD...c......
-00000f90: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-00000fa0: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
-00000fb0: 0188 0014 0091 0271 0453 0072 3800 0000  .......q.S.r8...
-00000fc0: 7238 0000 0029 02da 022e 30da 0178 2901  r8...)....0..x).
-00000fd0: da02 6476 7238 0000 0072 3900 0000 da0a  ..dvr8...r9.....
-00000fe0: 3c6c 6973 7463 6f6d 703e 6200 0000 f300  <listcomp>b.....
-00000ff0: 0000 007a 2452 6f76 6572 4172 6d45 6e76  ...z$RoverArmEnv
-00001000: 2e73 7465 702e 3c6c 6f63 616c 733e 2e3c  .step.<locals>.<
-00001010: 6c69 7374 636f 6d70 3e72 1600 0000 7214  listcomp>r....r.
-00001020: 0000 0072 4500 0000 7201 0000 0072 1200  ...rE...r....r..
-00001030: 0000 e906 0000 00e9 0d00 0000 723f 0000  ............r?..
-00001040: 0072 4000 0000 7241 0000 0072 4200 0000  .r@...rA...rB...
-00001050: 720f 0000 0072 1300 0000 7210 0000 0029  r....r....r....)
-00001060: 02da 0b63 6f6e 7472 6f6c 4d6f 6465 5a0f  ...controlModeZ.
-00001070: 7461 7267 6574 506f 7369 7469 6f6e 7367  targetPositionsg
-00001080: 1111 1111 1111 a13f 7211 0000 00e9 0a00  .......?r.......
-00001090: 0000 2905 5a0c 626f 6479 556e 6971 7565  ..).Z.bodyUnique
-000010a0: 4964 5a0c 6a6f 696e 7449 6e64 6963 6573  IdZ.jointIndices
-000010b0: 726b 0000 005a 1074 6172 6765 7456 656c  rk...Z.targetVel
-000010c0: 6f63 6974 6965 735a 0666 6f72 6365 7329  ocitiesZ.forces)
-000010d0: 0246 4654 67fc a9f1 d24d 6250 3f63 0100  .FFTg....MbP?c..
-000010e0: 0000 0000 0000 0000 0000 0400 0000 0200  ................
-000010f0: 0000 1300 0000 733c 0000 007c 005c 027d  ......s<...|.\.}
-00001100: 017d 027c 0188 006a 000b 006b 046f 1c7c  .}.|...j...k.o.|
-00001110: 0188 006a 006b 007d 037c 036f 367c 0288  ...j.k.}.|.o6|..
-00001120: 006a 000b 006b 046f 367c 0288 006a 006b  .j...k.o6|...j.k
-00001130: 007d 037c 0353 00a9 014e 2901 722c 0000  .}.|.S...N).r,..
-00001140: 0029 0472 6000 0000 5a02 7278 5a02 7279  .).r`...Z.rxZ.ry
-00001150: 5a07 696e 426f 756e 64a9 0172 3500 0000  Z.inBound..r5...
-00001160: 7238 0000 0072 3900 0000 da06 696e 4761  r8...r9.....inGa
-00001170: 6d65 a800 0000 7308 0000 0000 0108 0116  me....s.........
-00001180: 011a 017a 2052 6f76 6572 4172 6d45 6e76  ...z RoverArmEnv
-00001190: 2e73 7465 702e 3c6c 6f63 616c 733e 2e69  .step.<locals>.i
-000011a0: 6e47 616d 65da 0f6f 626a 6563 745f 706f  nGame..object_po
-000011b0: 7369 7469 6f6e 2921 721e 0000 00da 1667  sition)!r......g
-000011c0: 6574 5175 6174 6572 6e69 6f6e 4672 6f6d  etQuaternionFrom
-000011d0: 4575 6c65 72da 046d 6174 68da 0270 6972  Euler..math..pir
-000011e0: 5800 0000 7254 0000 00da 1a63 616c 6375  X...rT.....calcu
-000011f0: 6c61 7465 496e 7665 7273 654b 696e 656d  lateInverseKinem
-00001200: 6174 6963 73da 1973 6574 4a6f 696e 744d  atics..setJointM
-00001210: 6f74 6f72 436f 6e74 726f 6c41 7272 6179  otorControlArray
-00001220: da04 6c69 7374 7255 0000 00da 1050 4f53  ..listrU.....POS
-00001230: 4954 494f 4e5f 434f 4e54 524f 4cda 036d  ITION_CONTROL..m
-00001240: 696e da03 6d61 7872 2e00 0000 7230 0000  in..maxr....r0..
-00001250: 0072 3200 0000 7231 0000 0072 3300 0000  .r2...r1...r3...
-00001260: 7234 0000 0072 2f00 0000 da10 5645 4c4f  r4...r/.....VELO
-00001270: 4349 5459 5f43 4f4e 5452 4f4c da1d 6765  CITY_CONTROL..ge
-00001280: 7442 6173 6550 6f73 6974 696f 6e41 6e64  tBasePositionAnd
-00001290: 4f72 6965 6e74 6174 696f 6e72 5700 0000  OrientationrW...
-000012a0: da0e 7374 6570 5369 6d75 6c61 7469 6f6e  ..stepSimulation
-000012b0: 7259 0000 0072 2900 0000 da03 6162 7372  rY...r).....absr
-000012c0: 2a00 0000 7246 0000 0072 1b00 0000 725a  *...rF...r....rZ
-000012d0: 0000 0072 5b00 0000 725c 0000 0029 2272  ...r[...r\...)"r
-000012e0: 3500 0000 da06 6163 7469 6f6e 5a0b 6f72  5.....actionZ.or
-000012f0: 6965 6e74 6174 696f 6e5a 0464 785f 615a  ientationZ.dx_aZ
-00001300: 0464 795f 615a 0464 7a5f 615a 0766 696e  .dy_aZ.dz_aZ.fin
-00001310: 6765 7273 5a0b 6375 7272 656e 7450 6f73  gersZ.currentPos
-00001320: 655a 0f63 7572 7265 6e74 506f 7369 7469  eZ.currentPositi
-00001330: 6f6e 5a0b 6e65 7750 6f73 6974 696f 6e5a  onZ.newPositionZ
-00001340: 0a6a 6f69 6e74 506f 7365 735a 106a 6f69  .jointPosesZ.joi
-00001350: 6e74 506f 7365 735f 726f 7665 725a 0e6a  ntPoses_roverZ.j
-00001360: 6f69 6e74 506f 7365 735f 6172 6d5a 0874  ointPoses_armZ.t
-00001370: 6872 6f74 746c 655a 0e73 7465 6572 696e  hrottleZ.steerin
-00001380: 675f 616e 676c 655a 0866 7269 6374 696f  g_angleZ.frictio
-00001390: 6e5a 0c61 6363 656c 6572 6174 696f 6e5a  nZ.accelerationZ
-000013a0: 1173 7461 7465 5f6f 626a 6563 745f 7072  .state_object_pr
-000013b0: 6576 da01 5f72 5f00 0000 7260 0000 0072  ev.._r_...r`...r
-000013c0: 6100 0000 7262 0000 00da 0a74 6572 6d69  a...rb.....termi
-000013d0: 6e61 7465 64da 0974 7275 6e63 6174 6564  nated..truncated
-000013e0: da06 7265 7761 7264 da02 7830 5a02 7930  ..reward..x0Z.y0
-000013f0: 5a02 7a30 da02 7831 da02 7931 da02 7a31  Z.z0..x1..y1..z1
-00001400: 726f 0000 00da 0469 6e66 6f72 3800 0000  ro.....infor8...
-00001410: 2902 7266 0000 0072 3500 0000 7239 0000  ).rf...r5...r9..
-00001420: 00da 0473 7465 705e 0000 0073 7800 0000  ...step^...sx...
-00001430: 0002 1a01 0401 2001 0802 0e02 0802 0a01  ...... .........
-00001440: 0a01 0afe 0403 1201 1a01 3402 1004 1001  ..........4.....
-00001450: 1003 0c01 0401 08fe 0606 1001 04ff 0603  ................
-00001460: 0e03 1002 1a04 0401 0401 0401 0401 0a01  ................
-00001470: 08fb 0607 1002 0802 1001 1a01 1201 2402  ..............$.
-00001480: 0801 0e01 0401 0602 2001 2001 1801 0e01  ........ . .....
-00001490: 0a02 0402 0e01 0c06 0a01 0401 0402 0e01  ................
-000014a0: 0401 0402 0802 0e02 7a10 526f 7665 7241  ........z.RoverA
-000014b0: 726d 456e 762e 7374 6570 4e63 0300 0000  rmEnv.stepNc....
-000014c0: 0000 0000 0000 0000 0c00 0000 0800 0000  ................
-000014d0: 4300 0000 7342 0100 007c 0164 006b 0273  C...sB...|.d.k.s
-000014e0: 107c 0264 006b 0272 1c7c 006a 007d 017c  .|.d.k.r.|.j.}.|
-000014f0: 006a 017d 027c 006a 0264 016b 0372 2a64  .j.}.|.j.d.k.r*d
-00001500: 0053 0074 036a 047c 006a 057c 006a 067c  .S.t.j.|.j.|.j.|
-00001510: 006a 077c 006a 0864 0264 0364 048d 067d  .j.|.j.d.d.d...}
-00001520: 0374 036a 0467 0064 05a2 0164 0664 0764  .t.j.g.d...d.d.d
-00001530: 0864 0264 0364 048d 067d 0474 036a 0964  .d.d.d...}.t.j.d
-00001540: 0974 0a7c 0183 017c 021b 0064 0a64 0b64  .t.|...|...d.d.d
-00001550: 0c8d 047d 0574 036a 0b7c 017c 027c 037c  ...}.t.j.|.|.|.|
-00001560: 0574 036a 0c64 0d8d 055c 057d 067d 067d  .t.j.d...\.}.}.}
-00001570: 077d 067d 0674 036a 0b7c 017c 027c 047c  .}.}.t.j.|.|.|.|
-00001580: 0574 036a 0c64 0d8d 055c 057d 067d 067d  .t.j.d...\.}.}.}
-00001590: 087d 067d 0674 0d6a 0e7c 0774 0d6a 0f64  .}.}.t.j.|.t.j.d
-000015a0: 0e8d 027d 0974 0da0 107c 097c 027c 0164  ...}.t...|.|.|.d
-000015b0: 0f66 03a1 0264 0064 0085 0264 0064 0085  .f...d.d...d.d..
-000015c0: 0264 0064 1085 0266 0319 007d 0974 0d6a  .d.d...f...}.t.j
-000015d0: 0e7c 0874 0d6a 0f64 0e8d 027d 0a74 0da0  .|.t.j.d...}.t..
-000015e0: 107c 0a7c 027c 0164 0f66 03a1 0264 0064  .|.|.|.d.f...d.d
-000015f0: 0085 0264 0064 0085 0264 0064 1085 0266  ...d.d...d.d...f
-00001600: 0319 007d 0a74 0d6a 117c 097c 0a66 0264  ...}.t.j.|.|.f.d
-00001610: 0264 118d 027d 0b7c 0b53 0029 124e 7208  .d...}.|.S.).Nr.
-00001620: 0000 0072 0100 0000 7216 0000 0029 0672  ...r....r....).r
-00001630: 0e00 0000 da08 6469 7374 616e 6365 5a03  ......distanceZ.
-00001640: 7961 775a 0570 6974 6368 da04 726f 6c6c  yawZ.pitch..roll
-00001650: 5a0b 7570 4178 6973 496e 6465 7829 03e7  Z.upAxisIndex)..
-00001660: 6666 6666 6666 e63f 7201 0000 0072 4400  ffffff.?r....rD.
-00001670: 0000 728b 0000 00e9 5a00 0000 69ba ffff  ..r.....Z...i...
-00001680: ffe9 3c00 0000 679a 9999 9999 99b9 3f67  ..<...g.......?g
-00001690: 0000 0000 0000 5940 2904 5a03 666f 76da  ......Y@).Z.fov.
-000016a0: 0661 7370 6563 745a 076e 6561 7256 616c  .aspectZ.nearVal
-000016b0: 5a06 6661 7256 616c 2905 7236 0000 0072  Z.farVal).r6...r
-000016c0: 3700 0000 5a0a 7669 6577 4d61 7472 6978  7...Z.viewMatrix
-000016d0: 5a10 7072 6f6a 6563 7469 6f6e 4d61 7472  Z.projectionMatr
-000016e0: 6978 5a08 7265 6e64 6572 6572 2901 da05  ixZ.renderer)...
-000016f0: 6474 7970 6572 1100 0000 720c 0000 0029  dtyper....r....)
-00001700: 01da 0461 7869 7329 1272 1c00 0000 721d  ...axis).r....r.
-00001710: 0000 0072 1900 0000 721e 0000 00da 2163  ...r....r.....!c
-00001720: 6f6d 7075 7465 5669 6577 4d61 7472 6978  omputeViewMatrix
-00001730: 4672 6f6d 5961 7750 6974 6368 526f 6c6c  FromYawPitchRoll
-00001740: 7227 0000 0072 2400 0000 7225 0000 0072  r'...r$...r%...r
-00001750: 2600 0000 da1a 636f 6d70 7574 6550 726f  &.....computePro
-00001760: 6a65 6374 696f 6e4d 6174 7269 7846 4f56  jectionMatrixFOV
-00001770: da05 666c 6f61 74da 0e67 6574 4361 6d65  ..float..getCame
-00001780: 7261 496d 6167 65da 1945 525f 4255 4c4c  raImage..ER_BULL
-00001790: 4554 5f48 4152 4457 4152 455f 4f50 454e  ET_HARDWARE_OPEN
-000017a0: 474c 7229 0000 0072 2a00 0000 da05 7569  GLr)...r*.....ui
-000017b0: 6e74 38da 0772 6573 6861 7065 da0b 636f  nt8..reshape..co
-000017c0: 6e63 6174 656e 6174 6529 0c72 3500 0000  ncatenate).r5...
-000017d0: 7236 0000 0072 3700 0000 5a0c 7669 6577  r6...r7...Z.view
-000017e0: 5f6d 6174 7269 7831 5a0c 7669 6577 5f6d  _matrix1Z.view_m
-000017f0: 6174 7269 7832 5a0b 7072 6f6a 5f6d 6174  atrix2Z.proj_mat
-00001800: 7269 7872 7f00 0000 5a03 7078 315a 0370  rixr....Z.px1Z.p
-00001810: 7832 5a0a 7267 625f 6172 7261 7931 5a0a  x2Z.rgb_array1Z.
-00001820: 7267 625f 6172 7261 7932 7208 0000 0072  rgb_array2r....r
-00001830: 3800 0000 7238 0000 0072 3900 0000 da06  8...r8...r9.....
-00001840: 7265 6e64 6572 bd00 0000 7354 0000 0000  render....sT....
-00001850: 0710 0106 0106 010a 0104 0108 0104 0104  ................
-00001860: 0104 0102 0102 fb06 060a 0102 0102 0102  ................
-00001870: 0102 0102 fb06 0606 010a 0102 0102 fd06  ................
-00001880: 0506 0102 0102 0102 0104 fc10 0606 0102  ................
-00001890: 0102 0102 0104 fc10 0610 0128 0210 0128  ...........(...(
-000018a0: 0312 027a 1252 6f76 6572 4172 6d45 6e76  ...z.RoverArmEnv
-000018b0: 2e72 656e 6465 7263 0100 0000 0000 0000  .renderc........
-000018c0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000018d0: 7306 0000 007c 006a 0053 0072 6d00 0000  s....|.j.S.rm...
-000018e0: 2901 725a 0000 0072 6e00 0000 7238 0000  ).rZ...rn...r8..
-000018f0: 0072 3800 0000 7239 0000 00da 0a5f 6765  .r8...r9....._ge
-00001900: 745f 7374 6174 65f1 0000 0073 0200 0000  t_state....s....
-00001910: 0001 7a16 526f 7665 7241 726d 456e 762e  ..z.RoverArmEnv.
-00001920: 5f67 6574 5f73 7461 7465 6301 0000 0000  _get_statec.....
-00001930: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00001940: 0000 0073 0c00 0000 7400 a001 a100 0100  ...s....t.......
-00001950: 6400 5300 726d 0000 0029 0272 1e00 0000  d.S.rm...).r....
-00001960: da0a 6469 7363 6f6e 6e65 6374 726e 0000  ..disconnectrn..
-00001970: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
-00001980: da05 636c 6f73 65f4 0000 0073 0200 0000  ..close....s....
-00001990: 0001 7a11 526f 7665 7241 726d 456e 762e  ..z.RoverArmEnv.
-000019a0: 636c 6f73 6529 024e 4e29 0cda 085f 5f6e  close).NN)...__n
-000019b0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000019c0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000019d0: 086d 6574 6164 6174 61da 0d70 7962 756c  .metadata..pybul
-000019e0: 6c65 745f 6461 7461 5a0b 6765 7444 6174  let_dataZ.getDat
-000019f0: 6150 6174 6872 3a00 0000 7263 0000 0072  aPathr:...rc...r
-00001a00: 8800 0000 7299 0000 0072 9a00 0000 729c  ....r....r....r.
-00001a10: 0000 0072 3800 0000 7238 0000 0072 3800  ...r8...r8...r8.
-00001a20: 0000 7239 0000 0072 0600 0000 0e00 0000  ..r9...r........
-00001a30: 7312 0000 0008 010c 020c 0104 ff0a 2708  s.............'.
-00001a40: 2608 5f0a 3408 0372 0600 0000 2911 da03  &._.4..r....)...
-00001a50: 6779 6d72 0200 0000 7203 0000 0072 0400  gymr....r....r..
-00001a60: 0000 da09 6779 6d2e 7574 696c 7372 0500  ....gym.utilsr..
-00001a70: 0000 724c 0000 00da 0870 7962 756c 6c65  ..rL.....pybulle
-00001a80: 7472 1e00 0000 72a1 0000 0072 7200 0000  tr....r....rr...
-00001a90: da05 6e75 6d70 7972 2900 0000 724f 0000  ..numpyr)...rO..
-00001aa0: 0072 5200 0000 da03 456e 7672 0600 0000  .rR.....Envr....
-00001ab0: 7238 0000 0072 3800 0000 7238 0000 0072  r8...r8...r8...r
-00001ac0: 3900 0000 da08 3c6d 6f64 756c 653e 0100  9.....<module>..
-00001ad0: 0000 7314 0000 0008 0114 010c 0208 0108  ..s.............
-00001ae0: 0108 0108 0108 0108 0108 03              ...........
+00000720: 640c 1700 7d05 640d 7d05 7401 6a06 7c05  d...}.d.}.t.j.|.
+00000730: 640e 1700 7c03 7c04 640f 6703 6405 8d02  d...|.|.d.g.d...
+00000740: 7c00 5f11 7412 6410 6411 8302 4400 5d1c  |._.t.d.d...D.].
+00000750: 7d06 7401 a013 7c00 6a11 7c06 7c02 7c06  }.t...|.j.|.|.|.
+00000760: 6410 1800 1900 a103 0100 71b4 7401 a013  d.........q.t...
+00000770: 7c00 6a11 6412 6413 a103 0100 7401 a013  |.j.d.d.....t...
+00000780: 7c00 6a11 6414 6413 a103 0100 7401 6a06  |.j.d.d.....t.j.
+00000790: 7407 6a08 a009 7c00 6a0a 6415 a102 6700  t.j...|.j.d...g.
+000007a0: 6416 a201 6417 6418 8d03 7d07 7401 6a06  d...d.d...}.t.j.
+000007b0: 7407 6a08 a009 7c00 6a0a 6419 a102 6700  t.j...|.j.d...g.
+000007c0: 641a a201 6417 6418 8d03 7d08 740c a00e  d...d.d...}.t...
+000007d0: 641b 6417 a102 740c a00e 641c 641d a102  d.d...t...d.d...
+000007e0: 641e 6703 7d09 7401 6a06 7407 6a08 a009  d.g.}.t.j.t.j...
+000007f0: 7c00 6a0a 641f a102 7c09 6420 6418 8d03  |.j.d...|.d d...
+00000800: 7c00 5f14 7401 a015 7c00 6a11 6401 a102  |._.t...|.j.d...
+00000810: 6401 1900 6400 640a 8502 1900 7d0a 7401  d...d.d.....}.t.
+00000820: a015 7c00 6a11 6421 a102 6401 1900 7d0b  ..|.j.d!..d...}.
+00000830: 7401 a016 7c00 6a11 6412 a102 6401 1900  t...|.j.d...d...
+00000840: 7401 a016 7c00 6a11 6414 a102 6401 1900  t...|.j.d...d...
+00000850: 6602 7d0c 7c0a 7c0b 1700 7c0c 1700 7c00  f.}.|.|...|...|.
+00000860: 5f17 7401 a003 7401 6a04 6422 a102 0100  _.t...t.j.d"....
+00000870: 740b a018 7c00 6a17 a101 a019 740b 6a1a  t...|.j.....t.j.
+00000880: a101 5300 2923 4e72 0100 0000 69f6 ffff  ..S.)#Nr....i...
+00000890: ff7a 0a70 6c61 6e65 2e75 7264 6629 0372  .z.plane.urdf).r
+000008a0: 0100 0000 7201 0000 00e7 cdcc cccc cccc  ....r...........
+000008b0: e4bf 2901 da0c 6261 7365 506f 7369 7469  ..)...basePositi
+000008c0: 6f6e 2909 7201 0000 0067 85eb 51b8 1e85  on).r....g..Q...
+000008d0: cbbf 7201 0000 0067 8fc2 f528 5c8f 04c0  ..r....g...(\...
+000008e0: 7201 0000 00e7 0c02 2b87 16d9 0240 723d  r.......+....@r=
+000008f0: 0000 00e7 7b14 ae47 e17a b43f 723e 0000  ....{..G.z.?r>..
+00000900: 0072 0f00 0000 6733 3333 3333 33d3 bf67  .r....g333333..g
+00000910: 0000 0000 0000 f43f 7216 0000 0067 0000  .......?r....g..
+00000920: 0000 0000 0440 7a10 2f72 6f76 6572 5f61  .....@z./rover_a
+00000930: 726d 2f64 6174 612f 7a11 2e2f 726f 7665  rm/data/z../rove
+00000940: 725f 6172 6d2f 6461 7461 2f7a 0d72 6f76  r_arm/data/z.rov
+00000950: 6572 5f61 726d 2e78 6d6c 6700 0000 0000  er_arm.xmlg.....
+00000960: 00e0 bfe9 0700 0000 e90e 0000 00e9 1000  ................
+00000970: 0000 7215 0000 00e9 1100 0000 7a10 7461  ..r.........z.ta
+00000980: 626c 652f 7461 626c 652e 7572 6466 2903  ble/table.urdf).
+00000990: e700 0000 0000 00e0 3f72 0100 0000 723b  ........?r....r;
+000009a0: 0000 0072 4300 0000 2902 723c 0000 005a  ...rC...).r<...Z
+000009b0: 0d67 6c6f 6261 6c53 6361 6c69 6e67 7a11  .globalScalingz.
+000009c0: 7472 6179 2f74 7261 7962 6f78 2e75 7264  tray/traybox.urd
+000009d0: 6629 0367 cdcc cccc cccc dc3f 7201 0000  f).g.......?r...
+000009e0: 0067 713d 0ad7 a370 d5bf 679a 9999 9999  .gq=...p..g.....
+000009f0: 99d9 3f67 9a99 9999 9999 a9bf e79a 9999  ..?g............
+00000a00: 9999 99a9 3f72 0b00 0000 7a19 7261 6e64  ....?r....z.rand
+00000a10: 6f6d 5f75 7264 6673 2f30 3030 2f30 3030  om_urdfs/000/000
+00000a20: 2e75 7264 6667 9a99 9999 9999 e93f e912  .urdfg.......?..
+00000a30: 0000 0072 1200 0000 291b da0c 7374 6570  ...r....)...step
+00000a40: 5f63 6f75 6e74 6572 721e 0000 00da 0f72  _counterr......r
+00000a50: 6573 6574 5369 6d75 6c61 7469 6f6e da18  esetSimulation..
+00000a60: 636f 6e66 6967 7572 6544 6562 7567 5669  configureDebugVi
+00000a70: 7375 616c 697a 6572 da14 434f 565f 454e  sualizer..COV_EN
+00000a80: 4142 4c45 5f52 454e 4445 5249 4e47 da0a  ABLE_RENDERING..
+00000a90: 7365 7447 7261 7669 7479 da08 6c6f 6164  setGravity..load
+00000aa0: 5552 4446 da02 6f73 da04 7061 7468 da04  URDF..os..path..
+00000ab0: 6a6f 696e 721a 0000 0072 2900 0000 da06  joinr....r).....
+00000ac0: 7261 6e64 6f6d da06 6368 6f69 6365 da07  random..choice..
+00000ad0: 756e 6966 6f72 6dda 0473 6974 65da 0f67  uniform..site..g
+00000ae0: 6574 7369 7465 7061 636b 6167 6573 da0b  etsitepackages..
+00000af0: 726f 7665 7261 726d 5569 64da 0572 616e  roverarmUid..ran
+00000b00: 6765 da0f 7265 7365 744a 6f69 6e74 5374  ge..resetJointSt
+00000b10: 6174 65da 096f 626a 6563 7455 6964 da0c  ate..objectUid..
+00000b20: 6765 744c 696e 6b53 7461 7465 da0d 6765  getLinkState..ge
+00000b30: 744a 6f69 6e74 5374 6174 65da 0b6f 6273  tJointState..obs
+00000b40: 6572 7661 7469 6f6e 722a 0000 00da 0661  ervationr*.....a
+00000b50: 7374 7970 65da 0766 6c6f 6174 3332 290d  stype..float32).
+00000b60: 7235 0000 005a 0870 6c61 6e65 5569 645a  r5...Z.planeUidZ
+00000b70: 0a72 6573 745f 706f 7365 735a 0578 5f70  .rest_posesZ.x_p
+00000b80: 6f73 5a05 795f 706f 73da 0842 4153 455f  osZ.y_pos..BASE_
+00000b90: 4449 52da 0169 5a08 7461 626c 6555 6964  DIR..iZ.tableUid
+00000ba0: 5a07 7472 6179 5569 64da 0c73 7461 7465  Z.trayUid..state
+00000bb0: 5f6f 626a 6563 74da 0b73 7461 7465 5f72  _object..state_r
+00000bc0: 6f76 6572 da09 7374 6174 655f 6172 6dda  over..state_arm.
+00000bd0: 0d73 7461 7465 5f66 696e 6765 7273 7238  .state_fingersr8
+00000be0: 0000 0072 3800 0000 7239 0000 00da 0572  ...r8...r9.....r
+00000bf0: 6573 6574 3800 0000 7332 0000 0000 0106  eset8...s2......
+00000c00: 0108 010e 020e 021e 0208 0220 010c 0210  ........... ....
+00000c10: 0104 011a 030e 011a 0110 0110 0220 0120  ............. . 
+00000c20: 021a 011e 021a 0112 0124 020e 020e 017a  .........$.....z
+00000c30: 1152 6f76 6572 4172 6d45 6e76 2e72 6573  .RoverArmEnv.res
+00000c40: 6574 6302 0000 0000 0000 0000 0000 0022  etc............"
+00000c50: 0000 0008 0000 0003 0000 0073 2803 0000  ...........s(...
+00000c60: 7400 a001 6401 7402 6a03 0b00 7402 6a03  t...d.t.j...t.j.
+00000c70: 6402 1b00 6703 a101 7d02 6403 8900 8700  d...g...}.d.....
+00000c80: 6601 6404 6405 8408 7c01 6406 6407 8502  f.d.d...|.d.d...
+00000c90: 1900 4400 8301 5c03 7d03 7d04 7d05 7c01  ..D...\.}.}.}.|.
+00000ca0: 6407 1900 7d06 7400 a004 8801 6a05 6408  d...}.t.....j.d.
+00000cb0: a102 7d07 7c07 6409 1900 7d08 7c08 6409  ..}.|.d...}.|.d.
+00000cc0: 1900 7c03 1700 7c08 640a 1900 7c04 1700  ..|...|.d...|...
+00000cd0: 7c08 6406 1900 7c05 1700 6703 7d09 7400  |.d...|...g.}.t.
+00000ce0: a006 8801 6a05 6408 7c09 7c02 a104 7d0a  ....j.d.|.|...}.
+00000cf0: 7c0a 6400 640b 8502 1900 7c0a 640b 640c  |.d.d.....|.d.d.
+00000d00: 8502 1900 0200 7d0b 7d0c 7400 a007 8801  ......}.}.t.....
+00000d10: 6a05 7408 7409 640d 640e 8302 8301 640f  j.t.t.d.d.....d.
+00000d20: 6410 6702 1700 7400 6a0a 7408 7c0c 8301  d.g...t.j.t.|...
+00000d30: 6406 7c06 6701 1400 1700 a104 0100 7c01  d.|.g.........|.
+00000d40: 6400 6406 8502 1900 5c02 7d0d 7d0e 740b  d.d.....\.}.}.t.
+00000d50: 740c 7c0d 6411 8302 640a 8302 7d0d 740c  t.|.d...d...}.t.
+00000d60: 740b 7c0e 6412 8302 6413 8302 7d0e 7400  t.|.d...d...}.t.
+00000d70: 6a07 8801 6a05 8801 6a0d 7400 6a0a 7c0e  j...j...j.t.j.|.
+00000d80: 6701 6406 1400 6414 8d04 0100 8801 6a0e  g.d...d.......j.
+00000d90: 0b00 8801 6a0e 8801 6a0f 1400 8801 6a10  ....j...j.....j.
+00000da0: 1700 1400 7d0f 8801 6a11 7c0d 1400 7c0f  ....}...j.|...|.
+00000db0: 1700 7d10 8801 6a0e 6415 7c10 1400 1700  ..}...j.d.|.....
+00000dc0: 8801 5f0e 740b 740c 8801 6a0e 8801 6a12  .._.t.t...j...j.
+00000dd0: 0b00 8302 8801 6a12 8302 8801 5f0e 7400  ......j....._.t.
+00000de0: 6a07 8801 6a05 8801 6a13 7400 6a14 8801  j...j...j.t.j...
+00000df0: 6a0e 6701 6416 1400 6417 6701 6416 1400  j.g.d...d.g.d...
+00000e00: 6418 8d05 0100 7400 a015 8801 6a16 a101  d.....t.....j...
+00000e10: 5c02 7d11 7d12 7400 a017 a100 0100 7400  \.}.}.t.......t.
+00000e20: a015 8801 6a16 a101 5c02 7d13 7d12 7400  ....j...\.}.}.t.
+00000e30: a004 8801 6a05 6409 a102 6409 1900 6400  ....j.d...d...d.
+00000e40: 6406 8502 1900 7d14 7400 a004 8801 6a05  d.....}.t.....j.
+00000e50: 6408 a102 6409 1900 7d15 7400 a018 8801  d...d...}.t.....
+00000e60: 6a05 640f a102 6409 1900 7400 a018 8801  j.d...d...t.....
+00000e70: 6a05 6410 a102 6409 1900 6602 7d16 6419  j.d...d...f.}.d.
+00000e80: 5c02 7d17 7d18 7c13 6406 1900 6409 6b04  \.}.}.|.d...d.k.
+00000e90: 9002 723e 640a 7d19 641a 7d17 6e74 7419  ..r>d.}.d.}.ntt.
+00000ea0: a01a 7419 a01b 7c08 a101 7419 a01b 7c11  ..t...|...t...|.
+00000eb0: a101 1800 a101 5c03 7d1a 7d1b 7d1c 7419  ......\.}.}.}.t.
+00000ec0: a01a 7419 a01b 7c15 a101 7419 a01b 7c13  ..t...|...t...|.
+00000ed0: a101 1800 a101 5c03 7d1d 7d1e 7d1f 7c1a  ......\.}.}.}.|.
+00000ee0: 7c1d 1800 7c1b 1700 7c1e 1800 7c1c 1700  |...|...|...|...
+00000ef0: 7c1f 1800 7d19 741a 7c19 8301 641b 6b04  |...}.t.|...d.k.
+00000f00: 9002 72ae 7c19 6417 1b00 7d19 6e04 6409  ..r.|.d...}.n.d.
+00000f10: 7d19 8801 0400 6a1c 640a 3700 0200 5f1c  }.....j.d.7..._.
+00000f20: 8701 6601 641c 641d 8408 7d20 7c20 7c14  ..f.d.d...} | |.
+00000f30: 8301 9002 73de 6411 7d19 641a 7d17 8801  ....s.d.}.d.}...
+00000f40: 6a1c 8801 6a1d 6b04 9002 72f4 6409 7d19  j...j.k...r.d.}.
+00000f50: 641a 7d18 641e 7c13 6901 7d21 7c14 7c15  d.}.d.|.i.}!|.|.
+00000f60: 1700 7c16 1700 8801 5f1e 7419 a01b 8801  ..|....._.t.....
+00000f70: 6a1e a101 a01f 7419 6a20 a101 7c19 7c17  j.....t.j ..|.|.
+00000f80: 7c18 7c21 6605 5300 291f 4e67 0000 0000  |.|!f.S.).Ng....
+00000f90: 0000 0000 6700 0000 0000 0000 4072 4400  ....g.......@rD.
+00000fa0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000fb0: 0000 0004 0000 0013 0000 0073 1400 0000  ...........s....
+00000fc0: 6700 7c00 5d0c 7d01 7c01 8800 1400 9102  g.|.].}.|.......
+00000fd0: 7104 5300 7238 0000 0072 3800 0000 2902  q.S.r8...r8...).
+00000fe0: da02 2e30 da01 7829 01da 0264 7672 3800  ...0..x)...dvr8.
+00000ff0: 0000 7239 0000 00da 0a3c 6c69 7374 636f  ..r9.....<listco
+00001000: 6d70 3e63 0000 00f3 0000 0000 7a24 526f  mp>c........z$Ro
+00001010: 7665 7241 726d 456e 762e 7374 6570 2e3c  verArmEnv.step.<
+00001020: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001030: 703e 7216 0000 0072 1400 0000 7245 0000  p>r....r....rE..
+00001040: 0072 0100 0000 7212 0000 00e9 0600 0000  .r....r.........
+00001050: e90d 0000 0072 3f00 0000 7240 0000 0072  .....r?...r@...r
+00001060: 4100 0000 7242 0000 0072 0f00 0000 7213  A...rB...r....r.
+00001070: 0000 0072 1000 0000 2902 da0b 636f 6e74  ...r....)...cont
+00001080: 726f 6c4d 6f64 655a 0f74 6172 6765 7450  rolModeZ.targetP
+00001090: 6f73 6974 696f 6e73 6711 1111 1111 11a1  ositionsg.......
+000010a0: 3f72 1100 0000 e90a 0000 0029 055a 0c62  ?r.........).Z.b
+000010b0: 6f64 7955 6e69 7175 6549 645a 0c6a 6f69  odyUniqueIdZ.joi
+000010c0: 6e74 496e 6469 6365 7372 6b00 0000 5a10  ntIndicesrk...Z.
+000010d0: 7461 7267 6574 5665 6c6f 6369 7469 6573  targetVelocities
+000010e0: 5a06 666f 7263 6573 2902 4646 5467 fca9  Z.forces).FFTg..
+000010f0: f1d2 4d62 503f 6301 0000 0000 0000 0000  ..MbP?c.........
+00001100: 0000 0004 0000 0002 0000 0013 0000 0073  ...............s
+00001110: 3c00 0000 7c00 5c02 7d01 7d02 7c01 8800  <...|.\.}.}.|...
+00001120: 6a00 0b00 6b04 6f1c 7c01 8800 6a00 6b00  j...k.o.|...j.k.
+00001130: 7d03 7c03 6f36 7c02 8800 6a00 0b00 6b04  }.|.o6|...j...k.
+00001140: 6f36 7c02 8800 6a00 6b00 7d03 7c03 5300  o6|...j.k.}.|.S.
+00001150: a901 4e29 0172 2c00 0000 2904 7260 0000  ..N).r,...).r`..
+00001160: 00da 0272 785a 0272 795a 0769 6e42 6f75  ...rxZ.ryZ.inBou
+00001170: 6e64 a901 7235 0000 0072 3800 0000 7239  nd..r5...r8...r9
+00001180: 0000 00da 0669 6e47 616d 65a9 0000 0073  .....inGame....s
+00001190: 0800 0000 0001 0801 1601 1a01 7a20 526f  ............z Ro
+000011a0: 7665 7241 726d 456e 762e 7374 6570 2e3c  verArmEnv.step.<
+000011b0: 6c6f 6361 6c73 3e2e 696e 4761 6d65 da0f  locals>.inGame..
+000011c0: 6f62 6a65 6374 5f70 6f73 6974 696f 6e29  object_position)
+000011d0: 2172 1e00 0000 da16 6765 7451 7561 7465  !r......getQuate
+000011e0: 726e 696f 6e46 726f 6d45 756c 6572 da04  rnionFromEuler..
+000011f0: 6d61 7468 da02 7069 7258 0000 0072 5400  math..pirX...rT.
+00001200: 0000 da1a 6361 6c63 756c 6174 6549 6e76  ....calculateInv
+00001210: 6572 7365 4b69 6e65 6d61 7469 6373 da19  erseKinematics..
+00001220: 7365 744a 6f69 6e74 4d6f 746f 7243 6f6e  setJointMotorCon
+00001230: 7472 6f6c 4172 7261 79da 046c 6973 7472  trolArray..listr
+00001240: 5500 0000 da10 504f 5349 5449 4f4e 5f43  U.....POSITION_C
+00001250: 4f4e 5452 4f4c da03 6d69 6eda 036d 6178  ONTROL..min..max
+00001260: 722e 0000 0072 3000 0000 7232 0000 0072  r....r0...r2...r
+00001270: 3100 0000 7233 0000 0072 3400 0000 722f  1...r3...r4...r/
+00001280: 0000 00da 1056 454c 4f43 4954 595f 434f  .....VELOCITY_CO
+00001290: 4e54 524f 4cda 1d67 6574 4261 7365 506f  NTROL..getBasePo
+000012a0: 7369 7469 6f6e 416e 644f 7269 656e 7461  sitionAndOrienta
+000012b0: 7469 6f6e 7257 0000 00da 0e73 7465 7053  tionrW.....stepS
+000012c0: 696d 756c 6174 696f 6e72 5900 0000 7229  imulationrY...r)
+000012d0: 0000 00da 0361 6273 722a 0000 0072 4600  .....absr*...rF.
+000012e0: 0000 721b 0000 0072 5a00 0000 725b 0000  ..r....rZ...r[..
+000012f0: 0072 5c00 0000 2922 7235 0000 00da 0661  .r\...)"r5.....a
+00001300: 6374 696f 6e5a 0b6f 7269 656e 7461 7469  ctionZ.orientati
+00001310: 6f6e 5a04 6478 5f61 5a04 6479 5f61 5a04  onZ.dx_aZ.dy_aZ.
+00001320: 647a 5f61 5a07 6669 6e67 6572 735a 0b63  dz_aZ.fingersZ.c
+00001330: 7572 7265 6e74 506f 7365 5a0f 6375 7272  urrentPoseZ.curr
+00001340: 656e 7450 6f73 6974 696f 6e5a 0b6e 6577  entPositionZ.new
+00001350: 506f 7369 7469 6f6e 5a0a 6a6f 696e 7450  PositionZ.jointP
+00001360: 6f73 6573 5a10 6a6f 696e 7450 6f73 6573  osesZ.jointPoses
+00001370: 5f72 6f76 6572 5a0e 6a6f 696e 7450 6f73  _roverZ.jointPos
+00001380: 6573 5f61 726d 5a08 7468 726f 7474 6c65  es_armZ.throttle
+00001390: 5a0e 7374 6565 7269 6e67 5f61 6e67 6c65  Z.steering_angle
+000013a0: 5a08 6672 6963 7469 6f6e 5a0c 6163 6365  Z.frictionZ.acce
+000013b0: 6c65 7261 7469 6f6e 5a11 7374 6174 655f  lerationZ.state_
+000013c0: 6f62 6a65 6374 5f70 7265 76da 015f 725f  object_prev.._r_
+000013d0: 0000 0072 6000 0000 7261 0000 0072 6200  ...r`...ra...rb.
+000013e0: 0000 da0a 7465 726d 696e 6174 6564 da09  ....terminated..
+000013f0: 7472 756e 6361 7465 64da 0672 6577 6172  truncated..rewar
+00001400: 64da 0278 305a 0279 305a 027a 30da 0278  d..x0Z.y0Z.z0..x
+00001410: 31da 0279 31da 027a 3172 7000 0000 da04  1..y1..z1rp.....
+00001420: 696e 666f 7238 0000 0029 0272 6600 0000  infor8...).rf...
+00001430: 7235 0000 0072 3900 0000 da04 7374 6570  r5...r9.....step
+00001440: 5f00 0000 7378 0000 0000 021a 0104 0120  _...sx......... 
+00001450: 0108 020e 0208 020a 010a 010a fe04 0312  ................
+00001460: 011a 0134 0210 0410 0110 030c 0104 0108  ...4............
+00001470: fe06 0610 0104 ff06 030e 0310 021a 0404  ................
+00001480: 0104 0104 0104 010a 0108 fb06 0710 0208  ................
+00001490: 0210 011a 0112 0124 0208 010e 0104 0106  .......$........
+000014a0: 0220 0120 0118 010e 010a 0204 020e 010c  . . ............
+000014b0: 060a 0104 0104 020e 0104 0104 0208 020e  ................
+000014c0: 027a 1052 6f76 6572 4172 6d45 6e76 2e73  .z.RoverArmEnv.s
+000014d0: 7465 704e 6303 0000 0000 0000 0000 0000  tepNc...........
+000014e0: 000c 0000 0008 0000 0043 0000 0073 4201  .........C...sB.
+000014f0: 0000 7c01 6400 6b02 7310 7c02 6400 6b02  ..|.d.k.s.|.d.k.
+00001500: 721c 7c00 6a00 7d01 7c00 6a01 7d02 7c00  r.|.j.}.|.j.}.|.
+00001510: 6a02 6401 6b03 722a 6400 5300 7403 6a04  j.d.k.r*d.S.t.j.
+00001520: 7c00 6a05 7c00 6a06 7c00 6a07 7c00 6a08  |.j.|.j.|.j.|.j.
+00001530: 6402 6403 6404 8d06 7d03 7403 6a04 6700  d.d.d...}.t.j.g.
+00001540: 6405 a201 6406 6407 6408 6402 6403 6404  d...d.d.d.d.d.d.
+00001550: 8d06 7d04 7403 6a09 6409 740a 7c01 8301  ..}.t.j.d.t.|...
+00001560: 7c02 1b00 640a 640b 640c 8d04 7d05 7403  |...d.d.d...}.t.
+00001570: 6a0b 7c01 7c02 7c03 7c05 7403 6a0c 640d  j.|.|.|.|.t.j.d.
+00001580: 8d05 5c05 7d06 7d06 7d07 7d06 7d06 7403  ..\.}.}.}.}.}.t.
+00001590: 6a0b 7c01 7c02 7c04 7c05 7403 6a0c 640d  j.|.|.|.|.t.j.d.
+000015a0: 8d05 5c05 7d06 7d06 7d08 7d06 7d06 740d  ..\.}.}.}.}.}.t.
+000015b0: 6a0e 7c07 740d 6a0f 640e 8d02 7d09 740d  j.|.t.j.d...}.t.
+000015c0: a010 7c09 7c02 7c01 640f 6603 a102 6400  ..|.|.|.d.f...d.
+000015d0: 6400 8502 6400 6400 8502 6400 6410 8502  d...d.d...d.d...
+000015e0: 6603 1900 7d09 740d 6a0e 7c08 740d 6a0f  f...}.t.j.|.t.j.
+000015f0: 640e 8d02 7d0a 740d a010 7c0a 7c02 7c01  d...}.t...|.|.|.
+00001600: 640f 6603 a102 6400 6400 8502 6400 6400  d.f...d.d...d.d.
+00001610: 8502 6400 6410 8502 6603 1900 7d0a 740d  ..d.d...f...}.t.
+00001620: 6a11 7c09 7c0a 6602 6402 6411 8d02 7d0b  j.|.|.f.d.d...}.
+00001630: 7c0b 5300 2912 4e72 0800 0000 7201 0000  |.S.).Nr....r...
+00001640: 0072 1600 0000 2906 720e 0000 00da 0864  .r....).r......d
+00001650: 6973 7461 6e63 655a 0379 6177 5a05 7069  istanceZ.yawZ.pi
+00001660: 7463 68da 0472 6f6c 6c5a 0b75 7041 7869  tch..rollZ.upAxi
+00001670: 7349 6e64 6578 2903 e766 6666 6666 66e6  sIndex)..ffffff.
+00001680: 3f72 0100 0000 7244 0000 0072 8c00 0000  ?r....rD...r....
+00001690: e95a 0000 0069 baff ffff e93c 0000 0067  .Z...i.....<...g
+000016a0: 9a99 9999 9999 b93f 6700 0000 0000 0059  .......?g......Y
+000016b0: 4029 045a 0366 6f76 da06 6173 7065 6374  @).Z.fov..aspect
+000016c0: 5a07 6e65 6172 5661 6c5a 0666 6172 5661  Z.nearValZ.farVa
+000016d0: 6c29 0572 3600 0000 7237 0000 005a 0a76  l).r6...r7...Z.v
+000016e0: 6965 774d 6174 7269 785a 1070 726f 6a65  iewMatrixZ.proje
+000016f0: 6374 696f 6e4d 6174 7269 785a 0872 656e  ctionMatrixZ.ren
+00001700: 6465 7265 7229 01da 0564 7479 7065 7211  derer)...dtyper.
+00001710: 0000 0072 0c00 0000 2901 da04 6178 6973  ...r....)...axis
+00001720: 2912 721c 0000 0072 1d00 0000 7219 0000  ).r....r....r...
+00001730: 0072 1e00 0000 da21 636f 6d70 7574 6556  .r.....!computeV
+00001740: 6965 774d 6174 7269 7846 726f 6d59 6177  iewMatrixFromYaw
+00001750: 5069 7463 6852 6f6c 6c72 2700 0000 7224  PitchRollr'...r$
+00001760: 0000 0072 2500 0000 7226 0000 00da 1a63  ...r%...r&.....c
+00001770: 6f6d 7075 7465 5072 6f6a 6563 7469 6f6e  omputeProjection
+00001780: 4d61 7472 6978 464f 56da 0566 6c6f 6174  MatrixFOV..float
+00001790: da0e 6765 7443 616d 6572 6149 6d61 6765  ..getCameraImage
+000017a0: da19 4552 5f42 554c 4c45 545f 4841 5244  ..ER_BULLET_HARD
+000017b0: 5741 5245 5f4f 5045 4e47 4c72 2900 0000  WARE_OPENGLr)...
+000017c0: 722a 0000 00da 0575 696e 7438 da07 7265  r*.....uint8..re
+000017d0: 7368 6170 65da 0b63 6f6e 6361 7465 6e61  shape..concatena
+000017e0: 7465 290c 7235 0000 0072 3600 0000 7237  te).r5...r6...r7
+000017f0: 0000 005a 0c76 6965 775f 6d61 7472 6978  ...Z.view_matrix
+00001800: 315a 0c76 6965 775f 6d61 7472 6978 325a  1Z.view_matrix2Z
+00001810: 0b70 726f 6a5f 6d61 7472 6978 7280 0000  .proj_matrixr...
+00001820: 005a 0370 7831 5a03 7078 325a 0a72 6762  .Z.px1Z.px2Z.rgb
+00001830: 5f61 7272 6179 315a 0a72 6762 5f61 7272  _array1Z.rgb_arr
+00001840: 6179 3272 0800 0000 7238 0000 0072 3800  ay2r....r8...r8.
+00001850: 0000 7239 0000 00da 0672 656e 6465 72be  ..r9.....render.
+00001860: 0000 0073 5400 0000 0007 1001 0601 0601  ...sT...........
+00001870: 0a01 0401 0801 0401 0401 0401 0201 02fb  ................
+00001880: 0606 0a01 0201 0201 0201 0201 02fb 0606  ................
+00001890: 0601 0a01 0201 02fd 0605 0601 0201 0201  ................
+000018a0: 0201 04fc 1006 0601 0201 0201 0201 04fc  ................
+000018b0: 1006 1001 2802 1001 2803 1202 7a12 526f  ....(...(...z.Ro
+000018c0: 7665 7241 726d 456e 762e 7265 6e64 6572  verArmEnv.render
+000018d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000018e0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+000018f0: 6a00 5300 726d 0000 0029 0172 5a00 0000  j.S.rm...).rZ...
+00001900: 726f 0000 0072 3800 0000 7238 0000 0072  ro...r8...r8...r
+00001910: 3900 0000 da0a 5f67 6574 5f73 7461 7465  9....._get_state
+00001920: f200 0000 7302 0000 0000 017a 1652 6f76  ....s......z.Rov
+00001930: 6572 4172 6d45 6e76 2e5f 6765 745f 7374  erArmEnv._get_st
+00001940: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+00001950: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00001960: 0074 00a0 01a1 0001 0064 0053 0072 6d00  .t.......d.S.rm.
+00001970: 0000 2902 721e 0000 00da 0a64 6973 636f  ..).r......disco
+00001980: 6e6e 6563 7472 6f00 0000 7238 0000 0072  nnectro...r8...r
+00001990: 3800 0000 7239 0000 00da 0563 6c6f 7365  8...r9.....close
+000019a0: f500 0000 7302 0000 0000 017a 1152 6f76  ....s......z.Rov
+000019b0: 6572 4172 6d45 6e76 2e63 6c6f 7365 2902  erArmEnv.close).
+000019c0: 4e4e 290c da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
+000019d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000019e0: 616c 6e61 6d65 5f5f da08 6d65 7461 6461  alname__..metada
+000019f0: 7461 da0d 7079 6275 6c6c 6574 5f64 6174  ta..pybullet_dat
+00001a00: 615a 0b67 6574 4461 7461 5061 7468 723a  aZ.getDataPathr:
+00001a10: 0000 0072 6300 0000 7289 0000 0072 9a00  ...rc...r....r..
+00001a20: 0000 729b 0000 0072 9d00 0000 7238 0000  ..r....r....r8..
+00001a30: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
+00001a40: 7206 0000 000e 0000 0073 1200 0000 0801  r........s......
+00001a50: 0c02 0c01 04ff 0a27 0827 085f 0a34 0803  .......'.'._.4..
+00001a60: 7206 0000 0029 12da 0967 796d 6e61 7369  r....)...gymnasi
+00001a70: 756d da03 6779 6d72 0200 0000 7203 0000  um..gymr....r...
+00001a80: 0072 0400 0000 da0f 6779 6d6e 6173 6975  .r......gymnasiu
+00001a90: 6d2e 7574 696c 7372 0500 0000 724c 0000  m.utilsr....rL..
+00001aa0: 00da 0870 7962 756c 6c65 7472 1e00 0000  ...pybulletr....
+00001ab0: 72a2 0000 0072 7300 0000 da05 6e75 6d70  r....rs.....nump
+00001ac0: 7972 2900 0000 724f 0000 0072 5200 0000  yr)...rO...rR...
+00001ad0: da03 456e 7672 0600 0000 7238 0000 0072  ..Envr....r8...r
+00001ae0: 3800 0000 7238 0000 0072 3900 0000 da08  8...r8...r9.....
+00001af0: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
+00001b00: 0008 0114 010c 0208 0108 0108 0108 0108  ................
+00001b10: 0108 0108 03                             .....
```

### Comparing `rover_arm-1.0.7/rover_arm/envs/roverarm_env.py` & `rover_arm-1.0.8/rover_arm/envs/roverarm_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import gym 
-from gym import error, spaces, utils
-from gym.utils import seeding
+import gymnasium as gym 
+from gymnasium import error, spaces, utils
+from gymnasium.utils import seeding
 
 import os
 import pybullet as p
 import pybullet_data
 import math
 import numpy as np
 import random
@@ -64,14 +64,15 @@
 
         rest_poses = [0,-0.215,0,-2.57,0,2.356,2.356,0.08,0.08]
         
         x_pos = np.random.choice([random.uniform(-1, -0.3), random.uniform(1.25,2)])
         y_pos = random.uniform(-1, 2.5)
         
         BASE_DIR = site.getsitepackages()[0] + "/rover_arm/data/"
+        BASE_DIR = "./rover_arm/data/"
         self.roverarmUid = p.loadURDF(BASE_DIR + "rover_arm.xml", basePosition=[ x_pos, y_pos ,-0.5])
 
 
         for i in range(7,14):
             p.resetJointState(self.roverarmUid,i, rest_poses[i - 7])
         p.resetJointState(self.roverarmUid, 16, 0.07)
         p.resetJointState(self.roverarmUid, 17, 0.07)
```

### Comparing `rover_arm-1.0.7/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.0.8/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.0.8/rover_arm/envs/roverarm_env_place.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import gym 
-from gym import error, spaces, utils
-from gym.utils import seeding
+import gymnasium as gym 
+from gymnasium import error, spaces, utils
+from gymnasium.utils import seeding
 
 import os
 import pybullet as p
 import pybullet_data
 import math
 import numpy as np
 import random
```

### Comparing `rover_arm-1.0.7/rover_arm/keyboard_control.py` & `rover_arm-1.0.8/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.0.8/rover_arm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover-arm
-Version: 1.0.7
+Version: 1.0.8
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.0.7/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.0.8/rover_arm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.7/setup.py` & `rover_arm-1.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.0.7',
+    version='1.0.8',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
```


# Comparing `tmp/rover_arm-1.0.8.tar.gz` & `tmp/rover_arm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.0.8.tar", last modified: Thu Apr 27 19:34:05 2023, max compression
+gzip compressed data, was "rover_arm-1.0.9.tar", last modified: Thu Apr 27 19:47:40 2023, max compression
```

## Comparing `rover_arm-1.0.8.tar` & `rover_arm-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.815303 rover_arm-1.0.8/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.0.8/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.0.8/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.0.8/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:34:05.815164 rover_arm-1.0.8/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.0.8/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.802462 rover_arm-1.0.8/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.0.8/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.0.8/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803338 rover_arm-1.0.8/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803532 rover_arm-1.0.8/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.805682 rover_arm-1.0.8/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.813129 rover_arm-1.0.8/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.0.8/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.814723 rover_arm-1.0.8/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.0.8/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.814967 rover_arm-1.0.8/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.0.8/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     6933 2023-04-27 19:31:10.000000 rover_arm-1.0.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    10582 2023-04-27 19:31:07.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.0.8/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2371 2023-03-29 22:55:55.000000 rover_arm-1.0.8/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:34:05.803041 rover_arm-1.0.8/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-04-27 19:34:05.000000 rover_arm-1.0.8/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-04-27 19:34:05.815350 rover_arm-1.0.8/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-04-27 19:34:03.000000 rover_arm-1.0.8/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.673194 rover_arm-1.0.9/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.0.9/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.0.9/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.0.9/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:47:40.673049 rover_arm-1.0.9/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.0.9/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.660527 rover_arm-1.0.9/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.0.9/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.0.9/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.661520 rover_arm-1.0.9/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.661712 rover_arm-1.0.9/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.663356 rover_arm-1.0.9/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.669111 rover_arm-1.0.9/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.0.9/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.672449 rover_arm-1.0.9/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.0.9/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.672805 rover_arm-1.0.9/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.0.9/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6933 2023-04-27 19:31:10.000000 rover_arm-1.0.9/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10584 2023-04-27 19:46:59.000000 rover_arm-1.0.9/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.0.9/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.0.9/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2371 2023-03-29 22:55:55.000000 rover_arm-1.0.9/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-04-27 19:47:40.661223 rover_arm-1.0.9/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-04-27 19:47:40.000000 rover_arm-1.0.9/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-04-27 19:47:40.000000 rover_arm-1.0.9/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-04-27 19:47:40.000000 rover_arm-1.0.9/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-04-27 19:47:40.000000 rover_arm-1.0.9/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-04-27 19:47:40.000000 rover_arm-1.0.9/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-04-27 19:47:40.673246 rover_arm-1.0.9/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-04-27 19:47:35.000000 rover_arm-1.0.9/setup.py
```

### Comparing `rover_arm-1.0.8/.DS_Store` & `rover_arm-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/PKG-INFO` & `rover_arm-1.0.9/rover_arm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover_arm
-Version: 1.0.8
+Name: rover-arm
+Version: 1.0.9
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.0.8/README.md` & `rover_arm-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/.DS_Store` & `rover_arm-1.0.9/rover_arm/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.0.9/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.0.9/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/panda.urdf` & `rover_arm-1.0.9/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/data/rover_arm.xml` & `rover_arm-1.0.9/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.0.9/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/envs/roverarm_env.py` & `rover_arm-1.0.9/rover_arm/envs/roverarm_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         rest_poses = [0,-0.215,0,-2.57,0,2.356,2.356,0.08,0.08]
         
         x_pos = np.random.choice([random.uniform(-1, -0.3), random.uniform(1.25,2)])
         y_pos = random.uniform(-1, 2.5)
         
         BASE_DIR = site.getsitepackages()[0] + "/rover_arm/data/"
-        BASE_DIR = "./rover_arm/data/"
+        # BASE_DIR = "./rover_arm/data/"
         self.roverarmUid = p.loadURDF(BASE_DIR + "rover_arm.xml", basePosition=[ x_pos, y_pos ,-0.5])
 
 
         for i in range(7,14):
             p.resetJointState(self.roverarmUid,i, rest_poses[i - 7])
         p.resetJointState(self.roverarmUid, 16, 0.07)
         p.resetJointState(self.roverarmUid, 17, 0.07)
```

### Comparing `rover_arm-1.0.8/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.0.9/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.0.9/rover_arm/envs/roverarm_env_place.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm/keyboard_control.py` & `rover_arm-1.0.9/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover-arm
-Version: 1.0.8
+Name: rover_arm
+Version: 1.0.9
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.0.8/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.0.9/rover_arm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover_arm-1.0.8/setup.py` & `rover_arm-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.0.8',
+    version='1.0.9',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
```


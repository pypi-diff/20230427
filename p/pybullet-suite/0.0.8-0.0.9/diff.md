# Comparing `tmp/pybullet_suite-0.0.8.tar.gz` & `tmp/pybullet_suite-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybullet_suite-0.0.8.tar", last modified: Thu Mar 23 14:44:22 2023, max compression
+gzip compressed data, was "pybullet_suite-0.0.9.tar", last modified: Fri Mar 24 00:50:43 2023, max compression
```

## Comparing `pybullet_suite-0.0.8.tar` & `pybullet_suite-0.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       59 2023-03-23 14:19:34.000000 pybullet_suite-0.0.8/MANIFEST.in
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      197 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/PKG-INFO
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      442 2023-03-23 09:21:36.000000 pybullet_suite-0.0.8/README.md
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       62 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/__init__.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      280 2023-03-23 14:08:50.000000 pybullet_suite-0.0.8/pybullet_suite/assets/__init__.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/__pycache__/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      421 2023-03-23 09:16:16.000000 pybullet_suite-0.0.8/pybullet_suite/assets/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    10172 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/LICENSE.txt
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 13:29:55.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/__init__.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    11277 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/franka_panda.urdf
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     2529 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/hand.urdf
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     7603 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/finger.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    15247 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/hand.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    14925 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link0.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22976 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link1.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22688 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link2.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22870 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link3.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    68016 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link4.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    67745 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link5.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3827 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)   140218 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    45132 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link7.obj
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    33337 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/colors.png
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      481 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    65359 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     1132 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)   713204 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      262 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1070650 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      261 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1084458 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      931 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1237175 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      925 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1272305 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      676 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1582192 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3552 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.mtl
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  2236857 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.obj
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    26999 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/visualShapeBench.json_0.json
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3581 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/panda_hand.urdf
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/pybullet_suite/base/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      101 2023-03-23 05:11:14.000000 pybullet_suite-0.0.8/pybullet_suite/base/__init__.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     9651 2023-03-23 04:48:15.000000 pybullet_suite-0.0.8/pybullet_suite/base/body.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3705 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/base/camera.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      196 2023-03-23 14:43:44.000000 pybullet_suite-0.0.8/pybullet_suite/base/data.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4818 2023-02-03 02:47:09.000000 pybullet_suite-0.0.8/pybullet_suite/base/robot.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     5840 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/base/tf.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    16139 2023-03-23 11:46:27.000000 pybullet_suite-0.0.8/pybullet_suite/base/world.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/pybullet_suite/robots/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       66 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/robots/__init__.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      888 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/robots/dualarm.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4650 2023-03-23 14:34:35.000000 pybullet_suite-0.0.8/pybullet_suite/robots/gripper.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4375 2023-03-23 14:34:16.000000 pybullet_suite-0.0.8/pybullet_suite/robots/panda.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/pybullet_suite/utils/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       26 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/utils/__init__.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    17183 2023-03-08 13:08:37.000000 pybullet_suite-0.0.8/pybullet_suite/utils/scene_maker.py
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      361 2022-12-22 13:39:30.000000 pybullet_suite-0.0.8/pybullet_suite/utils/utils.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.019338 pybullet_suite-0.0.8/pybullet_suite.egg-info/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      197 2023-03-23 14:44:21.000000 pybullet_suite-0.0.8/pybullet_suite.egg-info/PKG-INFO
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     2756 2023-03-23 14:44:21.000000 pybullet_suite-0.0.8/pybullet_suite.egg-info/SOURCES.txt
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)        1 2023-03-23 14:44:21.000000 pybullet_suite-0.0.8/pybullet_suite.egg-info/dependency_links.txt
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       29 2023-03-23 14:44:21.000000 pybullet_suite-0.0.8/pybullet_suite.egg-info/requires.txt
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       15 2023-03-23 14:44:21.000000 pybullet_suite-0.0.8/pybullet_suite.egg-info/top_level.txt
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       38 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/setup.cfg
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      958 2023-03-23 14:44:15.000000 pybullet_suite-0.0.8/setup.py
-drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 14:44:22.027338 pybullet_suite-0.0.8/test/
--rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     1033 2023-03-23 11:52:59.000000 pybullet_suite-0.0.8/test/test.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       59 2023-03-23 14:19:34.000000 pybullet_suite-0.0.9/MANIFEST.in
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      197 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/PKG-INFO
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      442 2023-03-23 09:21:36.000000 pybullet_suite-0.0.9/README.md
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       62 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/__init__.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      280 2023-03-23 14:08:50.000000 pybullet_suite-0.0.9/pybullet_suite/assets/__init__.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/__pycache__/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      421 2023-03-23 09:16:16.000000 pybullet_suite-0.0.9/pybullet_suite/assets/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    10172 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/LICENSE.txt
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-23 13:29:55.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/__init__.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    11277 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/franka_panda.urdf
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     2529 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/hand.urdf
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     7603 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/finger.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    15247 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/hand.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    14925 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link0.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22976 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link1.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22688 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link2.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    22870 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link3.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    68016 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link4.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    67745 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link5.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3827 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)   140218 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    45132 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link7.obj
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.612798 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    33337 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/colors.png
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      481 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    65359 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     1132 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)   713204 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      262 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1070650 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      261 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1084458 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      931 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1237175 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      925 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1272305 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      676 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  1582192 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3552 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.mtl
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)  2236857 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.obj
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    26999 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/visualShapeBench.json_0.json
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3581 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/panda_hand.urdf
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/pybullet_suite/base/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      101 2023-03-23 05:11:14.000000 pybullet_suite-0.0.9/pybullet_suite/base/__init__.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     9651 2023-03-23 04:48:15.000000 pybullet_suite-0.0.9/pybullet_suite/base/body.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     3705 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/base/camera.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      196 2023-03-23 14:43:44.000000 pybullet_suite-0.0.9/pybullet_suite/base/data.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4818 2023-02-03 02:47:09.000000 pybullet_suite-0.0.9/pybullet_suite/base/robot.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     5840 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/base/tf.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    16139 2023-03-23 11:46:27.000000 pybullet_suite-0.0.9/pybullet_suite/base/world.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/pybullet_suite/robots/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       66 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/robots/__init__.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      888 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/robots/dualarm.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4650 2023-03-23 14:34:35.000000 pybullet_suite-0.0.9/pybullet_suite/robots/gripper.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     4375 2023-03-23 14:34:16.000000 pybullet_suite-0.0.9/pybullet_suite/robots/panda.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/pybullet_suite/utils/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       26 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/utils/__init__.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)    17107 2023-03-24 00:47:35.000000 pybullet_suite-0.0.9/pybullet_suite/utils/scene_maker.py
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      361 2022-12-22 13:39:30.000000 pybullet_suite-0.0.9/pybullet_suite/utils/utils.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.604798 pybullet_suite-0.0.9/pybullet_suite.egg-info/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      197 2023-03-24 00:50:43.000000 pybullet_suite-0.0.9/pybullet_suite.egg-info/PKG-INFO
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     2756 2023-03-24 00:50:43.000000 pybullet_suite-0.0.9/pybullet_suite.egg-info/SOURCES.txt
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)        1 2023-03-24 00:50:43.000000 pybullet_suite-0.0.9/pybullet_suite.egg-info/dependency_links.txt
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       29 2023-03-24 00:50:43.000000 pybullet_suite-0.0.9/pybullet_suite.egg-info/requires.txt
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       15 2023-03-24 00:50:43.000000 pybullet_suite-0.0.9/pybullet_suite.egg-info/top_level.txt
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)       38 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/setup.cfg
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)      958 2023-03-24 00:50:38.000000 pybullet_suite-0.0.9/setup.py
+drwxrwxr-x   0 kh11kim   (1000) kh11kim   (1000)        0 2023-03-24 00:50:43.616798 pybullet_suite-0.0.9/test/
+-rw-rw-r--   0 kh11kim   (1000) kh11kim   (1000)     1055 2023-03-24 00:48:32.000000 pybullet_suite-0.0.9/test/test.py
```

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/LICENSE.txt` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/franka_panda.urdf` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/franka_panda.urdf`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/hand.urdf` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/hand.urdf`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/finger.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/hand.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link0.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link1.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link2.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link3.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link4.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link5.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/collision/link7.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/colors.png` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.mtl` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.obj` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/meshes/visual/visualShapeBench.json_0.json` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/meshes/visual/visualShapeBench.json_0.json`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/assets/urdfs/panda/panda_hand.urdf` & `pybullet_suite-0.0.9/pybullet_suite/assets/urdfs/panda/panda_hand.urdf`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/base/body.py` & `pybullet_suite-0.0.9/pybullet_suite/base/body.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/base/camera.py` & `pybullet_suite-0.0.9/pybullet_suite/base/camera.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/base/robot.py` & `pybullet_suite-0.0.9/pybullet_suite/base/robot.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/base/tf.py` & `pybullet_suite-0.0.9/pybullet_suite/base/tf.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/base/world.py` & `pybullet_suite-0.0.9/pybullet_suite/base/world.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/robots/dualarm.py` & `pybullet_suite-0.0.9/pybullet_suite/robots/dualarm.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/robots/gripper.py` & `pybullet_suite-0.0.9/pybullet_suite/robots/gripper.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/robots/panda.py` & `pybullet_suite-0.0.9/pybullet_suite/robots/panda.py`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/pybullet_suite/utils/scene_maker.py` & `pybullet_suite-0.0.9/pybullet_suite/utils/scene_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,15 @@
         
     def create_cylinder(
         self,
         body_name: str,
         radius: float,
         height: float,
         mass: float,
-        position: np.ndarray,
-        orientation: None,
+        pose: Pose,
         rgba_color: Optional[np.ndarray] = np.zeros(4),
         specular_color: np.ndarray = np.zeros(3),
         ghost: bool = False,
         lateral_friction: Optional[float] = None,
         spinning_friction: Optional[float] = None,
     ) -> Body:
         """Create a cylinder.
@@ -158,16 +157,15 @@
             "rgbaColor": rgba_color,
         }
         collision_kwargs = {"radius": radius, "height": height}
         return self._create_geometry(
             body_name,
             geom_type=self.physics_client.GEOM_CYLINDER,
             mass=mass,
-            position=position,
-            orientation=orientation,
+            pose=pose,
             ghost=ghost,
             lateral_friction=lateral_friction,
             spinning_friction=spinning_friction,
             visual_kwargs=visual_kwargs,
             collision_kwargs=collision_kwargs,
         )
 
@@ -223,15 +221,15 @@
             z_offset (float): Offset of the plane.
         """
         body_name = "plane"
         return self.create_box(
             body_name=body_name,
             half_extents=np.array([3.0, 3.0, 0.01]),
             mass=0.0,
-            position=np.array([0.0, 0.0, z_offset - 0.01]),
+            pose=Pose(trans=[0.0, 0.0, z_offset - 0.01]),
             specular_color=np.zeros(3),
             rgba_color=np.array([0.85, 0.85, 0.85, 1.0]),
         )
 
     def create_table(
         self,
         body_name: str,
@@ -269,15 +267,15 @@
     
     def make_sphere_obstacle(self, name, position, rgb_color=[0.,0.,1.]):
         if not name in self.world.bodies:
             self.create_sphere(
                 body_name=name,
                 radius=0.02,
                 mass=0.0,
-                position=position,
+                pose=Pose(trans=position),
                 rgba_color=[*rgb_color,0.3],
                 ghost=False
             )
         else:
             body = self.world.bodies[name]
             pose = Pose(Rotation.Identity(), position)
             body.set_base_pose(name, pose)
```

### Comparing `pybullet_suite-0.0.8/pybullet_suite.egg-info/SOURCES.txt` & `pybullet_suite-0.0.9/pybullet_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybullet_suite-0.0.8/setup.py` & `pybullet_suite-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       ext = os.path.splitext(fn)[1][1:]
       if ext and ext in 'yaml index meta data-00000-of-00001 png gif jpg urdf sdf obj txt mtl dae off stl STL xml gin npy '.split():
          fn = root + "/" + fn
          need_files.append(datadir+"/"+fn[1 + len(hh):])
 
 setup(
    name='pybullet_suite',
-   version='0.0.8', 
+   version='0.0.9', 
    description='Pybullet wrapper for easy use',
    author='Kanghyun Kim',
    author_email='kh11kim@kaist.ac.kr',
    packages=find_packages(),  #same as name
    install_requires=[
       "numpy",
       "scipy",
```

### Comparing `pybullet_suite-0.0.8/test/test.py` & `pybullet_suite-0.0.9/test/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 world = BulletWorld(gui=True)
 robot: Panda = world.load_robot(name="robot", robot_class=Panda)
 robot.set_joint_angles([0,0,0,-1,-1,-1,0])
 
 
 sm = BulletSceneMaker(world)
-box = sm.create_box("table", [0.5, 0.5, 0.5], 1,
-                    pose=Pose(trans=[0,0,0]))
+sm.create_plane()
+# box = sm.create_box("table", [0.5, 0.5, 0.5], 1,
+#                     pose=Pose(trans=[0,0,0]))
 world.set_view([1.7, -0.4, 1.], [0,0,0])
 # get_contact_points
 tic = time.time()
 #world.step(only_collision_detection=True)
 
 points = world.physics_client.getContactPoints(robot.uid)
 elapsed = time.time() - tic
```


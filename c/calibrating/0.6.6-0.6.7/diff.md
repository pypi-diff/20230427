# Comparing `tmp/calibrating-0.6.6.tar.gz` & `tmp/calibrating-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibrating-0.6.6.tar", last modified: Wed Apr 26 05:52:59 2023, max compression
+gzip compressed data, was "dist/calibrating-0.6.7.tar", last modified: Thu Apr 27 03:23:07 2023, max compression
```

## Comparing `calibrating-0.6.6.tar` & `calibrating-0.6.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.6/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-26 05:52:59.000000 calibrating-0.6.6/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.6/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/calibrating/
--rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-26 05:47:41.000000 calibrating-0.6.6/calibrating/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      280 2023-04-25 05:33:13.000000 calibrating-0.6.6/calibrating/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.6/calibrating/boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21816 2023-04-23 07:58:22.000000 calibrating-0.6.6/calibrating/camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.6/calibrating/feature_libs.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.6/calibrating/multi_boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.6/calibrating/reconstruction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    17456 2023-04-25 06:03:55.000000 calibrating-0.6.6/calibrating/stereo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6901 2023-04-26 05:50:03.000000 calibrating-0.6.6/calibrating/stereo_matching.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    26459 2023-04-25 07:15:58.000000 calibrating-0.6.6/calibrating/utils.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-26 05:52:59.000000 calibrating-0.6.6/calibrating.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      473 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-26 05:52:58.000000 calibrating-0.6.6/calibrating.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.6/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-26 05:52:59.000000 calibrating-0.6.6/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.6/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:07.000000 calibrating-0.6.7/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.7/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-27 03:23:07.000000 calibrating-0.6.7/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.7/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-27 03:21:56.000000 calibrating-0.6.7/calibrating/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      280 2023-04-25 05:33:13.000000 calibrating-0.6.7/calibrating/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.7/calibrating/boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    22684 2023-04-27 03:22:15.000000 calibrating-0.6.7/calibrating/camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.7/calibrating/feature_libs.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.7/calibrating/multi_boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.7/calibrating/reconstruction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    17456 2023-04-25 06:03:55.000000 calibrating-0.6.7/calibrating/stereo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6901 2023-04-26 05:50:03.000000 calibrating-0.6.7/calibrating/stereo_matching.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    27170 2023-04-27 03:22:15.000000 calibrating-0.6.7/calibrating/utils.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:07.000000 calibrating-0.6.7/calibrating.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      473 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.7/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-27 03:23:07.000000 calibrating-0.6.7/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.7/setup.py
```

### Comparing `calibrating-0.6.6/PKG-INFO` & `calibrating-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.6
+Version: 0.6.7
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.6/README.md` & `calibrating-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/__info__.py` & `calibrating-0.6.7/calibrating/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 __description__ = "Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibrating-0.6.6/calibrating/boards.py` & `calibrating-0.6.7/calibrating/boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/camera.py` & `calibrating-0.6.7/calibrating/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,14 +465,37 @@
         for idx in range(k):
             dic["xy"] = dic["xy"][::-1]
             dic["fx"], dic["fy"] = dic["fy"], dic["fx"]
             dic["cx"], dic["cy"] = dic["xy"][0] - dic["cy"], dic["cx"]
         new = type(self).load(dic)
         return new
 
+    def crop(self, udlr_or_slice, set_D_zero=True):
+        assert not self.D.any() or set_D_zero
+        cam_croped = self.copy()
+        if isinstance(udlr_or_slice[0], slice):
+            u, d, l, r = (
+                udlr_or_slice[0].start,
+                udlr_or_slice[0].stop,
+                udlr_or_slice[1].start,
+                udlr_or_slice[1].stop,
+            )
+        else:
+            u, d, l, r = udlr_or_slice
+        cam_croped.K[0, 2] -= l
+        cam_croped.K[1, 2] -= u
+        cam_croped.xy = r - l, d - u
+        if set_D_zero:
+            cam_croped.D = np.zeros_like(cam_croped.D)
+        return cam_croped
+
+    def resize(self, reize_arg):
+        # like boxx.resize's arg
+        raise NotImplemented("")
+
     @property
     def fx(self):
         return self.K[0, 0]
 
     @property
     def fy(self):
         return self.K[1, 1]
@@ -483,14 +506,15 @@
 
     @property
     def cy(self):
         return self.K[1, 2]
 
     @property
     def fovs(self):
+        # TODO 两个点来通过 depth 1 的点云计算 fov, 并在 stereo.cam1.crop([0,900,0,1250]) 上验证是否刚好一半
         fovx = 2 * boxx.arctan(self.xy[0] / 2 / self.fx)
         fovy = 2 * boxx.arctan(self.xy[1] / 2 / self.fy)
         fov = 2 * boxx.arctan(
             (boxx.tan(fovx / 2) ** 2 + boxx.tan(fovy / 2) ** 2) ** 0.5
         )
         return dict(fov=fov, fovx=fovx, fovy=fovy)
```

### Comparing `calibrating-0.6.6/calibrating/feature_libs.py` & `calibrating-0.6.7/calibrating/feature_libs.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/multi_boards.py` & `calibrating-0.6.7/calibrating/multi_boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/reconstruction.py` & `calibrating-0.6.7/calibrating/reconstruction.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/stereo.py` & `calibrating-0.6.7/calibrating/stereo.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/stereo_matching.py` & `calibrating-0.6.7/calibrating/stereo_matching.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.6/calibrating/utils.py` & `calibrating-0.6.7/calibrating/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,36 @@
         r = r_R_T
     elif r_R_T.size >= 9:
         r = T_to_r(r_R_T).squeeze()
     deg = np.linalg.norm(r) * 180 / np.pi
     return deg
 
 
+def round_R(R):
+    """
+    Round a rotation matrix to the nearest axis-aligned rotation matrix.
+
+    This function finds the nearest rotation matrix where all rotation angles
+    are multiples of 90 degrees, and the rotated coordinate axes are parallel
+    to the original coordinate axes.
+
+    Parameters:
+    R (numpy.array): The input rotation matrix.
+
+    Returns:
+    R_round (numpy.array): The rounded, axis-aligned rotation matrix.
+    """
+    R_round = np.zeros((3, 3))
+    # Assign 1 to the maximum absolute value in each row of R
+    R_round[range(3), np.abs(R).argmax(1)] = 1
+    # Correct the sign of the elements in R_round based on the input R
+    R_round *= 1 - 2 * (R < 0)
+    return R_round
+
+
 def T_to_deg_distance(T, compare_T=None):
     """
     Translate the T matrix into items that humans can intuitively understand,
     such as degrees of rotation and displacement distances
     Set compare_T to compare the difference between two Ts
 
     Returns
```

### Comparing `calibrating-0.6.6/calibrating.egg-info/PKG-INFO` & `calibrating-0.6.7/calibrating.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.6
+Version: 0.6.7
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.6/setup.py` & `calibrating-0.6.7/setup.py`

 * *Files identical despite different names*


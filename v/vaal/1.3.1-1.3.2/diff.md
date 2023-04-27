# Comparing `tmp/vaal-1.3.1-py3-none-any.whl.zip` & `tmp/vaal-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11278 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      453 b- defN 23-Apr-27 17:49 deepview/vaal/__init__.py
--rw-rw-r--  2.0 unx     1514 b- defN 23-Apr-27 17:49 deepview/vaal/camera.py
--rw-rw-r--  2.0 unx    10634 b- defN 23-Apr-27 17:49 deepview/vaal/context.py
--rw-rw-r--  2.0 unx     7879 b- defN 23-Apr-27 17:49 deepview/vaal/library.py
--rw-rw-r--  2.0 unx    11710 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      229 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/RECORD
-9 files, 33218 bytes uncompressed, 10084 bytes compressed:  69.6%
+Zip file size: 11386 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      453 b- defN 23-Apr-27 21:32 deepview/vaal/__init__.py
+-rw-rw-r--  2.0 unx     1514 b- defN 23-Apr-27 21:32 deepview/vaal/camera.py
+-rw-rw-r--  2.0 unx    11346 b- defN 23-Apr-27 21:32 deepview/vaal/context.py
+-rw-rw-r--  2.0 unx     7879 b- defN 23-Apr-27 21:32 deepview/vaal/library.py
+-rw-rw-r--  2.0 unx    11710 b- defN 23-Apr-27 21:36 vaal-1.3.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      229 b- defN 23-Apr-27 21:36 vaal-1.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 21:36 vaal-1.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-27 21:36 vaal-1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 23-Apr-27 21:36 vaal-1.3.2.dist-info/RECORD
+9 files, 33930 bytes uncompressed, 10192 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: deepview/vaal/context.py
 Comment: 
 
 Filename: deepview/vaal/library.py
 Comment: 
 
-Filename: vaal-1.3.1.dist-info/LICENSE.txt
+Filename: vaal-1.3.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vaal-1.3.1.dist-info/METADATA
+Filename: vaal-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: vaal-1.3.1.dist-info/WHEEL
+Filename: vaal-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: vaal-1.3.1.dist-info/top_level.txt
+Filename: vaal-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vaal-1.3.1.dist-info/RECORD
+Filename: vaal-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepview/vaal/context.py

```diff
@@ -215,61 +215,74 @@
         err = lib.vaal_boxes(self._handle, byref(bxs), len(bxs), byref(n_bxs))
         if err != 0:
             raise RuntimeError('failed to get boxes: %s' % strerror(err))
         if n_bxs.value > 0:
             return bxs[0:n_bxs.value]
         return []
 
-    def load_image(self, image, tensor=None):
+    def load_image(self, image, tensor=None, roi=None):
         if tensor is not None:
             import deepview.rt as rt
             tensor_ptr = rt.ffi.cast('intptr_t', tensor.ptr)
             tensor_ptr = cast(int(tensor_ptr), c_void_p)
         else:
             tensor_ptr = None
+        
+        c_roi = None
+        if roi is not None:
+            c_roi = (c_int32 * 4)(*roi)
 
         if isinstance(image, str):
             err = lib.vaal_load_image_file(
-                self._handle, tensor_ptr, image.encode('utf-8'), None, 0)
+                self._handle, tensor_ptr, image.encode('utf-8'), c_roi, 0)
             if err != 0:
                 raise RuntimeError('failed to load image: %s' % strerror(err))
             return
         elif hasattr(image, '__gtype__') and \
                 image.__gtype__.name == 'GstSample':
-            return self.load_gst_sample(image, tensor)
+            return self.load_gst_sample(image, tensor, c_roi)
         else:
             import numpy as np
             if isinstance(image, np.ndarray):
                 buf = image.ctypes.data_as(c_void_p)
                 fourcc = 0
-                width = 0
-                height = 0
-                raise RuntimeError(
-                    'loading image from numpy array not currently supported')
+                if len(image.shape) == 3:
+                    if image.shape[2] == 4:
+                        fourcc = int.from_bytes(bytes('RGBA', 'utf-8'), byteorder='little')
+                    elif image.shape[2] == 3:
+                        fourcc = int.from_bytes(bytes('RGB', 'utf-8'), byteorder='little')
+                elif len(image.shape) == 4:
+                    if image.shape[3] == 4:
+                        fourcc = int.from_bytes(bytes('RGBA', 'utf-8'), byteorder='little')
+                    elif image.shape[3] == 3:
+                        fourcc = int.from_bytes(bytes('RGB', 'utf-8'), byteorder='little')
+                width = image.shape[1]
+                height = image.shape[0]
                 err = lib.vaal_load_frame_memory(
-                    self._handle, None, buf, fourcc, width, height, None, 0)
+                    self._handle, None, buf, fourcc, width, height, c_roi, 0)
+                return err
         raise RuntimeError(
             'load_image called with unsupported type', type(image))
 
-    def load_frame(self, width, height, fourcc, dmabuf=None, tensor=None):
+    def load_frame(self, width, height, fourcc, dmabuf=None, tensor=None, roi=None):
         if tensor is not None:
             import deepview.rt as rt
             tensor_ptr = rt.ffi.cast('intptr_t', tensor.ptr)
             tensor_ptr = cast(int(tensor_ptr), c_void_p)
         else:
             tensor_ptr = None
 
         if dmabuf is None:
             raise RuntimeError('load_frame must be called with a valid dmabuf')
         err = lib.vaal_load_frame_dmabuf(
-            self._handle, tensor_ptr, dmabuf, fourcc, width, height, None, 0)
+            self._handle, tensor_ptr, dmabuf, fourcc, width, height, roi, 0)
         if err != 0:
             raise RuntimeError('failed to load frame: %s' % strerror(err))
 
-    def load_gst_sample(self, sample, tensor=None):
+    def load_gst_sample(self, sample, tensor=None, roi=None):
         import gi
         gi.require_version("GstAllocators", "1.0")
         from gi.repository import GstAllocators
 
         caps = sample.get_caps()
 
         buffer = sample.get_buffer()
@@ -281,8 +294,8 @@
         dmabuf = GstAllocators.dmabuf_memory_get_fd(memory)
 
         width = caps.get_structure(0).get_value("width")
         height = caps.get_structure(0).get_value("height")
         format = caps.get_structure(0).get_value("format")
         fourcc = int.from_bytes(bytes(format, 'utf-8'), byteorder='little')
 
-        self.load_frame(width, height, fourcc, dmabuf, tensor)
+        self.load_frame(width, height, fourcc, dmabuf, tensor, roi)
```

## Comparing `vaal-1.3.1.dist-info/LICENSE.txt` & `vaal-1.3.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vaal-1.3.1.dist-info/RECORD` & `vaal-1.3.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 deepview/vaal/__init__.py,sha256=B5eUs-IeZXpXYCPS_JYr3-Bp81_1ez02CE6WVS9O9O4,453
 deepview/vaal/camera.py,sha256=HPXZVEk2yy_1VYIRZJZ2LnQAaRs-09P7eakwhDjR6Co,1514
-deepview/vaal/context.py,sha256=QGLbFuU20tf4Dm7Eg3yVd6WMA5BGrdG9md5dWBf0asM,10634
+deepview/vaal/context.py,sha256=IMOxGNfsDKtEgTCx38rtTLQjDeYO1xNs8ysGGL3YE-o,11346
 deepview/vaal/library.py,sha256=B5M1RRbnU-Pfdc2Rd3JNaxrvlm_o797YsW8f95_TkkE,7879
-vaal-1.3.1.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
-vaal-1.3.1.dist-info/METADATA,sha256=TvsBj5WiMVb9JCLySIuXcTe9Z4HH9fjfbrq2Vvtba-w,229
-vaal-1.3.1.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
-vaal-1.3.1.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
-vaal-1.3.1.dist-info/RECORD,,
+vaal-1.3.2.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
+vaal-1.3.2.dist-info/METADATA,sha256=QHLdkVq3Z7Ye-UQwACnNsts4I9er-d0qtJf9xcI8WE8,229
+vaal-1.3.2.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
+vaal-1.3.2.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
+vaal-1.3.2.dist-info/RECORD,,
```


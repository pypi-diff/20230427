# Comparing `tmp/vaal-1.2.18-py3-none-any.whl.zip` & `tmp/vaal-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,11 @@
-Zip file size: 22577 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      453 b- defN 23-Mar-21 16:34 deepview/vaal/__init__.py
--rw-rw-r--  2.0 unx     1514 b- defN 23-Mar-21 16:34 deepview/vaal/camera.py
--rw-rw-r--  2.0 unx    10634 b- defN 23-Mar-21 16:34 deepview/vaal/context.py
--rw-rw-r--  2.0 unx     7879 b- defN 23-Mar-21 16:34 deepview/vaal/library.py
--rw-rw-r--  2.0 unx     5450 b- defN 23-Mar-21 16:34 deepview/vaal/validator/__main__.py
--rw-rw-r--  2.0 unx     5523 b- defN 23-Mar-21 16:34 deepview/vaal/validator/dataset.py
--rw-rw-r--  2.0 unx     6308 b- defN 23-Mar-21 16:34 deepview/vaal/validator/drawer.py
--rw-rw-r--  2.0 unx     7363 b- defN 23-Mar-21 16:34 deepview/vaal/validator/evaluator.py
--rw-rw-r--  2.0 unx     4029 b- defN 23-Mar-21 16:34 deepview/vaal/validator/runner.py
--rw-rw-r--  2.0 unx     6275 b- defN 23-Mar-21 16:34 deepview/vaal/validator/utils.py
--rw-rw-r--  2.0 unx    11710 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      230 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/WHEEL
--rw-rw-r--  2.0 unx       69 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1341 b- defN 23-Mar-21 16:38 vaal-1.2.18.dist-info/RECORD
-16 files, 68879 bytes uncompressed, 20359 bytes compressed:  70.4%
+Zip file size: 11278 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      453 b- defN 23-Apr-27 17:49 deepview/vaal/__init__.py
+-rw-rw-r--  2.0 unx     1514 b- defN 23-Apr-27 17:49 deepview/vaal/camera.py
+-rw-rw-r--  2.0 unx    10634 b- defN 23-Apr-27 17:49 deepview/vaal/context.py
+-rw-rw-r--  2.0 unx     7879 b- defN 23-Apr-27 17:49 deepview/vaal/library.py
+-rw-rw-r--  2.0 unx    11710 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      229 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 23-Apr-27 17:53 vaal-1.3.1.dist-info/RECORD
+9 files, 33218 bytes uncompressed, 10084 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -6,44 +6,23 @@
 
 Filename: deepview/vaal/context.py
 Comment: 
 
 Filename: deepview/vaal/library.py
 Comment: 
 
-Filename: deepview/vaal/validator/__main__.py
+Filename: vaal-1.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: deepview/vaal/validator/dataset.py
+Filename: vaal-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: deepview/vaal/validator/drawer.py
+Filename: vaal-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: deepview/vaal/validator/evaluator.py
+Filename: vaal-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: deepview/vaal/validator/runner.py
-Comment: 
-
-Filename: deepview/vaal/validator/utils.py
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/LICENSE.txt
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/METADATA
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/WHEEL
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/entry_points.txt
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/top_level.txt
-Comment: 
-
-Filename: vaal-1.2.18.dist-info/RECORD
+Filename: vaal-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vaal-1.2.18.dist-info/LICENSE.txt` & `vaal-1.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vaal-1.2.18.dist-info/RECORD` & `vaal-1.3.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 deepview/vaal/__init__.py,sha256=B5eUs-IeZXpXYCPS_JYr3-Bp81_1ez02CE6WVS9O9O4,453
 deepview/vaal/camera.py,sha256=HPXZVEk2yy_1VYIRZJZ2LnQAaRs-09P7eakwhDjR6Co,1514
 deepview/vaal/context.py,sha256=QGLbFuU20tf4Dm7Eg3yVd6WMA5BGrdG9md5dWBf0asM,10634
 deepview/vaal/library.py,sha256=B5M1RRbnU-Pfdc2Rd3JNaxrvlm_o797YsW8f95_TkkE,7879
-deepview/vaal/validator/__main__.py,sha256=Z_pAppNMdEkm33oOFTlzvQZguJiukGgoeFZUkQPoqw8,5450
-deepview/vaal/validator/dataset.py,sha256=xu4gUwPVwW7skPTK_zN1eCR4ee66PWOWoOhVf71DRus,5523
-deepview/vaal/validator/drawer.py,sha256=FhWU50XOP0ZBilZJH9Jq6we3dVQb2D4x_5FRj3jrFKI,6308
-deepview/vaal/validator/evaluator.py,sha256=00wUWQmZo0TGvhWSThDGwuuungH5DoxFOhL1IVsMTOU,7363
-deepview/vaal/validator/runner.py,sha256=tFqnf-RsSsc6KvK_UQIdC6wjv4KZsq6LaE9lR8kSWL4,4029
-deepview/vaal/validator/utils.py,sha256=L9SrVUQqwb6s9Sv5DV4a_HSUn8G0e9tSyxNCwcBXQ0M,6275
-vaal-1.2.18.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
-vaal-1.2.18.dist-info/METADATA,sha256=5txT-Hup2D1wpjm3PDmQ6Vma3HyQklHRLuw6UjHnXSc,230
-vaal-1.2.18.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
-vaal-1.2.18.dist-info/entry_points.txt,sha256=wNKpdsntSSVzIsBThKevsNNeXSKMfprHVFKhPOSOlTg,69
-vaal-1.2.18.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
-vaal-1.2.18.dist-info/RECORD,,
+vaal-1.3.1.dist-info/LICENSE.txt,sha256=tRF0H4BBjc7hxfxRe2Y573C-tye_wJQBFdZu_wG_rLQ,11710
+vaal-1.3.1.dist-info/METADATA,sha256=TvsBj5WiMVb9JCLySIuXcTe9Z4HH9fjfbrq2Vvtba-w,229
+vaal-1.3.1.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
+vaal-1.3.1.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
+vaal-1.3.1.dist-info/RECORD,,
```


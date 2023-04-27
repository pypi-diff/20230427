# Comparing `tmp/miniball-1.1.0.tar.gz` & `tmp/miniball-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniball-1.1.0.tar", last modified: Wed Apr 28 14:46:15 2021, max compression
+gzip compressed data, was "miniball-1.2.0.tar", last modified: Thu Apr 27 09:13:28 2023, max compression
```

## Comparing `miniball-1.1.0.tar` & `miniball-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-04-28 14:46:15.682672 miniball-1.1.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1078 2021-04-28 12:28:46.000000 miniball-1.1.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)       41 2021-04-28 12:10:24.000000 miniball-1.1.0/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     5269 2021-04-28 14:46:15.682672 miniball-1.1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     3552 2021-04-28 14:32:21.000000 miniball-1.1.0/README.rst
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-04-28 14:46:15.679339 miniball-1.1.0/miniball.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     5269 2021-04-28 14:46:15.000000 miniball-1.1.0/miniball.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      237 2021-04-28 14:46:15.000000 miniball-1.1.0/miniball.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2021-04-28 14:46:15.000000 miniball-1.1.0/miniball.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       12 2021-04-28 14:46:15.000000 miniball-1.1.0/miniball.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        9 2021-04-28 14:46:15.000000 miniball-1.1.0/miniball.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)     4135 2021-04-28 13:42:54.000000 miniball-1.1.0/miniball.py
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2021-04-28 14:46:15.682672 miniball-1.1.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     2505 2021-04-28 14:12:41.000000 miniball-1.1.0/setup.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3559 2021-04-28 13:40:58.000000 miniball-1.1.0/test_miniball.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-27 09:13:28.228454 miniball-1.2.0/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1078 2023-04-27 09:12:56.000000 miniball-1.2.0/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)       41 2023-04-27 09:12:56.000000 miniball-1.2.0/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     4671 2023-04-27 09:13:28.228454 miniball-1.2.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     3899 2023-04-27 09:12:56.000000 miniball-1.2.0/README.rst
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-27 09:13:28.228454 miniball-1.2.0/miniball.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4671 2023-04-27 09:13:28.000000 miniball-1.2.0/miniball.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      237 2023-04-27 09:13:28.000000 miniball-1.2.0/miniball.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-04-27 09:13:28.000000 miniball-1.2.0/miniball.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       12 2023-04-27 09:13:28.000000 miniball-1.2.0/miniball.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-04-27 09:13:28.000000 miniball-1.2.0/miniball.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)     4216 2023-04-27 09:12:56.000000 miniball-1.2.0/miniball.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-04-27 09:13:28.228454 miniball-1.2.0/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)     2505 2023-04-27 09:12:56.000000 miniball-1.2.0/setup.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3561 2023-04-27 09:12:56.000000 miniball-1.2.0/test_miniball.py
```

### Comparing `miniball-1.1.0/LICENSE` & `miniball-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2021 Devert Alexandre
+Copyright (c) 2019-2023 Devert Alexandre
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `miniball-1.1.0/README.rst` & `miniball-1.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 `Bernd Gaertner's C++ library <https://people.inf.ethz.ch/gaertner/subdir/software/miniball.html>`__.
 
 This project is licensed under the MIT License
 
 Requirements
 ============
 
-miniball 1.1 requires
+miniball 1.2 requires
 
 * Python >= 3.5
 * Numpy >= 1.17
 
 Installation
 ============
 
@@ -73,15 +73,15 @@
 	>>> C, r2 = miniball.get_bounding_ball(S, epsilon=1e-7)
 
 
 Repeatability
 -------------
 
 The algorithm to compute bounding balls relies on a pseudo-random number generator.
-Although the algorithms return an exact solution, it is only exact up to the epsilon
+Although the algorithms return an exact solution, it is only exact up to the ``epsilon``
 parameter. As a consequence, running the ``get_bounding_ball`` function twice on 
 the same input might not return exactly the same output.
 
 By default, each call to ``get_bounding_ball`` pull out a new, freshly seeded 
 pseudo-random number generator. Therefore, if you wish to get repeatable results 
 from ``get_bounding_ball``, you have to (and only have to) pass the same pseudo-random 
 number generator, using with the ``rng`` keyword argument
@@ -91,25 +91,35 @@
 	>>> import numpy
 	>>> import miniball	
 	>>> S = numpy.random.randn(100, 2)	
 	>>> rng = numpy.random.RandomState(42)
 	>>> C, r2 = miniball.get_bounding_ball(S, rng = rng)
 
 
+Duplicated input points
+-----------------------
+
+Duplicated input points might trigger failures. This implementation do not check 
+for duplicated input points, the guaranty of non-duplication is defered to you, the
+programmer. This is by design, to avoid to pay the cost of de-duplication when we
+are sure that the input has no duplicates.
+
+
 Implementation notes
 ====================
 
 The algorithm implemented is Welzl's algorithm. It is a pure Python implementation,
 it is not a binding of the popular C++ package `Bernd Gaertner's miniball <https://people.inf.ethz.ch/gaertner/subdir/software/miniball.html>`__.
 
 The algorithm, although often presented in its recursive form, is here implemented
 in an iterative fashion. Python have an hard-coded recursion limit, therefore
 a recursive implementation of Welzl's algorithm would have an artificially limited
 number of point it could process.
 
+
 Authors
 =======
 
 * **Alexandre Devert** - *Initial work* - `marmakoide <https://github.com/marmakoide>`__
 
 License
 =======
```

### Comparing `miniball-1.1.0/miniball.py` & `miniball-1.2.0/miniball.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2019-2021 Alexandre Devert
+# Copyright (c) 2019-2023 Alexandre Devert
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,15 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy
 
 
 __author__ = "Alexandre Devert <marmakoide@hotmail.fr>"
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 
 def get_circumsphere(S):
     """
     Computes the circumsphere of a set of points
 
     Parameters
@@ -38,19 +38,19 @@
     Returns
     -------
     C, r2 : ((2) ndarray, float)
             The center and the squared radius of the circumsphere
     """
 
     U = S[1:] - S[0]
-    B = numpy.sqrt(numpy.sum(U ** 2, axis=1))
+    B = numpy.sqrt(numpy.square(U).sum(axis=1))
     U /= B[:, None]
     B /= 2
     C = numpy.dot(numpy.linalg.solve(numpy.inner(U, U), B), U)
-    r2 = numpy.sum(C ** 2)
+    r2 = numpy.square(C).sum()
     C += S[0]
     return C, r2
 
 
 def get_bounding_ball(S, epsilon=1e-7, rng=numpy.random.default_rng()):
     """
     Computes the smallest bounding ball of a set of points
@@ -75,25 +75,25 @@
     """
 
     # Iterative implementation of Welzl's algorithm, see
     # "Smallest enclosing disks (balls and ellipsoids)" Emo Welzl 1991
 
     def circle_contains(D, p):
         c, r2 = D
-        return numpy.sum((p - c) ** 2) <= r2
+        return numpy.square(p - c).sum() <= r2
 
     def get_boundary(R):
         if len(R) == 0:
             return numpy.zeros(S.shape[1]), 0.0
 
         if len(R) <= S.shape[1] + 1:
             return get_circumsphere(S[R])
 
         c, r2 = get_circumsphere(S[R[: S.shape[1] + 1]])
-        if numpy.all(numpy.fabs(numpy.sum((S[R] - c) ** 2, axis=1) - r2) < epsilon):
+        if numpy.all(numpy.fabs(numpy.square(S[R] - c).sum(axis=1) - r2) < epsilon):
             return c, r2
 
     class Node(object):
         def __init__(self, P, R):
             self.P = P
             self.R = R
             self.D = None
@@ -105,24 +105,25 @@
         stack = [node]
         while len(stack) > 0:
             node = stack.pop()
 
             if len(node.P) == 0 or len(node.R) >= S.shape[1] + 1:
                 node.D = get_boundary(node.R)
             elif node.left is None:
-                node.pivot = rng.choice(node.P)
-                node.left = Node(list(set(node.P) - set([node.pivot])), node.R)
+                pivot_index = rng.integers(len(node.P))
+                node.pivot = node.P[pivot_index]
+                node.left = Node(node.P[:pivot_index] + node.P[pivot_index + 1:], node.R)
                 stack.extend((node, node.left))
             elif node.right is None:
                 if circle_contains(node.left.D, S[node.pivot]):
                     node.D = node.left.D
                 else:
                     node.right = Node(node.left.P, node.R + [node.pivot])
                     stack.extend((node, node.right))
             else:
                 node.D = node.right.D
                 node.left, node.right = None, None
 
     S = S.astype(float, copy=False)
-    root = Node(range(S.shape[0]), [])
+    root = Node(list(range(S.shape[0])), [])
     traverse(root)
     return root.D
```

### Comparing `miniball-1.1.0/setup.py` & `miniball-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2019-2021 Alexandre Devert
+# Copyright (c) 2019-2023 Alexandre Devert
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the 'Software'), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `miniball-1.1.0/test_miniball.py` & `miniball-1.2.0/test_miniball.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2019-2021 Alexandre Devert
+# Copyright (c) 2019-2023 Alexandre Devert
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -60,28 +60,28 @@
             # Generate points
             S = numpy.random.randn(count, n)
 
             # Get the bounding sphere
             C, r2 = miniball.get_bounding_ball(S)
 
             # Check that all points are inside the bounding sphere up to machine precision
-            assert numpy.all(numpy.sum((S - C) ** 2, axis=1) - r2 < 1e-12)
+            assert numpy.all(numpy.square(S - C).sum(axis=1) - r2 < 1e-12)
 
 
 def test_bounding_ball_optimality():
     # Check that the bounding ball are optimal
     for n in range(2, 10):
         for count in range(n + 2, n + 30):
             # Generate a support sphere from n+1 points
             S_support = numpy.random.randn(n + 1, n)
             C_support, r2_support = miniball.get_bounding_ball(S_support)
 
             # Generate points inside the support sphere
             S = numpy.random.randn(count - S_support.shape[0], n)
-            S /= numpy.sqrt(numpy.sum(S ** 2, axis=1))[:, None]
+            S /= numpy.sqrt(numpy.square(S).sum(axis=1))[:, None]
             S *= (0.9 * numpy.sqrt(r2_support)) * numpy.random.rand(
                 count - S_support.shape[0], 1
             )
             S = S + C_support
 
             # Get the bounding sphere
             C, r2 = miniball.get_bounding_ball(
```


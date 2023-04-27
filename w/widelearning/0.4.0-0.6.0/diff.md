# Comparing `tmp/widelearning-0.4.0.tar.gz` & `tmp/widelearning-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.4.0.tar", max compression
+gzip compressed data, was "widelearning-0.6.0.tar", max compression
```

## Comparing `widelearning-0.4.0.tar` & `widelearning-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      317 2022-12-23 17:02:48.918136 widelearning-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    70944 2022-12-23 16:49:52.063413 widelearning-0.4.0/widelearning.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 widelearning-0.4.0/setup.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 widelearning-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-04-27 04:21:13.787954 widelearning-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    74117 2023-04-27 04:13:48.010957 widelearning-0.6.0/widelearning.py
+-rw-r--r--   0        0        0      505 2023-04-27 04:21:23.242814 widelearning-0.6.0/setup.py
+-rw-r--r--   0        0        0      514 2023-04-27 04:21:23.243043 widelearning-0.6.0/PKG-INFO
```

### Comparing `widelearning-0.4.0/widelearning.py` & `widelearning-0.6.0/widelearning.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
 import numpy as np
-import pandas as pd
-import os
-import shutil
-import glob
-import math as m
 
 def txt_kernel(file_path):	
     f = open(file_path, 'r')
 	
     weights = []
 
     for i in f:
@@ -21,75 +16,14 @@
         for i1, elem in enumerate(ii):
             ii[i1] = [[int(elem)]]
             
     with open('kernel.txt', 'w') as file:
         file.write(str(weights))
 
     return weights 
-    
-def vert(n):
-    for i in range(len(n)):
-        print(*[x for x in n],'',sep=',')
-
-def hor(n):
-    hr = []
-    for i in n:
-        hr.append(len(n)*[i])
-	
-    for k1 in range(len(hr)):
-        print()
-        for k2 in range(len(hr[k1])):
-            print(hr[k1][k2], end=',')
-            
-def diag(d):
-    n = [0, -2, -1, 1, 2]
-
-    if(d % 2 == 0):
-        m1 = d//2
-        m2 = (d/2) - 1
-    else:
-        m1 = d // 2
-        m2 = d // 2
-
-    L = {}
-
-    c = 1
-    for i1 in range(int(m2)):
-        L[c] = [n[3]]*(d-c) 
-        c += 1
-    for i2 in range(int(m1)):
-        L[c] = [n[4]]*(d-c)
-        c += 1
-    
-    c = -1
-    for j1 in range(int(m2)):
-        L[c] = [n[2]]*(d+c) 
-        c -= 1
-    for j2 in range(int(m1)):
-        L[c] = [n[1]]*(d+c)
-        c -= 1
-
-    diag1 = 0
-    for u in L:
-        diag1 = diag1 + np.diag(L[u],u)
-        z1 = np.diag(np.full(d,n[0]))+diag1
-        
-    z2 = np.fliplr(z1)
-
-    for h in range(len(z1)):
-        print()
-        for g in range(len(z1[h])):
-            print(z1[h][g], end=',')
-            
-    print()
-    
-    for hh in range(len(z2)):
-        print()
-        for gg in range(len(z2[hh])):
-            print(z2[hh][gg], end=',')
 
 def add_kernel(path, init_kernel):
     ff = open(path, 'r')
     
     w1 = init_kernel
 
     weights = []
@@ -109,14 +43,197 @@
             w1[i][j][0].append(weights[i][j])
 
     with open('kernel.txt', 'w') as file:
         file.write(str(w1))
         
     return w1
     
+# horizontal(32, [-7,-5,-3,-1,1,3,5,7])
+def horizontal(dim, values):
+    horizontal = []
+    for i in range(dim):
+        row = []
+        for j in range(dim):
+            row.append(values[i % len(values)])
+        horizontal.append(row)
+        
+    with open('horizontal.txt', 'w') as f:
+        for row in horizontal:
+            f.write(','.join(str(x) for x in row) + ',\n')
+    return horizontal
+
+# vertical(32, [-7,-5,-3,-1,1,3,5,7])	
+def vertical(dim, values):
+    vertical = []
+    for i in range(dim):
+        row = []
+        for j in range(dim):
+            row.append(values[j % len(values)])
+        vertical.append(row)
+        
+    with open('vertical.txt', 'w') as f:    
+        for row in vertical:
+            f.write(','.join(str(x) for x in row) + ',\n')
+    return vertical
+
+# diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)	
+def diagonal(up, down, d, dimension):
+
+    matrix = [[0 for i in range(dimension)] for j in range(dimension)] 
+    for i in range(dimension):
+        for j in range(dimension):
+            if i == j: 
+                matrix[i][j] = d
+            elif i < j: 
+                matrix[i][j] = up[(j-i-1) % len(up)]
+            else: 
+                matrix[i][j] = down[(i-j-1) % len(down)]
+    
+    with open('diagonal1.txt', 'w') as file:
+        for i in matrix:
+            for j in i:
+                file.write(str(j) + ',')
+            file.write('\n')
+            
+    matrix2 = np.fliplr(matrix)
+    
+    with open('diagonal2.txt', 'w') as file:
+        for i in matrix2:
+            for j in i:
+                file.write(str(j) + ',')
+            file.write('\n')
+    
+    return matrix
+    
+def show_kernel(N, name):
+
+    ff = name.layers[N].get_weights()
+
+    for nn in range(len(ff[0][0][0][0])):
+      print('\n' + f'Номер сверточного ядра: {nn}')
+      for kk in range(len(ff[0][0][0])):
+        print(f'-----------ЦВЕТОВОЙ КАНАЛ №{kk}-----------')
+        for i in range(len(ff[0])):
+          for j in range(len(ff[0][i])):
+            print(ff[0][i][j][kk][nn], end=',')
+          print()
+        print('\n')
+        
+def txt_kernel_rgb(k1, k2, k3): 
+
+    f1 = open(k1, 'r')
+    f2 = open(k2, 'r')
+    f3 = open(k3, 'r')
+	
+    w1 = []
+
+    for i in f1:
+        w1.append(i.strip().split(','))
+    for j in w1:
+        j.pop()
+
+    for ii in w1:
+        for i1, elem in enumerate(ii):
+            ii[i1] = [[int(elem)]]
+
+    w2 = []
+
+    for i in f2:
+        w2.append(i.strip().split(','))
+
+    for j in w2:
+        j.pop()
+
+    for ii in w2:
+        for i1, elem in enumerate(ii):
+            ii[i1] = [int(elem)]
+
+    for i in range(len(w1[0])):
+        for j in range(len(w1[0])):
+            w1[i][j].append(w2[i][j])
+
+    w3 = []
+
+    for i in f3:
+        w3.append(i.strip().split(','))
+
+    for j in w3:
+        j.pop()
+
+    for ii in w3:
+        for i1, elem in enumerate(ii):
+            ii[i1] = [int(elem)]
+
+    for i in range(len(w1[0])):
+        for j in range(len(w1[0])):
+            w1[i][j].append(w3[i][j])
+			
+    return w1
+
+#weights1 = txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')
+
+def add_kernel_rgb(k1, k2, k3, w):
+
+    f1 = open(k1, 'r')
+    f2 = open(k2, 'r')
+    f3 = open(k3, 'r')
+	
+    w11 = []
+
+    for i in f1:
+        w11.append(i.strip().split(','))
+
+    for j in w11:
+        j.pop()
+
+    for ii in w11:
+        for i1, elem in enumerate(ii):
+            ii[i1] = int(elem)
+
+    w22 = []
+
+    for i in f2:
+        w22.append(i.strip().split(','))
+
+    for j in w22:
+        j.pop()
+
+    for ii in w22:
+        for i1, elem in enumerate(ii):
+            ii[i1] = int(elem)
+
+    w33 = []
+
+    for i in f3:
+        w33.append(i.strip().split(','))
+
+    for j in w33:
+        j.pop()
+
+    for ii in w33:
+        for i1, elem in enumerate(ii):
+            ii[i1] = int(elem)
+
+    for i in range(len(w1)):
+        for j in range(len(w1)):
+            w[i][j][0].append(w11[i][j])
+	########################################
+    for i in range(len(w1)):
+        for j in range(len(w1)):
+            w[i][j][1].append(w22[i][j])
+	########################################
+    for i in range(len(w1)):
+        for j in range(len(w1)):
+            w[i][j][2].append(w33[i][j])
+	########################################
+	
+    return w
+
+#weights2 = add_kernel_rgb('k3.txt', 'k2.txt', 'k1.txt', weights1)
+        
 def select_top(path, label):
     # label - название столбца с метками классов ('Wine')
     # z - индекс в переборе меток классов
     all_classes = pd.read_csv(path)#('wine_train.csv')
     all_classes.drop(all_classes.columns[0], axis=1, inplace=True)
 
     uniq = pd.unique(all_classes[[label]].values.ravel('K'))
@@ -1995,8 +2112,7 @@
     #print(lstm)
     
     data_train = data.drop(labels = lstm,axis = 0)
     data_train.to_csv(f'{name}_train.csv')
     
     return data
 
-
```

### Comparing `widelearning-0.4.0/PKG-INFO` & `widelearning-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: widelearning
-Version: 0.4.0
+Version: 0.6.0
 Summary: Library for searching the optimal neural network architecture
 Author: Brinkinvision
 Author-email: brinkinvision@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
```


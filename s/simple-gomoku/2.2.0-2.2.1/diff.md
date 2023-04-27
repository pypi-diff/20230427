# Comparing `tmp/simple_gomoku-2.2.0-py3-none-any.whl.zip` & `tmp/simple_gomoku-2.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3880 bytes, number of entries: 8
--rw-r--r--  2.0 unx      161 b- defN 23-Apr-11 15:31 simple_gomoku/__init__.py
--rw-r--r--  2.0 unx     3973 b- defN 23-Apr-11 15:31 simple_gomoku/env/Gomoku.py
--rw-r--r--  2.0 unx     1711 b- defN 23-Apr-11 15:31 simple_gomoku/env/TicTacToe.py
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-11 15:31 simple_gomoku/env/__init__.py
--rw-r--r--  2.0 unx      435 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      657 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/RECORD
-8 files, 7130 bytes uncompressed, 2724 bytes compressed:  61.8%
+Zip file size: 3888 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      161 b- defN 23-Apr-27 06:03 simple_gomoku/__init__.py
+-rw-r--r--  2.0 unx     4007 b- defN 23-Apr-27 06:03 simple_gomoku/env/Gomoku.py
+-rw-r--r--  2.0 unx     1711 b- defN 23-Apr-27 06:03 simple_gomoku/env/TicTacToe.py
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-27 06:03 simple_gomoku/env/__init__.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-27 06:03 simple_gomoku-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 06:03 simple_gomoku-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-27 06:03 simple_gomoku-2.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      657 b- defN 23-Apr-27 06:03 simple_gomoku-2.2.1.dist-info/RECORD
+8 files, 7164 bytes uncompressed, 2732 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: simple_gomoku/env/TicTacToe.py
 Comment: 
 
 Filename: simple_gomoku/env/__init__.py
 Comment: 
 
-Filename: simple_gomoku-2.2.0.dist-info/METADATA
+Filename: simple_gomoku-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: simple_gomoku-2.2.0.dist-info/WHEEL
+Filename: simple_gomoku-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: simple_gomoku-2.2.0.dist-info/top_level.txt
+Filename: simple_gomoku-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_gomoku-2.2.0.dist-info/RECORD
+Filename: simple_gomoku-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_gomoku/env/Gomoku.py

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import numpy as np
-
+# @title gomoku 
 class Gomoku():
 
-    def __init__(self, row=5, width=6):
+    def __init__(self, row=5, width=5):
         self.state = None
         self.row = row
         self.width = width
         self.action_size = self.width * self.width
         self.board_edges = self._get_board_edges()
         """ search_directions: [-w-1, -w, -w+1, -1, 1, w-1, w, w+1] """     
         self.search_directions = self._get_search_directions() # ((0,1),(1,0),(1,1),(-1,1))
@@ -26,16 +26,17 @@
 
         x1, x2 = (a // self.width), (a % self.width)
 
         self.state[x1][x2] = self.player
         self.player = -self.player
 
         if self._is_done(a):
+            # 打ち終わって終了なら勝ち
             self.done = True
-            self.reward = -1 # 打つ手がないので負け
+            self.reward = 1 
 
         elif self._is_draw():
             self.done = True
             self.reward = 0
 
         else:
             pass
@@ -45,34 +46,14 @@
     def get_legal_actions(self):
         state = np.array(self.state).reshape(-1)
         return np.where(state==0)[0]
 
     def show(self, state):
         print(state)
 
-    def render(self):
-        state = self.state
-        print("  ", end="")
-
-        for i in range(len(state)):
-            print(i, end=" ")
-        print()
-
-        for i, row in enumerate(state):
-            print(i, end=" ")
-            for piece in row:
-                if piece == -1:
-                    print("X", end=" ")
-                elif piece == 1:
-                    print("O", end=" ")
-                else:
-                    print("-", end=" ")
-            print()
-        print()
-
     def _pass(self):
         self.player = -self.player
         pass
 
     def _is_done(self, a):
         """ a: action """
        
@@ -148,7 +129,27 @@
                 edges.append(opposite_h)
 
         return edges
 
     def _get_search_directions(self):
         w = self.width
         return [1, w-1, w, w+1]
+
+    def render(self):
+        state = self.state
+        print("  ", end="")
+
+        for i in range(len(state)):
+            print(i, end=" ")
+        print()
+
+        for i, row in enumerate(state):
+            print(i, end=" ")
+            for piece in row:
+                if piece == -1:
+                    print("X", end=" ")
+                elif piece == 1:
+                    print("O", end=" ")
+                else:
+                    print("-", end=" ")
+            print()
+        print()
```

## Comparing `simple_gomoku-2.2.0.dist-info/RECORD` & `simple_gomoku-2.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 simple_gomoku/__init__.py,sha256=ARIH18Pe-DC085xKnxNY4T9jH6Mjn-3q-z_cOCQ8zds,161
-simple_gomoku/env/Gomoku.py,sha256=WG-Qhuul0SjIa45sbYx14QgQbnwJOGwpmn5a6I8I8I0,3973
+simple_gomoku/env/Gomoku.py,sha256=45wvs5lP43TvZRKz75WUxnLyDHaiNn1cuzecezH_8oI,4007
 simple_gomoku/env/TicTacToe.py,sha256=pi1He4on_ZkxOvdiVf33PkYx1mSGTJeRtqKZquhKFbA,1711
 simple_gomoku/env/__init__.py,sha256=h0I4nPUtBBW9qn3TXxt913TJG9YixC83Sx7evCK8Xbc,87
-simple_gomoku-2.2.0.dist-info/METADATA,sha256=GQ6YUfBXB3A3ZsBDZ1sG5j4q9iXnLvfllFdwQu6pF4E,435
-simple_gomoku-2.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simple_gomoku-2.2.0.dist-info/top_level.txt,sha256=P3MSbNvbZ_Tvlt8wunMwWVIE2bGtwRqdy78qhtLEQvI,14
-simple_gomoku-2.2.0.dist-info/RECORD,,
+simple_gomoku-2.2.1.dist-info/METADATA,sha256=4zX8iwNNfxqUEqAHPMWqp90eMdKUZgASKn8KWfn_bzQ,435
+simple_gomoku-2.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simple_gomoku-2.2.1.dist-info/top_level.txt,sha256=P3MSbNvbZ_Tvlt8wunMwWVIE2bGtwRqdy78qhtLEQvI,14
+simple_gomoku-2.2.1.dist-info/RECORD,,
```


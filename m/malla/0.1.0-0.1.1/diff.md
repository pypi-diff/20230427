# Comparing `tmp/malla-0.1.0.tar.gz` & `tmp/malla-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.0.tar", max compression
+gzip compressed data, was "malla-0.1.1.tar", max compression
```

## Comparing `malla-0.1.0.tar` & `malla-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.0/malla/__init__.py
--rw-r--r--   0        0        0     6002 2023-04-25 21:38:09.823435 malla-0.1.0/malla/directed_edge.py
--rw-r--r--   0        0        0      834 2023-04-25 21:43:28.263441 malla-0.1.0/malla/off.py
--rw-r--r--   0        0        0      266 2023-04-25 21:05:46.133399 malla-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 malla-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.1/malla/__init__.py
+-rw-r--r--   0        0        0     6382 2023-04-27 15:52:38.670048 malla-0.1.1/malla/directed_edge.py
+-rw-r--r--   0        0        0      618 2023-04-27 15:46:05.623373 malla-0.1.1/malla/off.py
+-rw-r--r--   0        0        0      266 2023-04-27 17:09:35.293468 malla-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 malla-0.1.1/PKG-INFO
```

### Comparing `malla-0.1.0/malla/directed_edge.py` & `malla-0.1.1/malla/directed_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,25 @@
         hf = 3*f
         for i in range(3):
             h = hf+i
             mate = self.half_edge(h).mate
             if mate > -1:
                 yield self.face(mate)
 
+    def face_strings(self) -> Generator[str, None, None]:
+        for f in range(self.number_of_faces()):
+            i = m.half_edge(3*f).dst
+            j = m.half_edge(3*f+1).dst
+            k = m.half_edge(3*f+2).dst
+            yield f'3 {i} {j} {k}'
+
+    def vertex_strings(self) -> Generator[str, None, None]:
+        for v in self.vertices:
+            yield str(v.data)
+
     def __add_face(self, f: any) -> None:
         self.__put_half_edge(f[0], f[1])
         self.__put_half_edge(f[1], f[2])
         self.__put_half_edge(f[2], f[0])
 
     def __put_half_edge(self, vi: int, vj: int) -> None:
         pair = (vi, vj)
```

### Comparing `malla-0.1.0/malla/off.py` & `malla-0.1.1/malla/off.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-#!/usr/bin/python3 
+#!/usr/bin/python3
 
 def read(filename):
     with open(filename, 'r') as file:
         lines = [l for l in file.readlines() if not l.isspace() ]
         nv = int(lines[1].split()[0])
         v = [tuple(float(x) for x in l.split())   for l in lines[2:nv+2] ]
         f = [tuple(int(x) for x in l.split()[1:]) for l in lines[nv+2:]  ]
     return v, f
 
 
-def write(filename, m):
+def write(filename, v, f):
     with open(filename, 'w') as file:
         file.write('OFF\n')
-        file.write(f'{m.number_of_vertices()} ' +
-                   f'{m.number_of_faces()} 0\n')
-        for v in m.vertices:
-            file.write(f'{v.data.x} {v.data.y} {v.data.z}\n')
-        for f in range(m.number_of_faces()):
-            i = m.half_edge(3*f).dst
-            j = m.half_edge(3*f+1).dst
-            k = m.half_edge(3*f+2).dst
-            file.write(f'3 {i} {j} {k}\n')
+        file.write(f'{len(v)} {len(f)} 0\n')
+        for vstring in v:
+            file.write(f'{vstring}\n')
+        for fstring in f:
+            file.write(f'{fstring}\n')
```


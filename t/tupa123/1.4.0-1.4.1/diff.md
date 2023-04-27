# Comparing `tmp/tupa123-1.4.0.tar.gz` & `tmp/tupa123-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.0.tar", last modified: Wed Apr 26 19:22:20 2023, max compression
+gzip compressed data, was "tupa123-1.4.1.tar", last modified: Thu Apr 27 11:23:22 2023, max compression
```

## Comparing `tupa123-1.4.0.tar` & `tupa123-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 19:22:20.012606 tupa123-1.4.0/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-04-26 19:22:20.012606 tupa123-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 19:22:20.012606 tupa123-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-26 19:21:23.000000 tupa123-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:22:19.996984 tupa123-1.4.0/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.0/tupa123/__init__.py
--rw-rw-rw-   0        0        0    67785 2023-04-26 19:06:25.000000 tupa123-1.4.0/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:22:20.012606 tupa123-1.4.0/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.565594 tupa123-1.4.1/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-04-27 11:23:22.565594 tupa123-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 11:23:22.565594 tupa123-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-27 11:19:28.000000 tupa123-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.555559 tupa123-1.4.1/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.1/tupa123/__init__.py
+-rw-rw-rw-   0        0        0       52 2023-04-27 11:22:32.000000 tupa123-1.4.1/tupa123/teste.py
+-rw-rw-rw-   0        0        0    67989 2023-04-27 11:14:58.000000 tupa123-1.4.1/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.565594 tupa123-1.4.1/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.0/LICENSE.txt` & `tupa123-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.0/PKG-INFO` & `tupa123-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.0
+Version: 1.4.1
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.0/README.md` & `tupa123-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.0/setup.py` & `tupa123-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.0',
+    version='1.4.1',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.0/tupa123/tupa123.py` & `tupa123-1.4.1/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
 
 
 
 
 
 
 #Plota o erro em relação ao alvo,que é o centro do grafico
-def PlotDispe3(Calculated, Targeted):
+def PlotDispe3(Calculated, Targeted, minx=0, maxx=0, miny=0, maxy=0):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
         eixoY1 = Targeted[:,j]
         eixoY2 = Calculated[:,j]
@@ -419,14 +419,18 @@
         sigma = np.std(eixoY2 - eixoY1)
         eixoY4 = (erro_medio/sigma) + eixoY3/sigma
                                 
         plt.title('Accuracy Trend Graph, variable '+ str(j+1))
         plt.scatter(eixoY4,razao,color='red', s=15 , marker = '.', alpha=0.1) #grafico de correlação entre as variaveis procuradas e alvo---
         plt.xlabel('Standard deviation sigma')
         plt.ylabel('Proportion error = calculated/target')
+        
+        if (maxx!=0) or (minx!=0):# Definindo os limites dos eixos x e y se o usuario entrar
+            plt.xlim(minx, maxx)
+            plt.ylim(miny, maxy)
 
         plt.plot([-1,1], [1,1], color='black', alpha=0.9, linestyle='dashed')
         plt.plot([0,0], [1-(np.max(razao)-1)*0.5,1+(np.max(razao)-1)*0.5], color='black', alpha=0.9, linestyle='dashed')
         
         plt.show()
```

### Comparing `tupa123-1.4.0/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.1/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.0
+Version: 1.4.1
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```


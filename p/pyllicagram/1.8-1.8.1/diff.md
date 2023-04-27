# Comparing `tmp/pyllicagram-1.8.tar.gz` & `tmp/pyllicagram-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyllicagram-1.8.tar", last modified: Sun Apr  9 17:53:57 2023, max compression
+gzip compressed data, was "dist/pyllicagram-1.8.1.tar", last modified: Thu Apr 27 10:54:44 2023, max compression
```

## Comparing `pyllicagram-1.8.tar` & `pyllicagram-1.8.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.188885 pyllicagram-1.8/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 17:53:57.187823 pyllicagram-1.8/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 17:19:41.000000 pyllicagram-1.8/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 17:53:57.189208 pyllicagram-1.8/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      404 2023-04-09 17:53:30.000000 pyllicagram-1.8/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.179420 pyllicagram-1.8/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.182776 pyllicagram-1.8/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     3703 2023-04-09 17:53:18.000000 pyllicagram-1.8/src/pyllicagram/__init__.py
--rw-r--r--   0 benoit2c   (501) staff       (20)      612 2023-04-09 17:37:23.000000 pyllicagram-1.8/src/pyllicagram/joker.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.186841 pyllicagram-1.8/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.047212 pyllicagram-1.8.1/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-27 10:54:44.044973 pyllicagram-1.8.1/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     5361 2023-04-19 08:35:16.000000 pyllicagram-1.8.1/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-27 10:54:44.048403 pyllicagram-1.8.1/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      413 2023-04-27 10:54:29.000000 pyllicagram-1.8.1/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.022748 pyllicagram-1.8.1/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.028258 pyllicagram-1.8.1/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     3853 2023-04-27 10:53:28.000000 pyllicagram-1.8.1/src/pyllicagram/__init__.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.043840 pyllicagram-1.8.1/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.8/src/pyllicagram/__init__.py` & `pyllicagram-1.8.1/src/pyllicagram/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*-coding:Utf-8 -*
 #
 # pyllicagram.py:
 #    Un micro package python pour importer des données de [Gallicagram]
 #
 import urllib
 import sys
+from tqdm import tqdm
 import os
 import collections
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 # import pandas
 try:
         import pandas as pd
@@ -26,26 +27,29 @@
 # API CALL
 def pyllicagram(recherche,corpus="presse",debut=1789,fin=1950,resolution="default",somme=False):
         if not isinstance(recherche, str) and not isinstance(recherche, list):
             raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
         if not isinstance(recherche, list): recherche = [recherche]
         assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
         assert resolution in ["default","annee","mois"], 'Vous devez choisir la résolution parmi "default", "annee" ou "mois"'
-        for gram in recherche:
+        result = []
+        for gram in tqdm(recherche):
                 gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace("+"," ")
                 gram = gram.replace(" ","%20")
-                df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus={corpus}&mot={gram}&from={debut}&to={fin}")
-                if resolution=="mois" and corpus != "livres":
-                        df = df.groupby(["annee","mois", "gram"]).agg({'n':'sum','total':'sum'}).reset_index()
-                if resolution=="annee":
-                        df = df.groupby(["annee","gram"]).agg({'n':'sum','total':'sum'}).reset_index()
-                if 'result' in locals():
-                        result = pd.concat([result, df])
-                else:
-                        result = df
+                df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus={corpus}&mot={gram}&from={debut}&to={fin}&resolution={resolution:}")
+                #if resolution=="mois" and corpus != "livres":
+                #        df = df.groupby(["annee","mois", "gram"]).agg({'n':'sum','total':'sum'}).reset_index()
+                #if resolution=="annee":
+                #        df = df.groupby(["annee","gram"]).agg({'n':'sum','total':'sum'}).reset_index()
+                #if 'result' in locals():
+                #        result = pd.concat([result, df])
+                #else:
+                #        result = df
+                result.append(df)
+        result = pd.concat(result)
         if somme:
                 result = result.groupby(["annee",*(("mois",) if "mois" in result.columns else()),*(("jour",) if 'jour' in result.columns else())]).agg({'n':'sum','total':'mean'}).reset_index()
                 result["gram"] = "+".join(recherche)
         result["ratio"] = result.n.values/result.total.values
         return result
```


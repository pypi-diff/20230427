# Comparing `tmp/IPAkor-2.5.tar.gz` & `tmp/IPAkor-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.5.tar", last modified: Thu Apr 27 21:21:44 2023, max compression
+gzip compressed data, was "IPAkor-2.5.1.tar", last modified: Thu Apr 27 21:27:14 2023, max compression
```

## Comparing `IPAkor-2.5.tar` & `IPAkor-2.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:21:44.239821 IPAkor-2.5/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:21:44.234682 IPAkor-2.5/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.5/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.5/IPAkor/border_maker.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:21:44.237033 IPAkor-2.5/IPAkor/static/
--rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.5/IPAkor/static/final_trans.csv
--rw-r--r--   0 eneminova   (501) staff       (20)    15014 2023-04-27 21:20:08.000000 IPAkor-2.5/IPAkor/transcription.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:21:44.236735 IPAkor-2.5/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 21:21:44.000000 IPAkor-2.5/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 21:21:44.000000 IPAkor-2.5/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 21:21:44.000000 IPAkor-2.5/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 21:21:44.000000 IPAkor-2.5/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 21:21:44.000000 IPAkor-2.5/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.5/MANIFEST.in
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 21:21:44.239965 IPAkor-2.5/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.5/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 21:21:44.240476 IPAkor-2.5/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      583 2023-04-27 21:21:36.000000 IPAkor-2.5/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611902 IPAkor-2.5.1/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.609421 IPAkor-2.5.1/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.5.1/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.5.1/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611272 IPAkor-2.5.1/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.5.1/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    15016 2023-04-27 21:27:08.000000 IPAkor-2.5.1/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611005 IPAkor-2.5.1/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.5.1/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:27:14.612030 IPAkor-2.5.1/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.5.1/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 21:27:14.612583 IPAkor-2.5.1/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-27 21:25:10.000000 IPAkor-2.5.1/setup.py
```

### Comparing `IPAkor-2.5/IPAkor/border_maker.py` & `IPAkor-2.5.1/IPAkor/border_maker.py`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5/IPAkor/static/final_trans.csv` & `IPAkor-2.5.1/IPAkor/static/final_trans.csv`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5/IPAkor/transcription.py` & `IPAkor-2.5.1/IPAkor/transcription.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         for char in word:
             ready_word += '-' + self.final_trans[char]
         return ready_word.strip('-')
 
     def separator(self, text: str) -> str:
         syll_dict = dict()
 
-        with open(self.filename, 'r') as csvfile:
+        with open(self.weight_path, 'r') as csvfile:
             spamreader = csv.reader(csvfile)
             sylls = list(spamreader)
             for s in sylls:
                 syll_dict[s[0]] = s[2]
 
         good_text = ' '
         twit_morph = self.twitter.pos(text, norm=True)
@@ -360,8 +360,7 @@
         given = self.spirantization(given)
         given = self.sonor_assim(given)
         given = self.coronal_asim(given)
         given = self.patchims(given)
         given = self.voicing_and_h(given)
         given = self.pot(given)
         return given
-
```

### Comparing `IPAkor-2.5/README.md` & `IPAkor-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5/setup.py` & `IPAkor-2.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.5',
+                 version='2.5.1',
                  packages=['IPAkor'],
                  package_data={'IPAkor': ['static/final_trans.csv']},
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
```


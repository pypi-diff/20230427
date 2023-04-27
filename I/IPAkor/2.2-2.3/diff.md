# Comparing `tmp/IPAkor-2.2.tar.gz` & `tmp/IPAkor-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.2.tar", last modified: Wed Apr 26 04:37:41 2023, max compression
+gzip compressed data, was "IPAkor-2.3.tar", last modified: Thu Apr 27 20:37:38 2023, max compression
```

## Comparing `IPAkor-2.2.tar` & `IPAkor-2.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.156512 IPAkor-2.2/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.153366 IPAkor-2.2/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       63 2023-04-25 19:57:07.000000 IPAkor-2.2/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     4065 2023-04-26 04:36:37.000000 IPAkor-2.2/IPAkor/border_maker.py
--rw-r--r--   0 eneminova   (501) staff       (20)     8605 2023-04-26 04:36:37.000000 IPAkor-2.2/IPAkor/rules.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.156221 IPAkor-2.2/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      235 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:37:41.156638 IPAkor-2.2/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.2/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-26 04:37:41.157646 IPAkor-2.2/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      572 2023-04-26 04:36:37.000000 IPAkor-2.2/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.408332 IPAkor-2.3/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.403386 IPAkor-2.3/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.3/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     4085 2023-04-27 20:31:57.000000 IPAkor-2.3/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.406162 IPAkor-2.3/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.3/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    15041 2023-04-27 20:34:26.000000 IPAkor-2.3/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.405607 IPAkor-2.3/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.3/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:37:38.408453 IPAkor-2.3/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.3/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 20:37:38.408892 IPAkor-2.3/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      578 2023-04-27 20:28:43.000000 IPAkor-2.3/setup.py
```

### Comparing `IPAkor-2.2/IPAkor/border_maker.py` & `IPAkor-2.3/IPAkor/border_maker.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 from konlpy.tag import Twitter
 from konlpy.tag import Kkma
 import csv
 import re
 import wget
 
 
-class BorderMaker():
+class BorderMaker:
 
     def __init__(self):
         self.twitter = Twitter()
         self.kkma = Kkma()
 
         self.final_trans = dict()
-        self.filename = wget.download(
-            'https://raw.githubusercontent.com/Ne-minus/kor_to_phonemes/main/IPAkor/final_trans.csv')
+        self.filename = 'static/final_trans.csv'
         with open(self.filename, encoding='utf-8') as ft_file:
             spamreader = csv.reader(ft_file)
 
             for row in spamreader:
                 self.final_trans[row[0]] = row[2]
 
     def intruser(self, word: str) -> str:
@@ -86,18 +85,20 @@
                         tr = ''.join(reversed(list(rtr)))
 
                     # проверяем, аттрибутивное или предикативное употребление
                     if 'ETD' in self.kkma.pos(entity[0])[-1][1]:
                         good_text += tr + '#'
                     else:
                         good_text += tr + ' / '
-
-
             elif entity[1] == 'Punctuation':
                 good_text = good_text.strip(" /-#") + ' / '
             elif entity[1] in bad:
                 pass
 
             else:
                 good_text += self.intruser(entity[0]) + '#'
 
         return good_text.strip(' /#') + ' / '
+
+
+transcript = BorderMaker()
+print(transcript.separator('너 덕분에 또 만들거야 없지만 만들거예요'))
```

### Comparing `IPAkor-2.2/README.md` & `IPAkor-2.3/README.md`

 * *Files identical despite different names*

### Comparing `IPAkor-2.2/setup.py` & `IPAkor-2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.2',
+                 version='2.3',
+                 package_data={'static': ['*']},
                  packages=setuptools.find_packages(),
-                 include_package_data=True,
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
                  install_requires=['konlpy', 'wget'],
                  python_requires='>=3',
                  author_email='neminova2.0@gmail.com'
-                 )
+                 )
```


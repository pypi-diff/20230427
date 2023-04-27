# Comparing `tmp/IPAkor-2.3.tar.gz` & `tmp/IPAkor-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.3.tar", last modified: Thu Apr 27 20:37:38 2023, max compression
+gzip compressed data, was "IPAkor-2.4.tar", last modified: Thu Apr 27 20:43:52 2023, max compression
```

## Comparing `IPAkor-2.3.tar` & `IPAkor-2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.408332 IPAkor-2.3/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.403386 IPAkor-2.3/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.3/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     4085 2023-04-27 20:31:57.000000 IPAkor-2.3/IPAkor/border_maker.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.406162 IPAkor-2.3/IPAkor/static/
--rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.3/IPAkor/static/final_trans.csv
--rw-r--r--   0 eneminova   (501) staff       (20)    15041 2023-04-27 20:34:26.000000 IPAkor-2.3/IPAkor/transcription.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:37:38.405607 IPAkor-2.3/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 20:37:38.000000 IPAkor-2.3/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.3/MANIFEST.in
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:37:38.408453 IPAkor-2.3/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.3/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 20:37:38.408892 IPAkor-2.3/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      578 2023-04-27 20:28:43.000000 IPAkor-2.3/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:43:52.577215 IPAkor-2.4/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:43:52.574940 IPAkor-2.4/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.4/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.4/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:43:52.576725 IPAkor-2.4/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.4/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    14923 2023-04-27 20:42:31.000000 IPAkor-2.4/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:43:52.576377 IPAkor-2.4/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:43:52.000000 IPAkor-2.4/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 20:43:52.000000 IPAkor-2.4/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 20:43:52.000000 IPAkor-2.4/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 20:43:52.000000 IPAkor-2.4/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 20:43:52.000000 IPAkor-2.4/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.4/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-27 20:43:52.577333 IPAkor-2.4/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.4/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 20:43:52.577881 IPAkor-2.4/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      578 2023-04-27 20:40:43.000000 IPAkor-2.4/setup.py
```

### Comparing `IPAkor-2.3/IPAkor/border_maker.py` & `IPAkor-2.4/IPAkor/border_maker.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,11 +94,7 @@
             elif entity[1] in bad:
                 pass
 
             else:
                 good_text += self.intruser(entity[0]) + '#'
 
         return good_text.strip(' /#') + ' / '
-
-
-transcript = BorderMaker()
-print(transcript.separator('너 덕분에 또 만들거야 없지만 만들거예요'))
```

### Comparing `IPAkor-2.3/IPAkor/static/final_trans.csv` & `IPAkor-2.4/IPAkor/static/final_trans.csv`

 * *Files identical despite different names*

### Comparing `IPAkor-2.3/IPAkor/transcription.py` & `IPAkor-2.4/IPAkor/transcription.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,10 +360,7 @@
         given = self.sonor_assim(given)
         given = self.coronal_asim(given)
         given = self.patchims(given)
         given = self.voicing_and_h(given)
         given = self.pot(given)
         return given
 
-
-transcript = Transcription()
-print(transcript.transcribe('너 덕분에 또 만들거야 없지만 만들거예요'))
```

### Comparing `IPAkor-2.3/README.md` & `IPAkor-2.4/README.md`

 * *Files identical despite different names*

### Comparing `IPAkor-2.3/setup.py` & `IPAkor-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.3',
+                 version='2.4',
                  package_data={'static': ['*']},
                  packages=setuptools.find_packages(),
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
```


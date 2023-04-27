# Comparing `tmp/Pydule-3.2.6.tar.gz` & `tmp/Pydule-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.2.6.tar", last modified: Wed Apr 19 15:44:11 2023, max compression
+gzip compressed data, was "Pydule-3.2.7.tar", last modified: Thu Apr 27 14:17:53 2023, max compression
```

## Comparing `Pydule-3.2.6.tar` & `Pydule-3.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:44:11.014132 Pydule-3.2.6/
--rw-rw-rw-   0        0        0     2082 2023-04-19 15:44:11.003513 Pydule-3.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1294 2023-04-19 15:42:06.000000 Pydule-3.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 15:44:11.014132 Pydule-3.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-19 15:40:36.000000 Pydule-3.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:44:10.733695 Pydule-3.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:44:10.994959 Pydule-3.2.6/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2082 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 15:44:09.000000 Pydule-3.2.6/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7999 2023-04-19 15:35:42.000000 Pydule-3.2.6/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:17:53.429921 Pydule-3.2.7/
+-rw-rw-rw-   0        0        0     2372 2023-04-27 14:17:53.412301 Pydule-3.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1584 2023-04-27 14:15:29.000000 Pydule-3.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 14:17:53.429921 Pydule-3.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-04-27 14:10:06.000000 Pydule-3.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:17:53.352069 Pydule-3.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:17:53.405254 Pydule-3.2.7/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2372 2023-04-27 14:17:52.000000 Pydule-3.2.7/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-04-27 14:17:53.000000 Pydule-3.2.7/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:17:52.000000 Pydule-3.2.7/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-27 14:17:53.000000 Pydule-3.2.7/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 14:17:53.000000 Pydule-3.2.7/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10000 2023-04-27 14:05:46.000000 Pydule-3.2.7/src/Pydule.py
```

### Comparing `Pydule-3.2.6/PKG-INFO` & `Pydule-3.2.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.6
+Version: 3.2.7
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -16,14 +16,17 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
+- Encode and Decode a String
+- Seperate String
+- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
@@ -47,14 +50,24 @@
  ```
 # test.py
 import Pydule as py
 
 # to Search 
 py.search('Youtube')
 
+# to Swap Dictionary
+d={1:2,2:3,3:4}
+print(py.swapdict(d))
+
+# to Encode String
+string,Key=py.codestr('Hello World')
+
+# to Decode String
+print(py.dcodestr(string,swapdict(key)))
+
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
 # to Get all Available Functions
 py.functions()
```

### Comparing `Pydule-3.2.6/README.md` & `Pydule-3.2.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
+- Encode and Decode a String
+- Seperate String
+- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
@@ -33,14 +36,24 @@
  ```
 # test.py
 import Pydule as py
 
 # to Search 
 py.search('Youtube')
 
+# to Swap Dictionary
+d={1:2,2:3,3:4}
+print(py.swapdict(d))
+
+# to Encode String
+string,Key=py.codestr('Hello World')
+
+# to Decode String
+print(py.dcodestr(string,swapdict(key)))
+
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
 # to Get all Available Functions
 py.functions()
```

### Comparing `Pydule-3.2.6/setup.py` & `Pydule-3.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.2.6',
+	version='3.2.7',
 	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
```

### Comparing `Pydule-3.2.6/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.2.7/src/Pydule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.6
+Version: 3.2.7
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -16,14 +16,17 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
+- Encode and Decode a String
+- Seperate String
+- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
@@ -47,14 +50,24 @@
  ```
 # test.py
 import Pydule as py
 
 # to Search 
 py.search('Youtube')
 
+# to Swap Dictionary
+d={1:2,2:3,3:4}
+print(py.swapdict(d))
+
+# to Encode String
+string,Key=py.codestr('Hello World')
+
+# to Decode String
+print(py.dcodestr(string,swapdict(key)))
+
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
 # to Get all Available Functions
 py.functions()
```


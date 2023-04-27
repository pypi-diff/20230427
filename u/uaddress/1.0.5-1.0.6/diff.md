# Comparing `tmp/uaddress-1.0.5.tar.gz` & `tmp/uaddress-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uaddress-1.0.5.tar", last modified: Fri Mar 10 10:46:45 2023, max compression
+gzip compressed data, was "uaddress-1.0.6.tar", last modified: Thu Apr 27 10:08:50 2023, max compression
```

## Comparing `uaddress-1.0.5.tar` & `uaddress-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-03-10 10:46:45.548948 uaddress-1.0.5/
--rwxr--r--   0 jack      (1000) jack      (1000)     1084 2021-11-04 12:07:45.000000 uaddress-1.0.5/LICENSE
--rw-r--r--   0 jack      (1000) jack      (1000)     6634 2023-03-10 10:46:45.548948 uaddress-1.0.5/PKG-INFO
--rwxr--r--   0 jack      (1000) jack      (1000)     5196 2022-07-22 07:13:41.000000 uaddress-1.0.5/README.md
--rwxr--r--   0 jack      (1000) jack      (1000)      210 2023-03-10 10:46:45.548948 uaddress-1.0.5/setup.cfg
--rwxr--r--   0 jack      (1000) jack      (1000)     1033 2022-11-15 11:05:55.000000 uaddress-1.0.5/setup.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-03-10 10:46:45.544948 uaddress-1.0.5/uaddress/
--rwxr--r--   0 jack      (1000) jack      (1000)     5744 2022-11-15 11:15:55.000000 uaddress-1.0.5/uaddress/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)      639 2023-02-26 17:24:15.000000 uaddress-1.0.5/uaddress/labels.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2595 2022-11-15 11:15:46.000000 uaddress-1.0.5/uaddress/types.py
--rw-rw-r--   0 jack      (1000) jack      (1000)   164084 2023-03-10 10:41:10.000000 uaddress-1.0.5/uaddress/uaddr.crfsuite
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-03-10 10:46:45.544948 uaddress-1.0.5/uaddress.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)     6634 2023-03-10 10:46:45.000000 uaddress-1.0.5/uaddress.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      246 2023-03-10 10:46:45.000000 uaddress-1.0.5/uaddress.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-03-10 10:46:45.000000 uaddress-1.0.5/uaddress.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        9 2023-03-10 10:46:45.000000 uaddress-1.0.5/uaddress.egg-info/top_level.txt
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-04-27 10:08:50.602141 uaddress-1.0.6/
+-rwxr--r--   0 jack      (1000) jack      (1000)     1084 2023-04-27 10:04:36.000000 uaddress-1.0.6/LICENSE
+-rw-r--r--   0 jack      (1000) jack      (1000)     6634 2023-04-27 10:08:50.602141 uaddress-1.0.6/PKG-INFO
+-rwxr--r--   0 jack      (1000) jack      (1000)     5196 2022-07-22 07:13:41.000000 uaddress-1.0.6/README.md
+-rwxr--r--   0 jack      (1000) jack      (1000)      210 2023-04-27 10:08:50.602141 uaddress-1.0.6/setup.cfg
+-rwxr--r--   0 jack      (1000) jack      (1000)     1033 2023-04-27 10:04:19.000000 uaddress-1.0.6/setup.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-04-27 10:08:50.578142 uaddress-1.0.6/uaddress/
+-rwxr--r--   0 jack      (1000) jack      (1000)     5744 2023-04-13 08:56:24.000000 uaddress-1.0.6/uaddress/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      639 2023-02-26 17:24:15.000000 uaddress-1.0.6/uaddress/labels.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2665 2023-04-24 10:27:05.000000 uaddress-1.0.6/uaddress/types.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)   164084 2023-03-10 10:41:10.000000 uaddress-1.0.6/uaddress/uaddr.crfsuite
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-04-27 10:08:50.602141 uaddress-1.0.6/uaddress.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6634 2023-04-27 10:08:50.000000 uaddress-1.0.6/uaddress.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      246 2023-04-27 10:08:50.000000 uaddress-1.0.6/uaddress.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-04-27 10:08:50.000000 uaddress-1.0.6/uaddress.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        9 2023-04-27 10:08:50.000000 uaddress-1.0.6/uaddress.egg-info/top_level.txt
```

### Comparing `uaddress-1.0.5/LICENSE` & `uaddress-1.0.6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020-2022 Evgen Kytonin
+Copyright (c) 2020-2023 Evgen Kytonin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `uaddress-1.0.5/PKG-INFO` & `uaddress-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uaddress
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ukrainian address parser
 Home-page: https://github.com/RapidappsIT/uaddress
 Author: Evgen Kytonin
 Author-email: killfess@gmail.com
 License: MIT
 Description: ![header](https://github.com/RapidappsIT/uaddress/raw/master/doc/header.png)
         # Описание
```

### Comparing `uaddress-1.0.5/README.md` & `uaddress-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `uaddress-1.0.5/setup.py` & `uaddress-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         "for installing setuptools"
     )
 
 setup(
     name='uaddress',
     packages=['uaddress'],
     description='Ukrainian address parser',
-    version='1.0.5',
+    version='1.0.6',
     author='Evgen Kytonin',
     author_email='killfess@gmail.com',
     license='MIT',
     keywords=['nlp', 'ukraine', 'address', 'research', 'parsing'],
     url='https://github.com/RapidappsIT/uaddress',
     package_data={'uaddress': ['uaddr.crfsuite']},
     classifiers=[
```

### Comparing `uaddress-1.0.5/uaddress/__init__.py` & `uaddress-1.0.6/uaddress/__init__.py`

 * *Files identical despite different names*

### Comparing `uaddress-1.0.5/uaddress/labels.py` & `uaddress-1.0.6/uaddress/labels.py`

 * *Files identical despite different names*

### Comparing `uaddress-1.0.5/uaddress/types.py` & `uaddress-1.0.6/uaddress/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
     # REGION
     "обл", "обл.", "область",
     # CITY
     "м", "м.", "місто", "г", "г.", "город",
     # DISTRICT
     "р-н", "р-н.", "рн", "рн.", "р-он", "район",
     # MICRODISTRICT
-    "мікр", "мікр.", "мн", "мр", "мкрн", "мкр", "мікрорайон", "микр", "микр.", "микрорайон", "м-н",
+    "мікр", "мікр.", "мн", "мр", "мкрн", "мкр", "мікрорайон", "микр", "микр.", "микрорайон", "м-н", "м-р",
     # VILLAGE
     "пос", "пос.", "смт", "смт.", "с.м.т", "пгт", "п г т", "пгт.", "село", "селище", "поселок", "с-ще",
     # STREET    
     "вул", "вул.", "вулиця", "ул", "ул.", "улица", "влу.", "в.", "вулю", "улиця",
     "пров", "пров.", "провулок", "пер", "пер.", "переулок", "прос", "провул", "прв.", "перевуло", "про",
     "бул", "бул.", "б-р", "бр", "бр.", "бур", "бур.", "бульвар", "бульв.", "бул-р.",
     "просп", "просп.", "прт", "прт.", "прокт", "прокт.", "пр", "пр.", "п-т", "п-т.", "п-рт.", "проспект", "п-т", "пр-кт", "пр-к", "прпосп"
-    "ж\м" , "масив", "массив", "житловий масив", "жилой массив", "ж.м.",
+    "ж\м", "ж/м", "масив", "массив", "житловий масив", "жилой массив", "ж.м.",
     "ш.", "шосе", "шоссе",
     "алея", "аллея",
     "майд", "майд.", "майдан",
     "розвилка", "развилка",
     "узвіз", "спуск",
     "проїзд", "проезд",
     "дорога",
@@ -36,15 +36,17 @@
     "в'їзд", "въезд",
     "лінія", "линия",
     "траса", "трасса",
     "урочище",
     "шахта",
     "хутір", "хутор",
     "роз'їзд", "разъезд",
-    "квартал",
+    "квартал", "кв-л",
+    "присілок",
+    "плесо",
     # HOUSING
     "корп.", "корп", "корпус",
     # HOSTEL
     "гурт", "гурт.", "гуртожиток", "общ", "общ.", "общежитие",
     # HOUSE
     "буд.", "будинок", "дом", "д.", "б.",
     # APARTMENT
```

### Comparing `uaddress-1.0.5/uaddress/uaddr.crfsuite` & `uaddress-1.0.6/uaddress/uaddr.crfsuite`

 * *Files identical despite different names*

### Comparing `uaddress-1.0.5/uaddress.egg-info/PKG-INFO` & `uaddress-1.0.6/uaddress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uaddress
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ukrainian address parser
 Home-page: https://github.com/RapidappsIT/uaddress
 Author: Evgen Kytonin
 Author-email: killfess@gmail.com
 License: MIT
 Description: ![header](https://github.com/RapidappsIT/uaddress/raw/master/doc/header.png)
         # Описание
```


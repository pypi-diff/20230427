# Comparing `tmp/haytool-0.0.8.tar.gz` & `tmp/haytool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haytool-0.0.8.tar", last modified: Wed Nov 30 02:52:26 2022, max compression
+gzip compressed data, was "haytool-0.0.9.tar", last modified: Thu Apr 27 15:50:06 2023, max compression
```

## Comparing `haytool-0.0.8.tar` & `haytool-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 02:52:26.135084 haytool-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-11-30 02:52:16.000000 haytool-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      575 2022-11-30 02:52:26.135084 haytool-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-30 02:52:16.000000 haytool-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 02:52:26.135084 haytool-0.0.8/haytool/
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/audio.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/file_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2022-11-30 02:52:16.000000 haytool-0.0.8/haytool/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 02:52:26.135084 haytool-0.0.8/haytool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      575 2022-11-30 02:52:26.000000 haytool-0.0.8/haytool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      348 2022-11-30 02:52:26.000000 haytool-0.0.8/haytool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 02:52:26.000000 haytool-0.0.8/haytool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-11-30 02:52:26.000000 haytool-0.0.8/haytool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-30 02:52:26.000000 haytool-0.0.8/haytool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 02:52:26.135084 haytool-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      755 2022-11-30 02:52:16.000000 haytool-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:50:06.562200 haytool-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-27 15:49:52.000000 haytool-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 15:50:06.562200 haytool-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 15:49:52.000000 haytool-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:50:06.562200 haytool-0.0.9/haytool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-27 15:49:52.000000 haytool-0.0.9/haytool/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:50:06.562200 haytool-0.0.9/haytool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 15:50:06.000000 haytool-0.0.9/haytool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 15:50:06.000000 haytool-0.0.9/haytool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:50:06.000000 haytool-0.0.9/haytool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 15:50:06.000000 haytool-0.0.9/haytool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 15:50:06.000000 haytool-0.0.9/haytool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:50:06.562200 haytool-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 15:49:52.000000 haytool-0.0.9/setup.py
```

### Comparing `haytool-0.0.8/LICENSE` & `haytool-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/PKG-INFO` & `haytool-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haytool
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hayman's toolbox
 Author: Hayman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `haytool-0.0.8/haytool/__init__.py` & `haytool-0.0.9/haytool/__init__.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool/dataframe.py` & `haytool-0.0.9/haytool/dataframe.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool/file_helper.py` & `haytool-0.0.9/haytool/file_helper.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool/json.py` & `haytool-0.0.9/haytool/json.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool/parallel.py` & `haytool-0.0.9/haytool/parallel.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool/string.py` & `haytool-0.0.9/haytool/string.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,7 +8,11 @@
     words = random.randint(3, 20) if freestyle else 1
     for word in range(words):
         string_length = random.randint(2, 12) if string_length is None else string_length
         rando_word = ''.join(secrets.choice(string.ascii_uppercase + string.ascii_lowercase) for i in range(string_length))
         gen_words.append(rando_word)
         string_length = None
     return ' '.join(gen_words)
+
+
+def generate_random_numbers(num_length, start_zero=False):
+    return ''.join([str(random.randint(0 if start_zero else 1, 9)) for x in range(num_length)])
```

### Comparing `haytool-0.0.8/haytool/time.py` & `haytool-0.0.9/haytool/time.py`

 * *Files identical despite different names*

### Comparing `haytool-0.0.8/haytool.egg-info/PKG-INFO` & `haytool-0.0.9/haytool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haytool
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hayman's toolbox
 Author: Hayman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `haytool-0.0.8/setup.py` & `haytool-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='haytool',
-    version='0.0.8',
+    version='0.0.9',
     description="Hayman's toolbox",
     long_description_content_type='text/markdown',
     author='Hayman',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```


# Comparing `tmp/with_timeout-0.0.2.tar.gz` & `tmp/with_timeout-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "with_timeout-0.0.2.tar", last modified: Thu Apr 27 14:01:50 2023, max compression
+gzip compressed data, was "with_timeout-0.0.3.tar", last modified: Thu Apr 27 14:06:06 2023, max compression
```

## Comparing `with_timeout-0.0.2.tar` & `with_timeout-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:01:50.808736 with_timeout-0.0.2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1069 2023-04-27 12:58:14.000000 with_timeout-0.0.2/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)       17 2023-04-27 13:07:40.000000 with_timeout-0.0.2/MANIFEST.in
--rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:01:50.808798 with_timeout-0.0.2/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      154 2023-04-27 13:07:40.000000 with_timeout-0.0.2/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)       79 2023-04-27 14:01:50.808998 with_timeout-0.0.2/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      739 2023-04-27 14:01:14.000000 with_timeout-0.0.2/setup.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:01:50.808657 with_timeout-0.0.2/with_timeout.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:01:50.000000 with_timeout-0.0.2/with_timeout.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      243 2023-04-27 14:01:50.000000 with_timeout-0.0.2/with_timeout.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-04-27 14:01:50.000000 with_timeout-0.0.2/with_timeout.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       17 2023-04-27 14:01:50.000000 with_timeout-0.0.2/with_timeout.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       13 2023-04-27 14:01:50.000000 with_timeout-0.0.2/with_timeout.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1304 2023-04-27 13:02:50.000000 with_timeout-0.0.2/with_timeout.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:06:06.821612 with_timeout-0.0.3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1069 2023-04-27 12:58:14.000000 with_timeout-0.0.3/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)       17 2023-04-27 13:07:40.000000 with_timeout-0.0.3/MANIFEST.in
+-rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:06:06.821678 with_timeout-0.0.3/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      154 2023-04-27 13:07:40.000000 with_timeout-0.0.3/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)       79 2023-04-27 14:06:06.821932 with_timeout-0.0.3/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      734 2023-04-27 14:05:32.000000 with_timeout-0.0.3/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:06:06.821503 with_timeout-0.0.3/with_timeout.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:06:06.000000 with_timeout-0.0.3/with_timeout.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      243 2023-04-27 14:06:06.000000 with_timeout-0.0.3/with_timeout.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-04-27 14:06:06.000000 with_timeout-0.0.3/with_timeout.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       15 2023-04-27 14:06:06.000000 with_timeout-0.0.3/with_timeout.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       13 2023-04-27 14:06:06.000000 with_timeout-0.0.3/with_timeout.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1304 2023-04-27 13:02:50.000000 with_timeout-0.0.3/with_timeout.py
```

### Comparing `with_timeout-0.0.2/LICENSE` & `with_timeout-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `with_timeout-0.0.2/PKG-INFO` & `with_timeout-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: with_timeout
-Version: 0.0.2
+Version: 0.0.3
 Summary: 模拟requests的timeout参数，使任意函数都拥有超时跳出的功能，防止访问超时阻塞影响代码的运行
 Home-page: https://github.com/snjyor/with_timeout
 Author: Jeffrey Yang
 Author-email: snjyor@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `with_timeout-0.0.2/setup.py` & `with_timeout-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 abs_path = path.abspath(path.dirname(__file__))
 with io.open(path.join(abs_path, 'README.md'), encoding='utf-8') as f:
     readme_data = f.read()
 
 setup(
     name='with_timeout',
     py_modules=['with_timeout'],
-    version='0.0.2',
+    version='0.0.3',
     description='模拟requests的timeout参数，使任意函数都拥有超时跳出的功能，防止访问超时阻塞影响代码的运行',
     author='Jeffrey Yang',
     author_email='snjyor@163.com',
     url='https://github.com/snjyor/with_timeout',
     install_requires=[
-        'functools', 'signal'
+        'beautifulsoup4'
     ],
     license='MIT',
     long_description=readme_data,
     long_description_content_type='text/markdown',
 )
```

### Comparing `with_timeout-0.0.2/with_timeout.egg-info/PKG-INFO` & `with_timeout-0.0.3/with_timeout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: with-timeout
-Version: 0.0.2
+Version: 0.0.3
 Summary: 模拟requests的timeout参数，使任意函数都拥有超时跳出的功能，防止访问超时阻塞影响代码的运行
 Home-page: https://github.com/snjyor/with_timeout
 Author: Jeffrey Yang
 Author-email: snjyor@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `with_timeout-0.0.2/with_timeout.py` & `with_timeout-0.0.3/with_timeout.py`

 * *Files identical despite different names*


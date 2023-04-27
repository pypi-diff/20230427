# Comparing `tmp/m-utilities-1.0.4.tar.gz` & `tmp/m-utilities-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-utilities-1.0.4.tar", last modified: Mon Mar 27 05:50:07 2023, max compression
+gzip compressed data, was "m-utilities-1.0.5.tar", last modified: Thu Apr 27 03:09:40 2023, max compression
```

## Comparing `m-utilities-1.0.4.tar` & `m-utilities-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:50:07.174168 m-utilities-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1194 2023-03-27 05:50:07.173168 m-utilities-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-03-27 05:49:05.000000 m-utilities-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:50:07.172168 m-utilities-1.0.4/m_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1194 2023-03-27 05:50:07.000000 m-utilities-1.0.4/m_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-03-27 05:50:07.000000 m-utilities-1.0.4/m_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 05:50:07.000000 m-utilities-1.0.4/m_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      187 2023-03-27 05:50:07.000000 m-utilities-1.0.4/m_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 05:50:07.000000 m-utilities-1.0.4/m_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 05:50:07.174168 m-utilities-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1287 2023-03-27 05:50:06.000000 m-utilities-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:09:40.979000 m-utilities-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-27 03:09:40.978000 m-utilities-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      741 2023-04-27 03:08:29.000000 m-utilities-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:09:40.977000 m-utilities-1.0.5/m_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-27 03:09:40.000000 m-utilities-1.0.5/m_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-27 03:09:40.000000 m-utilities-1.0.5/m_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:09:40.000000 m-utilities-1.0.5/m_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2023-04-27 03:09:40.000000 m-utilities-1.0.5/m_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:09:40.000000 m-utilities-1.0.5/m_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 03:09:40.979000 m-utilities-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-04-27 03:09:39.000000 m-utilities-1.0.5/setup.py
```

### Comparing `m-utilities-1.0.4/PKG-INFO` & `m-utilities-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.
 Home-page: UNKNOWN
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Description: # MobioUtilities
         
@@ -13,14 +13,14 @@
         Danh sách các thư viện:
         * m-singleton==0.3 (https://pypi.org/project/m-singleton)
         * m-monitor==0.6  (https://pypi.org/project/m-monitor)
         * m-validator==0.1 (https://pypi.org/project/m-validator)
         * m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
         * m-cipher==1.5.1 (https://pypi.org/project/m-cipher)
         * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
-        * m-caching==0.1.8 (https://pypi.org/project/m-caching)
+        * m-caching==0.1.12 (https://pypi.org/project/m-caching)
         * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
         * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
-        * m-kafka-sdk-v2==0.1.5 (https://pypi.org/project/m-kafka-sdk-v2)
+        * m-kafka-sdk-v2==0.1.7 (https://pypi.org/project/m-kafka-sdk-v2)
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `m-utilities-1.0.4/README.md` & `m-utilities-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 Danh sách các thư viện:
 * m-singleton==0.3 (https://pypi.org/project/m-singleton)
 * m-monitor==0.6  (https://pypi.org/project/m-monitor)
 * m-validator==0.1 (https://pypi.org/project/m-validator)
 * m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
 * m-cipher==1.5.1 (https://pypi.org/project/m-cipher)
 * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
-* m-caching==0.1.8 (https://pypi.org/project/m-caching)
+* m-caching==0.1.12 (https://pypi.org/project/m-caching)
 * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
 * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
-* m-kafka-sdk-v2==0.1.5 (https://pypi.org/project/m-kafka-sdk-v2)
+* m-kafka-sdk-v2==0.1.7 (https://pypi.org/project/m-kafka-sdk-v2)
```

### Comparing `m-utilities-1.0.4/m_utilities.egg-info/PKG-INFO` & `m-utilities-1.0.5/m_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.
 Home-page: UNKNOWN
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Description: # MobioUtilities
         
@@ -13,14 +13,14 @@
         Danh sách các thư viện:
         * m-singleton==0.3 (https://pypi.org/project/m-singleton)
         * m-monitor==0.6  (https://pypi.org/project/m-monitor)
         * m-validator==0.1 (https://pypi.org/project/m-validator)
         * m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
         * m-cipher==1.5.1 (https://pypi.org/project/m-cipher)
         * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
-        * m-caching==0.1.8 (https://pypi.org/project/m-caching)
+        * m-caching==0.1.12 (https://pypi.org/project/m-caching)
         * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
         * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
-        * m-kafka-sdk-v2==0.1.5 (https://pypi.org/project/m-kafka-sdk-v2)
+        * m-kafka-sdk-v2==0.1.7 (https://pypi.org/project/m-kafka-sdk-v2)
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `m-utilities-1.0.4/setup.py` & `m-utilities-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 # read the contents of your README file
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 version_dev='1.0.0'
-version_prod='1.0.4'
+version_prod='1.0.5'
 
 run_mode=''
 
 setup(name='m-utilities' + run_mode,
-      version='1.0.4',
+      version='1.0.5',
       description='Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.',
       url='',
       author='MOBIO',
       author_email='contact@mobio.vn',
       license='MIT',
       package_dir={'': './'},
       packages=find_packages('./'),
       install_requires=['m-singleton==0.3',
                         'm-monitor==0.6',
                         'm-validator==0.1',
                         'm-filetypes==0.1.5',
                         'm-cipher==1.5.1',
                         'm-schedule==0.6.7',
-                        'm-caching==0.1.10',
+                        'm-caching==0.1.12',
                         'm-threadpool==0.2',
                         'm-formatter-logging>=1.0.2',
-                        'm-kafka-sdk-v2==0.1.5',
+                        'm-kafka-sdk-v2==0.1.7',
                         ],
       long_description=long_description,
       long_description_content_type='text/markdown',
       python_requires='>=3.8'
       )
```


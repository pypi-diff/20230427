# Comparing `tmp/lazy_testdata-1.1.8.tar.gz` & `tmp/lazy_testdata-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lazy_testdata-1.1.8.tar", last modified: Tue Jun  1 09:18:40 2021, max compression
+gzip compressed data, was "lazy_testdata-1.1.9.tar", last modified: Tue Jan 17 06:19:40 2023, max compression
```

## Comparing `lazy_testdata-1.1.8.tar` & `lazy_testdata-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 qa         (501) staff       (20)        0 2021-06-01 09:18:40.098809 lazy_testdata-1.1.8/
--rw-r--r--   0 qa         (501) staff       (20)     1133 2021-06-01 09:18:40.098515 lazy_testdata-1.1.8/PKG-INFO
--rwxrwxrwx   0 qa         (501) staff       (20)      412 2020-06-08 02:44:23.000000 lazy_testdata-1.1.8/README.md
-drwxr-xr-x   0 qa         (501) staff       (20)        0 2021-06-01 09:18:40.095386 lazy_testdata-1.1.8/lazy_testdata/
--rwxrwxrwx   0 qa         (501) staff       (20)       22 2018-08-06 01:37:33.000000 lazy_testdata-1.1.8/lazy_testdata/__init__.py
--rwxrwxrwx   0 qa         (501) staff       (20)    28242 2018-01-17 02:03:59.000000 lazy_testdata-1.1.8/lazy_testdata/chinacitycode.py
--rwxrwxrwx   0 qa         (501) staff       (20)     1676 2018-01-17 02:03:41.000000 lazy_testdata-1.1.8/lazy_testdata/chinesecardbin.py
--rwxrwxrwx   0 qa         (501) staff       (20)    32708 2019-09-23 06:49:23.000000 lazy_testdata-1.1.8/lazy_testdata/chinesename.py
--rwxrwxrwx   0 qa         (501) staff       (20)    22450 2021-06-01 09:18:16.000000 lazy_testdata-1.1.8/lazy_testdata/core.py
--rwxrwxrwx   0 qa         (501) staff       (20)      567 2020-08-21 06:04:45.000000 lazy_testdata-1.1.8/lazy_testdata/dbhelper.py
--rwxrwxrwx   0 qa         (501) staff       (20)      523 2019-09-23 07:38:40.000000 lazy_testdata-1.1.8/lazy_testdata/sh_and_os_ext.py
-drwxr-xr-x   0 qa         (501) staff       (20)        0 2021-06-01 09:18:40.098093 lazy_testdata-1.1.8/lazy_testdata.egg-info/
--rwxrwxrwx   0 qa         (501) staff       (20)     1133 2021-06-01 09:18:39.000000 lazy_testdata-1.1.8/lazy_testdata.egg-info/PKG-INFO
--rwxrwxrwx   0 qa         (501) staff       (20)      399 2021-06-01 09:18:39.000000 lazy_testdata-1.1.8/lazy_testdata.egg-info/SOURCES.txt
--rwxrwxrwx   0 qa         (501) staff       (20)        1 2021-06-01 09:18:39.000000 lazy_testdata-1.1.8/lazy_testdata.egg-info/dependency_links.txt
--rwxrwxrwx   0 qa         (501) staff       (20)       74 2021-06-01 09:18:39.000000 lazy_testdata-1.1.8/lazy_testdata.egg-info/requires.txt
--rwxrwxrwx   0 qa         (501) staff       (20)       14 2021-06-01 09:18:39.000000 lazy_testdata-1.1.8/lazy_testdata.egg-info/top_level.txt
--rw-r--r--   0 qa         (501) staff       (20)       38 2021-06-01 09:18:40.098888 lazy_testdata-1.1.8/setup.cfg
--rwxrwxrwx   0 qa         (501) staff       (20)     1198 2021-06-01 09:18:07.000000 lazy_testdata-1.1.8/setup.py
+drwxr-xr-x   0 yuweipeng   (501) staff       (20)        0 2023-01-17 06:19:40.557353 lazy_testdata-1.1.9/
+-rw-r--r--   0 yuweipeng   (501) staff       (20)     1022 2023-01-17 06:19:40.557097 lazy_testdata-1.1.9/PKG-INFO
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)      412 2020-06-08 02:44:23.000000 lazy_testdata-1.1.9/README.md
+drwxr-xr-x   0 yuweipeng   (501) staff       (20)        0 2023-01-17 06:19:40.555089 lazy_testdata-1.1.9/lazy_testdata/
+-rw-r--r--   0 yuweipeng   (501) staff       (20)       22 2023-01-17 01:58:17.000000 lazy_testdata-1.1.9/lazy_testdata/__init__.py
+-rw-r--r--   0 yuweipeng   (501) staff       (20)    28242 2023-01-17 01:58:17.000000 lazy_testdata-1.1.9/lazy_testdata/chinacitycode.py
+-rw-r--r--   0 yuweipeng   (501) staff       (20)     1676 2023-01-17 01:58:17.000000 lazy_testdata-1.1.9/lazy_testdata/chinesecardbin.py
+-rw-r--r--   0 yuweipeng   (501) staff       (20)    32708 2023-01-17 01:58:17.000000 lazy_testdata-1.1.9/lazy_testdata/chinesename.py
+-rw-r--r--   0 yuweipeng   (501) staff       (20)    22588 2023-01-17 06:18:57.000000 lazy_testdata-1.1.9/lazy_testdata/core.py
+-rw-r--r--   0 yuweipeng   (501) staff       (20)      567 2023-01-17 01:58:17.000000 lazy_testdata-1.1.9/lazy_testdata/dbhelper.py
+drwxr-xr-x   0 yuweipeng   (501) staff       (20)        0 2023-01-17 06:19:40.556684 lazy_testdata-1.1.9/lazy_testdata.egg-info/
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)     1022 2023-01-17 06:19:40.000000 lazy_testdata-1.1.9/lazy_testdata.egg-info/PKG-INFO
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)      368 2023-01-17 06:19:40.000000 lazy_testdata-1.1.9/lazy_testdata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)        1 2023-01-17 06:19:40.000000 lazy_testdata-1.1.9/lazy_testdata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)       74 2023-01-17 06:19:40.000000 lazy_testdata-1.1.9/lazy_testdata.egg-info/requires.txt
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)       14 2023-01-17 06:19:40.000000 lazy_testdata-1.1.9/lazy_testdata.egg-info/top_level.txt
+-rw-r--r--   0 yuweipeng   (501) staff       (20)       38 2023-01-17 06:19:40.557448 lazy_testdata-1.1.9/setup.cfg
+-rwxrwxrwx   0 yuweipeng   (501) staff       (20)     1130 2023-01-17 06:19:14.000000 lazy_testdata-1.1.9/setup.py
```

### Comparing `lazy_testdata-1.1.8/lazy_testdata/chinacitycode.py` & `lazy_testdata-1.1.9/lazy_testdata/chinacitycode.py`

 * *Files identical despite different names*

### Comparing `lazy_testdata-1.1.8/lazy_testdata/chinesecardbin.py` & `lazy_testdata-1.1.9/lazy_testdata/chinesecardbin.py`

 * *Files identical despite different names*

### Comparing `lazy_testdata-1.1.8/lazy_testdata/chinesename.py` & `lazy_testdata-1.1.9/lazy_testdata/chinesename.py`

 * *Files identical despite different names*

### Comparing `lazy_testdata-1.1.8/lazy_testdata/core.py` & `lazy_testdata-1.1.9/lazy_testdata/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,21 +93,23 @@
                 7: '5',
                 8: '4',
                 9: '3',
                 10: '2'
             }
             return bd[b]
 
-    def create_idcard(self):
+    def create_idcard(self, min_age=18, max_age=50, city_code_list=None) -> str:
         """
         身份证
         """
         cur = datetime.now()
-        id = str(random.choice(CITYCODE_LIST))  #地区码
-        id = id + str(random.randint(cur.year-100, cur.year-18))  #年份项
+        if not city_code_list:
+            city_code_list = CITYCODE_LIST
+        id = str(random.choice(city_code_list))  #地区码
+        id = id + str(random.randint(cur.year-max_age, cur.year-min_age))  #年份项
         da = date.today() + timedelta(days=random.randint(1, 366))  #月份和日期项
         id = id + da.strftime('%m%d')
         id = id + str(random.randint(100, 300))  #顺序号简单处理
         id = id + self._generateCheckCode(id)
         return id
 
     def create_bankcardno(self):
```

### Comparing `lazy_testdata-1.1.8/lazy_testdata/dbhelper.py` & `lazy_testdata-1.1.9/lazy_testdata/dbhelper.py`

 * *Files identical despite different names*

### Comparing `lazy_testdata-1.1.8/setup.py` & `lazy_testdata-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 '''
 Author: yuweipeng
 Date: 2019-09-23 15:49:54
 LastEditors: yuweipeng
-LastEditTime: 2020-10-30 10:24:21
+LastEditTime: 2023-01-17 14:19:14
 Description: file content
 '''
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazy_testdata",
-    version="1.1.8",
+    version="1.1.9",
     author="YuWeiPeng",
     author_email="404051211@qq.com",
     description="""
     testdata include chinese personal four element and offen use datetime 测试数据包含随机生成的中国公民四要素，及常用的日期时间
-    通过身份证号获得性别、生日、年龄，识别真伪
     根据swagger文档生成规则用例
     """,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.cnblogs.com/yicaifeitian/",
     packages=setuptools.find_packages(),
     classifiers=["Programming Language :: Python :: 3",
```


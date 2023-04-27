# Comparing `tmp/jmcomic-1.7.0.tar.gz` & `tmp/jmcomic-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-gp4omas4/jmcomic-1.7.0.tar", last modified: Tue Apr 25 03:16:19 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-hgonnaqk/jmcomic-1.8.0.tar", last modified: Thu Apr 27 06:39:37 2023, max compression
```

## Comparing `jmcomic-1.7.0.tar` & `jmcomic-1.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 03:16:07.000000 jmcomic-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-25 03:16:19.000000 jmcomic-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-25 03:16:07.000000 jmcomic-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:16:19.000000 jmcomic-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 03:16:07.000000 jmcomic-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:39:37.000000 jmcomic-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 06:39:21.000000 jmcomic-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-27 06:39:37.000000 jmcomic-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-27 06:39:21.000000 jmcomic-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:39:37.000000 jmcomic-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-27 06:39:21.000000 jmcomic-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-04-27 06:39:21.000000 jmcomic-1.8.0/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 06:39:37.000000 jmcomic-1.8.0/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.7.0/LICENSE` & `jmcomic-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/PKG-INFO` & `jmcomic-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-1.7.0/README.md` & `jmcomic-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/setup.py` & `jmcomic-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic/api.py` & `jmcomic-1.8.0/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_client.py` & `jmcomic-1.8.0/src/jmcomic/jm_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -137,17 +137,20 @@
             raise AssertionError(f"请求失败，"
                                  f"响应状态码为{resp.status_code}，"
                                  f"URL=[{resp.url}]，"
                                  +
                                  (f"响应文本=[{resp.text}]" if len(resp.text) < 50 else
                                   f'响应文本过长(len={len(resp.text)})，不打印')
                                  )
+        # 图片请求，直接返回
+        if is_api is False:
+            return resp
 
-        if is_api is True:
-            JmModuleConfig.check_html(resp.text.strip(), url)
+        # 检查请求是否成功
+        self.require_resp_success_else_raise(resp, url)
 
         return resp
 
     # -- 类方法 --
 
     @classmethod
     def is_empty_image(cls, resp):
@@ -185,14 +188,35 @@
 
     def get_jmcomic_url(self, postman=None):
         return JmModuleConfig.get_jmcomic_url(postman or self)
 
     def get_jmcomic_url_all(self, postman=None):
         return JmModuleConfig.get_jmcomic_url_all(postman or self)
 
+    @classmethod
+    def require_resp_success_else_raise(cls, resp, url):
+        # 1. 是否 album_missing
+        if resp.url.endswith('/error/album_missing'):
+            raise AssertionError(f'请求的本子不存在！({url})\n'
+                                 '原因可能为:\n'
+                                 '1. id有误，检查你的本子/章节id\n'
+                                 '2. 该漫画只对登录用户可见，请配置你的cookies\n')
+
+        # 2. 是否是特殊html页
+        cls.check_special_html(resp.text.strip(), url)
+
+    @classmethod
+    def check_special_html(cls, html: str, url=None):
+        html = html.strip()
+        error_msg = JmModuleConfig.JM_ERROR_RESPONSE_HTML.get(html, None)
+        if error_msg is None:
+            return
+
+        raise AssertionError(f'{error_msg}' + f': {url}' if url is not None else '')
+
 
 # 爬取策略
 class FetchStrategy:
 
     def __init__(self,
                  from_index,
                  photo_len,
```

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_config.py` & `jmcomic-1.8.0/src/jmcomic/jm_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,19 +98,10 @@
         resp = postman.get(cls.JM_PUB_URL)
         if resp.status_code != 200:
             raise AssertionError(resp.text)
 
         from .jm_toolkit import JmcomicText
         return JmcomicText.analyse_jm_pub_html(resp.text)
 
-    @classmethod
-    def check_html(cls, html: str, url=None):
-        html = html.strip()
-        error_msg = cls.JM_ERROR_RESPONSE_HTML.get(html, None)
-        if error_msg is None:
-            return
-
-        raise AssertionError(f'{error_msg}' + f': {url}' if url is not None else '')
-
 
 jm_debug = JmModuleConfig.jm_debug
 disable_jm_debug = JmModuleConfig.disable_jm_debug
```

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_entity.py` & `jmcomic-1.8.0/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_option.py` & `jmcomic-1.8.0/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_service.py` & `jmcomic-1.8.0/src/jmcomic/jm_service.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic/jm_toolkit.py` & `jmcomic-1.8.0/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.7.0/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-1.8.0/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


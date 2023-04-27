# Comparing `tmp/fuo_netease-0.9.4.tar.gz` & `tmp/fuo_netease-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_netease-0.9.4.tar", last modified: Mon Mar 27 14:10:02 2023, max compression
+gzip compressed data, was "fuo_netease-0.9.5.tar", last modified: Thu Apr 27 07:21:30 2023, max compression
```

## Comparing `fuo_netease-0.9.4.tar` & `fuo_netease-0.9.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 14:10:01.810000 fuo_netease-0.9.4/
--rw-rw-rw-   0        0        0      516 2023-03-27 14:10:04.000000 fuo_netease-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     2400 2023-03-27 12:47:54.000000 fuo_netease-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 14:10:01.810000 fuo_netease-0.9.4/fuo_netease/
--rw-rw-rw-   0        0        0      987 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/__init__.py
--rw-rw-rw-   0        0        0    24670 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/api.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:10:01.820000 fuo_netease-0.9.4/fuo_netease/assets/
--rw-rw-rw-   0        0        0     5332 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/assets/icon.svg
-drwxrwxrwx   0        0        0        0 2023-03-27 14:10:01.820000 fuo_netease-0.9.4/fuo_netease/cloud_helpers/
--rw-rw-rw-   0        0        0     1056 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/cloud_helpers/__init__.py
--rw-rw-rw-   0        0        0     7300 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/cloud_helpers/cloud_api.py
--rw-rw-rw-   0        0        0    10206 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/cloud_helpers/security.py
--rw-rw-rw-   0        0        0      188 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/consts.py
--rw-rw-rw-   0        0        0     3226 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/downloader.py
--rw-rw-rw-   0        0        0      176 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/excs.py
--rw-rw-rw-   0        0        0     3519 2023-03-27 12:47:52.000000 fuo_netease-0.9.4/fuo_netease/login_controller.py
--rw-rw-rw-   0        0        0     7803 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/models.py
--rw-rw-rw-   0        0        0     3710 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/nem.py
--rw-rw-rw-   0        0        0      709 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/page_daily_recommendation.py
--rw-rw-rw-   0        0        0     3130 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/page_explore.py
--rw-rw-rw-   0        0        0     4966 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/page_fav.py
--rw-rw-rw-   0        0        0    15658 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/provider.py
--rw-rw-rw-   0        0        0    10914 2023-03-27 12:47:52.000000 fuo_netease-0.9.4/fuo_netease/schemas.py
--rw-rw-rw-   0        0        0     5127 2023-01-08 06:11:10.000000 fuo_netease-0.9.4/fuo_netease/ui.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:10:01.820000 fuo_netease-0.9.4/fuo_netease.egg-info/
--rw-rw-rw-   0        0        0      516 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      128 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-27 14:10:02.000000 fuo_netease-0.9.4/fuo_netease.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       98 2023-03-27 14:10:04.000000 fuo_netease-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-03-27 12:47:54.000000 fuo_netease-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23986 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/cloud_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/login_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/nem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_daily_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/setup.py
```

### Comparing `fuo_netease-0.9.4/PKG-INFO` & `fuo_netease-0.9.5/fuo_netease.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1
-Name: fuo_netease
-Version: 0.9.4
-Summary: feeluown netease plugin
-Home-page: https://github.com/feeluown/feeluown-netease
-Author: Cosven
-Author-email: yinshaowen241@gmail.com
-Keywords: feeluown,plugin,netease
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: fuo-netease
+Version: 0.9.5
+Summary: feeluown netease plugin
+Home-page: https://github.com/feeluown/feeluown-netease
+Author: Cosven
+Author-email: yinshaowen241@gmail.com
+License: UNKNOWN
+Description: UNKNOWN
+Keywords: feeluown,plugin,netease
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Provides-Extra: dev
```

### Comparing `fuo_netease-0.9.4/README.md` & `fuo_netease-0.9.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,87 @@
-# feeluown 网易云音乐插件
-
-[![Build](https://github.com/feeluown/feeluown-netease/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/feeluown/feeluown-netease/actions/workflows/build.yml)
-[![PyPI](https://img.shields.io/pypi/v/fuo_netease.svg)](https://pypi.python.org/pypi/fuo-netease)
-[![Coverage Status](https://coveralls.io/repos/github/feeluown/feeluown-netease/badge.svg?branch=master)](https://coveralls.io/github/feeluown/feeluown-netease?branch=master)
-
-## 安装
-
-```sh
-pip3 install fuo-netease
-```
-
-## changelog
-### 0.9.4 (2023-03-27)
-- 提供专辑发布日期数据
-- 优化登陆时错误处理
-
-### 0.9.3 (2022-12-07)
-- 修复获取每日推荐失败的问题
-
-### 0.9.2 (2022-06-29)
-- 修复加载用户名/歌单失败的问题
-
-### 0.9.1 (2022-04-14)
-- 修复歌单只能加载前 50 首的问题
-
-### 0.9 (2022-03-30)
-- 适配 FeelUOwn 最新版以提升稳定性
-- 更好的支持云盘歌曲，比如上传等
-
-### 0.8 (2021-11-06)
-- 新增个人电台功能
-- 移除老的 SongModel/MvModel 等，适配 library v2
-
-### 0.7.1 (2021-06-25)
-- 修复 https://github.com/feeluown/FeelUOwn/issues/474
-
-### 0.7 (2021-06-01)
-- 支持云盘歌曲
-- 修复不能显示歌曲评论的问题
-
-### 0.6 (2021-04-23)
-- 适配 fuo 若干新功能
-  - 平台图标
-  - 支持 library current_user 接口
-  - 改进对多品质音乐的支持
-- 加入一个发现音乐的页面
-
-### 0.5 (2021-01-07)
-- 适配 fuo library v2，支持相似歌曲、歌曲评论
-
-### 0.4.4 (2020-12-30)
-- 修复不能搜索歌单的问题 #11
-- 支持展示收藏歌手 #11
-- 支持使用国外手机号登录 #14
-
-### 0.4.3 (2020-08-21)
-- 用户没有绑定手机号时，进行提醒 [bugfix](https://github.com/feeluown/FeelUOwn/issues/389)
-
-### 0.4.2 (2020-02-08)
-- 依赖 feeluown>=3.3.10
-- 支持显示我的专辑收藏
-- 支持每日推荐
-
-### 0.4.1 (2020-02-08)
-- 支持私人 FM，依赖 feeluown>=3.3.9
-
-### 0.4 (2019-11-27)
-- 使用 marshmallow >= 3.0
-- 启用单测和质量检查，并接入 travis，
-
-### 0.3 (2019-10-28)
-
-- 支持获取歌手专辑
-- 支持获取播放列表的所有歌曲
-
-### 0.2 (2019-06-30)
-
-- 适配 fuocore.models.Media 新设计
-- 支持多品质音乐
-
-### 0.1 (2019-03-18)
-
-- 支持用户登录、歌曲搜索、歌词/歌曲/mv/歌手/专辑详情获取
+# feeluown 网易云音乐插件
+
+[![Build](https://github.com/feeluown/feeluown-netease/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/feeluown/feeluown-netease/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/fuo_netease.svg)](https://pypi.python.org/pypi/fuo-netease)
+[![Coverage Status](https://coveralls.io/repos/github/feeluown/feeluown-netease/badge.svg?branch=master)](https://coveralls.io/github/feeluown/feeluown-netease?branch=master)
+
+## 安装
+
+```sh
+pip3 install fuo-netease
+```
+
+## changelog
+### 0.9.5 (2023-04-27)
+- 提供双语歌词
+
+### 0.9.4 (2023-03-27)
+- 提供专辑发布日期数据
+- 优化登陆时错误处理
+
+### 0.9.3 (2022-12-07)
+- 修复获取每日推荐失败的问题
+
+### 0.9.2 (2022-06-29)
+- 修复加载用户名/歌单失败的问题
+
+### 0.9.1 (2022-04-14)
+- 修复歌单只能加载前 50 首的问题
+
+### 0.9 (2022-03-30)
+- 适配 FeelUOwn 最新版以提升稳定性
+- 更好的支持云盘歌曲，比如上传等
+
+### 0.8 (2021-11-06)
+- 新增个人电台功能
+- 移除老的 SongModel/MvModel 等，适配 library v2
+
+### 0.7.1 (2021-06-25)
+- 修复 https://github.com/feeluown/FeelUOwn/issues/474
+
+### 0.7 (2021-06-01)
+- 支持云盘歌曲
+- 修复不能显示歌曲评论的问题
+
+### 0.6 (2021-04-23)
+- 适配 fuo 若干新功能
+  - 平台图标
+  - 支持 library current_user 接口
+  - 改进对多品质音乐的支持
+- 加入一个发现音乐的页面
+
+### 0.5 (2021-01-07)
+- 适配 fuo library v2，支持相似歌曲、歌曲评论
+
+### 0.4.4 (2020-12-30)
+- 修复不能搜索歌单的问题 #11
+- 支持展示收藏歌手 #11
+- 支持使用国外手机号登录 #14
+
+### 0.4.3 (2020-08-21)
+- 用户没有绑定手机号时，进行提醒 [bugfix](https://github.com/feeluown/FeelUOwn/issues/389)
+
+### 0.4.2 (2020-02-08)
+- 依赖 feeluown>=3.3.10
+- 支持显示我的专辑收藏
+- 支持每日推荐
+
+### 0.4.1 (2020-02-08)
+- 支持私人 FM，依赖 feeluown>=3.3.9
+
+### 0.4 (2019-11-27)
+- 使用 marshmallow >= 3.0
+- 启用单测和质量检查，并接入 travis，
+
+### 0.3 (2019-10-28)
+
+- 支持获取歌手专辑
+- 支持获取播放列表的所有歌曲
+
+### 0.2 (2019-06-30)
+
+- 适配 fuocore.models.Media 新设计
+- 支持多品质音乐
+
+### 0.1 (2019-03-18)
+
+- 支持用户登录、歌曲搜索、歌词/歌曲/mv/歌手/专辑详情获取
```

### Comparing `fuo_netease-0.9.4/fuo_netease/api.py` & `fuo_netease-0.9.5/fuo_netease/api.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,684 +1,684 @@
-#!/usr/bin/env python
-# encoding: UTF-8
-
-import base64
-import binascii
-import hashlib
-import os
-import json
-import logging
-
-from bs4 import BeautifulSoup
-import requests
-from Crypto.Cipher import AES
-
-from .excs import NeteaseIOError
-
-site_uri = 'http://music.163.com'
-uri = 'http://music.163.com/api'
-uri_we = 'http://music.163.com/weapi'
-uri_v1 = 'http://music.163.com/weapi/v1'
-uri_v3 = 'http://music.163.com/weapi/v3'
-uri_e = 'https://music.163.com/eapi'
-
-logger = logging.getLogger(__name__)
-
-
-class CodeShouldBe200(NeteaseIOError):
-    def __init__(self, data):
-        self._code = data['code']
-
-    def __str__(self):
-        return 'json code field should be 200, got {}'.format(self._code)
-
-
-class API(object):
-    def __init__(self):
-        super().__init__()
-        self.headers = {
-            'Host': 'music.163.com',
-            'Connection': 'keep-alive',
-            'Referer': 'http://music.163.com/',
-            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2)'
-                          ' AppleWebKit/537.36 (KHTML, like Gecko)'
-                          ' Chrome/33.0.1750.152 Safari/537.36'
-        }
-        self._cookies = dict(appver="1.2.1", os="osx")
-        self._http = None
-
-    @property
-    def cookies(self):
-        return self._cookies
-
-    def load_cookies(self, cookies):
-        self._cookies.update(cookies)
-        # 云盘资源发布仅有似乎不支持osx平台
-        self._cookies.update(dict(appver="7.2.24", os="android"))
-
-    def set_http(self, http):
-        self._http = http
-
-    @property
-    def http(self):
-        return requests if self._http is None else self._http
-
-    def request(self, method, action, query=None, timeout=2):
-        # logger.info('method=%s url=%s data=%s' % (method, action, query))
-        if method == "GET":
-            res = self.http.get(action, headers=self.headers,
-                                cookies=self._cookies, timeout=timeout)
-        elif method == "POST":
-            res = self.http.post(action, data=query, headers=self.headers,
-                                 cookies=self._cookies, timeout=timeout)
-        elif method == "POST_UPDATE":
-            res = self.http.post(action, data=query, headers=self.headers,
-                                 cookies=self._cookies, timeout=timeout)
-            self._cookies.update(res.cookies.get_dict())
-        content = res.content
-        content_str = content.decode('utf-8')
-        content_dict = json.loads(content_str)
-        return content_dict
-
-    def login(self, country_code, username, pw_encrypt, phone=False):
-        action = 'http://music.163.com/api/login/'
-        phone_action = 'http://music.163.com/api/login/cellphone/'
-        data = {
-            'password': pw_encrypt,
-            'rememberLogin': 'true'
-        }
-        if username.isdigit() and (len(username) == 11 or country_code):
-            phone = True
-            data.update({'phone': username, 'countrycode': country_code or '86'})
-        else:
-            data.update({'username': username})
-        if phone:
-            res_data = self.request("POST_UPDATE", phone_action, data)
-            return res_data
-        else:
-            res_data = self.request("POST_UPDATE", action, data)
-            return res_data
-
-    def check_cookies(self):
-        url = uri + '/push/init'
-        data = self.request("POST_UPDATE", url, {})
-        if data['code'] == 200:
-            return True
-        return False
-
-    def confirm_captcha(self, captcha_id, text):
-        action = uri + '/image/captcha/verify/hf?id=' + str(captcha_id) +\
-            '&captcha=' + str(text)
-        data = self.request('GET', action)
-        return data
-
-    def get_captcha_url(self, captcha_id):
-        action = 'http://music.163.com/captcha?id=' + str(captcha_id)
-        return action
-
-    def user_profile(self, user_id):
-        """
-        {'nickname': 'cosven',
-         'avatarImg': 'xx.jpg',
-         'userType': 0,
-         'authStatus': 0,
-         'expertTags': None,
-         'backgroundUrl': 'xx.jpg',
-         'playCount': 2892,
-         'createdplCnt': 8,
-         'starPlaylist': {...},
-         'playlist': [...],
-         'code': 200
-        }
-        """
-        action = uri_we + '/share/userprofile/info'
-        data = {'userId': user_id}
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', action, payload)
-        code = res_data['code']
-        if code == 200:
-            return res_data
-        elif code == 400:
-            logger.warn(f'user:{user_id} may be invalid')
-        raise CodeShouldBe200(res_data)
-
-    # 用户歌单
-    def user_playlists(self, uid, offset=0, limit=200):
-        action = uri + '/user/playlist/?offset=' + str(offset) +\
-            '&limit=' + str(limit) + '&uid=' + str(uid)
-        data = self.request('GET', action)
-        if data['code'] == 200:
-            return data['playlist']
-        return []
-
-    def user_favorite_albums(self, offset=0, limit=30):
-        action = uri_we + '/album/sublist'
-        data = {
-            'offset': offset,
-            'limit': limit,
-            'csrf_token': self._cookies.get('__csrf')}
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', action, payload)
-        if res_data['code'] == 200:
-            return res_data
-        return None
-
-    def user_favorite_artists(self, offset=0, limit=30):
-        action = uri_we + '/artist/sublist'
-        data = {
-            'offset': offset,
-            'limit': limit,
-            'csrf_token': self._cookies.get('__csrf')}
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', action, payload)
-        if res_data['code'] == 200:
-            return res_data
-        return None
-
-    # 搜索单曲(1)，歌手(100)，专辑(10)，歌单(1000)，用户(1002) *(type)*
-    def search(self, s, stype=1, offset=0, total='true', limit=30):
-        """get songs list from search keywords"""
-        action = uri + '/search/get'
-        data = {
-            's': s,
-            'type': stype,
-            'offset': offset,
-            'total': total,
-            'limit': limit
-        }
-        resp = self.request('POST', action, data)
-        if resp['code'] == 200:
-            return resp['result']
-        return []
-
-    def playlist_detail_v3(self, pid, offset=0, limit=200):
-        """
-        该接口返回的 ['playlist']['trackIds'] 字段会包含所有的歌曲
-        """
-        action = '/playlist/detail'
-        url = uri_v3 + action
-        data = dict(id=pid, limit=limit, offset=offset, n=limit)
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', url, payload)
-        if res_data['code'] == 200:
-            return res_data['playlist']
-        raise CodeShouldBe200(res_data)
-
-    def update_playlist_name(self, pid, name):
-        url = uri + '/playlist/update/name'
-        data = {
-            'id': pid,
-            'name': name
-        }
-        res_data = self.request('POST', url, data)
-        return res_data
-
-    def new_playlist(self, uid, name='default'):
-        url = uri + '/playlist/create'
-        data = {
-            'uid': uid,
-            'name': name
-        }
-        res_data = self.request('POST', url, data)
-        return res_data
-
-    def delete_playlist(self, pid):
-        url = uri + '/playlist/delete'
-        data = {
-            'id': pid,
-            'pid': pid
-        }
-        return self.request('POST', url, data)
-
-    def artist_infos(self, artist_id):
-        """
-        :param artist_id: artist_id
-        :return: {
-            code: int,
-            artist: {artist},
-            more: boolean,
-            hotSongs: [songs]
-        }
-        """
-        action = uri + '/artist/' + str(artist_id)
-        data = self.request('GET', action)
-        return data
-
-    def artist_songs(self, artist_id, offset=0, limit=50):
-        action = uri_we + '/artist/songs'
-        data = dict(id=artist_id, limit=limit, offset=offset, n=limit)
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', action, payload)
-        if res_data['code'] == 200:
-            return res_data
-        raise CodeShouldBe200(res_data)
-
-    def artist_albums(self, artist_id, offset=0, limit=20):
-        action = ('{uri}/artist/albums/{artist_id}?'
-                  'offset={offset}&limit={limit}')
-        action = action.format(uri=uri,
-                               artist_id=artist_id,
-                               offset=offset,
-                               limit=limit)
-        data = self.request('GET', action)
-        return data
-
-    # album id --> song id set
-    def album_infos(self, album_id):
-        """
-        :param album_id:
-        :return: {
-            code: int,
-            album: { album }
-        }
-        """
-        action = uri + '/album/' + str(album_id)
-        data = self.request('GET', action)
-        if data['code'] == 200:
-            return data['album']
-
-    def album_desc(self, album_id):
-        action = site_uri + '/album'
-        data = {'id': album_id}
-        res = self.http.get(action, data, headers=self.headers)
-        if res is None:
-            return None
-        soup = BeautifulSoup(res.content, 'html.parser')
-        albdescs = soup.select('.n-albdesc')
-        if albdescs:
-            return albdescs[0].prettify()
-        return ''
-
-    def artist_desc(self, artist_id):
-        action = site_uri + '/artist/desc'
-        data = {'id': artist_id}
-        res = self.http.get(action, data, headers=self.headers)
-        if res is None:
-            return None
-        soup = BeautifulSoup(res.content, 'html.parser')
-        artdescs = soup.select('.n-artdesc')
-        if artdescs:
-            artdesc = artdescs[0]
-            # FIXME: 艺术家描述是 html 格式的，它有一个 header 为
-            # ``<h2>{artist_name}简介</h2>``, 而在 FeelUOwn 的 UI 设计中，
-            # FeelUown 是把艺术家描述显示在艺术家名字下面，
-            # 而艺术家名字也是用 ``<h2>{artist_name}</h2>`` 来渲染的，
-            # 这样在视觉上就会出现两个非常相似的文字，非常难看，
-            # 所以我们在这里把描述中的标题去掉。
-            # 另外，我们还把描述中所有的 h2 header 替换成 h3 header。
-            artdesc.h2.decompose()
-            for h2 in artdesc.select('h2'):
-                h2.name = 'h3'
-            return artdesc.prettify()
-        return ''
-
-    # song id --> song url ( details )
-    def song_detail(self, music_id):
-        action = uri + '/song/detail/?id=' + str(music_id) + '&ids=[' +\
-            str(music_id) + ']'
-        data = self.request('GET', action)
-        if data['songs']:
-            return data['songs'][0]
-        return
-
-    def weapi_songs_url(self, music_ids, bitrate=320000):
-        """
-        When the expected bitrate song url does not exist, server will
-        return a fallback song url. For example, we request a song
-        url with bitrate=320000. If there only exists a song url with
-        bitrate=128000, the server will return it.
-
-        NOTE(cosven): After some manual testing, we found that the url is
-        None in following cases:
-        1. the song is for vip-user and the current user is not vip.
-        2. the song is a paid song and the current user(may be a vip)
-           has not bought it.
-        """
-        url = uri_we + '/song/enhance/player/url'
-        data = {
-            'ids': music_ids,
-            'br': bitrate,
-            'csrf_token': self._cookies.get('__csrf')
-        }
-        payload = self.encrypt_request(data)
-        data = self.request('POST', url, payload)
-        if data['code'] == 200:
-            return data['data']
-        return []
-
-    def songs_detail(self, music_ids):
-        """批量获取歌曲的详细信息（老版）
-
-        经过测试 music_ids 不能超过 200 个。
-        """
-        music_ids = [str(music_id) for music_id in music_ids]
-        action = uri + '/song/detail?ids=[' +\
-            ','.join(music_ids) + ']'
-        data = self.request('GET', action)
-        if data['code'] == 200:
-            return data['songs']
-        return []
-
-    def songs_detail_v3(self, music_ids):
-        """批量获取歌曲的详细信息
-
-        经过测试 music_ids 不能超过 1000 个
-        """
-        action = '/song/detail'
-        url = uri_v3 + action
-        params = {
-            'c': json.dumps([{'id': id_} for id_ in music_ids]),
-            'ids': json.dumps(music_ids)
-        }
-        payload = self.encrypt_request(params)
-        data = self.request('POST', url, payload)
-        if data['code'] == 200:
-            return data['songs']
-        return []
-
-    def op_music_to_playlist(self, mid, pid, op):
-        """
-        :param op: add or del
-        """
-        url_add = uri + '/playlist/manipulate/tracks'
-        trackIds = '["' + str(mid) + '"]'
-        data_add = {
-            'tracks': str(mid),  # music id
-            'pid': str(pid),    # playlist id
-            'trackIds': trackIds,  # music id str
-            'op': op   # opation
-        }
-        data = self.request('POST', url_add, data_add)
-        print(data)
-        code = data.get('code')
-
-        # 从歌单中成功的移除歌曲时，code 是 200
-        # 当从歌单中移除一首不存在的歌曲时，code 也是 200
-        # 当向歌单添加歌曲时，如果歌曲已经在列表当中，返回 code 为 502
-        # code 为 521 时，可能是因为：绑定手机号后才可操作哦
-        if code == 200:
-            return 1
-        elif code == 502:
-            return -1
-        else:
-            return 0
-
-    def set_music_favorite(self, mid, flag):
-        url = uri + '/song/like'
-        data = {
-            "trackId": mid,
-            "like": str(flag).lower(),
-            "time": 0
-        }
-        return self.request("POST", url, data)
-
-    def get_radio_music(self):
-        url = uri + '/radio/get'
-        data = self.request('GET', url)
-        if data['code'] == 200:
-            return data['data']
-        return None
-
-    def get_mv_detail(self, mvid):
-        """Get mv detail
-        :param mvid: mv id
-        :return:
-        """
-        url = uri + '/mv/detail?id=' + str(mvid)
-        data = self.request('GET', url)
-        if data['code'] == 200:
-            return data['data']
-        raise CodeShouldBe200(data)
-
-    def get_lyric_by_songid(self, mid):
-        """Get song lyric
-        :param mid: music id
-        :return: {
-            lrc: {
-                version: int,
-                lyric: str
-            },
-            tlyric: {
-                version: int,
-                lyric: str
-            }
-            sgc: bool,
-            qfy: bool,
-            sfy: bool,
-            transUser: {},
-            code: int,
-        }
-        """
-        # tv 表示翻译。-1：表示要翻译，1：不要
-        url = uri + '/song/lyric?' + 'id=' + str(mid) + '&lv=1&kv=1&tv=-1'
-        return self.request('GET', url)
-
-    def get_similar_song(self, mid, offset=0, limit=10):
-        url = (f"http://music.163.com/api/discovery/simiSong"
-               f"?songid={mid}&offset={offset}&total=true&limit={limit}")
-        data = self.request('GET', url)
-        if data['code'] == 200:
-            return data['songs']
-        raise CodeShouldBe200(data)
-
-    def get_recommend_songs(self):
-        url = uri_v3 + '/discovery/recommend/songs'
-        payload = self.encrypt_request({})
-        res_data = self.request('POST', url, payload)
-        print(res_data)
-        if res_data['code'] == 200:
-            return res_data['data']['dailySongs']
-        raise CodeShouldBe200(res_data)
-
-    def get_recommend_playlists(self):
-        url = uri + '/discovery/recommend/resource'
-        payload = self.encrypt_request({})
-        data = self.request('POST', url, payload)
-        if data['code'] == 200:
-            return data['recommend']
-        raise CodeShouldBe200(data)
-
-    def get_comment(self, comment_id):
-        data = {
-            'rid': comment_id,
-            'offset': '0',
-            'total': 'true',
-            'limit': '20',
-            'csrf_token': self._cookies.get('__csrf')
-        }
-        url = uri_v1 + '/resource/comments/' + comment_id
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', url, payload)
-        if res_data['code'] == 200:
-            return res_data
-        raise CodeShouldBe200(res_data)
-
-    def accumulate_pl_count(self, mid):
-        data = {"ids": "[%d]" % mid, "br": 128000,
-                "csrf_token": self._cookies.get('__scrf')}
-        url = uri_we + '/pl/count'
-        payload = self.encrypt_request(data)
-        return self.request('POST', url, payload)
-
-    def cloud_songs(self, offset=0, limit=30):
-        data = dict(limit=limit, offset=offset)
-        url = uri_v1 + '/cloud/get'
-        payload = self.encrypt_request(data)
-        res_data = self.request('POST', url, payload)
-        if res_data['code'] == 200:
-            return res_data
-        raise CodeShouldBe200(res_data)
-
-    def cloud_songs_detail(self, music_ids):
-        data = dict(songIds=music_ids.split(","))
-        url = uri_v1 + '/cloud/get/byids'
-        payload = self.encrypt_request(data)
-        return self.request('POST', url, payload)
-
-    def cloud_songs_delete(self, music_ids):
-        data = dict(songIds=music_ids.split(","))
-        url = uri_we + '/cloud/del'
-        payload = self.encrypt_request(data)
-        return self.request('POST', url, payload)
-
-    def cloud_song_match(self, sid, asid):
-        url = uri + f'/cloud/user/song/match?songId={sid}&adjustSongId={asid}'
-        data = self.request('GET', url)
-        if data['code'] == 200:
-            return data['data']
-        raise CodeShouldBe200(data)
-
-    def cloud_song_upload(self, path):
-        def md5sum(file):
-            md5sum = hashlib.md5()
-            with open(file, 'rb') as f:
-                # while chunk := f.read():
-                #     md5sum.update(chunk)
-                md5sum.update(f.read())
-            return md5sum
-
-        from .cloud_helpers.cloud_api import Cloud_API
-        cloud_api = Cloud_API(self, uri_e)
-
-        fname = os.path.basename(path)
-        fext = path.split('.')[-1]
-        '''Parsing file names'''
-        fsize = os.stat(path).st_size
-        md5 = md5sum(path).hexdigest()
-        logger.debug(f'[-] Checking file ( MD5: {md5} )')
-        cresult = cloud_api.GetCheckCloudUpload(md5)
-        if cresult['code'] != 200:
-            return 'UPLOAD_CHECK_FAILED'
-
-        '''网盘资源发布 4 步走：'''
-        '''1.拿到上传令牌 - 需要文件名，MD5，文件大小'''
-        token = cloud_api.GetNosToken(fname, md5, fsize, fext)
-        if token['code'] != 200:
-            return 'TOKEN_ALLOC_FAILED'
-        token = token['result']
-
-        '''2. 若文件未曾上传完毕，则完成其上传'''
-        if cresult['needUpload']:
-            logger.info(f'[+] {fname} needs to be uploaded ( {fsize} B )')
-            try:
-                upload_result = cloud_api.SetUploadObject(
-                    open(path, 'rb'),
-                    md5, fsize, token['objectKey'], token['token']
-                )
-            except Exception:
-                return 'UPLOAD_FAILED'
-            logger.debug(f'[-] Response:\n  {upload_result}')
-
-        '''3. 提交资源'''
-        songId = cresult['songId']
-        logger.debug(f'''[!] Assuming upload has finished,preparing to submit
-        ID  :   {songId}
-        MD5 :   {md5}
-        NAME:   {fname}''')
-        metadata = cloud_api.GetMetadata(path)
-        submit_result = cloud_api.SetUploadCloudInfo(
-            token['resourceId'], songId, md5, fname,
-            song=metadata.get('title', '.'),
-            artist=metadata.get('artist', '.'),
-            album=metadata.get('album', '.')
-        )
-        if submit_result['code'] != 200:
-            return 'SUBMIT_FAILED'
-        logger.debug(f'[-] Response:\n  {submit_result}')
-
-        '''4. 发布资源'''
-        publish_result = cloud_api.SetPublishCloudResource(submit_result['songId'])
-        if publish_result['code'] != 200:
-            return 'PUBLISH_FAILED'
-        logger.debug(f'[-] Response:\n  {publish_result}')
-
-        return 'STATUS_SUCCEEDED'
-
-    def subscribed_djradio(self, limit=0, offset=0):
-        data = dict(limit=100, time=0, needFee=False)
-        url = uri_e + '/djradio/subed/v1'
-        payload = self.eapi_encrypt(b'/api/djradio/subed/v1', data)
-        return self.request('POST', url, {'params': payload})
-
-    def djradio_detail(self, radio_id):
-        data = dict(id=radio_id)
-        url = uri_e + '/djradio/v2/get'
-        payload = self.eapi_encrypt(b'/api/djradio/v2/get', data)
-        return self.request('POST', url, {'params': payload})
-
-    def djradio_song_detail(self, id_):
-        data = dict(id=id_)
-        url = uri_e + '/dj/program/detail'
-        payload = self.eapi_encrypt(b'/api/dj/program/detail', data)
-        return self.request('POST', url, {'params': payload})
-
-    def djradio_list(self, radio_id, limit=50, offset=0, asc=False):
-        data = dict(radioId=radio_id, limit=limit, offset=offset, asc=asc)
-        url = uri_e + '/v1/dj/program/byradio'
-        payload = self.eapi_encrypt(b'/api/v1/dj/program/byradio', data)
-        return self.request('POST', url, {'params': payload})
-
-    def _create_aes_key(self, size):
-        return (''.join([hex(b)[2:] for b in os.urandom(size)]))[0:16]
-
-    def _aes_encrypt(self, text, key):
-        pad = 16 - len(text) % 16
-        text = text + pad * chr(pad)
-        encryptor = AES.new(bytes(key, 'utf-8'), 2, b'0102030405060708')
-        enc_text = encryptor.encrypt(bytes(text, 'utf-8'))
-        enc_text_encode = base64.b64encode(enc_text)
-        return enc_text_encode
-
-    def _rsa_encrypt(self, text):
-        e = '010001'
-        n = '00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615'\
-            'bb7b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf'\
-            '695280104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46'\
-            'bee255932575cce10b424d813cfe4875d3e82047b97ddef52741d546b'\
-            '8e289dc6935b3ece0462db0a22b8e7'
-        reverse_text = text[::-1]
-        encrypted_text = pow(int(binascii.hexlify(reverse_text), 16),
-                             int(e, 16), int(n, 16))
-        return format(encrypted_text, "x").zfill(256)
-
-    def eapi_encrypt(self, path, params):
-        """
-        eapi接口参数加密
-        :param bytes path: 请求的路径
-        :param params: 请求参数
-        :return str: 加密结果
-        """
-        params = json.dumps(params, separators=(',', ':')).encode()
-        sign_src = b'nobody' + path + b'use' + params + b'md5forencrypt'
-        m = hashlib.md5()
-        m.update(sign_src)
-        sign = m.hexdigest()
-        aes_src = path + b'-36cd479b6b5-' + params + b'-36cd479b6b5-' + sign.encode()
-        pad = 16 - len(aes_src) % 16
-        aes_src = aes_src + bytearray([pad] * pad)
-        crypt = AES.new(b'e82ckenh8dichen8', AES.MODE_ECB)
-        ret = crypt.encrypt(aes_src)
-        return binascii.b2a_hex(ret).upper()
-
-    def encrypt_request(self, data):
-        text = json.dumps(data)
-        first_aes_key = '0CoJUm6Qyw8W8jud'
-        second_aes_key = self._create_aes_key(16)
-        enc_text = self._aes_encrypt(
-            self._aes_encrypt(text, first_aes_key).decode('ascii'),
-            second_aes_key).decode('ascii')
-        enc_aes_key = self._rsa_encrypt(second_aes_key.encode('ascii'))
-        payload = {
-            'params': enc_text,
-            'encSecKey': enc_aes_key,
-        }
-        return payload
-
-
-api = API()
-
-
-if __name__ == '__main__':
-    from fuo_netease.login_controller import LoginController
-    user = LoginController.load()
-    api.load_cookies(user.cookies)
-    print(api.djradio_song_detail(1883706033))
+#!/usr/bin/env python
+# encoding: UTF-8
+
+import base64
+import binascii
+import hashlib
+import os
+import json
+import logging
+
+from bs4 import BeautifulSoup
+import requests
+from Crypto.Cipher import AES
+
+from .excs import NeteaseIOError
+
+site_uri = 'http://music.163.com'
+uri = 'http://music.163.com/api'
+uri_we = 'http://music.163.com/weapi'
+uri_v1 = 'http://music.163.com/weapi/v1'
+uri_v3 = 'http://music.163.com/weapi/v3'
+uri_e = 'https://music.163.com/eapi'
+
+logger = logging.getLogger(__name__)
+
+
+class CodeShouldBe200(NeteaseIOError):
+    def __init__(self, data):
+        self._code = data['code']
+
+    def __str__(self):
+        return 'json code field should be 200, got {}'.format(self._code)
+
+
+class API(object):
+    def __init__(self):
+        super().__init__()
+        self.headers = {
+            'Host': 'music.163.com',
+            'Connection': 'keep-alive',
+            'Referer': 'http://music.163.com/',
+            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2)'
+                          ' AppleWebKit/537.36 (KHTML, like Gecko)'
+                          ' Chrome/33.0.1750.152 Safari/537.36'
+        }
+        self._cookies = dict(appver="1.2.1", os="osx")
+        self._http = None
+
+    @property
+    def cookies(self):
+        return self._cookies
+
+    def load_cookies(self, cookies):
+        self._cookies.update(cookies)
+        # 云盘资源发布仅有似乎不支持osx平台
+        self._cookies.update(dict(appver="7.2.24", os="android"))
+
+    def set_http(self, http):
+        self._http = http
+
+    @property
+    def http(self):
+        return requests if self._http is None else self._http
+
+    def request(self, method, action, query=None, timeout=2):
+        # logger.info('method=%s url=%s data=%s' % (method, action, query))
+        if method == "GET":
+            res = self.http.get(action, headers=self.headers,
+                                cookies=self._cookies, timeout=timeout)
+        elif method == "POST":
+            res = self.http.post(action, data=query, headers=self.headers,
+                                 cookies=self._cookies, timeout=timeout)
+        elif method == "POST_UPDATE":
+            res = self.http.post(action, data=query, headers=self.headers,
+                                 cookies=self._cookies, timeout=timeout)
+            self._cookies.update(res.cookies.get_dict())
+        content = res.content
+        content_str = content.decode('utf-8')
+        content_dict = json.loads(content_str)
+        return content_dict
+
+    def login(self, country_code, username, pw_encrypt, phone=False):
+        action = 'http://music.163.com/api/login/'
+        phone_action = 'http://music.163.com/api/login/cellphone/'
+        data = {
+            'password': pw_encrypt,
+            'rememberLogin': 'true'
+        }
+        if username.isdigit() and (len(username) == 11 or country_code):
+            phone = True
+            data.update({'phone': username, 'countrycode': country_code or '86'})
+        else:
+            data.update({'username': username})
+        if phone:
+            res_data = self.request("POST_UPDATE", phone_action, data)
+            return res_data
+        else:
+            res_data = self.request("POST_UPDATE", action, data)
+            return res_data
+
+    def check_cookies(self):
+        url = uri + '/push/init'
+        data = self.request("POST_UPDATE", url, {})
+        if data['code'] == 200:
+            return True
+        return False
+
+    def confirm_captcha(self, captcha_id, text):
+        action = uri + '/image/captcha/verify/hf?id=' + str(captcha_id) +\
+            '&captcha=' + str(text)
+        data = self.request('GET', action)
+        return data
+
+    def get_captcha_url(self, captcha_id):
+        action = 'http://music.163.com/captcha?id=' + str(captcha_id)
+        return action
+
+    def user_profile(self, user_id):
+        """
+        {'nickname': 'cosven',
+         'avatarImg': 'xx.jpg',
+         'userType': 0,
+         'authStatus': 0,
+         'expertTags': None,
+         'backgroundUrl': 'xx.jpg',
+         'playCount': 2892,
+         'createdplCnt': 8,
+         'starPlaylist': {...},
+         'playlist': [...],
+         'code': 200
+        }
+        """
+        action = uri_we + '/share/userprofile/info'
+        data = {'userId': user_id}
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', action, payload)
+        code = res_data['code']
+        if code == 200:
+            return res_data
+        elif code == 400:
+            logger.warn(f'user:{user_id} may be invalid')
+        raise CodeShouldBe200(res_data)
+
+    # 用户歌单
+    def user_playlists(self, uid, offset=0, limit=200):
+        action = uri + '/user/playlist/?offset=' + str(offset) +\
+            '&limit=' + str(limit) + '&uid=' + str(uid)
+        data = self.request('GET', action)
+        if data['code'] == 200:
+            return data['playlist']
+        return []
+
+    def user_favorite_albums(self, offset=0, limit=30):
+        action = uri_we + '/album/sublist'
+        data = {
+            'offset': offset,
+            'limit': limit,
+            'csrf_token': self._cookies.get('__csrf')}
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', action, payload)
+        if res_data['code'] == 200:
+            return res_data
+        return None
+
+    def user_favorite_artists(self, offset=0, limit=30):
+        action = uri_we + '/artist/sublist'
+        data = {
+            'offset': offset,
+            'limit': limit,
+            'csrf_token': self._cookies.get('__csrf')}
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', action, payload)
+        if res_data['code'] == 200:
+            return res_data
+        return None
+
+    # 搜索单曲(1)，歌手(100)，专辑(10)，歌单(1000)，用户(1002) *(type)*
+    def search(self, s, stype=1, offset=0, total='true', limit=30):
+        """get songs list from search keywords"""
+        action = uri + '/search/get'
+        data = {
+            's': s,
+            'type': stype,
+            'offset': offset,
+            'total': total,
+            'limit': limit
+        }
+        resp = self.request('POST', action, data)
+        if resp['code'] == 200:
+            return resp['result']
+        return []
+
+    def playlist_detail_v3(self, pid, offset=0, limit=200):
+        """
+        该接口返回的 ['playlist']['trackIds'] 字段会包含所有的歌曲
+        """
+        action = '/playlist/detail'
+        url = uri_v3 + action
+        data = dict(id=pid, limit=limit, offset=offset, n=limit)
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', url, payload)
+        if res_data['code'] == 200:
+            return res_data['playlist']
+        raise CodeShouldBe200(res_data)
+
+    def update_playlist_name(self, pid, name):
+        url = uri + '/playlist/update/name'
+        data = {
+            'id': pid,
+            'name': name
+        }
+        res_data = self.request('POST', url, data)
+        return res_data
+
+    def new_playlist(self, uid, name='default'):
+        url = uri + '/playlist/create'
+        data = {
+            'uid': uid,
+            'name': name
+        }
+        res_data = self.request('POST', url, data)
+        return res_data
+
+    def delete_playlist(self, pid):
+        url = uri + '/playlist/delete'
+        data = {
+            'id': pid,
+            'pid': pid
+        }
+        return self.request('POST', url, data)
+
+    def artist_infos(self, artist_id):
+        """
+        :param artist_id: artist_id
+        :return: {
+            code: int,
+            artist: {artist},
+            more: boolean,
+            hotSongs: [songs]
+        }
+        """
+        action = uri + '/artist/' + str(artist_id)
+        data = self.request('GET', action)
+        return data
+
+    def artist_songs(self, artist_id, offset=0, limit=50):
+        action = uri_we + '/artist/songs'
+        data = dict(id=artist_id, limit=limit, offset=offset, n=limit)
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', action, payload)
+        if res_data['code'] == 200:
+            return res_data
+        raise CodeShouldBe200(res_data)
+
+    def artist_albums(self, artist_id, offset=0, limit=20):
+        action = ('{uri}/artist/albums/{artist_id}?'
+                  'offset={offset}&limit={limit}')
+        action = action.format(uri=uri,
+                               artist_id=artist_id,
+                               offset=offset,
+                               limit=limit)
+        data = self.request('GET', action)
+        return data
+
+    # album id --> song id set
+    def album_infos(self, album_id):
+        """
+        :param album_id:
+        :return: {
+            code: int,
+            album: { album }
+        }
+        """
+        action = uri + '/album/' + str(album_id)
+        data = self.request('GET', action)
+        if data['code'] == 200:
+            return data['album']
+
+    def album_desc(self, album_id):
+        action = site_uri + '/album'
+        data = {'id': album_id}
+        res = self.http.get(action, data, headers=self.headers)
+        if res is None:
+            return None
+        soup = BeautifulSoup(res.content, 'html.parser')
+        albdescs = soup.select('.n-albdesc')
+        if albdescs:
+            return albdescs[0].prettify()
+        return ''
+
+    def artist_desc(self, artist_id):
+        action = site_uri + '/artist/desc'
+        data = {'id': artist_id}
+        res = self.http.get(action, data, headers=self.headers)
+        if res is None:
+            return None
+        soup = BeautifulSoup(res.content, 'html.parser')
+        artdescs = soup.select('.n-artdesc')
+        if artdescs:
+            artdesc = artdescs[0]
+            # FIXME: 艺术家描述是 html 格式的，它有一个 header 为
+            # ``<h2>{artist_name}简介</h2>``, 而在 FeelUOwn 的 UI 设计中，
+            # FeelUown 是把艺术家描述显示在艺术家名字下面，
+            # 而艺术家名字也是用 ``<h2>{artist_name}</h2>`` 来渲染的，
+            # 这样在视觉上就会出现两个非常相似的文字，非常难看，
+            # 所以我们在这里把描述中的标题去掉。
+            # 另外，我们还把描述中所有的 h2 header 替换成 h3 header。
+            artdesc.h2.decompose()
+            for h2 in artdesc.select('h2'):
+                h2.name = 'h3'
+            return artdesc.prettify()
+        return ''
+
+    # song id --> song url ( details )
+    def song_detail(self, music_id):
+        action = uri + '/song/detail/?id=' + str(music_id) + '&ids=[' +\
+            str(music_id) + ']'
+        data = self.request('GET', action)
+        if data['songs']:
+            return data['songs'][0]
+        return
+
+    def weapi_songs_url(self, music_ids, bitrate=320000):
+        """
+        When the expected bitrate song url does not exist, server will
+        return a fallback song url. For example, we request a song
+        url with bitrate=320000. If there only exists a song url with
+        bitrate=128000, the server will return it.
+
+        NOTE(cosven): After some manual testing, we found that the url is
+        None in following cases:
+        1. the song is for vip-user and the current user is not vip.
+        2. the song is a paid song and the current user(may be a vip)
+           has not bought it.
+        """
+        url = uri_we + '/song/enhance/player/url'
+        data = {
+            'ids': music_ids,
+            'br': bitrate,
+            'csrf_token': self._cookies.get('__csrf')
+        }
+        payload = self.encrypt_request(data)
+        data = self.request('POST', url, payload)
+        if data['code'] == 200:
+            return data['data']
+        return []
+
+    def songs_detail(self, music_ids):
+        """批量获取歌曲的详细信息（老版）
+
+        经过测试 music_ids 不能超过 200 个。
+        """
+        music_ids = [str(music_id) for music_id in music_ids]
+        action = uri + '/song/detail?ids=[' +\
+            ','.join(music_ids) + ']'
+        data = self.request('GET', action)
+        if data['code'] == 200:
+            return data['songs']
+        return []
+
+    def songs_detail_v3(self, music_ids):
+        """批量获取歌曲的详细信息
+
+        经过测试 music_ids 不能超过 1000 个
+        """
+        action = '/song/detail'
+        url = uri_v3 + action
+        params = {
+            'c': json.dumps([{'id': id_} for id_ in music_ids]),
+            'ids': json.dumps(music_ids)
+        }
+        payload = self.encrypt_request(params)
+        data = self.request('POST', url, payload)
+        if data['code'] == 200:
+            return data['songs']
+        return []
+
+    def op_music_to_playlist(self, mid, pid, op):
+        """
+        :param op: add or del
+        """
+        url_add = uri + '/playlist/manipulate/tracks'
+        trackIds = '["' + str(mid) + '"]'
+        data_add = {
+            'tracks': str(mid),  # music id
+            'pid': str(pid),    # playlist id
+            'trackIds': trackIds,  # music id str
+            'op': op   # opation
+        }
+        data = self.request('POST', url_add, data_add)
+        print(data)
+        code = data.get('code')
+
+        # 从歌单中成功的移除歌曲时，code 是 200
+        # 当从歌单中移除一首不存在的歌曲时，code 也是 200
+        # 当向歌单添加歌曲时，如果歌曲已经在列表当中，返回 code 为 502
+        # code 为 521 时，可能是因为：绑定手机号后才可操作哦
+        if code == 200:
+            return 1
+        elif code == 502:
+            return -1
+        else:
+            return 0
+
+    def set_music_favorite(self, mid, flag):
+        url = uri + '/song/like'
+        data = {
+            "trackId": mid,
+            "like": str(flag).lower(),
+            "time": 0
+        }
+        return self.request("POST", url, data)
+
+    def get_radio_music(self):
+        url = uri + '/radio/get'
+        data = self.request('GET', url)
+        if data['code'] == 200:
+            return data['data']
+        return None
+
+    def get_mv_detail(self, mvid):
+        """Get mv detail
+        :param mvid: mv id
+        :return:
+        """
+        url = uri + '/mv/detail?id=' + str(mvid)
+        data = self.request('GET', url)
+        if data['code'] == 200:
+            return data['data']
+        raise CodeShouldBe200(data)
+
+    def get_lyric_by_songid(self, mid):
+        """Get song lyric
+        :param mid: music id
+        :return: {
+            lrc: {
+                version: int,
+                lyric: str
+            },
+            tlyric: {
+                version: int,
+                lyric: str
+            }
+            sgc: bool,
+            qfy: bool,
+            sfy: bool,
+            transUser: {},
+            code: int,
+        }
+        """
+        # tv 表示翻译。-1：表示要翻译，1：不要
+        url = uri + '/song/lyric?' + 'id=' + str(mid) + '&lv=1&kv=1&tv=-1'
+        return self.request('GET', url)
+
+    def get_similar_song(self, mid, offset=0, limit=10):
+        url = (f"http://music.163.com/api/discovery/simiSong"
+               f"?songid={mid}&offset={offset}&total=true&limit={limit}")
+        data = self.request('GET', url)
+        if data['code'] == 200:
+            return data['songs']
+        raise CodeShouldBe200(data)
+
+    def get_recommend_songs(self):
+        url = uri_v3 + '/discovery/recommend/songs'
+        payload = self.encrypt_request({})
+        res_data = self.request('POST', url, payload)
+        print(res_data)
+        if res_data['code'] == 200:
+            return res_data['data']['dailySongs']
+        raise CodeShouldBe200(res_data)
+
+    def get_recommend_playlists(self):
+        url = uri + '/discovery/recommend/resource'
+        payload = self.encrypt_request({})
+        data = self.request('POST', url, payload)
+        if data['code'] == 200:
+            return data['recommend']
+        raise CodeShouldBe200(data)
+
+    def get_comment(self, comment_id):
+        data = {
+            'rid': comment_id,
+            'offset': '0',
+            'total': 'true',
+            'limit': '20',
+            'csrf_token': self._cookies.get('__csrf')
+        }
+        url = uri_v1 + '/resource/comments/' + comment_id
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', url, payload)
+        if res_data['code'] == 200:
+            return res_data
+        raise CodeShouldBe200(res_data)
+
+    def accumulate_pl_count(self, mid):
+        data = {"ids": "[%d]" % mid, "br": 128000,
+                "csrf_token": self._cookies.get('__scrf')}
+        url = uri_we + '/pl/count'
+        payload = self.encrypt_request(data)
+        return self.request('POST', url, payload)
+
+    def cloud_songs(self, offset=0, limit=30):
+        data = dict(limit=limit, offset=offset)
+        url = uri_v1 + '/cloud/get'
+        payload = self.encrypt_request(data)
+        res_data = self.request('POST', url, payload)
+        if res_data['code'] == 200:
+            return res_data
+        raise CodeShouldBe200(res_data)
+
+    def cloud_songs_detail(self, music_ids):
+        data = dict(songIds=music_ids.split(","))
+        url = uri_v1 + '/cloud/get/byids'
+        payload = self.encrypt_request(data)
+        return self.request('POST', url, payload)
+
+    def cloud_songs_delete(self, music_ids):
+        data = dict(songIds=music_ids.split(","))
+        url = uri_we + '/cloud/del'
+        payload = self.encrypt_request(data)
+        return self.request('POST', url, payload)
+
+    def cloud_song_match(self, sid, asid):
+        url = uri + f'/cloud/user/song/match?songId={sid}&adjustSongId={asid}'
+        data = self.request('GET', url)
+        if data['code'] == 200:
+            return data['data']
+        raise CodeShouldBe200(data)
+
+    def cloud_song_upload(self, path):
+        def md5sum(file):
+            md5sum = hashlib.md5()
+            with open(file, 'rb') as f:
+                # while chunk := f.read():
+                #     md5sum.update(chunk)
+                md5sum.update(f.read())
+            return md5sum
+
+        from .cloud_helpers.cloud_api import Cloud_API
+        cloud_api = Cloud_API(self, uri_e)
+
+        fname = os.path.basename(path)
+        fext = path.split('.')[-1]
+        '''Parsing file names'''
+        fsize = os.stat(path).st_size
+        md5 = md5sum(path).hexdigest()
+        logger.debug(f'[-] Checking file ( MD5: {md5} )')
+        cresult = cloud_api.GetCheckCloudUpload(md5)
+        if cresult['code'] != 200:
+            return 'UPLOAD_CHECK_FAILED'
+
+        '''网盘资源发布 4 步走：'''
+        '''1.拿到上传令牌 - 需要文件名，MD5，文件大小'''
+        token = cloud_api.GetNosToken(fname, md5, fsize, fext)
+        if token['code'] != 200:
+            return 'TOKEN_ALLOC_FAILED'
+        token = token['result']
+
+        '''2. 若文件未曾上传完毕，则完成其上传'''
+        if cresult['needUpload']:
+            logger.info(f'[+] {fname} needs to be uploaded ( {fsize} B )')
+            try:
+                upload_result = cloud_api.SetUploadObject(
+                    open(path, 'rb'),
+                    md5, fsize, token['objectKey'], token['token']
+                )
+            except Exception:
+                return 'UPLOAD_FAILED'
+            logger.debug(f'[-] Response:\n  {upload_result}')
+
+        '''3. 提交资源'''
+        songId = cresult['songId']
+        logger.debug(f'''[!] Assuming upload has finished,preparing to submit
+        ID  :   {songId}
+        MD5 :   {md5}
+        NAME:   {fname}''')
+        metadata = cloud_api.GetMetadata(path)
+        submit_result = cloud_api.SetUploadCloudInfo(
+            token['resourceId'], songId, md5, fname,
+            song=metadata.get('title', '.'),
+            artist=metadata.get('artist', '.'),
+            album=metadata.get('album', '.')
+        )
+        if submit_result['code'] != 200:
+            return 'SUBMIT_FAILED'
+        logger.debug(f'[-] Response:\n  {submit_result}')
+
+        '''4. 发布资源'''
+        publish_result = cloud_api.SetPublishCloudResource(submit_result['songId'])
+        if publish_result['code'] != 200:
+            return 'PUBLISH_FAILED'
+        logger.debug(f'[-] Response:\n  {publish_result}')
+
+        return 'STATUS_SUCCEEDED'
+
+    def subscribed_djradio(self, limit=0, offset=0):
+        data = dict(limit=100, time=0, needFee=False)
+        url = uri_e + '/djradio/subed/v1'
+        payload = self.eapi_encrypt(b'/api/djradio/subed/v1', data)
+        return self.request('POST', url, {'params': payload})
+
+    def djradio_detail(self, radio_id):
+        data = dict(id=radio_id)
+        url = uri_e + '/djradio/v2/get'
+        payload = self.eapi_encrypt(b'/api/djradio/v2/get', data)
+        return self.request('POST', url, {'params': payload})
+
+    def djradio_song_detail(self, id_):
+        data = dict(id=id_)
+        url = uri_e + '/dj/program/detail'
+        payload = self.eapi_encrypt(b'/api/dj/program/detail', data)
+        return self.request('POST', url, {'params': payload})
+
+    def djradio_list(self, radio_id, limit=50, offset=0, asc=False):
+        data = dict(radioId=radio_id, limit=limit, offset=offset, asc=asc)
+        url = uri_e + '/v1/dj/program/byradio'
+        payload = self.eapi_encrypt(b'/api/v1/dj/program/byradio', data)
+        return self.request('POST', url, {'params': payload})
+
+    def _create_aes_key(self, size):
+        return (''.join([hex(b)[2:] for b in os.urandom(size)]))[0:16]
+
+    def _aes_encrypt(self, text, key):
+        pad = 16 - len(text) % 16
+        text = text + pad * chr(pad)
+        encryptor = AES.new(bytes(key, 'utf-8'), 2, b'0102030405060708')
+        enc_text = encryptor.encrypt(bytes(text, 'utf-8'))
+        enc_text_encode = base64.b64encode(enc_text)
+        return enc_text_encode
+
+    def _rsa_encrypt(self, text):
+        e = '010001'
+        n = '00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615'\
+            'bb7b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf'\
+            '695280104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46'\
+            'bee255932575cce10b424d813cfe4875d3e82047b97ddef52741d546b'\
+            '8e289dc6935b3ece0462db0a22b8e7'
+        reverse_text = text[::-1]
+        encrypted_text = pow(int(binascii.hexlify(reverse_text), 16),
+                             int(e, 16), int(n, 16))
+        return format(encrypted_text, "x").zfill(256)
+
+    def eapi_encrypt(self, path, params):
+        """
+        eapi接口参数加密
+        :param bytes path: 请求的路径
+        :param params: 请求参数
+        :return str: 加密结果
+        """
+        params = json.dumps(params, separators=(',', ':')).encode()
+        sign_src = b'nobody' + path + b'use' + params + b'md5forencrypt'
+        m = hashlib.md5()
+        m.update(sign_src)
+        sign = m.hexdigest()
+        aes_src = path + b'-36cd479b6b5-' + params + b'-36cd479b6b5-' + sign.encode()
+        pad = 16 - len(aes_src) % 16
+        aes_src = aes_src + bytearray([pad] * pad)
+        crypt = AES.new(b'e82ckenh8dichen8', AES.MODE_ECB)
+        ret = crypt.encrypt(aes_src)
+        return binascii.b2a_hex(ret).upper()
+
+    def encrypt_request(self, data):
+        text = json.dumps(data)
+        first_aes_key = '0CoJUm6Qyw8W8jud'
+        second_aes_key = self._create_aes_key(16)
+        enc_text = self._aes_encrypt(
+            self._aes_encrypt(text, first_aes_key).decode('ascii'),
+            second_aes_key).decode('ascii')
+        enc_aes_key = self._rsa_encrypt(second_aes_key.encode('ascii'))
+        payload = {
+            'params': enc_text,
+            'encSecKey': enc_aes_key,
+        }
+        return payload
+
+
+api = API()
+
+
+if __name__ == '__main__':
+    from fuo_netease.login_controller import LoginController
+    user = LoginController.load()
+    api.load_cookies(user.cookies)
+    print(api.djradio_song_detail(1883706033))
```

### Comparing `fuo_netease-0.9.4/fuo_netease/assets/icon.svg` & `fuo_netease-0.9.5/fuo_netease/assets/icon.svg`

 * *Files 8% similar despite different names*

```diff
@@ -1,334 +1,329 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c73 7667 0d0a 2020  "no"?>..<svg..  
-00000040: 2078 6d6c 6e73 3a64 633d 2268 7474 703a   xmlns:dc="http:
-00000050: 2f2f 7075 726c 2e6f 7267 2f64 632f 656c  //purl.org/dc/el
-00000060: 656d 656e 7473 2f31 2e31 2f22 0d0a 2020  ements/1.1/"..  
-00000070: 2078 6d6c 6e73 3a63 633d 2268 7474 703a   xmlns:cc="http:
-00000080: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
-00000090: 732e 6f72 672f 6e73 2322 0d0a 2020 2078  s.org/ns#"..   x
-000000a0: 6d6c 6e73 3a72 6466 3d22 6874 7470 3a2f  mlns:rdf="http:/
-000000b0: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
-000000c0: 2f30 322f 3232 2d72 6466 2d73 796e 7461  /02/22-rdf-synta
-000000d0: 782d 6e73 2322 0d0a 2020 2078 6d6c 6e73  x-ns#"..   xmlns
-000000e0: 3a73 7667 3d22 6874 7470 3a2f 2f77 7777  :svg="http://www
-000000f0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000100: 220d 0a20 2020 786d 6c6e 733d 2268 7474  "..   xmlns="htt
-00000110: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00000120: 3030 302f 7376 6722 0d0a 2020 2078 6d6c  000/svg"..   xml
-00000130: 6e73 3a73 6f64 6970 6f64 693d 2268 7474  ns:sodipodi="htt
-00000140: 703a 2f2f 736f 6469 706f 6469 2e73 6f75  p://sodipodi.sou
-00000150: 7263 6566 6f72 6765 2e6e 6574 2f44 5444  rceforge.net/DTD
-00000160: 2f73 6f64 6970 6f64 692d 302e 6474 6422  /sodipodi-0.dtd"
-00000170: 0d0a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ..   xmlns:inksc
-00000180: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
-00000190: 696e 6b73 6361 7065 2e6f 7267 2f6e 616d  inkscape.org/nam
-000001a0: 6573 7061 6365 732f 696e 6b73 6361 7065  espaces/inkscape
-000001b0: 220d 0a20 2020 7769 6474 683d 2232 3536  "..   width="256
-000001c0: 2e30 7078 220d 0a20 2020 6865 6967 6874  .0px"..   height
-000001d0: 3d22 3235 362e 3070 7822 0d0a 2020 2076  ="256.0px"..   v
-000001e0: 6965 7742 6f78 3d22 3020 3020 3235 362e  iewBox="0 0 256.
-000001f0: 3020 3235 362e 3022 0d0a 2020 2076 6572  0 256.0"..   ver
-00000200: 7369 6f6e 3d22 312e 3122 0d0a 2020 2069  sion="1.1"..   i
-00000210: 643d 2253 5647 526f 6f74 220d 0a20 2020  d="SVGRoot"..   
-00000220: 736f 6469 706f 6469 3a64 6f63 6e61 6d65  sodipodi:docname
-00000230: 3d22 6e65 7465 6173 655f 6963 6f6e 2e73  ="netease_icon.s
-00000240: 7667 220d 0a20 2020 696e 6b73 6361 7065  vg"..   inkscape
-00000250: 3a76 6572 7369 6f6e 3d22 312e 302e 3120  :version="1.0.1 
-00000260: 2833 6263 3265 3831 3366 352c 2032 3032  (3bc2e813f5, 202
-00000270: 302d 3039 2d30 3729 223e 0d0a 2020 3c64  0-09-07)">..  <d
-00000280: 6566 730d 0a20 2020 2020 6964 3d22 6465  efs..     id="de
-00000290: 6673 3130 223e 0d0a 2020 2020 3c73 7479  fs10">..    <sty
-000002a0: 6c65 0d0a 2020 2020 2020 2074 7970 653d  le..       type=
-000002b0: 2274 6578 742f 6373 7322 0d0a 2020 2020  "text/css"..    
-000002c0: 2020 2069 643d 2273 7479 6c65 3131 3822     id="style118"
-000002d0: 202f 3e0d 0a20 203c 2f64 6566 733e 0d0a   />..  </defs>..
-000002e0: 2020 3c73 6f64 6970 6f64 693a 6e61 6d65    <sodipodi:name
-000002f0: 6476 6965 770d 0a20 2020 2020 6964 3d22  dview..     id="
-00000300: 6261 7365 220d 0a20 2020 2020 7061 6765  base"..     page
-00000310: 636f 6c6f 723d 2223 6666 6666 6666 220d  color="#ffffff".
-00000320: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
-00000330: 723d 2223 3636 3636 3636 220d 0a20 2020  r="#666666"..   
-00000340: 2020 626f 7264 6572 6f70 6163 6974 793d    borderopacity=
-00000350: 2231 2e30 220d 0a20 2020 2020 696e 6b73  "1.0"..     inks
-00000360: 6361 7065 3a70 6167 656f 7061 6369 7479  cape:pageopacity
-00000370: 3d22 302e 3022 0d0a 2020 2020 2069 6e6b  ="0.0"..     ink
-00000380: 7363 6170 653a 7061 6765 7368 6164 6f77  scape:pageshadow
-00000390: 3d22 3222 0d0a 2020 2020 2069 6e6b 7363  ="2"..     inksc
-000003a0: 6170 653a 7a6f 6f6d 3d22 312e 3422 0d0a  ape:zoom="1.4"..
-000003b0: 2020 2020 2069 6e6b 7363 6170 653a 6378       inkscape:cx
-000003c0: 3d22 3232 372e 3232 3237 3422 0d0a 2020  ="227.22274"..  
-000003d0: 2020 2069 6e6b 7363 6170 653a 6379 3d22     inkscape:cy="
-000003e0: 3130 362e 3522 0d0a 2020 2020 2069 6e6b  106.5"..     ink
-000003f0: 7363 6170 653a 646f 6375 6d65 6e74 2d75  scape:document-u
-00000400: 6e69 7473 3d22 7078 220d 0a20 2020 2020  nits="px"..     
-00000410: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
-00000420: 2d6c 6179 6572 3d22 6c61 7965 7231 220d  -layer="layer1".
-00000430: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000440: 6f63 756d 656e 742d 726f 7461 7469 6f6e  ocument-rotation
-00000450: 3d22 3022 0d0a 2020 2020 2073 686f 7767  ="0"..     showg
-00000460: 7269 643d 2274 7275 6522 0d0a 2020 2020  rid="true"..    
-00000470: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000480: 2d77 6964 7468 3d22 3134 3538 220d 0a20  -width="1458".. 
-00000490: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-000004a0: 646f 772d 6865 6967 6874 3d22 3130 3435  dow-height="1045
-000004b0: 220d 0a20 2020 2020 696e 6b73 6361 7065  "..     inkscape
-000004c0: 3a77 696e 646f 772d 783d 2233 3633 220d  :window-x="363".
-000004d0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-000004e0: 696e 646f 772d 793d 2231 3031 220d 0a20  indow-y="101".. 
-000004f0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-00000500: 646f 772d 6d61 7869 6d69 7a65 643d 2230  dow-maximized="0
-00000510: 223e 0d0a 2020 2020 3c69 6e6b 7363 6170  ">..    <inkscap
-00000520: 653a 6772 6964 0d0a 2020 2020 2020 2074  e:grid..       t
-00000530: 7970 653d 2278 7967 7269 6422 0d0a 2020  ype="xygrid"..  
-00000540: 2020 2020 2069 643d 2267 7269 6431 3922       id="grid19"
-00000550: 202f 3e0d 0a20 203c 2f73 6f64 6970 6f64   />..  </sodipod
-00000560: 693a 6e61 6d65 6476 6965 773e 0d0a 2020  i:namedview>..  
-00000570: 3c6d 6574 6164 6174 610d 0a20 2020 2020  <metadata..     
-00000580: 6964 3d22 6d65 7461 6461 7461 3133 223e  id="metadata13">
-00000590: 0d0a 2020 2020 3c72 6466 3a52 4446 3e0d  ..    <rdf:RDF>.
-000005a0: 0a20 2020 2020 203c 6363 3a57 6f72 6b0d  .      <cc:Work.
-000005b0: 0a20 2020 2020 2020 2020 7264 663a 6162  .         rdf:ab
-000005c0: 6f75 743d 2222 3e0d 0a20 2020 2020 2020  out="">..       
-000005d0: 203c 6463 3a66 6f72 6d61 743e 696d 6167   <dc:format>imag
-000005e0: 652f 7376 672b 786d 6c3c 2f64 633a 666f  e/svg+xml</dc:fo
-000005f0: 726d 6174 3e0d 0a20 2020 2020 2020 203c  rmat>..        <
-00000600: 6463 3a74 7970 650d 0a20 2020 2020 2020  dc:type..       
-00000610: 2020 2020 7264 663a 7265 736f 7572 6365      rdf:resource
-00000620: 3d22 6874 7470 3a2f 2f70 7572 6c2e 6f72  ="http://purl.or
-00000630: 672f 6463 2f64 636d 6974 7970 652f 5374  g/dc/dcmitype/St
-00000640: 696c 6c49 6d61 6765 2220 2f3e 0d0a 2020  illImage" />..  
-00000650: 2020 2020 2020 3c64 633a 7469 746c 653e        <dc:title>
-00000660: 3c2f 6463 3a74 6974 6c65 3e0d 0a20 2020  </dc:title>..   
-00000670: 2020 203c 2f63 633a 576f 726b 3e0d 0a20     </cc:Work>.. 
-00000680: 2020 203c 2f72 6466 3a52 4446 3e0d 0a20     </rdf:RDF>.. 
-00000690: 203c 2f6d 6574 6164 6174 613e 0d0a 2020   </metadata>..  
-000006a0: 3c67 0d0a 2020 2020 2069 6e6b 7363 6170  <g..     inkscap
-000006b0: 653a 6c61 6265 6c3d 22e5 9bbe e5b1 8220  e:label="...... 
-000006c0: 3122 0d0a 2020 2020 2069 6e6b 7363 6170  1"..     inkscap
-000006d0: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
-000006e0: 6572 220d 0a20 2020 2020 6964 3d22 6c61  er"..     id="la
-000006f0: 7965 7231 220d 0a20 2020 2020 3e0d 0a20  yer1"..     >.. 
-00000700: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-00000710: 2064 3d22 6d20 3135 352e 3834 3930 382c   d="m 155.84908,
-00000720: 362e 3438 3734 3434 3820 6320 362e 3932  6.4874448 c 6.92
-00000730: 3339 322c 2d31 2e35 3338 3635 3034 2031  392,-1.5386504 1
-00000740: 342e 3233 3235 312c 2d31 2e35 3338 3635  4.23251,-1.53865
-00000750: 3034 2032 302e 3338 3731 322c 3020 372e  04 20.38712,0 7.
-00000760: 3639 3332 352c 312e 3533 3836 3530 3420  69325,1.5386504 
-00000770: 3135 2e30 3031 3834 2c35 2e33 3835 3237  15.00184,5.38527
-00000780: 3632 2032 312e 3135 3634 342c 3130 2e33  62 21.15644,10.3
-00000790: 3835 3839 3032 2032 2e33 3037 3937 2c31  858902 2.30797,1
-000007a0: 2e35 3338 3635 3120 342e 3631 3539 352c  .538651 4.61595,
-000007b0: 332e 3834 3636 3236 2035 2e33 3835 3238  3.846626 5.38528
-000007c0: 2c36 2e39 3233 3932 3720 312e 3932 3333  ,6.923927 1.9233
-000007d0: 312c 332e 3834 3636 3236 2031 2e39 3233  1,3.846626 1.923
-000007e0: 3331 2c38 2e34 3632 3537 3720 2d31 2e35  31,8.462577 -1.5
-000007f0: 3338 3636 2c31 322e 3639 3338 3636 202d  3866,12.693866 -
-00000800: 322e 3330 3739 372c 332e 3037 3733 3031  2.30797,3.077301
-00000810: 202d 352e 3338 3532 372c 352e 3338 3532   -5.38527,5.3852
-00000820: 3737 202d 392e 3233 3139 2c36 2e31 3534  77 -9.2319,6.154
-00000830: 3630 3220 2d33 2e30 3737 332c 302e 3736  602 -3.0773,0.76
-00000840: 3933 3235 202d 362e 3135 3436 2c30 202d  9325 -6.1546,0 -
-00000850: 392e 3233 3139 2c2d 312e 3533 3836 3531  9.2319,-1.538651
-00000860: 202d 312e 3533 3836 352c 2d30 2e37 3639   -1.53865,-0.769
-00000870: 3332 3520 2d32 2e33 3037 3938 2c2d 322e  325 -2.30798,-2.
-00000880: 3330 3739 3735 202d 332e 3834 3636 332c  307975 -3.84663,
-00000890: 2d33 2e30 3737 3320 2d33 2e38 3436 3632  -3.0773 -3.84662
-000008a0: 2c2d 322e 3330 3739 3736 202d 382e 3436  ,-2.307976 -8.46
-000008b0: 3235 372c 2d34 2e36 3135 3935 3220 2d31  257,-4.615952 -1
-000008c0: 332e 3436 3331 392c 2d34 2e36 3135 3935  3.46319,-4.61595
-000008d0: 3220 2d33 2e30 3737 332c 3020 2d36 2e31  2 -3.0773,0 -6.1
-000008e0: 3534 362c 322e 3330 3739 3736 202d 382e  546,2.307976 -8.
-000008f0: 3436 3235 372c 342e 3631 3539 3532 202d  46257,4.615952 -
-00000900: 322e 3330 3739 382c 322e 3330 3739 3735  2.30798,2.307975
-00000910: 202d 332e 3037 3733 312c 352e 3338 3532   -3.07731,5.3852
-00000920: 3736 202d 322e 3330 3739 382c 382e 3436  76 -2.30798,8.46
-00000930: 3235 3737 2031 2e35 3338 3635 2c36 2e31  2577 1.53865,6.1
-00000940: 3534 3630 3220 332e 3037 3733 2c31 322e  54602 3.0773,12.
-00000950: 3639 3338 3636 2034 2e36 3135 3935 2c31  693866 4.61595,1
-00000960: 382e 3834 3834 3638 2031 312e 3932 3435  8.848468 11.9245
-00000970: 342c 302e 3736 3933 3235 2032 342e 3233  4,0.769325 24.23
-00000980: 3337 342c 332e 3834 3636 3236 2033 342e  374,3.846626 34.
-00000990: 3631 3936 342c 3130 2e33 3835 3839 2031  61964,10.38589 1
-000009a0: 302e 3338 3538 392c 362e 3135 3436 3032  0.38589,6.154602
-000009b0: 2031 382e 3834 3834 362c 3134 2e32 3332   18.84846,14.232
-000009c0: 3531 3620 3236 2e35 3431 3732 2c32 332e  516 26.54172,23.
-000009d0: 3436 3434 3233 2036 2e31 3534 362c 372e  464423 6.1546,7.
-000009e0: 3639 3332 3533 2031 312e 3135 3532 312c  693253 11.15521,
-000009f0: 3137 2e33 3039 3830 3320 3133 2e34 3633  17.309803 13.463
-00000a00: 3139 2c32 362e 3534 3137 3133 2033 2e30  19,26.541713 3.0
-00000a10: 3737 332c 3130 2e33 3835 3839 2033 2e38  773,10.38589 3.8
-00000a20: 3436 3632 2c32 312e 3135 3634 3420 332e  4662,21.15644 3.
-00000a30: 3037 3733 2c33 322e 3331 3136 3620 2d30  0773,32.31166 -0
-00000a40: 2e37 3639 3333 2c38 2e34 3632 3537 202d  .76933,8.46257 -
-00000a50: 322e 3330 3739 382c 3138 2e30 3739 3134  2.30798,18.07914
-00000a60: 202d 352e 3338 3532 382c 3235 2e37 3732   -5.38528,25.772
-00000a70: 3339 202d 372e 3639 3332 352c 3230 2e33  39 -7.69325,20.3
-00000a80: 3837 3133 202d 3231 2e39 3235 3737 2c33  8713 -21.92577,3
-00000a90: 382e 3436 3632 3720 2d34 302e 3737 3432  8.46627 -40.7742
-00000aa0: 342c 3530 2e30 3036 3135 202d 3133 2e34  4,50.00615 -13.4
-00000ab0: 3633 3139 2c38 2e34 3632 3538 202d 3238  6319,8.46258 -28
-00000ac0: 2e38 3439 3639 2c31 342e 3233 3235 3120  .84969,14.23251 
-00000ad0: 2d34 352e 3339 3031 382c 3135 2e37 3731  -45.39018,15.771
-00000ae0: 3135 202d 3131 2e31 3535 3232 2c31 2e35  15 -11.15522,1.5
-00000af0: 3338 3635 202d 3231 2e39 3235 3737 2c31  3865 -21.92577,1
-00000b00: 2e35 3338 3635 202d 3333 2e30 3830 3939  .53865 -33.08099
-00000b10: 2c2d 302e 3736 3933 3320 4320 3839 2e36  ,-0.76933 C 89.6
-00000b20: 3837 3130 382c 3234 342e 3937 3832 3420  87108,244.97824 
-00000b30: 3638 2e35 3330 3636 352c 3233 332e 3832  68.530665,233.82
-00000b40: 3330 3320 3532 2e37 3539 3439 382c 3231  303 52.759498,21
-00000b50: 372e 3238 3235 3420 3336 2e39 3838 3333  7.28254 36.98833
-00000b60: 312c 3230 312e 3531 3133 3720 3235 2e34  1,201.51137 25.4
-00000b70: 3438 3435 332c 3138 302e 3335 3439 3420  48453,180.35494 
-00000b80: 3231 2e32 3137 3136 342c 3135 382e 3432  21.217164,158.42
-00000b90: 3931 3720 3137 2e37 3535 3230 312c 3134  917 17.755201,14
-00000ba0: 322e 3237 3333 3420 3137 2e37 3535 3230  2.27334 17.75520
-00000bb0: 312c 3132 352e 3733 3238 3520 3231 2e39  1,125.73285 21.9
-00000bc0: 3836 3438 392c 3130 392e 3139 3233 3620  86489,109.19236 
-00000bd0: 3236 2e36 3032 3434 312c 3839 2e35 3734  26.602441,89.574
-00000be0: 3536 3820 3336 2e32 3139 3030 362c 3730  568 36.219006,70
-00000bf0: 2e37 3236 3120 3530 2e30 3636 3836 2c35  .7261 50.06686,5
-00000c00: 352e 3732 3432 3538 2036 312e 3939 3134  5.724258 61.9914
-00000c10: 2c34 332e 3739 3937 3138 2037 352e 3036  ,43.799718 75.06
-00000c20: 3939 3239 2c33 332e 3739 3834 3920 3930  9929,33.79849 90
-00000c30: 2e38 3431 3039 362c 3237 2e36 3433 3838  .841096,27.64388
-00000c40: 3820 6320 312e 3533 3836 352c 2d30 2e37  8 c 1.53865,-0.7
-00000c50: 3639 3332 3520 332e 3037 3733 3031 2c2d  69325 3.077301,-
-00000c60: 312e 3533 3836 3520 342e 3631 3539 3531  1.53865 4.615951
-00000c70: 2c2d 312e 3533 3836 3520 332e 3834 3636  ,-1.53865 3.8466
-00000c80: 3236 2c2d 302e 3736 3933 3235 2037 2e36  26,-0.769325 7.6
-00000c90: 3933 3235 332c 3020 3130 2e33 3835 3839  93253,0 10.38589
-00000ca0: 332c 322e 3330 3739 3735 2033 2e38 3436  3,2.307975 3.846
-00000cb0: 3633 2c33 2e30 3737 3330 3120 362e 3135  63,3.077301 6.15
-00000cc0: 3436 2c37 2e36 3933 3235 3220 352e 3338  46,7.693252 5.38
-00000cd0: 3532 382c 3132 2e36 3933 3836 3620 2d30  528,12.693866 -0
-00000ce0: 2e37 3639 3333 2c34 2e36 3135 3935 3220  .76933,4.615952 
-00000cf0: 2d33 2e38 3436 3633 2c39 2e32 3331 3930  -3.84663,9.23190
-00000d00: 3320 2d38 2e34 3632 3538 2c31 312e 3135  3 -8.46258,11.15
-00000d10: 3532 3136 202d 3135 2e37 3731 3137 2c35  5216 -15.77117,5
-00000d20: 2e33 3835 3237 3620 2d32 392e 3631 3930  .385276 -29.6190
-00000d30: 3234 2c31 362e 3534 3034 3932 202d 3339  24,16.540492 -39
-00000d40: 2e32 3335 3538 392c 3239 2e36 3139 3032  .235589,29.61902
-00000d50: 3120 2d38 2e34 3632 3537 372c 3131 2e39  1 -8.462577,11.9
-00000d60: 3234 3534 202d 3135 2e30 3031 3834 322c  2454 -15.001842,
-00000d70: 3235 2e37 3732 3339 3420 2d31 362e 3534  25.772394 -16.54
-00000d80: 3034 3932 2c34 302e 3737 3432 3334 202d  0492,40.774234 -
-00000d90: 322e 3330 3739 3736 2c31 352e 3030 3138  2.307976,15.0018
-00000da0: 3420 302c 3239 2e36 3139 3032 2034 2e36  4 0,29.61902 4.6
-00000db0: 3135 3935 312c 3433 2e30 3832 3231 2037  15951,43.08221 7
-00000dc0: 2e36 3933 3235 322c 3230 2e33 3837 3132  .693252,20.38712
-00000dd0: 2032 322e 3639 3530 3934 2c33 372e 3639   22.695094,37.69
-00000de0: 3639 3220 3431 2e35 3433 3536 322c 3436  692 41.543562,46
-00000df0: 2e39 3238 3834 2031 312e 3932 3435 3338  .92884 11.924538
-00000e00: 2c36 2e31 3534 3539 2032 342e 3233 3337  ,6.15459 24.2337
-00000e10: 3438 2c39 2e32 3331 3931 2033 372e 3639  48,9.23191 37.69
-00000e20: 3639 3338 2c38 2e34 3632 3538 2031 312e  6938,8.46258 11.
-00000e30: 3135 3532 312c 3020 3231 2e31 3536 3434  15521,0 21.15644
-00000e40: 2c2d 312e 3533 3836 3520 3331 2e35 3432  ,-1.53865 31.542
-00000e50: 3333 2c2d 352e 3338 3532 3720 382e 3436  33,-5.38527 8.46
-00000e60: 3235 382c 2d33 2e30 3737 3331 2031 372e  258,-3.07731 17.
-00000e70: 3330 3938 322c 2d37 2e36 3933 3236 2032  30982,-7.69326 2
-00000e80: 342e 3233 3337 352c 2d31 342e 3233 3235  4.23375,-14.2325
-00000e90: 3420 362e 3135 3436 2c2d 352e 3338 3532  4 6.1546,-5.3852
-00000ea0: 3820 3131 2e39 3234 3534 2c2d 3132 2e36  8 11.92454,-12.6
-00000eb0: 3933 3836 2031 362e 3534 3034 392c 2d32  9386 16.54049,-2
-00000ec0: 302e 3338 3731 3120 322e 3330 3739 372c  0.38711 2.30797,
-00000ed0: 2d33 2e38 3436 3632 2033 2e38 3436 3632  -3.84662 3.84662
-00000ee0: 2c2d 372e 3639 3332 3520 352e 3338 3532  ,-7.69325 5.3852
-00000ef0: 372c 2d31 322e 3639 3338 3620 332e 3037  7,-12.69386 3.07
-00000f00: 3733 312c 2d31 322e 3639 3338 3720 332e  731,-12.69387 3.
-00000f10: 3834 3636 332c 2d32 352e 3737 3234 2030  84663,-25.7724 0
-00000f20: 2c2d 3337 2e36 3936 3934 202d 332e 3834  ,-37.69694 -3.84
-00000f30: 3636 322c 2d38 2e34 3632 3538 202d 3130  662,-8.46258 -10
-00000f40: 2e33 3835 3839 2c2d 3138 2e30 3739 3133  .38589,-18.07913
-00000f50: 202d 3138 2e30 3739 3134 2c2d 3235 2e30   -18.07914,-25.0
-00000f60: 3033 3036 202d 332e 3834 3636 322c 2d33  0306 -3.84662,-3
-00000f70: 2e30 3737 3320 2d36 2e39 3233 3933 2c2d  .0773 -6.92393,-
-00000f80: 362e 3135 3436 3033 202d 3131 2e39 3234  6.154603 -11.924
-00000f90: 3534 2c2d 382e 3436 3235 3820 2d33 2e38  54,-8.46258 -3.8
-00000fa0: 3436 3632 2c2d 322e 3330 3739 3736 202d  4662,-2.307976 -
-00000fb0: 372e 3639 3332 352c 2d33 2e30 3737 3330  7.69325,-3.07730
-00000fc0: 3120 2d31 312e 3932 3435 342c 2d34 2e36  1 -11.92454,-4.6
-00000fd0: 3135 3935 3120 332e 3037 3733 2c31 312e  15951 3.0773,11.
-00000fe0: 3135 3532 3231 2035 2e33 3835 3238 2c32  155221 5.38528,2
-00000ff0: 312e 3932 3537 3731 2038 2e34 3632 3538  1.925771 8.46258
-00001000: 2c33 332e 3038 3039 3831 2030 2e37 3639  ,33.080981 0.769
-00001010: 3332 2c32 2e33 3037 3937 2030 2e37 3639  32,2.30797 0.769
-00001020: 3332 2c35 2e33 3835 3237 2031 2e35 3338  32,5.38527 1.538
-00001030: 3635 2c37 2e36 3933 3235 2030 2e37 3639  65,7.69325 0.769
-00001040: 3332 2c31 312e 3135 3532 3120 2d33 2e38  32,11.15521 -3.8
-00001050: 3436 3633 2c32 322e 3639 3530 3920 2d31  4663,22.69509 -1
-00001060: 312e 3135 3532 322c 3331 2e35 3432 3333  1.15522,31.54233
-00001070: 202d 362e 3932 3339 322c 372e 3639 3332   -6.92392,7.6932
-00001080: 3520 2d31 362e 3534 3034 392c 3134 2e32  5 -16.54049,14.2
-00001090: 3332 3532 202d 3236 2e35 3431 3732 2c31  3252 -26.54172,1
-000010a0: 352e 3737 3131 3720 2d31 312e 3135 3532  5.77117 -11.1552
-000010b0: 312c 322e 3330 3739 3720 2d32 332e 3436  1,2.30797 -23.46
-000010c0: 3434 322c 3020 2d33 332e 3038 3039 382c  442,0 -33.08098,
-000010d0: 2d36 2e31 3534 3620 2d39 2e32 3331 3930  -6.1546 -9.23190
-000010e0: 352c 2d35 2e33 3835 3238 202d 3135 2e37  5,-5.38528 -15.7
-000010f0: 3731 3136 392c 2d31 352e 3030 3138 3420  71169,-15.00184 
-00001100: 2d31 392e 3631 3737 3935 2c2d 3235 2e30  -19.617795,-25.0
-00001110: 3033 3037 202d 322e 3330 3739 3736 2c2d  0307 -2.307976,-
-00001120: 352e 3338 3532 3820 2d33 2e30 3737 3330  5.38528 -3.07730
-00001130: 312c 2d31 312e 3932 3435 3420 2d33 2e30  1,-11.92454 -3.0
-00001140: 3737 3330 312c 2d31 382e 3037 3931 3420  77301,-18.07914 
-00001150: 2d30 2e37 3639 3332 352c 2d31 332e 3436  -0.769325,-13.46
-00001160: 3332 2033 2e30 3737 3330 312c 2d32 362e  32 3.077301,-26.
-00001170: 3534 3137 3120 3130 2e33 3835 3839 2c2d  54171 10.38589,-
-00001180: 3337 2e36 3936 3933 3420 382e 3436 3235  37.696934 8.4625
-00001190: 3736 2c2d 3133 2e34 3633 3139 3120 3232  76,-13.463191 22
-000011a0: 2e36 3935 3039 362c 2d32 312e 3932 3537  .695096,-21.9257
-000011b0: 3638 2033 372e 3639 3639 3336 2c2d 3236  68 37.696936,-26
-000011c0: 2e35 3431 3731 3920 2d30 2e37 3639 3332  .541719 -0.76932
-000011d0: 2c2d 332e 3834 3636 3236 202d 322e 3330  ,-3.846626 -2.30
-000011e0: 3739 382c 2d38 2e34 3632 3537 3820 2d33  798,-8.462578 -3
-000011f0: 2e30 3737 332c 2d31 322e 3639 3338 3636  .0773,-12.693866
-00001200: 202d 332e 3037 3733 2c2d 392e 3233 3139   -3.0773,-9.2319
-00001210: 3033 202d 322e 3330 3739 382c 2d31 392e  03 -2.30798,-19.
-00001220: 3631 3737 3933 2032 2e33 3037 3938 2c2d  617793 2.30798,-
-00001230: 3238 2e30 3830 3337 3120 322e 3330 3739  28.080371 2.3079
-00001240: 372c 2d34 2e36 3135 3935 3120 352e 3338  7,-4.615951 5.38
-00001250: 3532 372c 2d38 2e34 3632 3537 3720 392e  527,-8.462577 9.
-00001260: 3233 3139 2c2d 3132 2e36 3933 3836 3620  2319,-12.693866 
-00001270: 352e 3338 3532 372c 2d32 2e36 3932 3633  5.38527,-2.69263
-00001280: 3820 3130 2e37 3730 3535 2c2d 352e 3736  8 10.77055,-5.76
-00001290: 3939 3338 3820 3136 2e31 3535 3833 2c2d  99388 16.15583,-
-000012a0: 372e 3330 3835 3839 3220 4d20 3131 392e  7.3085892 M 119.
-000012b0: 3639 3037 392c 3130 362e 3131 3530 3620  69079,106.11506 
-000012c0: 6320 2d33 2e38 3436 3632 2c33 2e38 3436  c -3.84662,3.846
-000012d0: 3633 202d 362e 3932 3339 322c 392e 3233  63 -6.92392,9.23
-000012e0: 3139 3120 2d37 2e36 3933 3235 2c31 352e  191 -7.69325,15.
-000012f0: 3030 3138 3320 2d30 2e37 3639 3332 2c35  00183 -0.76932,5
-00001300: 2e33 3835 3238 202d 302e 3736 3933 322c  .38528 -0.76932,
-00001310: 3130 2e33 3835 3920 302c 3135 2e37 3731  10.3859 0,15.771
-00001320: 3137 2031 2e35 3338 3635 2c35 2e33 3835  17 1.53865,5.385
-00001330: 3238 2033 2e38 3436 3633 2c31 312e 3135  28 3.84663,11.15
-00001340: 3532 3220 392e 3233 3139 2c31 352e 3030  522 9.2319,15.00
-00001350: 3138 3420 332e 3834 3636 332c 322e 3330  184 3.84663,2.30
-00001360: 3739 3820 382e 3436 3235 382c 332e 3037  798 8.46258,3.07
-00001370: 3733 2031 332e 3436 3331 392c 322e 3330  73 13.46319,2.30
-00001380: 3739 3820 382e 3436 3235 382c 2d31 2e35  798 8.46258,-1.5
-00001390: 3338 3635 2031 352e 3030 3138 352c 2d39  3865 15.00185,-9
-000013a0: 2e32 3331 3920 3135 2e37 3731 3137 2c2d  .2319 15.77117,-
-000013b0: 3138 2e30 3739 3134 2030 2c2d 322e 3330  18.07914 0,-2.30
-000013c0: 3739 3820 2d30 2e37 3639 3332 2c2d 332e  798 -0.76932,-3.
-000013d0: 3834 3636 3320 2d31 2e35 3338 3635 2c2d  84663 -1.53865,-
-000013e0: 362e 3135 3436 3120 2d33 2e30 3737 332c  6.15461 -3.0773,
-000013f0: 2d31 312e 3932 3435 3420 2d36 2e31 3534  -11.92454 -6.154
-00001400: 362c 2d32 332e 3436 3434 202d 392e 3233  6,-23.4644 -9.23
-00001410: 3139 2c2d 3335 2e33 3838 3934 3820 2d38  19,-35.388948 -8
-00001420: 2e30 3737 3932 2c32 2e33 3037 3937 3520  .07792,2.307975 
-00001430: 2d31 342e 3233 3235 322c 362e 3135 3436  -14.23252,6.1546
-00001440: 3038 202d 3230 2e30 3032 3436 2c31 312e  08 -20.00246,11.
-00001450: 3533 3938 3738 207a 220d 0a20 2020 2020  539878 z"..     
-00001460: 2020 6669 6c6c 3d22 2344 4430 3031 4222    fill="#DD001B"
-00001470: 0d0a 2020 2020 2020 2070 2d69 643d 2234  ..       p-id="4
-00001480: 3038 3622 0d0a 2020 2020 2020 2069 643d  086"..       id=
-00001490: 2270 6174 6831 3232 220d 0a20 2020 2020  "path122"..     
-000014a0: 2020 7374 796c 653d 2273 7472 6f6b 652d    style="stroke-
-000014b0: 7769 6474 683a 302e 3234 3034 3134 2220  width:0.240414" 
-000014c0: 2f3e 0d0a 2020 3c2f 673e 0d0a 3c2f 7376  />..  </g>..</sv
-000014d0: 673e 0d0a                                g>..
+00000030: 226e 6f22 3f3e 0a3c 7376 670a 2020 2078  "no"?>.<svg.   x
+00000040: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
+00000050: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
+00000060: 656e 7473 2f31 2e31 2f22 0a20 2020 786d  ents/1.1/".   xm
+00000070: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
+00000080: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
+00000090: 7267 2f6e 7323 220a 2020 2078 6d6c 6e73  rg/ns#".   xmlns
+000000a0: 3a72 6466 3d22 6874 7470 3a2f 2f77 7777  :rdf="http://www
+000000b0: 2e77 332e 6f72 672f 3139 3939 2f30 322f  .w3.org/1999/02/
+000000c0: 3232 2d72 6466 2d73 796e 7461 782d 6e73  22-rdf-syntax-ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7376 673d  #".   xmlns:svg=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f32 3030 302f 7376 6722 0a20 2020  rg/2000/svg".   
+00000100: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00000110: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
+00000120: 6722 0a20 2020 786d 6c6e 733a 736f 6469  g".   xmlns:sodi
+00000130: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
+00000140: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
+00000150: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
+00000160: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
+00000170: 6e73 3a69 6e6b 7363 6170 653d 2268 7474  ns:inkscape="htt
+00000180: 703a 2f2f 7777 772e 696e 6b73 6361 7065  p://www.inkscape
+00000190: 2e6f 7267 2f6e 616d 6573 7061 6365 732f  .org/namespaces/
+000001a0: 696e 6b73 6361 7065 220a 2020 2077 6964  inkscape".   wid
+000001b0: 7468 3d22 3235 362e 3070 7822 0a20 2020  th="256.0px".   
+000001c0: 6865 6967 6874 3d22 3235 362e 3070 7822  height="256.0px"
+000001d0: 0a20 2020 7669 6577 426f 783d 2230 2030  .   viewBox="0 0
+000001e0: 2032 3536 2e30 2032 3536 2e30 220a 2020   256.0 256.0".  
+000001f0: 2076 6572 7369 6f6e 3d22 312e 3122 0a20   version="1.1". 
+00000200: 2020 6964 3d22 5356 4752 6f6f 7422 0a20    id="SVGRoot". 
+00000210: 2020 736f 6469 706f 6469 3a64 6f63 6e61    sodipodi:docna
+00000220: 6d65 3d22 6e65 7465 6173 655f 6963 6f6e  me="netease_icon
+00000230: 2e73 7667 220a 2020 2069 6e6b 7363 6170  .svg".   inkscap
+00000240: 653a 7665 7273 696f 6e3d 2231 2e30 2e31  e:version="1.0.1
+00000250: 2028 3362 6332 6538 3133 6635 2c20 3230   (3bc2e813f5, 20
+00000260: 3230 2d30 392d 3037 2922 3e0a 2020 3c64  20-09-07)">.  <d
+00000270: 6566 730a 2020 2020 2069 643d 2264 6566  efs.     id="def
+00000280: 7331 3022 3e0a 2020 2020 3c73 7479 6c65  s10">.    <style
+00000290: 0a20 2020 2020 2020 7479 7065 3d22 7465  .       type="te
+000002a0: 7874 2f63 7373 220a 2020 2020 2020 2069  xt/css".       i
+000002b0: 643d 2273 7479 6c65 3131 3822 202f 3e0a  d="style118" />.
+000002c0: 2020 3c2f 6465 6673 3e0a 2020 3c73 6f64    </defs>.  <sod
+000002d0: 6970 6f64 693a 6e61 6d65 6476 6965 770a  ipodi:namedview.
+000002e0: 2020 2020 2069 643d 2262 6173 6522 0a20       id="base". 
+000002f0: 2020 2020 7061 6765 636f 6c6f 723d 2223      pagecolor="#
+00000300: 6666 6666 6666 220a 2020 2020 2062 6f72  ffffff".     bor
+00000310: 6465 7263 6f6c 6f72 3d22 2336 3636 3636  dercolor="#66666
+00000320: 3622 0a20 2020 2020 626f 7264 6572 6f70  6".     borderop
+00000330: 6163 6974 793d 2231 2e30 220a 2020 2020  acity="1.0".    
+00000340: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
+00000350: 6163 6974 793d 2230 2e30 220a 2020 2020  acity="0.0".    
+00000360: 2069 6e6b 7363 6170 653a 7061 6765 7368   inkscape:pagesh
+00000370: 6164 6f77 3d22 3222 0a20 2020 2020 696e  adow="2".     in
+00000380: 6b73 6361 7065 3a7a 6f6f 6d3d 2231 2e34  kscape:zoom="1.4
+00000390: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000003a0: 6378 3d22 3232 372e 3232 3237 3422 0a20  cx="227.22274". 
+000003b0: 2020 2020 696e 6b73 6361 7065 3a63 793d      inkscape:cy=
+000003c0: 2231 3036 2e35 220a 2020 2020 2069 6e6b  "106.5".     ink
+000003d0: 7363 6170 653a 646f 6375 6d65 6e74 2d75  scape:document-u
+000003e0: 6e69 7473 3d22 7078 220a 2020 2020 2069  nits="px".     i
+000003f0: 6e6b 7363 6170 653a 6375 7272 656e 742d  nkscape:current-
+00000400: 6c61 7965 723d 226c 6179 6572 3122 0a20  layer="layer1". 
+00000410: 2020 2020 696e 6b73 6361 7065 3a64 6f63      inkscape:doc
+00000420: 756d 656e 742d 726f 7461 7469 6f6e 3d22  ument-rotation="
+00000430: 3022 0a20 2020 2020 7368 6f77 6772 6964  0".     showgrid
+00000440: 3d22 7472 7565 220a 2020 2020 2069 6e6b  ="true".     ink
+00000450: 7363 6170 653a 7769 6e64 6f77 2d77 6964  scape:window-wid
+00000460: 7468 3d22 3134 3538 220a 2020 2020 2069  th="1458".     i
+00000470: 6e6b 7363 6170 653a 7769 6e64 6f77 2d68  nkscape:window-h
+00000480: 6569 6768 743d 2231 3034 3522 0a20 2020  eight="1045".   
+00000490: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
+000004a0: 772d 783d 2233 3633 220a 2020 2020 2069  w-x="363".     i
+000004b0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
+000004c0: 3d22 3130 3122 0a20 2020 2020 696e 6b73  ="101".     inks
+000004d0: 6361 7065 3a77 696e 646f 772d 6d61 7869  cape:window-maxi
+000004e0: 6d69 7a65 643d 2230 223e 0a20 2020 203c  mized="0">.    <
+000004f0: 696e 6b73 6361 7065 3a67 7269 640a 2020  inkscape:grid.  
+00000500: 2020 2020 2074 7970 653d 2278 7967 7269       type="xygri
+00000510: 6422 0a20 2020 2020 2020 6964 3d22 6772  d".       id="gr
+00000520: 6964 3139 2220 2f3e 0a20 203c 2f73 6f64  id19" />.  </sod
+00000530: 6970 6f64 693a 6e61 6d65 6476 6965 773e  ipodi:namedview>
+00000540: 0a20 203c 6d65 7461 6461 7461 0a20 2020  .  <metadata.   
+00000550: 2020 6964 3d22 6d65 7461 6461 7461 3133    id="metadata13
+00000560: 223e 0a20 2020 203c 7264 663a 5244 463e  ">.    <rdf:RDF>
+00000570: 0a20 2020 2020 203c 6363 3a57 6f72 6b0a  .      <cc:Work.
+00000580: 2020 2020 2020 2020 2072 6466 3a61 626f           rdf:abo
+00000590: 7574 3d22 223e 0a20 2020 2020 2020 203c  ut="">.        <
+000005a0: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
+000005b0: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
+000005c0: 6174 3e0a 2020 2020 2020 2020 3c64 633a  at>.        <dc:
+000005d0: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
+000005e0: 7264 663a 7265 736f 7572 6365 3d22 6874  rdf:resource="ht
+000005f0: 7470 3a2f 2f70 7572 6c2e 6f72 672f 6463  tp://purl.org/dc
+00000600: 2f64 636d 6974 7970 652f 5374 696c 6c49  /dcmitype/StillI
+00000610: 6d61 6765 2220 2f3e 0a20 2020 2020 2020  mage" />.       
+00000620: 203c 6463 3a74 6974 6c65 3e3c 2f64 633a   <dc:title></dc:
+00000630: 7469 746c 653e 0a20 2020 2020 203c 2f63  title>.      </c
+00000640: 633a 576f 726b 3e0a 2020 2020 3c2f 7264  c:Work>.    </rd
+00000650: 663a 5244 463e 0a20 203c 2f6d 6574 6164  f:RDF>.  </metad
+00000660: 6174 613e 0a20 203c 670a 2020 2020 2069  ata>.  <g.     i
+00000670: 6e6b 7363 6170 653a 6c61 6265 6c3d 22e5  nkscape:label=".
+00000680: 9bbe e5b1 8220 3122 0a20 2020 2020 696e  ..... 1".     in
+00000690: 6b73 6361 7065 3a67 726f 7570 6d6f 6465  kscape:groupmode
+000006a0: 3d22 6c61 7965 7222 0a20 2020 2020 6964  ="layer".     id
+000006b0: 3d22 6c61 7965 7231 220a 2020 2020 203e  ="layer1".     >
+000006c0: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+000006d0: 2020 643d 226d 2031 3535 2e38 3439 3038    d="m 155.84908
+000006e0: 2c36 2e34 3837 3434 3438 2063 2036 2e39  ,6.4874448 c 6.9
+000006f0: 3233 3932 2c2d 312e 3533 3836 3530 3420  2392,-1.5386504 
+00000700: 3134 2e32 3332 3531 2c2d 312e 3533 3836  14.23251,-1.5386
+00000710: 3530 3420 3230 2e33 3837 3132 2c30 2037  504 20.38712,0 7
+00000720: 2e36 3933 3235 2c31 2e35 3338 3635 3034  .69325,1.5386504
+00000730: 2031 352e 3030 3138 342c 352e 3338 3532   15.00184,5.3852
+00000740: 3736 3220 3231 2e31 3536 3434 2c31 302e  762 21.15644,10.
+00000750: 3338 3538 3930 3220 322e 3330 3739 372c  3858902 2.30797,
+00000760: 312e 3533 3836 3531 2034 2e36 3135 3935  1.538651 4.61595
+00000770: 2c33 2e38 3436 3632 3620 352e 3338 3532  ,3.846626 5.3852
+00000780: 382c 362e 3932 3339 3237 2031 2e39 3233  8,6.923927 1.923
+00000790: 3331 2c33 2e38 3436 3632 3620 312e 3932  31,3.846626 1.92
+000007a0: 3333 312c 382e 3436 3235 3737 202d 312e  331,8.462577 -1.
+000007b0: 3533 3836 362c 3132 2e36 3933 3836 3620  53866,12.693866 
+000007c0: 2d32 2e33 3037 3937 2c33 2e30 3737 3330  -2.30797,3.07730
+000007d0: 3120 2d35 2e33 3835 3237 2c35 2e33 3835  1 -5.38527,5.385
+000007e0: 3237 3720 2d39 2e32 3331 392c 362e 3135  277 -9.2319,6.15
+000007f0: 3436 3032 202d 332e 3037 3733 2c30 2e37  4602 -3.0773,0.7
+00000800: 3639 3332 3520 2d36 2e31 3534 362c 3020  69325 -6.1546,0 
+00000810: 2d39 2e32 3331 392c 2d31 2e35 3338 3635  -9.2319,-1.53865
+00000820: 3120 2d31 2e35 3338 3635 2c2d 302e 3736  1 -1.53865,-0.76
+00000830: 3933 3235 202d 322e 3330 3739 382c 2d32  9325 -2.30798,-2
+00000840: 2e33 3037 3937 3520 2d33 2e38 3436 3633  .307975 -3.84663
+00000850: 2c2d 332e 3037 3733 202d 332e 3834 3636  ,-3.0773 -3.8466
+00000860: 322c 2d32 2e33 3037 3937 3620 2d38 2e34  2,-2.307976 -8.4
+00000870: 3632 3537 2c2d 342e 3631 3539 3532 202d  6257,-4.615952 -
+00000880: 3133 2e34 3633 3139 2c2d 342e 3631 3539  13.46319,-4.6159
+00000890: 3532 202d 332e 3037 3733 2c30 202d 362e  52 -3.0773,0 -6.
+000008a0: 3135 3436 2c32 2e33 3037 3937 3620 2d38  1546,2.307976 -8
+000008b0: 2e34 3632 3537 2c34 2e36 3135 3935 3220  .46257,4.615952 
+000008c0: 2d32 2e33 3037 3938 2c32 2e33 3037 3937  -2.30798,2.30797
+000008d0: 3520 2d33 2e30 3737 3331 2c35 2e33 3835  5 -3.07731,5.385
+000008e0: 3237 3620 2d32 2e33 3037 3938 2c38 2e34  276 -2.30798,8.4
+000008f0: 3632 3537 3720 312e 3533 3836 352c 362e  62577 1.53865,6.
+00000900: 3135 3436 3032 2033 2e30 3737 332c 3132  154602 3.0773,12
+00000910: 2e36 3933 3836 3620 342e 3631 3539 352c  .693866 4.61595,
+00000920: 3138 2e38 3438 3436 3820 3131 2e39 3234  18.848468 11.924
+00000930: 3534 2c30 2e37 3639 3332 3520 3234 2e32  54,0.769325 24.2
+00000940: 3333 3734 2c33 2e38 3436 3632 3620 3334  3374,3.846626 34
+00000950: 2e36 3139 3634 2c31 302e 3338 3538 3920  .61964,10.38589 
+00000960: 3130 2e33 3835 3839 2c36 2e31 3534 3630  10.38589,6.15460
+00000970: 3220 3138 2e38 3438 3436 2c31 342e 3233  2 18.84846,14.23
+00000980: 3235 3136 2032 362e 3534 3137 322c 3233  2516 26.54172,23
+00000990: 2e34 3634 3432 3320 362e 3135 3436 2c37  .464423 6.1546,7
+000009a0: 2e36 3933 3235 3320 3131 2e31 3535 3231  .693253 11.15521
+000009b0: 2c31 372e 3330 3938 3033 2031 332e 3436  ,17.309803 13.46
+000009c0: 3331 392c 3236 2e35 3431 3731 3320 332e  319,26.541713 3.
+000009d0: 3037 3733 2c31 302e 3338 3538 3920 332e  0773,10.38589 3.
+000009e0: 3834 3636 322c 3231 2e31 3536 3434 2033  84662,21.15644 3
+000009f0: 2e30 3737 332c 3332 2e33 3131 3636 202d  .0773,32.31166 -
+00000a00: 302e 3736 3933 332c 382e 3436 3235 3720  0.76933,8.46257 
+00000a10: 2d32 2e33 3037 3938 2c31 382e 3037 3931  -2.30798,18.0791
+00000a20: 3420 2d35 2e33 3835 3238 2c32 352e 3737  4 -5.38528,25.77
+00000a30: 3233 3920 2d37 2e36 3933 3235 2c32 302e  239 -7.69325,20.
+00000a40: 3338 3731 3320 2d32 312e 3932 3537 372c  38713 -21.92577,
+00000a50: 3338 2e34 3636 3237 202d 3430 2e37 3734  38.46627 -40.774
+00000a60: 3234 2c35 302e 3030 3631 3520 2d31 332e  24,50.00615 -13.
+00000a70: 3436 3331 392c 382e 3436 3235 3820 2d32  46319,8.46258 -2
+00000a80: 382e 3834 3936 392c 3134 2e32 3332 3531  8.84969,14.23251
+00000a90: 202d 3435 2e33 3930 3138 2c31 352e 3737   -45.39018,15.77
+00000aa0: 3131 3520 2d31 312e 3135 3532 322c 312e  115 -11.15522,1.
+00000ab0: 3533 3836 3520 2d32 312e 3932 3537 372c  53865 -21.92577,
+00000ac0: 312e 3533 3836 3520 2d33 332e 3038 3039  1.53865 -33.0809
+00000ad0: 392c 2d30 2e37 3639 3333 2043 2038 392e  9,-0.76933 C 89.
+00000ae0: 3638 3731 3038 2c32 3434 2e39 3738 3234  687108,244.97824
+00000af0: 2036 382e 3533 3036 3635 2c32 3333 2e38   68.530665,233.8
+00000b00: 3233 3033 2035 322e 3735 3934 3938 2c32  2303 52.759498,2
+00000b10: 3137 2e32 3832 3534 2033 362e 3938 3833  17.28254 36.9883
+00000b20: 3331 2c32 3031 2e35 3131 3337 2032 352e  31,201.51137 25.
+00000b30: 3434 3834 3533 2c31 3830 2e33 3534 3934  448453,180.35494
+00000b40: 2032 312e 3231 3731 3634 2c31 3538 2e34   21.217164,158.4
+00000b50: 3239 3137 2031 372e 3735 3532 3031 2c31  2917 17.755201,1
+00000b60: 3432 2e32 3733 3334 2031 372e 3735 3532  42.27334 17.7552
+00000b70: 3031 2c31 3235 2e37 3332 3835 2032 312e  01,125.73285 21.
+00000b80: 3938 3634 3839 2c31 3039 2e31 3932 3336  986489,109.19236
+00000b90: 2032 362e 3630 3234 3431 2c38 392e 3537   26.602441,89.57
+00000ba0: 3435 3638 2033 362e 3231 3930 3036 2c37  4568 36.219006,7
+00000bb0: 302e 3732 3631 2035 302e 3036 3638 362c  0.7261 50.06686,
+00000bc0: 3535 2e37 3234 3235 3820 3631 2e39 3931  55.724258 61.991
+00000bd0: 342c 3433 2e37 3939 3731 3820 3735 2e30  4,43.799718 75.0
+00000be0: 3639 3932 392c 3333 2e37 3938 3439 2039  69929,33.79849 9
+00000bf0: 302e 3834 3130 3936 2c32 372e 3634 3338  0.841096,27.6438
+00000c00: 3838 2063 2031 2e35 3338 3635 2c2d 302e  88 c 1.53865,-0.
+00000c10: 3736 3933 3235 2033 2e30 3737 3330 312c  769325 3.077301,
+00000c20: 2d31 2e35 3338 3635 2034 2e36 3135 3935  -1.53865 4.61595
+00000c30: 312c 2d31 2e35 3338 3635 2033 2e38 3436  1,-1.53865 3.846
+00000c40: 3632 362c 2d30 2e37 3639 3332 3520 372e  626,-0.769325 7.
+00000c50: 3639 3332 3533 2c30 2031 302e 3338 3538  693253,0 10.3858
+00000c60: 3933 2c32 2e33 3037 3937 3520 332e 3834  93,2.307975 3.84
+00000c70: 3636 332c 332e 3037 3733 3031 2036 2e31  663,3.077301 6.1
+00000c80: 3534 362c 372e 3639 3332 3532 2035 2e33  546,7.693252 5.3
+00000c90: 3835 3238 2c31 322e 3639 3338 3636 202d  8528,12.693866 -
+00000ca0: 302e 3736 3933 332c 342e 3631 3539 3532  0.76933,4.615952
+00000cb0: 202d 332e 3834 3636 332c 392e 3233 3139   -3.84663,9.2319
+00000cc0: 3033 202d 382e 3436 3235 382c 3131 2e31  03 -8.46258,11.1
+00000cd0: 3535 3231 3620 2d31 352e 3737 3131 372c  55216 -15.77117,
+00000ce0: 352e 3338 3532 3736 202d 3239 2e36 3139  5.385276 -29.619
+00000cf0: 3032 342c 3136 2e35 3430 3439 3220 2d33  024,16.540492 -3
+00000d00: 392e 3233 3535 3839 2c32 392e 3631 3930  9.235589,29.6190
+00000d10: 3231 202d 382e 3436 3235 3737 2c31 312e  21 -8.462577,11.
+00000d20: 3932 3435 3420 2d31 352e 3030 3138 3432  92454 -15.001842
+00000d30: 2c32 352e 3737 3233 3934 202d 3136 2e35  ,25.772394 -16.5
+00000d40: 3430 3439 322c 3430 2e37 3734 3233 3420  40492,40.774234 
+00000d50: 2d32 2e33 3037 3937 362c 3135 2e30 3031  -2.307976,15.001
+00000d60: 3834 2030 2c32 392e 3631 3930 3220 342e  84 0,29.61902 4.
+00000d70: 3631 3539 3531 2c34 332e 3038 3232 3120  615951,43.08221 
+00000d80: 372e 3639 3332 3532 2c32 302e 3338 3731  7.693252,20.3871
+00000d90: 3220 3232 2e36 3935 3039 342c 3337 2e36  2 22.695094,37.6
+00000da0: 3936 3932 2034 312e 3534 3335 3632 2c34  9692 41.543562,4
+00000db0: 362e 3932 3838 3420 3131 2e39 3234 3533  6.92884 11.92453
+00000dc0: 382c 362e 3135 3435 3920 3234 2e32 3333  8,6.15459 24.233
+00000dd0: 3734 382c 392e 3233 3139 3120 3337 2e36  748,9.23191 37.6
+00000de0: 3936 3933 382c 382e 3436 3235 3820 3131  96938,8.46258 11
+00000df0: 2e31 3535 3231 2c30 2032 312e 3135 3634  .15521,0 21.1564
+00000e00: 342c 2d31 2e35 3338 3635 2033 312e 3534  4,-1.53865 31.54
+00000e10: 3233 332c 2d35 2e33 3835 3237 2038 2e34  233,-5.38527 8.4
+00000e20: 3632 3538 2c2d 332e 3037 3733 3120 3137  6258,-3.07731 17
+00000e30: 2e33 3039 3832 2c2d 372e 3639 3332 3620  .30982,-7.69326 
+00000e40: 3234 2e32 3333 3735 2c2d 3134 2e32 3332  24.23375,-14.232
+00000e50: 3534 2036 2e31 3534 362c 2d35 2e33 3835  54 6.1546,-5.385
+00000e60: 3238 2031 312e 3932 3435 342c 2d31 322e  28 11.92454,-12.
+00000e70: 3639 3338 3620 3136 2e35 3430 3439 2c2d  69386 16.54049,-
+00000e80: 3230 2e33 3837 3131 2032 2e33 3037 3937  20.38711 2.30797
+00000e90: 2c2d 332e 3834 3636 3220 332e 3834 3636  ,-3.84662 3.8466
+00000ea0: 322c 2d37 2e36 3933 3235 2035 2e33 3835  2,-7.69325 5.385
+00000eb0: 3237 2c2d 3132 2e36 3933 3836 2033 2e30  27,-12.69386 3.0
+00000ec0: 3737 3331 2c2d 3132 2e36 3933 3837 2033  7731,-12.69387 3
+00000ed0: 2e38 3436 3633 2c2d 3235 2e37 3732 3420  .84663,-25.7724 
+00000ee0: 302c 2d33 372e 3639 3639 3420 2d33 2e38  0,-37.69694 -3.8
+00000ef0: 3436 3632 2c2d 382e 3436 3235 3820 2d31  4662,-8.46258 -1
+00000f00: 302e 3338 3538 392c 2d31 382e 3037 3931  0.38589,-18.0791
+00000f10: 3320 2d31 382e 3037 3931 342c 2d32 352e  3 -18.07914,-25.
+00000f20: 3030 3330 3620 2d33 2e38 3436 3632 2c2d  00306 -3.84662,-
+00000f30: 332e 3037 3733 202d 362e 3932 3339 332c  3.0773 -6.92393,
+00000f40: 2d36 2e31 3534 3630 3320 2d31 312e 3932  -6.154603 -11.92
+00000f50: 3435 342c 2d38 2e34 3632 3538 202d 332e  454,-8.46258 -3.
+00000f60: 3834 3636 322c 2d32 2e33 3037 3937 3620  84662,-2.307976 
+00000f70: 2d37 2e36 3933 3235 2c2d 332e 3037 3733  -7.69325,-3.0773
+00000f80: 3031 202d 3131 2e39 3234 3534 2c2d 342e  01 -11.92454,-4.
+00000f90: 3631 3539 3531 2033 2e30 3737 332c 3131  615951 3.0773,11
+00000fa0: 2e31 3535 3232 3120 352e 3338 3532 382c  .155221 5.38528,
+00000fb0: 3231 2e39 3235 3737 3120 382e 3436 3235  21.925771 8.4625
+00000fc0: 382c 3333 2e30 3830 3938 3120 302e 3736  8,33.080981 0.76
+00000fd0: 3933 322c 322e 3330 3739 3720 302e 3736  932,2.30797 0.76
+00000fe0: 3933 322c 352e 3338 3532 3720 312e 3533  932,5.38527 1.53
+00000ff0: 3836 352c 372e 3639 3332 3520 302e 3736  865,7.69325 0.76
+00001000: 3933 322c 3131 2e31 3535 3231 202d 332e  932,11.15521 -3.
+00001010: 3834 3636 332c 3232 2e36 3935 3039 202d  84663,22.69509 -
+00001020: 3131 2e31 3535 3232 2c33 312e 3534 3233  11.15522,31.5423
+00001030: 3320 2d36 2e39 3233 3932 2c37 2e36 3933  3 -6.92392,7.693
+00001040: 3235 202d 3136 2e35 3430 3439 2c31 342e  25 -16.54049,14.
+00001050: 3233 3235 3220 2d32 362e 3534 3137 322c  23252 -26.54172,
+00001060: 3135 2e37 3731 3137 202d 3131 2e31 3535  15.77117 -11.155
+00001070: 3231 2c32 2e33 3037 3937 202d 3233 2e34  21,2.30797 -23.4
+00001080: 3634 3432 2c30 202d 3333 2e30 3830 3938  6442,0 -33.08098
+00001090: 2c2d 362e 3135 3436 202d 392e 3233 3139  ,-6.1546 -9.2319
+000010a0: 3035 2c2d 352e 3338 3532 3820 2d31 352e  05,-5.38528 -15.
+000010b0: 3737 3131 3639 2c2d 3135 2e30 3031 3834  771169,-15.00184
+000010c0: 202d 3139 2e36 3137 3739 352c 2d32 352e   -19.617795,-25.
+000010d0: 3030 3330 3720 2d32 2e33 3037 3937 362c  00307 -2.307976,
+000010e0: 2d35 2e33 3835 3238 202d 332e 3037 3733  -5.38528 -3.0773
+000010f0: 3031 2c2d 3131 2e39 3234 3534 202d 332e  01,-11.92454 -3.
+00001100: 3037 3733 3031 2c2d 3138 2e30 3739 3134  077301,-18.07914
+00001110: 202d 302e 3736 3933 3235 2c2d 3133 2e34   -0.769325,-13.4
+00001120: 3633 3220 332e 3037 3733 3031 2c2d 3236  632 3.077301,-26
+00001130: 2e35 3431 3731 2031 302e 3338 3538 392c  .54171 10.38589,
+00001140: 2d33 372e 3639 3639 3334 2038 2e34 3632  -37.696934 8.462
+00001150: 3537 362c 2d31 332e 3436 3331 3931 2032  576,-13.463191 2
+00001160: 322e 3639 3530 3936 2c2d 3231 2e39 3235  2.695096,-21.925
+00001170: 3736 3820 3337 2e36 3936 3933 362c 2d32  768 37.696936,-2
+00001180: 362e 3534 3137 3139 202d 302e 3736 3933  6.541719 -0.7693
+00001190: 322c 2d33 2e38 3436 3632 3620 2d32 2e33  2,-3.846626 -2.3
+000011a0: 3037 3938 2c2d 382e 3436 3235 3738 202d  0798,-8.462578 -
+000011b0: 332e 3037 3733 2c2d 3132 2e36 3933 3836  3.0773,-12.69386
+000011c0: 3620 2d33 2e30 3737 332c 2d39 2e32 3331  6 -3.0773,-9.231
+000011d0: 3930 3320 2d32 2e33 3037 3938 2c2d 3139  903 -2.30798,-19
+000011e0: 2e36 3137 3739 3320 322e 3330 3739 382c  .617793 2.30798,
+000011f0: 2d32 382e 3038 3033 3731 2032 2e33 3037  -28.080371 2.307
+00001200: 3937 2c2d 342e 3631 3539 3531 2035 2e33  97,-4.615951 5.3
+00001210: 3835 3237 2c2d 382e 3436 3235 3737 2039  8527,-8.462577 9
+00001220: 2e32 3331 392c 2d31 322e 3639 3338 3636  .2319,-12.693866
+00001230: 2035 2e33 3835 3237 2c2d 322e 3639 3236   5.38527,-2.6926
+00001240: 3338 2031 302e 3737 3035 352c 2d35 2e37  38 10.77055,-5.7
+00001250: 3639 3933 3838 2031 362e 3135 3538 332c  699388 16.15583,
+00001260: 2d37 2e33 3038 3538 3932 204d 2031 3139  -7.3085892 M 119
+00001270: 2e36 3930 3739 2c31 3036 2e31 3135 3036  .69079,106.11506
+00001280: 2063 202d 332e 3834 3636 322c 332e 3834   c -3.84662,3.84
+00001290: 3636 3320 2d36 2e39 3233 3932 2c39 2e32  663 -6.92392,9.2
+000012a0: 3331 3931 202d 372e 3639 3332 352c 3135  3191 -7.69325,15
+000012b0: 2e30 3031 3833 202d 302e 3736 3933 322c  .00183 -0.76932,
+000012c0: 352e 3338 3532 3820 2d30 2e37 3639 3332  5.38528 -0.76932
+000012d0: 2c31 302e 3338 3539 2030 2c31 352e 3737  ,10.3859 0,15.77
+000012e0: 3131 3720 312e 3533 3836 352c 352e 3338  117 1.53865,5.38
+000012f0: 3532 3820 332e 3834 3636 332c 3131 2e31  528 3.84663,11.1
+00001300: 3535 3232 2039 2e32 3331 392c 3135 2e30  5522 9.2319,15.0
+00001310: 3031 3834 2033 2e38 3436 3633 2c32 2e33  0184 3.84663,2.3
+00001320: 3037 3938 2038 2e34 3632 3538 2c33 2e30  0798 8.46258,3.0
+00001330: 3737 3320 3133 2e34 3633 3139 2c32 2e33  773 13.46319,2.3
+00001340: 3037 3938 2038 2e34 3632 3538 2c2d 312e  0798 8.46258,-1.
+00001350: 3533 3836 3520 3135 2e30 3031 3835 2c2d  53865 15.00185,-
+00001360: 392e 3233 3139 2031 352e 3737 3131 372c  9.2319 15.77117,
+00001370: 2d31 382e 3037 3931 3420 302c 2d32 2e33  -18.07914 0,-2.3
+00001380: 3037 3938 202d 302e 3736 3933 322c 2d33  0798 -0.76932,-3
+00001390: 2e38 3436 3633 202d 312e 3533 3836 352c  .84663 -1.53865,
+000013a0: 2d36 2e31 3534 3631 202d 332e 3037 3733  -6.15461 -3.0773
+000013b0: 2c2d 3131 2e39 3234 3534 202d 362e 3135  ,-11.92454 -6.15
+000013c0: 3436 2c2d 3233 2e34 3634 3420 2d39 2e32  46,-23.4644 -9.2
+000013d0: 3331 392c 2d33 352e 3338 3839 3438 202d  319,-35.388948 -
+000013e0: 382e 3037 3739 322c 322e 3330 3739 3735  8.07792,2.307975
+000013f0: 202d 3134 2e32 3332 3532 2c36 2e31 3534   -14.23252,6.154
+00001400: 3630 3820 2d32 302e 3030 3234 362c 3131  608 -20.00246,11
+00001410: 2e35 3339 3837 3820 7a22 0a20 2020 2020  .539878 z".     
+00001420: 2020 6669 6c6c 3d22 2344 4430 3031 4222    fill="#DD001B"
+00001430: 0a20 2020 2020 2020 702d 6964 3d22 3430  .       p-id="40
+00001440: 3836 220a 2020 2020 2020 2069 643d 2270  86".       id="p
+00001450: 6174 6831 3232 220a 2020 2020 2020 2073  ath122".       s
+00001460: 7479 6c65 3d22 7374 726f 6b65 2d77 6964  tyle="stroke-wid
+00001470: 7468 3a30 2e32 3430 3431 3422 202f 3e0a  th:0.240414" />.
+00001480: 2020 3c2f 673e 0a3c 2f73 7667 3e0a         </g>.</svg>.
```

### Comparing `fuo_netease-0.9.4/fuo_netease/cloud_helpers/__init__.py` & `fuo_netease-0.9.5/fuo_netease/cloud_helpers/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-# 核心代码均借鉴于 https://github.com/greats3an/pyncm
-import random
-from hashlib import md5
-
-BASE62 = "PJArHa0dpwhvMNYqKnTbitWfEmosQ9527ZBx46IXUgOzD81VuSFyckLRljG3eC"
-BASE64 = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
-
-
-def RandomString(len, chars=BASE62):
-    # Generates random string of `len` chars within a selected number of chars
-    return "".join([random.choice(chars) for i in range(0, len)])
-
-
-def HexDigest(data: bytearray):
-    # Digests a `bytearray` to a hex string
-    return "".join([hex(d)[2:].zfill(2) for d in data])
-
-
-def HexCompose(hexstr: str):
-    # Composes a hex string back to a `bytearray`
-    return bytearray(
-        [int(hexstr[i : i + 2], 16) for i in range(0, len(hexstr), 2)]
-    )
-
-
-def HashDigest(text):
-    # Digests 128 bit md5 hash
-    HASH = md5(text.encode("utf-8"))
-    return HASH.digest()
-
-
-def HashHexDigest(text):
-    """Digests 128 bit md5 hash,then digest it as a hexstring"""
-    return HexDigest(HashDigest(text))
+# -*- coding: utf-8 -*-
+# 核心代码均借鉴于 https://github.com/greats3an/pyncm
+import random
+from hashlib import md5
+
+BASE62 = "PJArHa0dpwhvMNYqKnTbitWfEmosQ9527ZBx46IXUgOzD81VuSFyckLRljG3eC"
+BASE64 = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
+
+
+def RandomString(len, chars=BASE62):
+    # Generates random string of `len` chars within a selected number of chars
+    return "".join([random.choice(chars) for i in range(0, len)])
+
+
+def HexDigest(data: bytearray):
+    # Digests a `bytearray` to a hex string
+    return "".join([hex(d)[2:].zfill(2) for d in data])
+
+
+def HexCompose(hexstr: str):
+    # Composes a hex string back to a `bytearray`
+    return bytearray(
+        [int(hexstr[i : i + 2], 16) for i in range(0, len(hexstr), 2)]
+    )
+
+
+def HashDigest(text):
+    # Digests 128 bit md5 hash
+    HASH = md5(text.encode("utf-8"))
+    return HASH.digest()
+
+
+def HashHexDigest(text):
+    """Digests 128 bit md5 hash,then digest it as a hexstring"""
+    return HexDigest(HashDigest(text))
```

### Comparing `fuo_netease-0.9.4/fuo_netease/downloader.py` & `fuo_netease-0.9.5/fuo_netease/downloader.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import asyncio
-from functools import partial
-import logging
-import os
-
-from PyQt5.QtCore import QObject, pyqtSignal
-
-from feeluown.consts import SONG_DIR
-from feeluown.utils import emit_requests_progress
-
-
-logger = logging.getLogger(__name__)
-
-
-class Downloader(QObject):
-    download_progress_signal = pyqtSignal([int])
-
-    def __init__(self, app, parent=None):
-        super().__init__(parent)
-        self._app = app
-
-        self.is_downloading = False
-        self.current_song = None
-        self.queue = []
-
-    def _access_queue(self):
-        if self.queue:
-            song = self.queue.pop(0)
-            self.download_song(song)
-        else:
-            self._app.message('下载队列下载完毕')
-
-    def download_song(self, song):
-        for s in self.queue:
-            if s.mid == song.mid:
-                self._app.message('%s 已经在下载队列中' % song.title)
-                self._app.message('当前正在下载 %s' % self.current_song.title)
-                return
-
-        if self.is_downloading:
-            if len(self.queue) > 10:
-                self._app.message('下载队列已满，请稍后加入', error=True)
-                return
-            self.queue.append(song)
-            self._app.message('%s 加入下载队列之中' % song.title)
-            return
-
-        self.is_downloading = True
-        event_loop = asyncio.get_event_loop()
-        event_loop.create_task(self._download(song))
-
-    @asyncio.coroutine
-    def _download(self, song):
-        f_name = song.filename
-        f_path = os.path.join(SONG_DIR, f_name)
-        if os.path.exists(f_path):
-            logger.warning('%s have been downloaded' % song.title)
-            self._app.message('%s 这首歌已经存在' % song.title)
-            self.is_downloading = False
-            self._access_queue()
-            return True
-        self.current_song = song
-        if song.url is not None:
-            try:
-                event_loop = asyncio.get_event_loop()
-                self._app.message('准备下载 %s' % song.title)
-                res = song._api.http.get(song.url, stream=True, timeout=30)
-                if res.status_code != 200:
-                    raise Exception('response not ok while download song')
-                future = event_loop.run_in_executor(
-                    None,
-                    partial(emit_requests_progress, res,
-                            self.download_progress_signal))
-                content = yield from future
-                if not content:
-                    raise Exception('error in downloaded song')
-                with open(f_path, 'wb') as f:
-                    f.write(content)
-                logger.info('download song %s successfully' % song.title)
-                self._app.message('%s 下载成功' % song.title)
-                self.is_downloading = False
-                self._access_queue()
-                return True
-            except Exception as e:
-                logger.error(e)
-
-        self._app.message('下载 %s 失败' % song.title, error=True)
-        self.is_downloading = False
-        self._access_queue()
-        return False
+import asyncio
+from functools import partial
+import logging
+import os
+
+from PyQt5.QtCore import QObject, pyqtSignal
+
+from feeluown.consts import SONG_DIR
+from feeluown.utils import emit_requests_progress
+
+
+logger = logging.getLogger(__name__)
+
+
+class Downloader(QObject):
+    download_progress_signal = pyqtSignal([int])
+
+    def __init__(self, app, parent=None):
+        super().__init__(parent)
+        self._app = app
+
+        self.is_downloading = False
+        self.current_song = None
+        self.queue = []
+
+    def _access_queue(self):
+        if self.queue:
+            song = self.queue.pop(0)
+            self.download_song(song)
+        else:
+            self._app.message('下载队列下载完毕')
+
+    def download_song(self, song):
+        for s in self.queue:
+            if s.mid == song.mid:
+                self._app.message('%s 已经在下载队列中' % song.title)
+                self._app.message('当前正在下载 %s' % self.current_song.title)
+                return
+
+        if self.is_downloading:
+            if len(self.queue) > 10:
+                self._app.message('下载队列已满，请稍后加入', error=True)
+                return
+            self.queue.append(song)
+            self._app.message('%s 加入下载队列之中' % song.title)
+            return
+
+        self.is_downloading = True
+        event_loop = asyncio.get_event_loop()
+        event_loop.create_task(self._download(song))
+
+    @asyncio.coroutine
+    def _download(self, song):
+        f_name = song.filename
+        f_path = os.path.join(SONG_DIR, f_name)
+        if os.path.exists(f_path):
+            logger.warning('%s have been downloaded' % song.title)
+            self._app.message('%s 这首歌已经存在' % song.title)
+            self.is_downloading = False
+            self._access_queue()
+            return True
+        self.current_song = song
+        if song.url is not None:
+            try:
+                event_loop = asyncio.get_event_loop()
+                self._app.message('准备下载 %s' % song.title)
+                res = song._api.http.get(song.url, stream=True, timeout=30)
+                if res.status_code != 200:
+                    raise Exception('response not ok while download song')
+                future = event_loop.run_in_executor(
+                    None,
+                    partial(emit_requests_progress, res,
+                            self.download_progress_signal))
+                content = yield from future
+                if not content:
+                    raise Exception('error in downloaded song')
+                with open(f_path, 'wb') as f:
+                    f.write(content)
+                logger.info('download song %s successfully' % song.title)
+                self._app.message('%s 下载成功' % song.title)
+                self.is_downloading = False
+                self._access_queue()
+                return True
+            except Exception as e:
+                logger.error(e)
+
+        self._app.message('下载 %s 失败' % song.title, error=True)
+        self.is_downloading = False
+        self._access_queue()
+        return False
```

### Comparing `fuo_netease-0.9.4/fuo_netease/login_controller.py` & `fuo_netease-0.9.5/fuo_netease/login_controller.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import json
-import logging
-import os
-
-from .api import api
-from .schemas import NeteaseUserSchema
-from .models import _deserialize
-from .consts import USERS_INFO_FILE
-
-logger = logging.getLogger(__name__)
-
-
-def create_user(identifier, name, cookies):
-    user = _deserialize(dict(
-        id=int(identifier),
-        name=name,
-        cookies=cookies,
-    ), NeteaseUserSchema)
-    return user
-
-
-class LoginController(object):
-    _api = api
-
-    def __init__(self, username, uid, name, img):
-        super().__init__()
-        self.username = username
-        self.uid = uid
-        self.name = name
-
-    @classmethod
-    def create(cls, data):
-        user_data = data['data']
-        # img = user_data['profile']['avatarUrl']
-        uid = user_data['profile']['userId']
-        name = user_data['profile']['nickname']
-        user = create_user(uid, name, cls._api.cookies)
-        return user
-
-    @classmethod
-    def check(cls, country_code, username, pw):
-        data = cls._api.login(country_code, username, pw)
-        if data is None:
-            return {'code': 408, 'message': '网络状况不好'}
-        elif data['code'] == 200:
-            if data.get("profile") is None:
-                return {'code': 302, 'message': '请先在网页版绑定手机'}
-            return {'code': 200, 'message': '登陆成功',
-                    'data': data, 'username': username}
-        elif data['code'] == 415:
-            captcha_id = data['captchaId']
-            url = cls._api.get_captcha_url(captcha_id)
-            return {'code': 415, 'message': '本次登陆需要验证码',
-                    'captcha_url': url, 'captchar_id': captcha_id}
-        elif data['code'] == 501:
-            return {'code': 501, 'message': '用户名不存在'}
-        elif data['code'] == 502:
-            return {'code': 502, 'message': '密码错误'}
-        elif data['code'] == 509:
-            return {'code': 509, 'message': '请休息几分钟再尝试'}
-        else:
-            return {'code': data['code'], 'message': data['message']}
-
-    @classmethod
-    def check_captcha(cls, captcha_id, text):
-        flag, cid = cls._api.confirm_captcha(captcha_id, text)
-        if flag is not True:
-            url = cls._api.get_captcha_url(cid)
-            return {'code': 415, 'message': '验证码错误',
-                    'captcha_url': url, 'captcha_id': cid}
-        return {'code': 200, 'message': '验证码正确'}
-
-    @classmethod
-    def save(cls, user):
-        with open(USERS_INFO_FILE, 'w+') as f:
-            data = {
-                user.name: {
-                    'uid': user.identifier,
-                    'name': user.name,
-                    'cookies': user.cookies
-                }
-            }
-            if f.read() != '':
-                data.update(json.load(f))
-            json.dump(data, f, indent=4)
-
-    @classmethod
-    def load(cls):
-        if not os.path.exists(USERS_INFO_FILE):
-            return None
-        with open(USERS_INFO_FILE, 'r') as f:
-            text = f.read()
-            if text == '':
-                return None
-            data = json.loads(text)
-            username = next(iter(data.keys()))
-            user_data = data[username]
-            uid = user_data['uid']
-            name = user_data['name']
-            cookies = user_data.get('cookies', cls._api.cookies)
-            user = create_user(uid, name, cookies)
-        return user
+import json
+import logging
+import os
+
+from .api import api
+from .schemas import NeteaseUserSchema
+from .models import _deserialize
+from .consts import USERS_INFO_FILE
+
+logger = logging.getLogger(__name__)
+
+
+def create_user(identifier, name, cookies):
+    user = _deserialize(dict(
+        id=int(identifier),
+        name=name,
+        cookies=cookies,
+    ), NeteaseUserSchema)
+    return user
+
+
+class LoginController(object):
+    _api = api
+
+    def __init__(self, username, uid, name, img):
+        super().__init__()
+        self.username = username
+        self.uid = uid
+        self.name = name
+
+    @classmethod
+    def create(cls, data):
+        user_data = data['data']
+        # img = user_data['profile']['avatarUrl']
+        uid = user_data['profile']['userId']
+        name = user_data['profile']['nickname']
+        user = create_user(uid, name, cls._api.cookies)
+        return user
+
+    @classmethod
+    def check(cls, country_code, username, pw):
+        data = cls._api.login(country_code, username, pw)
+        if data is None:
+            return {'code': 408, 'message': '网络状况不好'}
+        elif data['code'] == 200:
+            if data.get("profile") is None:
+                return {'code': 302, 'message': '请先在网页版绑定手机'}
+            return {'code': 200, 'message': '登陆成功',
+                    'data': data, 'username': username}
+        elif data['code'] == 415:
+            captcha_id = data['captchaId']
+            url = cls._api.get_captcha_url(captcha_id)
+            return {'code': 415, 'message': '本次登陆需要验证码',
+                    'captcha_url': url, 'captchar_id': captcha_id}
+        elif data['code'] == 501:
+            return {'code': 501, 'message': '用户名不存在'}
+        elif data['code'] == 502:
+            return {'code': 502, 'message': '密码错误'}
+        elif data['code'] == 509:
+            return {'code': 509, 'message': '请休息几分钟再尝试'}
+        else:
+            return {'code': data['code'], 'message': data['message']}
+
+    @classmethod
+    def check_captcha(cls, captcha_id, text):
+        flag, cid = cls._api.confirm_captcha(captcha_id, text)
+        if flag is not True:
+            url = cls._api.get_captcha_url(cid)
+            return {'code': 415, 'message': '验证码错误',
+                    'captcha_url': url, 'captcha_id': cid}
+        return {'code': 200, 'message': '验证码正确'}
+
+    @classmethod
+    def save(cls, user):
+        with open(USERS_INFO_FILE, 'w+') as f:
+            data = {
+                user.name: {
+                    'uid': user.identifier,
+                    'name': user.name,
+                    'cookies': user.cookies
+                }
+            }
+            if f.read() != '':
+                data.update(json.load(f))
+            json.dump(data, f, indent=4)
+
+    @classmethod
+    def load(cls):
+        if not os.path.exists(USERS_INFO_FILE):
+            return None
+        with open(USERS_INFO_FILE, 'r') as f:
+            text = f.read()
+            if text == '':
+                return None
+            data = json.loads(text)
+            username = next(iter(data.keys()))
+            user_data = data[username]
+            uid = user_data['uid']
+            name = user_data['name']
+            cookies = user_data.get('cookies', cls._api.cookies)
+            user = create_user(uid, name, cookies)
+        return user
```

### Comparing `fuo_netease-0.9.4/fuo_netease/models.py` & `fuo_netease-0.9.5/fuo_netease/models.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-import logging
-
-from marshmallow.exceptions import ValidationError
-
-from feeluown.models import (
-    cached_field,
-    BaseModel,
-    PlaylistModel,
-    UserModel,
-    SearchModel,
-)
-from feeluown.utils.reader import RandomSequentialReader, SequentialReader
-
-from .provider import provider
-from .excs import NeteaseIOError
-
-logger = logging.getLogger(__name__)
-
-
-def _deserialize(data, schema_cls):
-    schema = schema_cls()
-    obj = schema.load(data)
-    return obj
-
-
-def create_g(func, schema=None, data_field=None):
-    data = func(limit=0)
-    if data is None:
-        raise NeteaseIOError('server responses with error status code')
-    if data_field is None:
-        data_field = 'data'
-
-    count = int(data['count'])
-
-    def read_func(start, end):
-        data = func(start, end - start)
-        return [_deserialize(data, schema)
-                for data in data[data_field]]
-
-    reader = RandomSequentialReader(count,
-                                    read_func=read_func,
-                                    max_per_read=200)
-    return reader
-
-
-def create_cloud_songs_g(func, func_extra, schema=None, schema_extra=None,
-                         data_field=None, data_key=None):
-    data = func(limit=0)
-    if data is None:
-        raise NeteaseIOError('server responses with error status code')
-    if data_field is None:
-        data_field = 'data'
-
-    count = int(data['count'])
-
-    def read_func(start, end):
-        songs_data = func(start, end - start)
-
-        songs = []
-        extra_songs_info = []
-        for idx, song_data in enumerate(songs_data[data_field]):
-            if data_key:
-                song_data = song_data[data_key]
-            try:
-                song = _deserialize(song_data, schema)
-            except ValidationError:
-                # FIXME: 有些云盘歌曲在 netease 上不存在，这时不能把它们转换成
-                # SongModel。因为 SongModel 的逻辑没有考虑 song 不存在的情况。
-                # 这类歌曲往往没有 ar/al 等字段，在反序列化的时候会报 ValidationError，
-                # 所以这里如果检测到 ValidationError，就跳过这首歌曲。
-                #
-                # 可能的修复方法：
-                # 1. 在 SongModel 上加一个 flag 来标识该歌曲是否为云盘歌曲，
-                #    如果是的话，则使用 cloud_song_detail 接口来获取相关信息。
-                # name = song_data['name']
-                # logger.warn(f'cloud song:{name} may not exist on netease, skip it.')
-                extra_songs_info.append((idx, song_data['id']))
-                # song_data = func_extra(str(song_data['id']))[data_field][0]
-                # song = _deserialize(song_data, schema_extra)
-            else:
-                songs.append(song)
-
-        if extra_songs_info:
-            extra_song_ids = ','.join([str(id) for (_, id) in extra_songs_info])
-            extra_songs_data = func_extra(extra_song_ids)
-            for idx, song_data in enumerate(extra_songs_data[data_field]):
-                song = _deserialize(song_data, schema_extra)
-                songs.insert(extra_songs_info[idx][0], song)
-
-        return songs
-
-    reader = RandomSequentialReader(count,
-                                    read_func=read_func,
-                                    max_per_read=200)
-    return reader
-
-
-class NBaseModel(BaseModel):
-    # FIXME: remove _detail_fields and _api to Meta
-    _api = provider.api
-
-    class Meta:
-        allow_get = True
-        provider = provider
-
-
-class NRadioModel(PlaylistModel, NBaseModel):
-    class Meta:
-        allow_create_songs_g = True
-
-    def create_songs_g(self):
-        data = self._api.djradio_list(self.identifier, limit=1, offset=0)
-        count = data.get('count', 0)
-
-        def g():
-            offset = 0
-            per = 50  # speed up first request
-            while offset < count:
-                tracks_data = self._api.djradio_list(
-                    self.identifier, limit=per, offset=offset)
-                for track_data in tracks_data.get('programs', []):
-                    yield _deserialize(track_data, NDjradioSchema)
-                offset += per
-
-        return SequentialReader(g(), count)
-
-    @classmethod
-    def get(cls, identifier):
-        data = cls._api.djradio_detail(identifier)
-        radio = _deserialize(data, NDjradioSchema)
-        return radio
-
-
-class NSearchModel(SearchModel, NBaseModel):
-    pass
-
-
-class NUserModel(UserModel, NBaseModel):
-    class Meta:
-        fields = ('cookies',)
-        fields_no_get = ('cookies', 'rec_songs', 'rec_playlists',
-                         'fav_artists', 'fav_albums', )
-
-    @classmethod
-    def get(cls, identifier):
-        user = {'id': identifier}
-        user_profile = cls._api.user_profile(identifier)
-        user['name'] = user_profile['nickname']
-        playlists = cls._api.user_playlists(identifier)
-
-        user['playlists'] = []
-        user['fav_playlists'] = []
-        for pl in playlists:
-            if str(pl['userId']) == str(identifier):
-                user['playlists'].append(pl)
-            else:
-                user['fav_playlists'].append(pl)
-        # FIXME: GUI模式下无法显示歌单描述
-        user = _deserialize(user, NeteaseUserSchema)
-        return user
-
-    @cached_field()
-    def rec_playlists(self):
-        playlists_data = self._api.get_recommend_playlists()
-        rec_playlists = []
-        for playlist_data in playlists_data:
-            # FIXME: GUI模式下无法显示歌单描述
-            playlist_data['coverImgUrl'] = playlist_data['picUrl']
-            playlist_data['description'] = None
-            playlist = _deserialize(playlist_data, V2PlaylistSchema)
-            rec_playlists.append(playlist)
-        return rec_playlists
-
-    @property
-    def fav_djradio(self):
-        return create_g(self._api.subscribed_djradio, NeteaseDjradioSchema, 'djRadios')
-
-    @fav_djradio.setter
-    def fav_djradio(self, _):
-        pass
-
-    @property
-    def fav_artists(self):
-        return create_g(self._api.user_favorite_artists, V2BriefArtistSchema)
-
-    @fav_artists.setter
-    def fav_artists(self, _): pass
-
-    @property
-    def fav_albums(self):
-        return create_g(self._api.user_favorite_albums, V2BriefAlbumSchema)
-
-    @fav_albums.setter
-    def fav_albums(self, _): pass
-
-    @property
-    def cloud_songs(self):
-        return create_cloud_songs_g(
-            self._api.cloud_songs,
-            self._api.cloud_songs_detail,
-            V2SongSchemaForV3,
-            NCloudSchema,
-            data_key='simpleSong'
-        )
-
-    @cloud_songs.setter
-    def cloud_songs(self, _): pass
-
-    # 根据过去经验，每日推荐歌曲在每天早上 6:00 刷新，
-    # ttl 设置为 60s 是为了能够比较即时的获取今天推荐。
-    @cached_field(ttl=60)
-    def rec_songs(self):
-        songs_data = self._api.get_recommend_songs()
-        return [_deserialize(song_data, V2SongSchemaForV3)
-                for song_data in songs_data]
-
-    def get_radio(self):
-        songs_data = self._api.get_radio_music()
-        if songs_data is None:
-            logger.error('data should not be None')
-            return None
-        return [_deserialize(song_data, V2SongSchema)
-                for song_data in songs_data]
-
-
-# import loop
-from .schemas import (  # noqa
-    V2SongSchema,
-    V2BriefAlbumSchema,
-    V2BriefArtistSchema,
-    V2PlaylistSchema,
-    NeteaseUserSchema,
-    V2SongSchemaForV3,
-    NDjradioSchema, NeteaseDjradioSchema, NCloudSchema,
-)  # noqa
+import logging
+
+from marshmallow.exceptions import ValidationError
+
+from feeluown.models import (
+    cached_field,
+    BaseModel,
+    PlaylistModel,
+    UserModel,
+    SearchModel,
+)
+from feeluown.utils.reader import RandomSequentialReader, SequentialReader
+
+from .provider import provider
+from .excs import NeteaseIOError
+
+logger = logging.getLogger(__name__)
+
+
+def _deserialize(data, schema_cls):
+    schema = schema_cls()
+    obj = schema.load(data)
+    return obj
+
+
+def create_g(func, schema=None, data_field=None):
+    data = func(limit=0)
+    if data is None:
+        raise NeteaseIOError('server responses with error status code')
+    if data_field is None:
+        data_field = 'data'
+
+    count = int(data['count'])
+
+    def read_func(start, end):
+        data = func(start, end - start)
+        return [_deserialize(data, schema)
+                for data in data[data_field]]
+
+    reader = RandomSequentialReader(count,
+                                    read_func=read_func,
+                                    max_per_read=200)
+    return reader
+
+
+def create_cloud_songs_g(func, func_extra, schema=None, schema_extra=None,
+                         data_field=None, data_key=None):
+    data = func(limit=0)
+    if data is None:
+        raise NeteaseIOError('server responses with error status code')
+    if data_field is None:
+        data_field = 'data'
+
+    count = int(data['count'])
+
+    def read_func(start, end):
+        songs_data = func(start, end - start)
+
+        songs = []
+        extra_songs_info = []
+        for idx, song_data in enumerate(songs_data[data_field]):
+            if data_key:
+                song_data = song_data[data_key]
+            try:
+                song = _deserialize(song_data, schema)
+            except ValidationError:
+                # FIXME: 有些云盘歌曲在 netease 上不存在，这时不能把它们转换成
+                # SongModel。因为 SongModel 的逻辑没有考虑 song 不存在的情况。
+                # 这类歌曲往往没有 ar/al 等字段，在反序列化的时候会报 ValidationError，
+                # 所以这里如果检测到 ValidationError，就跳过这首歌曲。
+                #
+                # 可能的修复方法：
+                # 1. 在 SongModel 上加一个 flag 来标识该歌曲是否为云盘歌曲，
+                #    如果是的话，则使用 cloud_song_detail 接口来获取相关信息。
+                # name = song_data['name']
+                # logger.warn(f'cloud song:{name} may not exist on netease, skip it.')
+                extra_songs_info.append((idx, song_data['id']))
+                # song_data = func_extra(str(song_data['id']))[data_field][0]
+                # song = _deserialize(song_data, schema_extra)
+            else:
+                songs.append(song)
+
+        if extra_songs_info:
+            extra_song_ids = ','.join([str(id) for (_, id) in extra_songs_info])
+            extra_songs_data = func_extra(extra_song_ids)
+            for idx, song_data in enumerate(extra_songs_data[data_field]):
+                song = _deserialize(song_data, schema_extra)
+                songs.insert(extra_songs_info[idx][0], song)
+
+        return songs
+
+    reader = RandomSequentialReader(count,
+                                    read_func=read_func,
+                                    max_per_read=200)
+    return reader
+
+
+class NBaseModel(BaseModel):
+    # FIXME: remove _detail_fields and _api to Meta
+    _api = provider.api
+
+    class Meta:
+        allow_get = True
+        provider = provider
+
+
+class NRadioModel(PlaylistModel, NBaseModel):
+    class Meta:
+        allow_create_songs_g = True
+
+    def create_songs_g(self):
+        data = self._api.djradio_list(self.identifier, limit=1, offset=0)
+        count = data.get('count', 0)
+
+        def g():
+            offset = 0
+            per = 50  # speed up first request
+            while offset < count:
+                tracks_data = self._api.djradio_list(
+                    self.identifier, limit=per, offset=offset)
+                for track_data in tracks_data.get('programs', []):
+                    yield _deserialize(track_data, NDjradioSchema)
+                offset += per
+
+        return SequentialReader(g(), count)
+
+    @classmethod
+    def get(cls, identifier):
+        data = cls._api.djradio_detail(identifier)
+        radio = _deserialize(data, NDjradioSchema)
+        return radio
+
+
+class NSearchModel(SearchModel, NBaseModel):
+    pass
+
+
+class NUserModel(UserModel, NBaseModel):
+    class Meta:
+        fields = ('cookies',)
+        fields_no_get = ('cookies', 'rec_songs', 'rec_playlists',
+                         'fav_artists', 'fav_albums', )
+
+    @classmethod
+    def get(cls, identifier):
+        user = {'id': identifier}
+        user_profile = cls._api.user_profile(identifier)
+        user['name'] = user_profile['nickname']
+        playlists = cls._api.user_playlists(identifier)
+
+        user['playlists'] = []
+        user['fav_playlists'] = []
+        for pl in playlists:
+            if str(pl['userId']) == str(identifier):
+                user['playlists'].append(pl)
+            else:
+                user['fav_playlists'].append(pl)
+        # FIXME: GUI模式下无法显示歌单描述
+        user = _deserialize(user, NeteaseUserSchema)
+        return user
+
+    @cached_field()
+    def rec_playlists(self):
+        playlists_data = self._api.get_recommend_playlists()
+        rec_playlists = []
+        for playlist_data in playlists_data:
+            # FIXME: GUI模式下无法显示歌单描述
+            playlist_data['coverImgUrl'] = playlist_data['picUrl']
+            playlist_data['description'] = None
+            playlist = _deserialize(playlist_data, V2PlaylistSchema)
+            rec_playlists.append(playlist)
+        return rec_playlists
+
+    @property
+    def fav_djradio(self):
+        return create_g(self._api.subscribed_djradio, NeteaseDjradioSchema, 'djRadios')
+
+    @fav_djradio.setter
+    def fav_djradio(self, _):
+        pass
+
+    @property
+    def fav_artists(self):
+        return create_g(self._api.user_favorite_artists, V2BriefArtistSchema)
+
+    @fav_artists.setter
+    def fav_artists(self, _): pass
+
+    @property
+    def fav_albums(self):
+        return create_g(self._api.user_favorite_albums, V2BriefAlbumSchema)
+
+    @fav_albums.setter
+    def fav_albums(self, _): pass
+
+    @property
+    def cloud_songs(self):
+        return create_cloud_songs_g(
+            self._api.cloud_songs,
+            self._api.cloud_songs_detail,
+            V2SongSchemaForV3,
+            NCloudSchema,
+            data_key='simpleSong'
+        )
+
+    @cloud_songs.setter
+    def cloud_songs(self, _): pass
+
+    # 根据过去经验，每日推荐歌曲在每天早上 6:00 刷新，
+    # ttl 设置为 60s 是为了能够比较即时的获取今天推荐。
+    @cached_field(ttl=60)
+    def rec_songs(self):
+        songs_data = self._api.get_recommend_songs()
+        return [_deserialize(song_data, V2SongSchemaForV3)
+                for song_data in songs_data]
+
+    def get_radio(self):
+        songs_data = self._api.get_radio_music()
+        if songs_data is None:
+            logger.error('data should not be None')
+            return None
+        return [_deserialize(song_data, V2SongSchema)
+                for song_data in songs_data]
+
+
+# import loop
+from .schemas import (  # noqa
+    V2SongSchema,
+    V2BriefAlbumSchema,
+    V2BriefArtistSchema,
+    V2PlaylistSchema,
+    NeteaseUserSchema,
+    V2SongSchemaForV3,
+    NDjradioSchema, NeteaseDjradioSchema, NCloudSchema,
+)  # noqa
```

### Comparing `fuo_netease-0.9.4/fuo_netease/nem.py` & `fuo_netease-0.9.5/fuo_netease/nem.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import asyncio
-import logging
-
-from PyQt5.QtCore import QObject
-
-from .excs import NeteaseIOError
-from .provider import provider
-from .login_controller import LoginController
-from .ui import LoginDialog
-
-
-logger = logging.getLogger(__name__)
-
-
-class Nem(QObject):
-    """
-
-    FIXME: 简化 login_as 和 ready_to_login 两个方法的实现逻辑
-    """
-
-    def __init__(self, app):
-        super(Nem, self).__init__(parent=app)
-        self._app = app
-        self.login_dialog = LoginDialog(
-            verify_captcha=LoginController.check_captcha,
-            verify_userpw=LoginController.check,
-            create_user=LoginController.create,
-        )
-        self._user = None
-        self._pm = None
-
-    def initialize(self):
-        from .page_explore import render as explore_render # noqa
-        from .page_fav import render as fav_render  # noqa
-        from .page_daily_recommendation import render as dr_render
-
-        self._app.browser.route('/providers/netease/explore')(explore_render)
-        self._app.browser.route('/providers/netease/fav')(fav_render)
-        self._app.browser.route('/providers/netease/daily_recommendation')(dr_render)
-
-    def ready_to_login(self):
-        if self._user is not None:
-            logger.debug('You have already logined in.')
-            asyncio.ensure_future(self.login_as(self._user))
-            return
-        logger.debug('Trying to load last login user...')
-        user = LoginController.load()
-        if user is None or 'MUSIC_U' not in user.cookies:
-            logger.debug('Trying to load last login user...failed')
-            self.login_dialog.show()
-            self.login_dialog.load_user_pw()
-            self.login_dialog.login_success.connect(
-                lambda user: asyncio.ensure_future(self.login_as(user)))
-        else:
-            logger.debug('Trying to load last login user...done')
-            asyncio.ensure_future(self.login_as(user))
-
-    async def login_as(self, user):
-        provider.auth(user)
-        self._user = user
-        LoginController.save(user)
-        left_panel = self._app.ui.left_panel
-        left_panel.playlists_con.show()
-        left_panel.my_music_con.show()
-
-        mymusic_explore_item = self._app.mymusic_uimgr.create_item('🎵 发现音乐')
-        mymusic_explore_item.clicked.connect(
-            lambda: self._app.browser.goto(page='/providers/netease/explore'),
-            weak=False)
-        mymusic_fm_item = self._app.mymusic_uimgr.create_item('📻 私人 FM')
-        mymusic_fm_item.clicked.connect(self.activate_fm)
-        mymusic_fav_item = self._app.mymusic_uimgr.create_item('♥ 收藏与关注')
-        mymusic_fav_item.clicked.connect(
-            lambda: self._app.browser.goto(page='/providers/netease/fav'),
-            weak=False)
-
-        self._app.mymusic_uimgr.clear()
-        self._app.mymusic_uimgr.add_item(mymusic_explore_item)
-        self._app.mymusic_uimgr.add_item(mymusic_fm_item)
-        self._app.mymusic_uimgr.add_item(mymusic_fav_item)
-
-        loop = asyncio.get_event_loop()
-        playlists = await loop.run_in_executor(None, lambda: user.playlists)
-        self._app.pl_uimgr.clear()
-        self._app.pl_uimgr.add(playlists)
-        self._app.pl_uimgr.add(user.fav_playlists, is_fav=True)
-        # self._app.pl_uimgr.add(user.rec_playlists)
-
-    def activate_fm(self):
-        self._app.fm.activate(self.fetch_fm_songs)
-
-    def fetch_fm_songs(self, *args, **kwargs):
-        songs = provider._user.get_radio()  # noqa
-        if songs is None:
-            raise NeteaseIOError('unknown error: get no radio songs')
-        return songs
+import asyncio
+import logging
+
+from PyQt5.QtCore import QObject
+
+from .excs import NeteaseIOError
+from .provider import provider
+from .login_controller import LoginController
+from .ui import LoginDialog
+
+
+logger = logging.getLogger(__name__)
+
+
+class Nem(QObject):
+    """
+
+    FIXME: 简化 login_as 和 ready_to_login 两个方法的实现逻辑
+    """
+
+    def __init__(self, app):
+        super(Nem, self).__init__(parent=app)
+        self._app = app
+        self.login_dialog = LoginDialog(
+            verify_captcha=LoginController.check_captcha,
+            verify_userpw=LoginController.check,
+            create_user=LoginController.create,
+        )
+        self._user = None
+        self._pm = None
+
+    def initialize(self):
+        from .page_explore import render as explore_render # noqa
+        from .page_fav import render as fav_render  # noqa
+        from .page_daily_recommendation import render as dr_render
+
+        self._app.browser.route('/providers/netease/explore')(explore_render)
+        self._app.browser.route('/providers/netease/fav')(fav_render)
+        self._app.browser.route('/providers/netease/daily_recommendation')(dr_render)
+
+    def ready_to_login(self):
+        if self._user is not None:
+            logger.debug('You have already logined in.')
+            asyncio.ensure_future(self.login_as(self._user))
+            return
+        logger.debug('Trying to load last login user...')
+        user = LoginController.load()
+        if user is None or 'MUSIC_U' not in user.cookies:
+            logger.debug('Trying to load last login user...failed')
+            self.login_dialog.show()
+            self.login_dialog.load_user_pw()
+            self.login_dialog.login_success.connect(
+                lambda user: asyncio.ensure_future(self.login_as(user)))
+        else:
+            logger.debug('Trying to load last login user...done')
+            asyncio.ensure_future(self.login_as(user))
+
+    async def login_as(self, user):
+        provider.auth(user)
+        self._user = user
+        LoginController.save(user)
+        left_panel = self._app.ui.left_panel
+        left_panel.playlists_con.show()
+        left_panel.my_music_con.show()
+
+        mymusic_explore_item = self._app.mymusic_uimgr.create_item('🎵 发现音乐')
+        mymusic_explore_item.clicked.connect(
+            lambda: self._app.browser.goto(page='/providers/netease/explore'),
+            weak=False)
+        mymusic_fm_item = self._app.mymusic_uimgr.create_item('📻 私人 FM')
+        mymusic_fm_item.clicked.connect(self.activate_fm)
+        mymusic_fav_item = self._app.mymusic_uimgr.create_item('♥ 收藏与关注')
+        mymusic_fav_item.clicked.connect(
+            lambda: self._app.browser.goto(page='/providers/netease/fav'),
+            weak=False)
+
+        self._app.mymusic_uimgr.clear()
+        self._app.mymusic_uimgr.add_item(mymusic_explore_item)
+        self._app.mymusic_uimgr.add_item(mymusic_fm_item)
+        self._app.mymusic_uimgr.add_item(mymusic_fav_item)
+
+        loop = asyncio.get_event_loop()
+        playlists = await loop.run_in_executor(None, lambda: user.playlists)
+        self._app.pl_uimgr.clear()
+        self._app.pl_uimgr.add(playlists)
+        self._app.pl_uimgr.add(user.fav_playlists, is_fav=True)
+        # self._app.pl_uimgr.add(user.rec_playlists)
+
+    def activate_fm(self):
+        self._app.fm.activate(self.fetch_fm_songs)
+
+    def fetch_fm_songs(self, *args, **kwargs):
+        songs = provider._user.get_radio()  # noqa
+        if songs is None:
+            raise NeteaseIOError('unknown error: get no radio songs')
+        return songs
```

### Comparing `fuo_netease-0.9.4/fuo_netease/page_daily_recommendation.py` & `fuo_netease-0.9.5/fuo_netease/page_daily_recommendation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from feeluown.utils import aio
-from feeluown.gui.page_containers.table import Renderer
-
-
-async def render(req, **kwargs):
-    app = req.ctx['app']
-    provider = app.library.get('netease')
-    user = provider._user
-
-    app.ui.right_panel.set_body(app.ui.right_panel.table_container)
-    renderer = DailyRecommendationRenderer(user)
-    await app.ui.right_panel.table_container.set_renderer(renderer)
-
-
-class DailyRecommendationRenderer(Renderer):
-    def __init__(self, user):
-        self._user = user
-
-    async def render(self):
-        self.meta_widget.title = '每日推荐'
-        self.meta_widget.show()
-
-        self.show_songs(await aio.run_fn(lambda: self._user.rec_songs))
+from feeluown.utils import aio
+from feeluown.gui.page_containers.table import Renderer
+
+
+async def render(req, **kwargs):
+    app = req.ctx['app']
+    provider = app.library.get('netease')
+    user = provider._user
+
+    app.ui.right_panel.set_body(app.ui.right_panel.table_container)
+    renderer = DailyRecommendationRenderer(user)
+    await app.ui.right_panel.table_container.set_renderer(renderer)
+
+
+class DailyRecommendationRenderer(Renderer):
+    def __init__(self, user):
+        self._user = user
+
+    async def render(self):
+        self.meta_widget.title = '每日推荐'
+        self.meta_widget.show()
+
+        self.show_songs(await aio.run_fn(lambda: self._user.rec_songs))
```

### Comparing `fuo_netease-0.9.4/fuo_netease/page_explore.py` & `fuo_netease-0.9.5/fuo_netease/page_explore.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QLabel, QHBoxLayout
-
-from feeluown.utils.reader import wrap
-from feeluown.gui.widgets.playlist import PlaylistListView, PlaylistListModel, \
-    PlaylistFilterProxyModel
-from feeluown.gui.widgets.textbtn import TextButton
-from feeluown.gui.helpers import fetch_cover_wrapper, BgTransparentMixin
-
-
-async def render(req, **kwargs):
-    app = req.ctx['app']
-    provider = app.library.get('netease')
-
-    playlists = provider._user.rec_playlists
-    view = ExploreView()
-    view.daily_rec_btn.clicked.connect(
-        lambda: app.browser.goto(page='/providers/netease/daily_recommendation'))
-    model = PlaylistListModel(wrap(playlists),
-                              fetch_cover_wrapper(app),
-                              {p.identifier: p.name for p in app.library.list()})
-    filter_model = PlaylistFilterProxyModel()
-    filter_model.setSourceModel(model)
-    view.playlist_list_view.setModel(filter_model)
-    view.playlist_list_view.show_playlist_needed.connect(
-        lambda model: app.browser.goto(model=model))
-    app.ui.right_panel.set_body(view)
-
-
-class HeaderLabel(QLabel):
-    def __init__(self):
-        super().__init__()
-
-        self.setTextFormat(Qt.RichText)
-        # Margin is same as playlist list view CoverSpacing
-        self.setIndent(20)
-
-
-class _PlaylistListView(PlaylistListView, BgTransparentMixin):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, no_scroll_v=True, **kwargs)
-        BgTransparentMixin.__init__(self)
-
-
-class ExploreView(QWidget):
-    def __init__(self):
-        super().__init__(parent=None)
-
-        self.header_title = HeaderLabel()
-        self.header_playlist_list = HeaderLabel()
-        self.header_daily_rec = HeaderLabel()
-        self.playlist_list_view = _PlaylistListView(img_min_width=100)
-        self.daily_rec_btn = TextButton('查看每日推荐')
-
-        self.header_title.setText('<h1>发现音乐</h1>')
-        self.header_playlist_list.setText('<h2>个性化推荐</h2>')
-        self.header_daily_rec.setText('<h2>每日推荐</h2>')
-
-        self._daily_rec_layout = QHBoxLayout()
-        self._layout = QVBoxLayout(self)
-        self._setup_ui()
-
-    def _setup_ui(self):
-        self.playlist_list_view.setWrapping(False)
-
-        self._layout.setContentsMargins(0, 10, 0, 0)
-        self._layout.setSpacing(0)
-        self._layout.addWidget(self.header_title)
-        self._layout.addSpacing(30)
-        self._layout.addWidget(self.header_daily_rec)
-        self._layout.addSpacing(5)
-        self._layout.addLayout(self._daily_rec_layout)
-        self._layout.addSpacing(20)
-        self._layout.addWidget(self.header_playlist_list)
-        self._layout.addWidget(self.playlist_list_view)
-        self._layout.addStretch(0)
-
-        # NOTE(cosven): 人肉设置一个 25 的间距，在 macOS 看起来勉强还行
-        self._daily_rec_layout.addSpacing(25)
-        self._daily_rec_layout.addWidget(self.daily_rec_btn)
-        self._daily_rec_layout.addStretch(0)
+from PyQt5.QtCore import Qt
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QLabel, QHBoxLayout
+
+from feeluown.utils.reader import wrap
+from feeluown.gui.widgets.playlist import PlaylistListView, PlaylistListModel, \
+    PlaylistFilterProxyModel
+from feeluown.gui.widgets.textbtn import TextButton
+from feeluown.gui.helpers import fetch_cover_wrapper, BgTransparentMixin
+
+
+async def render(req, **kwargs):
+    app = req.ctx['app']
+    provider = app.library.get('netease')
+
+    playlists = provider._user.rec_playlists
+    view = ExploreView()
+    view.daily_rec_btn.clicked.connect(
+        lambda: app.browser.goto(page='/providers/netease/daily_recommendation'))
+    model = PlaylistListModel(wrap(playlists),
+                              fetch_cover_wrapper(app),
+                              {p.identifier: p.name for p in app.library.list()})
+    filter_model = PlaylistFilterProxyModel()
+    filter_model.setSourceModel(model)
+    view.playlist_list_view.setModel(filter_model)
+    view.playlist_list_view.show_playlist_needed.connect(
+        lambda model: app.browser.goto(model=model))
+    app.ui.right_panel.set_body(view)
+
+
+class HeaderLabel(QLabel):
+    def __init__(self):
+        super().__init__()
+
+        self.setTextFormat(Qt.RichText)
+        # Margin is same as playlist list view CoverSpacing
+        self.setIndent(20)
+
+
+class _PlaylistListView(PlaylistListView, BgTransparentMixin):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, no_scroll_v=True, **kwargs)
+        BgTransparentMixin.__init__(self)
+
+
+class ExploreView(QWidget):
+    def __init__(self):
+        super().__init__(parent=None)
+
+        self.header_title = HeaderLabel()
+        self.header_playlist_list = HeaderLabel()
+        self.header_daily_rec = HeaderLabel()
+        self.playlist_list_view = _PlaylistListView(img_min_width=100)
+        self.daily_rec_btn = TextButton('查看每日推荐')
+
+        self.header_title.setText('<h1>发现音乐</h1>')
+        self.header_playlist_list.setText('<h2>个性化推荐</h2>')
+        self.header_daily_rec.setText('<h2>每日推荐</h2>')
+
+        self._daily_rec_layout = QHBoxLayout()
+        self._layout = QVBoxLayout(self)
+        self._setup_ui()
+
+    def _setup_ui(self):
+        self.playlist_list_view.setWrapping(False)
+
+        self._layout.setContentsMargins(0, 10, 0, 0)
+        self._layout.setSpacing(0)
+        self._layout.addWidget(self.header_title)
+        self._layout.addSpacing(30)
+        self._layout.addWidget(self.header_daily_rec)
+        self._layout.addSpacing(5)
+        self._layout.addLayout(self._daily_rec_layout)
+        self._layout.addSpacing(20)
+        self._layout.addWidget(self.header_playlist_list)
+        self._layout.addWidget(self.playlist_list_view)
+        self._layout.addStretch(0)
+
+        # NOTE(cosven): 人肉设置一个 25 的间距，在 macOS 看起来勉强还行
+        self._daily_rec_layout.addSpacing(25)
+        self._daily_rec_layout.addWidget(self.daily_rec_btn)
+        self._daily_rec_layout.addStretch(0)
```

### Comparing `fuo_netease-0.9.4/fuo_netease/schemas.py` & `fuo_netease-0.9.5/fuo_netease/schemas.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-"""
-
-关于命名
-~~~~~~~~~~~~~~~
-V2{X}Schema 返回的 model 都是 v2 版本的 Model 实例，也就是从 feeluown.library
-模块导入进来的 Model 类。
-
-{X}SchemaForV3 的数据来源都是 api uri_v3 接口获取的数据。
-"""
-
-import logging
-from datetime import datetime
-
-from marshmallow import Schema, post_load, fields, EXCLUDE
-
-from feeluown.library import (
-    SongModel, BriefAlbumModel, BriefArtistModel, ModelState, BriefSongModel,
-    VideoModel, AlbumModel, ArtistModel, PlaylistModel, BriefUserModel,
-)
-from feeluown.media import Quality, MediaType, Media
-
-logger = logging.getLogger(__name__)
-
-
-class BaseSchema(Schema):
-    source = fields.Str(missing='netease')
-
-    class Meta:
-        unknown = EXCLUDE
-
-
-Schema = BaseSchema
-Unknown = 'Unknown'
-
-
-def create_model(model_cls, data, fields_to_cache=None):
-    """
-    maybe this function should be provided by feeluown
-
-    :param fields_to_cache: list of fields name to be cached
-    """
-    if fields_to_cache is not None:
-        cache_data = {}
-        for field in fields_to_cache:
-            value = data.pop(field)
-            if value is not None:
-                cache_data[field] = value
-        model = model_cls(**data)
-        for field, value in cache_data.items():
-            model.cache_set(field, value)
-    else:
-        model = model_cls(**data)
-    return model
-
-
-class V2MvSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    title = fields.Str(required=True, data_key='name')
-    cover = fields.Str(required=True)
-    brs = fields.Dict(required=True)
-    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
-    duration = fields.Int(required=True)
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        brs = data.pop('brs')
-        q_media_mapping = {}
-        for q, url in brs.items():
-            media = Media(url, type_=MediaType.video)
-            if q == '1080':
-                quality = Quality.Video.fhd
-            elif q == '720':
-                quality = Quality.Video.hd
-            elif q == '480':
-                quality = Quality.Video.sd
-            elif q == '240':
-                quality = Quality.Video.ld
-            else:
-                logger.warning('There exists another quality:%s mv.', q)
-                quality = Quality.Video.sd
-            q_media_mapping[quality] = media
-        data['q_media_mapping'] = q_media_mapping
-        data['identifier'] = 'mv_' + str(data['identifier'])
-        return create_model(VideoModel, data, ['q_media_mapping'])
-
-
-class V2BriefAlbumSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True, allow_none=True)
-    # cover = fields.Str(data_key='picUrl', allow_none=True)
-    artist = fields.Dict()
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        if data['name'] is None:
-            data['name'] = Unknown
-        if 'artist' in data:
-            artist = data.pop('artist')
-            data['artists_name'] = artist['name']
-        return BriefAlbumModel(**data)
-
-
-class V2BriefArtistSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True, allow_none=True)
-
-    # cover = fields.Str(data_key='picUrl', allow_none=True)
-    # songs = fields.List(fields.Nested('V2SongSchema'))
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        if data['name'] is None:
-            data['name'] = Unknown
-        return BriefArtistModel(**data)
-
-
-class V2SongSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    title = fields.Str(required=True, data_key='name', allow_none=True)
-    duration = fields.Float(required=True)
-    album = fields.Nested('V2BriefAlbumSchema')
-    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
-
-    mv_id = fields.Int(required=True, data_key='mvid')
-    comment_thread_id = fields.Str(data_key='commentThreadId',
-                                   allow_none=True, missing=None)
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        # https://github.com/feeluown/FeelUOwn/issues/499
-        if data['title'] is None:
-            data['title'] = Unknown
-        return create_model(SongModel, data, ['mv_id', 'comment_thread_id'])
-
-
-class V2SongSchemaForV3(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    title = fields.Str(required=True, data_key='name')
-    duration = fields.Float(required=True, data_key='dt')
-    album = fields.Nested('V2BriefAlbumSchema', data_key='al')
-    artists = fields.List(fields.Nested('V2BriefArtistSchema'), data_key='ar')
-
-    mv_id = fields.Int(required=True, data_key='mv')
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        return create_model(SongModel, data, ['mv_id'])
-
-
-class V2AlbumSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True)
-    cover = fields.Str(data_key='picUrl', allow_none=True)
-    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
-    # 收藏和搜索接口返回的 album 数据中的 songs 为 None
-    songs = fields.List(fields.Nested('V2SongSchema'), allow_none=True)
-
-    # Description is fetched seperatelly by `album_desc` API.
-    description = fields.Str(missing='')
-    released = fields.Int(data_key='publishTime', missing=0)
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        released = data['released']
-        if released:
-            released_date = datetime.fromtimestamp(released / 1000)
-            released_str = released_date.strftime('%Y-%m-%d')
-            data['released'] = released_str
-        return AlbumModel(**data)
-
-
-class V2ArtistSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str()
-    pic_url = fields.Str(data_key='picUrl', allow_none=True)
-    hot_songs = fields.List(fields.Nested('V2SongSchema'), data_key='songs')
-
-    # TODO:
-    aliases = fields.List(fields.Str(), missing=[])
-
-    # Description is fetched seperatelly by `artist_desc` API.
-    description = fields.Str(missing='')
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        return ArtistModel(**data)
-
-
-class NAlbumSchemaV3(Schema):
-    # 如果 album 无效，id 则为 0
-    # 只有当 album 无效时，name 才可能为 None
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True, allow_none=True)
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        album = BriefAlbumModel(**data)
-        if album.identifier == 0:
-            album.state = ModelState.not_exists
-            album.name = ''
-        return album
-
-
-class NeteaseDjradioSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True)
-    desc = fields.Str(required=False)
-    cover = fields.Str(required=False, data_key='picUrl')
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        return NRadioModel(**data)
-
-
-class NDjradioSchema(Schema):
-    # identifier = fields.Int(required=True, data_key='id')
-    # title = fields.Str(required=True, data_key='name')
-    main_song = fields.Dict(required=True, data_key='mainSong')
-    # cover = fields.Str(required=False, data_key='coverUrl')
-    radio = fields.Dict(required=True, data_key='radio')
-
-    @post_load
-    def create_model(self, data, **kwargs):
-
-        def to_duration_ms(duration):
-            seconds = duration / 1000
-            m, s = seconds / 60, seconds % 60
-            return '{:02}:{:02}'.format(int(m), int(s))
-
-        song = data.pop('main_song')
-        album_name = data.pop('radio')['name']
-        artists_name = ','.join([artist['name'] for artist in song['artists']])
-
-        return BriefSongModel(identifier=song['id'],
-                              title=song['name'],
-                              duration_ms=to_duration_ms(song['duration']),
-                              artists_name=artists_name,
-                              album_name=album_name,
-                              state=ModelState.cant_upgrade,
-                              **data)
-
-
-class NCloudSchema(Schema):
-    main_song = fields.Dict(required=True, data_key='simpleSong')
-    album_name = fields.Str(required=True, data_key='album')
-    artists_name = fields.Str(required=True, data_key='artist')
-
-    @post_load
-    def create_model(self, data, **kwargs):
-
-        def to_duration_ms(duration):
-            seconds = duration / 1000
-            m, s = seconds / 60, seconds % 60
-            return '{:02}:{:02}'.format(int(m), int(s))
-
-        song = data.pop('main_song')
-
-        return BriefSongModel(identifier=song['id'],
-                              title=song['name'],
-                              duration_ms=to_duration_ms(song['dt']),
-                              state=ModelState.cant_upgrade,
-                              **data)
-
-
-class V2PlaylistCreatorScehma(Schema):
-    identifier = fields.Int(required=True, data_key='userId')
-    name = fields.Str(required=True, data_key='nickname')
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        data['identifier'] = str(data['identifier'])
-        return BriefUserModel(**data)
-
-
-class V2PlaylistSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    creator = fields.Nested(V2PlaylistCreatorScehma, missing=None)
-    name = fields.Str(required=True)
-    description = fields.Str(required=True, allow_none=True, data_key='description')
-    cover = fields.Url(required=True, data_key='coverImgUrl')
-
-    @post_load
-    def create_v2_model(self, data, **kwargs):
-        if data.get('description') is None:
-            data['description'] = ''
-        return PlaylistModel(**data)
-
-
-class NeteaseUserSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True)
-    playlists = fields.List(fields.Nested(V2PlaylistSchema))
-    fav_playlists = fields.List(fields.Nested(V2PlaylistSchema))
-    cookies = fields.Dict()
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        return NUserModel(**data)
-
-
-class NeteaseSearchSchema(Schema):
-    """搜索结果 Schema"""
-    songs = fields.List(fields.Nested(V2SongSchema))
-    albums = fields.List(fields.Nested(V2BriefAlbumSchema))
-    artists = fields.List(fields.Nested(V2BriefArtistSchema))
-    playlists = fields.List(fields.Nested(V2PlaylistSchema))
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        return NSearchModel(**data)
-
-
-from .models import (  # noqa
-    NUserModel,
-    NSearchModel,
-    NRadioModel,
-)  # noqa
+"""
+
+关于命名
+~~~~~~~~~~~~~~~
+V2{X}Schema 返回的 model 都是 v2 版本的 Model 实例，也就是从 feeluown.library
+模块导入进来的 Model 类。
+
+{X}SchemaForV3 的数据来源都是 api uri_v3 接口获取的数据。
+"""
+
+import logging
+from datetime import datetime
+
+from marshmallow import Schema, post_load, fields, EXCLUDE
+
+from feeluown.library import (
+    SongModel, BriefAlbumModel, BriefArtistModel, ModelState, BriefSongModel,
+    VideoModel, AlbumModel, ArtistModel, PlaylistModel, BriefUserModel,
+)
+from feeluown.media import Quality, MediaType, Media
+
+logger = logging.getLogger(__name__)
+
+
+class BaseSchema(Schema):
+    source = fields.Str(missing='netease')
+
+    class Meta:
+        unknown = EXCLUDE
+
+
+Schema = BaseSchema
+Unknown = 'Unknown'
+
+
+def create_model(model_cls, data, fields_to_cache=None):
+    """
+    maybe this function should be provided by feeluown
+
+    :param fields_to_cache: list of fields name to be cached
+    """
+    if fields_to_cache is not None:
+        cache_data = {}
+        for field in fields_to_cache:
+            value = data.pop(field)
+            if value is not None:
+                cache_data[field] = value
+        model = model_cls(**data)
+        for field, value in cache_data.items():
+            model.cache_set(field, value)
+    else:
+        model = model_cls(**data)
+    return model
+
+
+class V2MvSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    title = fields.Str(required=True, data_key='name')
+    cover = fields.Str(required=True)
+    brs = fields.Dict(required=True)
+    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
+    duration = fields.Int(required=True)
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        brs = data.pop('brs')
+        q_media_mapping = {}
+        for q, url in brs.items():
+            media = Media(url, type_=MediaType.video)
+            if q == '1080':
+                quality = Quality.Video.fhd
+            elif q == '720':
+                quality = Quality.Video.hd
+            elif q == '480':
+                quality = Quality.Video.sd
+            elif q == '240':
+                quality = Quality.Video.ld
+            else:
+                logger.warning('There exists another quality:%s mv.', q)
+                quality = Quality.Video.sd
+            q_media_mapping[quality] = media
+        data['q_media_mapping'] = q_media_mapping
+        data['identifier'] = 'mv_' + str(data['identifier'])
+        return create_model(VideoModel, data, ['q_media_mapping'])
+
+
+class V2BriefAlbumSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True, allow_none=True)
+    # cover = fields.Str(data_key='picUrl', allow_none=True)
+    artist = fields.Dict()
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        if data['name'] is None:
+            data['name'] = Unknown
+        if 'artist' in data:
+            artist = data.pop('artist')
+            data['artists_name'] = artist['name']
+        return BriefAlbumModel(**data)
+
+
+class V2BriefArtistSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True, allow_none=True)
+
+    # cover = fields.Str(data_key='picUrl', allow_none=True)
+    # songs = fields.List(fields.Nested('V2SongSchema'))
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        if data['name'] is None:
+            data['name'] = Unknown
+        return BriefArtistModel(**data)
+
+
+class V2SongSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    title = fields.Str(required=True, data_key='name', allow_none=True)
+    duration = fields.Float(required=True)
+    album = fields.Nested('V2BriefAlbumSchema')
+    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
+
+    mv_id = fields.Int(required=True, data_key='mvid')
+    comment_thread_id = fields.Str(data_key='commentThreadId',
+                                   allow_none=True, missing=None)
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        # https://github.com/feeluown/FeelUOwn/issues/499
+        if data['title'] is None:
+            data['title'] = Unknown
+        return create_model(SongModel, data, ['mv_id', 'comment_thread_id'])
+
+
+class V2SongSchemaForV3(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    title = fields.Str(required=True, data_key='name')
+    duration = fields.Float(required=True, data_key='dt')
+    album = fields.Nested('V2BriefAlbumSchema', data_key='al')
+    artists = fields.List(fields.Nested('V2BriefArtistSchema'), data_key='ar')
+
+    mv_id = fields.Int(required=True, data_key='mv')
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        return create_model(SongModel, data, ['mv_id'])
+
+
+class V2AlbumSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True)
+    cover = fields.Str(data_key='picUrl', allow_none=True)
+    artists = fields.List(fields.Nested('V2BriefArtistSchema'))
+    # 收藏和搜索接口返回的 album 数据中的 songs 为 None
+    songs = fields.List(fields.Nested('V2SongSchema'), allow_none=True)
+
+    # Description is fetched seperatelly by `album_desc` API.
+    description = fields.Str(missing='')
+    released = fields.Int(data_key='publishTime', missing=0)
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        released = data['released']
+        if released:
+            released_date = datetime.fromtimestamp(released / 1000)
+            released_str = released_date.strftime('%Y-%m-%d')
+            data['released'] = released_str
+        return AlbumModel(**data)
+
+
+class V2ArtistSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str()
+    pic_url = fields.Str(data_key='picUrl', allow_none=True)
+    hot_songs = fields.List(fields.Nested('V2SongSchema'), data_key='songs')
+
+    # TODO:
+    aliases = fields.List(fields.Str(), missing=[])
+
+    # Description is fetched seperatelly by `artist_desc` API.
+    description = fields.Str(missing='')
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        return ArtistModel(**data)
+
+
+class NAlbumSchemaV3(Schema):
+    # 如果 album 无效，id 则为 0
+    # 只有当 album 无效时，name 才可能为 None
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True, allow_none=True)
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        album = BriefAlbumModel(**data)
+        if album.identifier == 0:
+            album.state = ModelState.not_exists
+            album.name = ''
+        return album
+
+
+class NeteaseDjradioSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True)
+    desc = fields.Str(required=False)
+    cover = fields.Str(required=False, data_key='picUrl')
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return NRadioModel(**data)
+
+
+class NDjradioSchema(Schema):
+    # identifier = fields.Int(required=True, data_key='id')
+    # title = fields.Str(required=True, data_key='name')
+    main_song = fields.Dict(required=True, data_key='mainSong')
+    # cover = fields.Str(required=False, data_key='coverUrl')
+    radio = fields.Dict(required=True, data_key='radio')
+
+    @post_load
+    def create_model(self, data, **kwargs):
+
+        def to_duration_ms(duration):
+            seconds = duration / 1000
+            m, s = seconds / 60, seconds % 60
+            return '{:02}:{:02}'.format(int(m), int(s))
+
+        song = data.pop('main_song')
+        album_name = data.pop('radio')['name']
+        artists_name = ','.join([artist['name'] for artist in song['artists']])
+
+        return BriefSongModel(identifier=song['id'],
+                              title=song['name'],
+                              duration_ms=to_duration_ms(song['duration']),
+                              artists_name=artists_name,
+                              album_name=album_name,
+                              state=ModelState.cant_upgrade,
+                              **data)
+
+
+class NCloudSchema(Schema):
+    main_song = fields.Dict(required=True, data_key='simpleSong')
+    album_name = fields.Str(required=True, data_key='album')
+    artists_name = fields.Str(required=True, data_key='artist')
+
+    @post_load
+    def create_model(self, data, **kwargs):
+
+        def to_duration_ms(duration):
+            seconds = duration / 1000
+            m, s = seconds / 60, seconds % 60
+            return '{:02}:{:02}'.format(int(m), int(s))
+
+        song = data.pop('main_song')
+
+        return BriefSongModel(identifier=song['id'],
+                              title=song['name'],
+                              duration_ms=to_duration_ms(song['dt']),
+                              state=ModelState.cant_upgrade,
+                              **data)
+
+
+class V2PlaylistCreatorScehma(Schema):
+    identifier = fields.Int(required=True, data_key='userId')
+    name = fields.Str(required=True, data_key='nickname')
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        data['identifier'] = str(data['identifier'])
+        return BriefUserModel(**data)
+
+
+class V2PlaylistSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    creator = fields.Nested(V2PlaylistCreatorScehma, missing=None)
+    name = fields.Str(required=True)
+    description = fields.Str(required=True, allow_none=True, data_key='description')
+    cover = fields.Url(required=True, data_key='coverImgUrl')
+
+    @post_load
+    def create_v2_model(self, data, **kwargs):
+        if data.get('description') is None:
+            data['description'] = ''
+        return PlaylistModel(**data)
+
+
+class NeteaseUserSchema(Schema):
+    identifier = fields.Int(required=True, data_key='id')
+    name = fields.Str(required=True)
+    playlists = fields.List(fields.Nested(V2PlaylistSchema))
+    fav_playlists = fields.List(fields.Nested(V2PlaylistSchema))
+    cookies = fields.Dict()
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return NUserModel(**data)
+
+
+class NeteaseSearchSchema(Schema):
+    """搜索结果 Schema"""
+    songs = fields.List(fields.Nested(V2SongSchema))
+    albums = fields.List(fields.Nested(V2BriefAlbumSchema))
+    artists = fields.List(fields.Nested(V2BriefArtistSchema))
+    playlists = fields.List(fields.Nested(V2PlaylistSchema))
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return NSearchModel(**data)
+
+
+from .models import (  # noqa
+    NUserModel,
+    NSearchModel,
+    NRadioModel,
+)  # noqa
```

### Comparing `fuo_netease-0.9.4/fuo_netease/ui.py` & `fuo_netease-0.9.5/fuo_netease/ui.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import hashlib
-import json
-import logging
-import os
-
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import (QVBoxLayout, QLineEdit,
-                             QDialog, QPushButton,
-                             QLabel)
-
-from .consts import USER_PW_FILE
-
-logger = logging.getLogger(__name__)
-
-
-class LoginDialog(QDialog):
-    login_success = pyqtSignal([object])
-
-    def __init__(self, verify_captcha, verify_userpw, create_user,
-                 parent=None):
-        super().__init__(parent)
-
-        self.verify_captcha = verify_captcha
-        self.verify_userpw = verify_userpw
-        self.create_user = create_user
-
-        self.is_encrypted = False
-        self.captcha_needed = False
-        self.captcha_id = 0
-
-        self.country_code_input = QLineEdit(self)
-        self.username_input = QLineEdit(self)
-        self.pw_input = QLineEdit(self)
-        self.pw_input.setEchoMode(QLineEdit.Password)
-        # self.remember_checkbox = FCheckBox(self)
-        self.captcha_label = QLabel(self)
-        self.captcha_label.hide()
-        self.captcha_input = QLineEdit(self)
-        self.captcha_input.hide()
-        self.hint_label = QLabel(self)
-        self.ok_btn = QPushButton('登录', self)
-        self._layout = QVBoxLayout(self)
-
-        self.country_code_input.setPlaceholderText('国际电话区号（默认为86）')
-        self.username_input.setPlaceholderText('网易邮箱或者手机号')
-        self.pw_input.setPlaceholderText('密码')
-
-        self.pw_input.textChanged.connect(self.dis_encrypt)
-        self.ok_btn.clicked.connect(self.login)
-
-        self.setFixedWidth(200)
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self._layout.setSpacing(0)
-        self._layout.addWidget(self.country_code_input)
-        self._layout.addWidget(self.username_input)
-        self._layout.addWidget(self.pw_input)
-        self._layout.addWidget(self.captcha_label)
-        self._layout.addWidget(self.captcha_input)
-        self._layout.addWidget(self.hint_label)
-        # self._layout.addWidget(self.remember_checkbox)
-        self._layout.addWidget(self.ok_btn)
-
-    def fill(self, data):
-        self.country_code_input.setText(data.get('country_code'))
-        self.username_input.setText(data['username'])
-        self.pw_input.setText(data['password'])
-        self.is_encrypted = True
-
-    def show_hint(self, text):
-        self.hint_label.setText(text)
-
-    @property
-    def data(self):
-        country_code = self.country_code_input.text()
-        username = self.username_input.text()
-        pw = self.pw_input.text()
-        if self.is_encrypted:
-            password = pw
-        else:
-            password = hashlib.md5(pw.encode('utf-8')).hexdigest()
-        d = dict(country_code=country_code, username=username, password=password)
-        return d
-
-    def captcha_verify(self, data):
-        self.captcha_needed = True
-        self.captcha_id = data['captcha_id']
-        self.captcha_input.show()
-        self.captcha_label.show()
-        # FIXME: get pixmap from url
-        # self._app.pixmap_from_url(url, self.captcha_label.setPixmap)
-
-    def dis_encrypt(self, text):
-        self.is_encrypted = False
-
-    def login(self):
-        if self.captcha_needed:
-            captcha = str(self.captcha_input.text())
-            captcha_id = self.captcha_id
-            data = self.check_captcha(captcha_id, captcha)
-            if data['code'] == 200:
-                self.captcha_input.hide()
-                self.captcha_label.hide()
-            else:
-                self.captcha_verify(data)
-
-        user_data = self.data
-        self.show_hint('正在登录...')
-        data = self.verify_userpw(user_data['country_code'],
-                                  user_data['username'],
-                                  user_data['password'])
-        message = data['message']
-        self.show_hint(message)
-        if data['code'] == 200:
-            self.save_user_pw(user_data)
-            user = self.create_user(data)
-            self.login_success.emit(user)
-            self.hide()
-        elif data['code'] == 415:
-            self.captcha_verify(data)
-
-    def save_user_pw(self, data):
-        with open(USER_PW_FILE, 'w+') as f:
-            if f.read() == '':
-                d = dict()
-            else:
-                d = json.load(f)
-            d['default'] = data['username']
-            d[d['default']] = data
-            json.dump(d, f, indent=4)
-
-        logger.info('save username and password to %s' % USER_PW_FILE)
-
-    def load_user_pw(self):
-        if not os.path.exists(USER_PW_FILE):
-            return
-        with open(USER_PW_FILE, 'r') as f:
-            d = json.load(f)
-            data = d[d['default']]
-        self.country_code_input.setText(data.get('country_code'))
-        self.username_input.setText(data['username'])
-        self.pw_input.setText(data['password'])
-        self.is_encrypted = True
-
-        logger.info('load username and password from %s' % USER_PW_FILE)
+import hashlib
+import json
+import logging
+import os
+
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import (QVBoxLayout, QLineEdit,
+                             QDialog, QPushButton,
+                             QLabel)
+
+from .consts import USER_PW_FILE
+
+logger = logging.getLogger(__name__)
+
+
+class LoginDialog(QDialog):
+    login_success = pyqtSignal([object])
+
+    def __init__(self, verify_captcha, verify_userpw, create_user,
+                 parent=None):
+        super().__init__(parent)
+
+        self.verify_captcha = verify_captcha
+        self.verify_userpw = verify_userpw
+        self.create_user = create_user
+
+        self.is_encrypted = False
+        self.captcha_needed = False
+        self.captcha_id = 0
+
+        self.country_code_input = QLineEdit(self)
+        self.username_input = QLineEdit(self)
+        self.pw_input = QLineEdit(self)
+        self.pw_input.setEchoMode(QLineEdit.Password)
+        # self.remember_checkbox = FCheckBox(self)
+        self.captcha_label = QLabel(self)
+        self.captcha_label.hide()
+        self.captcha_input = QLineEdit(self)
+        self.captcha_input.hide()
+        self.hint_label = QLabel(self)
+        self.ok_btn = QPushButton('登录', self)
+        self._layout = QVBoxLayout(self)
+
+        self.country_code_input.setPlaceholderText('国际电话区号（默认为86）')
+        self.username_input.setPlaceholderText('网易邮箱或者手机号')
+        self.pw_input.setPlaceholderText('密码')
+
+        self.pw_input.textChanged.connect(self.dis_encrypt)
+        self.ok_btn.clicked.connect(self.login)
+
+        self.setFixedWidth(200)
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self._layout.setSpacing(0)
+        self._layout.addWidget(self.country_code_input)
+        self._layout.addWidget(self.username_input)
+        self._layout.addWidget(self.pw_input)
+        self._layout.addWidget(self.captcha_label)
+        self._layout.addWidget(self.captcha_input)
+        self._layout.addWidget(self.hint_label)
+        # self._layout.addWidget(self.remember_checkbox)
+        self._layout.addWidget(self.ok_btn)
+
+    def fill(self, data):
+        self.country_code_input.setText(data.get('country_code'))
+        self.username_input.setText(data['username'])
+        self.pw_input.setText(data['password'])
+        self.is_encrypted = True
+
+    def show_hint(self, text):
+        self.hint_label.setText(text)
+
+    @property
+    def data(self):
+        country_code = self.country_code_input.text()
+        username = self.username_input.text()
+        pw = self.pw_input.text()
+        if self.is_encrypted:
+            password = pw
+        else:
+            password = hashlib.md5(pw.encode('utf-8')).hexdigest()
+        d = dict(country_code=country_code, username=username, password=password)
+        return d
+
+    def captcha_verify(self, data):
+        self.captcha_needed = True
+        self.captcha_id = data['captcha_id']
+        self.captcha_input.show()
+        self.captcha_label.show()
+        # FIXME: get pixmap from url
+        # self._app.pixmap_from_url(url, self.captcha_label.setPixmap)
+
+    def dis_encrypt(self, text):
+        self.is_encrypted = False
+
+    def login(self):
+        if self.captcha_needed:
+            captcha = str(self.captcha_input.text())
+            captcha_id = self.captcha_id
+            data = self.check_captcha(captcha_id, captcha)
+            if data['code'] == 200:
+                self.captcha_input.hide()
+                self.captcha_label.hide()
+            else:
+                self.captcha_verify(data)
+
+        user_data = self.data
+        self.show_hint('正在登录...')
+        data = self.verify_userpw(user_data['country_code'],
+                                  user_data['username'],
+                                  user_data['password'])
+        message = data['message']
+        self.show_hint(message)
+        if data['code'] == 200:
+            self.save_user_pw(user_data)
+            user = self.create_user(data)
+            self.login_success.emit(user)
+            self.hide()
+        elif data['code'] == 415:
+            self.captcha_verify(data)
+
+    def save_user_pw(self, data):
+        with open(USER_PW_FILE, 'w+') as f:
+            if f.read() == '':
+                d = dict()
+            else:
+                d = json.load(f)
+            d['default'] = data['username']
+            d[d['default']] = data
+            json.dump(d, f, indent=4)
+
+        logger.info('save username and password to %s' % USER_PW_FILE)
+
+    def load_user_pw(self):
+        if not os.path.exists(USER_PW_FILE):
+            return
+        with open(USER_PW_FILE, 'r') as f:
+            d = json.load(f)
+            data = d[d['default']]
+        self.country_code_input.setText(data.get('country_code'))
+        self.username_input.setText(data['username'])
+        self.pw_input.setText(data['password'])
+        self.is_encrypted = True
+
+        logger.info('load username and password from %s' % USER_PW_FILE)
```

### Comparing `fuo_netease-0.9.4/fuo_netease.egg-info/SOURCES.txt` & `fuo_netease-0.9.5/fuo_netease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.4/setup.py` & `fuo_netease-0.9.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python3
-
-from setuptools import setup, find_packages
-
-
-setup(
-    name='fuo_netease',
-    version='0.9.4',
-    description='feeluown netease plugin',
-    author='Cosven',
-    author_email='yinshaowen241@gmail.com',
-    packages=find_packages(exclude=('tests*',)),
-    package_data={
-        '': ['assets/*.svg',
-             ]
-        },
-    url='https://github.com/feeluown/feeluown-netease',
-    keywords=['feeluown', 'plugin', 'netease'],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3 :: Only',
-    ],
-    install_requires=[
-        'feeluown>=3.8.10.dev',
-        'beautifulsoup4',
-        'pycryptodome',
-        'marshmallow>=3.0',
-        'requests',
-        'mutagen>=1.37',
-    ],
-    extras_require={
-        'dev': [
-            # lint
-            'flake8',
-
-            # unittest
-            'pytest>=5.4.0',
-            'pytest-cov',
-        ],
-    },
-    entry_points={
-        'fuo.plugins_v1': [
-            'netease = fuo_netease',
-        ]
-    },
-)
+#!/usr/bin/env python3
+
+from setuptools import setup, find_packages
+
+
+setup(
+    name='fuo_netease',
+    version='0.9.5',
+    description='feeluown netease plugin',
+    author='Cosven',
+    author_email='yinshaowen241@gmail.com',
+    packages=find_packages(exclude=('tests*',)),
+    package_data={
+        '': ['assets/*.svg',
+             ]
+        },
+    url='https://github.com/feeluown/feeluown-netease',
+    keywords=['feeluown', 'plugin', 'netease'],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3 :: Only',
+    ],
+    install_requires=[
+        'feeluown>=3.8.10',
+        'beautifulsoup4',
+        'pycryptodome',
+        'marshmallow>=3.0',
+        'requests',
+        'mutagen>=1.37',
+    ],
+    extras_require={
+        'dev': [
+            # lint
+            'flake8',
+
+            # unittest
+            'pytest>=5.4.0',
+            'pytest-cov',
+        ],
+    },
+    entry_points={
+        'fuo.plugins_v1': [
+            'netease = fuo_netease',
+        ]
+    },
+)
```


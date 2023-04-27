# Comparing `tmp/clife_svc-1.1.tar.gz` & `tmp/clife_svc-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clife_svc-1.1.tar", last modified: Tue Jan 31 09:19:23 2023, max compression
+gzip compressed data, was "clife_svc-1.11.tar", last modified: Thu Apr 27 10:56:05 2023, max compression
```

## Comparing `clife_svc-1.1.tar` & `clife_svc-1.11.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.184860 clife_svc-1.1/
--rw-rw-rw-   0        0        0      419 2023-01-31 09:19:23.184860 clife_svc-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.028614 clife_svc-1.1/clife_svc/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.1/clife_svc/__init__.py
--rw-rw-rw-   0        0        0    12083 2023-01-13 10:01:51.000000 clife_svc-1.1/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.075528 clife_svc-1.1/clife_svc/config/
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.1/clife_svc/config/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.1/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5545 2023-01-13 06:38:56.000000 clife_svc-1.1/clife_svc/config/disconf.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.106722 clife_svc-1.1/clife_svc/errors/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.1/clife_svc/errors/__init__.py
--rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.1/clife_svc/errors/error_code.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.184860 clife_svc-1.1/clife_svc/libs/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.1/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.1/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    14254 2023-01-31 09:11:49.000000 clife_svc-1.1/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2509 2023-01-14 02:43:51.000000 clife_svc-1.1/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3461 2023-01-13 06:23:00.000000 clife_svc-1.1/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.1/clife_svc/libs/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:19:23.044236 clife_svc-1.1/clife_svc.egg-info/
--rw-rw-rw-   0        0        0      419 2023-01-31 09:19:22.000000 clife_svc-1.1/clife_svc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-01-31 09:19:22.000000 clife_svc-1.1/clife_svc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 09:19:22.000000 clife_svc-1.1/clife_svc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-01-31 09:19:22.000000 clife_svc-1.1/clife_svc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-31 09:19:22.000000 clife_svc-1.1/clife_svc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 09:19:23.184860 clife_svc-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-01-31 09:18:59.000000 clife_svc-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.931491 clife_svc-1.11/
+-rw-rw-rw-   0        0        0      420 2023-04-27 10:56:05.930494 clife_svc-1.11/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.799795 clife_svc-1.11/clife_svc/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/__init__.py
+-rw-rw-rw-   0        0        0    12238 2023-04-27 10:53:11.000000 clife_svc-1.11/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.840733 clife_svc-1.11/clife_svc/config/
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.11/clife_svc/config/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.11/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.11/clife_svc/config/disconf.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.866664 clife_svc-1.11/clife_svc/errors/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/errors/__init__.py
+-rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.11/clife_svc/errors/error_code.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.928499 clife_svc-1.11/clife_svc/libs/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.11/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    14254 2023-01-31 09:11:49.000000 clife_svc-1.11/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2649 2023-04-27 10:46:36.000000 clife_svc-1.11/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3461 2023-01-13 06:23:00.000000 clife_svc-1.11/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.11/clife_svc/libs/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.808770 clife_svc-1.11/clife_svc.egg-info/
+-rw-rw-rw-   0        0        0      420 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:56:05.931491 clife_svc-1.11/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-27 10:54:10.000000 clife_svc-1.11/setup.py
```

### Comparing `clife_svc-1.1/clife_svc/application.py` & `clife_svc-1.11/clife_svc/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,30 @@
         """
         if not cls._instance:
             with cls._instance_lock:
                 if not cls._instance:
                     cls._instance = super().__new__(cls)
         return cls._instance
 
-    def __init__(self, app_name: str, log_root_path: str = '/www/logs', *conf: Union[str, list]):
+    def __init__(self, app_name: str, log_root_path: str = '/www/logs', conf: Union[str, list] = None, log_level: str = 'DEBUG'):
         """
         构造函数
         :param app_name 项目名称
         :param log_root_path 项目输出的日志根路径，推荐使用/www/logs，便于线上统一采集日志
         :param conf: 配置文件名称列表，提供字符串列表或逗号分隔字符串
+        :param log_level: 日志收集器级别，从低到高依次为 TRACE|DEBUG|INFO|SUCCESS|WARNING|ERROR|CRITICAL
         """
 
         # app_name参数校验
 
         if not re.match(r'^([a-zA-Z0-9]+-?[a-zA-Z0-9]+)+$', app_name):
             raise Exception('app_name can only be letters, numbers, or strike-through!')
 
         self.__app_name = app_name
-        init_log(os.path.join(log_root_path, app_name), log_level='DEBUG')
+        init_log(os.path.join(log_root_path, app_name), log_level=log_level)
 
         self.__disconf_item = Disconf('clife-ai', '0.0.1-SNAPSHOT', conf).get_disconf()
         self.__configmap = ConfigMap()
 
         self.__ClientRequest = ClientRequest(self)
         self.__MQHandler = MQHandler(app=self, app_name=app_name)
```

### Comparing `clife_svc-1.1/clife_svc/config/configmap.py` & `clife_svc-1.11/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/clife_svc/config/disconf.py` & `clife_svc-1.11/clife_svc/config/disconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 配置中心
 __author__ = 'andy.hu'
 __mtime__ = '2021/07/09'
 
 """
 import os
 import sys
+from typing import Union
 
 import requests
 
 from clife_svc.libs.log import clogger
 from clife_svc.libs import utils
 
 
@@ -36,15 +37,15 @@
 
 
 class Disconf:
     """
     从 disconf 下载配置文件
     """
 
-    def __init__(self, apps, version, keys: tuple):
+    def __init__(self, apps, version, keys: Union[str, list]):
         """ 构造函数
         :param apps: disconf配置app，多个使用逗号分隔
         :param version: 配置版本号
         :param keys: 配置文件名，缺省时只加载ai-commons.properties
         """
         __ENV = int(os.environ.get("ENVIRONMENT", -1))
         self.__ROOT_DIR = os.path.abspath(os.path.dirname(sys.argv[0]))
```

### Comparing `clife_svc-1.1/clife_svc/errors/error_code.py` & `clife_svc-1.11/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/clife_svc/libs/http_request.py` & `clife_svc-1.11/clife_svc/libs/http_request.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/clife_svc/libs/log.py` & `clife_svc-1.11/clife_svc/libs/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,43 @@
 
 def _console_log_filter(record) -> bool:
     record['req_id'] = request_id.get()
     return True
 
 
 def _format(record):
-    if record['req_id']:
+    if 'req_id' in record and record['req_id']:
         return "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | " \
                "<level>{level: <8}</level> | " \
                "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> | " \
                "<cyan>{req_id}</cyan> | " \
                "<level>{message}</level>\n{exception}"
     else:
         return "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | " \
                "<level>{level: <8}</level> | " \
                "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> | " \
                "<level>{message}</level>\n{exception}"
 
 
 klogger.remove(handler_id=None)
-klogger.add(sys.stderr, filter=_console_log_filter, format=_format)
+std_handler_id = klogger.add(sys.stderr, filter=_console_log_filter, format=_format)
 tlogger = klogger.bind(time=True)
 clogger = klogger.bind(config=True)
 
 
 def init_log(log_path: str, log_level='INFO'):
     """
     初始化服务日志模块
     :param log_path: 日志输出路径
     :param log_level: 日志级别，从低到高依次为 TRACE|DEBUG|INFO|SUCCESS|WARNING|ERROR|CRITICAL
     :return:
     """
+    klogger.remove(handler_id=std_handler_id)
+    klogger.add(sys.stderr, level=log_level, filter=_console_log_filter, format=_format)
+
     # 配置项日志
     klogger.add(os.path.join(log_path, 'config.log'), format=_format,
                 filter=lambda record: record['extra'].get('config'))
 
     # 探针日志
     klogger.add(os.path.join(log_path, 'probe.log'), format=_format, retention='1 week',
                 filter=lambda record: record['extra'].get('time'))
@@ -57,16 +60,15 @@
                 format=_format,
                 level=log_level,
                 enqueue=True,
                 rotation='00:00',
                 retention='10 days',
                 encoding='utf-8',
                 compression='zip',
-                filter=lambda record: not record['extra'].get('time') and
-                                      not record['extra'].get('config'))
+                filter=lambda record: not record['extra'].get('time') and not record['extra'].get('config'))
 
 
 if __name__ == '__main__':
     print(os.path.dirname(__file__))
     print(os.path.dirname(os.path.dirname(__file__)))
     print(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
     print(os.path.abspath(os.path.dirname(os.path.dirname(os.path.dirname(__file__)))))
```

### Comparing `clife_svc-1.1/clife_svc/libs/mq_handler.py` & `clife_svc-1.11/clife_svc/libs/mq_handler.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/clife_svc/libs/utils.py` & `clife_svc-1.11/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/clife_svc.egg-info/SOURCES.txt` & `clife_svc-1.11/clife_svc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc-1.1/setup.py` & `clife_svc-1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc',   # 需要打包的名字,即本模块要发布的名字
-    version='1.01',     # 版本
+    version='1.11',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```


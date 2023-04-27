# Comparing `tmp/inhandtest-0.0.36.tar.gz` & `tmp/inhandtest-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.36.tar", last modified: Mon Apr 24 03:19:28 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.37.tar", last modified: Thu Apr 27 06:35:05 2023, max compression
```

## Comparing `inhandtest-0.0.36.tar` & `inhandtest-0.0.37.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/
--rw-rw-rw-   0        0        0      535 2023-04-24 03:19:28.000000 inhandtest-0.0.36/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.36/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.36/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.36/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.36/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.36/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.36/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.36/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.36/inhandtest/file.py
--rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.36/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     2605 2023-04-23 10:26:25.000000 inhandtest-0.0.36/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.36/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    45323 2023-04-23 10:35:33.000000 inhandtest-0.0.36/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.36/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.36/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.36/inhandtest/ip.py
--rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.36/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1222 2023-04-18 01:10:09.000000 inhandtest-0.0.36/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.36/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    22700 2023-04-24 03:15:39.000000 inhandtest-0.0.36/inhandtest/tools.py
--rw-rw-rw-   0        0        0      115 2023-04-24 03:15:39.000000 inhandtest-0.0.36/requirements.txt
--rw-rw-rw-   0        0        0     1419 2023-04-24 03:18:46.000000 inhandtest-0.0.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 06:35:05.000000 inhandtest-0.0.37/
+-rw-rw-rw-   0        0        0      535 2023-04-27 06:35:05.000000 inhandtest-0.0.37/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.37/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 06:35:05.000000 inhandtest-0.0.37/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.37/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 06:35:05.000000 inhandtest-0.0.37/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.37/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.37/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.37/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.37/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.37/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.37/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.37/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.37/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.37/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.37/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.37/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.37/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.37/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.37/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1222 2023-04-18 01:10:09.000000 inhandtest-0.0.37/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.37/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25000 2023-04-27 06:29:37.000000 inhandtest-0.0.37/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      115 2023-04-24 03:15:39.000000 inhandtest-0.0.37/requirements.txt
+-rw-rw-rw-   0        0        0     1419 2023-04-27 06:34:55.000000 inhandtest-0.0.37/setup.py
```

### Comparing `inhandtest-0.0.36/README.md` & `inhandtest-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.37/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/base_page/base_page.py` & `inhandtest-0.0.37/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.37/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/exception.py` & `inhandtest-0.0.37/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/file.py` & `inhandtest-0.0.37/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/inmodbus.py` & `inhandtest-0.0.37/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/inmqtt.py` & `inhandtest-0.0.37/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/inrequest.py` & `inhandtest-0.0.37/inhandtest/inrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,19 +583,25 @@
         for sn_ in sn:
             response = self.api.send_request('/api/v1/devices', method='get',
                                              param={"expand": 'firmwareUpgradeStatus,compatibilities,org', "limit": 10,
                                                     "compatibilities": 'nezha_device_config,nezha_device_webui',
                                                     'serialNumber': sn_}).json()
             if response.get('total') == 1:
                 res = response.get('result')[0]
+                state = res.get('state') if res.get('state') else None
                 result.append(
-                    {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('state').get('iccid'),
-                     'imei': res.get('state').get('imei'), 'imsi': res.get('state').get('imsi'),
-                     'version': res.get('firmware'), 'licenseStatus': res.get('licenseStatus'),
-                     'address': res.get('address'), 'id': res.get('_id'), 'name': res.get('name')})
+                    {'sn': sn_, 'online': res.get('online'),
+                     'iccid': state.get('iccid') if state else None,
+                     'imei': state.get('imei') if state else None,
+                     'imsi': state.get('imsi') if state else None,
+                     'version': res.get('firmware'),
+                     'licenseStatus': res.get('licenseStatus'),
+                     'address': res.get('address'),
+                     'id': res.get('_id'),
+                     'name': res.get('name')})
             else:
                 result.append(
                     {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None,
                      'version': None, 'licenseStatus': None, 'address': None, 'id': None, 'name': None})
         return result
 
     def add_device(self, sn: str, mac_or_imei: str) -> None:
```

### Comparing `inhandtest-0.0.36/inhandtest/insocket.py` & `inhandtest-0.0.37/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/inssh.py` & `inhandtest-0.0.37/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/ip.py` & `inhandtest-0.0.37/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/mail.py` & `inhandtest-0.0.37/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/pytest_email.html` & `inhandtest-0.0.37/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/telnet.py` & `inhandtest-0.0.37/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.36/inhandtest/tools.py` & `inhandtest-0.0.37/inhandtest/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 import re
 import string
 import subprocess
 import time
 import datetime
 from typing import List
 import pytz
+import winreg
 import requests
 from inhandtest.file import file_hash
+from inhandtest.exception import ResourceNotFoundError
 
 
 def loop_inspector(flag='status', timeout=90, interval=5, assertion=True):
     """装饰器，期望接收函数返回的值为True，如果为False时进行轮询，直至超时失败，如果正确就退出
 
     :param flag:  功能名称，用以输出日志，如果不填  默认为’状态’二字
     :param timeout:  循环检测超时时间
@@ -46,14 +48,45 @@
                     raise AssertionError(f'{flag} assert timeout failure')
 
         return inspector
 
     return timeout_
 
 
+def check_device_model(support_model: list, current_model: str, decorator_scope='func'):
+    """ 设备型号装饰器: 用于判断即将使用某方法或类的设备是否支持使用该方法或类
+    :param support_model: 方法或类 支持的设备型号 list, 如：['ir302', 'ir305']
+    :param current_model: 设备当前型号, str 如：'ir302'
+    :param decorator_scope: 装饰器作用域，'func'：函数级别，'class'：类级别, 默认是函数级别
+    :return:
+    """
+    if decorator_scope == 'class':
+        def wrapper(cls):
+            class Inner(cls):
+                def __init__(self, *args, **kwargs):
+                    super().__init__(*args, **kwargs)
+                    if current_model.lower() not in support_model:
+                        raise Exception(f"This class not support this device that model is {current_model}")
+
+            return Inner
+
+        return wrapper
+    elif decorator_scope == 'func':
+        def wrapper(func):
+            def inner(*args, **kwargs):
+                if current_model.lower() in support_model:
+                    return func(*args, **kwargs)
+                else:
+                    raise Exception(f"This method not support this device that model is {current_model}")
+
+            return inner
+
+        return wrapper
+
+
 def dict_merge(*dicts) -> dict:
     """合并多个字典
 
     :param dicts:
     :return:
     """
     result = {}
@@ -187,15 +220,15 @@
         for proc in psutil.process_iter(['pid', 'name']):
             try:
                 conn_list = proc.connections()
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 continue
             for conn in conn_list:
                 if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
-                    logging.info(f"进程 {proc.pid} 正在占用端口 {one_port}")
+                    logging.info(f"process {proc.pid} already use port {one_port}")
                     # 终止进程
                     proc.kill()
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
@@ -513,14 +546,38 @@
 
     try:
         _async_raise(thread.ident, SystemExit)
     except Exception as e:
         logging.warning(e)
 
 
+def is_installed(name):
+    """
+    判断windows系统是否安装了某个软件
+    :param name:
+    :return: ResourceNotFoundError
+    """
+    key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall")
+    all_installed = []
+    for i in range(0, winreg.QueryInfoKey(key)[0]):
+        skey_name = winreg.EnumKey(key, i)
+        skey = winreg.OpenKey(key, skey_name)
+        try:
+            value = winreg.QueryValueEx(skey, 'DisplayName')[0]
+            all_installed.append(value)
+            if name in value:
+                logging.info(f'Found the software {name}')
+                break
+        except:
+            pass
+    else:
+        logging.info(f'all installed software is {all_installed}')
+        raise ResourceNotFoundError(f'Not found the software {name}')
+
+
 class DotDict(dict):
     """使用点号深度获取字典key的值
 
     """
 
     def __getattr__(self, key):
         try:
@@ -533,10 +590,11 @@
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
+    is_installed('Google Chrome123')
+    # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.36/setup.py` & `inhandtest-0.0.37/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.36',
+    version='0.0.37',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```


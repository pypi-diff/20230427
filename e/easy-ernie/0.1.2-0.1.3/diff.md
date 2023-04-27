# Comparing `tmp/easy-ernie-0.1.2.tar.gz` & `tmp/easy-ernie-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-ernie-0.1.2.tar", last modified: Wed Apr 26 08:59:19 2023, max compression
+gzip compressed data, was "easy-ernie-0.1.3.tar", last modified: Thu Apr 27 03:41:12 2023, max compression
```

## Comparing `easy-ernie-0.1.2.tar` & `easy-ernie-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.606637 easy-ernie-0.1.2/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.2/LICENSE
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1590 2023-04-26 08:59:19.606487 easy-ernie-0.1.2/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      977 2023-04-26 08:55:17.000000 easy-ernie-0.1.2/README.md
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-04-26 08:59:19.606674 easy-ernie-0.1.2/setup.cfg
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      934 2023-04-26 08:56:41.000000 easy-ernie-0.1.2/setup.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.604332 easy-ernie-0.1.2/src/
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.605559 easy-ernie-0.1.2/src/easy_ernie/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      124 2023-04-26 08:15:00.000000 easy-ernie-0.1.2/src/easy_ernie/__init__.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7106 2023-04-26 08:32:27.000000 easy-ernie-0.1.2/src/easy_ernie/ernie.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:50:57.000000 easy-ernie-0.1.2/src/easy_ernie/fast_ernie.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.606308 easy-ernie-0.1.2/src/easy_ernie.egg-info/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1590 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/top_level.txt
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.382001 easy-ernie-0.1.3/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.3/LICENSE
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1654 2023-04-27 03:41:12.381861 easy-ernie-0.1.3/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1041 2023-04-27 03:38:01.000000 easy-ernie-0.1.3/README.md
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-04-27 03:41:12.382044 easy-ernie-0.1.3/setup.cfg
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      936 2023-04-26 13:00:36.000000 easy-ernie-0.1.3/setup.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.380411 easy-ernie-0.1.3/src/
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.381157 easy-ernie-0.1.3/src/easy_ernie/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      126 2023-04-26 09:22:07.000000 easy-ernie-0.1.3/src/easy_ernie/__init__.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7272 2023-04-27 03:36:55.000000 easy-ernie-0.1.3/src/easy_ernie/ernie.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      985 2023-04-27 03:36:51.000000 easy-ernie-0.1.3/src/easy_ernie/fast_ernie.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.381697 easy-ernie-0.1.3/src/easy_ernie.egg-info/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1654 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/requires.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy-ernie-0.1.2/LICENSE` & `easy-ernie-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.2/PKG-INFO` & `easy-ernie-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.2
+Version: 0.1.3
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -12,37 +12,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Release](https://img.shields.io/badge/Release-0.1.3-blue)
+---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
 ## 安装
-pip3 install easy_ernie
+pip3 install easy-ernie
 ## Cookie
 ![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Cookie Value的值.
 7. BDUSS_BFESS同理.
 ## 使用
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
-    fastErnie = FastErnie('BDUSS_BFESS', 'BAIDUID')
+    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## Acs-Token
-由于文心一言的Acs-Token的时间戳参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
+由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.2/setup.py` & `easy-ernie-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r', encoding='utf-8') as file:
+with open('./README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.1.2',
+    version='0.1.3',
     description='简洁的调用文心一言的WebAPI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
```

### Comparing `easy-ernie-0.1.2/src/easy_ernie/ernie.py` & `easy-ernie-0.1.3/src/easy_ernie/ernie.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     
     def getSign(self) -> str:
         data = requests.get(f'https://api.hack-er.cn/ernie/acs_token?BAIDUID={self.BAIDUID}',).json()
         return data.get('data')
     
     def checkRequest(self) -> None:
         if self.request.status_code != 200:
-            raise Exception(f'请求失败,请检查网络')
+            raise Exception('请求失败,请检查网络')
         
         try:
             self.request.json()
         except:
-            raise Exception(f'请求失败,响应格式错误')
+            raise Exception('请求失败,响应格式错误')
         
         if self.request.json().get('msg') == '请先登录':
-            raise Exception(f'请求失败,请先登录')
+            raise Exception('请求失败,请先登录')
         elif self.request.json().get('msg') == '用户访问被限制':
-            raise Exception(f'请求失败,用户访问被限制')
+            raise Exception('请求失败,用户访问被限制')
 
     def get(self, url: str) -> requests:
         self.request = requests.get(url, headers=self.header)
         self.checkRequest()
         return self.request
     
     def post(self, url: str, data: dict) -> requests:
@@ -147,14 +147,15 @@
                 'sign': sign
             }
         ).json()
         botChatId = data.get('data').get('botChat').get('id')
         botParentChatId = data.get('data').get('botChat').get('parent')
 
         fullAnswer = ''
+        pattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
         urls = []
         sentenceId = 0
         while True:
             sign = self.getSign()
             self.header['Acs-Token'] = sign
             data = self.post(
                 'https://yiyan.baidu.com/eb/chat/query',
@@ -168,38 +169,42 @@
                     'deviceType': 'pc',
                     'sign': sign
                 }
             ).json()
             data = data.get('data')
             sentenceId = data.get('sent_id')
             content = data.get('content')
-
+            
             if content.strip():
-                pattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
-                urls.extend(re.findall(pattern, content))
+                fullAnswer += content
                 content = re.sub(pattern, '', content)
                 content = content.replace('<br>', '\n')
                 content = content.strip()
-                fullAnswer += content
 
                 yield {
                     'answer': content,
                     'urls': urls,
                     'sessionId': sessionId,
-                    'chatId': botChatId,
+                    'botChatId': botChatId,
                     'done': False
                 }
 
             if data.get('stop') == 1 or data.get('is_end') == 1:
                 break
+        
+        urls.extend(re.findall(pattern, fullAnswer))
+        fullAnswer = re.sub(pattern, '', fullAnswer)
+        fullAnswer = fullAnswer.replace('<br>', '\n')
+        fullAnswer = fullAnswer.strip()
+        
         yield {
             'answer': fullAnswer,
             'urls': urls,
             'sessionId': sessionId,
-            'chatId': botChatId,
+            'botChatId': botChatId,
             'done': True
         }
 
     def ask(self, question: str, sessionId: str='', parentChatId: str='') -> dict:
         result = {}
         for item in self.askStream(question, sessionId, parentChatId):
             result = item
```

### Comparing `easy-ernie-0.1.2/src/easy_ernie/fast_ernie.py` & `easy-ernie-0.1.3/src/easy_ernie/fast_ernie.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Author: XiaoXinYo
 
 from typing import Generator
-from ernie import Ernie
+from .ernie import Ernie
 
 class FastErnie:
-    def __init__(self, BAIDUID, BDUSS_BFESS):
+    def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.ernie = Ernie(BAIDUID, BDUSS_BFESS)
         self.sessionId = ''
         self.parentChatId = 0
 
     def askStream(self, question: str) -> Generator:
         if not self.sessionId:
             self.sessionId = self.ernie.newConversation(question)
         for item in self.ernie.askStream(question, self.sessionId, self.parentChatId):
-            self.parentChatId = item.get('chatId')
+            self.parentChatId = item.get('botChatId')
             yield item
-
+    
     def ask(self, question: str) -> dict:
-        if not self.sessionId:
-            self.sessionId = self.ernie.newConversation(question)
-        data = self.ernie.ask(question, self.sessionId, self.parentChatId)
-        self.parentChatId = data.get('chatId')
-        return data
+        result = {}
+        for item in self.askStream(question):
+            result = item
+        del result['done']
+        return result
     
     def close(self) -> bool:
         if self.ernie.deleteConversation(self.sessionId):
             self.sessionId = ''
             self.parentChatId = 0
             return True
         return False
```

### Comparing `easy-ernie-0.1.2/src/easy_ernie.egg-info/PKG-INFO` & `easy-ernie-0.1.3/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.2
+Version: 0.1.3
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -12,37 +12,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Release](https://img.shields.io/badge/Release-0.1.3-blue)
+---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
 ## 安装
-pip3 install easy_ernie
+pip3 install easy-ernie
 ## Cookie
 ![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Cookie Value的值.
 7. BDUSS_BFESS同理.
 ## 使用
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
-    fastErnie = FastErnie('BDUSS_BFESS', 'BAIDUID')
+    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## Acs-Token
-由于文心一言的Acs-Token的时间戳参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
+由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```


# Comparing `tmp/gpt4free-0.1.0.tar.gz` & `tmp/gpt4free-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\gpt4free package\dist\.tmp-vwtk1lcw\gpt4free-0.1.0.tar", last modified: Thu Apr 27 07:44:49 2023, max compression
+gzip compressed data, was "F:\Progamming Project\gpt4free package\dist\.tmp-emxh83ft\gpt4free-0.1.1.tar", last modified: Thu Apr 27 08:35:18 2023, max compression
```

## Comparing `gpt4free-0.1.0.tar` & `gpt4free-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.965187 gpt4free-0.1.0/
--rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.0/AUTHORS.md
--rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0       13 2023-04-27 07:39:57.000000 gpt4free-0.1.0/HISTORY.md
--rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1360 2023-04-27 07:44:49.966186 gpt4free-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-27 06:30:06.000000 gpt4free-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.938190 gpt4free-0.1.0/gpt4free/
--rw-rw-rw-   0        0        0      136 2023-04-27 06:08:54.000000 gpt4free-0.1.0/gpt4free/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.951187 gpt4free-0.1.0/gpt4free/forefront/
--rw-rw-rw-   0        0        0     5464 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/forefront/__init__.py
--rw-rw-rw-   0        0        0     2147 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/forefront/mail.py
--rw-rw-rw-   0        0        0     1795 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/forefront/typing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.958187 gpt4free-0.1.0/gpt4free/quora/
--rw-rw-rw-   0        0        0    22519 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/quora/__init__.py
--rw-rw-rw-   0        0        0    19819 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/quora/api.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.960187 gpt4free-0.1.0/gpt4free/quora/graphql/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/quora/graphql/__init__.py
--rw-rw-rw-   0        0        0     2391 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/quora/mail.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.963186 gpt4free-0.1.0/gpt4free/theb/
--rw-rw-rw-   0        0        0     1699 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/theb/__init__.py
--rw-rw-rw-   0        0        0      104 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/theb/theb_test.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.964187 gpt4free-0.1.0/gpt4free/you/
--rw-rw-rw-   0        0        0     3716 2023-04-27 05:59:26.000000 gpt4free-0.1.0/gpt4free/you/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:44:49.947185 gpt4free-0.1.0/gpt4free.egg-info/
--rw-rw-rw-   0        0        0     1360 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      124 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 07:44:49.000000 gpt4free-0.1.0/gpt4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-04-27 07:44:49.968186 gpt4free-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2212 2023-04-27 07:19:19.000000 gpt4free-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.274922 gpt4free-0.1.1/
+-rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.1/HISTORY.md
+-rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1536 2023-04-27 08:35:18.274922 gpt4free-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.158734 gpt4free-0.1.1/gpt4free/
+-rw-rw-rw-   0        0        0      136 2023-04-27 08:29:49.000000 gpt4free-0.1.1/gpt4free/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.171923 gpt4free-0.1.1/gpt4free/forefront/
+-rw-rw-rw-   0        0        0     5330 2023-04-27 08:09:30.000000 gpt4free-0.1.1/gpt4free/forefront/__init__.py
+-rw-rw-rw-   0        0        0     2147 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/forefront/mail.py
+-rw-rw-rw-   0        0        0     1795 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/forefront/typing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.173926 gpt4free-0.1.1/gpt4free/gui/
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:22:19.000000 gpt4free-0.1.1/gpt4free/gui/__init__.py
+-rw-rw-rw-   0        0        0     1535 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/gui/streamlit_app.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.176925 gpt4free-0.1.1/gpt4free/quora/
+-rw-rw-rw-   0        0        0    22029 2023-04-27 08:09:31.000000 gpt4free-0.1.1/gpt4free/quora/__init__.py
+-rw-rw-rw-   0        0        0    19819 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/quora/api.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.271955 gpt4free-0.1.1/gpt4free/quora/graphql/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/quora/graphql/__init__.py
+-rw-rw-rw-   0        0        0     2391 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/quora/mail.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.272921 gpt4free-0.1.1/gpt4free/theb/
+-rw-rw-rw-   0        0        0     1699 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/theb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.273921 gpt4free-0.1.1/gpt4free/you/
+-rw-rw-rw-   0        0        0     3716 2023-04-27 05:59:26.000000 gpt4free-0.1.1/gpt4free/you/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:18.167926 gpt4free-0.1.1/gpt4free.egg-info/
+-rw-rw-rw-   0        0        0     1536 2023-04-27 08:35:18.000000 gpt4free-0.1.1/gpt4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-27 08:35:18.000000 gpt4free-0.1.1/gpt4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:35:18.000000 gpt4free-0.1.1/gpt4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 08:35:17.000000 gpt4free-0.1.1/gpt4free.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      124 2023-04-27 08:35:18.000000 gpt4free-0.1.1/gpt4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 08:35:18.000000 gpt4free-0.1.1/gpt4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-04-27 08:35:18.275927 gpt4free-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2212 2023-04-27 08:35:03.000000 gpt4free-0.1.1/setup.py
```

### Comparing `gpt4free-0.1.0/CONTRIBUTING.md` & `gpt4free-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/LICENSE` & `gpt4free-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/PKG-INFO` & `gpt4free-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.0
+Version: 0.1.1
 Summary:  decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's ( poe.com, phind.com, chat.openai.com, writesonic.com, sqlchat.ai, t3nsor.com, you.com etc...)
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
@@ -21,12 +21,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
+decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's ( poe.com, phind.com, chat.openai.com, writesonic.com, sqlchat.ai, t3nsor.com, you.com etc...)
 
 
-
-## History
-
```

### Comparing `gpt4free-0.1.0/gpt4free/forefront/__init__.py` & `gpt4free-0.1.1/gpt4free/forefront/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-from json import loads
-from re import match
-from time import time, sleep
-from uuid import uuid4
-
-from requests import post
-from tls_client import Session
-
-from forefront.mail import Mail
-from forefront.typing import ForeFrontResponse
-
-
-class Account:
-    @staticmethod
-    def create(proxy=None, logging=False):
-
-        proxies = {
-            'http': 'http://' + proxy,
-            'https': 'http://' + proxy} if proxy else False
-
-        start = time()
-
-        mail = Mail(proxies)
-        mail_token = None
-        mail_adress = mail.get_mail()
-
-        # print(mail_adress)
-
-        client = Session(client_identifier='chrome110')
-        client.proxies = proxies
-        client.headers = {
-            "origin": "https://accounts.forefront.ai",
-            "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
-        }
-
-        response = client.post('https://clerk.forefront.ai/v1/client/sign_ups?_clerk_js_version=4.32.6',
-                               data={
-                                   "email_address": mail_adress
-                               }
-                               )
-
-        trace_token = response.json()['response']['id']
-        if logging: print(trace_token)
-
-        response = client.post(
-            f"https://clerk.forefront.ai/v1/client/sign_ups/{trace_token}/prepare_verification?_clerk_js_version=4.32.6",
-            data={
-                "strategy": "email_code",
-            }
-            )
-
-        if logging: print(response.text)
-
-        if not 'sign_up_attempt' in response.text:
-            return 'Failed to create account!'
-
-        while True:
-            sleep(1)
-            for _ in mail.fetch_inbox():
-                print(mail.get_message_content(_["id"]))
-                mail_token = match(r"(\d){5,6}", mail.get_message_content(_["id"])).group(0)
-
-            if mail_token:
-                break
-
-        if logging: print(mail_token)
-
-        response = client.post(
-            f'https://clerk.forefront.ai/v1/client/sign_ups/{trace_token}/attempt_verification?_clerk_js_version=4.38.4',
-            data={
-                'code': mail_token,
-                'strategy': 'email_code'
-            })
-
-        if logging: print(response.json())
-
-        token = response.json()['client']['sessions'][0]['last_active_token']['jwt']
-
-        with open('accounts.txt', 'a') as f:
-            f.write(f'{mail_adress}:{token}\n')
-
-        if logging: print(time() - start)
-
-        return token
-
-
-class StreamingCompletion:
-    @staticmethod
-    def create(
-            token=None,
-            chatId=None,
-            prompt='',
-            actionType='new',
-            defaultPersona='607e41fe-95be-497e-8e97-010a59b2e2c0',  # default
-            model='gpt-4') -> ForeFrontResponse:
-
-        if not token: raise Exception('Token is required!')
-        if not chatId: chatId = str(uuid4())
-
-        headers = {
-            'authority': 'chat-server.tenant-forefront-default.knative.chi.coreweave.com',
-            'accept': '*/*',
-            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
-            'authorization': 'Bearer ' + token,
-            'cache-control': 'no-cache',
-            'content-type': 'application/json',
-            'origin': 'https://chat.forefront.ai',
-            'pragma': 'no-cache',
-            'referer': 'https://chat.forefront.ai/',
-            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'cross-site',
-            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
-        }
-
-        json_data = {
-            'text': prompt,
-            'action': actionType,
-            'parentId': chatId,
-            'workspaceId': chatId,
-            'messagePersona': defaultPersona,
-            'model': model
-        }
-
-        for chunk in post('https://chat-server.tenant-forefront-default.knative.chi.coreweave.com/chat',
-                          headers=headers, json=json_data, stream=True).iter_lines():
-
-            if b'finish_reason":null' in chunk:
-                data = loads(chunk.decode('utf-8').split('data: ')[1])
-                token = data['choices'][0]['delta'].get('content')
-
-                if token != None:
-                    yield ForeFrontResponse({
-                        'id': chatId,
-                        'object': 'text_completion',
-                        'created': int(time()),
-                        'model': model,
-                        'choices': [{
-                            'text': token,
-                            'index': 0,
-                            'logprobs': None,
-                            'finish_reason': 'stop'
-                        }],
-                        'usage': {
-                            'prompt_tokens': len(prompt),
-                            'completion_tokens': len(token),
-                            'total_tokens': len(prompt) + len(token)
-                        }
-                    })
+from json import loads
+from re import match
+from time import time, sleep
+from uuid import uuid4
+
+from requests import post
+from tls_client import Session
+
+from gpt4free.forefront.mail import Mail
+from gpt4free.forefront.typing import ForeFrontResponse
+
+
+class Account:
+    @staticmethod
+    def create(proxy=None, logging=False):
+
+        proxies = {
+            'http': 'http://' + proxy,
+            'https': 'http://' + proxy} if proxy else False
+
+        start = time()
+
+        mail = Mail(proxies)
+        mail_token = None
+        mail_adress = mail.get_mail()
+
+        # print(mail_adress)
+
+        client = Session(client_identifier='chrome110')
+        client.proxies = proxies
+        client.headers = {
+            "origin": "https://accounts.forefront.ai",
+            "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
+        }
+
+        response = client.post('https://clerk.forefront.ai/v1/client/sign_ups?_clerk_js_version=4.32.6',
+                               data={
+                                   "email_address": mail_adress
+                               }
+                               )
+
+        trace_token = response.json()['response']['id']
+        if logging: print(trace_token)
+
+        response = client.post(
+            f"https://clerk.forefront.ai/v1/client/sign_ups/{trace_token}/prepare_verification?_clerk_js_version=4.32.6",
+            data={
+                "strategy": "email_code",
+            }
+            )
+
+        if logging: print(response.text)
+
+        if not 'sign_up_attempt' in response.text:
+            return 'Failed to create account!'
+
+        while True:
+            sleep(1)
+            for _ in mail.fetch_inbox():
+                print(mail.get_message_content(_["id"]))
+                mail_token = match(r"(\d){5,6}", mail.get_message_content(_["id"])).group(0)
+
+            if mail_token:
+                break
+
+        if logging: print(mail_token)
+
+        response = client.post(
+            f'https://clerk.forefront.ai/v1/client/sign_ups/{trace_token}/attempt_verification?_clerk_js_version=4.38.4',
+            data={
+                'code': mail_token,
+                'strategy': 'email_code'
+            })
+
+        if logging: print(response.json())
+
+        token = response.json()['client']['sessions'][0]['last_active_token']['jwt']
+
+        with open('accounts.txt', 'a') as f:
+            f.write(f'{mail_adress}:{token}\n')
+
+        if logging: print(time() - start)
+
+        return token
+
+
+class StreamingCompletion:
+    @staticmethod
+    def create(
+            token=None,
+            chatId=None,
+            prompt='',
+            actionType='new',
+            defaultPersona='607e41fe-95be-497e-8e97-010a59b2e2c0',  # default
+            model='gpt-4') -> ForeFrontResponse:
+
+        if not token: raise Exception('Token is required!')
+        if not chatId: chatId = str(uuid4())
+
+        headers = {
+            'authority': 'chat-server.tenant-forefront-default.knative.chi.coreweave.com',
+            'accept': '*/*',
+            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
+            'authorization': 'Bearer ' + token,
+            'cache-control': 'no-cache',
+            'content-type': 'application/json',
+            'origin': 'https://chat.forefront.ai',
+            'pragma': 'no-cache',
+            'referer': 'https://chat.forefront.ai/',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'cross-site',
+            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+        }
+
+        json_data = {
+            'text': prompt,
+            'action': actionType,
+            'parentId': chatId,
+            'workspaceId': chatId,
+            'messagePersona': defaultPersona,
+            'model': model
+        }
+
+        for chunk in post('https://chat-server.tenant-forefront-default.knative.chi.coreweave.com/chat',
+                          headers=headers, json=json_data, stream=True).iter_lines():
+
+            if b'finish_reason":null' in chunk:
+                data = loads(chunk.decode('utf-8').split('data: ')[1])
+                token = data['choices'][0]['delta'].get('content')
+
+                if token != None:
+                    yield ForeFrontResponse({
+                        'id': chatId,
+                        'object': 'text_completion',
+                        'created': int(time()),
+                        'model': model,
+                        'choices': [{
+                            'text': token,
+                            'index': 0,
+                            'logprobs': None,
+                            'finish_reason': 'stop'
+                        }],
+                        'usage': {
+                            'prompt_tokens': len(prompt),
+                            'completion_tokens': len(token),
+                            'total_tokens': len(prompt) + len(token)
+                        }
+                    })
```

### Comparing `gpt4free-0.1.0/gpt4free/forefront/mail.py` & `gpt4free-0.1.1/gpt4free/forefront/mail.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free/forefront/typing.py` & `gpt4free-0.1.1/gpt4free/forefront/typing.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free/quora/__init__.py` & `gpt4free-0.1.1/gpt4free/quora/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,495 +1,495 @@
-import json
-from datetime import datetime
-from hashlib import md5
-from json import dumps
-from pathlib import Path
-from random import choice, choices, randint
-from re import search, findall
-from string import ascii_letters, digits
-from typing import Optional, Union
-from urllib.parse import unquote
-
-import selenium.webdriver.support.expected_conditions as EC
-from fake_useragent import UserAgent
-from pypasser import reCaptchaV3
-from requests import Session
-from selenium.webdriver import Firefox, Chrome, FirefoxOptions, ChromeOptions
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.wait import WebDriverWait
-from tls_client import Session as TLS
-
-from quora.api import Client as PoeClient
-from quora.mail import Emailnator
-
-SELENIUM_WEB_DRIVER_ERROR_MSG = b'''The error message you are receiving is due to the `geckodriver` executable not 
-being found in your system\'s PATH. To resolve this issue, you need to download the geckodriver and add its location 
-to your system\'s PATH.\n\nHere are the steps to resolve the issue:\n\n1. Download the geckodriver for your platform 
-(Windows, macOS, or Linux) from the following link: https://github.com/mozilla/geckodriver/releases\n\n2. Extract the 
-downloaded archive and locate the geckodriver executable.\n\n3. Add the geckodriver executable to your system\'s 
-PATH.\n\nFor macOS and Linux:\n\n- Open a terminal window.\n- Move the geckodriver executable to a directory that is 
-already in your PATH, or create a new directory and add it to your PATH:\n\n```bash\n# Example: Move geckodriver to 
-/usr/local/bin\nmv /path/to/your/geckodriver /usr/local/bin\n```\n\n- If you created a new directory, add it to your 
-PATH:\n\n```bash\n# Example: Add a new directory to PATH\nexport PATH=$PATH:/path/to/your/directory\n```\n\nFor 
-Windows:\n\n- Right-click on "My Computer" or "This PC" and select "Properties".\n- Click on "Advanced system 
-settings".\n- Click on the "Environment Variables" button.\n- In the "System variables" section, find the "Path" 
-variable, select it, and click "Edit".\n- Click "New" and add the path to the directory containing the geckodriver 
-executable.\n\nAfter adding the geckodriver to your PATH, restart your terminal or command prompt and try running 
-your script again. The error should be resolved.'''
-
-# from twocaptcha import TwoCaptcha
-# solver = TwoCaptcha('72747bf24a9d89b4dcc1b24875efd358')
-
-MODELS = {
-    'Sage': 'capybara',
-    'GPT-4': 'beaver',
-    'Claude+': 'a2_2',
-    'Claude-instant': 'a2',
-    'ChatGPT': 'chinchilla',
-    'Dragonfly': 'nutria',
-    'NeevaAI': 'hutia',
-}
-
-
-def extract_formkey(html):
-    script_regex = r'<script>if\(.+\)throw new Error;(.+)</script>'
-    script_text = search(script_regex, html).group(1)
-    key_regex = r'var .="([0-9a-f]+)",'
-    key_text = search(key_regex, script_text).group(1)
-    cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
-    cipher_pairs = findall(cipher_regex, script_text)
-
-    formkey_list = [''] * len(cipher_pairs)
-    for pair in cipher_pairs:
-        formkey_index, key_index = map(int, pair)
-        formkey_list[formkey_index] = key_text[key_index]
-    formkey = ''.join(formkey_list)
-
-    return formkey
-
-
-class PoeResponse:
-    class Completion:
-        class Choices:
-            def __init__(self, choice: dict) -> None:
-                self.text = choice['text']
-                self.content = self.text.encode()
-                self.index = choice['index']
-                self.logprobs = choice['logprobs']
-                self.finish_reason = choice['finish_reason']
-
-            def __repr__(self) -> str:
-                return f'''<__main__.APIResponse.Completion.Choices(\n    text           = {self.text.encode()},\n    index          = {self.index},\n    logprobs       = {self.logprobs},\n    finish_reason  = {self.finish_reason})object at 0x1337>'''
-
-        def __init__(self, choices: dict) -> None:
-            self.choices = [self.Choices(choice) for choice in choices]
-
-    class Usage:
-        def __init__(self, usage_dict: dict) -> None:
-            self.prompt_tokens = usage_dict['prompt_tokens']
-            self.completion_tokens = usage_dict['completion_tokens']
-            self.total_tokens = usage_dict['total_tokens']
-
-        def __repr__(self):
-            return f'''<__main__.APIResponse.Usage(\n    prompt_tokens      = {self.prompt_tokens},\n    completion_tokens  = {self.completion_tokens},\n    total_tokens       = {self.total_tokens})object at 0x1337>'''
-
-    def __init__(self, response_dict: dict) -> None:
-        self.response_dict = response_dict
-        self.id = response_dict['id']
-        self.object = response_dict['object']
-        self.created = response_dict['created']
-        self.model = response_dict['model']
-        self.completion = self.Completion(response_dict['choices'])
-        self.usage = self.Usage(response_dict['usage'])
-
-    def json(self) -> dict:
-        return self.response_dict
-
-
-class ModelResponse:
-    def __init__(self, json_response: dict) -> None:
-        self.id = json_response['data']['poeBotCreate']['bot']['id']
-        self.name = json_response['data']['poeBotCreate']['bot']['displayName']
-        self.limit = json_response['data']['poeBotCreate']['bot']['messageLimit']['dailyLimit']
-        self.deleted = json_response['data']['poeBotCreate']['bot']['deletionState']
-
-
-class Model:
-    @staticmethod
-    def create(
-            token: str,
-            model: str = 'gpt-3.5-turbo',  # claude-instant
-            system_prompt: str = 'You are ChatGPT a large language model developed by Openai. Answer as consisely as possible',
-            description: str = 'gpt-3.5 language model from openai, skidded by poe.com',
-            handle: str = None,
-    ) -> ModelResponse:
-        models = {
-            'gpt-3.5-turbo': 'chinchilla',
-            'claude-instant-v1.0': 'a2',
-            'gpt-4': 'beaver',
-        }
-
-        if not handle:
-            handle = f'gptx{randint(1111111, 9999999)}'
-
-        client = Session()
-        client.cookies['p-b'] = token
-
-        formkey = extract_formkey(client.get('https://poe.com').text)
-        settings = client.get('https://poe.com/api/settings').json()
-
-        client.headers = {
-            'host': 'poe.com',
-            'origin': 'https://poe.com',
-            'referer': 'https://poe.com/',
-            'poe-formkey': formkey,
-            'poe-tchannel': settings['tchannelData']['channel'],
-            'user-agent': UserAgent().random,
-            'connection': 'keep-alive',
-            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'content-type': 'application/json',
-            'sec-fetch-site': 'same-origin',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-dest': 'empty',
-            'accept': '*/*',
-            'accept-encoding': 'gzip, deflate, br',
-            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
-        }
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'CreateBotMain_poeBotCreate_Mutation',
-                'variables': {
-                    'model': models[model],
-                    'handle': handle,
-                    'prompt': system_prompt,
-                    'isPromptPublic': True,
-                    'introduction': '',
-                    'description': description,
-                    'profilePictureUrl': 'https://qph.fs.quoracdn.net/main-qimg-24e0b480dcd946e1cc6728802c5128b6',
-                    'apiUrl': None,
-                    'apiKey': ''.join(choices(ascii_letters + digits, k=32)),
-                    'isApiBot': False,
-                    'hasLinkification': False,
-                    'hasMarkdownRendering': False,
-                    'hasSuggestedReplies': False,
-                    'isPrivateBot': False,
-                },
-                'query': 'mutation CreateBotMain_poeBotCreate_Mutation(\n  $model: String!\n  $handle: String!\n  $prompt: String!\n  $isPromptPublic: Boolean!\n  $introduction: String!\n  $description: String!\n  $profilePictureUrl: String\n  $apiUrl: String\n  $apiKey: String\n  $isApiBot: Boolean\n  $hasLinkification: Boolean\n  $hasMarkdownRendering: Boolean\n  $hasSuggestedReplies: Boolean\n  $isPrivateBot: Boolean\n) {\n  poeBotCreate(model: $model, handle: $handle, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {\n    status\n    bot {\n      id\n      ...BotHeader_bot\n    }\n  }\n}\n\nfragment BotHeader_bot on Bot {\n  displayName\n  messageLimit {\n    dailyLimit\n  }\n  ...BotImage_bot\n  ...BotLink_bot\n  ...IdAnnotation_node\n  ...botHelpers_useViewerCanAccessPrivateBot\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotImage_bot on Bot {\n  displayName\n  ...botHelpers_useDeletion_bot\n  ...BotImage_useProfileImage_bot\n}\n\nfragment BotImage_useProfileImage_bot on Bot {\n  image {\n    __typename\n    ... on LocalBotImage {\n      localName\n    }\n    ... on UrlBotImage {\n      url\n    }\n  }\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotLink_bot on Bot {\n  displayName\n}\n\nfragment IdAnnotation_node on Node {\n  __isNode: __typename\n  id\n}\n\nfragment botHelpers_useDeletion_bot on Bot {\n  deletionState\n}\n\nfragment botHelpers_useViewerCanAccessPrivateBot on Bot {\n  isPrivateBot\n  viewerIsCreator\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-
-        if 'success' not in response.text:
-            raise Exception(
-                '''
-                Bot creation Failed
-                !! Important !!
-                Bot creation was not enabled on this account
-                please use: quora.Account.create with enable_bot_creation set to True
-            '''
-            )
-
-        return ModelResponse(response.json())
-
-
-class Account:
-    @staticmethod
-    def create(
-            proxy: Optional[str] = None,
-            logging: bool = False,
-            enable_bot_creation: bool = False,
-    ):
-        client = TLS(client_identifier='chrome110')
-        client.proxies = {'http': f'http://{proxy}', 'https': f'http://{proxy}'} if proxy else None
-
-        mail_client = Emailnator()
-        mail_address = mail_client.get_mail()
-
-        if logging:
-            print('email', mail_address)
-
-        client.headers = {
-            'authority': 'poe.com',
-            'accept': '*/*',
-            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
-            'content-type': 'application/json',
-            'origin': 'https://poe.com',
-            'poe-tag-id': 'null',
-            'referer': 'https://poe.com/login',
-            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-origin',
-            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
-            'poe-formkey': extract_formkey(client.get('https://poe.com/login').text),
-            'poe-tchannel': client.get('https://poe.com/api/settings').json()['tchannelData']['channel'],
-        }
-
-        token = reCaptchaV3(
-            'https://www.recaptcha.net/recaptcha/enterprise/anchor?ar=1&k=6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG&co=aHR0cHM6Ly9wb2UuY29tOjQ0Mw..&hl=en&v=4PnKmGB9wRHh1i04o7YUICeI&size=invisible&cb=bi6ivxoskyal'
-        )
-        # token = solver.recaptcha(sitekey='6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG',
-        #     url        = 'https://poe.com/login?redirect_url=%2F',
-        #     version    = 'v3',
-        #     enterprise = 1,
-        #     invisible  = 1,
-        #     action     = 'login',)['code']
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'MainSignupLoginSection_sendVerificationCodeMutation_Mutation',
-                'variables': {
-                    'emailAddress': mail_address,
-                    'phoneNumber': None,
-                    'recaptchaToken': token,
-                },
-                'query': 'mutation MainSignupLoginSection_sendVerificationCodeMutation_Mutation(\n  $emailAddress: String\n  $phoneNumber: String\n  $recaptchaToken: String\n) {\n  sendVerificationCode(verificationReason: login, emailAddress: $emailAddress, phoneNumber: $phoneNumber, recaptchaToken: $recaptchaToken) {\n    status\n    errorMessage\n  }\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        print(dumps(client.headers, indent=4))
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-
-        if 'automated_request_detected' in response.text:
-            print('please try using a proxy / wait for fix')
-
-        if 'Bad Request' in response.text:
-            if logging:
-                print('bad request, retrying...', response.json())
-            quit()
-
-        if logging:
-            print('send_code', response.json())
-
-        mail_content = mail_client.get_message()
-        mail_token = findall(r';">(\d{6,7})</div>', mail_content)[0]
-
-        if logging:
-            print('code', mail_token)
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation',
-                'variables': {
-                    'verificationCode': str(mail_token),
-                    'emailAddress': mail_address,
-                    'phoneNumber': None,
-                },
-                'query': 'mutation SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation(\n  $verificationCode: String!\n  $emailAddress: String\n  $phoneNumber: String\n) {\n  signupWithVerificationCode(verificationCode: $verificationCode, emailAddress: $emailAddress, phoneNumber: $phoneNumber) {\n    status\n    errorMessage\n  }\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-        if logging:
-            print('verify_code', response.json())
-
-    def get(self):
-        cookies = open(Path(__file__).resolve().parent / 'cookies.txt', 'r').read().splitlines()
-        return choice(cookies)
-
-
-class StreamingCompletion:
-    @staticmethod
-    def create(
-            model: str = 'gpt-4',
-            custom_model: bool = None,
-            prompt: str = 'hello world',
-            token: str = '',
-    ):
-        _model = MODELS[model] if not custom_model else custom_model
-
-        client = PoeClient(token)
-
-        for chunk in client.send_message(_model, prompt):
-            yield PoeResponse(
-                {
-                    'id': chunk['messageId'],
-                    'object': 'text_completion',
-                    'created': chunk['creationTime'],
-                    'model': _model,
-                    'choices': [
-                        {
-                            'text': chunk['text_new'],
-                            'index': 0,
-                            'logprobs': None,
-                            'finish_reason': 'stop',
-                        }
-                    ],
-                    'usage': {
-                        'prompt_tokens': len(prompt),
-                        'completion_tokens': len(chunk['text_new']),
-                        'total_tokens': len(prompt) + len(chunk['text_new']),
-                    },
-                }
-            )
-
-
-class Completion:
-    def create(
-            model: str = 'gpt-4',
-            custom_model: str = None,
-            prompt: str = 'hello world',
-            token: str = '',
-    ):
-        models = {
-            'sage': 'capybara',
-            'gpt-4': 'beaver',
-            'claude-v1.2': 'a2_2',
-            'claude-instant-v1.0': 'a2',
-            'gpt-3.5-turbo': 'chinchilla',
-        }
-
-        _model = models[model] if not custom_model else custom_model
-
-        client = PoeClient(token)
-
-        for chunk in client.send_message(_model, prompt):
-            pass
-
-        return PoeResponse(
-            {
-                'id': chunk['messageId'],
-                'object': 'text_completion',
-                'created': chunk['creationTime'],
-                'model': _model,
-                'choices': [
-                    {
-                        'text': chunk['text'],
-                        'index': 0,
-                        'logprobs': None,
-                        'finish_reason': 'stop',
-                    }
-                ],
-                'usage': {
-                    'prompt_tokens': len(prompt),
-                    'completion_tokens': len(chunk['text']),
-                    'total_tokens': len(prompt) + len(chunk['text']),
-                },
-            }
-        )
-
-
-class Poe:
-    def __init__(
-            self,
-            model: str = 'ChatGPT',
-            driver: str = 'firefox',
-            download_driver: bool = False,
-            driver_path: Optional[str] = None,
-            cookie_path: str = './quora/cookie.json',
-    ):
-        # validating the model
-        if model and model not in MODELS:
-            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
-        self.model = MODELS[model]
-        self.cookie_path = cookie_path
-        self.cookie = self.__load_cookie(driver, download_driver, driver_path=driver_path)
-        self.client = PoeClient(self.cookie)
-
-    def __load_cookie(self, driver: str, download_driver: bool, driver_path: Optional[str] = None) -> str:
-        if (cookie_file := Path(self.cookie_path)).exists():
-            with cookie_file.open() as fp:
-                cookie = json.load(fp)
-                if datetime.fromtimestamp(cookie['expiry']) < datetime.now():
-                    cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
-                else:
-                    print('Loading the cookie from file')
-        else:
-            cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
-
-        return unquote(cookie['value'])
-
-    def __register_and_get_cookie(self, driver: str, driver_path: Optional[str] = None) -> dict:
-        mail_client = Emailnator()
-        mail_address = mail_client.get_mail()
-
-        driver = self.__resolve_driver(driver, driver_path=driver_path)
-        driver.get("https://www.poe.com")
-
-        # clicking use email button
-        driver.find_element(By.XPATH, '//button[contains(text(), "Use email")]').click()
-
-        email = WebDriverWait(driver, 30).until(EC.presence_of_element_located((By.XPATH, '//input[@type="email"]')))
-        email.send_keys(mail_address)
-        driver.find_element(By.XPATH, '//button[text()="Go"]').click()
-
-        code = findall(r';">(\d{6,7})</div>', mail_client.get_message())[0]
-        print(code)
-
-        verification_code = WebDriverWait(driver, 30).until(
-            EC.presence_of_element_located((By.XPATH, '//input[@placeholder="Code"]'))
-        )
-        verification_code.send_keys(code)
-        verify_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Verify"]'))
-        login_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Log In"]'))
-
-        WebDriverWait(driver, 30).until(EC.any_of(verify_button, login_button)).click()
-
-        cookie = driver.get_cookie('p-b')
-
-        with open(self.cookie_path, 'w') as fw:
-            json.dump(cookie, fw)
-
-        driver.close()
-        return cookie
-
-    @classmethod
-    def __resolve_driver(cls, driver: str, driver_path: Optional[str] = None) -> Union[Firefox, Chrome]:
-        options = FirefoxOptions() if driver == 'firefox' else ChromeOptions()
-        options.add_argument('-headless')
-
-        if driver_path:
-            options.binary_location = driver_path
-        try:
-            return Firefox(options=options) if driver == 'firefox' else Chrome(options=options)
-        except Exception:
-            raise Exception(SELENIUM_WEB_DRIVER_ERROR_MSG)
-
-    def chat(self, message: str, model: Optional[str] = None) -> str:
-        if model and model not in MODELS:
-            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
-        model = MODELS[model] if model else self.model
-        response = None
-        for chunk in self.client.send_message(model, message):
-            response = chunk['text']
-        return response
-
-    def create_bot(
-            self,
-            name: str,
-            /,
-            prompt: str = '',
-            base_model: str = 'ChatGPT',
-            description: str = '',
-    ) -> None:
-        if base_model not in MODELS:
-            raise RuntimeError('Sorry, the base_model you provided does not exist. Please check and try again.')
-
-        response = self.client.create_bot(
-            handle=name,
-            prompt=prompt,
-            base_model=MODELS[base_model],
-            description=description,
-        )
-        print(f'Successfully created bot with name: {response["bot"]["displayName"]}')
-
-    def list_bots(self) -> list:
-        return list(self.client.bot_names.values())
+import json
+from datetime import datetime
+from hashlib import md5
+from json import dumps
+from pathlib import Path
+from random import choice, choices, randint
+from re import search, findall
+from string import ascii_letters, digits
+from typing import Optional, Union
+from urllib.parse import unquote
+
+import selenium.webdriver.support.expected_conditions as EC
+from fake_useragent import UserAgent
+from pypasser import reCaptchaV3
+from requests import Session
+from selenium.webdriver import Firefox, Chrome, FirefoxOptions, ChromeOptions
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.wait import WebDriverWait
+from tls_client import Session as TLS
+
+from gpt4free.quora.api import Client as PoeClient
+from gpt4free.quora.mail import Emailnator
+
+SELENIUM_WEB_DRIVER_ERROR_MSG = b'''The error message you are receiving is due to the `geckodriver` executable not
+being found in your system\'s PATH. To resolve this issue, you need to download the geckodriver and add its location
+to your system\'s PATH.\n\nHere are the steps to resolve the issue:\n\n1. Download the geckodriver for your platform
+(Windows, macOS, or Linux) from the following link: https://github.com/mozilla/geckodriver/releases\n\n2. Extract the
+downloaded archive and locate the geckodriver executable.\n\n3. Add the geckodriver executable to your system\'s
+PATH.\n\nFor macOS and Linux:\n\n- Open a terminal window.\n- Move the geckodriver executable to a directory that is
+already in your PATH, or create a new directory and add it to your PATH:\n\n```bash\n# Example: Move geckodriver to
+/usr/local/bin\nmv /path/to/your/geckodriver /usr/local/bin\n```\n\n- If you created a new directory, add it to your
+PATH:\n\n```bash\n# Example: Add a new directory to PATH\nexport PATH=$PATH:/path/to/your/directory\n```\n\nFor
+Windows:\n\n- Right-click on "My Computer" or "This PC" and select "Properties".\n- Click on "Advanced system
+settings".\n- Click on the "Environment Variables" button.\n- In the "System variables" section, find the "Path"
+variable, select it, and click "Edit".\n- Click "New" and add the path to the directory containing the geckodriver
+executable.\n\nAfter adding the geckodriver to your PATH, restart your terminal or command prompt and try running
+your script again. The error should be resolved.'''
+
+# from twocaptcha import TwoCaptcha
+# solver = TwoCaptcha('72747bf24a9d89b4dcc1b24875efd358')
+
+MODELS = {
+    'Sage': 'capybara',
+    'GPT-4': 'beaver',
+    'Claude+': 'a2_2',
+    'Claude-instant': 'a2',
+    'ChatGPT': 'chinchilla',
+    'Dragonfly': 'nutria',
+    'NeevaAI': 'hutia',
+}
+
+
+def extract_formkey(html):
+    script_regex = r'<script>if\(.+\)throw new Error;(.+)</script>'
+    script_text = search(script_regex, html).group(1)
+    key_regex = r'var .="([0-9a-f]+)",'
+    key_text = search(key_regex, script_text).group(1)
+    cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
+    cipher_pairs = findall(cipher_regex, script_text)
+
+    formkey_list = [''] * len(cipher_pairs)
+    for pair in cipher_pairs:
+        formkey_index, key_index = map(int, pair)
+        formkey_list[formkey_index] = key_text[key_index]
+    formkey = ''.join(formkey_list)
+
+    return formkey
+
+
+class PoeResponse:
+    class Completion:
+        class Choices:
+            def __init__(self, choice: dict) -> None:
+                self.text = choice['text']
+                self.content = self.text.encode()
+                self.index = choice['index']
+                self.logprobs = choice['logprobs']
+                self.finish_reason = choice['finish_reason']
+
+            def __repr__(self) -> str:
+                return f'''<__main__.APIResponse.Completion.Choices(\n    text           = {self.text.encode()},\n    index          = {self.index},\n    logprobs       = {self.logprobs},\n    finish_reason  = {self.finish_reason})object at 0x1337>'''
+
+        def __init__(self, choices: dict) -> None:
+            self.choices = [self.Choices(choice) for choice in choices]
+
+    class Usage:
+        def __init__(self, usage_dict: dict) -> None:
+            self.prompt_tokens = usage_dict['prompt_tokens']
+            self.completion_tokens = usage_dict['completion_tokens']
+            self.total_tokens = usage_dict['total_tokens']
+
+        def __repr__(self):
+            return f'''<__main__.APIResponse.Usage(\n    prompt_tokens      = {self.prompt_tokens},\n    completion_tokens  = {self.completion_tokens},\n    total_tokens       = {self.total_tokens})object at 0x1337>'''
+
+    def __init__(self, response_dict: dict) -> None:
+        self.response_dict = response_dict
+        self.id = response_dict['id']
+        self.object = response_dict['object']
+        self.created = response_dict['created']
+        self.model = response_dict['model']
+        self.completion = self.Completion(response_dict['choices'])
+        self.usage = self.Usage(response_dict['usage'])
+
+    def json(self) -> dict:
+        return self.response_dict
+
+
+class ModelResponse:
+    def __init__(self, json_response: dict) -> None:
+        self.id = json_response['data']['poeBotCreate']['bot']['id']
+        self.name = json_response['data']['poeBotCreate']['bot']['displayName']
+        self.limit = json_response['data']['poeBotCreate']['bot']['messageLimit']['dailyLimit']
+        self.deleted = json_response['data']['poeBotCreate']['bot']['deletionState']
+
+
+class Model:
+    @staticmethod
+    def create(
+            token: str,
+            model: str = 'gpt-3.5-turbo',  # claude-instant
+            system_prompt: str = 'You are ChatGPT a large language model developed by Openai. Answer as consisely as possible',
+            description: str = 'gpt-3.5 language model from openai, skidded by poe.com',
+            handle: str = None,
+    ) -> ModelResponse:
+        models = {
+            'gpt-3.5-turbo': 'chinchilla',
+            'claude-instant-v1.0': 'a2',
+            'gpt-4': 'beaver',
+        }
+
+        if not handle:
+            handle = f'gptx{randint(1111111, 9999999)}'
+
+        client = Session()
+        client.cookies['p-b'] = token
+
+        formkey = extract_formkey(client.get('https://poe.com').text)
+        settings = client.get('https://poe.com/api/settings').json()
+
+        client.headers = {
+            'host': 'poe.com',
+            'origin': 'https://poe.com',
+            'referer': 'https://poe.com/',
+            'poe-formkey': formkey,
+            'poe-tchannel': settings['tchannelData']['channel'],
+            'user-agent': UserAgent().random,
+            'connection': 'keep-alive',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"',
+            'content-type': 'application/json',
+            'sec-fetch-site': 'same-origin',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-dest': 'empty',
+            'accept': '*/*',
+            'accept-encoding': 'gzip, deflate, br',
+            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
+        }
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'CreateBotMain_poeBotCreate_Mutation',
+                'variables': {
+                    'model': models[model],
+                    'handle': handle,
+                    'prompt': system_prompt,
+                    'isPromptPublic': True,
+                    'introduction': '',
+                    'description': description,
+                    'profilePictureUrl': 'https://qph.fs.quoracdn.net/main-qimg-24e0b480dcd946e1cc6728802c5128b6',
+                    'apiUrl': None,
+                    'apiKey': ''.join(choices(ascii_letters + digits, k=32)),
+                    'isApiBot': False,
+                    'hasLinkification': False,
+                    'hasMarkdownRendering': False,
+                    'hasSuggestedReplies': False,
+                    'isPrivateBot': False,
+                },
+                'query': 'mutation CreateBotMain_poeBotCreate_Mutation(\n  $model: String!\n  $handle: String!\n  $prompt: String!\n  $isPromptPublic: Boolean!\n  $introduction: String!\n  $description: String!\n  $profilePictureUrl: String\n  $apiUrl: String\n  $apiKey: String\n  $isApiBot: Boolean\n  $hasLinkification: Boolean\n  $hasMarkdownRendering: Boolean\n  $hasSuggestedReplies: Boolean\n  $isPrivateBot: Boolean\n) {\n  poeBotCreate(model: $model, handle: $handle, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {\n    status\n    bot {\n      id\n      ...BotHeader_bot\n    }\n  }\n}\n\nfragment BotHeader_bot on Bot {\n  displayName\n  messageLimit {\n    dailyLimit\n  }\n  ...BotImage_bot\n  ...BotLink_bot\n  ...IdAnnotation_node\n  ...botHelpers_useViewerCanAccessPrivateBot\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotImage_bot on Bot {\n  displayName\n  ...botHelpers_useDeletion_bot\n  ...BotImage_useProfileImage_bot\n}\n\nfragment BotImage_useProfileImage_bot on Bot {\n  image {\n    __typename\n    ... on LocalBotImage {\n      localName\n    }\n    ... on UrlBotImage {\n      url\n    }\n  }\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotLink_bot on Bot {\n  displayName\n}\n\nfragment IdAnnotation_node on Node {\n  __isNode: __typename\n  id\n}\n\nfragment botHelpers_useDeletion_bot on Bot {\n  deletionState\n}\n\nfragment botHelpers_useViewerCanAccessPrivateBot on Bot {\n  isPrivateBot\n  viewerIsCreator\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+
+        if 'success' not in response.text:
+            raise Exception(
+                '''
+                Bot creation Failed
+                !! Important !!
+                Bot creation was not enabled on this account
+                please use: quora.Account.create with enable_bot_creation set to True
+            '''
+            )
+
+        return ModelResponse(response.json())
+
+
+class Account:
+    @staticmethod
+    def create(
+            proxy: Optional[str] = None,
+            logging: bool = False,
+            enable_bot_creation: bool = False,
+    ):
+        client = TLS(client_identifier='chrome110')
+        client.proxies = {'http': f'http://{proxy}', 'https': f'http://{proxy}'} if proxy else None
+
+        mail_client = Emailnator()
+        mail_address = mail_client.get_mail()
+
+        if logging:
+            print('email', mail_address)
+
+        client.headers = {
+            'authority': 'poe.com',
+            'accept': '*/*',
+            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
+            'content-type': 'application/json',
+            'origin': 'https://poe.com',
+            'poe-tag-id': 'null',
+            'referer': 'https://poe.com/login',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'poe-formkey': extract_formkey(client.get('https://poe.com/login').text),
+            'poe-tchannel': client.get('https://poe.com/api/settings').json()['tchannelData']['channel'],
+        }
+
+        token = reCaptchaV3(
+            'https://www.recaptcha.net/recaptcha/enterprise/anchor?ar=1&k=6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG&co=aHR0cHM6Ly9wb2UuY29tOjQ0Mw..&hl=en&v=4PnKmGB9wRHh1i04o7YUICeI&size=invisible&cb=bi6ivxoskyal'
+        )
+        # token = solver.recaptcha(sitekey='6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG',
+        #     url        = 'https://poe.com/login?redirect_url=%2F',
+        #     version    = 'v3',
+        #     enterprise = 1,
+        #     invisible  = 1,
+        #     action     = 'login',)['code']
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'MainSignupLoginSection_sendVerificationCodeMutation_Mutation',
+                'variables': {
+                    'emailAddress': mail_address,
+                    'phoneNumber': None,
+                    'recaptchaToken': token,
+                },
+                'query': 'mutation MainSignupLoginSection_sendVerificationCodeMutation_Mutation(\n  $emailAddress: String\n  $phoneNumber: String\n  $recaptchaToken: String\n) {\n  sendVerificationCode(verificationReason: login, emailAddress: $emailAddress, phoneNumber: $phoneNumber, recaptchaToken: $recaptchaToken) {\n    status\n    errorMessage\n  }\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        print(dumps(client.headers, indent=4))
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+
+        if 'automated_request_detected' in response.text:
+            print('please try using a proxy / wait for fix')
+
+        if 'Bad Request' in response.text:
+            if logging:
+                print('bad request, retrying...', response.json())
+            quit()
+
+        if logging:
+            print('send_code', response.json())
+
+        mail_content = mail_client.get_message()
+        mail_token = findall(r';">(\d{6,7})</div>', mail_content)[0]
+
+        if logging:
+            print('code', mail_token)
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation',
+                'variables': {
+                    'verificationCode': str(mail_token),
+                    'emailAddress': mail_address,
+                    'phoneNumber': None,
+                },
+                'query': 'mutation SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation(\n  $verificationCode: String!\n  $emailAddress: String\n  $phoneNumber: String\n) {\n  signupWithVerificationCode(verificationCode: $verificationCode, emailAddress: $emailAddress, phoneNumber: $phoneNumber) {\n    status\n    errorMessage\n  }\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+        if logging:
+            print('verify_code', response.json())
+
+    def get(self):
+        cookies = open(Path(__file__).resolve().parent / 'cookies.txt', 'r').read().splitlines()
+        return choice(cookies)
+
+
+class StreamingCompletion:
+    @staticmethod
+    def create(
+            model: str = 'gpt-4',
+            custom_model: bool = None,
+            prompt: str = 'hello world',
+            token: str = '',
+    ):
+        _model = MODELS[model] if not custom_model else custom_model
+
+        client = PoeClient(token)
+
+        for chunk in client.send_message(_model, prompt):
+            yield PoeResponse(
+                {
+                    'id': chunk['messageId'],
+                    'object': 'text_completion',
+                    'created': chunk['creationTime'],
+                    'model': _model,
+                    'choices': [
+                        {
+                            'text': chunk['text_new'],
+                            'index': 0,
+                            'logprobs': None,
+                            'finish_reason': 'stop',
+                        }
+                    ],
+                    'usage': {
+                        'prompt_tokens': len(prompt),
+                        'completion_tokens': len(chunk['text_new']),
+                        'total_tokens': len(prompt) + len(chunk['text_new']),
+                    },
+                }
+            )
+
+
+class Completion:
+    def create(
+            model: str = 'gpt-4',
+            custom_model: str = None,
+            prompt: str = 'hello world',
+            token: str = '',
+    ):
+        models = {
+            'sage': 'capybara',
+            'gpt-4': 'beaver',
+            'claude-v1.2': 'a2_2',
+            'claude-instant-v1.0': 'a2',
+            'gpt-3.5-turbo': 'chinchilla',
+        }
+
+        _model = models[model] if not custom_model else custom_model
+
+        client = PoeClient(token)
+
+        for chunk in client.send_message(_model, prompt):
+            pass
+
+        return PoeResponse(
+            {
+                'id': chunk['messageId'],
+                'object': 'text_completion',
+                'created': chunk['creationTime'],
+                'model': _model,
+                'choices': [
+                    {
+                        'text': chunk['text'],
+                        'index': 0,
+                        'logprobs': None,
+                        'finish_reason': 'stop',
+                    }
+                ],
+                'usage': {
+                    'prompt_tokens': len(prompt),
+                    'completion_tokens': len(chunk['text']),
+                    'total_tokens': len(prompt) + len(chunk['text']),
+                },
+            }
+        )
+
+
+class Poe:
+    def __init__(
+            self,
+            model: str = 'ChatGPT',
+            driver: str = 'firefox',
+            download_driver: bool = False,
+            driver_path: Optional[str] = None,
+            cookie_path: str = './quora/cookie.json',
+    ):
+        # validating the model
+        if model and model not in MODELS:
+            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
+        self.model = MODELS[model]
+        self.cookie_path = cookie_path
+        self.cookie = self.__load_cookie(driver, download_driver, driver_path=driver_path)
+        self.client = PoeClient(self.cookie)
+
+    def __load_cookie(self, driver: str, download_driver: bool, driver_path: Optional[str] = None) -> str:
+        if (cookie_file := Path(self.cookie_path)).exists():
+            with cookie_file.open() as fp:
+                cookie = json.load(fp)
+                if datetime.fromtimestamp(cookie['expiry']) < datetime.now():
+                    cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
+                else:
+                    print('Loading the cookie from file')
+        else:
+            cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
+
+        return unquote(cookie['value'])
+
+    def __register_and_get_cookie(self, driver: str, driver_path: Optional[str] = None) -> dict:
+        mail_client = Emailnator()
+        mail_address = mail_client.get_mail()
+
+        driver = self.__resolve_driver(driver, driver_path=driver_path)
+        driver.get("https://www.poe.com")
+
+        # clicking use email button
+        driver.find_element(By.XPATH, '//button[contains(text(), "Use email")]').click()
+
+        email = WebDriverWait(driver, 30).until(EC.presence_of_element_located((By.XPATH, '//input[@type="email"]')))
+        email.send_keys(mail_address)
+        driver.find_element(By.XPATH, '//button[text()="Go"]').click()
+
+        code = findall(r';">(\d{6,7})</div>', mail_client.get_message())[0]
+        print(code)
+
+        verification_code = WebDriverWait(driver, 30).until(
+            EC.presence_of_element_located((By.XPATH, '//input[@placeholder="Code"]'))
+        )
+        verification_code.send_keys(code)
+        verify_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Verify"]'))
+        login_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Log In"]'))
+
+        WebDriverWait(driver, 30).until(EC.any_of(verify_button, login_button)).click()
+
+        cookie = driver.get_cookie('p-b')
+
+        with open(self.cookie_path, 'w') as fw:
+            json.dump(cookie, fw)
+
+        driver.close()
+        return cookie
+
+    @classmethod
+    def __resolve_driver(cls, driver: str, driver_path: Optional[str] = None) -> Union[Firefox, Chrome]:
+        options = FirefoxOptions() if driver == 'firefox' else ChromeOptions()
+        options.add_argument('-headless')
+
+        if driver_path:
+            options.binary_location = driver_path
+        try:
+            return Firefox(options=options) if driver == 'firefox' else Chrome(options=options)
+        except Exception:
+            raise Exception(SELENIUM_WEB_DRIVER_ERROR_MSG)
+
+    def chat(self, message: str, model: Optional[str] = None) -> str:
+        if model and model not in MODELS:
+            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
+        model = MODELS[model] if model else self.model
+        response = None
+        for chunk in self.client.send_message(model, message):
+            response = chunk['text']
+        return response
+
+    def create_bot(
+            self,
+            name: str,
+            /,
+            prompt: str = '',
+            base_model: str = 'ChatGPT',
+            description: str = '',
+    ) -> None:
+        if base_model not in MODELS:
+            raise RuntimeError('Sorry, the base_model you provided does not exist. Please check and try again.')
+
+        response = self.client.create_bot(
+            handle=name,
+            prompt=prompt,
+            base_model=MODELS[base_model],
+            description=description,
+        )
+        print(f'Successfully created bot with name: {response["bot"]["displayName"]}')
+
+    def list_bots(self) -> list:
+        return list(self.client.bot_names.values())
```

### Comparing `gpt4free-0.1.0/gpt4free/quora/api.py` & `gpt4free-0.1.1/gpt4free/quora/api.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free/quora/mail.py` & `gpt4free-0.1.1/gpt4free/quora/mail.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free/theb/__init__.py` & `gpt4free-0.1.1/gpt4free/theb/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free/you/__init__.py` & `gpt4free-0.1.1/gpt4free/you/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.0/gpt4free.egg-info/PKG-INFO` & `gpt4free-0.1.1/gpt4free.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.0
+Version: 0.1.1
 Summary:  decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's ( poe.com, phind.com, chat.openai.com, writesonic.com, sqlchat.ai, t3nsor.com, you.com etc...)
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
@@ -21,12 +21,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
+decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's ( poe.com, phind.com, chat.openai.com, writesonic.com, sqlchat.ai, t3nsor.com, you.com etc...)
 
 
-
-## History
-
```

### Comparing `gpt4free-0.1.0/gpt4free.egg-info/SOURCES.txt` & `gpt4free-0.1.1/gpt4free.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 gpt4free.egg-info/dependency_links.txt
 gpt4free.egg-info/not-zip-safe
 gpt4free.egg-info/requires.txt
 gpt4free.egg-info/top_level.txt
 gpt4free/forefront/__init__.py
 gpt4free/forefront/mail.py
 gpt4free/forefront/typing.py
+gpt4free/gui/__init__.py
+gpt4free/gui/streamlit_app.py
 gpt4free/quora/__init__.py
 gpt4free/quora/api.py
 gpt4free/quora/mail.py
 gpt4free/quora/graphql/__init__.py
 gpt4free/theb/__init__.py
-gpt4free/theb/theb_test.py
 gpt4free/you/__init__.py
```

### Comparing `gpt4free-0.1.0/setup.py` & `gpt4free-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         "Ai"
     ],
     name='gpt4free',
     packages=find_packages(include=['gpt4free', 'gpt4free.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rzashakeri/gpt4free',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
     project_urls={
         "Homepage": "https://github.com/rzashakeri/gpt4free",
         "Issue tracker": "https://github.com/rzashakeri/gpt4free/issues",
         "Release notes": "https://github.com/rzashakeri/gpt4free/releases",
         "Source": "https://github.com/rzashakeri/gpt4free",
         "Discussions": "https://github.com/rzashakeri/gpt4free/discussions",
```


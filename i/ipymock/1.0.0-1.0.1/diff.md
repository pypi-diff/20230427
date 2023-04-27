# Comparing `tmp/ipymock-1.0.0.tar.gz` & `tmp/ipymock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.0.0.tar", last modified: Mon Apr 24 01:56:16 2023, max compression
+gzip compressed data, was "ipymock-1.0.1.tar", last modified: Thu Apr 27 01:16:12 2023, max compression
```

## Comparing `ipymock-1.0.0.tar` & `ipymock-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.101354 ipymock-1.0.0/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.0/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.0/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-24 01:56:16.100237 ipymock-1.0.0/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-24 01:37:41.000000 ipymock-1.0.0/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.094857 ipymock-1.0.0/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1605 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     2306 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)    20991 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/agi.py
--rw-r--r--   0 saintway   (501) staff       (20)    11200 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/browser.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.098230 ipymock-1.0.0/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.099401 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      427 2023-04-24 01:56:16.000000 ipymock-1.0.0/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.0/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       62 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2519 2023-04-24 01:44:18.000000 ipymock-1.0.0/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-24 01:56:16.101551 ipymock-1.0.0/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.0/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.132060 ipymock-1.0.1/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.1/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.1/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-27 01:16:12.131773 ipymock-1.0.1/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-27 01:15:05.000000 ipymock-1.0.1/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.128148 ipymock-1.0.1/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1605 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     2405 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)    18088 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/agi.py
+-rw-r--r--   0 saintway   (501) staff       (20)    12854 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/browser.py
+-rw-r--r--   0 saintway   (501) staff       (20)      977 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/llm.py
+-rw-r--r--   0 saintway   (501) staff       (20)     2974 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.130286 ipymock-1.0.1/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.131154 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      460 2023-04-27 01:16:12.000000 ipymock-1.0.1/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.1/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       62 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2519 2023-04-27 01:14:32.000000 ipymock-1.0.1/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-27 01:16:12.132146 ipymock-1.0.1/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.1/setup.py
```

### Comparing `ipymock-1.0.0/LICENSE` & `ipymock-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.0/PKG-INFO` & `ipymock-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.0/README.md` & `ipymock-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.0/ipymock/__init__.py` & `ipymock-1.0.1/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.0/ipymock/_nbdev.py` & `ipymock-1.0.1/ipymock/_nbdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,46 +15,49 @@
          "rename_title": "2_browser.ipynb",
          "delete_conversation": "2_browser.ipynb",
          "recover_conversation": "2_browser.ipynb",
          "clear_conversations": "2_browser.ipynb",
          "attrdict": "2_browser.ipynb",
          "attributize": "2_browser.ipynb",
          "delta": "2_browser.ipynb",
-         "mock_create": "2_browser.ipynb",
+         "mock_create": "3_llm.ipynb",
          "chat_delta": "2_browser.ipynb",
          "mock_chat_create": "2_browser.ipynb",
          "mock_openai": "2_browser.ipynb",
          "embeddings_model": "4_agi.ipynb",
+         "mock_openai_embed": "3_llm.ipynb",
          "embedding_size": "4_agi.ipynb",
          "index": "4_agi.ipynb",
          "vectorstore": "4_agi.ipynb",
          "TaskCreationChain": "4_agi.ipynb",
          "TaskPrioritizationChain": "4_agi.ipynb",
          "ExecutionChain": "4_agi.ipynb",
          "get_next_task": "4_agi.ipynb",
          "prioritize_tasks": "4_agi.ipynb",
          "get_top_tasks": "4_agi.ipynb",
          "execute_task": "4_agi.ipynb",
          "BabyAGI": "4_agi.ipynb",
-         "DuckDuckGoSearchAPIWrapper": "4_agi.ipynb",
          "tools": "4_agi.ipynb",
          "ZeroRoundAgent": "4_agi.ipynb",
          "llm": "4_agi.ipynb",
          "FORMAT_INSTRUCTIONS": "4_agi.ipynb",
          "llm_chain": "4_agi.ipynb",
          "ChineseOutputParser": "4_agi.ipynb",
          "FINAL_ANSWER_ACTION": "4_agi.ipynb",
          "agent_executor": "4_agi.ipynb",
          "baby_agi": "4_agi.ipynb",
          "final_objective": "4_agi.ipynb",
          "test_baby_agi": "4_agi.ipynb",
-         "mock_baby_agi": "4_agi.ipynb"}
+         "mock_baby_agi": "4_agi.ipynb",
+         "DuckDuckGoSearchAPIWrapper": "4_tools_duckduckgo.ipynb"}
 
 modules = ["__init__.py",
            "browser.py",
-           "agi.py"]
+           "llm.py",
+           "agi.py",
+           "reader.py"]
 
 doc_url = "https://seii-saintway.github.io/ipymock/"
 
 git_url = "https://github.com/seii-saintway/ipymock/tree/main/"
 
 def custom_doc_links(name): return None
```

### Comparing `ipymock-1.0.0/ipymock/agi.py` & `ipymock-1.0.1/ipymock/agi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/4_agi.ipynb (unless otherwise specified).
 
-__all__ = ['BabyAGI', 'DuckDuckGoSearchAPIWrapper', 'tools', 'ZeroRoundAgent', 'llm', 'FORMAT_INSTRUCTIONS',
-           'llm_chain', 'ChineseOutputParser', 'FINAL_ANSWER_ACTION', 'agent_executor', 'baby_agi', 'common',
-           'mock_baby_agi']
+__all__ = ['BabyAGI', 'tools', 'ZeroRoundAgent', 'llm', 'FORMAT_INSTRUCTIONS', 'llm_chain', 'ChineseOutputParser',
+           'FINAL_ANSWER_ACTION', 'agent_executor', 'baby_agi', 'common', 'mock_baby_agi']
 
 # Internal Cell
 import time
 from collections import deque
 from typing import Dict, List, Optional, Any
 
 # Internal Cell
@@ -313,108 +312,17 @@
             task_prioritization_chain = task_prioritization_chain,
             execution_chain = execution_chain,
             vectorstore = vectorstore,
             **kwargs,
         )
 
 # Cell
-from typing import Dict, List, Optional
-
-from pydantic import BaseModel, Extra
-from pydantic.class_validators import root_validator
-
-
-class DuckDuckGoSearchAPIWrapper(BaseModel):
-    """Wrapper for DuckDuckGo Search API.
-
-    Free and does not require any setup
-    """
-
-    k: int = 10
-    region: Optional[str] = "wt-wt"
-    safesearch: str = "moderate"
-    time: Optional[str] = "y"
-    max_results: int = 5
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
-    @root_validator()
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that python package exists in environment."""
-        try:
-            from duckduckgo_search import ddg  # noqa: F401
-        except ImportError:
-            raise ValueError(
-                "Could not import duckduckgo-search python package. "
-                "Please install it with `pip install duckduckgo-search`."
-            )
-        return values
-
-    def run(self, query: str) -> str:
-        from duckduckgo_search import ddg
-
-        """Run query through DuckDuckGo and return results."""
-        results = ddg(
-            query,
-            region=self.region,
-            safesearch=self.safesearch,
-            time=self.time,
-            max_results=self.max_results,
-        )
-        if results is None or len(results) == 0:
-            return f'搜索「{query}」没有发现好的｛DuckDuckGo 搜索结果：{results}｝'
-        snippets = '\n'.join([result['body'] for result in results])
-        return (
-            f'用 DuckDuckGo 搜索「{query}」的结果：「\n'
-            f'{snippets}\n'
-            f'」'
-        )
-
-    def results(self, query: str, num_results: int) -> List[Dict]:
-        """Run query through DuckDuckGo and return metadata.
-
-        Args:
-            query: The query to search for.
-            num_results: The number of results to return.
-
-        Returns:
-            A list of dictionaries with the following keys:
-                snippet - The description of the result.
-                title - The title of the result.
-                link - The link to the result.
-        """
-        from duckduckgo_search import ddg
-
-        results = ddg(
-            query,
-            region=self.region,
-            safesearch=self.safesearch,
-            time=self.time,
-            max_results=num_results,
-        )
-
-        if results is None or len(results) == 0:
-            return [{"Result": f'No good {{DuckDuckGo Search Result: {results}}} was found for query: {query}'}]
-
-        def to_metadata(result: Dict) -> Dict:
-            return {
-                "snippet": result["body"],
-                "title": result["title"],
-                "link": result["href"],
-            }
-
-        return [to_metadata(result) for result in results]
-
-# Cell
 from langchain import OpenAI, LLMChain
-# from langchain.utilities.duckduckgo_search import DuckDuckGoSearchAPIWrapper
 from langchain.agents import Tool
+from .reader import DuckDuckGoSearchAPIWrapper
 
 tools = [
     Tool(
         name = '搜索',
         func = DuckDuckGoSearchAPIWrapper().run,
         description = (
             '如果你需要在互联网上搜索一些你所不确定的最新信息来回答相关问题，请回复：「\n'
```

### Comparing `ipymock-1.0.0/ipymock/browser.py` & `ipymock-1.0.1/ipymock/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,19 +116,23 @@
         if line.endswith(b'[DONE]'):
             common.conversation_done_channel.put(True)
             continue
 
         try:
             make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
         except json.decoder.JSONDecodeError as err:
-            sys.stderr.write(f'Error JSON Decoding: {line}\n')
+            sys.stderr.write(f'Error JSON Decoding: line = {line}\n')
             continue
         if make_conversation_response is None:
             continue
-        parts = make_conversation_response['message']['content']['parts']
+        try:
+            parts = make_conversation_response['message']['content']['parts']
+        except TypeError as err:
+            sys.stderr.write(f'TypeError: {err}\nline = {line}\n')
+            continue
         if len(parts) > 0:
             common.response_text_channel.put(parts[0])
             yield parts[0]
         if common.conversation_id == '':
             temp_conversation_id = make_conversation_response['conversation_id']
         common.parent_message_id = make_conversation_response['message']['id']
         if make_conversation_response['message']['end_turn'] == True:
@@ -197,14 +201,17 @@
 def clear_conversations():
     requests.patch(f'{common.chat_gpt_base_url}/conversations', headers = {'Authorization': common.access_token}, data = {'is_visible': False})
 
     common.conversation_id = ''
     common.parent_message_id = ''
     common.reload_conversations_channel.put(True)
 
+# Internal Cell
+import random, string
+
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
 def attributize(obj):
     '''Add attributes to a dictionary and its sub-dictionaries.'''
@@ -213,24 +220,28 @@
             obj[key] = attributize(obj[key])
         return attrdict(obj)
     if isinstance(obj, list):
         return [attributize(item) for item in obj]
     return obj
 
 def delta(prompt):
+    id = ''.join(
+        random.choices(string.ascii_letters + string.digits, k = 29)
+    )
     res = ''
     for response in start_conversation(prompt):
         yield attributize({
             'choices': [
                 {
                     'index': 0,
                     'logprobs': None,
                     'text': response[len(res):],
                 }
             ],
+            'id': f'cmpl-{id}',
         })
         res = response
 
 def mock_create(*args, **kwargs):
     prompts = []
     if isinstance(kwargs['prompt'], str):
         prompts = [kwargs['prompt']]
@@ -255,16 +266,16 @@
                     f'response = {repr(response)}\n'
                     f'Retrying...\n'
                 )
                 status_code = err.response.status_code
                 if status_code == 413:
                     # todo: split the prompt
                     break
-                if status_code == 429:
-                    break
+                # if status_code == 429:
+                #     break
                 if status_code >= 400 and status_code != 500:
                     time.sleep(wait_second)
                     wait_second *= 2
                     continue
                 break
             if response == '':
                 sys.stderr.write(
@@ -277,63 +288,107 @@
             break
         choices.append({
             'finish_reason': 'stop',
             'index': 0,
             'logprobs': None,
             'text': response,
         })
+    id = ''.join(
+        random.choices(string.ascii_letters + string.digits, k = 29)
+    )
     return attributize({
         'choices': choices,
+        'id': f'cmpl-{id}',
         'usage': {
             'completion_tokens': 0,
             'prompt_tokens': 0,
             'total_tokens': 0,
         },
     })
 
 def chat_delta(prompt):
+    id = ''.join(
+        random.choices(string.ascii_letters + string.digits, k = 29)
+    )
     res = ''
     for response in start_conversation(prompt):
         yield attributize({
             'choices': [
                 {
                     'index': 0,
                     'delta': {
                         'content': response[len(res):],
                     }
                 }
             ],
+            'id': f'chatcmpl-{id}',
         })
         res = response
 
 def mock_chat_create(*args, **kwargs):
     summarized_prompt = ''
     for message in kwargs['messages']:
         summarized_prompt += f"{message['role']}:\n\n{message['content']}\n\n\n"
     summarized_prompt.strip()
 
     if kwargs.get('stream', False):
         return chat_delta(summarized_prompt)
 
     response = ''
-    for response in start_conversation(summarized_prompt):
-        pass
-    if response == '':
-        sys.stderr.write(f'Error Responding: {repr(response)}\n')
+    wait_second = 1
+    while True:
+        try:
+            for response in start_conversation(summarized_prompt):
+                pass
+        except requests.exceptions.HTTPError as err:
+            sys.stderr.write(
+                f'{err}\n'
+                f'response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            status_code = err.response.status_code
+            if status_code == 413:
+                # todo: split the prompt
+                break
+            # if status_code == 429:
+            #     break
+            if status_code >= 400 and status_code != 500:
+                time.sleep(wait_second)
+                wait_second *= 2
+                continue
+            break
+        if response == '':
+            sys.stderr.write(
+                f'Error Responding: response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            time.sleep(wait_second)
+            wait_second *= 2
+            continue
+        break
+    id = ''.join(
+        random.choices(string.ascii_letters + string.digits, k = 29)
+    )
     return attributize({
         'choices': [
             {
                 'finish_reason': 'stop',
                 'index': 0,
                 'message': {
                     'content': response,
                     'role': 'assistant',
                 }
             }
         ],
+        'id': f'chatcmpl-{id}',
+        'usage': {
+            'completion_tokens': 0,
+            'prompt_tokens': 0,
+            'total_tokens': 0,
+        },
     })
 
 # Internal Cell
 import openai, pytest
 
 # Cell
 @pytest.fixture
```

### Comparing `ipymock-1.0.0/ipymock.egg-info/PKG-INFO` & `ipymock-1.0.1/ipymock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.0/settings.ini` & `ipymock-1.0.1/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 1.0.0
+version = 1.0.1
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-1.0.0/setup.py` & `ipymock-1.0.1/setup.py`

 * *Files identical despite different names*


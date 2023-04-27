# Comparing `tmp/one-api-tool-0.2.1.tar.gz` & `tmp/one-api-tool-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.1.tar", last modified: Wed Apr 26 10:10:41 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.2.tar", last modified: Thu Apr 27 11:29:21 2023, max compression
```

## Comparing `one-api-tool-0.2.1.tar` & `one-api-tool-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.144932 one-api-tool-0.2.1/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.1/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 10:10:41.144676 one-api-tool-0.2.1/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.1/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.141544 one-api-tool-0.2.1/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      490 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       67 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.142301 one-api-tool-0.2.1/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.1/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.143553 one-api-tool-0.2.1/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.1/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1569 2023-04-26 09:30:39.000000 one-api-tool-0.2.1/oneapi/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1300 2023-04-26 10:05:38.000000 one-api-tool-0.2.1/oneapi/commands/one_api_eval_one.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1108 2023-04-26 09:25:26.000000 one-api-tool-0.2.1/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6162 2023-04-26 09:02:32.000000 one-api-tool-0.2.1/oneapi/one_ai_eval.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9519 2023-04-26 08:55:00.000000 one-api-tool-0.2.1/oneapi/one_api.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.144308 one-api-tool-0.2.1/oneapi/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-26 09:01:28.000000 one-api-tool-0.2.1/oneapi/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2540 2023-04-26 04:21:33.000000 one-api-tool-0.2.1/oneapi/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-26 10:10:41.145034 one-api-tool-0.2.1/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1184 2023-04-26 10:10:00.000000 one-api-tool-0.2.1/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.553032 one-api-tool-0.2.2/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.2/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:29:21.552875 one-api-tool-0.2.2/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.2/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.549750 one-api-tool-0.2.2/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      560 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.550373 one-api-tool-0.2.2/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.2/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.551392 one-api-tool-0.2.2/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.2/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.2/oneapi/commands/one_api_eval_file.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.2/oneapi/commands/one_api_eval_one.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.2/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6668 2023-04-27 11:29:05.000000 one-api-tool-0.2.2/oneapi/one_ai_eval.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.2/oneapi/one_api.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.551893 one-api-tool-0.2.2/oneapi/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.2/oneapi/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5614 2023-04-27 09:51:38.000000 one-api-tool-0.2.2/oneapi/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.552501 one-api-tool-0.2.2/oneapi/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.2/oneapi/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2657 2023-04-27 02:20:51.000000 one-api-tool-0.2.2/oneapi/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 11:29:21.553078 one-api-tool-0.2.2/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1245 2023-04-27 11:26:59.000000 one-api-tool-0.2.2/setup.py
```

### Comparing `one-api-tool-0.2.1/LICENSE` & `one-api-tool-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.1/PKG-INFO` & `one-api-tool-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.1/README.md` & `one-api-tool-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.1/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.2/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.1/oneapi/one_api.py` & `one-api-tool-0.2.2/oneapi/one_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,14 @@
     def simple_chat(self, prompt, model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
             msgs = [ChatGPTMessage(role="user", content=prompt)]
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
-        elif isinstance(self.tool.method, ClaudeMethod):
+        elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"\n\nHuman: {prompt}\n\nAssistant:", model=model if model else "claude-v1.3", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
```

### Comparing `one-api-tool-0.2.1/oneapi/utils/data_utils.py` & `one-api-tool-0.2.2/oneapi/utils/data_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         return json_dicts
     else:
         single_dict = {}
         for dict_obj in json_dicts:
             single_dict.update(dict_obj)
         return single_dict
 
+def extract_numbers(text):
+    numbers = re.findall(r'\d+', text)
+    numbers = [int(number) for number in numbers]
+
 
 def df2xlsx(df: pd.DataFrame, save_path: str, sheet_name='Sheet1', mode='w', index=False):
     if mode not in ['w', 'a']:
         raise AssertionError('mode not in [\'w\', \'a\']')
     if mode == 'a' and not os.path.isfile(save_path):
         mode = 'w'
     if mode == 'a':
```

### Comparing `one-api-tool-0.2.1/setup.py` & `one-api-tool-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
         "httpx",
         "aiohttp",
         "tokenizers",
         "pandas",
+        "openpyxl",
+        "tabulate",
+        "XlsxWriter"
     ],
     entry_points={
         "console_scripts": [
             "one-eval-file=oneapi.commands.one_api_eval_file:main",
             "one-eval-line=oneapi.commands.one_api_eval_one:main",
             "one-api=oneapi.commands.one_api_requst:main"
         ]
```


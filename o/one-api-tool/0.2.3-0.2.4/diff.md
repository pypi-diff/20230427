# Comparing `tmp/one-api-tool-0.2.3.tar.gz` & `tmp/one-api-tool-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.3.tar", last modified: Thu Apr 27 11:36:51 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.4.tar", last modified: Thu Apr 27 12:27:39 2023, max compression
```

## Comparing `one-api-tool-0.2.3.tar` & `one-api-tool-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.165367 one-api-tool-0.2.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:36:51.165185 one-api-tool-0.2.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.160107 one-api-tool-0.2.3/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      609 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.160853 one-api-tool-0.2.3/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.3/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.162036 one-api-tool-0.2.3/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.3/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.3/oneapi/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.3/oneapi/commands/one_api_eval_one.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.3/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6668 2023-04-27 11:29:05.000000 one-api-tool-0.2.3/oneapi/one_ai_eval.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.3/oneapi/one_api.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.163661 one-api-tool-0.2.3/oneapi/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.3/oneapi/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      858 2023-04-27 11:27:56.000000 one-api-tool-0.2.3/oneapi/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     5614 2023-04-27 09:51:38.000000 one-api-tool-0.2.3/oneapi/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.164819 one-api-tool-0.2.3/oneapi/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.3/oneapi/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2657 2023-04-27 02:20:51.000000 one-api-tool-0.2.3/oneapi/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 11:36:51.165413 one-api-tool-0.2.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1334 2023-04-27 11:36:50.000000 one-api-tool-0.2.3/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.220177 one-api-tool-0.2.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 12:27:39.220000 one-api-tool-0.2.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.216596 one-api-tool-0.2.4/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      609 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 12:27:39.000000 one-api-tool-0.2.4/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.217151 one-api-tool-0.2.4/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.4/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.218126 one-api-tool-0.2.4/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.4/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.4/oneapi/commands/one_api_eval_file.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.4/oneapi/commands/one_api_eval_one.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.4/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6714 2023-04-27 12:27:19.000000 one-api-tool-0.2.4/oneapi/one_ai_eval.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.4/oneapi/one_api.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.218993 one-api-tool-0.2.4/oneapi/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.4/oneapi/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      858 2023-04-27 11:27:56.000000 one-api-tool-0.2.4/oneapi/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5651 2023-04-27 12:02:51.000000 one-api-tool-0.2.4/oneapi/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:27:39.219658 one-api-tool-0.2.4/oneapi/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.4/oneapi/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2819 2023-04-27 11:59:07.000000 one-api-tool-0.2.4/oneapi/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 12:27:39.220230 one-api-tool-0.2.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1334 2023-04-27 12:27:31.000000 one-api-tool-0.2.4/setup.py
```

### Comparing `one-api-tool-0.2.3/LICENSE` & `one-api-tool-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/PKG-INFO` & `one-api-tool-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.3/README.md` & `one-api-tool-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.4/one_api_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.3/one_api_tool.egg-info/SOURCES.txt` & `one-api-tool-0.2.4/one_api_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/commands/one_api_eval_file.py` & `one-api-tool-0.2.4/oneapi/commands/one_api_eval_file.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/commands/one_api_eval_one.py` & `one-api-tool-0.2.4/oneapi/commands/one_api_eval_one.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.4/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/one_ai_eval.py` & `one-api-tool-0.2.4/oneapi/one_ai_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,22 +96,23 @@
         sample_keys = random.sample(grouped.groups.keys(), sample_num)
     else:
         sample_keys = grouped.groups.keys()
     return [grouped.get_group(key) for key in sample_keys]
 
 def log_score_results(eval_results_df: pd.DataFrame):
     if 'model' in eval_results_df.keys():
-        score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').to_markdown()
+        print( eval_results_df.groupby('model')['score'])
+        score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}')
         print(f'{"-"*20} SCORE BY MODEL {"-"*20}\n{score_models.to_markdown()}')
         if 'category' in eval_results_df.keys():
             score_category = eval_results_df.groupby([
                 'model', 'category'
             ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by='model')
             print(
-                f'{"-"*20} SCORE BY CATEGORY {"-"*20}\n{score_category.to_markdown(index=False)}'
+                f'\n{"-"*20} SCORE BY CATEGORY {"-"*20}\n{score_category.to_markdown(index=False)}'
             )
 
 def save_results(eval_results_df: pd.DataFrame, output_path: str):
     print(f'Saving score result: {output_path}')
     df_saver(eval_results_df, output_path)
     print(f'Saved successfully.')
```

### Comparing `one-api-tool-0.2.3/oneapi/one_api.py` & `one-api-tool-0.2.4/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/prompt_template/eval_prompt_template.json` & `one-api-tool-0.2.4/oneapi/prompt_template/eval_prompt_template.json`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.3/oneapi/prompt_template/prompter.py` & `one-api-tool-0.2.4/oneapi/prompt_template/prompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import List
 import abc
 import json
 sys.path.append(
     os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/../../"))
-from oneapi.utils.data_utils import load_json, generate_letters, extract_all_json, extract_numbers
+from oneapi.utils.data_utils import load_json, generate_letters, extract_last_json, extract_numbers
 
 
 class Prompter(abc.ABC):
     @abc.abstractmethod
     def generate_prompt(**kwargs):
         raise NotImplementedError
     
@@ -39,15 +39,15 @@
             'eval_without_target_instruction', '')
         score_output_type = template_data.get('score_output_type', 'json')
         response_score_position = template_data.get('response_score_position',
                                                     'tail')
 
         instruction_header = template_data.get('header', '')
         if verbose:
-            print(f'Using prompt templat: {json.dumps(template_data, sort_keys=True, indent=2)}')
+            print(f'Using prompt templat:\n {json.dumps(template_data, sort_keys=True, indent=2)}')
         return cls(eval_with_target_template, eval_without_target_template,
                    eval_with_target_instruction,
                    eval_without_target_instruction, score_output_type,
                    response_score_position, instruction_header, verbose)
 
     def __init__(self,
                  eval_with_target_template: str,
@@ -109,13 +109,13 @@
         Extract the result (scores) from the given model response.
         """
         if self._verbose:
             print(
                 f"{'-'*20} response detail ⭐️ {'-'*20}\n\n{response}\n\n{'-'*20} response end {'-'*20}\n"
             )
         if self.score_output_type == 'json':
-            result_json = extract_all_json(response)
-            scores = list(result_json.values())
+            result_json = extract_last_json(response.strip())
+            scores = list(map(lambda x: float(x), result_json.values()))
         elif self.score_output_type == 'list':
             score_positon = 0 if self.response_score_position == 'head' else -1
             scores = extract_numbers(response.split('\n')[score_positon])
         return scores
```

### Comparing `one-api-tool-0.2.3/oneapi/utils/data_utils.py` & `one-api-tool-0.2.4/oneapi/utils/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,22 @@
         return json_dicts
     else:
         single_dict = {}
         for dict_obj in json_dicts:
             single_dict.update(dict_obj)
         return single_dict
 
+def extract_last_json(text) -> dict:
+    json_str = re.search(r'\{[^}]*\}(?=[^{}]*$)', text).group()
+    json_data = json.loads(json_str)
+    return json_data
+
 def extract_numbers(text):
     numbers = re.findall(r'\d+', text)
-    numbers = [int(number) for number in numbers]
+    numbers = [float(number) for number in numbers]
 
 
 def df2xlsx(df: pd.DataFrame, save_path: str, sheet_name='Sheet1', mode='w', index=False):
     if mode not in ['w', 'a']:
         raise AssertionError('mode not in [\'w\', \'a\']')
     if mode == 'a' and not os.path.isfile(save_path):
         mode = 'w'
```

### Comparing `one-api-tool-0.2.3/setup.py` & `one-api-tool-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     package_data={
       "oneapi":["prompt_template/eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
```


# Comparing `tmp/pandasai-0.0.2.tar.gz` & `tmp/pandasai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.0.2.tar", last modified: Mon Apr 24 13:46:57 2023, max compression
+gzip compressed data, was "pandasai-0.0.3.tar", last modified: Thu Apr 27 09:19:18 2023, max compression
```

## Comparing `pandasai-0.0.2.tar` & `pandasai-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:57.007606 pandasai-0.0.2/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1055 2023-04-24 05:55:05.000000 pandasai-0.0.2/LICENSE
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)       28 2023-04-24 09:50:53.000000 pandasai-0.0.2/MANIFEST.in
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2362 2023-04-24 13:46:57.007453 pandasai-0.0.2/PKG-INFO
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1981 2023-04-24 13:46:06.000000 pandasai-0.0.2/README.md
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:56.999134 pandasai-0.0.2/pandasai/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2375 2023-04-24 13:38:36.000000 pandasai-0.0.2/pandasai/__init__.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:57.000944 pandasai-0.0.2/pandasai/__pycache__/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2308 2023-04-24 13:38:51.000000 pandasai-0.0.2/pandasai/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:57.003456 pandasai-0.0.2/pandasai/llm/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 11:19:15.000000 pandasai-0.0.2/pandasai/llm/__init__.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:57.007155 pandasai-0.0.2/pandasai/llm/__pycache__/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      160 2023-04-24 11:19:33.000000 pandasai-0.0.2/pandasai/llm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1416 2023-04-24 13:43:31.000000 pandasai-0.0.2/pandasai/llm/__pycache__/alpaca.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2384 2023-04-24 13:35:04.000000 pandasai-0.0.2/pandasai/llm/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      903 2023-04-24 12:44:16.000000 pandasai-0.0.2/pandasai/llm/__pycache__/fake.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1579 2023-04-22 21:09:53.000000 pandasai-0.0.2/pandasai/llm/__pycache__/open_assistant.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2502 2023-04-24 13:38:51.000000 pandasai-0.0.2/pandasai/llm/__pycache__/openai.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1065 2023-04-24 13:43:47.000000 pandasai-0.0.2/pandasai/llm/alpaca.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1827 2023-04-24 13:34:54.000000 pandasai-0.0.2/pandasai/llm/base.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      300 2023-04-24 13:34:20.000000 pandasai-0.0.2/pandasai/llm/fake.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      907 2023-04-24 13:34:14.000000 pandasai-0.0.2/pandasai/llm/open_assistant.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2533 2023-04-24 13:38:49.000000 pandasai-0.0.2/pandasai/llm/openai.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 13:46:57.000443 pandasai-0.0.2/pandasai.egg-info/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2362 2023-04-24 13:46:56.000000 pandasai-0.0.2/pandasai.egg-info/PKG-INFO
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      664 2023-04-24 13:46:56.000000 pandasai-0.0.2/pandasai.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        1 2023-04-24 13:46:56.000000 pandasai-0.0.2/pandasai.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        9 2023-04-24 13:46:56.000000 pandasai-0.0.2/pandasai.egg-info/top_level.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)       38 2023-04-24 13:46:57.007652 pandasai-0.0.2/setup.cfg
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      626 2023-04-24 13:46:47.000000 pandasai-0.0.2/setup.py
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.641090 pandasai-0.0.3/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1055 2023-04-24 05:55:05.000000 pandasai-0.0.3/LICENSE
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)       28 2023-04-24 09:50:53.000000 pandasai-0.0.3/MANIFEST.in
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3144 2023-04-27 09:19:18.640906 pandasai-0.0.3/PKG-INFO
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2763 2023-04-27 09:18:21.000000 pandasai-0.0.3/README.md
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.635156 pandasai-0.0.3/pandasai/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2982 2023-04-27 09:09:37.000000 pandasai-0.0.3/pandasai/__init__.py
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.636325 pandasai-0.0.3/pandasai/__pycache__/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2660 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3017 2023-04-27 09:14:30.000000 pandasai-0.0.3/pandasai/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.637782 pandasai-0.0.3/pandasai/llm/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 11:19:15.000000 pandasai-0.0.3/pandasai/llm/__init__.py
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.640469 pandasai-0.0.3/pandasai/llm/__pycache__/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      160 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/llm/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      160 2023-04-24 11:19:33.000000 pandasai-0.0.3/pandasai/llm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1416 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/llm/__pycache__/alpaca.cpython-38.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1416 2023-04-24 21:08:19.000000 pandasai-0.0.3/pandasai/llm/__pycache__/alpaca.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2353 2023-04-24 20:56:38.000000 pandasai-0.0.3/pandasai/llm/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2380 2023-04-24 21:08:19.000000 pandasai-0.0.3/pandasai/llm/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      903 2023-04-24 12:44:16.000000 pandasai-0.0.3/pandasai/llm/__pycache__/fake.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1547 2023-04-26 21:59:03.000000 pandasai-0.0.3/pandasai/llm/__pycache__/open_assistant.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2502 2023-04-24 22:45:27.000000 pandasai-0.0.3/pandasai/llm/__pycache__/openai.cpython-39.pyc
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1065 2023-04-24 13:43:47.000000 pandasai-0.0.3/pandasai/llm/alpaca.py
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1760 2023-04-24 21:08:02.000000 pandasai-0.0.3/pandasai/llm/base.py
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      300 2023-04-24 13:34:20.000000 pandasai-0.0.3/pandasai/llm/fake.py
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      907 2023-04-24 13:34:14.000000 pandasai-0.0.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2533 2023-04-24 22:45:22.000000 pandasai-0.0.3/pandasai/llm/openai.py
+drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.635935 pandasai-0.0.3/pandasai.egg-info/
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3144 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      850 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)        1 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)        9 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/top_level.txt
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)       38 2023-04-27 09:19:18.641143 pandasai-0.0.3/setup.cfg
+-rw-r--r--   0 gabrieleventuri   (501) staff       (20)      626 2023-04-27 09:18:57.000000 pandasai-0.0.3/setup.py
```

### Comparing `pandasai-0.0.2/LICENSE` & `pandasai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.2/PKG-INFO` & `pandasai-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper around pandas to make it conversational
 Author: Gabriele Venturi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -63,19 +63,44 @@
 
 The above code will return the following:
 
 ```
 14516000
 ```
 
+You can find more examples in the [examples](examples) directory.
+
+## Environment Variables
+
+In order to set the API key for the LLM (HuggingFaceHub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
+
+```bash
+cp .env.example .env
+```
+
+Then, edit the `.env` file and set the appropriate values.
+
+As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
+
+```python
+# OpenAI
+llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
+
+# OpenAssistant
+llm = OpenAssistant(api_token="YOUR_HF_API_KEY")
+```
+
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
-Contributions are welcome!
+Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 
 ### Todo
 
 - [ ] Add support for more LLMs
+- [ ] Make PandasAI available from a CLI
+- [ ] Create a web interface for PandasAI
+- [ ] Add CI/CD
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.0.2/README.md` & `pandasai-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -50,19 +50,44 @@
 
 The above code will return the following:
 
 ```
 14516000
 ```
 
+You can find more examples in the [examples](examples) directory.
+
+## Environment Variables
+
+In order to set the API key for the LLM (HuggingFaceHub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
+
+```bash
+cp .env.example .env
+```
+
+Then, edit the `.env` file and set the appropriate values.
+
+As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
+
+```python
+# OpenAI
+llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
+
+# OpenAssistant
+llm = OpenAssistant(api_token="YOUR_HF_API_KEY")
+```
+
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
-Contributions are welcome!
+Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 
 ### Todo
 
 - [ ] Add support for more LLMs
+- [ ] Make PandasAI available from a CLI
+- [ ] Create a web interface for PandasAI
+- [ ] Add CI/CD
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.0.2/pandasai/__init__.py` & `pandasai-0.0.3/pandasai/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,54 +2,67 @@
 from .llm.base import LLM
 import io
 import sys
 
 class PandasAI:
   """PandasAI is a wrapper around a LLM to make dataframes convesational"""
 
-  task_instruction: str = """
+  _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
 This is the result of `print(df.head())`:
-{df}.
+{df_head}.
 
 Return the python code (do not import anything) to get the answer to the following question:
 """
-  response_instruction: str = """
-The customer asked:
-{question}
+  _response_instruction: str = """
+Question: {question}
+Answer: {answer}
 
-To get the answer, run you run the following code in pandas (python):
-{code}
-
-Result:
-{answer}
-
-Write the answer to the customer
+Rewrite the answer to the question in a conversational way.
 """
-  llm: LLM
-  conversational_answer: bool
+  _llm: LLM
+  _verbose: bool = False
+  _is_conversational_answer: bool = True
+  last_code_generated: str = None
+  code_output: str = None
 
-  # default constructor
-  def __init__(self, llm = None, conversational_answer = True):
+  def __init__(self, llm = None, conversational = True, verbose = False):
     if llm is None:
       raise Exception("An LLM should be provided to instantiate a PandasAI instance")
-    self.llm = llm
-    self.conversational_answer = conversational_answer
+    self._llm = llm
+    self._is_conversational_answer = conversational
+    self._verbose = verbose
+
+  def conversational_answer(self, question: str, code: str, answer: str) -> str:
+    """Return the conversational answer"""
+    instruction = self._response_instruction.format(question = question, code = code, answer = answer)
+    return self._llm.call(instruction, answer)
 
-  def run(self, df: pd.DataFrame, prompt: str, conversational_answer: bool = None) -> str:
+  def run(self, df: pd.DataFrame, prompt: str, is_conversational_answer: bool = None) -> str:
     """Run the LLM with the given prompt"""
-    print(f"Running PandasAI with {self.llm._type} LLM...")
-    code = self.llm.generate_code(self.task_instruction.format(df = df.head()), prompt)
+    self.log(f"Running PandasAI with {self._llm._type} LLM...")
+
+    code = self._llm.generate_code(self._task_instruction.format(df_head = df.head()), prompt)
+    self.last_code_generated = code
+    self.log(f"""
+Code generated:
+```
+{code}
+```""")
+
     answer = self.run_code(code, df)
+    self.code_output = answer
+    self.log(f"Answer: {answer}")
 
-    if conversational_answer is None:
-      conversational_answer = self.conversational_answer
-    if conversational_answer:
-      return self.llm.call(self.response_instruction.format(question = prompt, code = code, answer = answer), answer)
+    if is_conversational_answer is None:
+      is_conversational_answer = self._is_conversational_answer
+    if is_conversational_answer:
+      answer = self.conversational_answer(prompt, code, answer)
+      self.log(f"Conversational answer: {answer}")
     return answer
 
   def run_code(self, code: str, df: pd.DataFrame):
     """Run the code in the current context and return the result"""
 
     # Redirect standard output to a StringIO buffer
     output = io.StringIO()
@@ -62,16 +75,21 @@
     sys.stdout = sys.__stdout__
     captured_output = output.getvalue()
 
     # Evaluate the last line and return its value or the captured output
     lines = code.strip().split('\n')
     last_line = lines[-1].strip()
     if last_line.startswith('print(') and last_line.endswith(')'):
-      # last line is already printing
+      # Last line is already printing
       return eval(last_line[6:-1])
     else:
-      # evaluate last line and return its value or the captured output
+      # Evaluate last line and return its value or the captured output
       try:
         result = eval(last_line)
         return result
       except:
-        return captured_output
+        return captured_output
+
+  def log(self, message: str):
+    """Log a message"""
+    if self._verbose:
+      print(message)
```

### Comparing `pandasai-0.0.2/pandasai/__pycache__/__init__.cpython-39.pyc` & `pandasai-0.0.3/pandasai/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 13:38:36 2023 UTC, .py size: 2375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,167 @@
-00000000: 610d 0d0a 0000 0000 5c86 4664 4709 0000  a.......\.FdG...
+00000000: 550d 0d0a 0000 0000 94b3 4664 830a 0000  U.........Fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a01 6402 6403 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c04 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a05 4700 6404 6405 8400 6405 8302 5a06  Z.G.d.d...d...Z.
 00000060: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
 00000070: 0029 01da 034c 4c4d 6300 0000 0000 0000  .)...LLMc.......
 00000080: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00000090: 0073 6e00 0000 6500 5a01 6400 5a02 5500  .sn...e.Z.d.Z.U.
+00000090: 0073 8c00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
 000000a0: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
 000000b0: 6404 5a07 6505 6506 6405 3c00 6508 6506  d.Z.e.e.d.<.e.e.
-000000c0: 6406 3c00 6509 6506 6407 3c00 6412 640a  d.<.e.e.d.<.d.d.
-000000d0: 640b 8401 5a0a 6413 650b 6a0c 6505 6509  d...Z.d.e.j.e.e.
-000000e0: 6505 640c 9c04 640d 640e 8405 5a0d 6505  e.d...d.d...Z.e.
-000000f0: 650b 6a0c 640f 9c02 6410 6411 8404 5a0e  e.j.d...d.d...Z.
-00000100: 6408 5300 2914 da08 5061 6e64 6173 4149  d.S.)...PandasAI
-00000110: 7a43 5061 6e64 6173 4149 2069 7320 6120  zCPandasAI is a 
-00000120: 7772 6170 7065 7220 6172 6f75 6e64 2061  wrapper around a
-00000130: 204c 4c4d 2074 6f20 6d61 6b65 2064 6174   LLM to make dat
-00000140: 6166 7261 6d65 7320 636f 6e76 6573 6174  aframes convesat
-00000150: 696f 6e61 6c7a db0a 5468 6572 6520 6973  ionalz..There is
-00000160: 2061 2064 6174 6166 7261 6d65 2069 6e20   a dataframe in 
-00000170: 7061 6e64 6173 2028 7079 7468 6f6e 292e  pandas (python).
-00000180: 0a54 6865 206e 616d 6520 6f66 2074 6865  .The name of the
-00000190: 2064 6174 6166 7261 6d65 2069 7320 6064   dataframe is `d
-000001a0: 6660 2e0a 5468 6973 2069 7320 7468 6520  f`..This is the 
-000001b0: 7265 7375 6c74 206f 6620 6070 7269 6e74  result of `print
-000001c0: 2864 662e 6865 6164 2829 2960 3a0a 7b64  (df.head())`:.{d
-000001d0: 667d 2e0a 0a52 6574 7572 6e20 7468 6520  f}...Return the 
-000001e0: 7079 7468 6f6e 2063 6f64 6520 2864 6f20  python code (do 
-000001f0: 6e6f 7420 696d 706f 7274 2061 6e79 7468  not import anyth
-00000200: 696e 6729 2074 6f20 6765 7420 7468 6520  ing) to get the 
-00000210: 616e 7377 6572 2074 6f20 7468 6520 666f  answer to the fo
-00000220: 6c6c 6f77 696e 6720 7175 6573 7469 6f6e  llowing question
-00000230: 3a0a da10 7461 736b 5f69 6e73 7472 7563  :...task_instruc
-00000240: 7469 6f6e 7aa2 0a54 6865 2063 7573 746f  tionz..The custo
-00000250: 6d65 7220 6173 6b65 643a 0a7b 7175 6573  mer asked:.{ques
-00000260: 7469 6f6e 7d0a 0a54 6f20 6765 7420 7468  tion}..To get th
-00000270: 6520 616e 7377 6572 2c20 7275 6e20 796f  e answer, run yo
-00000280: 7520 7275 6e20 7468 6520 666f 6c6c 6f77  u run the follow
-00000290: 696e 6720 636f 6465 2069 6e20 7061 6e64  ing code in pand
-000002a0: 6173 2028 7079 7468 6f6e 293a 0a7b 636f  as (python):.{co
-000002b0: 6465 7d0a 0a52 6573 756c 743a 0a7b 616e  de}..Result:.{an
-000002c0: 7377 6572 7d0a 0a57 7269 7465 2074 6865  swer}..Write the
-000002d0: 2061 6e73 7765 7220 746f 2074 6865 2063   answer to the c
-000002e0: 7573 746f 6d65 720a da14 7265 7370 6f6e  ustomer...respon
-000002f0: 7365 5f69 6e73 7472 7563 7469 6f6e da03  se_instruction..
-00000300: 6c6c 6dda 1563 6f6e 7665 7273 6174 696f  llm..conversatio
-00000310: 6e61 6c5f 616e 7377 6572 4e54 6303 0000  nal_answerNTc...
-00000320: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00000330: 0043 0000 0073 2000 0000 7c01 6400 7500  .C...s ...|.d.u.
-00000340: 7210 7400 6401 8301 8201 7c01 7c00 5f01  r.t.d.....|.|._.
-00000350: 7c02 7c00 5f02 6400 5300 2902 4e7a 3c41  |.|._.d.S.).Nz<A
-00000360: 6e20 4c4c 4d20 7368 6f75 6c64 2062 6520  n LLM should be 
-00000370: 7072 6f76 6964 6564 2074 6f20 696e 7374  provided to inst
-00000380: 616e 7469 6174 6520 6120 5061 6e64 6173  antiate a Pandas
-00000390: 4149 2069 6e73 7461 6e63 6529 03da 0945  AI instance)...E
-000003a0: 7863 6570 7469 6f6e 7207 0000 0072 0800  xceptionr....r..
-000003b0: 0000 2903 da04 7365 6c66 7207 0000 0072  ..)...selfr....r
-000003c0: 0800 0000 a900 720b 0000 00fa 412f 5573  ......r.....A/Us
-000003d0: 6572 732f 6761 6272 6965 6c65 7665 6e74  ers/gabrielevent
-000003e0: 7572 692f 5072 6f6a 6563 7473 2f61 692f  uri/Projects/ai/
-000003f0: 7061 6e64 6173 2d61 692f 7061 6e64 6173  pandas-ai/pandas
-00000400: 6169 2f5f 5f69 6e69 745f 5f2e 7079 da08  ai/__init__.py..
-00000410: 5f5f 696e 6974 5f5f 2100 0000 7308 0000  __init__!...s...
-00000420: 0000 0108 0108 0106 017a 1150 616e 6461  .........z.Panda
-00000430: 7341 492e 5f5f 696e 6974 5f5f 2904 da02  sAI.__init__)...
-00000440: 6466 da06 7072 6f6d 7074 7208 0000 00da  df..promptr.....
-00000450: 0672 6574 7572 6e63 0400 0000 0000 0000  .returnc........
-00000460: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
-00000470: 736e 0000 0074 0064 017c 006a 016a 029b  sn...t.d.|.j.j..
-00000480: 0064 029d 0383 0101 007c 006a 01a0 037c  .d.......|.j...|
-00000490: 006a 046a 057c 01a0 06a1 0064 038d 017c  .j.j.|.....d...|
-000004a0: 02a1 027d 047c 00a0 077c 047c 01a1 027d  ...}.|...|.|...}
-000004b0: 057c 0364 0475 0072 4a7c 006a 087d 037c  .|.d.u.rJ|.j.}.|
-000004c0: 0372 6a7c 006a 01a0 097c 006a 0a6a 057c  .rj|.j...|.j.j.|
-000004d0: 027c 047c 0564 058d 037c 05a1 0253 007c  .|.|.d...|...S.|
-000004e0: 0553 0029 067a 2152 756e 2074 6865 204c  .S.).z!Run the L
-000004f0: 4c4d 2077 6974 6820 7468 6520 6769 7665  LM with the give
-00000500: 6e20 7072 6f6d 7074 7a16 5275 6e6e 696e  n promptz.Runnin
-00000510: 6720 5061 6e64 6173 4149 2077 6974 6820  g PandasAI with 
-00000520: 7a07 204c 4c4d 2e2e 2e29 0172 0e00 0000  z. LLM...).r....
-00000530: 4e29 035a 0871 7565 7374 696f 6eda 0463  N).Z.question..c
-00000540: 6f64 65da 0661 6e73 7765 7229 0bda 0570  ode..answer)...p
-00000550: 7269 6e74 7207 0000 00da 055f 7479 7065  rintr......_type
-00000560: 5a0d 6765 6e65 7261 7465 5f63 6f64 6572  Z.generate_coder
-00000570: 0500 0000 da06 666f 726d 6174 da04 6865  ......format..he
-00000580: 6164 da08 7275 6e5f 636f 6465 7208 0000  ad..run_coder...
-00000590: 00da 0463 616c 6c72 0600 0000 2906 720a  ...callr....).r.
-000005a0: 0000 0072 0e00 0000 720f 0000 0072 0800  ...r....r....r..
-000005b0: 0000 7211 0000 0072 1200 0000 720b 0000  ..r....r....r...
-000005c0: 0072 0b00 0000 720c 0000 00da 0372 756e  .r....r......run
-000005d0: 2700 0000 7310 0000 0000 0214 011c 010c  '...s...........
-000005e0: 0208 0106 0104 011c 017a 0c50 616e 6461  .........z.Panda
-000005f0: 7341 492e 7275 6e29 0272 1100 0000 720e  sAI.run).r....r.
-00000600: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000610: 0800 0000 0600 0000 4300 0000 7388 0000  ........C...s...
-00000620: 0074 00a0 01a1 007d 037c 0374 025f 0374  .t.....}.|.t._.t
-00000630: 047c 0183 0101 0074 026a 0574 025f 037c  .|.....t.j.t._.|
-00000640: 03a0 06a1 007d 047c 01a0 07a1 00a0 0864  .....}.|.......d
-00000650: 01a1 017d 057c 0564 0219 00a0 07a1 007d  ...}.|.d.......}
-00000660: 067c 06a0 0964 03a1 0172 647c 06a0 0a64  .|...d...rd|...d
-00000670: 04a1 0172 6474 0b7c 0664 0564 0285 0219  ...rdt.|.d.d....
-00000680: 0083 0153 007a 0e74 0b7c 0683 017d 077c  ...S.z.t.|...}.|
-00000690: 0757 0053 0001 0001 0001 007c 0406 0059  .W.S.......|...Y
-000006a0: 0053 0030 0064 0653 0029 077a 3952 756e  .S.0.d.S.).z9Run
-000006b0: 2074 6865 2063 6f64 6520 696e 2074 6865   the code in the
-000006c0: 2063 7572 7265 6e74 2063 6f6e 7465 7874   current context
-000006d0: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
-000006e0: 7265 7375 6c74 da01 0ae9 ffff ffff 7a06  result........z.
-000006f0: 7072 696e 7428 fa01 29e9 0600 0000 4e29  print(..).....N)
-00000700: 0cda 0269 6fda 0853 7472 696e 6749 4fda  ...io..StringIO.
-00000710: 0373 7973 da06 7374 646f 7574 da04 6578  .sys..stdout..ex
-00000720: 6563 da0a 5f5f 7374 646f 7574 5f5f da08  ec..__stdout__..
-00000730: 6765 7476 616c 7565 da05 7374 7269 70da  getvalue..strip.
-00000740: 0573 706c 6974 da0a 7374 6172 7473 7769  .split..startswi
-00000750: 7468 da08 656e 6473 7769 7468 da04 6576  th..endswith..ev
-00000760: 616c 2908 720a 0000 0072 1100 0000 720e  al).r....r....r.
-00000770: 0000 00da 066f 7574 7075 745a 0f63 6170  .....outputZ.cap
-00000780: 7475 7265 645f 6f75 7470 7574 da05 6c69  tured_output..li
-00000790: 6e65 73da 096c 6173 745f 6c69 6e65 da06  nes..last_line..
-000007a0: 7265 7375 6c74 720b 0000 0072 0b00 0000  resultr....r....
-000007b0: 720c 0000 0072 1700 0000 3300 0000 731c  r....r....3...s.
-000007c0: 0000 0000 0408 0106 0308 0308 0108 030e  ................
-000007d0: 010c 0114 0210 0302 0108 0106 0106 017a  ...............z
-000007e0: 1150 616e 6461 7341 492e 7275 6e5f 636f  .PandasAI.run_co
-000007f0: 6465 2902 4e54 2901 4e29 0fda 085f 5f6e  de).NT).N)...__n
-00000800: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000810: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000820: 075f 5f64 6f63 5f5f 7205 0000 00da 0373  .__doc__r......s
-00000830: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
-00000840: 735f 5f72 0600 0000 7203 0000 00da 0462  s__r....r......b
-00000850: 6f6f 6c72 0d00 0000 da02 7064 da09 4461  oolr......pd..Da
-00000860: 7461 4672 616d 6572 1900 0000 7217 0000  taFramer....r...
-00000870: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000880: 720c 0000 0072 0400 0000 0600 0000 7310  r....r........s.
-00000890: 0000 000a 0104 020c 080c 0c08 0108 030a  ................
-000008a0: 0618 0c72 0400 0000 2907 da06 7061 6e64  ...r....)...pand
-000008b0: 6173 7235 0000 005a 086c 6c6d 2e62 6173  asr5...Z.llm.bas
-000008c0: 6572 0300 0000 721e 0000 0072 2000 0000  er....r....r ...
-000008d0: 7204 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000008e0: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-000008f0: 6c65 3e01 0000 0073 0800 0000 0801 0c01  le>....s........
-00000900: 0801 0802                                ....
+000000c0: 6406 3c00 6407 5a09 650a 6506 6408 3c00  d.<.d.Z.e.e.d.<.
+000000d0: 6409 5a0b 650a 6506 640a 3c00 6505 640b  d.Z.e.e.d.<.e.d.
+000000e0: 9c01 640c 640d 8404 5a0c 6417 640f 6410  ..d.d...Z.d.d.d.
+000000f0: 8401 5a0d 6418 650e 6a0f 6505 650a 6505  ..Z.d.e.j.e.e.e.
+00000100: 6411 9c04 6412 6413 8405 5a10 6505 650e  d...d.d...Z.e.e.
+00000110: 6a0f 6414 9c02 6415 6416 8404 5a11 640e  j.d...d.d...Z.d.
+00000120: 5300 2919 da08 5061 6e64 6173 4149 7a43  S.)...PandasAIzC
+00000130: 5061 6e64 6173 4149 2069 7320 6120 7772  PandasAI is a wr
+00000140: 6170 7065 7220 6172 6f75 6e64 2061 204c  apper around a L
+00000150: 4c4d 2074 6f20 6d61 6b65 2064 6174 6166  LM to make dataf
+00000160: 7261 6d65 7320 636f 6e76 6573 6174 696f  rames convesatio
+00000170: 6e61 6c7a db0a 5468 6572 6520 6973 2061  nalz..There is a
+00000180: 2064 6174 6166 7261 6d65 2069 6e20 7061   dataframe in pa
+00000190: 6e64 6173 2028 7079 7468 6f6e 292e 0a54  ndas (python)..T
+000001a0: 6865 206e 616d 6520 6f66 2074 6865 2064  he name of the d
+000001b0: 6174 6166 7261 6d65 2069 7320 6064 6660  ataframe is `df`
+000001c0: 2e0a 5468 6973 2069 7320 7468 6520 7265  ..This is the re
+000001d0: 7375 6c74 206f 6620 6070 7269 6e74 2864  sult of `print(d
+000001e0: 662e 6865 6164 2829 2960 3a0a 7b64 667d  f.head())`:.{df}
+000001f0: 2e0a 0a52 6574 7572 6e20 7468 6520 7079  ...Return the py
+00000200: 7468 6f6e 2063 6f64 6520 2864 6f20 6e6f  thon code (do no
+00000210: 7420 696d 706f 7274 2061 6e79 7468 696e  t import anythin
+00000220: 6729 2074 6f20 6765 7420 7468 6520 616e  g) to get the an
+00000230: 7377 6572 2074 6f20 7468 6520 666f 6c6c  swer to the foll
+00000240: 6f77 696e 6720 7175 6573 7469 6f6e 3a0a  owing question:.
+00000250: da10 7461 736b 5f69 6e73 7472 7563 7469  ..task_instructi
+00000260: 6f6e 7aa2 0a54 6865 2063 7573 746f 6d65  onz..The custome
+00000270: 7220 6173 6b65 643a 0a7b 7175 6573 7469  r asked:.{questi
+00000280: 6f6e 7d0a 0a54 6f20 6765 7420 7468 6520  on}..To get the 
+00000290: 616e 7377 6572 2c20 7275 6e20 796f 7520  answer, run you 
+000002a0: 7275 6e20 7468 6520 666f 6c6c 6f77 696e  run the followin
+000002b0: 6720 636f 6465 2069 6e20 7061 6e64 6173  g code in pandas
+000002c0: 2028 7079 7468 6f6e 293a 0a7b 636f 6465   (python):.{code
+000002d0: 7d0a 0a52 6573 756c 743a 0a7b 616e 7377  }..Result:.{answ
+000002e0: 6572 7d0a 0a57 7269 7465 2074 6865 2061  er}..Write the a
+000002f0: 6e73 7765 7220 746f 2074 6865 2063 7573  nswer to the cus
+00000300: 746f 6d65 720a da14 7265 7370 6f6e 7365  tomer...response
+00000310: 5f69 6e73 7472 7563 7469 6f6e da03 6c6c  _instruction..ll
+00000320: 6d46 da07 7665 7262 6f73 6554 da15 636f  mF..verboseT..co
+00000330: 6e76 6572 7361 7469 6f6e 616c 5f61 6e73  nversational_ans
+00000340: 7765 7229 01da 076d 6573 7361 6765 6302  wer)...messagec.
+00000350: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000360: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
+00000370: 720e 7401 7c01 8301 0100 6401 5300 2902  r.t.|.....d.S.).
+00000380: 7a0d 4c6f 6720 6120 6d65 7373 6167 654e  z.Log a messageN
+00000390: 2902 7208 0000 00da 0570 7269 6e74 2902  ).r......print).
+000003a0: da04 7365 6c66 720a 0000 00a9 0072 0d00  ..selfr......r..
+000003b0: 0000 fa41 2f55 7365 7273 2f67 6162 7269  ...A/Users/gabri
+000003c0: 656c 6576 656e 7475 7269 2f50 726f 6a65  eleventuri/Proje
+000003d0: 6374 732f 6169 2f70 616e 6461 732d 6169  cts/ai/pandas-ai
+000003e0: 2f70 616e 6461 7361 692f 5f5f 696e 6974  /pandasai/__init
+000003f0: 5f5f 2e70 79da 036c 6f67 2100 0000 7304  __.py..log!...s.
+00000400: 0000 0000 0206 017a 0c50 616e 6461 7341  .......z.PandasA
+00000410: 492e 6c6f 674e 6304 0000 0000 0000 0000  I.logNc.........
+00000420: 0000 0004 0000 0002 0000 0043 0000 0073  ...........C...s
+00000430: 2600 0000 7c01 6400 6b08 7210 7400 6401  &...|.d.k.r.t.d.
+00000440: 8301 8201 7c01 7c00 5f01 7c02 7c00 5f02  ....|.|._.|.|._.
+00000450: 7c03 7c00 5f03 6400 5300 2902 4e7a 3c41  |.|._.d.S.).Nz<A
+00000460: 6e20 4c4c 4d20 7368 6f75 6c64 2062 6520  n LLM should be 
+00000470: 7072 6f76 6964 6564 2074 6f20 696e 7374  provided to inst
+00000480: 616e 7469 6174 6520 6120 5061 6e64 6173  antiate a Pandas
+00000490: 4149 2069 6e73 7461 6e63 6529 04da 0945  AI instance)...E
+000004a0: 7863 6570 7469 6f6e 7207 0000 0072 0900  xceptionr....r..
+000004b0: 0000 7208 0000 0029 0472 0c00 0000 7207  ..r....).r....r.
+000004c0: 0000 0072 0900 0000 7208 0000 0072 0d00  ...r....r....r..
+000004d0: 0000 720d 0000 0072 0e00 0000 da08 5f5f  ..r....r......__
+000004e0: 696e 6974 5f5f 2700 0000 730a 0000 0000  init__'...s.....
+000004f0: 0108 0108 0106 0106 017a 1150 616e 6461  .........z.Panda
+00000500: 7341 492e 5f5f 696e 6974 5f5f 2904 da02  sAI.__init__)...
+00000510: 6466 da06 7072 6f6d 7074 7209 0000 00da  df..promptr.....
+00000520: 0672 6574 7572 6e63 0400 0000 0000 0000  .returnc........
+00000530: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
+00000540: 73a2 0000 007c 00a0 0064 017c 006a 016a  s....|...d.|.j.j
+00000550: 029b 0064 029d 03a1 0101 007c 006a 01a0  ...d.......|.j..
+00000560: 037c 006a 046a 057c 01a0 06a1 0064 038d  .|.j.j.|.....d..
+00000570: 017c 02a1 027d 047c 00a0 0064 047c 049b  .|...}.|...d.|..
+00000580: 0064 059d 03a1 0101 007c 00a0 077c 047c  .d.......|...|.|
+00000590: 01a1 027d 057c 00a0 0064 067c 059b 009d  ...}.|...d.|....
+000005a0: 02a1 0101 007c 0364 076b 0872 6e7c 006a  .....|.d.k.rn|.j
+000005b0: 087d 037c 0372 9e7c 006a 01a0 097c 006a  .}.|.r.|.j...|.j
+000005c0: 0a6a 057c 027c 047c 0564 088d 037c 05a1  .j.|.|.|.d...|..
+000005d0: 027d 057c 00a0 0064 097c 059b 009d 02a1  .}.|...d.|......
+000005e0: 0101 007c 0553 0029 0a7a 2152 756e 2074  ...|.S.).z!Run t
+000005f0: 6865 204c 4c4d 2077 6974 6820 7468 6520  he LLM with the 
+00000600: 6769 7665 6e20 7072 6f6d 7074 7a16 5275  given promptz.Ru
+00000610: 6e6e 696e 6720 5061 6e64 6173 4149 2077  nning PandasAI w
+00000620: 6974 6820 7a07 204c 4c4d 2e2e 2e29 0172  ith z. LLM...).r
+00000630: 1200 0000 7a15 0a43 6f64 6520 6765 6e65  ....z..Code gene
+00000640: 7261 7465 643a 0a60 6060 0a7a 040a 6060  rated:.```.z..``
+00000650: 607a 0841 6e73 7765 723a 204e 2903 5a08  `z.Answer: N).Z.
+00000660: 7175 6573 7469 6f6e da04 636f 6465 da06  question..code..
+00000670: 616e 7377 6572 7a17 436f 6e76 6572 7361  answerz.Conversa
+00000680: 7469 6f6e 616c 2061 6e73 7765 723a 2029  tional answer: )
+00000690: 0b72 0f00 0000 7207 0000 00da 055f 7479  .r....r......_ty
+000006a0: 7065 5a0d 6765 6e65 7261 7465 5f63 6f64  peZ.generate_cod
+000006b0: 6572 0500 0000 da06 666f 726d 6174 da04  er......format..
+000006c0: 6865 6164 da08 7275 6e5f 636f 6465 7209  head..run_coder.
+000006d0: 0000 00da 0463 616c 6c72 0600 0000 2906  .....callr....).
+000006e0: 720c 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000006f0: 0900 0000 7215 0000 0072 1600 0000 720d  ....r....r....r.
+00000700: 0000 0072 0d00 0000 720e 0000 00da 0372  ...r....r......r
+00000710: 756e 2e00 0000 731a 0000 0000 0216 011c  un....s.........
+00000720: 0106 0302 fd0a 050c 0110 0208 0106 0104  ................
+00000730: 011c 0110 017a 0c50 616e 6461 7341 492e  .....z.PandasAI.
+00000740: 7275 6e29 0272 1500 0000 7212 0000 0063  run).r....r....c
+00000750: 0300 0000 0000 0000 0000 0000 0800 0000  ................
+00000760: 0600 0000 4300 0000 7388 0000 0074 00a0  ....C...s....t..
+00000770: 01a1 007d 037c 0374 025f 0374 047c 0183  ...}.|.t._.t.|..
+00000780: 0101 0074 026a 0574 025f 037c 03a0 06a1  ...t.j.t._.|....
+00000790: 007d 047c 01a0 07a1 00a0 0864 01a1 017d  .}.|.......d...}
+000007a0: 057c 0564 0219 00a0 07a1 007d 067c 06a0  .|.d.......}.|..
+000007b0: 0964 03a1 0172 647c 06a0 0a64 04a1 0172  .d...rd|...d...r
+000007c0: 6474 0b7c 0664 0564 0285 0219 0083 0153  dt.|.d.d.......S
+000007d0: 007a 0e74 0b7c 0683 017d 077c 0757 0053  .z.t.|...}.|.W.S
+000007e0: 0001 0001 0001 007c 0406 0059 0053 0058  .......|...Y.S.X
+000007f0: 0064 0653 0029 077a 3952 756e 2074 6865  .d.S.).z9Run the
+00000800: 2063 6f64 6520 696e 2074 6865 2063 7572   code in the cur
+00000810: 7265 6e74 2063 6f6e 7465 7874 2061 6e64  rent context and
+00000820: 2072 6574 7572 6e20 7468 6520 7265 7375   return the resu
+00000830: 6c74 da01 0ae9 ffff ffff 7a06 7072 696e  lt........z.prin
+00000840: 7428 fa01 29e9 0600 0000 4e29 0cda 0269  t(..).....N)...i
+00000850: 6fda 0853 7472 696e 6749 4fda 0373 7973  o..StringIO..sys
+00000860: da06 7374 646f 7574 da04 6578 6563 da0a  ..stdout..exec..
+00000870: 5f5f 7374 646f 7574 5f5f da08 6765 7476  __stdout__..getv
+00000880: 616c 7565 da05 7374 7269 70da 0573 706c  alue..strip..spl
+00000890: 6974 da0a 7374 6172 7473 7769 7468 da08  it..startswith..
+000008a0: 656e 6473 7769 7468 da04 6576 616c 2908  endswith..eval).
+000008b0: 720c 0000 0072 1500 0000 7212 0000 00da  r....r....r.....
+000008c0: 066f 7574 7075 745a 0f63 6170 7475 7265  .outputZ.capture
+000008d0: 645f 6f75 7470 7574 da05 6c69 6e65 73da  d_output..lines.
+000008e0: 096c 6173 745f 6c69 6e65 da06 7265 7375  .last_line..resu
+000008f0: 6c74 720d 0000 0072 0d00 0000 720e 0000  ltr....r....r...
+00000900: 0072 1a00 0000 4100 0000 731c 0000 0000  .r....A...s.....
+00000910: 0408 0106 0308 0308 0108 030e 010c 0114  ................
+00000920: 0210 0302 0108 0106 0106 017a 1150 616e  ...........z.Pan
+00000930: 6461 7341 492e 7275 6e5f 636f 6465 2903  dasAI.run_code).
+00000940: 4e54 4629 014e 2912 da08 5f5f 6e61 6d65  NTF).N)...__name
+00000950: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000960: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000970: 646f 635f 5f72 0500 0000 da03 7374 72da  doc__r......str.
+00000980: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000990: 7206 0000 0072 0300 0000 7208 0000 00da  r....r....r.....
+000009a0: 0462 6f6f 6c72 0900 0000 720f 0000 0072  .boolr....r....r
+000009b0: 1100 0000 da02 7064 da09 4461 7461 4672  ......pd..DataFr
+000009c0: 616d 6572 1c00 0000 721a 0000 0072 0d00  amer....r....r..
+000009d0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000009e0: 0072 0400 0000 0600 0000 7314 0000 000a  .r........s.....
+000009f0: 0104 020c 080c 0c08 010c 010c 020e 060a  ................
+00000a00: 0718 1372 0400 0000 2907 da06 7061 6e64  ...r....)...pand
+00000a10: 6173 7238 0000 005a 086c 6c6d 2e62 6173  asr8...Z.llm.bas
+00000a20: 6572 0300 0000 7221 0000 0072 2300 0000  er....r!...r#...
+00000a30: 7204 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000a40: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
+00000a50: 6c65 3e01 0000 0073 0800 0000 0801 0c01  le>....s........
+00000a60: 0801 0802                                ....
```

### Comparing `pandasai-0.0.2/pandasai/llm/__pycache__/alpaca.cpython-39.pyc` & `pandasai-0.0.3/pandasai/llm/__pycache__/alpaca.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 13:43:28 2023 UTC, .py size: 1083 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8087 4664 3b04 0000  a.........Fd;...
+00000000: 610d 0d0a 0000 0000 9387 4664 2904 0000  a.........Fd)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6404 6405 8400 6405 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2906 e900 0000 004e e901  Z.d.S.)......N..
 00000060: 0000 0029 01da 034c 4c4d 6300 0000 0000  ...)...LLMc.....
 00000070: 0000 0000 0000 0000 0000 0007 0000 0040  ...............@
```

### Comparing `pandasai-0.0.2/pandasai/llm/__pycache__/base.cpython-39.pyc` & `pandasai-0.0.3/pandasai/llm/__pycache__/base.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 13:34:54 2023 UTC, .py size: 1827 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7e85 4664 2307 0000  a.......~.Fd#...
+00000000: 550d 0d0a 0000 0000 02ed 4664 c306 0000  U.........Fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 4700  d.l.Z.d.d.l.Z.G.
 00000040: 6402 6403 8400 6403 8302 5a02 6401 5300  d.d...d...Z.d.S.
 00000050: 2904 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
 00000060: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
 00000070: 0073 7e00 0000 6500 5a01 6400 5a02 6503  .s~...e.Z.d.Z.e.
@@ -25,125 +25,124 @@
 00000180: 0000 fa41 2f55 7365 7273 2f67 6162 7269  ...A/Users/gabri
 00000190: 656c 6576 656e 7475 7269 2f50 726f 6a65  eleventuri/Proje
 000001a0: 6374 732f 6169 2f70 616e 6461 732d 6169  cts/ai/pandas-ai
 000001b0: 2f70 616e 6461 7361 692f 6c6c 6d2f 6261  /pandasai/llm/ba
 000001c0: 7365 2e70 79da 055f 7479 7065 0500 0000  se.py.._type....
 000001d0: 7302 0000 0000 037a 094c 4c4d 2e5f 7479  s......z.LLM._ty
 000001e0: 7065 2902 da04 636f 6465 7203 0000 0063  pe)...coder....c
-000001f0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00000200: 0500 0000 4300 0000 7378 0000 0074 00a0  ....C...sx...t..
-00000210: 017c 01a1 017d 027c 026a 0264 0064 0085  .|...}.|.j.d.d..
-00000220: 0219 0044 005d 547d 0374 037c 0374 006a  ...D.]T}.t.|.t.j
-00000230: 0483 0272 547c 036a 0544 005d 107d 047c  ...rT|.j.D.].}.|
-00000240: 036a 05a0 067c 04a1 0101 0071 2e7c 036a  .j...|.....q.|.j
-00000250: 0573 6c7c 026a 02a0 067c 03a1 0101 0071  .sl|.j...|.....q
-00000260: 1874 037c 0374 006a 0783 0272 187c 026a  .t.|.t.j...r.|.j
-00000270: 02a0 067c 03a1 0101 0071 1874 00a0 087c  ...|.....q.t...|
-00000280: 02a1 0153 0029 014e 2909 da03 6173 74da  ...S.).N)...ast.
-00000290: 0570 6172 7365 da04 626f 6479 da0a 6973  .parse..body..is
-000002a0: 696e 7374 616e 6365 da06 496d 706f 7274  instance..Import
-000002b0: da05 6e61 6d65 73da 0672 656d 6f76 65da  ..names..remove.
-000002c0: 0a49 6d70 6f72 7446 726f 6dda 0775 6e70  .ImportFrom..unp
-000002d0: 6172 7365 2905 7206 0000 0072 0a00 0000  arse).r....r....
-000002e0: da04 7472 6565 da04 6e6f 6465 da04 6e61  ..tree..node..na
-000002f0: 6d65 7207 0000 0072 0700 0000 7208 0000  mer....r....r...
-00000300: 00da 0f5f 7265 6d6f 7665 5f69 6d70 6f72  ..._remove_impor
-00000310: 7473 0a00 0000 7314 0000 0000 010a 0212  ts....s.........
-00000320: 010c 010a 010e 0106 010e 010c 010e 027a  ...............z
-00000330: 134c 4c4d 2e5f 7265 6d6f 7665 5f69 6d70  .LLM._remove_imp
-00000340: 6f72 7473 6302 0000 0000 0000 0000 0000  ortsc...........
-00000350: 0002 0000 0005 0000 0043 0000 0073 4a00  .........C...sJ.
-00000360: 0000 7400 a001 6401 7c01 a102 721a 7400  ..t...d.|...r.t.
-00000370: a002 6401 6402 7c01 a103 7d01 7400 a001  ..d.d.|...}.t...
-00000380: 6403 7c01 a102 7234 7400 a002 6404 6405  d.|...r4t...d.d.
-00000390: 7c01 a103 7d01 7c00 a003 7c01 a101 0100  |...}.|...|.....
-000003a0: 7c01 a004 a100 7d01 7c01 5300 2906 7a83  |.....}.|.S.).z.
-000003b0: 506f 6c69 7368 2074 6865 2063 6f64 653a  Polish the code:
-000003c0: 0a20 2020 202d 2072 656d 6f76 6520 7468  .    - remove th
-000003d0: 6520 6c65 6164 696e 6720 2270 7974 686f  e leading "pytho
-000003e0: 6e22 206f 7220 2270 7922 0a20 2020 202d  n" or "py".    -
-000003f0: 2072 656d 6f76 6520 7468 6520 696d 706f   remove the impo
-00000400: 7274 730a 2020 2020 2d20 7265 6d6f 7665  rts.    - remove
-00000410: 2074 7261 696c 696e 6720 7370 6163 6573   trailing spaces
-00000420: 2061 6e64 206e 6577 206c 696e 6573 0a20   and new lines. 
-00000430: 2020 207a 0c5e 2870 7974 686f 6e7c 7079     z.^(python|py
-00000440: 29da 007a 065e 602e 2a60 247a 085e 6028  )..z.^`.*`$z.^`(
-00000450: 2e2a 2960 247a 025c 3129 05da 0272 65da  .*)`$z.\1)...re.
-00000460: 056d 6174 6368 da03 7375 6272 1700 0000  .match..subr....
-00000470: da05 7374 7269 7029 0272 0600 0000 720a  ..strip).r....r.
-00000480: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
-00000490: 0000 da0c 5f70 6f6c 6973 685f 636f 6465  ...._polish_code
-000004a0: 1800 0000 730e 0000 0000 070c 010e 010c  ....s...........
-000004b0: 010e 010a 0108 017a 104c 4c4d 2e5f 706f  .......z.LLM._po
-000004c0: 6c69 7368 5f63 6f64 6563 0200 0000 0000  lish_codec......
-000004d0: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-000004e0: 0000 732a 0000 007a 1074 00a0 017c 01a1  ..s*...z.t...|..
-000004f0: 0101 0057 0064 0153 0004 0074 0279 2401  ...W.d.S...t.y$.
-00000500: 0001 0001 0059 0064 0253 0030 0064 0053  .....Y.d.S.0.d.S
-00000510: 0029 034e 5446 2903 720b 0000 0072 0c00  .).NTF).r....r..
-00000520: 0000 da0b 5379 6e74 6178 4572 726f 7229  ....SyntaxError)
-00000530: 0272 0600 0000 da06 7374 7269 6e67 7207  .r......stringr.
-00000540: 0000 0072 0700 0000 7208 0000 00da 0f5f  ...r....r......_
-00000550: 6973 5f70 7974 686f 6e5f 636f 6465 2700  is_python_code'.
-00000560: 0000 730a 0000 0000 0102 010a 0106 010c  ..s.............
-00000570: 017a 134c 4c4d 2e5f 6973 5f70 7974 686f  .z.LLM._is_pytho
-00000580: 6e5f 636f 6465 fa03 6060 6029 03da 0872  n_code..```)...r
-00000590: 6573 706f 6e73 65da 0973 6570 6172 6174  esponse..separat
-000005a0: 6f72 7203 0000 0063 0300 0000 0000 0000  orr....c........
-000005b0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-000005c0: 7344 0000 007c 017d 0374 007c 01a0 017c  sD...|.}.t.|...|
-000005d0: 02a1 0183 0164 016b 0472 247c 01a0 017c  .....d.k.r$|...|
-000005e0: 02a1 0164 0119 007d 037c 00a0 027c 03a1  ...d...}.|...|..
-000005f0: 017d 037c 00a0 037c 03a1 0173 4074 0464  .}.|...|...s@t.d
-00000600: 0283 0182 017c 0353 0029 037a 2245 7874  .....|.S.).z"Ext
-00000610: 7261 6374 2074 6865 2063 6f64 6520 6672  ract the code fr
-00000620: 6f6d 2074 6865 2072 6573 706f 6e73 65e9  om the response.
-00000630: 0100 0000 7a1d 4e6f 2063 6f64 6520 666f  ....z.No code fo
-00000640: 756e 6420 696e 2074 6865 2072 6573 706f  und in the respo
-00000650: 6e73 6529 05da 036c 656e da05 7370 6c69  nse)...len..spli
-00000660: 7472 1d00 0000 7220 0000 0072 0500 0000  tr....r ...r....
-00000670: 2904 7206 0000 0072 2200 0000 7223 0000  ).r....r"...r#..
-00000680: 0072 0a00 0000 7207 0000 0072 0700 0000  .r....r....r....
-00000690: 7208 0000 00da 0d5f 6578 7472 6163 745f  r......_extract_
-000006a0: 636f 6465 2e00 0000 730e 0000 0000 0304  code....s.......
-000006b0: 0112 010e 010a 010a 0108 027a 114c 4c4d  ...........z.LLM
-000006c0: 2e5f 6578 7472 6163 745f 636f 6465 2903  ._extract_code).
-000006d0: da0b 696e 7374 7275 6374 696f 6eda 0569  ..instruction..i
-000006e0: 6e70 7574 7203 0000 0063 0300 0000 0000  nputr....c......
-000006f0: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
-00000700: 0000 730c 0000 0074 0064 0183 0182 0164  ..s....t.d.....d
-00000710: 0253 0029 037a 2545 7865 6375 7465 2074  .S.).z%Execute t
-00000720: 6865 206c 6c6d 2077 6974 6820 7468 6520  he llm with the 
-00000730: 6769 7665 6e20 7072 6f6d 7074 7a24 4361  given promptz$Ca
-00000740: 6c6c 206d 6574 686f 6420 6861 7320 6e6f  ll method has no
-00000750: 7420 6265 656e 2069 6d70 6c65 6d65 6e74  t been implement
-00000760: 6564 4e72 0400 0000 2903 7206 0000 0072  edNr....).r....r
-00000770: 2800 0000 7229 0000 0072 0700 0000 7207  (...r)...r....r.
-00000780: 0000 0072 0800 0000 da04 6361 6c6c 3a00  ...r......call:.
-00000790: 0000 7302 0000 0000 037a 084c 4c4d 2e63  ..s......z.LLM.c
-000007a0: 616c 6c29 0372 2800 0000 da06 7072 6f6d  all).r(.....prom
-000007b0: 7074 7203 0000 0063 0300 0000 0000 0000  ptr....c........
-000007c0: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
-000007d0: 7312 0000 007c 00a0 007c 00a0 017c 017c  s....|...|...|.|
-000007e0: 02a1 02a1 0153 0029 017a 3947 656e 6572  .....S.).z9Gener
-000007f0: 6174 6520 7468 6520 636f 6465 2062 6173  ate the code bas
-00000800: 6564 206f 6e20 7468 6520 696e 7374 7275  ed on the instru
-00000810: 6374 696f 6e20 616e 6420 7468 6520 7072  ction and the pr
-00000820: 6f6d 7074 2902 7227 0000 0072 2a00 0000  ompt).r'...r*...
-00000830: 2903 7206 0000 0072 2800 0000 722b 0000  ).r....r(...r+..
-00000840: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000850: da0d 6765 6e65 7261 7465 5f63 6f64 653f  ..generate_code?
-00000860: 0000 0073 0200 0000 0003 7a11 4c4c 4d2e  ...s......z.LLM.
-00000870: 6765 6e65 7261 7465 5f63 6f64 654e 2901  generate_codeN).
-00000880: 7221 0000 0029 0cda 085f 5f6e 616d 655f  r!...)...__name_
-00000890: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000008a0: 5f71 7561 6c6e 616d 655f 5fda 0870 726f  _qualname__..pro
-000008b0: 7065 7274 79da 0373 7472 7209 0000 0072  perty..strr....r
-000008c0: 1700 0000 721d 0000 0072 2000 0000 7227  ....r....r ...r'
-000008d0: 0000 0072 2a00 0000 722c 0000 0072 0700  ...r*...r,...r..
-000008e0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000008f0: 0072 0200 0000 0400 0000 7310 0000 0008  .r........s.....
-00000900: 0102 0110 0410 0e10 0f08 0714 0c12 0572  ...............r
-00000910: 0200 0000 2903 7219 0000 0072 0b00 0000  ....).r....r....
-00000920: 7202 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
-00000930: 0700 0000 7208 0000 00da 083c 6d6f 6475  ....r......<modu
-00000940: 6c65 3e01 0000 0073 0400 0000 0801 0802  le>....s........
+000001f0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00000200: 0500 0000 4300 0000 734c 0000 0074 00a0  ....C...sL...t..
+00000210: 017c 00a1 017d 0167 007d 027c 016a 0244  .|...}.g.}.|.j.D
+00000220: 005d 207d 0374 037c 0374 006a 0474 006a  .] }.t.|.t.j.t.j
+00000230: 0566 0283 0273 147c 02a0 067c 03a1 0101  .f...s.|...|....
+00000240: 0071 1474 006a 077c 0264 018d 017d 0474  .q.t.j.|.d...}.t
+00000250: 00a0 087c 04a1 0153 0029 024e 2901 da04  ...|...S.).N)...
+00000260: 626f 6479 2909 da03 6173 74da 0570 6172  body)...ast..par
+00000270: 7365 720b 0000 00da 0a69 7369 6e73 7461  ser......isinsta
+00000280: 6e63 65da 0649 6d70 6f72 74da 0a49 6d70  nce..Import..Imp
+00000290: 6f72 7446 726f 6dda 0661 7070 656e 64da  ortFrom..append.
+000002a0: 064d 6f64 756c 655a 0775 6e70 6172 7365  .ModuleZ.unparse
+000002b0: 2905 720a 0000 005a 0474 7265 655a 086e  ).r....Z.treeZ.n
+000002c0: 6577 5f62 6f64 79da 046e 6f64 655a 086e  ew_body..nodeZ.n
+000002d0: 6577 5f74 7265 6572 0700 0000 7207 0000  ew_treer....r...
+000002e0: 0072 0800 0000 da0f 5f72 656d 6f76 655f  .r......_remove_
+000002f0: 696d 706f 7274 730a 0000 0073 0e00 0000  imports....s....
+00000300: 0001 0a01 0402 0a01 1201 0c02 0c01 7a13  ..............z.
+00000310: 4c4c 4d2e 5f72 656d 6f76 655f 696d 706f  LLM._remove_impo
+00000320: 7274 7363 0200 0000 0000 0000 0000 0000  rtsc............
+00000330: 0200 0000 0500 0000 4300 0000 734a 0000  ........C...sJ..
+00000340: 0074 00a0 0164 017c 01a1 0272 1a74 00a0  .t...d.|...r.t..
+00000350: 0264 0164 027c 01a1 037d 0174 00a0 0164  .d.d.|...}.t...d
+00000360: 037c 01a1 0272 3474 00a0 0264 0464 057c  .|...r4t...d.d.|
+00000370: 01a1 037d 017c 00a0 037c 01a1 0101 007c  ...}.|...|.....|
+00000380: 01a0 04a1 007d 017c 0153 0029 067a 8350  .....}.|.S.).z.P
+00000390: 6f6c 6973 6820 7468 6520 636f 6465 3a0a  olish the code:.
+000003a0: 2020 2020 2d20 7265 6d6f 7665 2074 6865      - remove the
+000003b0: 206c 6561 6469 6e67 2022 7079 7468 6f6e   leading "python
+000003c0: 2220 6f72 2022 7079 220a 2020 2020 2d20  " or "py".    - 
+000003d0: 7265 6d6f 7665 2074 6865 2069 6d70 6f72  remove the impor
+000003e0: 7473 0a20 2020 202d 2072 656d 6f76 6520  ts.    - remove 
+000003f0: 7472 6169 6c69 6e67 2073 7061 6365 7320  trailing spaces 
+00000400: 616e 6420 6e65 7720 6c69 6e65 730a 2020  and new lines.  
+00000410: 2020 7a0c 5e28 7079 7468 6f6e 7c70 7929    z.^(python|py)
+00000420: da00 7a06 5e60 2e2a 6024 7a08 5e60 282e  ..z.^`.*`$z.^`(.
+00000430: 2a29 6024 7a02 5c31 2905 da02 7265 da05  *)`$z.\1)...re..
+00000440: 6d61 7463 68da 0373 7562 7214 0000 00da  match..subr.....
+00000450: 0573 7472 6970 2902 7206 0000 0072 0a00  .strip).r....r..
+00000460: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00000470: 00da 0c5f 706f 6c69 7368 5f63 6f64 6515  ..._polish_code.
+00000480: 0000 0073 0e00 0000 0007 0c01 0e01 0c01  ...s............
+00000490: 0e01 0a01 0801 7a10 4c4c 4d2e 5f70 6f6c  ......z.LLM._pol
+000004a0: 6973 685f 636f 6465 6302 0000 0000 0000  ish_codec.......
+000004b0: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
+000004c0: 0073 2c00 0000 7a10 7400 a001 7c01 a101  .s,...z.t...|...
+000004d0: 0100 5700 6401 5300 0400 7402 6b0a 7226  ..W.d.S...t.k.r&
+000004e0: 0100 0100 0100 5900 6402 5300 5800 6400  ......Y.d.S.X.d.
+000004f0: 5300 2903 4e54 4629 0372 0c00 0000 720d  S.).NTF).r....r.
+00000500: 0000 00da 0b53 796e 7461 7845 7272 6f72  .....SyntaxError
+00000510: 2902 7206 0000 00da 0673 7472 696e 6772  ).r......stringr
+00000520: 0700 0000 7207 0000 0072 0800 0000 da0f  ....r....r......
+00000530: 5f69 735f 7079 7468 6f6e 5f63 6f64 6524  _is_python_code$
+00000540: 0000 0073 0a00 0000 0001 0201 0a01 0601  ...s............
+00000550: 0e01 7a13 4c4c 4d2e 5f69 735f 7079 7468  ..z.LLM._is_pyth
+00000560: 6f6e 5f63 6f64 65fa 0360 6060 2903 da08  on_code..```)...
+00000570: 7265 7370 6f6e 7365 da09 7365 7061 7261  response..separa
+00000580: 746f 7272 0300 0000 6303 0000 0000 0000  torr....c.......
+00000590: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+000005a0: 0073 4400 0000 7c01 7d03 7400 7c01 a001  .sD...|.}.t.|...
+000005b0: 7c02 a101 8301 6401 6b04 7224 7c01 a001  |.....d.k.r$|...
+000005c0: 7c02 a101 6401 1900 7d03 7c00 a002 7c03  |...d...}.|...|.
+000005d0: a101 7d03 7c00 a003 7c03 a101 7340 7404  ..}.|...|...s@t.
+000005e0: 6402 8301 8201 7c03 5300 2903 7a22 4578  d.....|.S.).z"Ex
+000005f0: 7472 6163 7420 7468 6520 636f 6465 2066  tract the code f
+00000600: 726f 6d20 7468 6520 7265 7370 6f6e 7365  rom the response
+00000610: e901 0000 007a 1d4e 6f20 636f 6465 2066  .....z.No code f
+00000620: 6f75 6e64 2069 6e20 7468 6520 7265 7370  ound in the resp
+00000630: 6f6e 7365 2905 da03 6c65 6eda 0573 706c  onse)...len..spl
+00000640: 6974 721a 0000 0072 1d00 0000 7205 0000  itr....r....r...
+00000650: 0029 0472 0600 0000 721f 0000 0072 2000  .).r....r....r .
+00000660: 0000 720a 0000 0072 0700 0000 7207 0000  ..r....r....r...
+00000670: 0072 0800 0000 da0d 5f65 7874 7261 6374  .r......_extract
+00000680: 5f63 6f64 652b 0000 0073 0e00 0000 0003  _code+...s......
+00000690: 0401 1201 0e01 0a01 0a01 0802 7a11 4c4c  ............z.LL
+000006a0: 4d2e 5f65 7874 7261 6374 5f63 6f64 6529  M._extract_code)
+000006b0: 03da 0b69 6e73 7472 7563 7469 6f6e da05  ...instruction..
+000006c0: 696e 7075 7472 0300 0000 6303 0000 0000  inputr....c.....
+000006d0: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+000006e0: 0000 0073 0c00 0000 7400 6401 8301 8201  ...s....t.d.....
+000006f0: 6402 5300 2903 7a25 4578 6563 7574 6520  d.S.).z%Execute 
+00000700: 7468 6520 6c6c 6d20 7769 7468 2074 6865  the llm with the
+00000710: 2067 6976 656e 2070 726f 6d70 747a 2443   given promptz$C
+00000720: 616c 6c20 6d65 7468 6f64 2068 6173 206e  all method has n
+00000730: 6f74 2062 6565 6e20 696d 706c 656d 656e  ot been implemen
+00000740: 7465 644e 7204 0000 0029 0372 0600 0000  tedNr....).r....
+00000750: 7225 0000 0072 2600 0000 7207 0000 0072  r%...r&...r....r
+00000760: 0700 0000 7208 0000 00da 0463 616c 6c37  ....r......call7
+00000770: 0000 0073 0200 0000 0003 7a08 4c4c 4d2e  ...s......z.LLM.
+00000780: 6361 6c6c 2903 7225 0000 00da 0670 726f  call).r%.....pro
+00000790: 6d70 7472 0300 0000 6303 0000 0000 0000  mptr....c.......
+000007a0: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
+000007b0: 0073 1200 0000 7c00 a000 7c00 a001 7c01  .s....|...|...|.
+000007c0: 7c02 a102 a101 5300 2901 7a39 4765 6e65  |.....S.).z9Gene
+000007d0: 7261 7465 2074 6865 2063 6f64 6520 6261  rate the code ba
+000007e0: 7365 6420 6f6e 2074 6865 2069 6e73 7472  sed on the instr
+000007f0: 7563 7469 6f6e 2061 6e64 2074 6865 2070  uction and the p
+00000800: 726f 6d70 7429 0272 2400 0000 7227 0000  rompt).r$...r'..
+00000810: 0029 0372 0600 0000 7225 0000 0072 2800  .).r....r%...r(.
+00000820: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00000830: 00da 0d67 656e 6572 6174 655f 636f 6465  ...generate_code
+00000840: 3c00 0000 7302 0000 0000 037a 114c 4c4d  <...s......z.LLM
+00000850: 2e67 656e 6572 6174 655f 636f 6465 4e29  .generate_codeN)
+00000860: 0172 1e00 0000 290c da08 5f5f 6e61 6d65  .r....)...__name
+00000870: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000880: 5f5f 7175 616c 6e61 6d65 5f5f da08 7072  __qualname__..pr
+00000890: 6f70 6572 7479 da03 7374 7272 0900 0000  operty..strr....
+000008a0: 7214 0000 0072 1a00 0000 721d 0000 0072  r....r....r....r
+000008b0: 2400 0000 7227 0000 0072 2900 0000 7207  $...r'...r)...r.
+000008c0: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
+000008d0: 0000 7202 0000 0004 0000 0073 1000 0000  ..r........s....
+000008e0: 0801 0201 1004 100b 100f 0807 140c 1205  ................
+000008f0: 7202 0000 0029 0372 1600 0000 720c 0000  r....).r....r...
+00000900: 0072 0200 0000 7207 0000 0072 0700 0000  .r....r....r....
+00000910: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
+00000920: 756c 653e 0100 0000 7304 0000 0008 0108  ule>....s.......
+00000930: 02                                       .
```

### Comparing `pandasai-0.0.2/pandasai/llm/__pycache__/fake.cpython-39.pyc` & `pandasai-0.0.3/pandasai/llm/__pycache__/fake.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.2/pandasai/llm/__pycache__/open_assistant.cpython-39.pyc` & `pandasai-0.0.3/pandasai/llm/__pycache__/open_assistant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr 22 21:05:01 2023 UTC, .py size: 953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,97 @@
-00000000: 610d 0d0a 0000 0000 fd4b 4464 b903 0000  a........KDd....
+00000000: 610d 0d0a 0000 0000 5685 4664 8b03 0000  a.......V.Fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6503 8300 0100 4700 6404  m.Z...e.....G.d.
-00000060: 6405 8400 6405 6505 8303 5a06 6401 5300  d...d.e...Z.d.S.
-00000070: 2906 e900 0000 004e 2901 da0b 6c6f 6164  )......N)...load
-00000080: 5f64 6f74 656e 7629 01da 034c 4c4d 6300  _dotenv)...LLMc.
-00000090: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000000a0: 0000 0040 0000 0073 5200 0000 6500 5a01  ...@...sR...e.Z.
-000000b0: 6400 5a02 5500 6503 6504 6401 3c00 640e  d.Z.U.e.e.d.<.d.
-000000c0: 6503 6403 9c01 6404 6405 8405 5a05 6406  e.d...d.d...Z.d.
-000000d0: 6407 8400 5a06 6503 6503 6503 6408 9c03  d...Z.e.e.e.d...
-000000e0: 6409 640a 8404 5a07 6508 6503 640b 9c01  d.d...Z.e.e.d...
-000000f0: 640c 640d 8404 8301 5a09 6402 5300 290f  d.d.....Z.d.S.).
-00000100: da0d 4f70 656e 4173 7369 7374 616e 74da  ..OpenAssistant.
-00000110: 0961 7069 5f74 6f6b 656e 4e29 0172 0500  .api_tokenN).r..
-00000120: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000130: 0000 0003 0000 0043 0000 0073 2600 0000  .......C...s&...
-00000140: 7c01 700c 7400 a001 6401 a101 7c00 5f02  |.p.t...d...|._.
-00000150: 7c00 6a02 6400 7500 7222 7403 6402 8301  |.j.d.u.r"t.d...
-00000160: 8201 6400 5300 2903 4e5a 1548 5547 4749  ..d.S.).NZ.HUGGI
-00000170: 4e47 4641 4345 5f41 5049 5f54 4f4b 454e  NGFACE_API_TOKEN
-00000180: 7a25 4875 6767 696e 6746 6163 6520 4875  z%HuggingFace Hu
-00000190: 6220 4150 4920 746f 6b65 6e20 6973 2072  b API token is r
-000001a0: 6571 7569 7265 6429 04da 026f 73da 0667  equired)...os..g
-000001b0: 6574 656e 7672 0500 0000 da09 4578 6365  etenvr......Exce
-000001c0: 7074 696f 6e29 02da 0473 656c 6672 0500  ption)...selfr..
-000001d0: 0000 a900 720a 0000 00fa 422f 5573 6572  ....r.....B/User
-000001e0: 732f 6761 6272 6965 6c65 7665 6e74 7572  s/gabrieleventur
-000001f0: 692f 5072 6f6a 6563 7473 2f61 692f 7061  i/Projects/ai/pa
-00000200: 6e64 6173 2d61 692f 6c6c 6d2f 6f70 656e  ndas-ai/llm/open
-00000210: 5f61 7373 6973 7461 6e74 2e70 79da 085f  _assistant.py.._
-00000220: 5f69 6e69 745f 5f0b 0000 0073 0600 0000  _init__....s....
-00000230: 0001 1001 0a01 7a16 4f70 656e 4173 7369  ......z.OpenAssi
-00000240: 7374 616e 742e 5f5f 696e 6974 5f5f 6302  stant.__init__c.
-00000250: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000260: 0000 0043 0000 0073 2c00 0000 6401 7d02  ...C...s,...d.}.
-00000270: 6402 6403 a000 7c00 6a01 a101 6901 7d03  d.d...|.j...i.}.
-00000280: 7402 6a03 7c02 7c03 7c01 6404 8d03 7d04  t.j.|.|.|.d...}.
-00000290: 7c04 a004 a100 5300 2905 4e7a 5068 7474  |.....S.).NzPhtt
-000002a0: 7073 3a2f 2f61 7069 2d69 6e66 6572 656e  ps://api-inferen
-000002b0: 6365 2e68 7567 6769 6e67 6661 6365 2e63  ce.huggingface.c
-000002c0: 6f2f 6d6f 6465 6c73 2f4f 7065 6e41 7373  o/models/OpenAss
-000002d0: 6973 7461 6e74 2f6f 6173 7374 2d73 6674  istant/oasst-sft
-000002e0: 2d31 2d70 7974 6869 612d 3132 625a 0d41  -1-pythia-12bZ.A
-000002f0: 7574 686f 7269 7a61 7469 6f6e 7a09 4265  uthorizationz.Be
-00000300: 6172 6572 207b 7d29 02da 0768 6561 6465  arer {})...heade
-00000310: 7273 da04 6a73 6f6e 2905 da06 666f 726d  rs..json)...form
-00000320: 6174 7205 0000 00da 0872 6571 7565 7374  atr......request
-00000330: 73da 0470 6f73 7472 0e00 0000 2905 7209  s..postr....).r.
-00000340: 0000 00da 0770 6179 6c6f 6164 5a07 4150  .....payloadZ.AP
-00000350: 495f 5552 4c72 0d00 0000 da08 7265 7370  I_URLr......resp
-00000360: 6f6e 7365 720a 0000 0072 0a00 0000 720b  onser....r....r.
-00000370: 0000 00da 0571 7565 7279 1000 0000 7308  .....query....s.
-00000380: 0000 0000 0104 0110 0210 017a 134f 7065  ...........z.Ope
-00000390: 6e41 7373 6973 7461 6e74 2e71 7565 7279  nAssistant.query
-000003a0: 2903 da0b 696e 7374 7275 6374 696f 6eda  )...instruction.
-000003b0: 0569 6e70 7574 da06 7265 7475 726e 6303  .input..returnc.
-000003c0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000003d0: 0000 0043 0000 0073 3400 0000 7c00 a000  ...C...s4...|...
-000003e0: 6401 6402 7c01 1700 7c02 1700 6403 1700  d.d.|...|...d...
-000003f0: 6901 a101 7d03 7401 7c02 8301 0100 7c00  i...}.t.|.....|.
-00000400: a002 7c03 6404 1900 6405 1900 a101 5300  ..|.d...d.....S.
-00000410: 2906 4eda 0669 6e70 7574 737a 0c3c 7c70  ).N..inputsz.<|p
-00000420: 726f 6d70 7465 727c 3e7a 0d3c 7c65 6e64  rompter|>z.<|end
-00000430: 6f66 7465 7874 7c3e 7201 0000 005a 0e67  oftext|>r....Z.g
-00000440: 656e 6572 6174 6564 5f74 6578 7429 0372  enerated_text).r
-00000450: 1400 0000 da05 7072 696e 74da 0d5f 6578  ......print.._ex
-00000460: 7472 6163 745f 636f 6465 2904 7209 0000  tract_code).r...
-00000470: 0072 1500 0000 7216 0000 00da 066f 7574  .r....r......out
-00000480: 7075 7472 0a00 0000 720a 0000 0072 0b00  putr....r....r..
-00000490: 0000 da04 6361 6c6c 1700 0000 730a 0000  ....call....s...
-000004a0: 0000 0104 0110 ff06 0408 027a 124f 7065  ...........z.Ope
-000004b0: 6e41 7373 6973 7461 6e74 2e63 616c 6c29  nAssistant.call)
-000004c0: 0172 1700 0000 6301 0000 0000 0000 0000  .r....c.........
-000004d0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000004e0: 0400 0000 6401 5300 2902 4e7a 0e6f 7065  ....d.S.).Nz.ope
-000004f0: 6e2d 6173 7369 7374 616e 7472 0a00 0000  n-assistantr....
-00000500: 2901 7209 0000 0072 0a00 0000 720a 0000  ).r....r....r...
-00000510: 0072 0b00 0000 da05 5f74 7970 6520 0000  .r......_type ..
-00000520: 0073 0200 0000 0002 7a13 4f70 656e 4173  .s......z.OpenAs
-00000530: 7369 7374 616e 742e 5f74 7970 6529 014e  sistant._type).N
-00000540: 290a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000550: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000560: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
-00000570: 6e6e 6f74 6174 696f 6e73 5f5f 720c 0000  nnotations__r...
-00000580: 0072 1400 0000 721c 0000 00da 0870 726f  .r....r......pro
-00000590: 7065 7274 7972 1d00 0000 720a 0000 0072  pertyr....r....r
-000005a0: 0a00 0000 720a 0000 0072 0b00 0000 7204  ....r....r....r.
-000005b0: 0000 0008 0000 0073 0c00 0000 0a01 0802  .......s........
-000005c0: 1005 0807 1209 0201 7204 0000 0029 0772  ........r....).r
-000005d0: 1000 0000 7206 0000 005a 0664 6f74 656e  ....r....Z.doten
-000005e0: 7672 0200 0000 da08 6c6c 6d2e 6261 7365  vr......llm.base
-000005f0: 7203 0000 0072 0400 0000 720a 0000 0072  r....r....r....r
-00000600: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-00000610: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000620: 0008 0108 010c 010c 0206 02              ...........
+00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6503 8300 0100 4700 6405  m.Z...e.....G.d.
+00000060: 6406 8400 6406 6505 8303 5a06 6401 5300  d...d.e...Z.d.S.
+00000070: 2907 e900 0000 004e 2901 da0b 6c6f 6164  )......N)...load
+00000080: 5f64 6f74 656e 76e9 0100 0000 2901 da03  _dotenv.....)...
+00000090: 4c4c 4d63 0000 0000 0000 0000 0000 0000  LLMc............
+000000a0: 0000 0000 0400 0000 4000 0000 7352 0000  ........@...sR..
+000000b0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
+000000c0: 013c 0064 0e65 0364 039c 0164 0464 0584  .<.d.e.d...d.d..
+000000d0: 055a 0564 0664 0784 005a 0665 0365 0365  .Z.d.d...Z.e.e.e
+000000e0: 0364 089c 0364 0964 0a84 045a 0765 0865  .d...d.d...Z.e.e
+000000f0: 0364 0b9c 0164 0c64 0d84 0483 015a 0964  .d...d.d.....Z.d
+00000100: 0253 0029 0fda 0d4f 7065 6e41 7373 6973  .S.)...OpenAssis
+00000110: 7461 6e74 da09 6170 695f 746f 6b65 6e4e  tant..api_tokenN
+00000120: 2901 7206 0000 0063 0200 0000 0000 0000  ).r....c........
+00000130: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000140: 7326 0000 007c 0170 0c74 00a0 0164 01a1  s&...|.p.t...d..
+00000150: 017c 005f 027c 006a 0264 0075 0072 2274  .|._.|.j.d.u.r"t
+00000160: 0364 0283 0182 0164 0053 0029 034e 5a13  .d.....d.S.).NZ.
+00000170: 4855 4747 494e 4746 4143 455f 4150 495f  HUGGINGFACE_API_
+00000180: 4b45 597a 2348 7567 6769 6e67 4661 6365  KEYz#HuggingFace
+00000190: 2048 7562 2041 5049 206b 6579 2069 7320   Hub API key is 
+000001a0: 7265 7175 6972 6564 2904 da02 6f73 da06  required)...os..
+000001b0: 6765 7465 6e76 7206 0000 00da 0945 7863  getenvr......Exc
+000001c0: 6570 7469 6f6e 2902 da04 7365 6c66 7206  eption)...selfr.
+000001d0: 0000 00a9 0072 0b00 0000 fa4b 2f55 7365  .....r.....K/Use
+000001e0: 7273 2f67 6162 7269 656c 6576 656e 7475  rs/gabrieleventu
+000001f0: 7269 2f50 726f 6a65 6374 732f 6169 2f70  ri/Projects/ai/p
+00000200: 616e 6461 732d 6169 2f70 616e 6461 7361  andas-ai/pandasa
+00000210: 692f 6c6c 6d2f 6f70 656e 5f61 7373 6973  i/llm/open_assis
+00000220: 7461 6e74 2e70 79da 085f 5f69 6e69 745f  tant.py..__init_
+00000230: 5f0b 0000 0073 0600 0000 0001 1001 0a01  _....s..........
+00000240: 7a16 4f70 656e 4173 7369 7374 616e 742e  z.OpenAssistant.
+00000250: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
+00000260: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+00000270: 0073 2c00 0000 6401 7d02 6402 6403 a000  .s,...d.}.d.d...
+00000280: 7c00 6a01 a101 6901 7d03 7402 6a03 7c02  |.j...i.}.t.j.|.
+00000290: 7c03 7c01 6404 8d03 7d04 7c04 a004 a100  |.|.d...}.|.....
+000002a0: 5300 2905 4e7a 5068 7474 7073 3a2f 2f61  S.).NzPhttps://a
+000002b0: 7069 2d69 6e66 6572 656e 6365 2e68 7567  pi-inference.hug
+000002c0: 6769 6e67 6661 6365 2e63 6f2f 6d6f 6465  gingface.co/mode
+000002d0: 6c73 2f4f 7065 6e41 7373 6973 7461 6e74  ls/OpenAssistant
+000002e0: 2f6f 6173 7374 2d73 6674 2d31 2d70 7974  /oasst-sft-1-pyt
+000002f0: 6869 612d 3132 625a 0d41 7574 686f 7269  hia-12bZ.Authori
+00000300: 7a61 7469 6f6e 7a09 4265 6172 6572 207b  zationz.Bearer {
+00000310: 7d29 02da 0768 6561 6465 7273 da04 6a73  })...headers..js
+00000320: 6f6e 2905 da06 666f 726d 6174 7206 0000  on)...formatr...
+00000330: 00da 0872 6571 7565 7374 73da 0470 6f73  ...requests..pos
+00000340: 7472 0f00 0000 2905 720a 0000 00da 0770  tr....).r......p
+00000350: 6179 6c6f 6164 5a07 4150 495f 5552 4c72  ayloadZ.API_URLr
+00000360: 0e00 0000 da08 7265 7370 6f6e 7365 720b  ......responser.
+00000370: 0000 0072 0b00 0000 720c 0000 00da 0571  ...r....r......q
+00000380: 7565 7279 1000 0000 7308 0000 0000 0104  uery....s.......
+00000390: 0110 0210 017a 134f 7065 6e41 7373 6973  .....z.OpenAssis
+000003a0: 7461 6e74 2e71 7565 7279 2903 da0b 696e  tant.query)...in
+000003b0: 7374 7275 6374 696f 6eda 0569 6e70 7574  struction..input
+000003c0: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
+000003d0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+000003e0: 0073 2600 0000 7c00 a000 6401 6402 7c01  .s&...|...d.d.|.
+000003f0: 1700 7c02 1700 6403 1700 6901 a101 7d03  ..|...d...i...}.
+00000400: 7c03 6404 1900 6405 1900 5300 2906 4eda  |.d...d...S.).N.
+00000410: 0669 6e70 7574 737a 0c3c 7c70 726f 6d70  .inputsz.<|promp
+00000420: 7465 727c 3e7a 0d3c 7c65 6e64 6f66 7465  ter|>z.<|endofte
+00000430: 7874 7c3e 7201 0000 005a 0e67 656e 6572  xt|>r....Z.gener
+00000440: 6174 6564 5f74 6578 7429 0172 1500 0000  ated_text).r....
+00000450: 2904 720a 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000460: 00da 066f 7574 7075 7472 0b00 0000 720b  ...outputr....r.
+00000470: 0000 0072 0c00 0000 da04 6361 6c6c 1700  ...r......call..
+00000480: 0000 7308 0000 0000 0104 0110 ff06 037a  ..s............z
+00000490: 124f 7065 6e41 7373 6973 7461 6e74 2e63  .OpenAssistant.c
+000004a0: 616c 6c29 0172 1800 0000 6301 0000 0000  all).r....c.....
+000004b0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+000004c0: 0000 0073 0400 0000 6401 5300 2902 4e7a  ...s....d.S.).Nz
+000004d0: 0e6f 7065 6e2d 6173 7369 7374 616e 7472  .open-assistantr
+000004e0: 0b00 0000 2901 720a 0000 0072 0b00 0000  ....).r....r....
+000004f0: 720b 0000 0072 0c00 0000 da05 5f74 7970  r....r......_typ
+00000500: 651d 0000 0073 0200 0000 0002 7a13 4f70  e....s......z.Op
+00000510: 656e 4173 7369 7374 616e 742e 5f74 7970  enAssistant._typ
+00000520: 6529 014e 290a da08 5f5f 6e61 6d65 5f5f  e).N)...__name__
+00000530: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000540: 7175 616c 6e61 6d65 5f5f da03 7374 72da  qualname__..str.
+00000550: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000560: 720d 0000 0072 1500 0000 721b 0000 00da  r....r....r.....
+00000570: 0870 726f 7065 7274 7972 1c00 0000 720b  .propertyr....r.
+00000580: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000590: 0000 7205 0000 0008 0000 0073 0c00 0000  ..r........s....
+000005a0: 0a01 0802 1005 0807 1206 0201 7205 0000  ............r...
+000005b0: 0029 0772 1100 0000 7207 0000 005a 0664  .).r....r....Z.d
+000005c0: 6f74 656e 7672 0200 0000 da04 6261 7365  otenvr......base
+000005d0: 7204 0000 0072 0500 0000 720b 0000 0072  r....r....r....r
+000005e0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
+000005f0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000600: 0008 0108 010c 010c 0206 02              ...........
```

### Comparing `pandasai-0.0.2/pandasai/llm/__pycache__/openai.cpython-39.pyc` & `pandasai-0.0.3/pandasai/llm/__pycache__/openai.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 13:38:49 2023 UTC, .py size: 2533 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6986 4664 e509 0000  a.......i.Fd....
+00000000: 610d 0d0a 0000 0000 8206 4764 e509 0000  a.........Gd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c05 5a05 6502 8300 0100 4700 6405  d.l.Z.e.....G.d.
 00000060: 6406 8400 6406 6504 8303 5a06 6401 5300  d...d.e...Z.d.S.
 00000070: 2907 e900 0000 004e 2901 da0b 6c6f 6164  )......N)...load
@@ -21,23 +21,23 @@
 00000140: 1484 045a 0f65 0365 0364 129c 0264 1564  ...Z.e.e.d...d.d
 00000150: 1684 045a 1065 0365 0365 0364 179c 0364  ...Z.e.e.e.d...d
 00000160: 1864 1984 045a 1165 1265 0364 1a9c 0164  .d...Z.e.e.d...d
 00000170: 1b64 1c84 0483 015a 1364 0d53 0029 1eda  .d.....Z.d.S.)..
 00000180: 064f 7065 6e41 49da 0961 7069 5f74 6f6b  .OpenAI..api_tok
 00000190: 656e fa0d 6770 742d 332e 352d 7475 7262  en..gpt-3.5-turb
 000001a0: 6fda 056d 6f64 656c 7201 0000 00da 0b74  o..modelr......t
-000001b0: 656d 7065 7261 7475 7265 e996 0000 00da  emperature......
+000001b0: 656d 7065 7261 7475 7265 6900 0200 00da  emperaturei.....
 000001c0: 0a6d 6178 5f74 6f6b 656e 7372 0300 0000  .max_tokensr....
 000001d0: da05 746f 705f 70da 1166 7265 7175 656e  ..top_p..frequen
 000001e0: 6379 5f70 656e 616c 7479 6733 3333 3333  cy_penaltyg33333
 000001f0: 33e3 3fda 1070 7265 7365 6e63 655f 7065  3.?..presence_pe
 00000200: 6e61 6c74 794e da04 7374 6f70 2908 7206  naltyN..stop).r.
-00000210: 0000 0072 0800 0000 7209 0000 0072 0b00  ...r....r....r..
-00000220: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000230: 0072 0f00 0000 6309 0000 0000 0000 0000  .r....c.........
+00000210: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000220: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000230: 0072 0e00 0000 6309 0000 0000 0000 0000  .r....c.........
 00000240: 0000 0009 0000 0003 0000 0043 0000 0073  ...........C...s
 00000250: 8200 0000 7c01 700c 7400 a001 6401 a101  ....|.p.t...d...
 00000260: 7c00 5f02 7c00 6a02 6400 7500 7222 7403  |._.|.j.d.u.r"t.
 00000270: 6402 8301 8201 7c00 6a02 7404 5f05 7c02  d.....|.j.t._.|.
 00000280: 7032 7c00 6a06 7c00 5f06 7c03 703e 7c00  p2|.j.|._.|.p>|.
 00000290: 6a07 7c00 5f07 7c04 704a 7c00 6a08 7c00  j.|._.|.pJ|.j.|.
 000002a0: 5f08 7c05 7056 7c00 6a09 7c00 5f09 7c06  _.|.pV|.j.|._.|.
@@ -45,20 +45,20 @@
 000002c0: 6a0b 7c00 5f0b 7c08 707a 7c00 6a0c 7c00  j.|._.|.pz|.j.|.
 000002d0: 5f0c 6400 5300 2903 4e5a 0e4f 5045 4e41  _.d.S.).NZ.OPENA
 000002e0: 495f 4150 495f 4b45 597a 1a4f 7065 6e41  I_API_KEYz.OpenA
 000002f0: 4920 4150 4920 6b65 7920 6973 2072 6571  I API key is req
 00000300: 7569 7265 6429 0dda 026f 73da 0667 6574  uired)...os..get
 00000310: 656e 7672 0600 0000 da09 4578 6365 7074  envr......Except
 00000320: 696f 6eda 066f 7065 6e61 695a 0761 7069  ion..openaiZ.api
-00000330: 5f6b 6579 7208 0000 0072 0900 0000 720b  _keyr....r....r.
-00000340: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000350: 0000 720f 0000 0029 09da 0473 656c 6672  ..r....)...selfr
-00000360: 0600 0000 7208 0000 0072 0900 0000 720b  ....r....r....r.
-00000370: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000380: 0000 720f 0000 00a9 0072 1500 0000 fa43  ..r......r.....C
+00000330: 5f6b 6579 7208 0000 0072 0900 0000 720a  _keyr....r....r.
+00000340: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000350: 0000 720e 0000 0029 09da 0473 656c 6672  ..r....)...selfr
+00000360: 0600 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00000370: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000380: 0000 720e 0000 00a9 0072 1400 0000 fa43  ..r......r.....C
 00000390: 2f55 7365 7273 2f67 6162 7269 656c 6576  /Users/gabrielev
 000003a0: 656e 7475 7269 2f50 726f 6a65 6374 732f  enturi/Projects/
 000003b0: 6169 2f70 616e 6461 732d 6169 2f70 616e  ai/pandas-ai/pan
 000003c0: 6461 7361 692f 6c6c 6d2f 6f70 656e 6169  dasai/llm/openai
 000003d0: 2e70 79da 085f 5f69 6e69 745f 5f12 0000  .py..__init__...
 000003e0: 0073 1600 0000 0001 1001 0a01 0801 0802  .s..............
 000003f0: 0c01 0c01 0c01 0c01 0c01 0c01 7a0f 4f70  ............z.Op
@@ -68,90 +68,90 @@
 00000430: 0800 0000 4300 0000 7358 0000 007c 006a  ....C...sX...|.j
 00000440: 007c 017c 006a 017c 006a 027c 006a 037c  .|.|.j.|.j.|.j.|
 00000450: 006a 047c 006a 0564 019c 077d 027c 006a  .j.|.j.d...}.|.j
 00000460: 0664 0075 0172 367c 006a 0667 017c 0264  .d.u.r6|.j.g.|.d
 00000470: 023c 0074 076a 086a 0966 0069 007c 02a4  .<.t.j.j.f.i.|..
 00000480: 018e 017d 037c 0364 0319 0064 0419 0064  ...}.|.d...d...d
 00000490: 0519 0053 0029 064e 2907 7208 0000 0072  ...S.).N).r....r
-000004a0: 1800 0000 7209 0000 0072 0b00 0000 720c  ....r....r....r.
-000004b0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+000004a0: 1700 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+000004b0: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
 000004c0: 0000 da07 6368 6f69 6365 7372 0100 0000  ....choicesr....
 000004d0: da04 7465 7874 290a 7208 0000 0072 0900  ..text).r....r..
-000004e0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-000004f0: 0072 0e00 0000 720f 0000 0072 1300 0000  .r....r....r....
+000004e0: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+000004f0: 0072 0d00 0000 720e 0000 0072 1200 0000  .r....r....r....
 00000500: 5a0a 436f 6d70 6c65 7469 6f6e da06 6372  Z.Completion..cr
-00000510: 6561 7465 a904 7214 0000 0072 1800 0000  eate..r....r....
+00000510: 6561 7465 a904 7213 0000 0072 1700 0000  eate..r....r....
 00000520: da06 7061 7261 6d73 da08 7265 7370 6f6e  ..params..respon
-00000530: 7365 7215 0000 0072 1500 0000 7216 0000  ser....r....r...
+00000530: 7365 7214 0000 0072 1400 0000 7215 0000  ser....r....r...
 00000540: 00da 0a63 6f6d 706c 6574 696f 6e20 0000  ...completion ..
 00000550: 0073 1800 0000 0002 0401 0201 0401 0401  .s..............
 00000560: 0401 0401 04f9 060a 0a01 0c02 1202 7a11  ..............z.
 00000570: 4f70 656e 4149 2e63 6f6d 706c 6574 696f  OpenAI.completio
 00000580: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
 00000590: 0000 0900 0000 4300 0000 7364 0000 007c  ......C...sd...|
 000005a0: 006a 007c 006a 017c 006a 027c 006a 037c  .j.|.j.|.j.|.j.|
 000005b0: 006a 047c 006a 0564 017c 0164 029c 0267  .j.|.j.d.|.d...g
 000005c0: 0164 039c 077d 027c 006a 0664 0075 0172  .d...}.|.j.d.u.r
 000005d0: 3e7c 006a 0667 017c 0264 043c 0074 076a  >|.j.g.|.d.<.t.j
 000005e0: 086a 0966 0069 007c 02a4 018e 017d 037c  .j.f.i.|.....}.|
 000005f0: 0364 0519 0064 0619 0064 0719 0064 0819  .d...d...d...d..
 00000600: 0053 0029 094e da06 7379 7374 656d 2902  .S.).N..system).
 00000610: 5a04 726f 6c65 da07 636f 6e74 656e 7429  Z.role..content)
-00000620: 0772 0800 0000 7209 0000 0072 0b00 0000  .r....r....r....
-00000630: 720c 0000 0072 0d00 0000 720e 0000 005a  r....r....r....Z
-00000640: 086d 6573 7361 6765 7372 0f00 0000 721a  .messagesr....r.
+00000620: 0772 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000630: 720b 0000 0072 0c00 0000 720d 0000 005a  r....r....r....Z
+00000640: 086d 6573 7361 6765 7372 0e00 0000 7219  .messagesr....r.
 00000650: 0000 0072 0100 0000 da07 6d65 7373 6167  ...r......messag
-00000660: 6572 2200 0000 290a 7208 0000 0072 0900  er"...).r....r..
-00000670: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000680: 0072 0e00 0000 720f 0000 0072 1300 0000  .r....r....r....
+00000660: 6572 2100 0000 290a 7208 0000 0072 0900  er!...).r....r..
+00000670: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000680: 0072 0d00 0000 720e 0000 0072 1200 0000  .r....r....r....
 00000690: 5a0e 4368 6174 436f 6d70 6c65 7469 6f6e  Z.ChatCompletion
-000006a0: 721c 0000 0072 1d00 0000 7215 0000 0072  r....r....r....r
-000006b0: 1500 0000 7216 0000 00da 0f63 6861 745f  ....r......chat_
+000006a0: 721b 0000 0072 1c00 0000 7214 0000 0072  r....r....r....r
+000006b0: 1400 0000 7215 0000 00da 0f63 6861 745f  ....r......chat_
 000006c0: 636f 6d70 6c65 7469 6f6e 3200 0000 731c  completion2...s.
 000006d0: 0000 0000 0204 0104 0104 0104 0104 0104  ................
 000006e0: 0202 0102 fe06 f906 0d0a 010c 0212 027a  ...............z
 000006f0: 164f 7065 6e41 492e 6368 6174 5f63 6f6d  .OpenAI.chat_com
 00000700: 706c 6574 696f 6e29 03da 0b69 6e73 7472  pletion)...instr
-00000710: 7563 7469 6f6e da05 696e 7075 7472 1900  uction..inputr..
+00000710: 7563 7469 6f6e da05 696e 7075 7472 1800  uction..inputr..
 00000720: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
 00000730: 0000 0005 0000 0043 0000 0073 5000 0000  .......C...sP...
 00000740: 7c00 6a00 6401 6b02 7222 7c00 a001 7402  |.j.d.k.r"|...t.
 00000750: 7c01 8301 7402 7c02 8301 1700 a101 7d03  |...t.|.......}.
 00000760: 6e2a 7c00 6a00 6402 6b02 7244 7c00 a003  n*|.j.d.k.rD|...
 00000770: 7402 7c01 8301 7402 7c02 8301 1700 a101  t.|...t.|.......
 00000780: 7d03 6e08 7404 6403 8301 8201 7c03 5300  }.n.t.d.....|.S.
 00000790: 2904 4e7a 1074 6578 742d 6461 7669 6e63  ).Nz.text-davinc
 000007a0: 692d 3030 3372 0700 0000 7a11 556e 7375  i-003r....z.Unsu
 000007b0: 7070 6f72 7465 6420 6d6f 6465 6c29 0572  pported model).r
-000007c0: 0800 0000 7220 0000 00da 0373 7472 7224  ....r .....strr$
-000007d0: 0000 0072 1200 0000 2904 7214 0000 0072  ...r....).r....r
-000007e0: 2500 0000 7226 0000 0072 1f00 0000 7215  %...r&...r....r.
-000007f0: 0000 0072 1500 0000 7216 0000 00da 0463  ...r....r......c
+000007c0: 0800 0000 721f 0000 00da 0373 7472 7223  ....r......strr#
+000007d0: 0000 0072 1100 0000 2904 7213 0000 0072  ...r....).r....r
+000007e0: 2400 0000 7225 0000 0072 1e00 0000 7214  $...r%...r....r.
+000007f0: 0000 0072 1400 0000 7215 0000 00da 0463  ...r....r......c
 00000800: 616c 6c47 0000 0073 0c00 0000 0001 0a01  allG...s........
 00000810: 1801 0a01 1802 0802 7a0b 4f70 656e 4149  ........z.OpenAI
-00000820: 2e63 616c 6c29 0172 1900 0000 6301 0000  .call).r....c...
+00000820: 2e63 616c 6c29 0172 1800 0000 6301 0000  .call).r....c...
 00000830: 0000 0000 0000 0000 0001 0000 0001 0000  ................
 00000840: 0043 0000 0073 0400 0000 6401 5300 2902  .C...s....d.S.).
-00000850: 4e72 1300 0000 7215 0000 0029 0172 1400  Nr....r....).r..
-00000860: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000850: 4e72 1200 0000 7214 0000 0029 0172 1300  Nr....r....).r..
+00000860: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
 00000870: 00da 055f 7479 7065 5100 0000 7302 0000  ..._typeQ...s...
 00000880: 0000 027a 0c4f 7065 6e41 492e 5f74 7970  ...z.OpenAI._typ
 00000890: 6529 084e 4e4e 4e4e 4e4e 4e29 14da 085f  e).NNNNNNNN)..._
 000008a0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 000008b0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000008c0: 5f72 2700 0000 da0f 5f5f 616e 6e6f 7461  _r'.....__annota
+000008c0: 5f72 2600 0000 da0f 5f5f 616e 6e6f 7461  _r&.....__annota
 000008d0: 7469 6f6e 735f 5f72 0800 0000 7209 0000  tions__r....r...
-000008e0: 00da 0566 6c6f 6174 720b 0000 00da 0369  ...floatr......i
-000008f0: 6e74 720c 0000 0072 0d00 0000 720e 0000  ntr....r....r...
-00000900: 0072 0f00 0000 7217 0000 0072 2000 0000  .r....r....r ...
-00000910: 7224 0000 0072 2800 0000 da08 7072 6f70  r$...r(.....prop
-00000920: 6572 7479 7229 0000 0072 1500 0000 7215  ertyr)...r....r.
-00000930: 0000 0072 1500 0000 7216 0000 0072 0500  ...r....r....r..
+000008e0: 00da 0566 6c6f 6174 720a 0000 00da 0369  ...floatr......i
+000008f0: 6e74 720b 0000 0072 0c00 0000 720d 0000  ntr....r....r...
+00000900: 0072 0e00 0000 7216 0000 0072 1f00 0000  .r....r....r....
+00000910: 7223 0000 0072 2700 0000 da08 7072 6f70  r#...r'.....prop
+00000920: 6572 7479 7228 0000 0072 1400 0000 7214  ertyr(...r....r.
+00000930: 0000 0072 1400 0000 7215 0000 0072 0500  ...r....r....r..
 00000940: 0000 0800 0000 731c 0000 000a 0108 010c  ......s.........
 00000950: 010c 010c 010c 010c 010c 010c 021e 0e10  ................
-00000960: 1210 1512 0a02 0172 0500 0000 2907 7210  .......r....).r.
+00000960: 1210 1512 0a02 0172 0500 0000 2907 720f  .......r....).r.
 00000970: 0000 005a 0664 6f74 656e 7672 0200 0000  ...Z.dotenvr....
-00000980: da04 6261 7365 7204 0000 0072 1300 0000  ..baser....r....
-00000990: 7205 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000009a0: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
+00000980: da04 6261 7365 7204 0000 0072 1200 0000  ..baser....r....
+00000990: 7205 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+000009a0: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
 000009b0: 6c65 3e01 0000 0073 0a00 0000 0801 0c01  le>....s........
 000009c0: 0c01 0802 0602                           ......
```

### Comparing `pandasai-0.0.2/pandasai/llm/alpaca.py` & `pandasai-0.0.3/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.2/pandasai/llm/base.py` & `pandasai-0.0.3/pandasai/llm/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
 import ast
+import astor
 
 class LLM:
   @property
   def _type(self) -> str:
     """Return type of llm."""
     raise Exception("Type has not been implemented")
   
   def _remove_imports(self, code: str) -> str:
     tree = ast.parse(code)
+    new_body = []
 
-    for node in tree.body[:]:
-      if isinstance(node, ast.Import):
-        for name in node.names:
-          node.names.remove(name)
-        if not node.names:
-          tree.body.remove(node)
-      elif isinstance(node, ast.ImportFrom):
-        tree.body.remove(node)
+    for node in tree.body:
+        if not isinstance(node, (ast.Import, ast.ImportFrom)):
+            new_body.append(node)
 
-    return ast.unparse(tree)
+    new_tree = ast.Module(body=new_body)
+    return astor.to_source(new_tree)
 
   def _polish_code(self, code: str) -> str:
     """Polish the code:
     - remove the leading "python" or "py"
     - remove the imports
     - remove trailing spaces and new lines
     """
```

### Comparing `pandasai-0.0.2/pandasai/llm/open_assistant.py` & `pandasai-0.0.3/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.2/pandasai/llm/openai.py` & `pandasai-0.0.3/pandasai/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 load_dotenv()
 
 class OpenAI(LLM):
   api_token: str
   model: str = "gpt-3.5-turbo"
   temperature: float = 0
-  max_tokens: int = 150
+  max_tokens: int = 512
   top_p: float = 1
   frequency_penalty: float = 0
   presence_penalty: float = 0.6
   stop: str = None
 
   def __init__(self, api_token: str = None, model: str = None, temperature: float = None, max_tokens: int = None, top_p: float = None, frequency_penalty: float = None, presence_penalty: float = None, stop: str = None):
     self.api_token = api_token or os.getenv("OPENAI_API_KEY")
```

### Comparing `pandasai-0.0.2/pandasai.egg-info/PKG-INFO` & `pandasai-0.0.3/pandasai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper around pandas to make it conversational
 Author: Gabriele Venturi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -63,19 +63,44 @@
 
 The above code will return the following:
 
 ```
 14516000
 ```
 
+You can find more examples in the [examples](examples) directory.
+
+## Environment Variables
+
+In order to set the API key for the LLM (HuggingFaceHub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
+
+```bash
+cp .env.example .env
+```
+
+Then, edit the `.env` file and set the appropriate values.
+
+As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
+
+```python
+# OpenAI
+llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
+
+# OpenAssistant
+llm = OpenAssistant(api_token="YOUR_HF_API_KEY")
+```
+
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
-Contributions are welcome!
+Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 
 ### Todo
 
 - [ ] Add support for more LLMs
+- [ ] Make PandasAI available from a CLI
+- [ ] Create a web interface for PandasAI
+- [ ] Add CI/CD
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.0.2/pandasai.egg-info/SOURCES.txt` & `pandasai-0.0.3/pandasai.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 README.md
 setup.py
 pandasai/__init__.py
 pandasai.egg-info/PKG-INFO
 pandasai.egg-info/SOURCES.txt
 pandasai.egg-info/dependency_links.txt
 pandasai.egg-info/top_level.txt
+pandasai/__pycache__/__init__.cpython-38.pyc
 pandasai/__pycache__/__init__.cpython-39.pyc
 pandasai/llm/__init__.py
 pandasai/llm/alpaca.py
 pandasai/llm/base.py
 pandasai/llm/fake.py
 pandasai/llm/open_assistant.py
 pandasai/llm/openai.py
+pandasai/llm/__pycache__/__init__.cpython-38.pyc
 pandasai/llm/__pycache__/__init__.cpython-39.pyc
+pandasai/llm/__pycache__/alpaca.cpython-38.pyc
 pandasai/llm/__pycache__/alpaca.cpython-39.pyc
+pandasai/llm/__pycache__/base.cpython-38.pyc
 pandasai/llm/__pycache__/base.cpython-39.pyc
 pandasai/llm/__pycache__/fake.cpython-39.pyc
 pandasai/llm/__pycache__/open_assistant.cpython-39.pyc
 pandasai/llm/__pycache__/openai.cpython-39.pyc
```

### Comparing `pandasai-0.0.2/setup.py` & `pandasai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandasai",
-    version="0.0.2",
+    version="0.0.3",
     author="Gabriele Venturi",
     description="A wrapper around pandas to make it conversational",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```


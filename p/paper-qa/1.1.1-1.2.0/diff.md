# Comparing `tmp/paper-qa-1.1.1.tar.gz` & `tmp/paper-qa-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.1.1.tar", last modified: Tue Apr 11 06:03:49 2023, max compression
+gzip compressed data, was "paper-qa-1.2.0.tar", last modified: Thu Apr 27 07:47:24 2023, max compression
```

## Comparing `paper-qa-1.1.1.tar` & `paper-qa-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:03:23.000000 paper-qa-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-11 06:03:49.005178 paper-qa-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-11 06:03:23.000000 paper-qa-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 06:03:49.000000 paper-qa-1.1.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 06:03:48.000000 paper-qa-1.1.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 06:03:23.000000 paper-qa-1.1.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:03:49.005178 paper-qa-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 06:03:23.000000 paper-qa-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:03:49.005178 paper-qa-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-11 06:03:23.000000 paper-qa-1.1.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 07:46:47.000000 paper-qa-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-27 07:47:24.859447 paper-qa-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-27 07:46:47.000000 paper-qa-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.855447 paper-qa-1.2.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.855447 paper-qa-1.2.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:47:24.859447 paper-qa-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-27 07:46:47.000000 paper-qa-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-27 07:46:47.000000 paper-qa-1.2.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.1.1/LICENSE` & `paper-qa-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/PKG-INFO` & `paper-qa-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.1.1
+Version: 1.2.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.1.1/README.md` & `paper-qa-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.2.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.1.1
+Version: 1.2.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.1.1/paperqa/agent.py` & `paper-qa-1.2.0/paperqa/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from langchain.tools import BaseTool
 from .docs import Answer, Docs
 from langchain.agents import initialize_agent
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import LLMChain
+from langchain.agents import AgentType
 from .qaprompts import select_paper_prompt, make_chain
+from rmrkl import ChatZeroShotAgent, RetryAgentExecutor
 
 
 def status(answer: Answer, docs: Docs):
-    return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: {answer.cost}"
+    return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: ${answer.cost:.2f}"
 
 
 class PaperSelection(BaseTool):
     name = "Select Papers"
     description = "Select from current papers. Provide instructions as a string to use for choosing papers."
     docs: Docs = None
     answer: Answer = None
@@ -36,34 +38,34 @@
         raise NotImplementedError()
 
 
 class ReadPapers(BaseTool):
     name = "Gather Evidence"
     description = (
         "Give a specific question to a researcher that will return evidence for it. "
-        # "Optionally, you may specify papers using their key provided by the Select Papers tool. "
-        # "Use the format: $QUESTION or use format $QUESTION|$KEY1,$KEY2,..."
+        "Optionally, you may specify papers using their key provided by the Select Papers tool. "
+        "Use the format: $QUESTION or use format $QUESTION|$KEY1,$KEY2,..."
     )
     docs: Docs = None
     answer: Answer = None
 
     def __init__(self, docs, answer):
         # call the parent class constructor
         super(ReadPapers, self).__init__()
 
         self.docs = docs
         self.answer = answer
 
     def _run(self, query: str) -> str:
-        # if "|" in query:
-        #     question, keys = query.split("|")
-        #     keys = [k.strip() for k in keys.split(",")]
-        # else:
-        question = query
-        keys = None
+        if "|" in query:
+            question, keys = query.split("|")
+            keys = [k.strip() for k in keys.split(",")]
+        else:
+            question = query
+            keys = None
         # swap out the question
         old = self.answer.question
         self.answer.question = question
         # generator, so run it
         l0 = len(self.answer.contexts)
         self.docs.get_evidence(self.answer, key_filter=keys)
         l1 = len(self.answer.contexts)
@@ -86,19 +88,19 @@
         super(AnswerTool, self).__init__()
 
         self.docs = docs
         self.answer = answer
 
     def _run(self, query: str) -> str:
         self.answer = self.docs.query(
-            query, answer=self.answer, length_prompt="length as long as needed"
+            query, answer=self.answer
         )
         if "cannot answer" in self.answer.answer:
             self.answer = Answer(self.answer.question)
-            return "Failed to answer question. Deleting evidence." + status(
+            return "Failed to answer question. Deleting evidence. Consider rephrasing question or evidence statement." + status(
                 self.answer, self.docs
             )
         return self.answer.answer + status(self.answer, self.docs)
 
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
@@ -137,36 +139,32 @@
 
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
 
 
 def make_tools(docs, answer):
-    # putting here until langchain PR is merged
-    from langchain.tools.exception.tool import ExceptionTool
 
     tools = []
 
     tools.append(Search(docs, answer))
-    # tools.append(PaperSelection(docs, answer))
+    tools.append(PaperSelection(docs, answer))
     tools.append(ReadPapers(docs, answer))
     tools.append(AnswerTool(docs, answer))
-    tools.append(ExceptionTool())
     return tools
 
 
 def run_agent(docs, question, llm=None):
     if llm is None:
-        llm = ChatOpenAI(temperature=0.1, model="gpt-4")
+        llm = ChatOpenAI(temperature=0.0, model="gpt-4")
     answer = Answer(question)
     tools = make_tools(docs, answer)
-    mrkl = initialize_agent(
-        tools,
-        llm,
-        agent="chat-zero-shot-react-description",
+    mrkl = RetryAgentExecutor.from_agent_and_tools(
+        tools=tools,
+        agent=ChatZeroShotAgent.from_llm_and_tools(llm, tools),
         verbose=True,
     )
     mrkl.run(
         f"Answer question: {question}. Search for papers, gather evidence, and answer. If you do not have enough evidence, you can search for more papers (preferred) or gather more evidence. You may rephrase or breaking-up the question in those steps. "
         "Once you have five pieces of evidence, or you have tried for a while, call the Propose Answer tool. "
     )
```

### Comparing `paper-qa-1.1.1/paperqa/contrib/zotero.py` & `paper-qa-1.2.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/paperqa/docs.py` & `paper-qa-1.2.0/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/paperqa/qaprompts.py` & `paper-qa-1.2.0/paperqa/qaprompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     template="Write an answer ({length}) "
     "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
     "For each sentence in your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
     "Answer in an unbiased, comprehensive, and scholarly tone. "
+    "Complete your answer with a concluding 1-2 sentences, which may be opinionated. "
     "Use Markdown for formatting code or text, and try to use direct quotes to support arguments.\n\n"
     "{context_str}\n"
     "Question: {question}\n"
     "Answer: ",
 )
```

### Comparing `paper-qa-1.1.1/paperqa/readers.py` & `paper-qa-1.2.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/paperqa/types.py` & `paper-qa-1.2.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/paperqa/utils.py` & `paper-qa-1.2.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.1.1/setup.py` & `paper-qa-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         "pypdf",
         "langchain>=0.0.129",
         "openai>=0.27.0",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
+        "rmrkl"
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `paper-qa-1.1.1/tests/test_paperqa.py` & `paper-qa-1.2.0/tests/test_paperqa.py`

 * *Files identical despite different names*


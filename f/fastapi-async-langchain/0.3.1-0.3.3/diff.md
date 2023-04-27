# Comparing `tmp/fastapi_async_langchain-0.3.1.tar.gz` & `tmp/fastapi_async_langchain-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.3.1.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.3.3.tar", max compression
```

## Comparing `fastapi_async_langchain-0.3.1.tar` & `fastapi_async_langchain-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-04-24 14:54:18.787740 fastapi_async_langchain-0.3.1/LICENSE
--rw-r--r--   0        0        0     1574 2023-04-24 14:54:18.787740 fastapi_async_langchain-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      648 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/callback.py
--rw-r--r--   0        0        0      171 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     1839 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0     1182 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0     1493 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      481 2023-04-24 14:54:18.791740 fastapi_async_langchain-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 08:16:52.334951 fastapi_async_langchain-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1574 2023-04-27 08:16:52.334951 fastapi_async_langchain-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      648 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/base.py
+-rw-r--r--   0        0        0      733 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      171 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     1839 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0     1183 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0     1512 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      481 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.3.3/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.3.1/LICENSE` & `fastapi_async_langchain-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.3.1/README.md` & `fastapi_async_langchain-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.3.1/fastapi_async_langchain/callback.py` & `fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/base.py` & `fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/llm.py` & `fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Union
 
 from langchain import LLMChain
 from langchain.callbacks import AsyncCallbackManager
 from starlette.types import Send
 
-from ..callback import AsyncFastApiStreamingCallback
+from ..callbacks import AsyncFastApiStreamingCallback
 from .base import BaseLangchainStreamingResponse
 
 
 class LLMChainStreamingResponse(BaseLangchainStreamingResponse):
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
```

### Comparing `fastapi_async_langchain-0.3.1/fastapi_async_langchain/responses/retrieval_qa.py` & `fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/retrieval_qa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Union
 
 from langchain.callbacks import AsyncCallbackManager
 from langchain.chains.retrieval_qa.base import BaseRetrievalQA
 from starlette.types import Send
 
-from ..callback import AsyncFastApiStreamingCallback
+from ..callbacks import RetrievalQAFastApiStreamingCallback
 from .base import BaseLangchainStreamingResponse
 
 
 class RetrievalQAStreamingResponse(BaseLangchainStreamingResponse):
     """BaseLangchainStreamingResponse class wrapper for BaseRetrievalQA instances."""
 
     @staticmethod
@@ -20,18 +20,18 @@
             ):
                 raise TypeError(
                     "llm.callback_manager must be an instance of AsyncCallbackManager"
                 )
             for (
                 handler
             ) in chain.combine_documents_chain.llm_chain.llm.callback_manager.handlers:
-                if isinstance(handler, AsyncFastApiStreamingCallback):
+                if isinstance(handler, RetrievalQAFastApiStreamingCallback):
                     chain.combine_documents_chain.llm_chain.llm.callback_manager.remove_handler(
                         handler
                     )
                     break
             chain.combine_documents_chain.llm_chain.llm.callback_manager.add_handler(
-                AsyncFastApiStreamingCallback(send=send)
+                RetrievalQAFastApiStreamingCallback(send=send)
             )
             return await chain.acall(inputs)
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.3.1/PKG-INFO` & `fastapi_async_langchain-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.3.1
+Version: 0.3.3
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: langchain (>=0.0.144,<0.0.145)
+Requires-Dist: langchain (>=0.0.146,<0.0.147)
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
```


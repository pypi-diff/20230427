# Comparing `tmp/cohere-4.2.1.tar.gz` & `tmp/cohere-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.2.1.tar", max compression
+gzip compressed data, was "cohere-4.3.0.tar", max compression
```

## Comparing `cohere-4.2.1.tar` & `cohere-4.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-04-25 14:14:11.021253 cohere-4.2.1/LICENSE
--rw-r--r--   0        0        0     4480 2023-04-25 14:14:11.021253 cohere-4.2.1/README.md
--rw-r--r--   0        0        0      739 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/__init__.py
--rw-r--r--   0        0        0    34457 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/client.py
--rw-r--r--   0        0        0    25945 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/error.py
--rw-r--r--   0        0        0      529 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/logging.py
--rw-r--r--   0        0        0      792 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/base.py
--rw-r--r--   0        0        0     3438 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/bulk_embed.py
--rw-r--r--   0        0        0     3748 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/classify.py
--rw-r--r--   0        0        0     4826 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/cluster.py
--rw-r--r--   0        0        0      552 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      442 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      342 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     2614 2023-04-25 14:14:11.021253 cohere-4.2.1/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-04-25 14:14:11.025253 cohere-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.2.1/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-26 22:11:26.323550 cohere-4.3.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-04-26 22:11:26.323550 cohere-4.3.0/README.md
+-rw-r--r--   0        0        0      771 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/__init__.py
+-rw-r--r--   0        0        0    36120 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/client.py
+-rw-r--r--   0        0        0    27889 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/client_async.py
+-rw-r--r--   0        0        0     1187 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/logging.py
+-rw-r--r--   0        0        0      839 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     3748 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      436 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/codebook.py
+-rw-r--r--   0        0        0      552 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      587 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-04-26 22:11:26.323550 cohere-4.3.0/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-04-26 22:11:26.327550 cohere-4.3.0/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-04-26 22:11:26.327550 cohere-4.3.0/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     2614 2023-04-26 22:11:26.327550 cohere-4.3.0/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-04-26 22:11:26.327550 cohere-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.3.0/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.3.0/PKG-INFO
```

### Comparing `cohere-4.2.1/LICENSE` & `cohere-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/README.md` & `cohere-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/__init__.py` & `cohere-4.3.0/cohere/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 COHERE_API_URL = "https://api.cohere.ai"
 RETRY_STATUS_CODES = [429, 500, 502, 503, 504]
 
 API_VERSION = "1"
 COHERE_EMBED_BATCH_SIZE = 96
 CHAT_URL = "chat"
 CLASSIFY_URL = "classify"
+CODEBOOK_URL = "embed-codebook"
 DETECT_LANG_URL = "detect-language"
 EMBED_URL = "embed"
 GENERATE_FEEDBACK_URL = "feedback/generate"
 GENERATE_PREFERENCE_FEEDBACK_URL = "feedback/generate/preference"
 GENERATE_URL = "generate"
 SUMMARIZE_URL = "summarize"
 RERANK_URL = "rerank"
```

### Comparing `cohere-4.2.1/cohere/client.py` & `cohere-4.3.0/cohere/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import cohere
 from cohere.error import CohereAPIError, CohereConnectionError, CohereError
 from cohere.logging import logger
 from cohere.responses import (
     Classification,
     Classifications,
+    Codebook,
     Detokenization,
     Generations,
     StreamingGenerations,
     Tokens,
 )
 from cohere.responses.bulk_embed import BulkEmbedJob, CreateBulkEmbedJobResponse
 from cohere.responses.chat import Chat, StreamingChat
@@ -251,41 +252,78 @@
                     message="chatlog_override must be a list of dicts, but it contains a non-dict element"
                 )
             if len(entry) != 1:
                 raise CohereError(
                     message="chatlog_override must be a list of dicts, each mapping the agent to the message."
                 )
 
-    def embed(self, texts: List[str], model: Optional[str] = None, truncate: Optional[str] = None) -> Embeddings:
+    def embed(
+        self,
+        texts: List[str],
+        model: Optional[str] = None,
+        truncate: Optional[str] = None,
+        compress: Optional[bool] = False,
+        compression_codebook: Optional[str] = "default",
+    ) -> Embeddings:
         """Returns an Embeddings object for the provided texts. Visit https://cohere.ai/embed to learn about embeddings.
 
         Args:
             text (List[str]): A list of strings to embed.
             model (str): (Optional) The model ID to use for embedding the text.
             truncate (str): (Optional) One of NONE|START|END, defaults to END. How the API handles text longer than the maximum token length.
+            compress (bool): (Optional) Whether to compress the embeddings. When True, the compressed_embeddings will be returned as integers in the range [0, 255].
+            compression_codebook (str): (Optional) The compression codebook to use for compressed embeddings. Defaults to "default".
         """
-        responses = []
+        responses = {
+            "embeddings": [],
+            "compressed_embeddings": [],
+        }
         json_bodys = []
 
         for i in range(0, len(texts), self.batch_size):
             texts_batch = texts[i : i + self.batch_size]
             json_bodys.append(
                 {
                     "model": model,
                     "texts": texts_batch,
                     "truncate": truncate,
+                    "compress": compress,
+                    "compression_codebook": compression_codebook,
                 }
             )
 
         meta = None
         for result in self._executor.map(lambda json_body: self._request(cohere.EMBED_URL, json=json_body), json_bodys):
-            responses.extend(result["embeddings"])
+            responses["embeddings"].extend(result["embeddings"])
+            responses["compressed_embeddings"].extend(result.get("compressed_embeddings", []))
             meta = result["meta"] if not meta else meta
 
-        return Embeddings(responses, meta)
+        return Embeddings(
+            embeddings=responses["embeddings"],
+            compressed_embeddings=responses["compressed_embeddings"],
+            meta=meta,
+        )
+
+    def codebook(
+        self,
+        model: Optional[str] = None,
+        compression_codebook: Optional[str] = "default",
+    ) -> Codebook:
+        """Returns a codebook object for the provided model. Visit https://cohere.ai/embed to learn about compressed embeddings and codebooks.
+
+        Args:
+            model (str): (Optional) The model ID to use for embedding the text.
+            compression_codebook (str): (Optional) The compression codebook to use for compressed embeddings. Defaults to "default".
+        """
+        json_body = {
+            "model": model,
+            "compression_codebook": compression_codebook,
+        }
+        response = self._request(cohere.CODEBOOK_URL, json=json_body)
+        return Codebook(response["codebook"], response["meta"])
 
     def classify(
         self,
         inputs: List[str] = [],
         model: Optional[str] = None,
         preset: Optional[str] = None,
         examples: List[ClassifyExample] = [],
```

### Comparing `cohere-4.2.1/cohere/client_async.py` & `cohere-4.3.0/cohere/client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from cohere.error import CohereAPIError, CohereConnectionError, CohereError
 from cohere.logging import logger
 from cohere.responses import (
     AsyncCreateClusterJobResponse,
     Classification,
     Classifications,
     ClusterJobResult,
+    Codebook,
     DetectLanguageResponse,
     Detokenization,
     Embeddings,
     GenerateFeedbackResponse,
     GeneratePreferenceFeedbackResponse,
     Generations,
     LabelPrediction,
@@ -204,24 +205,67 @@
         response = await self._request(cohere.CHAT_URL, json=json_body, stream=stream)
 
         if stream:
             return StreamingChat(response)
         else:
             return AsyncChat.from_dict(response, query=query, client=self)
 
-    async def embed(self, texts: List[str], model: Optional[str] = None, truncate: Optional[str] = None) -> Embeddings:
+    async def embed(
+        self,
+        texts: List[str],
+        model: Optional[str] = None,
+        truncate: Optional[str] = None,
+        compress: Optional[bool] = False,
+        compression_codebook: Optional[str] = "default",
+    ) -> Embeddings:
+        """Returns an Embeddings object for the provided texts. Visit https://cohere.ai/embed to learn about embeddings.
+
+        Args:
+            text (List[str]): A list of strings to embed.
+            model (str): (Optional) The model ID to use for embedding the text.
+            truncate (str): (Optional) One of NONE|START|END, defaults to END. How the API handles text longer than the maximum token length.
+            compress (bool): (Optional) Whether to compress the embeddings. When True, the compressed_embeddings will be returned as integers in the range [0, 255].
+            compression_codebook (str): (Optional) The compression codebook to use for compressed embeddings. Defaults to "default".
+        """
         json_bodys = [
-            dict(texts=texts[i : i + cohere.COHERE_EMBED_BATCH_SIZE], model=model, truncate=truncate)
+            dict(
+                texts=texts[i : i + cohere.COHERE_EMBED_BATCH_SIZE],
+                model=model,
+                truncate=truncate,
+                compress=compress,
+                compression_codebook=compression_codebook,
+            )
             for i in range(0, len(texts), cohere.COHERE_EMBED_BATCH_SIZE)
         ]
         responses = await asyncio.gather(*[self._request(cohere.EMBED_URL, json) for json in json_bodys])
         meta = responses[0]["meta"] if responses else None
 
-        embeddings = Embeddings([e for res in responses for e in res["embeddings"]], meta)  # concatenate results
-        return embeddings
+        return Embeddings(
+            embeddings=[e for res in responses for e in res["embeddings"]],
+            compressed_embeddings=[e for res in responses for e in res["compressed_embeddings"]] if compress else None,
+            meta=meta,
+        )
+
+    async def codebook(
+        self,
+        model: Optional[str] = None,
+        compression_codebook: Optional[str] = "default",
+    ) -> Codebook:
+        """Returns a codebook object for the provided model. Visit https://cohere.ai/embed to learn about compressed embeddings and codebooks.
+
+        Args:
+            model (str): (Optional) The model ID to use for embedding the text.
+            compression_codebook (str): (Optional) The compression codebook to use for compressed embeddings. Defaults to "default".
+        """
+        json_body = {
+            "model": model,
+            "compression_codebook": compression_codebook,
+        }
+        response = await self._request(cohere.CODEBOOK_URL, json=json_body)
+        return Codebook(response["codebook"], response["meta"])
 
     async def classify(
         self,
         inputs: List[str] = [],
         model: Optional[str] = None,
         preset: Optional[str] = None,
         examples: List[ClassifyExample] = [],
```

### Comparing `cohere-4.2.1/cohere/error.py` & `cohere-4.3.0/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/logging.py` & `cohere-4.3.0/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/__init__.py` & `cohere-4.3.0/cohere/responses/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from cohere.responses.chat import Chat
 from cohere.responses.classify import Classification, Classifications, LabelPrediction
 from cohere.responses.cluster import (
     AsyncCreateClusterJobResponse,
     ClusterJobResult,
     CreateClusterJobResponse,
 )
+from cohere.responses.codebook import Codebook
 from cohere.responses.detectlang import DetectLanguageResponse, Language
 from cohere.responses.embeddings import Embeddings
 from cohere.responses.feedback import (
     GenerateFeedbackResponse,
     GeneratePreferenceFeedbackResponse,
     PreferenceRating,
 )
```

### Comparing `cohere-4.2.1/cohere/responses/base.py` & `cohere-4.3.0/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/bulk_embed.py` & `cohere-4.3.0/cohere/responses/bulk_embed.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/chat.py` & `cohere-4.3.0/cohere/responses/chat.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/classify.py` & `cohere-4.3.0/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/cluster.py` & `cohere-4.3.0/cohere/responses/cluster.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/detectlang.py` & `cohere-4.3.0/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/generation.py` & `cohere-4.3.0/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/rerank.py` & `cohere-4.3.0/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/summarize.py` & `cohere-4.3.0/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/responses/tokenize.py` & `cohere-4.3.0/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/cohere/utils.py` & `cohere-4.3.0/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-4.2.1/pyproject.toml` & `cohere-4.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.2.1"
+version = "4.3.0"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.2.1/setup.py` & `cohere-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.2.1',
+    'version': '4.3.0',
     'description': '',
     'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cohere-4.2.1/PKG-INFO` & `cohere-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.2.1
+Version: 4.3.0
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


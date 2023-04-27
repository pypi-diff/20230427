# Comparing `tmp/open_gpt_torch-0.0.1rc4.tar.gz` & `tmp/open_gpt_torch-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc4.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc5.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc4.tar` & `open_gpt_torch-0.0.1rc5.tar`

### file list

```diff
@@ -1,25 +1,41 @@
--rw-r--r--   0        0        0    10825 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/LICENSE
--rw-r--r--   0        0        0     7518 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/README.md
--rw-r--r--   0        0        0      453 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/__init__.py
--rw-r--r--   0        0        0      474 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/adapter.py
--rw-r--r--   0        0        0      503 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/executor.py
--rw-r--r--   0        0        0     2598 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/factory.py
--rw-r--r--   0        0        0     1767 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/hub.py
--rw-r--r--   0        0        0      349 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     5274 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     5658 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     8561 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0      863 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0      638 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/hf_model.py
--rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0      846 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0        0 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     1077 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0     2862 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/profile.py
--rw-r--r--   0        0        0      931 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/open_gpt/serve.py
--rw-r--r--   0        0        0     1887 2023-04-23 06:59:17.082478 open_gpt_torch-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0    19765 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/LICENSE
+-rw-r--r--   0        0        0     7518 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/README.md
+-rw-r--r--   0        0        0     1144 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/__main__.py
+-rw-r--r--   0        0        0      474 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/adapter.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0     1232 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     3088 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/factory.py
+-rw-r--r--   0        0        0     1767 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/hub.py
+-rw-r--r--   0        0        0      512 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     5274 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     5658 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     8561 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0     1074 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0      638 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/hf_model.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0      846 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      984 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     1860 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/loading.py
+-rw-r--r--   0        0        0     1422 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     1096 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0      790 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/stablelm/loading.py
+-rw-r--r--   0        0        0     2862 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0      437 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/flow.py
+-rw-r--r--   0        0        0      931 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0     2229 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/pyproject.toml
+-rw-r--r--   0        0        0    19858 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc5/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc4/LICENSE` & `open_gpt_torch-0.0.1rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/README.md` & `open_gpt_torch-0.0.1rc5/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc5/open_gpt/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,9 +74,21 @@
         )
     elif model_name.startswith('EleutherAI/pythia'):
         from .models.pythia.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config
         )
+    elif model_name.startswith('stabilityai/stablelm'):
+        from .models.stablelm.loading import load_model_and_tokenizer
+
+        return load_model_and_tokenizer(
+            model_name, device=device, dtype=dtype, **model_config
+        )
+    elif model_name.startswith('fnlp/moss-moon'):
+        from .models.moss.loading import load_model_and_tokenizer
+
+        return load_model_and_tokenizer(
+            model_name, device=device, dtype=dtype, **model_config, **kwargs
+        )
     else:
         raise ValueError(f'Unknown model name: {model_name}')
```

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/helper.py` & `open_gpt_torch-0.0.1rc5/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/flan/loading.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from accelerate import init_empty_weights, load_checkpoint_and_dispatch
 from transformers import AutoConfig, AutoTokenizer, T5ForConditionalGeneration
 
 if TYPE_CHECKING:
     import torch
 
 from loguru import logger
 
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
-    dtype: Union[str, 'torch.dtype'] = 'torch.float16',
+    tokenizer_name_or_path: Optional[str] = None,
+    device: Optional[torch.device] = None,
+    dtype: Optional[Union[str, torch.dtype]] = None,
     **kwargs
 ):
     """Load a model and tokenizer from HuggingFace."""
 
-    _ = kwargs.pop('device')
+    from ...helper import auto_dtype_and_device
+
+    dtype, device = auto_dtype_and_device(dtype, device)
 
     load_in_8bit = True if (str(dtype) == 'torch.int8') else False
 
     model = T5ForConditionalGeneration.from_pretrained(
         model_name_or_path,
         load_in_8bit=load_in_8bit,
-        torch_dtype=dtype if not load_in_8bit else None,
-        device_map="auto",
+        torch_dtype=dtype,
+        # device_map="auto",
         **kwargs
     )
-    tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
+    model.to(device)
+
+    tokenizer = AutoTokenizer.from_pretrained(
+        tokenizer_name_or_path or model_name_or_path
+    )
 
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/hf_model.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/hf_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.1rc5/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc5/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/open_gpt/serve.py` & `open_gpt_torch-0.0.1rc5/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc4/pyproject.toml` & `open_gpt_torch-0.0.1rc5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc4"
+version = "0.0.1rc5"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
@@ -17,52 +17,64 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 packages = [{ include = "open_gpt" }]
-exclude = ["tests/**/*", "docs/**/*", "examples/**/*"]
+exclude = ["**/*.pyc", "**/*.pyi", "tests/**/*", "docs/**/*", "examples/**/*"]
 
 # README file(s) are used as the package description
 readme = ["README.md", "LICENSE"]
 
 # Keywords (translated to tags on the package index)
 keywords = ["Pytorch", "LLM", "GPT"]
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
-python = ">=3.8"
-torch = "<2.0.0" # a meta device requires torch >= 1.9.0
+python = ">=3.8,<4.0"
+# torch = {version = "<2.0.0+cu116", source="torch_cuda"} # a meta device requires torch >= 1.9.0
+jina = "^3.15.0"
+docarray = "^0.21.0"
 loguru = "^0.5"
+cleo = "^2.0.0"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
-transformers = "^4.12.5"
+transformers = "^4.28.0"
 open_clip_torch = "~2.16.0"
 accelerate = "^0.18.0"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 open-flamingo = { version = "^0.0", optional = true }
 
 [tool.poetry.extras]
 flamingo = ["open-flamingo"]
 
 # Dependency groups are supported for organizing your dependencies
 [tool.poetry.group.dev.dependencies]
+pre-commit = ">=2.15.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0"
+pytest-mock = ">=3.5"
+
+[tool.pytest.ini_options]
+# Ignore deprecation warnings
+filterwarnings = [
+    "ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning"
+]
+
 
 # ...and can be installed only when explicitly requested
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.1.1"
 
-## Python-style entrypoints and scripts are easily expressed
-#[tool.poetry.scripts]
-#my-script = "my_package:main"
+# Python-style entrypoints and scripts are easily expressed
+[tool.poetry.scripts]
+opengpt = "open_gpt.cli.application:main"
```

### Comparing `open_gpt_torch-0.0.1rc4/PKG-INFO` & `open_gpt_torch-0.0.1rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: flamingo
 Requires-Dist: accelerate (>=0.18.0,<0.19.0)
+Requires-Dist: cleo (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
+Requires-Dist: jina (>=3.15.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo"
 Requires-Dist: open_clip_torch (>=2.16.0,<2.17.0)
-Requires-Dist: torch (<2.0.0)
-Requires-Dist: transformers (>=4.12.5,<5.0.0)
+Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/open_gpt
 Description-Content-Type: text/markdown
 
 # OpenGPT
 
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
```


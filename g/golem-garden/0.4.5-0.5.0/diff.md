# Comparing `tmp/golem_garden-0.4.5.tar.gz` & `tmp/golem_garden-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_garden-0.4.5.tar", last modified: Tue Apr 11 13:51:44 2023, max compression
+gzip compressed data, was "golem_garden-0.5.0.tar", last modified: Thu Apr 27 16:53:06 2023, max compression
```

## Comparing `golem_garden-0.4.5.tar` & `golem_garden-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,50 @@
--rw-r--r--   0        0        0      519 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.github/workflows/deploy_docs.yml
--rw-r--r--   0        0        0     1142 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1844 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.gitignore
--rw-r--r--   0        0        0    34523 2023-04-11 13:51:39.723108 golem_garden-0.4.5/LICENSE
--rw-r--r--   0        0        0      178 2023-04-11 13:51:39.723108 golem_garden-0.4.5/README.md
--rw-r--r--   0        0        0      114 2023-04-11 13:51:39.723108 golem_garden-0.4.5/RUN_ME.py
--rw-r--r--   0        0        0       14 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/contributing.md
--rw-r--r--   0        0        0     2359 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/style_guide.md
--rw-r--r--   0        0        0     2396 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/style_guide_for_gpt.md
--rw-r--r--   0        0        0     1306 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/index.md
--rw-r--r--   0        0        0    78233 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/Notebook_Companion_Embedding_as_a_Service.ipynb
--rw-r--r--   0        0        0     3739 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/knowledge_corpus_embeddings/string_chopper.py
--rw-r--r--   0        0        0     2341 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/pinecone_open_ai_ada_embedding.py
--rw-r--r--   0        0        0     1305 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/sentence_transformer.py
--rw-r--r--   0        0        0      313 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/__init__.py
--rw-r--r--   0        0        0      172 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/__main__.py
--rw-r--r--   0        0        0     2125 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/api/main.py
--rw-r--r--   0        0        0      712 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/command_line_interface.py
--rw-r--r--   0        0        0        0 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/__init__.py
--rw-r--r--   0        0        0      350 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/base_database.py
--rw-r--r--   0        0        0     3770 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/json_database.py
--rw-r--r--   0        0        0     3276 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/mongo_database.py
--rw-r--r--   0        0        0      502 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/database.json
--rw-r--r--   0        0        0     1293 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/database_factory.py
--rw-r--r--   0        0        0     3274 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem.py
--rw-r--r--   0        0        0     1993 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem_configs/_default_golem.toml
--rw-r--r--   0        0        0     1067 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem_configs/golem_config.py
--rw-r--r--   0        0        0     1603 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_api.py
--rw-r--r--   0        0        0      217 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_chat_configs/_default_openai_chat_config.toml
--rw-r--r--   0        0        0     1790 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_chat_configs/openai_chat_config.py
--rw-r--r--   0        0        0     1717 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/tests/test_string_chopper.py
--rw-r--r--   0        0        0      398 2023-04-11 13:51:39.723108 golem_garden-0.4.5/mkdocs.yml
--rw-r--r--   0        0        0     1152 2023-04-11 13:51:39.723108 golem_garden-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2988 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/directory_printer.py
--rw-r--r--   0        0        0     5029 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/grab_all_py_in_one_text_block.py
--rw-r--r--   0        0        0     2306 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/pinecone.py
--rw-r--r--   0        0        0      507 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/try_mongo_connection.py
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 golem_garden-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      834 2023-04-27 16:52:58.896213 golem_garden-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-04-27 16:52:58.896213 golem_garden-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-27 16:52:58.896213 golem_garden-0.5.0/.github/workflows/deploy_docs.yml
+-rw-r--r--   0        0        0     1142 2023-04-27 16:52:58.896213 golem_garden-0.5.0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1883 2023-04-27 16:52:58.896213 golem_garden-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3348 2023-04-27 16:52:58.896213 golem_garden-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-27 16:52:58.896213 golem_garden-0.5.0/LICENSE
+-rw-r--r--   0        0        0      178 2023-04-27 16:52:58.896213 golem_garden-0.5.0/README.md
+-rw-r--r--   0        0        0       79 2023-04-27 16:52:58.896213 golem_garden-0.5.0/RUN_ME.py
+-rw-r--r--   0        0        0       14 2023-04-27 16:52:58.896213 golem_garden-0.5.0/docs/development/contributing.md
+-rw-r--r--   0        0        0     2359 2023-04-27 16:52:58.896213 golem_garden-0.5.0/docs/development/style_guide.md
+-rw-r--r--   0        0        0     2396 2023-04-27 16:52:58.896213 golem_garden-0.5.0/docs/development/style_guide_for_gpt.md
+-rw-r--r--   0        0        0     1306 2023-04-27 16:52:58.896213 golem_garden-0.5.0/docs/index.md
+-rw-r--r--   0        0        0      251 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/data_loaders/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/data_loaders/async_load_url_with_playwright.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/golems/__init__.py
+-rw-r--r--   0        0        0     2124 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/golems/golem.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1186 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/output_parsers/output_parser.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/prompts/__init__.py
+-rw-r--r--   0        0        0     1777 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/prompts/prompts.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/tools/__init__.py
+-rw-r--r--   0        0        0     3378 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/tools/directory_printer.py
+-rw-r--r--   0        0        0     5029 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/tools/grab_all_py_in_one_text_block.py
+-rw-r--r--   0        0        0      484 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
+-rw-r--r--   0        0        0     3686 2023-04-27 16:52:58.896213 golem_garden-0.5.0/golem_garden/tools/tools.py
+-rw-r--r--   0        0        0    29940 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/ask_freemocap_docs.ipynb
+-rw-r--r--   0        0        0     8092 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/dog_mailer_auto_gpt.py
+-rw-r--r--   0        0        0    20524 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0     3912 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/langchain_agent_playground.py
+-rw-r--r--   0        0        0    26686 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/autogpt.ipynb
+-rw-r--r--   0        0        0    31113 2023-04-27 16:52:58.896213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
+-rw-r--r--   0        0        0    60363 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
+-rw-r--r--   0        0        0    44476 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
+-rw-r--r--   0        0        0    23377 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0      882 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
+-rw-r--r--   0        0        0    18760 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
+-rw-r--r--   0        0        0    60951 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/marathon_times.ipynb
+-rw-r--r--   0        0        0    23334 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
+-rw-r--r--   0        0        0    25052 2023-04-27 16:52:58.900213 golem_garden-0.5.0/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
+-rw-r--r--   0        0        0      398 2023-04-27 16:52:58.900213 golem_garden-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      356 2023-04-27 16:52:58.900213 golem_garden-0.5.0/notes/bluesky_todos.md
+-rw-r--r--   0        0        0     1214 2023-04-27 16:52:58.900213 golem_garden-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-04-27 16:52:58.900213 golem_garden-0.5.0/sample.env
+-rw-r--r--   0        0        0       99 2023-04-27 16:52:58.900213 golem_garden-0.5.0/utilities/env_setup.bat
+-rw-r--r--   0        0        0     2280 2023-04-27 16:52:58.900213 golem_garden-0.5.0/utilities/pinecone.py
+-rw-r--r--   0        0        0      507 2023-04-27 16:52:58.900213 golem_garden-0.5.0/utilities/try_mongo_connection.py
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 golem_garden-0.5.0/PKG-INFO
```

### Comparing `golem_garden-0.4.5/.github/workflows/deploy_docs.yml` & `golem_garden-0.5.0/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `golem_garden-0.5.0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/.gitignore` & `golem_garden-0.5.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -128,7 +128,10 @@
 # Pyre type checker
 .pyre/
 .idea
 .vscode
 utilities/output/*
 
 .DS_Store
+test_database.json
+
+utilities/output/*
```

### Comparing `golem_garden-0.4.5/LICENSE` & `golem_garden-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/docs/development/style_guide.md` & `golem_garden-0.5.0/docs/development/style_guide.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/docs/development/style_guide_for_gpt.md` & `golem_garden-0.5.0/docs/development/style_guide_for_gpt.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/docs/index.md` & `golem_garden-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/experimental/pinecone_open_ai_ada_embedding.py` & `golem_garden-0.5.0/utilities/pinecone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import openai
 from dotenv import load_dotenv
 import pinecone
 from pinecone import Index
-from datasets import load_dataset
-from tqdm.auto import tqdm
 
 # Load environment variables
 load_dotenv()
 openai.api_key = os.getenv("OPENAI_API_KEY")
 PINECONE_API_KEY = os.getenv("PINECONE_API_KEY")
 PINECONE_ENVIRONMENT = os.getenv("PINECONE_ENVIRONMENT")
```

### Comparing `golem_garden-0.4.5/pyproject.toml` & `golem_garden-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,36 +19,39 @@
     "chat"
 ]
 
 
 dependencies = [
     "python-dotenv",
     "openai",
-    "pymongo",
-    "motor",
     "toml",
     "openai",
     "fastapi",
     "uvicorn",
-    "torch",
-    "retry",
-    "sentence-transformers"
+    "google-search-results",
+    "langchain",
+    "rich",
+    "wikipedia",
+    "wolframalpha",
+    "chromadb",
+    "pydantic",
+    "faiss-cpu",
 ]
 requires-python = ">=3.8"
 
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/jonmatthis/golem_garden"
 
 [tool.bumpver]
-current_version = "v0.4.5"
+current_version = "v0.5.0"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
```

### Comparing `golem_garden-0.4.5/utilities/grab_all_py_in_one_text_block.py` & `golem_garden-0.5.0/golem_garden/tools/grab_all_py_in_one_text_block.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.5/PKG-INFO` & `golem_garden-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: golem_garden
-Version: 0.4.5
+Version: 0.5.0
 Summary: Welcome to the Garden - We're so glad you're here <3 
 Keywords: chat
 Author: Jonathan Samir Matthis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: python-dotenv
 Requires-Dist: openai
-Requires-Dist: pymongo
-Requires-Dist: motor
 Requires-Dist: toml
 Requires-Dist: openai
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
-Requires-Dist: torch
-Requires-Dist: retry
-Requires-Dist: sentence-transformers
+Requires-Dist: google-search-results
+Requires-Dist: langchain
+Requires-Dist: rich
+Requires-Dist: wikipedia
+Requires-Dist: wolframalpha
+Requires-Dist: chromadb
+Requires-Dist: pydantic
+Requires-Dist: faiss-cpu
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Project-URL: Homepage, https://github.com/jonmatthis/golem_garden
 Provides-Extra: dev
```


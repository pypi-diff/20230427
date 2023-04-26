# Comparing `tmp/owl-builder-0.2.0.tar.gz` & `tmp/owl-builder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl-builder-0.2.0.tar", max compression
+gzip compressed data, was "owl-builder-0.2.1.tar", max compression
```

## Comparing `owl-builder-0.2.0.tar` & `owl-builder-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     6140 2023-03-30 03:34:00.018797 owl-builder-0.2.0/owl_builder/__init__.py
--rw-r--r--   0        0        0     1333 2023-03-30 03:34:50.948193 owl-builder-0.2.0/owl_builder/builder/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 22:55:21.894266 owl-builder-0.2.0/owl_builder/builder/dmo/__init__.py
--rw-r--r--   0        0        0      150 2023-03-30 04:17:00.365348 owl-builder-0.2.0/owl_builder/builder/svc/__init__.py
--rw-r--r--   0        0        0     1986 2023-03-30 03:34:22.939820 owl-builder-0.2.0/owl_builder/builder/svc/generate_intent_name.py
--rw-r--r--   0        0        0     2205 2023-03-28 16:19:12.362926 owl-builder-0.2.0/owl_builder/builder/svc/generate_qa_pairs.py
--rw-r--r--   0        0        0     4547 2023-03-29 22:46:21.411316 owl-builder-0.2.0/owl_builder/builder/svc/generate_ttl_node.py
--rw-r--r--   0        0        0      110 2023-03-29 22:58:28.122824 owl-builder-0.2.0/owl_builder/keyterms/__init__.py
--rw-r--r--   0        0        0       57 2022-05-28 20:54:47.417119 owl-builder-0.2.0/owl_builder/keyterms/bp/__init__.py
--rw-r--r--   0        0        0    13425 2023-03-30 03:30:41.588577 owl-builder-0.2.0/owl_builder/keyterms/bp/autotaxo_orchestrator.py
--rw-r--r--   0        0        0      419 2023-03-29 22:58:22.459119 owl-builder-0.2.0/owl_builder/keyterms/dmo/__init__.py
--rw-r--r--   0        0        0     2031 2023-03-30 04:23:36.969193 owl-builder-0.2.0/owl_builder/keyterms/dmo/openai_keyterm_extractor.py
--rw-r--r--   0        0        0     1456 2023-03-29 19:58:21.080767 owl-builder-0.2.0/owl_builder/keyterms/dmo/stopword_filter.py
--rw-r--r--   0        0        0     5374 2023-01-10 20:59:12.243489 owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_keyterm_extractor.py
--rw-r--r--   0        0        0     4470 2023-03-29 19:58:21.082767 owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_ngram_extractor.py
--rw-r--r--   0        0        0     3980 2023-03-29 19:58:21.095266 owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_nounchunk_extractor.py
--rw-r--r--   0        0        0     3635 2023-03-29 19:58:21.097266 owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_term_extractor.py
--rw-r--r--   0        0        0     3745 2023-03-29 19:58:21.097266 owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_triple_extractor.py
--rw-r--r--   0        0        0       74 2022-10-26 22:08:53.161319 owl-builder-0.2.0/owl_builder/keyterms/dto/__init__.py
--rw-r--r--   0        0        0      309 2022-10-07 18:40:54.245465 owl-builder-0.2.0/owl_builder/keyterms/dto/spacy_model.py
--rw-r--r--   0        0        0     1397 2022-10-07 18:42:34.933475 owl-builder-0.2.0/owl_builder/keyterms/dto/stopwords_kb.py
--rw-r--r--   0        0        0     3442 2023-03-29 20:04:32.627932 owl-builder-0.2.0/owl_builder/keyterms/README.md
--rw-r--r--   0        0        0      216 2023-03-30 03:29:53.179271 owl-builder-0.2.0/owl_builder/keyterms/svc/__init__.py
--rw-r--r--   0        0        0     2908 2023-03-29 19:58:21.113766 owl-builder-0.2.0/owl_builder/keyterms/svc/extract_keyterms.py
--rw-r--r--   0        0        0     4671 2023-03-28 04:43:20.624262 owl-builder-0.2.0/owl_builder/keyterms/svc/filter_keyterms.py
--rw-r--r--   0        0        0     2731 2022-12-14 19:23:00.076688 owl-builder-0.2.0/owl_builder/keyterms/svc/generate_taxonomy_dataframe.py
--rw-r--r--   0        0        0     2939 2022-12-14 20:01:56.100993 owl-builder-0.2.0/owl_builder/keyterms/svc/generate_taxonomy_ttl.py
--rw-r--r--   0        0        0     2489 2023-03-30 04:18:29.866973 owl-builder-0.2.0/owl_builder/recipes/recipe_for_intent_mapping.py
--rw-r--r--   0        0        0       39 2022-07-20 15:44:37.044887 owl-builder-0.2.0/owl_builder/relationships/__init__.py
--rw-r--r--   0        0        0       57 2022-07-19 05:20:38.176469 owl-builder-0.2.0/owl_builder/relationships/bp/__init__.py
--rw-r--r--   0        0        0     1300 2023-03-29 20:06:16.207312 owl-builder-0.2.0/owl_builder/relationships/bp/autorels_orchestrator.py
--rw-r--r--   0        0        0      213 2022-10-26 22:08:52.070822 owl-builder-0.2.0/owl_builder/relationships/README.md
--rw-r--r--   0        0        0      200 2022-07-20 16:26:02.287403 owl-builder-0.2.0/owl_builder/relationships/svc/__init__.py
--rw-r--r--   0        0        0     2029 2023-03-28 04:43:20.645259 owl-builder-0.2.0/owl_builder/relationships/svc/find_implies_relationships.py
--rw-r--r--   0        0        0     2299 2023-03-28 04:43:20.645259 owl-builder-0.2.0/owl_builder/relationships/svc/find_requires_relationships.py
--rw-r--r--   0        0        0     2299 2023-03-28 04:43:20.645259 owl-builder-0.2.0/owl_builder/relationships/svc/generate_relationships_ttl.py
--rw-r--r--   0        0        0     1721 2023-03-29 21:27:50.868040 owl-builder-0.2.0/owl_builder/synonyms/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 21:14:41.081834 owl-builder-0.2.0/owl_builder/synonyms/bp/__init__.py
--rw-r--r--   0        0        0      178 2023-03-29 20:54:34.191355 owl-builder-0.2.0/owl_builder/synonyms/dmo/__init__.py
--rw-r--r--   0        0        0     1971 2023-03-28 04:43:20.645259 owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_cache_writer.py
--rw-r--r--   0        0        0     2277 2023-03-28 04:43:20.644258 owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_event_executor.py
--rw-r--r--   0        0        0     3905 2023-03-28 04:43:20.644258 owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_output_extractor.py
--rw-r--r--   0        0        0     1785 2023-03-29 21:00:57.838124 owl-builder-0.2.0/owl_builder/synonyms/dmo/synonym_prompt_generator.py
--rw-r--r--   0        0        0       39 2022-07-21 15:07:21.496228 owl-builder-0.2.0/owl_builder/synonyms/dto/__init__.py
--rw-r--r--   0        0        0     2891 2023-03-28 04:43:20.645259 owl-builder-0.2.0/owl_builder/synonyms/dto/openai_cache.py
--rw-r--r--   0        0        0      906 2023-03-29 22:58:28.112826 owl-builder-0.2.0/owl_builder/synonyms/README.md
--rw-r--r--   0        0        0      134 2023-03-29 20:12:08.390434 owl-builder-0.2.0/owl_builder/synonyms/svc/__init__.py
--rw-r--r--   0        0        0     2104 2023-03-29 20:05:04.373842 owl-builder-0.2.0/owl_builder/synonyms/svc/generate_english_inflections.py
--rw-r--r--   0        0        0     1935 2023-03-29 21:12:12.237207 owl-builder-0.2.0/owl_builder/synonyms/svc/generate_english_synonyms.py
--rw-r--r--   0        0        0     1847 2023-03-29 19:57:45.235399 owl-builder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3070 2023-03-28 16:25:03.911207 owl-builder-0.2.0/README.md
--rw-r--r--   0        0        0     4505 2023-03-30 04:24:42.992773 owl-builder-0.2.0/setup.py
--rw-r--r--   0        0        0     4267 2023-03-30 04:24:42.993275 owl-builder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6161 2023-03-31 17:50:22.658628 owl-builder-0.2.1/owl_builder/__init__.py
+-rw-r--r--   0        0        0     1333 2023-03-30 03:34:50.948193 owl-builder-0.2.1/owl_builder/builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 22:55:21.894266 owl-builder-0.2.1/owl_builder/builder/dmo/__init__.py
+-rw-r--r--   0        0        0      150 2023-03-30 04:17:00.365348 owl-builder-0.2.1/owl_builder/builder/svc/__init__.py
+-rw-r--r--   0        0        0     1986 2023-03-30 03:34:22.939820 owl-builder-0.2.1/owl_builder/builder/svc/generate_intent_name.py
+-rw-r--r--   0        0        0     2205 2023-03-28 16:19:12.362926 owl-builder-0.2.1/owl_builder/builder/svc/generate_qa_pairs.py
+-rw-r--r--   0        0        0     4547 2023-03-29 22:46:21.411316 owl-builder-0.2.1/owl_builder/builder/svc/generate_ttl_node.py
+-rw-r--r--   0        0        0       39 2023-03-31 17:49:44.882504 owl-builder-0.2.1/owl_builder/core/__init__.py
+-rw-r--r--   0        0        0     2917 2023-03-31 17:53:47.487273 owl-builder-0.2.1/owl_builder/core/openai_cache.py
+-rw-r--r--   0        0        0      110 2023-03-29 22:58:28.122824 owl-builder-0.2.1/owl_builder/keyterms/__init__.py
+-rw-r--r--   0        0        0       57 2022-05-28 20:54:47.417119 owl-builder-0.2.1/owl_builder/keyterms/bp/__init__.py
+-rw-r--r--   0        0        0    13425 2023-03-30 03:30:41.588577 owl-builder-0.2.1/owl_builder/keyterms/bp/autotaxo_orchestrator.py
+-rw-r--r--   0        0        0      419 2023-03-29 22:58:22.459119 owl-builder-0.2.1/owl_builder/keyterms/dmo/__init__.py
+-rw-r--r--   0        0        0     2424 2023-03-31 17:54:37.604769 owl-builder-0.2.1/owl_builder/keyterms/dmo/openai_keyterm_extractor.py
+-rw-r--r--   0        0        0     1456 2023-03-29 19:58:21.080767 owl-builder-0.2.1/owl_builder/keyterms/dmo/stopword_filter.py
+-rw-r--r--   0        0        0     5374 2023-01-10 20:59:12.243489 owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_keyterm_extractor.py
+-rw-r--r--   0        0        0     4470 2023-03-29 19:58:21.082767 owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_ngram_extractor.py
+-rw-r--r--   0        0        0     3980 2023-03-29 19:58:21.095266 owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_nounchunk_extractor.py
+-rw-r--r--   0        0        0     3635 2023-03-29 19:58:21.097266 owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_term_extractor.py
+-rw-r--r--   0        0        0     3745 2023-03-29 19:58:21.097266 owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_triple_extractor.py
+-rw-r--r--   0        0        0       74 2022-10-26 22:08:53.161319 owl-builder-0.2.1/owl_builder/keyterms/dto/__init__.py
+-rw-r--r--   0        0        0      309 2022-10-07 18:40:54.245465 owl-builder-0.2.1/owl_builder/keyterms/dto/spacy_model.py
+-rw-r--r--   0        0        0     1397 2022-10-07 18:42:34.933475 owl-builder-0.2.1/owl_builder/keyterms/dto/stopwords_kb.py
+-rw-r--r--   0        0        0     3442 2023-03-29 20:04:32.627932 owl-builder-0.2.1/owl_builder/keyterms/README.md
+-rw-r--r--   0        0        0      216 2023-03-30 03:29:53.179271 owl-builder-0.2.1/owl_builder/keyterms/svc/__init__.py
+-rw-r--r--   0        0        0     2908 2023-03-29 19:58:21.113766 owl-builder-0.2.1/owl_builder/keyterms/svc/extract_keyterms.py
+-rw-r--r--   0        0        0     4671 2023-03-28 04:43:20.624262 owl-builder-0.2.1/owl_builder/keyterms/svc/filter_keyterms.py
+-rw-r--r--   0        0        0     2731 2022-12-14 19:23:00.076688 owl-builder-0.2.1/owl_builder/keyterms/svc/generate_taxonomy_dataframe.py
+-rw-r--r--   0        0        0     2939 2022-12-14 20:01:56.100993 owl-builder-0.2.1/owl_builder/keyterms/svc/generate_taxonomy_ttl.py
+-rw-r--r--   0        0        0     7569 2023-03-31 17:46:29.342838 owl-builder-0.2.1/owl_builder/recipes/recipe_for_intent_mapping.py
+-rw-r--r--   0        0        0       39 2022-07-20 15:44:37.044887 owl-builder-0.2.1/owl_builder/relationships/__init__.py
+-rw-r--r--   0        0        0       57 2022-07-19 05:20:38.176469 owl-builder-0.2.1/owl_builder/relationships/bp/__init__.py
+-rw-r--r--   0        0        0     1300 2023-03-29 20:06:16.207312 owl-builder-0.2.1/owl_builder/relationships/bp/autorels_orchestrator.py
+-rw-r--r--   0        0        0      213 2022-10-26 22:08:52.070822 owl-builder-0.2.1/owl_builder/relationships/README.md
+-rw-r--r--   0        0        0      200 2022-07-20 16:26:02.287403 owl-builder-0.2.1/owl_builder/relationships/svc/__init__.py
+-rw-r--r--   0        0        0     2029 2023-03-28 04:43:20.645259 owl-builder-0.2.1/owl_builder/relationships/svc/find_implies_relationships.py
+-rw-r--r--   0        0        0     2299 2023-03-28 04:43:20.645259 owl-builder-0.2.1/owl_builder/relationships/svc/find_requires_relationships.py
+-rw-r--r--   0        0        0     2299 2023-03-28 04:43:20.645259 owl-builder-0.2.1/owl_builder/relationships/svc/generate_relationships_ttl.py
+-rw-r--r--   0        0        0     1721 2023-03-29 21:27:50.868040 owl-builder-0.2.1/owl_builder/synonyms/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 21:14:41.081834 owl-builder-0.2.1/owl_builder/synonyms/bp/__init__.py
+-rw-r--r--   0        0        0      178 2023-03-29 20:54:34.191355 owl-builder-0.2.1/owl_builder/synonyms/dmo/__init__.py
+-rw-r--r--   0        0        0     1971 2023-03-28 04:43:20.645259 owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_cache_writer.py
+-rw-r--r--   0        0        0     2277 2023-03-28 04:43:20.644258 owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_event_executor.py
+-rw-r--r--   0        0        0     3905 2023-03-28 04:43:20.644258 owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_output_extractor.py
+-rw-r--r--   0        0        0     1777 2023-03-31 17:49:55.100968 owl-builder-0.2.1/owl_builder/synonyms/dmo/synonym_prompt_generator.py
+-rw-r--r--   0        0        0      906 2023-03-29 22:58:28.112826 owl-builder-0.2.1/owl_builder/synonyms/README.md
+-rw-r--r--   0        0        0      134 2023-03-29 20:12:08.390434 owl-builder-0.2.1/owl_builder/synonyms/svc/__init__.py
+-rw-r--r--   0        0        0     2096 2023-03-31 17:50:35.593263 owl-builder-0.2.1/owl_builder/synonyms/svc/generate_english_inflections.py
+-rw-r--r--   0        0        0     1927 2023-03-31 17:50:04.877591 owl-builder-0.2.1/owl_builder/synonyms/svc/generate_english_synonyms.py
+-rw-r--r--   0        0        0     1847 2023-04-26 23:12:07.804200 owl-builder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3070 2023-03-28 16:25:03.911207 owl-builder-0.2.1/README.md
+-rw-r--r--   0        0        0     4497 2023-04-26 23:12:26.475200 owl-builder-0.2.1/setup.py
+-rw-r--r--   0        0        0     4267 2023-04-26 23:12:26.475700 owl-builder-0.2.1/PKG-INFO
```

### Comparing `owl-builder-0.2.0/owl_builder/__init__.py` & `owl-builder-0.2.1/owl_builder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import (
     List,
     Optional,
 )
 
 from pandas import DataFrame
 
+from .core import *
 from .builder import *
 from .synonyms import *
 from .relationships import *
 
 from .keyterms import *
 from .keyterms.bp import AutoTaxoOrchestrator
```

### Comparing `owl-builder-0.2.0/owl_builder/builder/__init__.py` & `owl-builder-0.2.1/owl_builder/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/builder/svc/generate_intent_name.py` & `owl-builder-0.2.1/owl_builder/builder/svc/generate_intent_name.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/builder/svc/generate_qa_pairs.py` & `owl-builder-0.2.1/owl_builder/builder/svc/generate_qa_pairs.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/builder/svc/generate_ttl_node.py` & `owl-builder-0.2.1/owl_builder/builder/svc/generate_ttl_node.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/bp/autotaxo_orchestrator.py` & `owl-builder-0.2.1/owl_builder/keyterms/bp/autotaxo_orchestrator.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/openai_keyterm_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/svc/extract_keyterms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,90 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-""" Extract Keyterms using an OpenAI Model """
+""" Extract Keyterms from Input Text using Textacy """
 
 
-from typing import List
+import pandas as pd
+from pandas import DataFrame
+
+from spacy.lang.en import English
 
 from baseblock import Enforcer
 from baseblock import Stopwatch
 from baseblock import BaseObject
 
-from openai_helper import chat
+from owl_builder.keyterms.dmo import TextacyKeytermExtractor
+from owl_builder.keyterms.dmo import TextacyNgramExtractor
+from owl_builder.keyterms.dmo import TextacyNounChunkExtractor
+from owl_builder.keyterms.dmo import TextacyTermExtractor
 
 
-class OpenAIKeytermExtractor(BaseObject):
-    """ Extract Keyterms using an OpenAI Model """
+class ExtractKeyterms(BaseObject):
+    """ Aggregation Service for Extracting Keyterms """
 
-    def __init__(self):
+    def __init__(self,
+                 model: English):
         """
         Created:
-            28-Mar-2023
+            18-Jul-2022
             craigtrim@gmail.com
-            *   https://github.com/craigtrim/owl-builder/issues/5
+            *   https://github.com/craigtrim/buildowl/issues/3
         """
         BaseObject.__init__(self, __name__)
+        self._extract_terms = TextacyTermExtractor(model).process
+        self._extract_ngrams = TextacyNgramExtractor(model).process
+        self._extract_keyterms = TextacyKeytermExtractor(model).process
+        self._extract_nounchunks = TextacyNounChunkExtractor(model).process
+
+    def _process(self,
+                 input_text: str,
+                 use_keyterms: bool,
+                 use_ngrams: bool,
+                 use_terms: bool,
+                 use_nounchunks: bool) -> DataFrame:
+
+        master = []
+
+        if self.isEnabledForDebug:
+            Enforcer.is_str(input_text)
+
+        input_text = input_text.replace('-', '')  # hyphens are problematic ...
+
+        if use_keyterms:
+            [master.append(x) for x in self._extract_keyterms(input_text)]
+
+        if use_ngrams:
+            [master.append(x) for x in self._extract_ngrams(input_text)]
+
+        if use_terms:
+            [master.append(x) for x in self._extract_terms(input_text)]
 
-    @staticmethod
-    def _prompt(input_text: str) -> str:
-        return f"Some text is provided below. Given the text, extract up to 10 keywords from the text. Avoid stopwords.---------------------\\n{input_text}\\n---------------------\\nProvide keywords in the following comma-separated format: \'KEYWORDS: <keywords>\'\\n"
-
-    @staticmethod
-    def _cleanse(input_text: str) -> str:
-        if input_text.endswith('.'):
-            input_text = input_text[:-1]
+        if use_nounchunks:
+            [master.append(x) for x in self._extract_nounchunks(input_text)]
 
-        return input_text
+        return pd.DataFrame(master)
 
     def process(self,
-                input_text: str) -> List[str]:
+                input_text: str,
+                use_terms: bool = True,
+                use_keyterms: bool = True,
+                use_ngrams: bool = False,
+                use_nounchunks: bool = False) -> DataFrame:
 
         sw = Stopwatch()
 
         if self.isEnabledForDebug:
             Enforcer.is_str(input_text)
 
-        keyterms = chat(
-            input_prompt=self._prompt(input_text),
-            messages=None,
-            remove_emojis=True)
-
-        if keyterms:
-
-            if keyterms.startswith('KEYWORDS:'):
-                keyterms = keyterms[9:].strip().split(',')
-
-            keyterms = [
-                x.strip() for x in keyterms
-            ]
-
-            keyterms = [
-                self._cleanse(x) for x in keyterms
-                if x and len(x)
-            ]
+        df = self._process(input_text,
+                           use_terms=use_terms,
+                           use_keyterms=use_keyterms,
+                           use_ngrams=use_ngrams,
+                           use_nounchunks=use_nounchunks)
 
         if self.isEnabledForInfo:
             self.logger.info('\n'.join([
                 "Keyword Extraction Complete",
                 f"\tTotal Time: {str(sw)}",
-                f"\tExtracted Terms: {keyterms}"]))
+                f"\tTotal Size: {len(df)}"]))
 
-        return keyterms
+        return df
```

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/stopword_filter.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/stopword_filter.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_keyterm_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_keyterm_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_ngram_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_ngram_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_nounchunk_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_nounchunk_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_term_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_term_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dmo/textacy_triple_extractor.py` & `owl-builder-0.2.1/owl_builder/keyterms/dmo/textacy_triple_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/dto/stopwords_kb.py` & `owl-builder-0.2.1/owl_builder/keyterms/dto/stopwords_kb.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/README.md` & `owl-builder-0.2.1/owl_builder/keyterms/README.md`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/svc/filter_keyterms.py` & `owl-builder-0.2.1/owl_builder/keyterms/svc/filter_keyterms.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/svc/generate_taxonomy_dataframe.py` & `owl-builder-0.2.1/owl_builder/keyterms/svc/generate_taxonomy_dataframe.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/keyterms/svc/generate_taxonomy_ttl.py` & `owl-builder-0.2.1/owl_builder/keyterms/svc/generate_taxonomy_ttl.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/relationships/bp/autorels_orchestrator.py` & `owl-builder-0.2.1/owl_builder/relationships/bp/autorels_orchestrator.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/relationships/svc/find_implies_relationships.py` & `owl-builder-0.2.1/owl_builder/relationships/svc/find_implies_relationships.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/relationships/svc/find_requires_relationships.py` & `owl-builder-0.2.1/owl_builder/relationships/svc/find_requires_relationships.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/relationships/svc/generate_relationships_ttl.py` & `owl-builder-0.2.1/owl_builder/relationships/svc/generate_relationships_ttl.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/__init__.py` & `owl-builder-0.2.1/owl_builder/synonyms/__init__.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_cache_writer.py` & `owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_cache_writer.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_event_executor.py` & `owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_event_executor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/dmo/openai_output_extractor.py` & `owl-builder-0.2.1/owl_builder/synonyms/dmo/openai_output_extractor.py`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/dmo/synonym_prompt_generator.py` & `owl-builder-0.2.1/owl_builder/synonyms/dmo/synonym_prompt_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Optional
 
 from baseblock import BaseObject
 
 from openai_helper import chat
 
-from owl_builder.synonyms.dto import OpenAICache
+from owl_builder.core import OpenAICache
 
 
 class SynonymPromptGenerator(BaseObject):
     """ Generate Synonym Prompts """
 
     def __init__(self):
         """
```

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/dto/openai_cache.py` & `owl-builder-0.2.1/owl_builder/core/openai_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,17 @@
             if len(file_name) >= 1:
                 return os.path.join(self._cache_path,
                                     file_name[0])
 
         base_dir = base()
 
         FileIO.exists_or_create(base_dir)
-        return os.path.join(base_dir, f"{file_name}.json")
+        file_path = FileIO.join_cwd(f"{file_name}.json")
+
+        return file_path
 
     def exists(self,
                file_name: str) -> bool:
         """ Check if File exists in Cache
 
         Args:
             file_name (str): the file name
```

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/README.md` & `owl-builder-0.2.1/owl_builder/synonyms/README.md`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/svc/generate_english_inflections.py` & `owl-builder-0.2.1/owl_builder/synonyms/svc/generate_english_inflections.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Optional
 
 from baseblock import BaseObject
 
 from openai_helper import chat
 
-from owl_builder.synonyms.dto import OpenAICache
+from owl_builder.core import OpenAICache
 
 
 class GenerateEnglishInflections(BaseObject):
     """ OpenAI: Generate Inflection Prompts """
 
     def __init__(self):
         """
```

### Comparing `owl-builder-0.2.0/owl_builder/synonyms/svc/generate_english_synonyms.py` & `owl-builder-0.2.1/owl_builder/synonyms/svc/generate_english_synonyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 from typing import Optional
 
 from baseblock import BaseObject
 
 from openai_helper import chat
 
-from owl_builder.synonyms.dto import OpenAICache
+from owl_builder.core import OpenAICache
 from owl_builder.synonyms.dmo import SynonymPromptGenerator
 
 
 class GenerateEnglishSynonyms(BaseObject):
     """ OpenAI: Generate Inflection Prompts """
 
     def __init__(self):
```

### Comparing `owl-builder-0.2.0/pyproject.toml` & `owl-builder-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Tools for Automating the Construction of an Ontology (OWL)"
 license = "None"
 name = "owl-builder"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 keywords = ["nlp", "nlu", "ai", "ontology", "automation"]
 repository = "https://github.com/craigtrim/owl-builder"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `owl-builder-0.2.0/README.md` & `owl-builder-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `owl-builder-0.2.0/setup.py` & `owl-builder-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from setuptools import setup
 
 packages = \
 ['owl_builder',
  'owl_builder.builder',
  'owl_builder.builder.dmo',
  'owl_builder.builder.svc',
+ 'owl_builder.core',
  'owl_builder.keyterms',
  'owl_builder.keyterms.bp',
  'owl_builder.keyterms.dmo',
  'owl_builder.keyterms.dto',
  'owl_builder.keyterms.svc',
  'owl_builder.recipes',
  'owl_builder.relationships',
  'owl_builder.relationships.bp',
  'owl_builder.relationships.svc',
  'owl_builder.synonyms',
  'owl_builder.synonyms.bp',
  'owl_builder.synonyms.dmo',
- 'owl_builder.synonyms.dto',
  'owl_builder.synonyms.svc']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['baseblock',
@@ -37,15 +37,15 @@
  'spacy==3.5.0',
  'tabulate',
  'textacy==0.12.0',
  'textblob>=0.17.1,<0.18.0']
 
 setup_kwargs = {
     'name': 'owl-builder',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Tools for Automating the Construction of an Ontology (OWL)',
     'long_description': '# Ontology Builder (owl-builder)\n\n##\n\n## Key Term Extraction\n```python\nfrom owl_builder import keyterms\n\ninput_text = """\nA local area network (LAN) is a computer network that interconnects computers within a limited area such as a residence, school, laboratory, university campus or office building.\n\nBy contrast, a wide area network (WAN) not only covers a larger geographic distance, but also generally involves leased telecommunication circuits.\n\nEthernet and Wi-Fi are the two most common technologies in use for local area networks.\n\nHistorical network technologies include ARCNET, Token Ring, and AppleTalk.\n"""\n\nresults = keyterms(\n    input_text=input_text,\n    use_openai=False,\n    use_terms=True,\n    use_keyterms=True,\n    use_ngrams=False,\n    use_nounchunks=False)\n```\n\nThe results are\n```json\n[\n   "leased telecommunication circuit",\n   "historical network technology",\n   "large geographic distance",\n   "interconnects computer",\n   "local area network",\n   "university campus",\n   "common technology",\n   "wide area network",\n   "computer network",\n   "office building",\n   "include arcnet",\n   "limited area",\n   "token ring"\n]\n```\n\nIf `use_openai` is set to `True`, then the following environment variables must be set:\n```python\nos.environ[\'USE_OPENAI\'] = "True"\nos.environ[\'OPENAI_KEY\'] = "<openai-key>"\nos.environ[\'OPENAI_ORG\'] = "<openai-org>"\n```\n\n## TTL Generation\n```python\nfrom owl_builder import build_ttl\n\nresults = build_ttl("He has aims to make Detroit a leader in green energy.")\n```\n\nThe result is\n```ttl\n###  http://graffl.ai/pathology#green_energy\n        :green_energy rdf:type owl:Class ;\n        rdfs:label "Green Energy" ;\n        rdfs:subClassOf :energy .\n###  http://graffl.ai/pathology#energy\n        :energy rdf:type owl:Class ;\n        rdfs:label "Energy" .\n```\n\nYou can also supply your own taxonomy like this:\n```python\nimport pandas as pd\n\nresults = build_ttl(pd.DataFrame([\n    {"Parent": "Alpha", "Child": "Alpha Beta"},\n    {"Parent": "Alpha Beta", "Child": "Alpha Beta Gamma"},\n    {"Parent": "Gamma", "Child": "Gamma Delta"},\n]))\n```\n\nThe result is\n```ttl\n###  http://graffl.ai/pathology#alpha_beta\n        :alpha_beta rdf:type owl:Class ;\n        rdfs:label "Alpha Beta" ;\n        rdfs:subClassOf :alpha .\n###  http://graffl.ai/pathology#alpha\n            :alpha rdf:type owl:Class ;\n            rdfs:label "Alpha" .\n###  http://graffl.ai/pathology#alpha_beta_gamma\n            :alpha_beta_gamma rdf:type owl:Class ;\n            rdfs:label "Alpha Beta Gamma" ;\n            rdfs:subClassOf :alpha_beta .\n###  http://graffl.ai/pathology#alpha_beta\n            :alpha_beta rdf:type owl:Class ;\n            rdfs:label "Alpha Beta" .\n###  http://graffl.ai/pathology#gamma_delta\n            :gamma_delta rdf:type owl:Class ;\n            rdfs:label "Gamma Delta" ;\n            rdfs:subClassOf :gamma .\n###  http://graffl.ai/pathology#gamma\n            :gamma rdf:type owl:Class ;\n            rdfs:label "Gamma" .\n```\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/owl-builder',
```

### Comparing `owl-builder-0.2.0/PKG-INFO` & `owl-builder-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for Automating the Construction of an Ontology (OWL)
 Home-page: https://github.com/craigtrim/owl-builder
 License: None
 Keywords: nlp,nlu,ai,ontology,automation
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```


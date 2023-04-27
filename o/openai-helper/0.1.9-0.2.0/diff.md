# Comparing `tmp/openai-helper-0.1.9.tar.gz` & `tmp/openai-helper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-helper-0.1.9.tar", max compression
+gzip compressed data, was "openai-helper-0.2.0.tar", max compression
```

## Comparing `openai-helper-0.1.9.tar` & `openai-helper-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,29 @@
--rw-r--r--   0        0        0       59 2022-08-04 23:49:16.132316 openai-helper-0.1.9/openai_helper/__init__.py
--rw-r--r--   0        0        0      144 2022-08-04 23:38:32.599317 openai-helper-0.1.9/openai_helper/bp/__init__.py
--rw-r--r--   0        0        0     3460 2022-08-18 22:30:50.835880 openai-helper-0.1.9/openai_helper/bp/extract_output.py
--rw-r--r--   0        0        0     3633 2022-08-18 21:51:35.642347 openai-helper-0.1.9/openai_helper/bp/openai_completion.py
--rw-r--r--   0        0        0     4121 2022-08-16 22:22:50.983812 openai-helper-0.1.9/openai_helper/bp/openai_custom_model.py
--rw-r--r--   0        0        0      355 2022-08-04 23:46:29.755316 openai-helper-0.1.9/openai_helper/dmo/__init__.py
--rw-r--r--   0        0        0     7294 2022-08-19 01:01:45.414112 openai-helper-0.1.9/openai_helper/dmo/completion_event_extractor.py
--rw-r--r--   0        0        0     2119 2022-08-16 17:56:12.406812 openai-helper-0.1.9/openai_helper/dmo/etl_handle_textcompletions.py
--rw-r--r--   0        0        0     2192 2022-09-14 05:06:41.421430 openai-helper-0.1.9/openai_helper/dmo/etl_remove_indicators.py
--rw-r--r--   0        0        0     1665 2022-08-16 17:56:12.406812 openai-helper-0.1.9/openai_helper/dmo/etl_replace_cliches.py
--rw-r--r--   0        0        0     1499 2022-08-16 17:56:12.406812 openai-helper-0.1.9/openai_helper/dmo/etl_replace_duplicatedinput.py
--rw-r--r--   0        0        0     1658 2022-07-28 22:33:11.197779 openai-helper-0.1.9/openai_helper/dmo/openai_connector.py
--rw-r--r--   0        0        0      164 2022-08-16 22:19:47.557312 openai-helper-0.1.9/openai_helper/svc/__init__.py
--rw-r--r--   0        0        0     2959 2022-08-16 22:23:18.065312 openai-helper-0.1.9/openai_helper/svc/create_openai_answer.py
--rw-r--r--   0        0        0     2554 2022-08-16 22:19:04.637312 openai-helper-0.1.9/openai_helper/svc/extract_top_response.py
--rw-r--r--   0        0        0     4889 2022-08-04 23:41:00.837316 openai-helper-0.1.9/openai_helper/svc/run_openai_completion.py
--rw-r--r--   0        0        0      395 2022-09-14 05:07:10.345639 openai-helper-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      693 2022-09-14 05:07:30.885387 openai-helper-0.1.9/setup.py
--rw-r--r--   0        0        0      285 2022-09-14 05:07:30.885387 openai-helper-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     7099 2023-03-28 19:57:26.769170 openai-helper-0.2.0/openai_helper/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-01 23:24:35.426289 openai-helper-0.2.0/openai_helper/bp/__init__.py
+-rw-r--r--   0        0        0     3145 2023-03-28 16:40:16.611674 openai-helper-0.2.0/openai_helper/bp/openai_chat_completion.py
+-rw-r--r--   0        0        0     3664 2023-03-01 22:37:49.356289 openai-helper-0.2.0/openai_helper/bp/openai_custom_model.py
+-rw-r--r--   0        0        0     4752 2023-03-01 22:13:34.947789 openai-helper-0.2.0/openai_helper/bp/openai_text_completion.py
+-rw-r--r--   0        0        0      745 2023-03-27 18:22:15.869933 openai-helper-0.2.0/openai_helper/dmo/__init__.py
+-rw-r--r--   0        0        0     1542 2023-03-01 23:24:44.090788 openai-helper-0.2.0/openai_helper/dmo/chat_message_formatter.py
+-rw-r--r--   0        0        0     7698 2022-12-08 01:40:33.067448 openai-helper-0.2.0/openai_helper/dmo/completion_event_extractor.py
+-rw-r--r--   0        0        0     2566 2023-02-13 05:49:27.009400 openai-helper-0.2.0/openai_helper/dmo/etl_handle_textcompletions.py
+-rw-r--r--   0        0        0     1351 2023-02-25 18:10:04.895458 openai-helper-0.2.0/openai_helper/dmo/etl_remove_emojis.py
+-rw-r--r--   0        0        0     3095 2023-03-11 18:30:15.174565 openai-helper-0.2.0/openai_helper/dmo/etl_remove_listindicators.py
+-rw-r--r--   0        0        0     2871 2023-03-14 16:16:21.916983 openai-helper-0.2.0/openai_helper/dmo/etl_remove_promptindicators.py
+-rw-r--r--   0        0        0     1665 2022-11-16 18:34:53.819884 openai-helper-0.2.0/openai_helper/dmo/etl_replace_cliches.py
+-rw-r--r--   0        0        0     1496 2022-09-29 21:43:12.370296 openai-helper-0.2.0/openai_helper/dmo/etl_replace_duplicatedinput.py
+-rw-r--r--   0        0        0     4123 2023-04-27 00:12:55.039700 openai-helper-0.2.0/openai_helper/dmo/input_token_counter.py
+-rw-r--r--   0        0        0     1172 2022-11-16 18:34:53.819381 openai-helper-0.2.0/openai_helper/dmo/no_openai_event.py
+-rw-r--r--   0        0        0     1719 2022-11-16 18:14:14.917879 openai-helper-0.2.0/openai_helper/dmo/openai_connector.py
+-rw-r--r--   0        0        0     6943 2023-03-01 23:21:18.381290 openai-helper-0.2.0/openai_helper/dmo/output_extractor_chat.py
+-rw-r--r--   0        0        0     8110 2023-03-01 23:21:47.463789 openai-helper-0.2.0/openai_helper/dmo/output_extractor_text.py
+-rw-r--r--   0        0        0      268 2023-03-16 18:41:15.424607 openai-helper-0.2.0/openai_helper/svc/__init__.py
+-rw-r--r--   0        0        0     2985 2022-11-19 06:19:01.788211 openai-helper-0.2.0/openai_helper/svc/create_openai_answer.py
+-rw-r--r--   0        0        0     2390 2023-03-25 05:55:44.937494 openai-helper-0.2.0/openai_helper/svc/extract_primary_topic.py
+-rw-r--r--   0        0        0     2554 2022-11-16 18:34:53.819884 openai-helper-0.2.0/openai_helper/svc/extract_top_response.py
+-rw-r--r--   0        0        0     5301 2023-03-28 16:40:16.616677 openai-helper-0.2.0/openai_helper/svc/run_chat_completion.py
+-rw-r--r--   0        0        0     8919 2023-04-27 00:03:17.192201 openai-helper-0.2.0/openai_helper/svc/run_text_completion.py
+-rw-r--r--   0        0        0     2191 2023-04-27 00:13:12.938200 openai-helper-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4102 2023-03-27 18:14:05.658957 openai-helper-0.2.0/README.md
+-rw-r--r--   0        0        0     4903 2023-04-27 00:13:31.677200 openai-helper-0.2.0/setup.py
+-rw-r--r--   0        0        0     4983 2023-04-27 00:13:31.677701 openai-helper-0.2.0/PKG-INFO
```

### Comparing `openai-helper-0.1.9/openai_helper/bp/openai_completion.py` & `openai-helper-0.2.0/openai_helper/bp/openai_text_completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,122 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ Run a Completion against openAI """
 
 
+from typing import Optional
+from typing import Callable
+
+from baseblock import EnvIO
 from baseblock import Enforcer
 from baseblock import BaseObject
 
 from openai_helper.dmo import OpenAIConnector
-from openai_helper.svc import RunOpenAICompletion
+from openai_helper.svc import RunTextCompletion
+from openai_helper.dmo import NoOpenAIEvent
+
 
+class OpenAITextCompletion(BaseObject):
+    """ Run a Text Completion against openAI """
 
-class OpenAICompletion(BaseObject):
-    """ Run a Completion against openAI """
+    __run = None
+    __conn = None
 
     def __init__(self,
                  conn: object = None):
         """ Change Log
 
         Created:
             28-Jul-2022
             craigtrim@gmail.com
         Updated:
             18-Aug-2022
             craigtrim@gmail.com
             *   allow optional conn as parameter
+        Updated:
+            29-Sept-2022
+            craigtrim@gmail.com
+            *   integrate 'no-openai-event'
+        Updated:
+            1-Mar-2023
+            craigtrim@gmail.com
+            *   renamed from 'openai-completion' in pursuit of
+                https://github.com/craigtrim/openai-helper/issues/9
+
+        Args:
+            conn (object): a connection to openAI
         """
         BaseObject.__init__(self, __name__)
-        if not conn:
-            conn = OpenAIConnector().process()
-        self._run = RunOpenAICompletion(conn).process
+        if conn:
+            self.__conn = conn
+
+    def _conn(self) -> object:
+        if not self.__conn:
+            self.__conn = OpenAIConnector().process()
+        return self.__conn
+
+    def _run(self) -> Callable:
+        if not self.__run:
+            self.__run = RunTextCompletion(self._conn()).process
+        return self.__run
 
     def run(self,
             input_prompt: str,
-            engine: str = None,
-            best_of: int = None,
-            temperature: float = None,
-            max_tokens: int = None,
-            top_p: float = None,
-            frequency_penalty: int = None,
-            presence_penalty: int = None) -> dict:
+            engine: Optional[str] = None,
+            best_of: Optional[int] = None,
+            temperature: Optional[float] = None,
+            max_tokens: Optional[int] = None,
+            top_p: Optional[float] = None,
+            frequency_penalty: Optional[int] = None,
+            presence_penalty: Optional[int] = None) -> dict:
         """ Run an OpenAI event
 
         Args:
             input_prompt (str): The Input Prompt to execute against OpenAI
             engine (str, optional): The OpenAI model (engine) to run against. Defaults to None.
-                Options as of July, 2022 are:
+                Options as of December, 2022 are:
+                    'text-davinci-003'
                     'text-davinci-002'
                     'text-curie-001',
                     'text-babbage-001'
                     'text-ada-001'
             best_of (int, optional): Generates Multiple Server-Side Combinations and only selects the best. Defaults to None.
                 This can really eat up OpenAI tokens so use with caution!
             temperature (float, optional): Control Randomness; Scale is 0.0 - 1.0. Defaults to None.
                 Scale is 0.0 - 1.0
                 Lower values approach predictable outputs and determinate behavior
                 Higher values are more engaging but also less predictable
                 Use High Values cautiously
             max_tokens (int, optional): The Maximum Number of tokens to generate. Defaults to None.
                 Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)
-                The higher this value, the more each request will cost.            
+                The higher this value, the more each request will cost.
             top_p (float, optional): Controls Diversity via Nucleus Sampling. Defaults to None.
                 no idea what this means
             frequency_penalty (int, optional): How much to penalize new tokens based on their frequency in the text so far. Defaults to None.
                 Scale: 0.0 - 2.0.
             presence_penalty (int, optional): Seems similar to frequency penalty. Defaults to None.
 
         Returns:
             dict: an output dictionary with two keys:
                 input: the input dictionary with validated parameters and default values where appropriate
                 output: the output event from OpenAI
         """
-        d_result = self._run(input_prompt=input_prompt,
-                             engine=engine,
-                             best_of=best_of,
-                             temperature=temperature,
-                             max_tokens=max_tokens,
-                             top_p=top_p,
-                             frequency_penalty=frequency_penalty,
-                             presence_penalty=presence_penalty)
+
+        if not EnvIO.is_true('USE_OPENAI'):
+            return NoOpenAIEvent().process(input_prompt, engine)
+
+        if self.isEnabledForDebug:
+            Enforcer.is_str(input_prompt)
+
+        d_result = self._run()(input_prompt=input_prompt,
+                               engine=engine,
+                               best_of=best_of,
+                               temperature=temperature,
+                               max_tokens=max_tokens,
+                               top_p=top_p,
+                               frequency_penalty=frequency_penalty,
+                               presence_penalty=presence_penalty)
 
         if self.isEnabledForDebug:
             Enforcer.keys(d_result, 'input', 'output')
 
         return d_result
```

### Comparing `openai-helper-0.1.9/openai_helper/bp/openai_custom_model.py` & `openai-helper-0.2.0/openai_helper/bp/openai_custom_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ Query a Custom Model in OpenAI """
 
 
-from random import sample
+from typing import Optional
+
 from functools import lru_cache
-from re import search
-from openai.error import InvalidRequestError
 
 from baseblock import EnvIO
 from baseblock import Stopwatch
 from baseblock import BaseObject
 from baseblock import Enforcer
 from baseblock import ServiceEventGenerator
 
 from openai_helper.svc import ExtractTopResponse
 from openai_helper.svc import CreateOpenAIAnswer
-from openai_helper.dmo import OpenAIConnector
+from openai_helper.dmo import NoOpenAIEvent
 
 
 class OpenAICustomModel(BaseObject):
     """ Query a Custom Model in OpenAI """
 
     def __init__(self,
                  model_name: str):
@@ -46,86 +45,68 @@
                 https://bast-ai.atlassian.net/browse/COR-94
 
         Args:
             openai (object): an instantiation of openAI
             model_name (str): the name of the custom model to query
         """
         BaseObject.__init__(self, __name__)
-        self._generate_event = ServiceEventGenerator().process
-        self._query = CreateOpenAIAnswer(model_name).process
-        self._extract_top_response = ExtractTopResponse().process
-
-    def _no_openai(self,
-                   input_text: str,
-                   search_model: str) -> dict:
-
-        sw = Stopwatch()
-        output_events = []
-
-        output_events.append(self._generate_event(
-            service_name=self.component_name(),
-            event_name="openai",
-            stopwatch=sw,
-            data={
-                'input_text': input_text,
-                'search_model': search_model,
-                'output_text': "*** OPENAI DISABLED ***"}))
-
-        return {
-            'text': None,
-            'events': output_events
-        }
+        # self._generate_event = ServiceEventGenerator().process
+        # self._query = CreateOpenAIAnswer(model_name).process
+        # self._extract_top_response = ExtractTopResponse().process
 
-    @lru_cache
     def process(self,
                 input_text: str,
-                search_model: str = 'text-davinci-002',
-                threshold: float = 25.0) -> tuple or None:
-        """ Call the OpenAI Text Summarizer
+                search_model: str = 'text-davinci-003',
+                threshold: float = 25.0) -> Optional[tuple]:
+        """ Call a custom OpenAI Model
 
         Args:
             input_text (str): the input text to send to OpenAI
             search_model (str): the model used to interpret the query and search
             threshold (float): the accuracy threshold for filtering results
 
         Returns:
             dict: the complete openAI event
         """
 
-        if not EnvIO.is_true("USE_OPENAI"):
-            return self._no_openai(input_text, search_model)
-
-        if self.isEnabledForDebug:
-            Enforcer.is_str(input_text)
-
-        sw = Stopwatch()
-        output_events = []
-
-        d_query = self._query(
-            input_text=input_text,
-            search_model=search_model)
-
-        [output_events.append(x) for x in d_query['events']]
-
-        if not d_query['results']:
-            return {
-                'text': None,
-                'events': output_events
-            }
-
-        d_top_response = self._extract_top_response(
-            d_query['results']['selected_documents'],
-            threshold=threshold)
-
-        [output_events.append(x) for x in d_top_response['events']]
-
-        if self.isEnabledForInfo:
-            self.logger.info('\n'.join([
-                f"OpenAI Service Completed",
-                f"\tTotal Time: {str(sw)}",
-                f"\tInput Text: {input_text.strip()}",
-                f"\tOutput Text: {d_top_response['text']}"]))
-
-        return {
-            'text': d_top_response['text'],
-            'events': output_events
-        }
+        # TODO: this API has changed in 0.27.0
+        #       will need to update the next time I use a custom model
+        raise NotImplementedError
+
+        # if not EnvIO.is_true('USE_OPENAI'):
+        #     return NoOpenAIEvent().process(input_text, search_model)
+
+        # if self.isEnabledForDebug:
+        #     Enforcer.is_str(input_text)
+
+        # sw = Stopwatch()
+        # output_events = []
+
+        # d_query = self._query(
+        #     input_text=input_text,
+        #     search_model=search_model)
+
+        # [output_events.append(x) for x in d_query['events']]
+
+        # if not d_query['results']:
+        #     return {
+        #         'text': None,
+        #         'events': output_events
+        #     }
+
+        # d_top_response = self._extract_top_response(
+        #     d_query['results']['selected_documents'],
+        #     threshold=threshold)
+
+        # [output_events.append(x) for x in d_top_response['events']]
+
+        # if self.isEnabledForInfo:
+        #     self.logger.info('\n'.join([
+        #         'OpenAI Service Completed',
+        #         f'\tTotal Time: {str(sw)}',
+        #         f'\tInput Text: {input_text.strip()}',
+        #         f"\tOutput Text: {d_top_response['text']}"]))
+
+        # return {
+        #     'text': d_top_response['text'],
+        #     'events': output_events
+        # }
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/completion_event_extractor.py` & `openai-helper-0.2.0/openai_helper/dmo/completion_event_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     def __init__(self,
                  timeout: int = 5):
         """ Change Log
 
         Created:
             28-Jul-2022
             craigtrim@gmail.com
+        Updated:
+            18-Nov-2022
+            craigtrim@gmail.com
+            *   add '_get*' top all methods to disambiguation from parameter list
+        Updated:
+            7-Dec-2022
+            craigtrim@gmail.com
+            *   default engine to 'text-davinci-003'
 
         Args:
             timeout (int, optional): the timeout for the API call. Defaults to 15.
         """
         BaseObject.__init__(self, __name__)
         self._timeout = EnvIO.int_or_default(
             'OPENAI_CREATE_TIMEOUT', timeout)  # GRAFFL-380
@@ -36,40 +44,41 @@
                 frequency_penalty: int = None,
                 presence_penalty: int = None) -> dict:
         """ Extract and Validate the Inputs into a single dictionary
 
         Args:
             input_prompt (str): The Input Prompt to execute against OpenAI
             engine (str, optional): The OpenAI model (engine) to run against. Defaults to None.
-                Options as of July, 2022 are:
+                Options as of December, 2022 are:
+                    'text-davinci-003'
                     'text-davinci-002'
                     'text-curie-001',
                     'text-babbage-001'
                     'text-ada-001'
             best_of (int, optional): Generates Multiple Server-Side Combinations and only selects the best. Defaults to None.
                 This can really eat up OpenAI tokens so use with caution!
             temperature (float, optional): Control Randomness; Scale is 0.0 - 1.0. Defaults to None.
                 Scale is 0.0 - 1.0
                 Lower values approach predictable outputs and determinate behavior
                 Higher values are more engaging but also less predictable
                 Use High Values cautiously
             max_tokens (int, optional): The Maximum Number of tokens to generate. Defaults to None.
                 Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)
-                The higher this value, the more each request will cost.            
+                The higher this value, the more each request will cost.
             top_p (float, optional): Controls Diversity via Nucleus Sampling. Defaults to None.
                 no idea what this means
             frequency_penalty (int, optional): How much to penalize new tokens based on their frequency in the text so far. Defaults to None.
                 Scale: 0.0 - 2.0.
             presence_penalty (int, optional): Seems similar to frequency penalty. Defaults to None.
 
         Returns:
             dict: a dictinoary of validated inputs with default values (where appropriate)
         """
 
-        def _input_prompt() -> str:
+        def _get_input_prompt() -> str:
             """ The Input Prompt to execute against OpenAI
 
             Raises:
                 ValueError: input prompt not given
 
             Returns:
                 str: the input prompt to execute
@@ -81,31 +90,31 @@
                 Enforcer.is_str(input_prompt)
 
             return input_prompt
 
         def _engine() -> str:
             """ The OpenAI model (engine) to run against
 
-            Options as of July, 2022 are:
-                'text-davinci-002'
+            Options as of December, 2022 are:
+                'text-davinci-003',
+                'text-davinci-002',
                 'text-curie-001',
                 'text-babbage-001'
                 'text-ada-001'
 
             Returns:
                 str: the openAI engine
             """
             if engine and len(engine):
                 if self.isEnabledForDebug:
                     Enforcer.is_str(engine)
                 return engine
 
-            # the best all-around engine as of July, 2022
-            # but also the most expensive
-            return 'text-davinci-002'
+            return EnvIO.str_or_default(env_var='OPENAI_ENGINE',
+                                        default='text-davinci-003')
 
         def _best_of() -> int:
             """ Generates Multiple Server-Side Combinations and only selects the best
             This can really eat up OpenAI tokens so use with caution!
 
             Returns:
                 int: the number of server-side combinations to generate
@@ -113,15 +122,15 @@
             if best_of:
                 if self.isEnabledForDebug:
                     Enforcer.is_int(best_of)
                 return int(best_of)
 
             return 1
 
-        def _temperature() -> float:
+        def _get_temperature() -> float:
             """ Control Randomness; Scale is 0.0 - 1.0
 
             Lower values approach predictable outputs and determinate behavior
             Higher values are more engaging but also less predictable
             Use High Values cautiously
 
             Returns:
@@ -133,15 +142,15 @@
                     assert temperature >= 0.0
                     assert temperature <= 1.0
                 return temperature
 
             # this seems to be a reasonable default
             return 0.7
 
-        def _max_tokens() -> int:
+        def _get_max_tokens() -> int:
             """ The Maximum Number of tokens to generate
             Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)
             The higher this value, the more each request will cost
 
             Returns:
                 int: the max tokens to generate
             """
@@ -149,51 +158,51 @@
                 if self.isEnabledForDebug:
                     Enforcer.is_int(max_tokens)
                 return max_tokens
 
             # whether this is reasonable depends entirely on the input prompt
             return 256
 
-        def _top_p() -> float:
+        def _get_top_p() -> float:
             """ Controls Diversity via Nucleus Sampling; no idea what this means
 
             Returns:
                 float: the top-p result
             """
             if top_p:
                 return top_p
 
             # I rarely change this setting
             return 1.0
 
-        def _frequency_penalty() -> int:
+        def _get_frequency_penalty() -> int:
             """ How much to penalize new tokens based on their frequency in the text so far
             Scale: 0.0 - 2.0
 
             Returns:
                 int: the frequency penalty
             """
             if frequency_penalty:
                 return frequency_penalty
             return 0.0
 
-        def _presence_penalty() -> int:
+        def _get_presence_penalty() -> int:
             """ Seems similar to frequency penalty
 
             Returns:
                 int: the presence penalty
             """
             if presence_penalty:
                 return presence_penalty
             return 2
 
         return {
             'engine': _engine(),
-            'input_prompt': _input_prompt(),
-            'temperature': _temperature(),
-            'max_tokens': _max_tokens(),
-            'top_p': _top_p(),
+            'input_prompt': _get_input_prompt(),
+            'temperature': _get_temperature(),
+            'max_tokens': _get_max_tokens(),
+            'top_p': _get_top_p(),
             'best_of': _best_of(),
-            'frequency_penalty': _frequency_penalty(),
-            'presence_penalty': _presence_penalty(),
+            'frequency_penalty': _get_frequency_penalty(),
+            'presence_penalty': _get_presence_penalty(),
             'timeout': self._timeout
         }
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/etl_handle_textcompletions.py` & `openai-helper-0.2.0/openai_helper/dmo/etl_replace_cliches.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-""" Handle Situations where OpenAI tries to complete a User Sentence """
+""" Replace Cliched Responses, which just add noise to the output """
 
 
 from baseblock import BaseObject
 
 
-class EtlHandleTextCompletions(BaseObject):
-    """ Handle Situations where OpenAI tries to complete a User Sentence """
+class EtlReplaceCliches(BaseObject):
+    """ A Generic Service to Extract Unstructured Output from an OpenAI response """
 
     def __init__(self):
         """ Change Log
 
         Created:
             4-Aug-2022
             craigtrim@gmail.com
             *   https://bast-ai.atlassian.net/browse/COR-56
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
                 input_text: str,
                 output_text: str) -> str:
-        """ Handle Situations where OpenAI tries to complete a User Sentence
-        These are not imperative to resolve, but resolution frequently results in cleaner output
+        """ Replace Cliched Responses, which just add noise to the output
 
         Args:
             input_text (str): the user input text
             output_text (str): the current state of the extracted text from OpenAI
 
         Returns:
             str: the potentially modified output text
         """
 
-        # this represents openAI trying to complete a user sentence
-        # openAI will generally do this if the user does not terminate their input with punctuation like .!?
-        # graffl now adds ending punctuation where none exists, so this pattern rarely takes place ...
-        if output_text.startswith(' ') and '\n\n' in output_text:
-            response = output_text.split('\n\n')[-1].strip()
-            if response and len(response):
-                return response
-
-        # this is more common and seems to represent another form of text completion
-        # an example is "0\n\nI'm not sure what you're asking"
-        # the text prior to the response tends to be brief
-        if '\n\n' in output_text:
-            lines = output_text.split('\n\n')
-            lines = [x.strip() for x in lines if x]
-            lines = [x for x in lines if len(x) > 5]
-            output_text = ' '.join(lines)
-            while '  ' in output_text:
-                output_text = output_text.replace('  ', ' ')
+        long_texts = [
+            "and that's where Loqi comes in.",
+            "If you're looking for a chatbot that will give you sassy responses to your questions",
+            'look no further than Loqi',
+            "He may not be the most helpful chatbot out there, but he's definitely the funniest",
+            'Loqi is a chatbot that reluctantly answers questions in a mocking tone'
+            'is a chatbot that responds to questions with',
+            'is a chatbot that reluctantly answers questions',
+        ]
+
+        for long_text in long_texts:
+            if long_text in output_text:
+                output_text = output_text.replace(long_text, '')
 
         return output_text
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/etl_remove_indicators.py` & `openai-helper-0.2.0/openai_helper/dmo/etl_remove_promptindicators.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 # -*- coding: UTF-8 -*-
 """ A Generic Service to Extract Unstructured Output from an OpenAI response """
 
 
 from baseblock import BaseObject
 
 
-class EtlRemoveIndicators(BaseObject):
+class EtlRemovePromptIndicators(BaseObject):
     """ A Generic Service to Extract Unstructured Output from an OpenAI response """
 
     def __init__(self):
         """ Change Log
 
         Created:
             4-Aug-2022
             craigtrim@gmail.com
             *   https://bast-ai.atlassian.net/browse/COR-56
+        Updated:
+            16-Nov-2022
+            craigtrim@gmail.com
+            *   renamed from 'etl-remove-indicators' in pursuit of
+                https://github.com/craigtrim/openai-helper/issues/2
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
                 input_text: str,
                 output_text: str) -> str:
         """ Eliminate Annoying Situations where OpenAI responds with something like
-            'Human: blah blah' 
+            'Human: blah blah'
         or
             'Assistant: blah blah'
 
         Args:
             input_text (str): the user input text
             output_text (str): the current state of the extracted text from OpenAI
 
@@ -56,14 +61,26 @@
         if 'Marv:' in output_text:
             output_text = output_text.replace('Marv:', '').strip()
 
         if 'Len:' in output_text:
             output_text = output_text.replace('Len:', '').strip()
 
         if "Marv's" in output_text:
-            output_text = output_text.replace("Marv's", "its")
+            output_text = output_text.replace("Marv's", 'its')
+
+        if "I'm an AI language model designed by OpenAI":
+            output_text = output_text.replace(
+                "I'm an AI language model designed by OpenAI", "I'm a bot")
+
+        if 'designed by OpenAI':
+            output_text = output_text.replace(
+                'designed by OpenAI', '')
+
+        if "I'm an AI language model":
+            output_text = output_text.replace(
+                "I'm an AI language model", "I'm a bot")
 
         if 'Two-Sentence Horror Story:' in output_text:
             output_text = output_text.replace(
                 'Two-Sentence Horror Story:', '').strip()
 
         return output_text
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/etl_replace_cliches.py` & `openai-helper-0.2.0/openai_helper/dmo/etl_replace_duplicatedinput.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-""" Replace Cliched Responses, which just add noise to the output """
+""" Replace any Input that is Quoted in the Output Text """
 
 
+from baseblock.common_utils import odds_of
+
 from baseblock import BaseObject
 
 
-class EtlReplaceCliches(BaseObject):
-    """ A Generic Service to Extract Unstructured Output from an OpenAI response """
+class EtlReplaceDuplicatedInput(BaseObject):
+    """ Replace any Input that is Quoted in the Output Text """
 
     def __init__(self):
         """ Change Log
 
         Created:
             4-Aug-2022
             craigtrim@gmail.com
             *   https://bast-ai.atlassian.net/browse/COR-56
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
                 input_text: str,
                 output_text: str) -> str:
-        """ Replace Cliched Responses, which just add noise to the output
+        """ Sometimes the Input is Quoted in the Output Text
+
+        Sample Input:
+            We are not put in this world for mere pleasure alone.
+
+        Sample Output:
+            We are not put in this world for mere pleasure alone.  Sometimes, we must suffer through pain and hardship to grow and become stronger.
+
+        Desired Output:
+            Sometimes, we must suffer through pain and hardship to grow and become stronger.
 
         Args:
             input_text (str): the user input text
-            output_text (str): the current state of the extracted text from OpenAI
+            output_text (str): the openAI response text
 
         Returns:
-            str: the potentially modified output text
+            str: the output text
         """
 
-        long_texts = [
-            "and that's where Loqi comes in.",
-            "If you're looking for a chatbot that will give you sassy responses to your questions",
-            "look no further than Loqi",
-            "He may not be the most helpful chatbot out there, but he's definitely the funniest",
-            "Loqi is a chatbot that reluctantly answers questions in a mocking tone"
-            "is a chatbot that responds to questions with",
-            "is a chatbot that reluctantly answers questions",
-        ]
-
-        for long_text in long_texts:
-            if long_text in output_text:
-                output_text = output_text.replace(long_text, "")
+        if input_text in output_text and input_text != output_text:
+            if odds_of(90):
+                output_text = output_text.replace(input_text, '')
 
         return output_text
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/etl_replace_duplicatedinput.py` & `openai-helper-0.2.0/openai_helper/dmo/etl_remove_emojis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-""" Replace any Input that is Quoted in the Output Text """
+""" A Generic Service to Remove Emoji Output from an OpenAI response """
 
 
-from baseblock.common_utils import odds_of
-
 from baseblock import BaseObject
 
 
-class EtlReplaceDuplicatedInput(BaseObject):
-    """ Replace any Input that is Quoted in the Output Text """
+class EtlRemoveEmojis(BaseObject):
+    """ A Generic Service to Remove Emoji Output from an OpenAI response """
 
     def __init__(self):
         """ Change Log
 
         Created:
-            4-Aug-2022
+            25-Feb-2023
             craigtrim@gmail.com
-            *   https://bast-ai.atlassian.net/browse/COR-56
+            *   https://github.com/craigtrim/openai-helper/issues/8
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
                 input_text: str,
                 output_text: str) -> str:
-        """ Sometimes the Input is Quoted in the Output Text
-
-        Sample Input: 
-            We are not put in this world for mere pleasure alone.
-
-        Sample Output: 
-            We are not put in this world for mere pleasure alone.  Sometimes, we must suffer through pain and hardship to grow and become stronger.
-
-        Desired Output: 
-            Sometimes, we must suffer through pain and hardship to grow and become stronger.
+        """ Entry Point
 
         Args:
             input_text (str): the user input text
-            output_text (str): the openAI response text
+            output_text (str): the current state of the extracted text from OpenAI
 
         Returns:
-            str: the output text
+            str: the potentially modified output text
         """
 
-        if input_text in output_text and input_text != output_text:
-            if odds_of(90):
-                output_text = output_text.replace(input_text, '')
+        if output_text.count(':') < 2:
+            return output_text
+
+        def is_emoji(token: str) -> bool:
+            if not token.startswith(':'):
+                return False
+            if not token.endswith(':'):
+                return False
+            return True
+
+        output_text = ' '.join([
+            x for x in output_text.split()
+            if not is_emoji(x)
+        ]).strip()
 
         return output_text
```

### Comparing `openai-helper-0.1.9/openai_helper/dmo/openai_connector.py` & `openai-helper-0.2.0/openai_helper/dmo/openai_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ Connect to OpenAI """
 
 
+from typing import Any
+from typing import Optional
+
 import openai
 
 from baseblock import EnvIO
 from baseblock import CryptoBase
 from baseblock import BaseObject
 
 
@@ -19,53 +22,53 @@
         Created:
             28-Jul-2022
             craigtrim@gmail.com
         """
         BaseObject.__init__(self, __name__)
 
     @classmethod
-    def _openai_key(cls) -> str:
+    def _openai_key(cls) -> Optional[str]:
         """ Retrieve OpenAI Key
 
         Use the encrypted key within the environment
 
         Returns:
             str: the decrypted OpenAI key
         """
         try:
             return CryptoBase().decrypt_str(EnvIO.str_or_exception('OPENAI_KEY'))
         except ValueError:
             return None
 
     @classmethod
-    def _openai_org(cls) -> str or None:
+    def _openai_org(cls) -> Optional[str]:
         """ Retrieve OpenAI org
 
         Use the encrypted key within the environment
 
         Returns:
             str: the decrypted OpenAI org
         """
         try:
             return CryptoBase().decrypt_str(EnvIO.str_or_exception('OPENAI_ORG'))
         except ValueError:
             return None
 
-    def _process(self) -> object:
+    def _process(self) -> Any:
         """ Connect to OpenAI
 
         Returns:
             object: an instantiated remote instance
         """
 
         openai.api_key = self._openai_key()
         openai.organization = self._openai_org()
 
         return openai
 
-    def process(self) -> object:
+    def process(self) -> Any:
         """ Connect to OpenAI
 
         Returns:
             object: an instantiated remote instance
         """
         return self._process()
```

### Comparing `openai-helper-0.1.9/openai_helper/svc/create_openai_answer.py` & `openai-helper-0.2.0/openai_helper/svc/create_openai_answer.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,52 +37,53 @@
     def _process(self,
                  input_text: str,
                  search_model: str) -> object or None:
         try:
 
             return self._conn.Answer.create(
                 search_model=search_model,
-                model="curie",
+                model='curie',
                 question=input_text,
                 return_metadata=True,
                 file=self._model_name,
-                examples_context="In 2017, U.S. life expectancy was 78.6 years.",
+                examples_context='In 2017, U.S. life expectancy was 78.6 years.',
                 examples=[
-                    ["What is human life expectancy in the United States?", "78 years."]],
+                    ['What is human life expectancy in the United States?', '78 years.']],
                 max_rerank=10,
                 max_tokens=5,
-                stop=["\n", "<|endoftext|>"]
+                stop=['\n', '<|endoftext|>']
             )
 
         except InvalidRequestError:
             # GRAFFL-350; not necessarily a defect, just didn't find similar documents
             if self.isEnabledForInfo:
                 self.logger.info('\n'.join([
-                    "No Similar Documents Were Found",
-                    f"\tInput Text: {input_text}",
-                    f"\tTrained Model: {self._model_name}",
-                    f"\tSearch Model: {search_model}"]))
+                    'No Similar Documents Were Found',
+                    f'\tInput Text: {input_text}',
+                    f'\tTrained Model: {self._model_name}',
+                    f'\tSearch Model: {search_model}']))
 
             return None
 
     def process(self,
                 input_text: str,
                 search_model: str) -> dict:
 
         sw = Stopwatch()
         output_events = []
 
         response = self._process(input_text=input_text,
                                  search_model=search_model)
 
-        response = dict(response)
+        if response:
+            response = dict(response)
 
         output_events.append(self._generate_event(
             service_name=self.component_name(),
-            event_name="create-openai-answer",
+            event_name='create-openai-answer',
             stopwatch=sw,
             data={
                 'input_text': input_text,
                 'search_model': search_model,
                 'response': response
             }))
```

### Comparing `openai-helper-0.1.9/openai_helper/svc/extract_top_response.py` & `openai-helper-0.2.0/openai_helper/svc/extract_top_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         output_events = []
 
         output_text = self._process(results=results,
                                     threshold=threshold)
 
         output_events.append(self._generate_event(
             service_name=self.component_name(),
-            event_name="extract-top-response",
+            event_name='extract-top-response',
             stopwatch=sw,
             data={
                 'input_text': results,
                 'threshold': threshold,
                 'output_text': output_text,
             }))
```

### Comparing `openai-helper-0.1.9/openai_helper/svc/run_openai_completion.py` & `openai-helper-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,118 @@
-#!/usr/bin/env python
-# -*- coding: UTF-8 -*-
-""" Run a Completion against openAI """
-
-
-from pprint import pformat
-
-from baseblock import EnvIO
-from baseblock import Enforcer
-from baseblock import Stopwatch
-from baseblock import BaseObject
-
-from openai_helper.dmo import CompletionEventExtractor
-
-
-class RunOpenAICompletion(BaseObject):
-    """ Run a Completion against openAI """
-
-    def __init__(self,
-                 conn: object,
-                 timeout: int = 5):
-        """ Change Log
-
-        Created:
-            28-Jul-2022
-            craigtrim@gmail.com
-
-        Args:
-            conn (object): a connected instance of OpenAI
-            timeout (int, optional): the timeout for the API call. Defaults to 15.
-        """
-        BaseObject.__init__(self, __name__)
-        self._completion = conn.Completion.create
-        self._extract_event = CompletionEventExtractor().process
-        self._timeout = EnvIO.int_or_default(
-            'OPENAI_CREATE_TIMEOUT', timeout)  # GRAFFL-380
-
-    def _process(self,
-                 d_event: dict) -> dict:
-
-        response = self._completion(
-            engine=d_event['engine'],
-            prompt=d_event['input_prompt'],
-            temperature=d_event['temperature'],
-            max_tokens=d_event['max_tokens'],
-            top_p=d_event['top_p'],
-            best_of=d_event['best_of'],
-            frequency_penalty=d_event['frequency_penalty'],
-            presence_penalty=d_event['presence_penalty'],
-            timeout=self._timeout  # GRAFFL-380
-        )
-
-        d_result = dict(response)
-        if self.isEnabledForDebug:
-            Enforcer.is_dict(d_event)
-            self.logger.debug('\n'.join([
-                "OpenAI Call Completed",
-                pformat(d_result)]))
-
-        return {
-            'input': d_event,
-            'output': d_result
-        }
-
-    def process(self,
-                input_prompt: str,
-                engine: str = None,
-                best_of: int = None,
-                temperature: float = None,
-                max_tokens: int = None,
-                top_p: float = None,
-                frequency_penalty: int = None,
-                presence_penalty: int = None) -> dict:
-        """ Run an OpenAI event
-
-        Args:
-            input_prompt (str): The Input Prompt to execute against OpenAI
-            engine (str, optional): The OpenAI model (engine) to run against. Defaults to None.
-                Options as of July, 2022 are:
-                    'text-davinci-002'
-                    'text-curie-001',
-                    'text-babbage-001'
-                    'text-ada-001'
-            best_of (int, optional): Generates Multiple Server-Side Combinations and only selects the best. Defaults to None.
-                This can really eat up OpenAI tokens so use with caution!
-            temperature (float, optional): Control Randomness; Scale is 0.0 - 1.0. Defaults to None.
-                Scale is 0.0 - 1.0
-                Lower values approach predictable outputs and determinate behavior
-                Higher values are more engaging but also less predictable
-                Use High Values cautiously
-            max_tokens (int, optional): The Maximum Number of tokens to generate. Defaults to None.
-                Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)
-                The higher this value, the more each request will cost.            
-            top_p (float, optional): Controls Diversity via Nucleus Sampling. Defaults to None.
-                no idea what this means
-            frequency_penalty (int, optional): How much to penalize new tokens based on their frequency in the text so far. Defaults to None.
-                Scale: 0.0 - 2.0.
-            presence_penalty (int, optional): Seems similar to frequency penalty. Defaults to None.
-
-        Returns:
-            dict: an output dictionary with two keys:
-                input: the input dictionary with validated parameters and default values where appropriate
-                output: the output event from OpenAI
-        """
-
-        sw = Stopwatch()
-
-        d_params = self._extract_event(
-            input_prompt=input_prompt,
-            engine=engine,
-            best_of=best_of,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            top_p=top_p,
-            frequency_penalty=frequency_penalty,
-            presence_penalty=presence_penalty)
-
-        d_result = self._process(d_params)
-
-        self.logger.debug('\n'.join([
-            "OpenAI Event Execution Completed",
-            f"\tTotal Time: {str(sw)}",
-            f"\tInput Params:\n{pformat(d_params)}",
-            f"\tOutput Result:\n{pformat(d_result)}"]))
+# OpenAI-Helper
+OpenAI Helper for Easy I/O
 
-        return d_result
+## Github
+https://github.com/craigtrim/openai-helper
+
+## Usage
+
+###  Set the OpenAI credentials
+```python
+import os
+os.environ['OPENAI_KEY'] = "<encrypted key>"
+os.environ['OPENAI_ORG'] = "<encrypted key>"
+```
+
+Use `CryptoBase.encrypt_str("...")` from https://pypi.org/project/baseblock/
+
+###  Initialize the OpenAI Helper:
+```python
+run = OpenAITextCompletion().run
+```
+This will connect to OpenAI and establish performant callbacks.
+
+### Call OpenAI:
+```python
+run(input_prompt="Generate a one random number between 1 and 5000")
+```
+
+or
+```python
+run(engine="text-ada-001",
+    temperature=1.0,
+    max_tokens=256,
+    input_prompt="Rewrite the input in grammatical English:\n\nInput: You believe I can help you understand what trust yourself? don't you?\nOutput:\n\n")
+```
+
+The output will contain both the input and output values:
+```json
+{
+   "input":{
+      "best_of":1,
+      "engine":"text-davinci-003",
+      "frequency_penalty":0.0,
+      "input_prompt":"Rewrite the input in grammatical English:\n\nInput: You believe I can help you understand what trust yourself? don't you?\nOutput:\n\n",
+      "max_tokens":256,
+      "presence_penalty":2,
+      "temperature":1.0,
+      "timeout":5,
+      "top_p":1.0
+   },
+   "output":{
+      "choices":[
+         {
+            "finish_reason":"stop",
+            "index":0,
+            "logprobs":"None",
+            "text":"Don't you believe that I can help you understand trust in yourself?"
+         }
+      ],
+      "created":1659051242,
+      "id":"cmpl-5Z7IwXM5bCwWj8IuHaGnOLn6bCvHz",
+      "model":"text-ada-001",
+      "object":"text_completion",
+      "usage":{
+         "completion_tokens":17,
+         "prompt_tokens":32,
+         "total_tokens":49
+      }
+   }
+}
+```
+
+## Supported Parameters and Defaults
+This method signature describes support:
+```python
+def process(self,
+            input_prompt: str,
+            engine: str = None,
+            best_of: int = None,
+            temperature: float = None,
+            max_tokens: int = None,
+            top_p: float = None,
+            frequency_penalty: int = None,
+            presence_penalty: int = None) -> dict:
+    """ Run an OpenAI event
+
+    Args:
+        input_prompt (str): The Input Prompt to execute against OpenAI
+        engine (str, optional): The OpenAI model (engine) to run against. Defaults to None.
+            Options as of July, 2022 are:
+                'text-davinci-003'
+                'text-curie-001',
+                'text-babbage-001'
+                'text-ada-001'
+        best_of (int, optional): Generates Multiple Server-Side Combinations and only selects the best. Defaults to None.
+            This can really eat up OpenAI tokens so use with caution!
+        temperature (float, optional): Control Randomness; Scale is 0.0 - 1.0. Defaults to None.
+            Scale is 0.0 - 1.0
+            Lower values approach predictable outputs and determinate behavior
+            Higher values are more engaging but also less predictable
+            Use High Values cautiously
+        max_tokens (int, optional): The Maximum Number of tokens to generate. Defaults to None.
+            Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)
+            The higher this value, the more each request will cost.
+        top_p (float, optional): Controls Diversity via Nucleus Sampling. Defaults to None.
+            no idea what this means
+        frequency_penalty (int, optional): How much to penalize new tokens based on their frequency in the text so far. Defaults to None.
+            Scale: 0.0 - 2.0.
+        presence_penalty (int, optional): Seems similar to frequency penalty. Defaults to None.
+
+    Returns:
+        dict: an output dictionary with two keys:
+            input: the input dictionary with validated parameters and default values where appropriate
+            output: the output event from OpenAI
+    """
+```
+
+## Counting Tokens (tiktoken)
```


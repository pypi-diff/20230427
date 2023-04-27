# Comparing `tmp/gentrace_py-0.5.5.tar.gz` & `tmp/gentrace_py-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.5.5.tar", max compression
+gzip compressed data, was "gentrace_py-0.5.6.tar", max compression
```

## Comparing `gentrace_py-0.5.5.tar` & `gentrace_py-0.5.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      968 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     1072 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    25461 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12257 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      968 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      967 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    25160 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      738 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12262 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-04-27 14:33:03.552108 gentrace_py-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.6/PKG-INFO
```

### Comparing `gentrace_py-0.5.5/gentrace/__init__.py` & `gentrace_py-0.5.6/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/api_client.py` & `gentrace_py-0.5.6/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/configuration.py` & `gentrace_py-0.5.6/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/exceptions.py` & `gentrace_py-0.5.6/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/feedback_request.py` & `gentrace_py-0.5.6/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/feedback_request.pyi` & `gentrace_py-0.5.6/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/feedback_response.py` & `gentrace_py-0.5.6/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/feedback_response.pyi` & `gentrace_py-0.5.6/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.5.6/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.5.6/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.5.6/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.5.6/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/models/__init__.py` & `gentrace_py-0.5.6/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.5.6/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.5.6/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/providers/llms/openai.py` & `gentrace_py-0.5.6/gentrace/providers/llms/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             )
         )
 
         if is_self_contained:
             submit_result = pipeline_run.submit()
 
             if not stream:
-                completion.pipeline_run_id = (
+                completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
 
 
 def create_stream_response(stream_list):
@@ -132,34 +132,28 @@
 
 
 def intercept_completion(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         prompt_template = kwargs.get("prompt_template")
         prompt_inputs = kwargs.get("prompt_inputs")
+        prompt = kwargs.get("prompt")
         pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
             if k not in ["prompt_template", "prompt_inputs"]
         }
 
-        if "prompt" in base_completion_options:
-            raise ValueError(
-                "The prompt attribute cannot be provided when using the Gentrace SDK. Use prompt_template and prompt_inputs instead."
-            )
-
-        if not prompt_template:
-            raise ValueError(
-                "The prompt_template attribute must be provided when using the Gentrace SDK."
-            )
-
         if stream:
-            rendered_prompt = pystache.render(prompt_template, prompt_inputs)
+            rendered_prompt = prompt
+
+            if prompt_template and prompt_inputs:
+                rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
             new_completion_options = {
                 **base_completion_options,
                 "prompt": rendered_prompt,
             }
 
             start_time = time.time()
@@ -169,15 +163,15 @@
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             def profiled_completion():
                 modified_response = []
                 for value in completion:
                     if value and is_self_contained:
-                        value["pipeline_run_id"] = pipeline_run_id
+                        value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
@@ -193,17 +187,23 @@
                     full_response,
                     pipeline_run_id if is_self_contained else None,
                     stream,
                 )
 
             return profiled_completion()
 
-        rendered_prompt = pystache.render(prompt_template, prompt_inputs)
+        rendered_prompt = prompt
+
+        if prompt_template and prompt_inputs:
+            rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
-        new_completion_options = {**base_completion_options, "prompt": rendered_prompt}
+        new_completion_options = {
+            **base_completion_options,
+            "prompt": rendered_prompt,
+        }
 
         start_time = time.time()
         completion = original_fn(**new_completion_options)
 
         end_time = time.time()
 
         create_completion_step_run(
@@ -226,34 +226,28 @@
 
 
 def intercept_completion_async(original_fn, gentrace_config: Configuration):
     @classmethod
     async def wrapper(cls, *args, **kwargs):
         prompt_template = kwargs.get("prompt_template")
         prompt_inputs = kwargs.get("prompt_inputs")
+        prompt = kwargs.get("prompt")
         pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
             if k not in ["prompt_template", "prompt_inputs"]
         }
 
-        if "prompt" in base_completion_options:
-            raise ValueError(
-                "The prompt attribute cannot be provided when using the Gentrace SDK. Use prompt_template and prompt_inputs instead."
-            )
-
-        if not prompt_template:
-            raise ValueError(
-                "The prompt_template attribute must be provided when using the Gentrace SDK."
-            )
-
         if stream:
-            rendered_prompt = pystache.render(prompt_template, prompt_inputs)
+            rendered_prompt = prompt
+
+            if prompt_template and prompt_inputs:
+                rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
             new_completion_options = {
                 **base_completion_options,
                 "prompt": rendered_prompt,
             }
 
             start_time = time.time()
@@ -263,15 +257,15 @@
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             async def profiled_completion():
                 modified_response = []
                 async for value in completion:
                     if value and is_self_contained:
-                        value["pipeline_run_id"] = pipeline_run_id
+                        value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
@@ -287,17 +281,23 @@
                     full_response,
                     pipeline_run_id if is_self_contained else None,
                     stream,
                 )
 
             return profiled_completion()
 
-        rendered_prompt = pystache.render(prompt_template, prompt_inputs)
+        rendered_prompt = prompt
+
+        if prompt_template and prompt_inputs:
+            rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
-        new_completion_options = {**base_completion_options, "prompt": rendered_prompt}
+        new_completion_options = {
+            **base_completion_options,
+            "prompt": rendered_prompt,
+        }
 
         start_time = time.time()
         completion = await original_fn(**new_completion_options)
         end_time = time.time()
 
         create_completion_step_run(
             cls,
@@ -337,15 +337,15 @@
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             def profiled_completion():
                 modified_response = []
                 for value in completion:
                     if value and is_self_contained:
-                        value["pipeline_run_id"] = pipeline_run_id
+                        value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 elapsed_time = int((end_time - start_time) * 1000)
 
@@ -412,15 +412,15 @@
                     model_params,
                     completion,
                 )
             )
 
             if is_self_contained:
                 submit_result = pipeline_run.submit()
-                completion.pipeline_run_id = (
+                completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
 
         return completion
 
@@ -446,15 +446,15 @@
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             async def profiled_completion():
                 modified_response = []
                 async for value in completion:
                     if value and is_self_contained:
-                        value["pipeline_run_id"] = pipeline_run_id
+                        value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
@@ -522,15 +522,15 @@
                     model_params,
                     completion,
                 )
             )
 
             if is_self_contained:
                 submit_result = pipeline_run.submit()
-                completion.pipeline_run_id = (
+                completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
         return completion
 
     return wrapper
@@ -574,15 +574,15 @@
                     {"model": model},
                     completion,
                 )
             )
 
             if is_self_contained:
                 submit_result = pipeline_run.submit()
-                completion.pipeline_run_id = (
+                completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
         return completion
 
     return wrapper
@@ -626,15 +626,15 @@
                     {"model": model},
                     completion,
                 )
             )
 
             if is_self_contained:
                 submit_result = pipeline_run.submit()
-                completion.pipeline_run_id = (
+                completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
 
         return completion
```

### Comparing `gentrace_py-0.5.5/gentrace/providers/pipeline.py` & `gentrace_py-0.5.6/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/providers/pipeline_run.py` & `gentrace_py-0.5.6/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/providers/step_run.py` & `gentrace_py-0.5.6/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/providers/utils.py` & `gentrace_py-0.5.6/gentrace/providers/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from gentrace.apis.tags.ingestion_api import IngestionApi
 from gentrace.models import PipelineRunRequest
 
 __all__ = ["to_date_string"]
 
 
 def to_date_string(time_value):
-    return (
-        datetime.fromtimestamp(time_value).strftime("%Y-%m-%dT%H:%M:%S.%fZ")[:-4] + "Z"
-    )
+    utc_time = datetime.utcfromtimestamp(time_value)
+    utc_time_str = utc_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+    return utc_time_str[:-4] + "Z"
 
 
 async def pipeline_run_post_background(
     api_instance: IngestionApi, pipeline_run_data: PipelineRunRequest
 ):
     with ThreadPoolExecutor() as executor:
         result = await asyncio.get_event_loop().run_in_executor(
```

### Comparing `gentrace_py-0.5.5/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.5.6/gentrace/providers/vectorstores/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 {"ids": ids, "namespace": namespace},
                 response.to_dict(),
             ),
             pipeline_id,
         )
 
         if pipeline_run_id:
-            response.pipeline_run_id = pipeline_run_id
+            response["pipelineRunId"] = pipeline_run_id
 
         return response
 
     def update(
         self,
         id: str,
         values: Optional[List[float]] = None,
@@ -125,15 +125,15 @@
                 },
                 response,
             ),
             pipeline_id,
         )
 
         if pipeline_run_id:
-            response.pipeline_run_id = pipeline_run_id
+            response["pipelineRunId"] = pipeline_run_id
 
         return response
 
     def query(
         self,
         vector: Optional[List[float]] = None,
         id: Optional[str] = None,
@@ -185,15 +185,15 @@
                 {**model_params},
                 response.to_dict(),
             ),
             pipeline_id,
         )
 
         if pipeline_run_id:
-            response.pipeline_run_id = pipeline_run_id
+            response["pipelineRunId"] = pipeline_run_id
 
         return response
 
     def upsert(
         self,
         vectors: Union[List[Vector], List[tuple], List[dict]],
         namespace: Optional[str] = None,
@@ -222,15 +222,15 @@
                 },
                 response.to_dict(),
             ),
             pipeline_id,
         )
 
         if pipeline_run_id:
-            response.pipeline_run_id = pipeline_run_id
+            response["pipelineRunId"] = pipeline_run_id
 
         return response
 
     def delete(
         self,
         ids: Optional[List[str]] = None,
         delete_all: Optional[bool] = None,
@@ -258,15 +258,15 @@
                 },
                 response,
             ),
             pipeline_id,
         )
 
         if pipeline_run_id:
-            response.pipeline_run_id = pipeline_run_id
+            response["pipelineRunId"] = pipeline_run_id
 
         return response
 
 
 def Index(index_name: str, pool_threads=1, *args, **kwargs):
     modified_index = ModifiedIndex(index_name, pool_threads, *args, **kwargs)
     return modified_index
```

### Comparing `gentrace_py-0.5.5/gentrace/rest.py` & `gentrace_py-0.5.6/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/gentrace/schemas.py` & `gentrace_py-0.5.6/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.5/pyproject.toml` & `gentrace_py-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.5.5"
+version = "0.5.6"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.5.5/PKG-INFO` & `gentrace_py-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


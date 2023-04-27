# Comparing `tmp/simplechain-0.0.3.tar.gz` & `tmp/simplechain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.3.tar", last modified: Sun Apr 16 16:54:24 2023, max compression
+gzip compressed data, was "simplechain-0.0.4.tar", last modified: Thu Apr 27 21:47:08 2023, max compression
```

## Comparing `simplechain-0.0.3.tar` & `simplechain-0.0.4.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.237884 simplechain-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      600 2023-04-16 16:54:24.236884 simplechain-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-16 16:54:24.237884 simplechain-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1103 2023-04-16 16:54:12.000000 simplechain-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.083884 simplechain-0.0.3/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.3/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.109884 simplechain-0.0.3/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.3/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.113885 simplechain-0.0.3/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.3/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.3/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.3/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.121884 simplechain-0.0.3/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.127883 simplechain-0.0.3/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.3/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.3/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.3/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.142883 simplechain-0.0.3/simplechain/stack/
--rw-rw-rw-   0        0        0      226 2023-04-11 18:57:45.000000 simplechain-0.0.3/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.155884 simplechain-0.0.3/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.3/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.3/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.3/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     2805 2023-04-11 21:35:31.000000 simplechain-0.0.3/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.156884 simplechain-0.0.3/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.3/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.157884 simplechain-0.0.3/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.3/simplechain/stack/pdf_loaders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.169885 simplechain-0.0.3/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.3/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.186886 simplechain-0.0.3/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.3/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.3/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1112 2023-04-11 15:45:29.000000 simplechain-0.0.3/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.189884 simplechain-0.0.3/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.3/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.203884 simplechain-0.0.3/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.228885 simplechain-0.0.3/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.3/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.3/simplechain/stack/vector_databases/annoy.py
--rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.3/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.3/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.3/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.101883 simplechain-0.0.3/simplechain.egg-info/
--rw-rw-rw-   0        0        0      600 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1764 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.235885 simplechain-0.0.3/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.736863 simplechain-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      600 2023-04-27 21:47:08.735856 simplechain-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-27 21:47:08.736863 simplechain-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2023-04-27 21:46:39.000000 simplechain-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.574855 simplechain-0.0.4/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.4/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.618878 simplechain-0.0.4/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.4/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.627874 simplechain-0.0.4/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.4/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.4/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.4/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.649876 simplechain-0.0.4/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.4/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.4/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.4/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.4/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.668872 simplechain-0.0.4/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.4/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.4/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.4/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.4/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.673856 simplechain-0.0.4/simplechain/stack/
+-rw-rw-rw-   0        0        0      226 2023-04-11 18:57:45.000000 simplechain-0.0.4/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.684868 simplechain-0.0.4/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.4/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.4/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.4/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     2942 2023-04-27 21:45:41.000000 simplechain-0.0.4/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.685857 simplechain-0.0.4/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.4/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.687874 simplechain-0.0.4/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.4/simplechain/stack/pdf_loaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.705872 simplechain-0.0.4/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.4/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.4/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.4/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.710856 simplechain-0.0.4/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.4/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-04-27 21:44:55.000000 simplechain-0.0.4/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.4/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1105 2023-04-27 21:45:05.000000 simplechain-0.0.4/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.713872 simplechain-0.0.4/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.4/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.4/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.719856 simplechain-0.0.4/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.4/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.4/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.4/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.4/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.726859 simplechain-0.0.4/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.4/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.4/simplechain/stack/vector_databases/annoy.py
+-rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.4/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.4/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.4/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.593857 simplechain-0.0.4/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-04-27 21:47:08.000000 simplechain-0.0.4/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1805 2023-04-27 21:47:08.000000 simplechain-0.0.4/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 21:47:08.000000 simplechain-0.0.4/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-27 21:47:08.000000 simplechain-0.0.4/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 21:47:08.732870 simplechain-0.0.4/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.4/tests/__init__.py
```

### Comparing `simplechain-0.0.3/LICENSE` & `simplechain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/PKG-INFO` & `simplechain-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.3/README.rst` & `simplechain-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/setup.py` & `simplechain-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.3/simplechain/pipeline/module.py` & `simplechain-0.0.4/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.4/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.4/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/pipeline/providers/database.py` & `simplechain-0.0.4/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.4/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/databases/base.py` & `simplechain-0.0.4/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/databases/sql.py` & `simplechain-0.0.4/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/factory.py` & `simplechain-0.0.4/simplechain/stack/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-import langchain
-
 from simplechain.stack.text_embedders.base import TextEmbedder
 from simplechain.stack.text_generators.base import TextGenerator
 from simplechain.stack.vector_databases.base import VectorDatabase
 
 
 class TextEmbedderFactory:
     @classmethod
-    def create(cls, name: str, *args, **kwargs) -> TextEmbedder:
+    def create(cls, name: str, **kwargs) -> TextEmbedder:
         if name == "openai":
             from simplechain.stack.text_embedders.openai import TextEmbedderOpenAI
-            return TextEmbedderOpenAI(*args, **kwargs)
+            return TextEmbedderOpenAI(**kwargs)
+        elif name == "ai21":
+            from simplechain.stack.text_embedders.ai21 import TextEmbedderAI21
+            return TextEmbedderAI21(**kwargs)
         else:
             raise ValueError(f"Invalid name: {name}.")
+
     @classmethod
-    def createOpenAI(cls, *args, **kwargs) -> TextEmbedder:
+    def createOpenAI(cls, **kwargs) -> TextEmbedder:
         from simplechain.stack.text_embedders.openai import TextEmbedderOpenAI
-        return TextEmbedderOpenAI(*args, **kwargs)
+        return TextEmbedderOpenAI(**kwargs)
+
 
 class VectorDatabaseFactory:
     @classmethod
     def create(cls, name: str, *args, **kwargs) -> VectorDatabase:
         if name == "annoy":
             from simplechain.stack.vector_databases.annoy import Annoy
             return Annoy(*args, **kwargs)
         else:
             raise ValueError(f"Invalid name: {name}.")
 
 
 class PDFLoaderFactory:
+    import langchain
+
     @classmethod
     def create(cls, name: str, file_path: str) -> langchain.document_loaders.pdf.BasePDFLoader:
         if name == "unstructured":
             from langchain.document_loaders import UnstructuredPDFLoader
             loader = UnstructuredPDFLoader(file_path)
             data = loader.load()
         elif name == "pdfminer":
@@ -51,19 +56,19 @@
             from langchain.document_loaders import PyMuPDFLoader
             loader = PyMuPDFLoader(file_path)
             data = loader.load()
         else:
             raise ValueError(f"Invalid name: {name}.")
         return data
 
+
 class TextGeneratorFactory:
     @classmethod
     def create(cls, name: str, **kwargs) -> TextGenerator:
         if name == "openai":
             from simplechain.stack.text_generators.llms.openai import TextGeneratorOpenAI
             return TextGeneratorOpenAI(**kwargs)
         elif name == "ai21":
             from simplechain.stack.text_generators.llms.ai21 import TextGeneratorAI21
             return TextGeneratorAI21(**kwargs)
         else:
             raise ValueError(f"Invalid name: {name}.")
-
```

### Comparing `simplechain-0.0.3/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.4/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.4/simplechain/stack/text_embedders/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List, Dict
+from typing import List, Dict
 
 import numpy as np
 import openai
 from pydantic import root_validator
 
 from simplechain.stack.text_embedders.base import TextEmbedder
 from simplechain.utils import get_from_dict_or_env
```

### Comparing `simplechain-0.0.3/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.4/simplechain/stack/text_generators/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.4/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.4/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/vector_databases/annoy.py` & `simplechain-0.0.4/simplechain/stack/vector_databases/annoy.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.4/simplechain/stack/vector_databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.4/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain/utils.py` & `simplechain-0.0.4/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.3/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.4/simplechain.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.3/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.4/simplechain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 simplechain/stack/databases/sql.py
 simplechain/stack/image_generators/__init__.py
 simplechain/stack/pdf_loaders/__init__.py
 simplechain/stack/search_engines/__init__.py
 simplechain/stack/search_engines/base.py
 simplechain/stack/search_engines/google_serper.py
 simplechain/stack/text_embedders/__init__.py
+simplechain/stack/text_embedders/ai21.py
 simplechain/stack/text_embedders/base.py
 simplechain/stack/text_embedders/openai.py
 simplechain/stack/text_generators/__init__.py
 simplechain/stack/text_generators/base.py
 simplechain/stack/text_generators/llms/__init__.py
 simplechain/stack/text_generators/llms/ai21.py
 simplechain/stack/text_generators/llms/llm.py
```


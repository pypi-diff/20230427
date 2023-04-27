# Comparing `tmp/mteval-0.0.1.tar.gz` & `tmp/mteval-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteval-0.0.1.tar", last modified: Mon Nov 21 19:22:36 2022, max compression
+gzip compressed data, was "mteval-0.0.2.tar", last modified: Thu Apr 27 16:50:59 2023, max compression
```

## Comparing `mteval-0.0.1.tar` & `mteval-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2022-11-21 19:22:36.452989 mteval-0.0.1/
--rw-r--r--   0 achim     (1000) achim     (1000)    11337 2022-11-04 18:44:24.000000 mteval-0.0.1/LICENSE
--rw-r--r--   0 achim     (1000) achim     (1000)      111 2022-11-04 18:44:24.000000 mteval-0.0.1/MANIFEST.in
--rw-r--r--   0 achim     (1000) achim     (1000)     7106 2022-11-21 19:22:36.452989 mteval-0.0.1/PKG-INFO
--rw-r--r--   0 achim     (1000) achim     (1000)     5156 2022-11-21 18:58:57.000000 mteval-0.0.1/README.md
-drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2022-11-21 19:22:36.452989 mteval-0.0.1/mteval/
--rw-r--r--   0 achim     (1000) achim     (1000)       22 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/__init__.py
--rw-r--r--   0 achim     (1000) achim     (1000)     4449 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/_modidx.py
--rw-r--r--   0 achim     (1000) achim     (1000)      814 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/awsmt.py
--rw-r--r--   0 achim     (1000) achim     (1000)     1671 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/bleu.py
--rw-r--r--   0 achim     (1000) achim     (1000)     3017 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/comet.py
--rw-r--r--   0 achim     (1000) achim     (1000)     4939 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/dataset.py
--rw-r--r--   0 achim     (1000) achim     (1000)     1460 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/deeplmt.py
--rw-r--r--   0 achim     (1000) achim     (1000)     1404 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/googlemt.py
--rw-r--r--   0 achim     (1000) achim     (1000)     1729 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/microsoftmt.py
--rw-r--r--   0 achim     (1000) achim     (1000)      691 2022-11-21 18:58:38.000000 mteval-0.0.1/mteval/util.py
-drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2022-11-21 19:22:36.452989 mteval-0.0.1/mteval.egg-info/
--rw-r--r--   0 achim     (1000) achim     (1000)     7106 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/PKG-INFO
--rw-r--r--   0 achim     (1000) achim     (1000)      438 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/SOURCES.txt
--rw-r--r--   0 achim     (1000) achim     (1000)        1 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/dependency_links.txt
--rw-r--r--   0 achim     (1000) achim     (1000)       55 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/entry_points.txt
--rw-r--r--   0 achim     (1000) achim     (1000)        1 2022-11-04 18:51:23.000000 mteval-0.0.1/mteval.egg-info/not-zip-safe
--rw-r--r--   0 achim     (1000) achim     (1000)      101 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/requires.txt
--rw-r--r--   0 achim     (1000) achim     (1000)        7 2022-11-21 19:22:36.000000 mteval-0.0.1/mteval.egg-info/top_level.txt
--rw-r--r--   0 achim     (1000) achim     (1000)     1038 2022-11-16 18:47:00.000000 mteval-0.0.1/settings.ini
--rw-r--r--   0 achim     (1000) achim     (1000)       38 2022-11-21 19:22:36.452989 mteval-0.0.1/setup.cfg
--rw-r--r--   0 achim     (1000) achim     (1000)     2541 2022-11-04 18:44:24.000000 mteval-0.0.1/setup.py
+drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2023-04-27 16:50:59.836310 mteval-0.0.2/
+-rw-r--r--   0 achim     (1000) achim     (1000)    11337 2022-11-04 18:44:24.000000 mteval-0.0.2/LICENSE
+-rw-r--r--   0 achim     (1000) achim     (1000)      111 2022-11-04 18:44:24.000000 mteval-0.0.2/MANIFEST.in
+-rw-r--r--   0 achim     (1000) achim     (1000)     7115 2023-04-27 16:50:59.836310 mteval-0.0.2/PKG-INFO
+-rw-r--r--   0 achim     (1000) achim     (1000)     5182 2023-03-10 01:32:03.000000 mteval-0.0.2/README.md
+drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2023-04-27 16:50:59.836310 mteval-0.0.2/mteval/
+-rw-r--r--   0 achim     (1000) achim     (1000)       22 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/__init__.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     6690 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/_modidx.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     1591 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/awsmt.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     1671 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/bleu.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     3128 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/comet.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     5065 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/dataset.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     2212 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/deeplmt.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     2736 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/googlemt.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     3358 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/microsoftmt.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     5395 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/modernmt.py
+-rw-r--r--   0 achim     (1000) achim     (1000)     4587 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/ter.py
+-rw-r--r--   0 achim     (1000) achim     (1000)      691 2023-04-27 16:26:45.000000 mteval-0.0.2/mteval/util.py
+drwxr-xr-x   0 achim     (1000) achim     (1000)        0 2023-04-27 16:50:59.836310 mteval-0.0.2/mteval.egg-info/
+-rw-r--r--   0 achim     (1000) achim     (1000)     7115 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/PKG-INFO
+-rw-r--r--   0 achim     (1000) achim     (1000)      471 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/SOURCES.txt
+-rw-r--r--   0 achim     (1000) achim     (1000)        1 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/dependency_links.txt
+-rw-r--r--   0 achim     (1000) achim     (1000)       55 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/entry_points.txt
+-rw-r--r--   0 achim     (1000) achim     (1000)        1 2022-11-04 18:51:23.000000 mteval-0.0.2/mteval.egg-info/not-zip-safe
+-rw-r--r--   0 achim     (1000) achim     (1000)      120 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/requires.txt
+-rw-r--r--   0 achim     (1000) achim     (1000)        7 2023-04-27 16:50:59.000000 mteval-0.0.2/mteval.egg-info/top_level.txt
+-rw-r--r--   0 achim     (1000) achim     (1000)      912 2023-04-27 16:26:45.000000 mteval-0.0.2/settings.ini
+-rw-r--r--   0 achim     (1000) achim     (1000)       38 2023-04-27 16:50:59.846310 mteval-0.0.2/setup.cfg
+-rw-r--r--   0 achim     (1000) achim     (1000)     2541 2022-11-04 18:44:24.000000 mteval-0.0.2/setup.py
```

### Comparing `mteval-0.0.1/LICENSE` & `mteval-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mteval-0.0.1/PKG-INFO` & `mteval-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mteval
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to automate machine translation evaluation
-Home-page: https://github.com/polyglottech/mteval
-Author: Polyglot Technology LLC
-Author-email: info@polyglot.technology
+Home-page: https://github.com/achimr/mteval
+Author: Achim Ruopp
+Author-email: achimru@gmail.com
 License: Apache Software License 2.0
 Description: mteval
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         <div>
@@ -48,14 +48,15 @@
             export GOOGLE_PROJECT_ID=''
             export MS_SUBSCRIPTION_KEY=''
             export MS_REGION=''
             export AWS_DEFAULT_REGION=''
             export AWS_ACCESS_KEY_ID=''
             export AWS_SECRET_ACCESS_KEY=''
             export DEEPL_API_KEY=''
+            export MMT_API_KEY=''
         
         #### How to obtain subscription credentials
         
         - [Amazon
           Translate](https://docs.aws.amazon.com/translate/latest/dg/setting-up.html)
         - [DeepL](https://www.deepl.com/docs-api/api-access/authentication/)
         - [Google Translate](https://cloud.google.com/translate/docs/setup)
```

### Comparing `mteval-0.0.1/README.md` & `mteval-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     export GOOGLE_PROJECT_ID=''
     export MS_SUBSCRIPTION_KEY=''
     export MS_REGION=''
     export AWS_DEFAULT_REGION=''
     export AWS_ACCESS_KEY_ID=''
     export AWS_SECRET_ACCESS_KEY=''
     export DEEPL_API_KEY=''
+    export MMT_API_KEY=''
 
 #### How to obtain subscription credentials
 
 - [Amazon
   Translate](https://docs.aws.amazon.com/translate/latest/dg/setting-up.html)
 - [DeepL](https://www.deepl.com/docs-api/api-access/authentication/)
 - [Google Translate](https://cloud.google.com/translate/docs/setup)
```

### Comparing `mteval-0.0.1/mteval/_modidx.py` & `mteval-0.0.2/mteval/_modidx.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/mteval',
-                'doc_host': 'https://polyglottech.github.io',
-                'git_url': 'https://github.com/polyglottech/mteval',
+                'doc_host': 'https://achimr.github.io',
+                'git_url': 'https://github.com/achimr/mteval',
                 'lib_path': 'mteval'},
   'syms': { 'mteval.awsmt': { 'mteval.awsmt.awstranslate': ('awsmt.html#awstranslate', 'mteval/awsmt.py'),
                               'mteval.awsmt.awstranslate.__init__': ('awsmt.html#awstranslate.__init__', 'mteval/awsmt.py'),
+                              'mteval.awsmt.awstranslate.check_langpair': ('awsmt.html#awstranslate.check_langpair', 'mteval/awsmt.py'),
                               'mteval.awsmt.awstranslate.translate_text': ('awsmt.html#awstranslate.translate_text', 'mteval/awsmt.py')},
             'mteval.bleu': { 'mteval.bleu.measure_bleu': ('bleu.html#measure_bleu', 'mteval/bleu.py'),
                              'mteval.bleu.measure_record_bleu': ('bleu.html#measure_record_bleu', 'mteval/bleu.py')},
             'mteval.comet': { 'mteval.comet.cometscoring': ('comet.html#cometscoring', 'mteval/comet.py'),
                               'mteval.comet.cometscoring.__init__': ('comet.html#cometscoring.__init__', 'mteval/comet.py'),
                               'mteval.comet.cometscoring.measure_comet': ('comet.html#cometscoring.measure_comet', 'mteval/comet.py'),
                               'mteval.comet.cometscoring.measure_record_comet': ( 'comet.html#cometscoring.measure_record_comet',
@@ -25,18 +26,35 @@
                                 'mteval.deeplmt.deepltranslate.check_langpair': ( 'deeplmt.html#deepltranslate.check_langpair',
                                                                                   'mteval/deeplmt.py'),
                                 'mteval.deeplmt.deepltranslate.translate_text': ( 'deeplmt.html#deepltranslate.translate_text',
                                                                                   'mteval/deeplmt.py')},
             'mteval.googlemt': { 'mteval.googlemt.googletranslate': ('googlemt.html#googletranslate', 'mteval/googlemt.py'),
                                  'mteval.googlemt.googletranslate.__init__': ( 'googlemt.html#googletranslate.__init__',
                                                                                'mteval/googlemt.py'),
+                                 'mteval.googlemt.googletranslate.check_langpair': ( 'googlemt.html#googletranslate.check_langpair',
+                                                                                     'mteval/googlemt.py'),
                                  'mteval.googlemt.googletranslate.translate_text': ( 'googlemt.html#googletranslate.translate_text',
                                                                                      'mteval/googlemt.py')},
             'mteval.microsoftmt': { 'mteval.microsoftmt.microsofttranslate': ( 'microsoftmt.html#microsofttranslate',
                                                                                'mteval/microsoftmt.py'),
                                     'mteval.microsoftmt.microsofttranslate.__init__': ( 'microsoftmt.html#microsofttranslate.__init__',
                                                                                         'mteval/microsoftmt.py'),
+                                    'mteval.microsoftmt.microsofttranslate.check_langpair': ( 'microsoftmt.html#microsofttranslate.check_langpair',
+                                                                                              'mteval/microsoftmt.py'),
                                     'mteval.microsoftmt.microsofttranslate.translate_text': ( 'microsoftmt.html#microsofttranslate.translate_text',
                                                                                               'mteval/microsoftmt.py')},
+            'mteval.modernmt': { 'mteval.modernmt.modernmttranslate': ('modernmt.html#modernmttranslate', 'mteval/modernmt.py'),
+                                 'mteval.modernmt.modernmttranslate.__init__': ( 'modernmt.html#modernmttranslate.__init__',
+                                                                                 'mteval/modernmt.py'),
+                                 'mteval.modernmt.modernmttranslate.add_reference_translation': ( 'modernmt.html#modernmttranslate.add_reference_translation',
+                                                                                                  'mteval/modernmt.py'),
+                                 'mteval.modernmt.modernmttranslate.check_langpair': ( 'modernmt.html#modernmttranslate.check_langpair',
+                                                                                       'mteval/modernmt.py'),
+                                 'mteval.modernmt.modernmttranslate.create_adaptation_tm': ( 'modernmt.html#modernmttranslate.create_adaptation_tm',
+                                                                                             'mteval/modernmt.py'),
+                                 'mteval.modernmt.modernmttranslate.translate_text': ( 'modernmt.html#modernmttranslate.translate_text',
+                                                                                       'mteval/modernmt.py')},
+            'mteval.ter': { 'mteval.ter.measure_record_ter': ('ter.html#measure_record_ter', 'mteval/ter.py'),
+                            'mteval.ter.measure_ter': ('ter.html#measure_ter', 'mteval/ter.py')},
             'mteval.util': { 'mteval.util.util': ('util.html#util', 'mteval/util.py'),
                              'mteval.util.util.__init__': ('util.html#util.__init__', 'mteval/util.py'),
                              'mteval.util.util.normalize_quotes': ('util.html#util.normalize_quotes', 'mteval/util.py')}}}
```

### Comparing `mteval-0.0.1/mteval/bleu.py` & `mteval-0.0.2/mteval/bleu.py`

 * *Files identical despite different names*

### Comparing `mteval-0.0.1/mteval/comet.py` & `mteval-0.0.2/mteval/comet.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 from comet import download_model, load_from_checkpoint
 from pathlib import Path
 import csv
 import os
 
 class cometscoring:
     """Class to calculate COMET score (with references)"""
-    def __init__(self,model_name="wmt20-comet-da"):
+    def __init__(self,model_name="Unbabel/wmt22-comet-da",gpus=1):
         """Constructor that downloads and loads the COMET model"""
         model_path = download_model(model_name)
         self.model = load_from_checkpoint(model_path)
+        self.gpus = gpus
 
     def measure_comet(self,source_lines,hypothesis_lines,reference_lines):
         """Function to calculate the comet score"""
         # Construct array necessary to measure COMET
         comet_data = []
         for (src,mt,ref) in zip(source_lines,hypothesis_lines,reference_lines):
             comet_dict = {"src":src,"mt":mt,"ref":ref}
             comet_data.append(comet_dict)
         # Run COMET
-        seg_scores, sys_score = self.model.predict(comet_data, batch_size=8, gpus=1)
+        outputs = self.model.predict(comet_data, batch_size=8, gpus=self.gpus)
+        sys_score = outputs.system_score
+        seg_scores = outputs.scores
 
         return seg_scores, sys_score
 
     def measure_record_comet(self,source_lines,hypothesis_lines,reference_lines,sourcelang,targetlang,test_set_name,test_date,mtengine,score_pathname,score_fname,domain=''):
         """Function to score hypothesis with COMET score and record score to a specified metrics file"""           
         seg_comet_scores, sys_score = self.measure_comet(source_lines,hypothesis_lines,reference_lines)
```

### Comparing `mteval-0.0.1/mteval/dataset.py` & `mteval-0.0.2/mteval/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,22 @@
     if not ref_file.exists():
         raise FileNotFoundError(errno.ENOENT,os.strerror(errno.ENOENT),ref_path) 
     
     return read_source_ref(source_path,ref_path)
 
 # %% ../nbs/02_dataset.ipynb 11
 import sys
-def get_translated_test_set(base_path,sourcelang,targetlang,mtengine,test_set_name,test_date):
+def get_translated_test_set(base_path,sourcelang,targetlang,mtengine,test_set_name,test_date,domain=''):
     """Read MT hypothesis translations for specified MT engine"""
     target_lines = []
     langpair = sourcelang+"-"+targetlang
-    output_filename = "hyp_"+mtengine+"."+langpair+"."+targetlang
+    if domain == '':
+        output_filename = "hyp_"+mtengine+"."+langpair+"."+targetlang
+    else:
+        output_filename = "hyp_"+mtengine+"."+domain+"."+langpair+"."+targetlang
     from pathlib import Path
     translate_file = Path(base_path+sourcelang+"_"+targetlang+"/"+test_date+"/"+test_set_name+"/"+output_filename)
     if translate_file.exists():
         with translate_file.open() as target_file:
             for target_line in target_file:
                 target_line = target_line.rstrip()
                 target_lines.append(target_line)
```

### Comparing `mteval-0.0.1/mteval/deeplmt.py` & `mteval-0.0.2/mteval/deeplmt.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,36 +3,50 @@
 # %% auto 0
 __all__ = ['deepltranslate']
 
 # %% ../nbs/07_deeplmt.ipynb 8
 import os
 import deepl
 from pathlib import Path
+from langcodes import *
 
 class deepltranslate:
     """Class to get translations from the DeepL API"""
     def __init__(self):
         """Constructor of deepltranslate class"""
         self._apikey = os.getenv('DEEPL_API_KEY')
         self._translator = deepl.Translator(self._apikey)
-
-    def translate_text(self,sourcelang, targetlang, text):
-        """Function to translate text into the target language"""
-        source_langid_upper = sourcelang.upper()
-        target_langid_upper = targetlang.upper()
-
-        result = self._translator.translate_text(text,source_lang=source_langid_upper,target_lang=target_langid_upper,split_sentences='off')
-
-        return result.text
+        # Caches for supported source and target language ids
+        self._source_languages = []
+        self._target_languages = []
 
     def check_langpair(self,sourcelang, targetlang):
         """Function to check if the language pair is supported"""
-        source_langid_upper = sourcelang.upper()
-        target_langid_upper = targetlang.upper()
-        supported_source_languages = [lang.code for lang in self._translator.get_source_languages()]
-        supported_target_languages = [lang.code for lang in self._translator.get_target_languages()]
-        
-        if source_langid_upper in supported_source_languages:
-            if target_langid_upper in supported_target_languages:
-                return True
+        if tag_is_valid(sourcelang) and tag_is_valid(targetlang):
+            source_langid_upper = sourcelang.upper()
+            target_langid_upper = targetlang.upper()
+            supported_source_languages = self._source_languages
+            if not supported_source_languages:
+                supported_source_languages = [lang.code for lang in self._translator.get_source_languages()]
+                self._source_languages = supported_source_languages
+            supported_target_languages = self._target_languages
+            if not supported_target_languages:
+                supported_target_languages = [lang.code for lang in self._translator.get_target_languages()]
+                self._target_languages = supported_target_languages
+
+            if source_langid_upper in supported_source_languages:
+                if target_langid_upper in supported_target_languages:
+                    return True
         
         return False
+
+    def translate_text(self,sourcelang, targetlang, text):
+        """Function to translate text into the target language"""
+        translated_text = ""
+        if self.check_langpair(sourcelang,targetlang):
+            source_langid_upper = sourcelang.upper()
+            target_langid_upper = targetlang.upper()
+            result = self._translator.translate_text(text,source_lang=source_langid_upper,target_lang=target_langid_upper,split_sentences='off')
+            translated_text = result.text
+
+        return translated_text
+
```

### Comparing `mteval-0.0.1/mteval/googlemt.py` & `mteval-0.0.2/mteval/awsmt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_googlemt.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_awsmt.ipynb.
 
 # %% auto 0
-__all__ = ['googletranslate']
+__all__ = ['awstranslate']
 
-# %% ../nbs/04_googlemt.ipynb 8
+# %% ../nbs/06_awsmt.ipynb 8
 import os
-import six
-from google.cloud import translate
-
-class googletranslate:
-    """Class to get translations from the Google Translate API"""
+import boto3
+import time
+from pathlib import Path
+from langcodes import *
 
+class awstranslate:
+    """Class to get translations from the Amazon Web Service Translate API"""
     def __init__(self):
-        """ Constructor of googletranslate class. Load the credentials for the Google API"""
-        # Google credentials need to be available in JSON file specified in the GOOGLE_APPLICATION_CREDENTIALS environment variable
-        project_id = os.getenv('GOOGLE_PROJECT_ID')
-        location = "global"
+        """Constructor of awstranslate class"""
+        # Authentication via environment variables
+        self._translate_client = boto3.client(service_name='translate', use_ssl=True)
         
-        self._translate_client = translate.TranslationServiceClient()
-        self._parent = f"projects/{project_id}/locations/{location}"
+        # Initializing the list of supported languages (source or target)
+        self._supported_langs = [x["LanguageCode"] for x in self._translate_client.list_languages()["Languages"]]
 
+    def check_langpair(self, sourcelang, targetlang):
+        """Function to verify if a language pair identified by language ids is supported"""
+        supported = False
+        if tag_is_valid(sourcelang) and tag_is_valid(targetlang):
+            if sourcelang in self._supported_langs and targetlang in self._supported_langs:
+                supported = True
+            
+        return supported
+    
     def translate_text(self,sourcelang, targetlang, text):
         """Function to translate text into the target language"""
-        if isinstance(text, six.binary_type):
-            text = text.decode("utf-8")
-
-        response = self._translate_client.translate_text(
-            request={
-                "parent": self._parent,
-                "contents": [text],
-                "mime_type": "text/plain",  # mime types: text/plain, text/html
-                "source_language_code": sourcelang,
-                "target_language_code": targetlang,
-            }
-        )
+        
+        translated_text = ""
+        if self.check_langpair(sourcelang,targetlang):
+            result = self._translate_client.translate_text(Text=text, SourceLanguageCode=sourcelang, TargetLanguageCode=targetlang)
+            translated_text = result.get('TranslatedText')
+        
+        return translated_text
+       
 
-        return response.translations[0].translated_text
```

### Comparing `mteval-0.0.1/mteval/microsoftmt.py` & `mteval-0.0.2/mteval/microsoftmt.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,53 +2,85 @@
 
 # %% auto 0
 __all__ = ['microsofttranslate']
 
 # %% ../nbs/05_microsoftmt.ipynb 8
 import requests, uuid
 import os
+from langcodes import *
 
 class microsofttranslate:
     """
     Class to get translations from the Microsoft Translator API
     """
     def __init__(self):
         """Constructor of microsofttranslate class"""
         self._subscription_key = os.getenv('MS_SUBSCRIPTION_KEY')
         self._region = os.getenv('MS_REGION')
-
-    def translate_text(self,sourcelang, targetlang, text):
-        """Function to translate text into the target language        """
-        # Add your subscription key and endpoint
-        subscription_key = self._subscription_key
-        endpoint = "https://api.cognitive.microsofttranslator.com"
-
-        # Add your location, also known as region. The default is global.
-        # This is required if using a Cognitive Services resource.
-        location = self._region
-
-        path = '/translate'
-        constructed_url = endpoint + path
-
+        self._endpoint = "https://api.cognitive.microsofttranslator.com"
+        self._languages_cache = []
+        
+    def check_langpair(self, sourcelang, targetlang):
+        """Function to verify if a language pair identified by language ids is supported"""
+        path = '/languages'
+        constructed_url = self._endpoint + path
         params = {
             'api-version': '3.0',
-            'from': sourcelang,
-            'to': [targetlang]
+            'scope': 'translation'
         }
-        constructed_url = endpoint + path
+        
+        supported_languages = self._languages_cache
+        # Cached language array empty if not initialized yet
+        if not supported_languages:
+            # Note that we aren't capturing the ETag from response header for the current language list -
+            # we are caching the list after the first call and assume that it doesn't change over the lifetime
+            # of the class,  we don't persist the list and call the API again when the class is re-instantiated
+            request = requests.get(constructed_url, params=params)
+            response = request.json()
+            supported_languages = response["translation"].keys()
+            self._languages_cache = supported_languages
+            
+        language_pair_supported = False
+        if tag_is_valid(sourcelang) and tag_is_valid(targetlang):
+            if sourcelang in supported_languages and targetlang in supported_languages:
+                language_pair_supported = True
+        
+        return language_pair_supported
 
-        headers = {
-            'Ocp-Apim-Subscription-Key': subscription_key,
-            'Ocp-Apim-Subscription-Region': location,
-            'Content-type': 'application/json',
-            'X-ClientTraceId': str(uuid.uuid4())
-        }
-
-        # You can pass more than one object in body.
-        body = [{
-            'text': text
-        }]
-
-        request = requests.post(constructed_url, params=params, headers=headers, json=body)
-        response = request.json()
+    def translate_text(self,sourcelang, targetlang, text):
+        """Function to translate text into the target language"""
+        translated_text = ""
+        if self.check_langpair(sourcelang,targetlang):
+            # Add your subscription key and endpoint
+            subscription_key = self._subscription_key
+            endpoint = self._endpoint
+
+            # Add your location, also known as region. The default is global.
+            # This is required if using a Cognitive Services resource.
+            location = self._region
+
+            path = '/translate'
+
+            params = {
+                'api-version': '3.0',
+                'from': sourcelang,
+                'to': [targetlang]
+            }
+            constructed_url = endpoint + path
+
+            headers = {
+                'Ocp-Apim-Subscription-Key': self._subscription_key,
+                'Ocp-Apim-Subscription-Region': location,
+                'Content-type': 'application/json',
+                'X-ClientTraceId': str(uuid.uuid4())
+            }
+
+            # You can pass more than one object in body.
+            body = [{
+                'text': text
+            }]
+
+            request = requests.post(constructed_url, params=params, headers=headers, json=body)
+            response = request.json()
+            translated_text = response[0]["translations"][0]["text"]
 
-        return response[0]["translations"][0]["text"]
+        return translated_text
```

### Comparing `mteval-0.0.1/mteval/util.py` & `mteval-0.0.2/mteval/util.py`

 * *Files identical despite different names*

### Comparing `mteval-0.0.1/mteval.egg-info/PKG-INFO` & `mteval-0.0.2/mteval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mteval
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to automate machine translation evaluation
-Home-page: https://github.com/polyglottech/mteval
-Author: Polyglot Technology LLC
-Author-email: info@polyglot.technology
+Home-page: https://github.com/achimr/mteval
+Author: Achim Ruopp
+Author-email: achimru@gmail.com
 License: Apache Software License 2.0
 Description: mteval
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         <div>
@@ -48,14 +48,15 @@
             export GOOGLE_PROJECT_ID=''
             export MS_SUBSCRIPTION_KEY=''
             export MS_REGION=''
             export AWS_DEFAULT_REGION=''
             export AWS_ACCESS_KEY_ID=''
             export AWS_SECRET_ACCESS_KEY=''
             export DEEPL_API_KEY=''
+            export MMT_API_KEY=''
         
         #### How to obtain subscription credentials
         
         - [Amazon
           Translate](https://docs.aws.amazon.com/translate/latest/dg/setting-up.html)
         - [DeepL](https://www.deepl.com/docs-api/api-access/authentication/)
         - [Google Translate](https://cloud.google.com/translate/docs/setup)
```

### Comparing `mteval-0.0.1/setup.py` & `mteval-0.0.2/setup.py`

 * *Files identical despite different names*


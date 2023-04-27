# Comparing `tmp/gptprobe-0.1.1.tar.gz` & `tmp/gptprobe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptprobe-0.1.1.tar", last modified: Thu Apr 27 17:14:31 2023, max compression
+gzip compressed data, was "gptprobe-0.1.2.tar", last modified: Thu Apr 27 19:33:21 2023, max compression
```

## Comparing `gptprobe-0.1.1.tar` & `gptprobe-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 17:14:02.000000 gptprobe-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 17:14:30.994270 gptprobe-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 17:14:02.000000 gptprobe-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.986270 gptprobe-0.1.1/gptprobe/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/gptprobe/askfor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/clarification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/clarificationfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfrompoorlyformattedtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromquestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromquestionwithratification.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromtext.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dicttext.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/flaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/flawfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/ratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/ratificationfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/rephrasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/rephrasingfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/textfrompoorlyformatteddicttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/textfromquestion.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/keysinenviron.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/public_setenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/gptprobe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/customtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/enginedefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/equivalence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/parsedictrobustly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.990270 gptprobe-0.1.1/gptprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:14:30.994270 gptprobe-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 17:14:02.000000 gptprobe-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:21.127570 gptprobe-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 19:32:48.000000 gptprobe-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 19:33:21.127570 gptprobe-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 19:32:48.000000 gptprobe-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:21.115570 gptprobe-0.1.2/gptprobe/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:21.123570 gptprobe-0.1.2/gptprobe/askfor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/clarification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/clarificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/dictfrompoorlyformattedtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/dictfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/dictfromquestionwithratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/dictfromtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/dicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/flawfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/ratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/ratificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/rephrasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/rephrasingfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/rephrasingfromquestionanswerandflaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/textfrompoorlyformatteddicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/askfor/textfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/keysinenviron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/public_setenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:21.127570 gptprobe-0.1.2/gptprobe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/utils/customtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/utils/enginedefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/utils/equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-27 19:32:48.000000 gptprobe-0.1.2/gptprobe/utils/parsedictrobustly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:21.119570 gptprobe-0.1.2/gptprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 19:33:21.000000 gptprobe-0.1.2/gptprobe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:21.127570 gptprobe-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 19:32:48.000000 gptprobe-0.1.2/setup.py
```

### Comparing `gptprobe-0.1.1/LICENSE` & `gptprobe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/PKG-INFO` & `gptprobe-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptprobe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Probing chatgpt
 Home-page: https://github.com/gptprobe/gptprobe
 Author: gptprobe
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptprobe-0.1.1/README.md` & `gptprobe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/askfor/clarificationfromquestionandanswer.py` & `gptprobe-0.1.2/gptprobe/askfor/clarificationfromquestionandanswer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 from gptprobe.askfor.dictfromquestion import ask_for_dict_from_question
 from gptprobe.askfor.flawfromquestionandanswer import ask_for_flaw_from_question_and_answer
 from gptprobe.utils.customtypes import DictOrStr
 
 
-def ask_for_clarification_from_question_and_answer(question: str, answer: str, reason=None, key_choice=0,
+def ask_for_clarification_from_question_and_answer(question: str, answer: str, flaw=None, key_choice=0,
                                                    min_clarification_len=15, as_dict=False) -> DictOrStr:
     """
           Ask for a suggested follow-up prompt to encourage a better answer to a previous question
 
     :param question:       Previously asked question
     :param answer:         An answer that wasn't acceptable
-    :param reason:         (Optional) reason given for why it isn't acceptable
+    :param flaw:         (Optional) reason given for why it isn't acceptable
     :param key_choice:
     :param open_kwargs:
     :return:         {"clarification": "The question asked for lowercase and you provided uppercase",
                       "success":1}
     """
     DEFAULT_CLARIFICATION = 'Please try again to answer the previous question precisely as asked, taking ' \
                             'into account formatting instructions, if any'
-    if reason is None:
+    if flaw is None:
         d = ask_for_flaw_from_question_and_answer(question=question, answer=answer)
         if d.get('success') != 1:
             # If we don't know what's wrong, might be best to keep the followup simple
             return {'success' :0 ,'clarification' :DEFAULT_CLARIFICATION}
-        reason = d['reason']
+        flaw = d['flaw']
 
     meta_question = """ I will provide now in xml-delimited style, a question, a previously given but unsatisfactory answer, 
-                        and a reason why it was not a good or well-formatted answer. 
-
+                        and a flaw - which is to say a reason why the answer was not satisfactory
+                        
                         Return a dictionary where the single double-quoted key is "clarification" and the value is 
                     a short clarification or the reason. The clarification should not repeat the question. The clarification
-                    should include the reason, albeit paraphrased as you see fit. 
+                    should include the reason (i.e. flaw), albeit paraphrased as you see fit. 
 
                     Just return this dictionary and nothing else. Ensure the 
                     key is double quoted. Here is the question, answer and reason why it was not satisfactory:
                        <question>""" + question + """</question>
                        <answer>""" + answer + """</answer>
-                       <reason>""" + reason + """</reason>
+                       <flaw>""" + flaw + """</flaw>
                     Let me emphasize that you should reply with a dict only and no other text"""
     d = ask_for_dict_from_question(question=meta_question, key_choice=key_choice, numeric_values_only=False)
     d['success'] = 0
     if (d.get('clarification') is None) or (len(d.get('clarification')) < min_clarification_len):
         d['clarification'] = DEFAULT_CLARIFICATION
     d['success'] = int(d['clarification'] != DEFAULT_CLARIFICATION)
     return d if as_dict else d['clarification']
 
 
 ask_for_clarification = ask_for_clarification_from_question_and_answer
 
 if __name__=='__main__':
-    from gptprobe.askfor.rephrasingfromquestionandanswer import ask_for_rephrasing_from_question_and_answer
+    from gptprobe.askfor.rephrasingfromquestionandanswer import ask_for_rephrasing_from_question_answer_and_flaw
     question = """ Please provide a dictionary where keys are town names and values are prime numbers 
               """
     answer = """ The dictionary is {'Dog':12312,'sydney':17} """
 
     d1 = ask_for_flaw_from_question_and_answer(question=question, answer=answer, as_dict=True)
     print(d1)
 
-    d2 = ask_for_rephrasing_from_question_and_answer(question=question, answer=answer, reason=d1['reason'])
+    d2 = ask_for_rephrasing_from_question_answer_and_flaw(question=question, answer=answer, flaw=d1['reason'])
     print(d2)
 
-    d3 = ask_for_rephrasing_from_question_and_answer(question=question, answer=answer, reason=None)
+    d3 = ask_for_rephrasing_from_question_answer_and_flaw(question=question, answer=answer, flaw=None)
     print(d3)
 
-    d4 = ask_for_clarification_from_question_and_answer(question=question, answer=answer, reason=d1['reason'])
+    d4 = ask_for_clarification_from_question_and_answer(question=question, answer=answer, flaw=d1['reason'])
     print(d4)
 
-    d5 = ask_for_clarification_from_question_and_answer(question=question, answer=answer, reason=None)
+    d5 = ask_for_clarification_from_question_and_answer(question=question, answer=answer, flaw=None)
     print(d5)
 
     # Does it help?
```

### Comparing `gptprobe-0.1.1/gptprobe/askfor/dictfrompoorlyformattedtext.py` & `gptprobe-0.1.2/gptprobe/askfor/dictfrompoorlyformattedtext.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/askfor/dictfromquestion.py` & `gptprobe-0.1.2/gptprobe/askfor/dictfromquestion.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/askfor/flawfromquestionandanswer.py` & `gptprobe-0.1.2/gptprobe/askfor/flawfromquestionandanswer.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/askfor/textfrompoorlyformatteddicttext.py` & `gptprobe-0.1.2/gptprobe/askfor/textfrompoorlyformatteddicttext.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/askfor/textfromquestion.py` & `gptprobe-0.1.2/gptprobe/askfor/textfromquestion.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.1/gptprobe/utils/parsedictrobustly.py` & `gptprobe-0.1.2/gptprobe/utils/parsedictrobustly.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 
 def parse_dict_robustly(text, numeric_values_only=False):
     """
     :param text:
     :param numeric_values_only:  If True,
     :return:
     """
+    try:
+        d = json.loads(text)
+        return d
+    except:
+        pass
+    text = text.replace("\n", " ")
     d1 = parse_dict_disjoint(text, numeric_values_only=numeric_values_only) or {}
     d2 = parse_dict_disjoint(switch_quotes(text), numeric_values_only=numeric_values_only) or {}
     d1.update(d2)
     if numeric_values_only:
         d = dict()
         for k,v in d1.items():
             try:
```

### Comparing `gptprobe-0.1.1/gptprobe.egg-info/PKG-INFO` & `gptprobe-0.1.2/gptprobe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptprobe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Probing chatgpt
 Home-page: https://github.com/gptprobe/gptprobe
 Author: gptprobe
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptprobe-0.1.1/gptprobe.egg-info/SOURCES.txt` & `gptprobe-0.1.2/gptprobe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 gptprobe/askfor/dicttext.py
 gptprobe/askfor/flaw.py
 gptprobe/askfor/flawfromquestionandanswer.py
 gptprobe/askfor/ratification.py
 gptprobe/askfor/ratificationfromquestionandanswer.py
 gptprobe/askfor/rephrasing.py
 gptprobe/askfor/rephrasingfromquestionandanswer.py
+gptprobe/askfor/rephrasingfromquestionanswerandflaw.py
 gptprobe/askfor/text.py
 gptprobe/askfor/textfrompoorlyformatteddicttext.py
 gptprobe/askfor/textfromquestion.py
 gptprobe/utils/__init__.py
 gptprobe/utils/customtypes.py
 gptprobe/utils/enginedefaults.py
 gptprobe/utils/equivalence.py
```

### Comparing `gptprobe-0.1.1/setup.py` & `gptprobe-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="gptprobe",
-    version="0.1.1",
+    version="0.1.2",
     description="Probing chatgpt",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/gptprobe/gptprobe",
     author="gptprobe",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
```


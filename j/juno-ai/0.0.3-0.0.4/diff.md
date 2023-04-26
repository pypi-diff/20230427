# Comparing `tmp/juno-ai-0.0.3.tar.gz` & `tmp/juno-ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juno-ai-0.0.3.tar", last modified: Tue Apr 25 20:36:07 2023, max compression
+gzip compressed data, was "juno-ai-0.0.4.tar", last modified: Wed Apr 26 23:26:41 2023, max compression
```

## Comparing `juno-ai-0.0.3.tar` & `juno-ai-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.794567 juno-ai-0.0.3/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-25 20:36:07.794196 juno-ai-0.0.3/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1940 2023-04-25 20:17:30.000000 juno-ai-0.0.3/README.md
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.791521 juno-ai-0.0.3/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.3/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.3/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    16283 2023-04-25 20:15:36.000000 juno-ai-0.0.3/juno/event_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1387 2023-04-25 20:00:00.000000 juno-ai-0.0.3/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1423 2023-04-25 20:00:24.000000 juno-ai-0.0.3/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.3/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    10061 2023-04-25 20:15:59.000000 juno-ai-0.0.3/juno/prompting_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2381 2023-04-16 21:49:54.000000 juno-ai-0.0.3/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-25 20:16:52.000000 juno-ai-0.0.3/juno/version.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.793786 juno-ai-0.0.3/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      355 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       34 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-25 20:36:07.794635 juno-ai-0.0.3/setup.cfg
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1219 2023-04-25 20:16:45.000000 juno-ai-0.0.3/setup.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-26 23:26:41.063176 juno-ai-0.0.4/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-26 23:26:41.062892 juno-ai-0.0.4/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1940 2023-04-25 20:17:30.000000 juno-ai-0.0.4/README.md
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-26 23:26:41.060823 juno-ai-0.0.4/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.4/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.4/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    16455 2023-04-26 23:26:15.000000 juno-ai-0.0.4/juno/event_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1387 2023-04-25 20:00:00.000000 juno-ai-0.0.4/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1649 2023-04-26 23:26:15.000000 juno-ai-0.0.4/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.4/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    10061 2023-04-26 20:48:37.000000 juno-ai-0.0.4/juno/prompting_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.4/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-26 23:26:15.000000 juno-ai-0.0.4/juno/version.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-26 23:26:41.062483 juno-ai-0.0.4/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-26 23:26:40.000000 juno-ai-0.0.4/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      355 2023-04-26 23:26:41.000000 juno-ai-0.0.4/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-26 23:26:40.000000 juno-ai-0.0.4/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-04-26 23:26:40.000000 juno-ai-0.0.4/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-26 23:26:40.000000 juno-ai-0.0.4/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-26 23:26:41.063271 juno-ai-0.0.4/setup.cfg
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1248 2023-04-26 23:26:15.000000 juno-ai-0.0.4/setup.py
```

### Comparing `juno-ai-0.0.3/PKG-INFO` & `juno-ai-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.3/README.md` & `juno-ai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.3/juno/client_setup.py` & `juno-ai-0.0.4/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.3/juno/event_javascript.py` & `juno-ai-0.0.4/juno/event_javascript.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,15 @@
     }}
     // list the commands juno can run with explanations
     junoInfo.innerHTML = "Juno is your data science co-pilot. Here are some things you can do with Juno:<br><br>" +
         "<b>%juno</b> - prompt juno to write code for you<br>" +
         "<b>✎ edit</b> - prompt juno to edit a cell for you<br>" +
         "<b>🪲 debug</b> - have juno automatically fix your code when it outputs an error<br>" +
         "<div style='display: block;width: 100%;height: 1px;background-color: color(srgb 0.765 0.765 0.765);margin-top: 10px;margin-bottom: 10px;'></div>" +
+        "<b>%disable_data / enable_data</b> - disable/enable shallow, PII-filtered data samples that <i>dramatically</i> improve juno's performance. (ON BY DEFAULT)<br>" +
         "<b><span style=''>%feedback</span></b> - send us some feedback on the alpha 🙏<br>"
     outputArea.element.append(junoInfo);
 }}
 displayJunoInfo({version});
 
 """
```

### Comparing `juno-ai-0.0.3/juno/juno.py` & `juno-ai-0.0.4/juno/juno.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.3/juno/magic.py` & `juno-ai-0.0.4/juno/magic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from IPython.core.magic import (Magics, magics_class, line_magic, cell_magic, needs_local_scope)
 from .juno import chat, debug, edit, feedback
-from .serialize_context import variable_description
+from .serialize_context import variable_description, set_values_enabled
 from .client_setup import setup
 
 @magics_class
 class Assistant(Magics):
 
     @line_magic
     @needs_local_scope
@@ -31,14 +31,22 @@
     def debug(self, line, local_ns=None):
         return debug(line, variable_description(local_ns))
     
     @line_magic
     @needs_local_scope
     def feedback(self, line, local_ns=None):
         return feedback(line)
+    
+    @line_magic
+    def enable_data(self, line, local_ns=None):
+        set_values_enabled(True)
+    
+    @line_magic
+    def disable_data(self, line, local_ns=None):
+        set_values_enabled(False)
 
 _loaded = False
 def load_ipython_extension(ip, **kwargs):
     """Load the extension in IPython."""
     global _loaded
     if not _loaded:
         ip.register_magics(Assistant)
```

### Comparing `juno-ai-0.0.3/juno/output_parser.py` & `juno-ai-0.0.4/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.3/juno/prompting_javascript.py` & `juno-ai-0.0.4/juno/prompting_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.3/juno/serialize_context.py` & `juno-ai-0.0.4/juno/serialize_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,81 @@
 import types
 import traitlets
-
+import validators
 import pandas as pd
+import re
+
+VALUES_ENABLED = True
 
+phone_pattern = r"(\+\d{1,2}\s?)?1?\-?\.?\s?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}"
+physical_address_pattern = r"\b(\d{1,6}\s([a-zA-z\.\s\-]+\s){0,3}([a-zA-z0-9\s]+[a-zA-Z\.])([\,\s]{0,2})?(road|street|avenue|boulevard|lane|drive|way|court|plaza|terrace|colony|close)[\,\s]{1,2}((Apt|Apartment|Floor|Suite|House)[\s\:]{1,2}\d{0,6}[\,\s]{1,2})?(([a-zA-Z]+[\s\-]?){1,4})?([\,\s]{0,2})?([A-Za-z]{2}|[a-zA-Z]+[\s\-])?([\,\s]{0,2}([0-9\-]{1,10})|[A-Z0-9]{3}\s[A-Z0-9]{3})?)\b"
 
+def set_values_enabled(enabled):
+    global VALUES_ENABLED
+    VALUES_ENABLED = enabled
+    
+def filter_dataframe_pii(df, column) -> list:
+    first_three_values = [truncate_value(v) for v in df[column].head(3).tolist()]
+    for i, value in enumerate(first_three_values):
+        if isinstance(value, str):
+            if validators.uuid(value) and ('id' in column or 'user' in column):
+                    first_three_values[i] = '(uuid)'
+            elif validators.email(value):
+                first_three_values[i] = '(email)'
+            elif validators.ip_address.ipv4(value) or validators.ip_address.ipv6(value):
+                first_three_values[i] = '(ip_address)'
+            elif validators.card.card_number(value):
+                first_three_values[i] = '(card_number)'
+            elif re.match(phone_pattern, value):
+                first_three_values[i] = '(phone)'
+            elif re.match(physical_address_pattern, value):
+                first_three_values[i] = '(address)'
+    return first_three_values
+    
 def describe_dataframe(df, max_cols=20) -> str:
     description = []
     for column in df.columns[:max_cols]:
         is_index = column == df.index.name
         dtype = df[column].dtype
-        first_three_values = [truncate_value(v) for v in df[column].head(3).tolist()]
-        description.append(f"{column}, index: {is_index}, dtype: {dtype}. First three values: {first_three_values}")
+        if VALUES_ENABLED:
+            first_three_values = filter_dataframe_pii(df, column)
+            description.append(f"{column}, index: {is_index}, dtype: {dtype}. First three values: {first_three_values}")
+        else:
+            description.append(f"{column}, index: {is_index}, dtype: {dtype}.")
     full_description = "\n".join(description)
     shape_description = f"Shape: {df.shape}"
     return shape_description + '\nColumns:\n' + full_description
 
+def describe_list(lst, max_length=50) -> str:
+    if VALUES_ENABLED:
+        truncated_list = list(lst)[:3]
+        list_repr = ', '.join(truncate_value(x, max_length - 3) for x in truncated_list)
+        return f"[{list_repr}{'...' if len(lst) > 3 else ''}] (length: {len(lst)})"
+    else:
+        return f"(length: {len(lst)})"
+
+def describe_dict(dct, max_length=50) -> str:
+    if VALUES_ENABLED:
+        truncated_dict = {k: v for i, (k, v) in enumerate(dct.items()) if i < 3}
+        dict_repr = ', '.join(f"{k}: {truncate_value(v, max_length - 5)}" for k, v in truncated_dict.items())
+        return f"{{{dict_repr}{'...' if len(dct) > 3 else ''}}} (length: {len(dct)})"
+    else:
+        value_types = set()
+        for value in dct.values():
+            value_types.add(type(value))
+        truncated_value_types = value_types[:3]
+        value_types_str = ', '.join(str(truncate_value(t, max_length - 3)) for t in truncated_value_types)
+        return f"(value-types: {value_types_str}{'...' if len(value_types) > 3 else ''} length: {len(dct)})"
 
 def truncate_value(value, max_length=50):
     value_str = ""
-
     if isinstance(value, (list, tuple, set)):
-        truncated_list = list(value)[:3]
-        list_repr = ', '.join(truncate_value(x, max_length - 3) for x in truncated_list)
-        value_str = f"[{list_repr}{'...' if len(value) > 3 else ''}] (length: {len(value)})"
+        value_str = describe_list(value, max_length)
     elif isinstance(value, dict):
-        truncated_dict = {k: v for i, (k, v) in enumerate(value.items()) if i < 3}
-        dict_repr = ', '.join(f"{k}: {truncate_value(v, max_length - 5)}" for k, v in truncated_dict.items())
-        value_str = f"{{{dict_repr}{'...' if len(value) > 3 else ''}}} (length: {len(value)})"
+        value_str = describe_dict(value, max_length)
     elif isinstance(value, pd.DataFrame):
         value_str = describe_dataframe(value)
     else:
         value_str = str(value)
         if len(value_str) > max_length:
             value_str = value_str[:max_length] + "..."
```

### Comparing `juno-ai-0.0.3/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.4/juno_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.3/setup.py` & `juno-ai-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.3',
+    version='0.0.4',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
     long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Framework :: IPython',
         'Intended Audience :: Developers',
@@ -26,12 +26,13 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
     ],
     install_requires=[
         'IPython',
         'traitlets',
         'notebook>=5.7.6',
+        'validators>=0.20.0'
     ],
     author='juno',
     author_email='hellojunoai@gmail.com',
     url="https://github.com/alexi/juno"
 )
```


# Comparing `tmp/streamlit_session_memo-0.1.3.tar.gz` & `tmp/streamlit_session_memo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_session_memo-0.1.3.tar", max compression
+gzip compressed data, was "streamlit_session_memo-0.2.0.tar", max compression
```

## Comparing `streamlit_session_memo-0.1.3.tar` & `streamlit_session_memo-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-04-26 20:05:14.690160 streamlit_session_memo-0.1.3/LICENSE
--rw-r--r--   0        0        0       24 2023-04-26 20:05:14.690160 streamlit_session_memo-0.1.3/README.md
--rw-r--r--   0        0        0      678 2023-04-26 20:05:14.690160 streamlit_session_memo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-26 20:05:14.690160 streamlit_session_memo-0.1.3/streamlit_session_memo/__init__.py
--rw-r--r--   0        0        0      799 2023-04-26 20:05:14.690160 streamlit_session_memo-0.1.3/streamlit_session_memo/session_memo.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 streamlit_session_memo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/README.md
+-rw-r--r--   0        0        0      678 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/streamlit_session_memo/__init__.py
+-rw-r--r--   0        0        0      802 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/streamlit_session_memo/session_memo.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 streamlit_session_memo-0.2.0/PKG-INFO
```

### Comparing `streamlit_session_memo-0.1.3/LICENSE` & `streamlit_session_memo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_session_memo-0.1.3/pyproject.toml` & `streamlit_session_memo-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-session-memo"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "streamlit_session_memo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `streamlit_session_memo-0.1.3/streamlit_session_memo/session_memo.py` & `streamlit_session_memo-0.2.0/streamlit_session_memo/session_memo.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def calc_cache_key(args, kwargs) -> Hashable:
     hashable_args = [a if isinstance(a, Hashable) else id(a) for a in args]
     hashable_kwargs = {k: v if isinstance(v, Hashable) else id(v) for k, v in kwargs.items()}
     return CACHE_KEY_PREFIX, tuple(hashable_args), tuple(sorted(hashable_kwargs.items()))
 
 
-def session_memo(func):
+def st_session_memo(func):
     def inner(*args, **kwargs):
         cache_key = calc_cache_key(args, kwargs)
 
         if cache_key in st.session_state:
             return st.session_state[cache_key]
 
         value = func(*args, **kwargs)
```

### Comparing `streamlit_session_memo-0.1.3/PKG-INFO` & `streamlit_session_memo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-session-memo
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Yuichiro Tachibana (Tsuchiya)
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


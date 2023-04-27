# Comparing `tmp/streamlit_session_memo-0.2.0.tar.gz` & `tmp/streamlit_session_memo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_session_memo-0.2.0.tar", max compression
+gzip compressed data, was "streamlit_session_memo-0.2.1.tar", max compression
```

## Comparing `streamlit_session_memo-0.2.0.tar` & `streamlit_session_memo-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/LICENSE
--rw-r--r--   0        0        0       24 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/README.md
--rw-r--r--   0        0        0      678 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/streamlit_session_memo/__init__.py
--rw-r--r--   0        0        0      802 2023-04-27 09:33:31.402037 streamlit_session_memo-0.2.0/streamlit_session_memo/session_memo.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 streamlit_session_memo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-27 09:57:46.481945 streamlit_session_memo-0.2.1/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-27 09:57:46.481945 streamlit_session_memo-0.2.1/README.md
+-rw-r--r--   0        0        0      678 2023-04-27 09:57:46.485945 streamlit_session_memo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-04-27 09:57:46.485945 streamlit_session_memo-0.2.1/streamlit_session_memo/__init__.py
+-rw-r--r--   0        0        0      802 2023-04-27 09:57:46.485945 streamlit_session_memo-0.2.1/streamlit_session_memo/session_memo.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 streamlit_session_memo-0.2.1/PKG-INFO
```

### Comparing `streamlit_session_memo-0.2.0/LICENSE` & `streamlit_session_memo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_session_memo-0.2.0/pyproject.toml` & `streamlit_session_memo-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-session-memo"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "streamlit_session_memo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `streamlit_session_memo-0.2.0/streamlit_session_memo/session_memo.py` & `streamlit_session_memo-0.2.1/streamlit_session_memo/session_memo.py`

 * *Files identical despite different names*

### Comparing `streamlit_session_memo-0.2.0/PKG-INFO` & `streamlit_session_memo-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-session-memo
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Yuichiro Tachibana (Tsuchiya)
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


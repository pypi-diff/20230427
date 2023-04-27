# Comparing `tmp/nldb-0.3.5.tar.gz` & `tmp/nldb-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nldb-0.3.5.tar", last modified: Thu Apr 27 10:01:43 2023, max compression
+gzip compressed data, was "nldb-0.3.7.tar", last modified: Thu Apr 27 10:43:10 2023, max compression
```

## Comparing `nldb-0.3.5.tar` & `nldb-0.3.7.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1824 2023-04-27 10:00:54.088720 nldb-0.3.5/.gitignore
--rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.5/LICENSE
--rw-r--r--   0        0        0     1955 2023-04-26 07:38:48.172206 nldb-0.3.5/README.md
--rw-r--r--   0        0        0       51 2023-04-27 09:59:52.998909 nldb-0.3.5/nldb/__init__.py
--rw-r--r--   0        0        0     1958 2023-04-26 14:39:27.585694 nldb-0.3.5/nldb/api.py
--rw-r--r--   0        0        0     2588 2023-04-26 12:11:29.217383 nldb-0.3.5/nldb/cli.py
--rw-r--r--   0        0        0     7221 2023-04-27 09:16:46.356273 nldb-0.3.5/nldb/core.py
--rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.5/nldb/templates/Dockerfile
--rw-r--r--   0        0        0     4703 2023-04-27 09:19:09.574559 nldb-0.3.5/nldb/templates/index.html
--rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.5/nldb/templates/prompt.txt
--rw-r--r--   0        0        0      936 2023-04-27 09:08:20.536154 nldb-0.3.5/notes.md
--rw-r--r--   0        0        0      539 2023-04-26 16:43:16.557273 nldb-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 nldb-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1824 2023-04-27 10:00:54.088720 nldb-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1955 2023-04-26 07:38:48.172206 nldb-0.3.7/README.md
+-rw-r--r--   0        0        0       51 2023-04-27 10:42:46.187726 nldb-0.3.7/nldb/__init__.py
+-rw-r--r--   0        0        0     1958 2023-04-26 14:39:27.585694 nldb-0.3.7/nldb/api.py
+-rw-r--r--   0        0        0     2588 2023-04-26 12:11:29.217383 nldb-0.3.7/nldb/cli.py
+-rw-r--r--   0        0        0     7292 2023-04-27 10:39:07.196449 nldb-0.3.7/nldb/core.py
+-rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.7/nldb/templates/Dockerfile
+-rw-r--r--   0        0        0     4703 2023-04-27 09:19:09.574559 nldb-0.3.7/nldb/templates/index.html
+-rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.7/nldb/templates/prompt.txt
+-rw-r--r--   0        0        0      557 2023-04-27 10:40:00.761170 nldb-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 nldb-0.3.7/PKG-INFO
```

### Comparing `nldb-0.3.5/.gitignore` & `nldb-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/LICENSE` & `nldb-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/README.md` & `nldb-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/nldb/api.py` & `nldb-0.3.7/nldb/api.py`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/nldb/cli.py` & `nldb-0.3.7/nldb/cli.py`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/nldb/core.py` & `nldb-0.3.7/nldb/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,16 @@
             {results}
 
             write some Python code with matplotlib.pyplot to create a chart 
             which illustrates this data.
 
             Don't use Pandas or pd.DataFrame.
 
+            Use plt.tight_layout() to make sure the chart is legible.
+
             Don't use plt.show(), use plt.save('image.png'). After saving the 
             chart, clear the figure by running 
             plt.clf()
             plt.cla()
             plt.close()
             """
         prompt_messages = [
```

### Comparing `nldb-0.3.5/nldb/templates/index.html` & `nldb-0.3.7/nldb/templates/index.html`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/nldb/templates/prompt.txt` & `nldb-0.3.7/nldb/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nldb-0.3.5/pyproject.toml` & `nldb-0.3.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 dependencies = [
     "openai",
     "fastapi",
     "uvicorn[standard]",
     "tabulate",
     "typer",
     "duckdb",
+    "matplotlib",
 ]
 
 [project.urls]
 Home = "https://github.com/tomdyson/nldb"
 
 [project.scripts]
 nldb = "nldb.cli:cli_wrapper"
```

### Comparing `nldb-0.3.5/PKG-INFO` & `nldb-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: nldb
-Version: 0.3.5
+Version: 0.3.7
 Summary: talk to your database
 Author-email: Tom Dyson <tom@torchbox.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: openai
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: tabulate
 Requires-Dist: typer
 Requires-Dist: duckdb
+Requires-Dist: matplotlib
 Project-URL: Home, https://github.com/tomdyson/nldb
 
 # nldb
 
 Natural Language Databasing. Talk to your data in English, via CLI, API or a simple web interface.
 
 ## Installation
```


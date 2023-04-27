# Comparing `tmp/nldb-0.3.4.tar.gz` & `tmp/nldb-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nldb-0.3.4.tar", last modified: Tue Apr 25 14:32:14 2023, max compression
+gzip compressed data, was "nldb-0.3.5.tar", last modified: Thu Apr 27 10:01:43 2023, max compression
```

## Comparing `nldb-0.3.4.tar` & `nldb-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1815 2023-04-25 12:52:44.252106 nldb-0.3.4/.gitignore
--rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.4/LICENSE
--rw-r--r--   0        0        0      118 2023-03-31 22:32:58.589210 nldb-0.3.4/README.md
--rw-r--r--   0        0        0       51 2023-04-25 14:31:44.497372 nldb-0.3.4/nldb/__init__.py
--rw-r--r--   0        0        0     1311 2023-04-18 16:47:22.620794 nldb-0.3.4/nldb/api.py
--rw-r--r--   0        0        0     2358 2023-04-25 14:31:34.655466 nldb-0.3.4/nldb/cli.py
--rw-r--r--   0        0        0     4595 2023-04-25 13:26:01.281585 nldb-0.3.4/nldb/core.py
--rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.4/nldb/templates/Dockerfile
--rw-r--r--   0        0        0     3803 2023-04-25 13:46:25.520393 nldb-0.3.4/nldb/templates/index.html
--rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.4/nldb/templates/prompt.txt
--rw-r--r--   0        0        0      435 2023-04-25 12:55:23.849992 nldb-0.3.4/notes.md
--rw-r--r--   0        0        0      539 2023-04-25 13:00:22.530315 nldb-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 nldb-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1824 2023-04-27 10:00:54.088720 nldb-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1955 2023-04-26 07:38:48.172206 nldb-0.3.5/README.md
+-rw-r--r--   0        0        0       51 2023-04-27 09:59:52.998909 nldb-0.3.5/nldb/__init__.py
+-rw-r--r--   0        0        0     1958 2023-04-26 14:39:27.585694 nldb-0.3.5/nldb/api.py
+-rw-r--r--   0        0        0     2588 2023-04-26 12:11:29.217383 nldb-0.3.5/nldb/cli.py
+-rw-r--r--   0        0        0     7221 2023-04-27 09:16:46.356273 nldb-0.3.5/nldb/core.py
+-rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.5/nldb/templates/Dockerfile
+-rw-r--r--   0        0        0     4703 2023-04-27 09:19:09.574559 nldb-0.3.5/nldb/templates/index.html
+-rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.5/nldb/templates/prompt.txt
+-rw-r--r--   0        0        0      936 2023-04-27 09:08:20.536154 nldb-0.3.5/notes.md
+-rw-r--r--   0        0        0      539 2023-04-26 16:43:16.557273 nldb-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 nldb-0.3.5/PKG-INFO
```

### Comparing `nldb-0.3.4/.gitignore` & `nldb-0.3.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -125,8 +125,9 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 demo*/
-.vscode/
+.vscode/
+notes.md
```

### Comparing `nldb-0.3.4/LICENSE` & `nldb-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nldb-0.3.4/nldb/api.py` & `nldb-0.3.5/nldb/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import Union
 
 import uvicorn
 from fastapi import FastAPI
 from fastapi.responses import FileResponse
+from pydantic import BaseModel
 
 from nldb.core import NLDB
 
 UVICORN_HOST = os.environ.get("UVICORN_HOST", "0.0.0.0")
 UVICORN_PORT = int(os.environ.get("UVICORN_PORT", 8080))
 
 app = FastAPI()
@@ -35,15 +36,38 @@
             "timings": nldb.timings,  # in seconds
             "tokens": nldb.tokens,
             "cost": nldb.tokens / 1000 * 0.002,  # gpt-3.5 is $0.002 per 1000 tokens,
         }
     }
 
 
+class ChartRequest(BaseModel):
+    question: str
+    results: str
+
+
+@app.post("/api/chart")
+async def chart(request_data: ChartRequest):
+    """Process a question and results,
+    executes returned code and returns filename of chart"""
+    nldb = NLDB()
+    filename, code = nldb.results_to_chart(request_data.question, request_data.results)
+    print(filename)
+    print(code)
+    exec(code)
+    return {"response": {"chart": filename}}
+
+
+@app.get("/charts/{filename}")
+async def serve_chart(filename: str):
+    """Serve charts from ./charts"""
+    return FileResponse(f"charts/{filename}")
+
+
 @app.get("/")
 async def serve_index():
     """Serve index.html"""
     return FileResponse("index.html")
 
 
 def serve():
-    uvicorn.run(app, host=UVICORN_HOST, port=UVICORN_PORT)
+    uvicorn.run("nldb.api:app", host=UVICORN_HOST, port=UVICORN_PORT, workers=2)
```

### Comparing `nldb-0.3.4/nldb/cli.py` & `nldb-0.3.5/nldb/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,19 @@
     for file in ["Dockerfile", "index.html", "prompt.txt"]:
         dest = os.path.join(os.getcwd(), file)
         if os.path.exists(dest):
             typer.echo(f"{file} already exists here")
         else:
             shutil.copyfile(os.path.join(package_dir, "templates", file), dest)
             typer.echo(f"Created {file} at {dest}")
+    # make a 'charts' directory if it doesn't exist
+    charts_dir = os.path.join(os.getcwd(), "charts")
+    if not os.path.exists(charts_dir):
+        os.mkdir(charts_dir)
+        typer.echo(f"Created directory at {charts_dir}")
 
 
 def deploy_instructions():
     typer.echo("Printing deployment instructions")
     openai_api_key = os.environ.get("OPENAI_API_KEY", "your OpenAI API key")
     instructions = inspect.cleandoc(
         f"""
```

### Comparing `nldb-0.3.4/nldb/templates/prompt.txt` & `nldb-0.3.5/nldb/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nldb-0.3.4/pyproject.toml` & `nldb-0.3.5/pyproject.toml`

 * *Files identical despite different names*


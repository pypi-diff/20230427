# Comparing `tmp/gpt-review-0.0.1rc80.post1.tar.gz` & `tmp/gpt-review-0.0.1rc82.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.0.1rc80.post1.tar", last modified: Wed Apr 26 19:27:14 2023, max compression
+gzip compressed data, was "gpt-review-0.0.1rc82.post1.tar", last modified: Thu Apr 27 02:47:33 2023, max compression
```

## Comparing `gpt-review-0.0.1rc80.post1.tar` & `gpt-review-0.0.1rc82.post1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      333 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1333 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      747 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      866 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.pypirc
--rw-r--r--   0        0        0      816 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/LICENSE
--rw-r--r--   0        0        0     1283 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/README.md
--rw-r--r--   0        0        0     5116 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/action.yml
--rw-r--r--   0        0        0     6847 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/review.py
--rw-r--r--   0        0        0      363 2023-04-26 19:27:14.142851 gpt-review-0.0.1rc80.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0     5796 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      413 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      792 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/tests/conftest.py
--rw-r--r--   0        0        0     1193 2023-04-26 19:27:04.006752 gpt-review-0.0.1rc80.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 gpt-review-0.0.1rc80.post1/PKG-INFO
+-rw-r--r--   0        0        0      333 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1333 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      747 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      866 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.pypirc
+-rw-r--r--   0        0        0      816 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/LICENSE
+-rw-r--r--   0        0        0      733 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/README.md
+-rw-r--r--   0        0        0     5116 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/action.yml
+-rw-r--r--   0        0        0     6847 2023-04-27 02:47:26.905226 gpt-review-0.0.1rc82.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/review.py
+-rw-r--r--   0        0        0      363 2023-04-27 02:47:33.221594 gpt-review-0.0.1rc82.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0     5796 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      413 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      792 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/tests/conftest.py
+-rw-r--r--   0        0        0     1193 2023-04-27 02:47:26.909226 gpt-review-0.0.1rc82.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 gpt-review-0.0.1rc82.post1/PKG-INFO
```

### Comparing `gpt-review-0.0.1rc80.post1/.devcontainer/devcontainer.json` & `gpt-review-0.0.1rc82.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/.github/workflows/python.yml` & `gpt-review-0.0.1rc82.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/.github/workflows/test-action.yml` & `gpt-review-0.0.1rc82.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/.gitignore` & `gpt-review-0.0.1rc82.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/.vscode/settings.json` & `gpt-review-0.0.1rc82.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/LICENSE` & `gpt-review-0.0.1rc82.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/action.yml` & `gpt-review-0.0.1rc82.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/pyproject.toml` & `gpt-review-0.0.1rc82.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/review.py` & `gpt-review-0.0.1rc82.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/src/gpt_review/_ask.py` & `gpt-review-0.0.1rc82.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.0.1rc82.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/tests/conftest.py` & `gpt-review-0.0.1rc82.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/tests/test_gpt_cli.py` & `gpt-review-0.0.1rc82.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc80.post1/PKG-INFO` & `gpt-review-0.0.1rc82.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.0.1rc80.post1
+Version: 0.0.1rc82.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,24 +40,17 @@
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://github.com/dciborow/action-gpt/tree/main#readme
 Project-URL: Source, https://github.com/dciborow/action-gpt
 Project-URL: Tracker, https://github.com/dciborow/action-gpt/issues
 Provides-Extra: test
 
-# GPTReview Workflow 🤖🔍
+# gpt-review
 
-Get OpenAI GPT models to suggest changes on your pull request in the comments.
-
-## How to integrate into your repo:
-
-1. Copy the workflow from this repo's .github/workflows/test-action.yml into your project in the same location and modify it to suit your needs, if you'd like. Update the action pointer from "./" to "microsoft/easy-gpt@<version>"
-2. Get an [OpenAI API Key here](https://beta.openai.com/account/api-keys)
-3. Get an [OpenAI Org ID here](https://beta.openai.com/account/org-settings)
-4. Create two secrets in your project's settings called OPENAI_API_KEY for your OpenAI API Key and OPENAI_ORG_KEY for your OpenAI Organization ID..
+A Python based CLI and GitHub Action to use Open AI or Azure Open AI models to review contents of pull requests.
 
 ## How to use CLI:
 
 Install the package via `pip` and set the environment variables for your OpenAI API Key and Organization ID.
 To use Azure OpenAI, set the environment variable `AZURE_OPENAI_API_URL` and `AZURE_OPENAI_API_URL_KEY` to the URL and key for your Azure OpenAI API.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


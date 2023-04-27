# Comparing `tmp/docstring_auditor-0.1.6.tar.gz` & `tmp/docstring_auditor-0.1.7.tar.gz`

## Comparing `docstring_auditor-0.1.6.tar` & `docstring_auditor-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/Dockerfile
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/action.yml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/.github/workflows/image-latest.yml
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/.github/workflows/image-release.yml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/docstring_auditor/__init__.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/docstring_auditor/main.py
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/tests/test_critique.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/tests/test_extractor.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/tests/test_reporter.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/LICENSE
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/README.md
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 docstring_auditor-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/Dockerfile
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/action.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/image-latest.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/image-release.yml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/docstring_auditor/__init__.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/docstring_auditor/main.py
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_critique.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_extractor.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_reporter.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/PKG-INFO
```

### Comparing `docstring_auditor-0.1.6/Dockerfile` & `docstring_auditor-0.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/action.yml` & `docstring_auditor-0.1.7/action.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 name: 'Docstring Auditor'
 author: 'Rob Luke'
 description: 'Use AI to review your code documentation.'
 runs:
   using: 'docker'
-  image: 'docker://ghcr.io/rob-luke/docstring-auditor:latest'
+  image: 'docker://ghcr.io/agencyenterprise/docstring-auditor:latest'
 branding:
   icon: 'check-square'
   color: 'white'
 
 inputs:
   analysis-path:
     description: 'Path to the file or directory you wish to analyse'
```

### Comparing `docstring_auditor-0.1.6/.github/workflows/image-latest.yml` & `docstring_auditor-0.1.7/.github/workflows/image-release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Docker Image Release
 
 on:
   push:
-    branches:
-      - 'main'
+    tags:
+      - '*'
 
 jobs:
   docker:
     runs-on: ubuntu-latest
     steps:
 
       - uses: actions/checkout@v2
@@ -17,15 +17,18 @@
       - name: Login to GitHub Container Registry
         uses: docker/login-action@v1
         with:
           registry: ghcr.io
           username: ${{ github.repository_owner }}
           password: ${{ secrets.GHCR_TOKEN }}
 
+      - name: Create environmental variable for release version
+        run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
+
       - name: Build docker image
         run: DOCKER_BUILDKIT=1 docker build --progress=plain -t ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} .
 
       - name: Tag image
-        run: docker tag ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} ghcr.io/rob-luke/docstring-auditor:latest
+        run: docker tag ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} ghcr.io/agencyenterprise/docstring-auditor:${{ env.RELEASE_VERSION }}
 
       - name: Push image to github
-        run: docker push ghcr.io/rob-luke/docstring-auditor:latest
+        run: docker push ghcr.io/agencyenterprise/docstring-auditor:${{ env.RELEASE_VERSION }}
```

### Comparing `docstring_auditor-0.1.6/.github/workflows/image-release.yml` & `docstring_auditor-0.1.7/.github/workflows/image-latest.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Docker Image Release
 
 on:
   push:
-    tags:
-      - '*'
+    branches:
+      - 'main'
 
 jobs:
   docker:
     runs-on: ubuntu-latest
     steps:
 
       - uses: actions/checkout@v2
@@ -17,18 +17,15 @@
       - name: Login to GitHub Container Registry
         uses: docker/login-action@v1
         with:
           registry: ghcr.io
           username: ${{ github.repository_owner }}
           password: ${{ secrets.GHCR_TOKEN }}
 
-      - name: Create environmental variable for release version
-        run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
-
       - name: Build docker image
         run: DOCKER_BUILDKIT=1 docker build --progress=plain -t ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} .
 
       - name: Tag image
-        run: docker tag ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} ghcr.io/rob-luke/docstring-auditor:${{ env.RELEASE_VERSION }}
+        run: docker tag ghcr.io/${GITHUB_REPOSITORY}/${GITHUB_REF##*/} ghcr.io/agencyenterprise/docstring-auditor:latest
 
       - name: Push image to github
-        run: docker push ghcr.io/rob-luke/docstring-auditor:${{ env.RELEASE_VERSION }}
+        run: docker push ghcr.io/agencyenterprise/docstring-auditor:latest
```

### Comparing `docstring_auditor-0.1.6/.github/workflows/test.yml` & `docstring_auditor-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/docstring_auditor/main.py` & `docstring_auditor-0.1.7/docstring_auditor/main.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/tests/test_critique.py` & `docstring_auditor-0.1.7/tests/test_critique.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/tests/test_extractor.py` & `docstring_auditor-0.1.7/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/tests/test_reporter.py` & `docstring_auditor-0.1.7/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/.gitignore` & `docstring_auditor-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/LICENSE` & `docstring_auditor-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.6/README.md` & `docstring_auditor-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Docstring Auditor
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
-[![tests](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml)
-[![Release](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml)
+[![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
+[![Release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
 
-Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation. Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings, ensuring they align with your code's true purpose. Accessible to both experts and novices, Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings. Say hello to better code documentation!
+Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
+Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
+ensuring they align with your code's true purpose. Accessible to both experts and novices,
+Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
+Say hello to better code documentation!
 
 ## Motivation
 
 Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on. Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
 
 Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language. By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation. The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent. Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
 
@@ -30,34 +34,22 @@
 1. Install [Docker](https://docs.docker.com/get-docker/)
 2. Run the following command:
 
 ```bash
 docker run -it --rm -e OPENAI_API_KEY=sk-XXXX -v /Path/to/code:/repo docstring-auditor
 ```
 
-
-### Local Installation
-You can also run Docstring Auditor locally by following these steps:
-
-1. Install [Python 3.6+](https://www.python.org/downloads/)
-2. Install [Git](https://git-scm.com/downloads)
-3. Clone the repository: `git clone git@github.com:rob-luke/docstring-auditor.git`
-4. Setup hatch: `pip install hatch`
-5. Run the package `hatch run docstring-auditor /path/to/your/python_file.py`
-
-
 ## Usage
-Using Docstring Auditor is as easy as running the following command:
+If you use the docker command above, Docstring Auditor will analyse all python files in your directory.
+If you wish for it to analyse a single file, pass in the file name with the repo prefix.
+For example, to analyse the file in  `src/module/file.py`...
 
 ```bash
-docstring-auditor path/to/your/python_file.py
+docker run -it --rm -e OPENAI_API_KEY=sk-XXXX -v /Path/to/code:/repo docstring-auditor /repo/src/module/file.py
 ```
-
-You can pass in a single file to analyse, or you can pass in a directory and it will analyse every file.
-
 The tool will then analyze the functions' docstrings in the specified file and display the critiques and suggestions for improvement.
 
 ## Example
 Let's say you have a Python file called example.py with the following content:
 
 ```python
 
@@ -121,10 +113,30 @@
 -------
 int or float
     The result of the addition or subtraction operation.
 """
 
 ```
 
+## Limitations
+
+1. There is currently no checking for malformed json from GPT4. Occasionaly GPT4 will return a bad json and the program will crash.
+2. There is no rate limiting on the GPT4 calls.
+3. Only GPT4 is included. It would be trivial to make this a variable. Pull requests are welcome.
+
+
 ## Contributing
 We welcome contributions to Docstring Auditor! If you'd like to contribute, please fork the repository and submit a pull request with your changes. We also appreciate bug reports and feature requests submitted through the GitHub issues page.
 
+
+## Advanced Usage
+
+### Local Installation
+You can also run Docstring Auditor locally by following these steps:
+
+1. Install [Python 3.6+](https://www.python.org/downloads/)
+2. Install [Git](https://git-scm.com/downloads)
+3. Clone the repository: `git clone git@github.com:agencyenterprise/docstring-auditor.git`
+4. Setup hatch: `pip install hatch`
+5. Run the package `hatch run docstring-auditor /path/to/your/python_file.py`
+
+
```

### Comparing `docstring_auditor-0.1.6/pyproject.toml` & `docstring_auditor-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "docstring-auditor"
-version = "0.1.6"
-authors = [{name = "Rob Luke", email = "code@robertluke.net"}]
+version = "0.1.7"
+authors = [{name = "Rob Luke", email = "rob.luke@ae.studio"}]
 description = "A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement"
 readme = "README.md"
 keywords = ["docstring", "auditor", "openai", "gpt"]
-url = "https://github.com/rob-luke/docstring-auditor"
+url = "https://github.com/agencyenterprise/docstring-auditor"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
```

### Comparing `docstring_auditor-0.1.6/PKG-INFO` & `docstring_auditor-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docstring-auditor
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement
-Author-email: Rob Luke <code@robertluke.net>
+Author-email: Rob Luke <rob.luke@ae.studio>
 License-File: LICENSE
 Keywords: auditor,docstring,gpt,openai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Docstring Auditor
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
-[![tests](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/test.yml)
-[![Release](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/rob-luke/docstring-auditor/actions/workflows/release.yml)
+[![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
+[![Release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
 
-Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation. Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings, ensuring they align with your code's true purpose. Accessible to both experts and novices, Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings. Say hello to better code documentation!
+Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
+Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
+ensuring they align with your code's true purpose. Accessible to both experts and novices,
+Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
+Say hello to better code documentation!
 
 ## Motivation
 
 Recognizing the need for a reliable tool to address the challenge of keeping code documentation in sync with evolving codebases, we developed Docstring Auditor to tackle this issue head-on. Our motivation was to create an accessible, user-friendly solution that empowers developers to maintain clear and up-to-date documentation with ease, enhancing their workflow and reducing misunderstandings.
 
 Docstring Auditor leverages the advanced capabilities of GPT-4, a powerful language model designed to deeply understand both code and natural language. By incorporating GPT-4 into our tool, Docstring Auditor examines the docstrings in your Python code, identifying discrepancies between the documentation and the actual code implementation. The analysis covers errors, warnings, and potential improvements, providing valuable critiques and suggestions to help you keep your documentation accurate and coherent. Docstring Auditor not only ensures that technical details, such as variables and types, are consistent, but it also verifies that the docstrings' meanings are in harmony with the code's functionality.
 
@@ -50,34 +54,22 @@
 1. Install [Docker](https://docs.docker.com/get-docker/)
 2. Run the following command:
 
 ```bash
 docker run -it --rm -e OPENAI_API_KEY=sk-XXXX -v /Path/to/code:/repo docstring-auditor
 ```
 
-
-### Local Installation
-You can also run Docstring Auditor locally by following these steps:
-
-1. Install [Python 3.6+](https://www.python.org/downloads/)
-2. Install [Git](https://git-scm.com/downloads)
-3. Clone the repository: `git clone git@github.com:rob-luke/docstring-auditor.git`
-4. Setup hatch: `pip install hatch`
-5. Run the package `hatch run docstring-auditor /path/to/your/python_file.py`
-
-
 ## Usage
-Using Docstring Auditor is as easy as running the following command:
+If you use the docker command above, Docstring Auditor will analyse all python files in your directory.
+If you wish for it to analyse a single file, pass in the file name with the repo prefix.
+For example, to analyse the file in  `src/module/file.py`...
 
 ```bash
-docstring-auditor path/to/your/python_file.py
+docker run -it --rm -e OPENAI_API_KEY=sk-XXXX -v /Path/to/code:/repo docstring-auditor /repo/src/module/file.py
 ```
-
-You can pass in a single file to analyse, or you can pass in a directory and it will analyse every file.
-
 The tool will then analyze the functions' docstrings in the specified file and display the critiques and suggestions for improvement.
 
 ## Example
 Let's say you have a Python file called example.py with the following content:
 
 ```python
 
@@ -141,10 +133,30 @@
 -------
 int or float
     The result of the addition or subtraction operation.
 """
 
 ```
 
+## Limitations
+
+1. There is currently no checking for malformed json from GPT4. Occasionaly GPT4 will return a bad json and the program will crash.
+2. There is no rate limiting on the GPT4 calls.
+3. Only GPT4 is included. It would be trivial to make this a variable. Pull requests are welcome.
+
+
 ## Contributing
 We welcome contributions to Docstring Auditor! If you'd like to contribute, please fork the repository and submit a pull request with your changes. We also appreciate bug reports and feature requests submitted through the GitHub issues page.
 
+
+## Advanced Usage
+
+### Local Installation
+You can also run Docstring Auditor locally by following these steps:
+
+1. Install [Python 3.6+](https://www.python.org/downloads/)
+2. Install [Git](https://git-scm.com/downloads)
+3. Clone the repository: `git clone git@github.com:agencyenterprise/docstring-auditor.git`
+4. Setup hatch: `pip install hatch`
+5. Run the package `hatch run docstring-auditor /path/to/your/python_file.py`
+
+
```


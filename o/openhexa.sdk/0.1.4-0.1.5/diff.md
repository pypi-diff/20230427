# Comparing `tmp/openhexa.sdk-0.1.4.tar.gz` & `tmp/openhexa.sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.sdk-0.1.4.tar", last modified: Wed Apr 26 12:52:01 2023, max compression
+gzip compressed data, was "openhexa.sdk-0.1.5.tar", last modified: Wed Apr 26 14:51:01 2023, max compression
```

## Comparing `openhexa.sdk-0.1.4.tar` & `openhexa.sdk-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.955214 openhexa.sdk-0.1.4/openhexa/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/cli/skeleton/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/cli/skeleton/workspace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.959214 openhexa.sdk-0.1.4/openhexa/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/openhexa/sdk/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.955214 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 12:52:01.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:51:51.000000 openhexa.sdk-0.1.4/openhexa.sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-26 12:52:01.967214 openhexa.sdk-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:52:01.963214 openhexa.sdk-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 12:51:45.000000 openhexa.sdk-0.1.4/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.204978 openhexa.sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-26 14:51:01.204978 openhexa.sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.196978 openhexa.sdk-0.1.5/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.200978 openhexa.sdk-0.1.5/openhexa/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.200978 openhexa.sdk-0.1.5/openhexa/cli/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/skeleton/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/skeleton/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/cli/skeleton/workspace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.200978 openhexa.sdk-0.1.5/openhexa/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.204978 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.204978 openhexa.sdk-0.1.5/openhexa/sdk/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/workspaces/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/openhexa/sdk/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.196978 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 14:51:01.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:50:47.000000 openhexa.sdk-0.1.5/openhexa.sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-26 14:51:01.208978 openhexa.sdk-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:51:01.204978 openhexa.sdk-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 14:50:39.000000 openhexa.sdk-0.1.5/tests/test_pipeline.py
```

### Comparing `openhexa.sdk-0.1.4/LICENCE` & `openhexa.sdk-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/PKG-INFO` & `openhexa.sdk-0.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
@@ -17,68 +17,84 @@
 
 # OpenHexa Python SDK
 
 The OpenHexa Python SDK is a tool that helps you write code for the OpenHexa platform.
 
 It is particularly useful to write OpenHexa data pipelines, but can also be used in the OpenHexa notebooks environment.
 
-## Writing data pipelines
+## Quickstart
 
-TBC
-
-## Using the SDK in the notebooks environment
+### Writing and deploying pipelines
 
-TBC
+Here's a super minimal example to get you started. First, create a new directory and a virtual environment:
 
-## Running the examples
+```shell
+mkdir openhexa-pipelines-quickstart
+cd openhexa-pipelines-quickstart
+virtualenv venv
+source venv/bin/activate
+```
 
-Clone the repo and install the dependencies, including the ones required to run the examples:
+You can then install the OpenHexa SDK:
 
 ```shell
-git checkout https://github.com/BLSQ/openhexa-sdk-python.git
-pip install ".[examples]"
+pip install openhexa.sdk
 ```
 
-Run a pipeline:
+Now that the SDK is installed withing your virtual environmentYou can now use the `openhexa` CLI utility to create 
+a new pipeline:
 
 ```shell
-cd examples/pipelines/logistic_stats
-python pipeline.py -c '{"deg":"qfxEYY9xAl6","periods":["2022Q1","2022Q2"]}'
+openhexa pipelines init "My awesome pipeline"
 ```
 
-Or using a config file:
+Great! As you can see in the console output, the OpenHexa CLI has created a new directory, which contains the basic 
+structure required for an OpenHexa pipeline. You can now `cd` in the new pipeline directory and run the pipeline:
 
 ```shell
-cd examples/pipelines/logistic_stats
-python pipeline.py -f example_conf.json
+cd my_awesome_pipeline
+python pipeline.py
 ```
 
-## Using the CLI
+Congratulations! You have successfully run your first pipeline locally.
 
-Now that your pipeline is functional, you can push it to the OpenHexa backend so that it can run online.
+If you inspect the actual pipeline code, you will see that it doesn't do a lot of things, but it is still a perfectly 
+valid OpenHexa pipeline.
 
-As code and data are organized with workspaces, the first think to do is to activate a workspace using the CLI.
+Let's publish to an actual OpenHexa workspace so that it can run online.
 
-Using the OpenHexa interface, chose a workspace, click on the "Pipelines" section and then on the "Create" 
-call-to-action at the top-right of the header. You will find ready-to use instructions on how to activate 
-the workspace, as well as the API token you need to use.
+Using the OpenHexa web interface, within a workspace, navigate to the Pipelines tab and click on "Create".
 
-The command looks as follows:
+Copy the command displayed in the popup in your terminal:
 
 ```shell
-openhexa workspaces add <workspace_slug>
+openhexa workspaces add <workspace>
 ```
 
-You can then push your pipeline:
+You will be prompted for an authentication token, you can find it in the popup as well.
+
+After adding the workspace using the CLI, you can now push your pipeline:
 
 ```shell
-openhexa pipelines push <pipeline_directory>
+openhexa pipelines push 
 ```
 
-## Development & testing
+As it is the first time, the CLI will ask you to confirm the creation operation. After confirmation the console will 
+output the link to the pipeline screen in the OpenHexa interface.
+
+You can now open the link and run the pipeline using the OpenHexa web interface.
+
+### Using the SDK in the notebooks environment
+
+TBC
+
+## Contributing
+
+The following sections explain how you can setup a local development environment if you want to participate to the 
+development of the SDK
 
 ### Development setup
 
 Install the SDK in editable mode:
 
 ```shell
 python -m venv venv # Create a virtual environment for this project
@@ -99,16 +115,15 @@
 
 Run the tests using pytest:
 
 ```shell
 pytest
 ```
 
-
-## Publishing the pipelines image
+### Publishing the pipelines image
 
 The docker image `openhexa-pipelines` is still build and published manually. Follow the steps below to publish a new docker image.
 
 ```shell
 cd openhexa-sdk-python
 python -m build .
 mv dist/*.whl docker/
```

### Comparing `openhexa.sdk-0.1.4/README.md` & `openhexa.sdk-0.1.5/openhexa.sdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,100 @@
+Metadata-Version: 2.1
+Name: openhexa.sdk
+Version: 0.1.5
+Summary: OpenHexa SDK
+Home-page: https://github.com/BLSQ/openhexa-sdk-python
+Author: Bluesquare
+Author-email: dev@bluesquarehub.com
+License: MIT License
+Keywords: openhexa,pipelines
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: examples
+License-File: LICENCE
+
 # OpenHexa Python SDK
 
 The OpenHexa Python SDK is a tool that helps you write code for the OpenHexa platform.
 
 It is particularly useful to write OpenHexa data pipelines, but can also be used in the OpenHexa notebooks environment.
 
-## Writing data pipelines
-
-TBC
+## Quickstart
 
-## Using the SDK in the notebooks environment
+### Writing and deploying pipelines
 
-TBC
+Here's a super minimal example to get you started. First, create a new directory and a virtual environment:
 
-## Running the examples
+```shell
+mkdir openhexa-pipelines-quickstart
+cd openhexa-pipelines-quickstart
+virtualenv venv
+source venv/bin/activate
+```
 
-Clone the repo and install the dependencies, including the ones required to run the examples:
+You can then install the OpenHexa SDK:
 
 ```shell
-git checkout https://github.com/BLSQ/openhexa-sdk-python.git
-pip install ".[examples]"
+pip install openhexa.sdk
 ```
 
-Run a pipeline:
+Now that the SDK is installed withing your virtual environmentYou can now use the `openhexa` CLI utility to create 
+a new pipeline:
 
 ```shell
-cd examples/pipelines/logistic_stats
-python pipeline.py -c '{"deg":"qfxEYY9xAl6","periods":["2022Q1","2022Q2"]}'
+openhexa pipelines init "My awesome pipeline"
 ```
 
-Or using a config file:
+Great! As you can see in the console output, the OpenHexa CLI has created a new directory, which contains the basic 
+structure required for an OpenHexa pipeline. You can now `cd` in the new pipeline directory and run the pipeline:
 
 ```shell
-cd examples/pipelines/logistic_stats
-python pipeline.py -f example_conf.json
+cd my_awesome_pipeline
+python pipeline.py
 ```
 
-## Using the CLI
+Congratulations! You have successfully run your first pipeline locally.
 
-Now that your pipeline is functional, you can push it to the OpenHexa backend so that it can run online.
+If you inspect the actual pipeline code, you will see that it doesn't do a lot of things, but it is still a perfectly 
+valid OpenHexa pipeline.
 
-As code and data are organized with workspaces, the first think to do is to activate a workspace using the CLI.
+Let's publish to an actual OpenHexa workspace so that it can run online.
 
-Using the OpenHexa interface, chose a workspace, click on the "Pipelines" section and then on the "Create" 
-call-to-action at the top-right of the header. You will find ready-to use instructions on how to activate 
-the workspace, as well as the API token you need to use.
+Using the OpenHexa web interface, within a workspace, navigate to the Pipelines tab and click on "Create".
 
-The command looks as follows:
+Copy the command displayed in the popup in your terminal:
 
 ```shell
-openhexa workspaces add <workspace_slug>
+openhexa workspaces add <workspace>
 ```
 
-You can then push your pipeline:
+You will be prompted for an authentication token, you can find it in the popup as well.
+
+After adding the workspace using the CLI, you can now push your pipeline:
 
 ```shell
-openhexa pipelines push <pipeline_directory>
+openhexa pipelines push 
 ```
 
-## Development & testing
+As it is the first time, the CLI will ask you to confirm the creation operation. After confirmation the console will 
+output the link to the pipeline screen in the OpenHexa interface.
+
+You can now open the link and run the pipeline using the OpenHexa web interface.
+
+### Using the SDK in the notebooks environment
+
+TBC
+
+## Contributing
+
+The following sections explain how you can setup a local development environment if you want to participate to the 
+development of the SDK
 
 ### Development setup
 
 Install the SDK in editable mode:
 
 ```shell
 python -m venv venv # Create a virtual environment for this project
@@ -82,16 +115,15 @@
 
 Run the tests using pytest:
 
 ```shell
 pytest
 ```
 
-
-## Publishing the pipelines image
+### Publishing the pipelines image
 
 The docker image `openhexa-pipelines` is still build and published manually. Follow the steps below to publish a new docker image.
 
 ```shell
 cd openhexa-sdk-python
 python -m build .
 mv dist/*.whl docker/
```

### Comparing `openhexa.sdk-0.1.4/openhexa/cli/api.py` & `openhexa.sdk-0.1.5/openhexa/cli/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/cli/cli.py` & `openhexa.sdk-0.1.5/openhexa/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,17 @@
     click.echo(
         f"Run it using {click.style(f'cd {new_pipeline_directory_name}', fg='cyan')} && "
         f"{click.style('python pipeline.py', fg='cyan')}"
     )
 
 
 @pipelines.command("push")
-@click.argument("path", type=click.Path(exists=True, file_okay=False, dir_okay=True))
+@click.argument(
+    "path", default=".", type=click.Path(exists=True, file_okay=False, dir_okay=True)
+)
 def pipelines_push(path: str):
     """
     Push a pipeline to the backend. If the pipeline already exists, it will be updated otherwise it will be created.
 
     PATH is the path to the pipeline file.
     """
 
@@ -280,15 +282,17 @@
         click.echo(
             f"Pushing pipeline {click.style(pipeline.code, bold=True)} to workspace {click.style(workspace, bold=True)}"
         )
 
         new_version = upload_pipeline(user_config, path)
         click.echo(f"New version created: {new_version}")
 
-        url = f"{user_config['openhexa']['url']}/workspaces/{workspace}/pipelines/{pipeline.code}"
+        url = f"{user_config['openhexa']['url']}/workspaces/{workspace}/pipelines/{pipeline.code}".replace(
+            "api", "app"
+        )
         click.echo(
             f"Done! You can view the pipeline in OpenHexa on {click.style(url, fg='bright_blue', underline=True)}"
         )
 
 
 @pipelines.command("list")
 def pipelines_list():
```

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/parameter.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/pipeline.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def task(self, function):
         """task decorator"""
 
         return PipelineWithTask(function, self)
 
     def run(self, config: typing.Dict[str, typing.Any]):
         now = datetime.datetime.utcnow().replace(microsecond=0).isoformat()
-        print(f'{now} Evaluating "{self.code}"')
+        print(f'{now} Starting pipeline "{self.code}"')
 
         # Validate / default parameters
         validated_config = {}
         for parameter in self.parameters:
             value = config.pop(parameter.code, None)
             validated_value = parameter.validate(value)
             validated_config[parameter.code] = validated_value
@@ -126,27 +126,29 @@
                     try:
                         task_com_result = result.get()
                         task.result = task_com_result.result
                         task.start_time = task_com_result.start_time
                         task.end_time = task_com_result.end_time
                         dag_step = True
                     except Exception as e:  # NOQA
-                        raise PipelineRunError(f"Pipeline failed: {e}")
+                        raise PipelineRunError(f"Pipeline {self.code} failed: {e}")
 
                 if dag_step:
                     # remove finished tasks
                     result_list = [(r, t) for r, t in result_list if not r.ready()]
                     break
                 else:
                     # busy loop
                     time.sleep(0.3)
 
         pool.close()
         pool.join()
 
+        print(f'{now} Successfully completed pipeline "{self.code}"')
+
     def get_available_tasks(self):
         return [task for task in self.tasks if task.is_ready()]
 
     def parameters_spec(self):
         return [arg.parameter_spec() for arg in self.parameters]
 
     def _update_progress(self, progress: int):
```

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/run.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/runtime.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/runtime.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/task.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/task.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/pipelines/utils.py` & `openhexa.sdk-0.1.5/openhexa/sdk/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa/sdk/workspaces/workspace.py` & `openhexa.sdk-0.1.5/openhexa/sdk/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/openhexa.sdk.egg-info/SOURCES.txt` & `openhexa.sdk-0.1.5/openhexa.sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/pyproject.toml` & `openhexa.sdk-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/setup.cfg` & `openhexa.sdk-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/tests/test_parameter.py` & `openhexa.sdk-0.1.5/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.4/tests/test_pipeline.py` & `openhexa.sdk-0.1.5/tests/test_pipeline.py`

 * *Files identical despite different names*


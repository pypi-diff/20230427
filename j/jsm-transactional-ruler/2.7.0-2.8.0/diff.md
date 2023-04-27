# Comparing `tmp/jsm_transactional_ruler-2.7.0.tar.gz` & `tmp/jsm_transactional_ruler-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_transactional_ruler-2.7.0.tar", max compression
+gzip compressed data, was "jsm_transactional_ruler-2.8.0.tar", max compression
```

## Comparing `jsm_transactional_ruler-2.7.0.tar` & `jsm_transactional_ruler-2.8.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     2510 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/README.md
--rw-r--r--   0        0        0     4222 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/enums.py
--rw-r--r--   0        0        0     1131 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/events.py
--rw-r--r--   0        0        0       49 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/exceptions.py
--rw-r--r--   0        0        0      938 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/publisher.py
--rw-r--r--   0        0        0     1514 2023-02-13 20:28:38.425363 jsm_transactional_ruler-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 jsm_transactional_ruler-2.7.0/setup.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 jsm_transactional_ruler-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2510 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/README.md
+-rw-r--r--   0        0        0     4322 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/enums.py
+-rw-r--r--   0        0        0     1131 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/events.py
+-rw-r--r--   0        0        0       49 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/exceptions.py
+-rw-r--r--   0        0        0      938 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/publisher.py
+-rw-r--r--   0        0        0     1545 2023-04-27 17:26:56.905798 jsm_transactional_ruler-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 jsm_transactional_ruler-2.8.0/PKG-INFO
```

### Comparing `jsm_transactional_ruler-2.7.0/README.md` & `jsm_transactional_ruler-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/enums.py` & `jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,11 +50,12 @@
     T_EVENT_ONE_LAST_STAMP_NEW_PROFISSIONAL_MAIS = "T_EVENT_ONE_LAST_STAMP_NEW_PROFISSIONAL_MAIS"
     T_EVENT_COMPLETE_CARD_NEW_PROFISSIONAL_MAIS = "T_EVENT_COMPLETE_CARD_NEW_PROFISSIONAL_MAIS"
     T_EVENT_LAST_30_DAYS_OF_BONUS_NEW_PROFISSIONAL_MAIS = "T_EVENT_LAST_30_DAYS_OF_BONUS_NEW_PROFISSIONAL_MAIS"
     T_EVENT_PURCHASE_TOP_CASHBACK = "T_EVENT_PURCHASE_TOP_CASHBACK"
     T_EVENT_PURCHASE_VOUCHER = "T_EVENT_PURCHASE_VOUCHER"
     T_EVENT_CERTIFICATION = "T_EVENT_CERTIFICATION"
     T_EVENT_NEW_LUCKY_NUMBER_AVAILABLE = "T_EVENT_NEW_LUCKY_NUMBER_AVAILABLE"
+    T_EVENT_POINTSBACK_SUCCESSFUL_RECEIVED_POINTS = "T_EVENT_POINTSBACK_SUCCESSFUL_RECEIVED_POINTS"
 
     @classmethod
     def get_choices(cls):
         return tuple(item.value for item in cls)
```

### Comparing `jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/events.py` & `jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/events.py`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.7.0/jsm_transactional_ruler/publisher.py` & `jsm_transactional_ruler-2.8.0/jsm_transactional_ruler/publisher.py`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.7.0/pyproject.toml` & `jsm_transactional_ruler-2.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "jsm-transactional-ruler"
-version = "2.7.0"
+version = "2.8.0"
 description = "Lib to post user events on transactional topics"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 maintainers = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 readme = "README.md"
 homepage = "https://juntossomosmais.com.br"
 repository = "https://github.com/juntossomosmais/transactional-ruler"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 django-stomp = ">=4.2.0"
 Django = "*"
+docopt = "0.6.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-tox = "^3.15.0"
+pytest = "*"
+tox = "4.5.1"
 black = "^19.10b0"
 pycodestyle = "^2.6.0"
 pytest-env = "^0.6.2"
 pytest-cov = "^2.8.1"
 flake8 = "^3.8.1"
 mypy = "^0.770"
 isort = "^4.3.21"
@@ -33,14 +34,15 @@
 [testenv]
 passenv = *
 deps = poetry
 commands =
     poetry install --no-root
     pytest tests -vv --cov=. --doctest-modules --junitxml=junit/test-results.xml --cov-report=xml --cov-report=html --cov-report=term --cov-append
 """
+docopt = "==0.6.2"
 
 [tool.isort]
 force_single_line = true
 line_length = 120
 use_parentheses = true
 multi_line_output = 5
 include_trailing_comma = true
```

### Comparing `jsm_transactional_ruler-2.7.0/setup.py` & `jsm_transactional_ruler-2.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jsm-transactional-ruler
+Version: 2.8.0
+Summary: Lib to post user events on transactional topics
+Home-page: https://juntossomosmais.com.br
+Author: Juntos Somos Mais
+Author-email: labs@juntossomosmais.com.br
+Maintainer: Juntos Somos Mais
+Maintainer-email: labs@juntossomosmais.com.br
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django
+Requires-Dist: django-stomp (>=4.2.0)
+Requires-Dist: docopt (==0.6.2)
+Project-URL: Repository, https://github.com/juntossomosmais/transactional-ruler
+Description-Content-Type: text/markdown
 
-packages = \
-['jsm_transactional_ruler']
+# Transactional Ruler
 
-package_data = \
-{'': ['*']}
+Lib to post user events on transactional topics
 
-install_requires = \
-['Django', 'django-stomp>=4.2.0']
-
-setup_kwargs = {
-    'name': 'jsm-transactional-ruler',
-    'version': '2.7.0',
-    'description': 'Lib to post user events on transactional topics',
-    'long_description': '# Transactional Ruler\n\nLib to post user events on transactional topics\n\n## Running tests and lint\n\n`docker-compose up integration-tests`\n`docker-compose up lint`\n\n## Installation\n\n`pip install jsm-transactional-ruler`\n\n## Example Usage\n\n```python\nfrom jsm_transactional_ruler.enums import EventType\nfrom jsm_transactional_ruler.events import Event\nfrom jsm_transactional_ruler.publisher import publish_event\n\nevent = Event(\n    user_id="fake_id", event_type=EventType.T_EVENT_REGISTERED_USER, data={"email": "teste@juntossomosmais.com.br"}\n)\npublish_event(event_trigger=event)\n```\n\nThe attribute `event_type` accepts only events registered in the `EventType` enum.\n\nThe `publish_event` method accepts the optional `queue` and `publisher_parameters` parameters to send to django-stomp:\n\n\n```python\nevent = Event(\n    user_id="fake_id", event_type=EventType.T_EVENT_REGISTERED_USER, data={"email": "teste@juntossomosmais.com.br"}\n)\npublish_event(event_trigger=event, queue="/topic/VirtualTopic.user-update-transactions", persistent=False)\n```\n\n## Versioning\nThis lib follows the [pypi version format](https://www.python.org/dev/peps/pep-0440/) with the convention of using \n_major_._minor_._patch_ version.\n\n### When to bump a patch version?\nBump the patch version if you are doing a quick fix, nothing that changes the library functionality.\n\n### When to bump the minor version?\nBump the minor version if you are adding new functionality without breaking backwards compatibility. For example, \nadding support to new events.\n\n### When to bump the major version?\nBump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.\n\n## Contributing\n\nThis project uses a [trunk based development](https://trunkbaseddevelopment.com/) flow, so that we have only one long-lived branch (`master`).\n\nFor any development, simply create a branch from it and follow the flow described [below](#how-to-upload-lib-to-pypi).\n\n## How to upload lib to PyPI\n\nIt is necessary to update the lib version using the command below:\n\n```shell\n$ poetry version major|minor|patch\n```\n\nAfter generating the version:\n* Create a new branch with the files updated by Poetry\n* Open PR based on the `master` branch\n* Merge PR into the master\n* Generate a new release based on the version. [Document to generate release](https://docs.github.com/en/enterprise/2.13/user/articles/creating-releases)\n* After generating the new release "Github Actions" will upload the lib to PyPI using Poetry.\n* Good job!',
-    'author': 'Juntos Somos Mais',
-    'author_email': 'labs@juntossomosmais.com.br',
-    'maintainer': 'Juntos Somos Mais',
-    'maintainer_email': 'labs@juntossomosmais.com.br',
-    'url': 'https://juntossomosmais.com.br',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+## Running tests and lint
 
+`docker-compose up integration-tests`
+`docker-compose up lint`
 
-setup(**setup_kwargs)
+## Installation
+
+`pip install jsm-transactional-ruler`
+
+## Example Usage
+
+```python
+from jsm_transactional_ruler.enums import EventType
+from jsm_transactional_ruler.events import Event
+from jsm_transactional_ruler.publisher import publish_event
+
+event = Event(
+    user_id="fake_id", event_type=EventType.T_EVENT_REGISTERED_USER, data={"email": "teste@juntossomosmais.com.br"}
+)
+publish_event(event_trigger=event)
+```
+
+The attribute `event_type` accepts only events registered in the `EventType` enum.
+
+The `publish_event` method accepts the optional `queue` and `publisher_parameters` parameters to send to django-stomp:
+
+
+```python
+event = Event(
+    user_id="fake_id", event_type=EventType.T_EVENT_REGISTERED_USER, data={"email": "teste@juntossomosmais.com.br"}
+)
+publish_event(event_trigger=event, queue="/topic/VirtualTopic.user-update-transactions", persistent=False)
+```
+
+## Versioning
+This lib follows the [pypi version format](https://www.python.org/dev/peps/pep-0440/) with the convention of using 
+_major_._minor_._patch_ version.
+
+### When to bump a patch version?
+Bump the patch version if you are doing a quick fix, nothing that changes the library functionality.
+
+### When to bump the minor version?
+Bump the minor version if you are adding new functionality without breaking backwards compatibility. For example, 
+adding support to new events.
+
+### When to bump the major version?
+Bump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.
+
+## Contributing
+
+This project uses a [trunk based development](https://trunkbaseddevelopment.com/) flow, so that we have only one long-lived branch (`master`).
+
+For any development, simply create a branch from it and follow the flow described [below](#how-to-upload-lib-to-pypi).
+
+## How to upload lib to PyPI
+
+It is necessary to update the lib version using the command below:
+
+```shell
+$ poetry version major|minor|patch
+```
+
+After generating the version:
+* Create a new branch with the files updated by Poetry
+* Open PR based on the `master` branch
+* Merge PR into the master
+* Generate a new release based on the version. [Document to generate release](https://docs.github.com/en/enterprise/2.13/user/articles/creating-releases)
+* After generating the new release "Github Actions" will upload the lib to PyPI using Poetry.
+* Good job!
```


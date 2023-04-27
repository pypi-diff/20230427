# Comparing `tmp/starlette_babel-0.2.4.tar.gz` & `tmp/starlette_babel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_babel-0.2.4.tar", max compression
+gzip compressed data, was "starlette_babel-1.0.0.tar", max compression
```

## Comparing `starlette_babel-0.2.4.tar` & `starlette_babel-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/LICENSE
--rw-r--r--   0        0        0    13359 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/README.md
--rw-r--r--   0        0        0     2653 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1454 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/__init__.py
--rw-r--r--   0        0        0        0 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/contrib/__init__.py
--rw-r--r--   0        0        0     1808 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/contrib/jinja.py
--rw-r--r--   0        0        0     4789 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/formatters.py
--rw-r--r--   0        0        0     6517 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/locale.py
--rw-r--r--   0        0        0        0 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/py.typed
--rw-r--r--   0        0        0     4717 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/timezone.py
--rw-r--r--   0        0        0     7376 2023-01-09 12:21:44.497570 starlette_babel-0.2.4/starlette_babel/translator.py
--rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 starlette_babel-0.2.4/setup.py
--rw-r--r--   0        0        0    14456 1970-01-01 00:00:00.000000 starlette_babel-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-27 13:13:10.856617 starlette_babel-1.0.0/LICENSE
+-rw-r--r--   0        0        0    13359 2023-04-27 13:13:10.856617 starlette_babel-1.0.0/README.md
+-rw-r--r--   0        0        0     2658 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1454 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/contrib/__init__.py
+-rw-r--r--   0        0        0     1808 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/contrib/jinja.py
+-rw-r--r--   0        0        0     4789 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/formatters.py
+-rw-r--r--   0        0        0     6517 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/locale.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/py.typed
+-rw-r--r--   0        0        0     4717 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/timezone.py
+-rw-r--r--   0        0        0     7376 2023-04-27 13:13:10.860617 starlette_babel-1.0.0/starlette_babel/translator.py
+-rw-r--r--   0        0        0    14516 1970-01-01 00:00:00.000000 starlette_babel-1.0.0/PKG-INFO
```

### Comparing `starlette_babel-0.2.4/LICENSE` & `starlette_babel-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/README.md` & `starlette_babel-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/pyproject.toml` & `starlette_babel-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "starlette_babel"
 description = "Locale support for Starlette"
-version = "0.2.4"
+version = "1.0.0"
 authors = ["Alex Oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alex-oleshkevich/starlette_babel"
 repository = "https://github.com/alex-oleshkevich/starlette_babel"
 documentation = "https://github.com/alex-oleshkevich/starlette_babel"
 keywords = []
@@ -19,23 +19,24 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-Babel = "^2.10.3"
+Babel = "^2.12"
+starlette = "*"
+pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
-starlette = "^0.21.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.18.0"
 pytest-cov = "^3.0"
-black = "^22.10.0"
-mypy = "^0.990"
+black = "^22.10"
+mypy = "^1.1"
 flake8 = "^4.0.1"
 httpx = "^0.23.0"
 types-babel = "^2.10.0"
 Jinja2 = "^3.1.2"
 uvicorn = "^0.18.3"
 
 [build-system]
```

### Comparing `starlette_babel-0.2.4/starlette_babel/__init__.py` & `starlette_babel-1.0.0/starlette_babel/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/starlette_babel/contrib/jinja.py` & `starlette_babel-1.0.0/starlette_babel/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/starlette_babel/formatters.py` & `starlette_babel-1.0.0/starlette_babel/formatters.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/starlette_babel/locale.py` & `starlette_babel-1.0.0/starlette_babel/locale.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/starlette_babel/timezone.py` & `starlette_babel-1.0.0/starlette_babel/timezone.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/starlette_babel/translator.py` & `starlette_babel-1.0.0/starlette_babel/translator.py`

 * *Files identical despite different names*

### Comparing `starlette_babel-0.2.4/setup.py` & `starlette_babel-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,544 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: starlette-babel
+Version: 1.0.0
+Summary: Locale support for Starlette
+Home-page: https://github.com/alex-oleshkevich/starlette_babel
+License: MIT
+Author: Alex Oleshkevich
+Author-email: alex.oleshkevich@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: Babel (>=2.12,<3.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: starlette
+Project-URL: Documentation, https://github.com/alex-oleshkevich/starlette_babel
+Project-URL: Repository, https://github.com/alex-oleshkevich/starlette_babel
+Description-Content-Type: text/markdown
 
-packages = \
-['starlette_babel', 'starlette_babel.contrib']
+# Starlette Babel
 
-package_data = \
-{'': ['*']}
+Provides translations, formatters, and timezone support for Starlette application by integrating Babel library.
 
-install_requires = \
-['Babel>=2.10.3,<3.0.0']
-
-setup_kwargs = {
-    'name': 'starlette-babel',
-    'version': '0.2.4',
-    'description': 'Locale support for Starlette',
-    'long_description': '# Starlette Babel\n\nProvides translations, formatters, and timezone support for Starlette application by integrating Babel library.\n\n![PyPI](https://img.shields.io/pypi/v/starlette_babel)\n![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/starlette_babel/Lint)\n![GitHub](https://img.shields.io/github/license/alex-oleshkevich/starlette_babel)\n![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/starlette_babel)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/starlette_babel)\n![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/starlette_babel)\n\n## Installation\n\nInstall `starlette_babel` using PIP or poetry:\n\n```bash\npip install starlette_babel\n# or\npoetry add starlette_babel\n```\n\n## Features\n\n- Locale middleware\n- Multi-domain translations\n- Locale selectors\n- Timezone middleware\n- Timezone selectors\n- Locale-aware formatters\n- Jinja2 integration\n\n## Quick start\n\nSee example application in [examples/](examples/) directory of this repository.\n\n## Setting up translator and locale features\n\n### Configure Starlette application\n\nTo start using locale aware formatters, text translation and other components you have to set up a translator\nand add middleware to your Starlette application.\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\n\nfrom starlette_babel import get_translator, LocaleMiddleware\n\nsupported_locales = [\'be\', \'en\', \'pl\']\nshared_translator = get_translator()  # process global instance\nshared_translator.load_from_directories([\'/path/to/locales/\'])  # one or multiple locale directories\n\napp = Starlette(\n    middleware=[\n        Middleware(LocaleMiddleware, locales=supported_locales, default_locale=\'en\'),\n    ]\n)\n```\n\n### Getting locale information\n\n#### From request object\n\nThe `LocaleMiddleware` adds two state options to the request: `locale` and `language`.\n\n```python\nfrom babel import Locale\n\n\ndef index_view(request):\n    current_locale: Locale = request.state.locale\n    current_language: str = request.state.language\n```\n\n#### Using `get_locale` helper\n\nAlternatively, use `get_locale` to get the locale information\n\n```python\nfrom babel import Locale\nfrom starlette_babel import get_locale\n\nlocale: Locale = get_locale()\n```\n\n### Locale selectors\n\n`LocaleMiddleware` uses locale selectors to detect the locale from the request object.\nThe selector is a callable that accepts `HTTPConnection` object and returns either a locale code as a string or\nNone. The first locale selector that returns non-None value wins.\nIf all selectors fail then the middleware sets locale from `default_locale` option.\nThe detected locale should be in the list defined by the `locales` option otherwise it won\'t be accepted.\n\nThe default selector order is:\n\n1. from `locale` query parameter\n2. from `language` cookie\n3. from `get_preferred_language` user method (will use `request.user`, if available)\n4. from `accept-language` header\n5. fallback to configured default locale\n\n#### Customizing locale selectors or changing their order\n\nIf you want to customize the way the middleware detects the locale, pass `selectors` option to the middleware:\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\n\nfrom starlette_babel import LocaleFromHeader, LocaleFromQuery, LocaleMiddleware\n\napp = Starlette(\n    middleware=[\n        Middleware(LocaleMiddleware, selectors=[\n            LocaleFromQuery(), LocaleFromHeader(),\n        ])\n    ]\n)\n```\n\nIn this example we use only two selectors. They will be called in the order they are defined.\n\n#### Custom locale selectors\n\nYou can define your own selector by writing a function or a callable object:\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\nfrom starlette.requests import HTTPConnection\n\nfrom starlette_babel import LocaleMiddleware\n\n\ndef my_locale_selector(conn: HTTPConnection) -> str | None:\n    return \'be_BY\'\n\n\napp = Starlette(\n    middleware=[\n        Middleware(LocaleMiddleware, selectors=[\n            my_locale_selector,\n        ])\n    ]\n)\n```\n\n### Mark translatable strings\n\nAt this point your application is translatable and each request contain locale information that you can use.\nLet\'s define some translatable strings\n\n> Please note, that we did not write any translations and the example below won\'t actually translate anything.\n> This is an example of how to mark strings for translation. We will cover message extraction a bit later.\n\n```python\nfrom starlette.responses import PlainTextResponse\n\nfrom starlette_babel import gettext_lazy as _\n\nwelcome_message = _(\'Welcome\')\n\n\ndef index_view(request):\n    return PlainTextResponse(welcome_message)\n```\n\n### Extract translatable strings from the source code\n\nStrings marked as translatable won\'t translate themselves. They should be extracted into `.po` files and compiled into\nmachine-readable `.mo` files. This topic is out of the scope if this documentation and is well-documented by the\n[official Babel documentation](https://babel.pocoo.org/en/latest/).\n\nA brief hint on what to do is:\n\n1. configure `pybabel` tool via `pybabel.ini`\n2. create directories for each supported locale\n3. extract strings from the source code using `pybabel extract` command\n4. update locale specific message catalogues (`messages.po`) using `pybabel update` command\n5. compile these catalogues into machine-readable format (`messages.mo`) using `pybabel compile` command.\n\nThese commands are documented\nat [https://babel.pocoo.org/en/latest/cmdline.html](https://babel.pocoo.org/en/latest/cmdline.html)\n\n#### Locales directory structure\n\nThe locales directory is a directory where we keep our translation files. Usually, this directory called `locales`.\nThe structure is like this: `locales/_code_/LC_MESSAGES/messages.po` where `_code_` is a locale code.\n\nExample:\n\n```shell\nyour_app_package_name/\n    locales/\n      en/\n        LC_MESSAGES/\n          messages.po\n      de/\n        LC_MESSAGES/\n          messages.po\n      messages.pot\n```\n\nIf the directory format does not match the expectation, translator would not be able to load messages and will fail\nsilently. You can use the [examples/locales](examples/locales) for a reference.\n\n### Enable Jinja2 plugin\n\nIf you use Jinja2 templates you can integrate translator and formatters provided by this library with Jinja.\n\n```python\nimport jinja2\n\nfrom starlette_babel.contrib.jinja import configure_jinja_env\n\njinja_env = jinja2.Environment()\nconfigure_jinja_env(jinja_env)\n```\n\nThe `configure_jinja_env` makes the following utilities available in the templates:\n\n#### Global functions\n\n- `_` - alias for `gettext`\n- `_p` - alias for `ngettext`\n\n```html\n\n<time>{{ _(\'Welcome\') }}</time>\n```\n\n#### Filters\n\n- datetime\n- date\n- time\n- timedelta\n- number\n- currency\n- percent\n- scientific\n\nAll these filters are locale-aware and will format passed data using locale defined format.\n\n```html\n\n<time>your local time is {{ now|datetime }}</time>\n```\n\n### Manually setting the locale\n\nYou can set the current locale manually\n\n```python\nfrom starlette_babel import set_locale\n\nset_locale(\'pl\')\n```\n\n### Temporary setting the locale\n\nYou can switch locale temporary for a code block using `switch_locale` context manager. When the manager exits the\nprevious locale gets restored. This utility is very useful in unit tests.\n\n```python\nfrom starlette_babel import switch_locale, set_locale\n\nset_locale(\'pl\')\n# all speak Polish here\n\nwith switch_locale(\'be\'):\n    # all speak Belarussian here\n    ...\n\n# all speak Polish here again\n```\n\n### Manually translating strings\n\nYou can translate messages using `translator.gettext` and `translator.ngettext` directly in the code of the view\nfunction:\n\n```python\nfrom starlette_babel import Translator\n\ntranslator = Translator([\'/path/to/locales\'])\n\n\ndef index_view(request):\n    translated = translator.gettext(\'Hello\', locale=\'en\')\n```\n\n### Translation domains\n\n> This is advanced topic. Most apps don\'t need this but library developers may need it.\n\nA translation domain is like a namespace. Same message can have different translations depending on the context (aka\ndomain). This library natively supports domains. We infer domain name from the .po file name, dropping the extension.\nFor the file like `locales/en/LC_MESSAGES/errors.po` the domain is `errors`.\nThe default translation domain is `messages`.\n\n```python\nfrom starlette_babel import Translator\n\ntranslator = Translator([\'/path/to/locales\'])\nhello_message = translator.gettext(\'Hello\', locale=\'en\')  # uses default `messages` domain\nshopping_hello_message = translator.gettext(\'Hello\', locale=\'en\', domain=\'shopping\')  # uses `shopping` domain\n```\n\n#### Directory structure\n\nThe structure is exactly the same as stated above.\n\n```shell\nyour_app_package_name/\n    locales/\n      en/\n        LC_MESSAGES/\n          messages.po\n          shopping.po # <-- new file. defines "shopping" domain\n```\n\n## Formatters\n\nThe library integrates formatting utilities from the Babel package.\nOur version automatically applies current locale/timezone without defining them manually.\n\nHere is the list of adapted formatters:\n\n- format_datetime\n- format_date\n- format_time\n- format_timedelta\n- format_interval\n- format_number\n- format_currency\n- format_percent\n- format_scientific\n\nConsult [Babel documentation](https://babel.pocoo.org/en/latest/index.html) for more information.\n\n### Usage\n\n```python\nimport datetime\n\nfrom starlette_babel import format_datetime, set_locale, set_timezone\n\nset_locale(\'be\')\nset_timezone(\'Europe/Minsk\')\nnow = datetime.datetime.now()\nlocal_time = format_datetime(now)  # <-- this\n```\n\n### Jinja integration\n\nThere formatters are automatically exposed to templates after applying `configure_jinja_env` on Jinja environment.\n\n## Timezone support\n\nTo enable timezone support add `TimezoneMiddleware`. The middleware behaves much like `LocaleMiddleware` and shares same\nconcepts.\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\n\nfrom starlette_babel import TimezoneMiddleware\n\napp = Starlette(\n    middleware=[\n        Middleware(TimezoneMiddleware, fallback=\'Europe/London\')\n    ]\n)\n```\n\nBy default, the middleware will try these selectors:\n\n1. from `tz` query parameter\n2. from `timezone` cookie\n2. from `get_timezone` user method\n\n### Retrieving timezone information\n\n#### Reading timezone from request object\n\n```python\nfrom pytz import BaseTzInfo\n\n\ndef index_view(request):\n    timezone: BaseTzInfo = request.state.timezone\n```\n\n#### Using `get_timezone` helper\n\nUse `get_timezone` helper to get the timezone information set by the middleware.\nIf middleware not used it will return UTC zone info.\n\n```python\nfrom pytz import BaseTzInfo\n\nfrom starlette_babel import get_timezone\n\ntz: BaseTzInfo = get_timezone()\n```\n\n### Customizing selectors or changing their order\n\nYou can change selectors set or the order they are defined by configuring `selectors` option of the middleware:\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\n\nfrom starlette_babel import TimezoneFromCookie, TimezoneFromQuery, TimezoneMiddleware\n\napp = Starlette(\n    middleware=[\n        Middleware(TimezoneMiddleware, fallback=\'Europe/London\', selectors=[\n            TimezoneFromQuery(), TimezoneFromCookie(),\n        ])\n    ]\n)\n```\n\n### Custom timezone selectors\n\nA selector is a callable that accepts `HTTPConnection` and returns timezone code as a string:\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\n\nfrom starlette_babel import TimezoneMiddleware\n\n\ndef my_timezone_selector(conn):\n    return \'Europe/Minsk\'\n\n\napp = Starlette(\n    middleware=[\n        Middleware(TimezoneMiddleware, fallback=\'Europe/London\', selectors=[\n            my_timezone_selector,\n        ])\n    ]\n)\n```\n\n### Setting timezone manually\n\nUse `set_timezone` to set the timezone.\n\n```python\nfrom starlette_babel import set_timezone\n\nset_timezone(\'Europe/Minsk\')\n```\n\n### Temporary switch timezone\n\nUse `set_timezone` to set the timezone.\n\n```python\nfrom starlette_babel import switch_timezone\n\nset_timezone(\'Europe/Minsk\')\n# time in +03\n\nwith switch_timezone(\'Europe/Warsaw\'):\n    # time in +02\n    ...\n\n# time in +03 again\n```\n\n### Convert datetime into user local time\n\nYou can apply currently active timezone to any datetime instance using `to_user_timezone` helper.\n\n```python\nimport datetime\nfrom starlette_babel import to_user_timezone, set_timezone\n\nset_timezone(\'Europe/Minsk\')\nnow = datetime.datetime.utcnow()  # time in UTC\nuser_now = to_user_timezone(now)  # time in Europe/Minsk\n```\n\n### Convert user local time to UTC\n\nYou can also convert datetime instance back to UTC using `to_utc` helper.\n\n```python\nimport datetime\n\nfrom starlette_babel import set_timezone, to_user_timezone, to_utc\n\nset_timezone(\'Europe/Minsk\')\nnow = datetime.datetime.now()  # time in UTC\nuser_now = to_user_timezone(now)  # time in Europe/Minsk\nutc_now = to_utc(user_now)  # time in UTC again\n```\n\n### Getting current time in user timezone\n\nTo get current user time use `now` helper.\n\n```python\nfrom starlette_babel import set_timezone, now\n\nset_timezone(\'Europe/Minsk\')\nuser_now = now()  # time in Europe/Minsk\n```\n',
-    'author': 'Alex Oleshkevich',
-    'author_email': 'alex.oleshkevich@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alex-oleshkevich/starlette_babel',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+![PyPI](https://img.shields.io/pypi/v/starlette_babel)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/starlette_babel/Lint)
+![GitHub](https://img.shields.io/github/license/alex-oleshkevich/starlette_babel)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/starlette_babel)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/starlette_babel)
+![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/starlette_babel)
 
+## Installation
+
+Install `starlette_babel` using PIP or poetry:
+
+```bash
+pip install starlette_babel
+# or
+poetry add starlette_babel
+```
+
+## Features
+
+- Locale middleware
+- Multi-domain translations
+- Locale selectors
+- Timezone middleware
+- Timezone selectors
+- Locale-aware formatters
+- Jinja2 integration
+
+## Quick start
+
+See example application in [examples/](examples/) directory of this repository.
+
+## Setting up translator and locale features
+
+### Configure Starlette application
+
+To start using locale aware formatters, text translation and other components you have to set up a translator
+and add middleware to your Starlette application.
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+
+from starlette_babel import get_translator, LocaleMiddleware
+
+supported_locales = ['be', 'en', 'pl']
+shared_translator = get_translator()  # process global instance
+shared_translator.load_from_directories(['/path/to/locales/'])  # one or multiple locale directories
+
+app = Starlette(
+    middleware=[
+        Middleware(LocaleMiddleware, locales=supported_locales, default_locale='en'),
+    ]
+)
+```
+
+### Getting locale information
+
+#### From request object
+
+The `LocaleMiddleware` adds two state options to the request: `locale` and `language`.
+
+```python
+from babel import Locale
+
+
+def index_view(request):
+    current_locale: Locale = request.state.locale
+    current_language: str = request.state.language
+```
+
+#### Using `get_locale` helper
+
+Alternatively, use `get_locale` to get the locale information
+
+```python
+from babel import Locale
+from starlette_babel import get_locale
+
+locale: Locale = get_locale()
+```
+
+### Locale selectors
+
+`LocaleMiddleware` uses locale selectors to detect the locale from the request object.
+The selector is a callable that accepts `HTTPConnection` object and returns either a locale code as a string or
+None. The first locale selector that returns non-None value wins.
+If all selectors fail then the middleware sets locale from `default_locale` option.
+The detected locale should be in the list defined by the `locales` option otherwise it won't be accepted.
+
+The default selector order is:
+
+1. from `locale` query parameter
+2. from `language` cookie
+3. from `get_preferred_language` user method (will use `request.user`, if available)
+4. from `accept-language` header
+5. fallback to configured default locale
+
+#### Customizing locale selectors or changing their order
+
+If you want to customize the way the middleware detects the locale, pass `selectors` option to the middleware:
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+
+from starlette_babel import LocaleFromHeader, LocaleFromQuery, LocaleMiddleware
+
+app = Starlette(
+    middleware=[
+        Middleware(LocaleMiddleware, selectors=[
+            LocaleFromQuery(), LocaleFromHeader(),
+        ])
+    ]
+)
+```
+
+In this example we use only two selectors. They will be called in the order they are defined.
+
+#### Custom locale selectors
+
+You can define your own selector by writing a function or a callable object:
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+from starlette.requests import HTTPConnection
+
+from starlette_babel import LocaleMiddleware
+
+
+def my_locale_selector(conn: HTTPConnection) -> str | None:
+    return 'be_BY'
+
+
+app = Starlette(
+    middleware=[
+        Middleware(LocaleMiddleware, selectors=[
+            my_locale_selector,
+        ])
+    ]
+)
+```
+
+### Mark translatable strings
+
+At this point your application is translatable and each request contain locale information that you can use.
+Let's define some translatable strings
+
+> Please note, that we did not write any translations and the example below won't actually translate anything.
+> This is an example of how to mark strings for translation. We will cover message extraction a bit later.
+
+```python
+from starlette.responses import PlainTextResponse
+
+from starlette_babel import gettext_lazy as _
+
+welcome_message = _('Welcome')
+
+
+def index_view(request):
+    return PlainTextResponse(welcome_message)
+```
+
+### Extract translatable strings from the source code
+
+Strings marked as translatable won't translate themselves. They should be extracted into `.po` files and compiled into
+machine-readable `.mo` files. This topic is out of the scope if this documentation and is well-documented by the
+[official Babel documentation](https://babel.pocoo.org/en/latest/).
+
+A brief hint on what to do is:
+
+1. configure `pybabel` tool via `pybabel.ini`
+2. create directories for each supported locale
+3. extract strings from the source code using `pybabel extract` command
+4. update locale specific message catalogues (`messages.po`) using `pybabel update` command
+5. compile these catalogues into machine-readable format (`messages.mo`) using `pybabel compile` command.
+
+These commands are documented
+at [https://babel.pocoo.org/en/latest/cmdline.html](https://babel.pocoo.org/en/latest/cmdline.html)
+
+#### Locales directory structure
+
+The locales directory is a directory where we keep our translation files. Usually, this directory called `locales`.
+The structure is like this: `locales/_code_/LC_MESSAGES/messages.po` where `_code_` is a locale code.
+
+Example:
+
+```shell
+your_app_package_name/
+    locales/
+      en/
+        LC_MESSAGES/
+          messages.po
+      de/
+        LC_MESSAGES/
+          messages.po
+      messages.pot
+```
+
+If the directory format does not match the expectation, translator would not be able to load messages and will fail
+silently. You can use the [examples/locales](examples/locales) for a reference.
+
+### Enable Jinja2 plugin
+
+If you use Jinja2 templates you can integrate translator and formatters provided by this library with Jinja.
+
+```python
+import jinja2
+
+from starlette_babel.contrib.jinja import configure_jinja_env
+
+jinja_env = jinja2.Environment()
+configure_jinja_env(jinja_env)
+```
+
+The `configure_jinja_env` makes the following utilities available in the templates:
+
+#### Global functions
+
+- `_` - alias for `gettext`
+- `_p` - alias for `ngettext`
+
+```html
+
+<time>{{ _('Welcome') }}</time>
+```
+
+#### Filters
+
+- datetime
+- date
+- time
+- timedelta
+- number
+- currency
+- percent
+- scientific
+
+All these filters are locale-aware and will format passed data using locale defined format.
+
+```html
+
+<time>your local time is {{ now|datetime }}</time>
+```
+
+### Manually setting the locale
+
+You can set the current locale manually
+
+```python
+from starlette_babel import set_locale
+
+set_locale('pl')
+```
+
+### Temporary setting the locale
+
+You can switch locale temporary for a code block using `switch_locale` context manager. When the manager exits the
+previous locale gets restored. This utility is very useful in unit tests.
+
+```python
+from starlette_babel import switch_locale, set_locale
+
+set_locale('pl')
+# all speak Polish here
+
+with switch_locale('be'):
+    # all speak Belarussian here
+    ...
+
+# all speak Polish here again
+```
+
+### Manually translating strings
+
+You can translate messages using `translator.gettext` and `translator.ngettext` directly in the code of the view
+function:
+
+```python
+from starlette_babel import Translator
+
+translator = Translator(['/path/to/locales'])
+
+
+def index_view(request):
+    translated = translator.gettext('Hello', locale='en')
+```
+
+### Translation domains
+
+> This is advanced topic. Most apps don't need this but library developers may need it.
+
+A translation domain is like a namespace. Same message can have different translations depending on the context (aka
+domain). This library natively supports domains. We infer domain name from the .po file name, dropping the extension.
+For the file like `locales/en/LC_MESSAGES/errors.po` the domain is `errors`.
+The default translation domain is `messages`.
+
+```python
+from starlette_babel import Translator
+
+translator = Translator(['/path/to/locales'])
+hello_message = translator.gettext('Hello', locale='en')  # uses default `messages` domain
+shopping_hello_message = translator.gettext('Hello', locale='en', domain='shopping')  # uses `shopping` domain
+```
+
+#### Directory structure
+
+The structure is exactly the same as stated above.
+
+```shell
+your_app_package_name/
+    locales/
+      en/
+        LC_MESSAGES/
+          messages.po
+          shopping.po # <-- new file. defines "shopping" domain
+```
+
+## Formatters
+
+The library integrates formatting utilities from the Babel package.
+Our version automatically applies current locale/timezone without defining them manually.
+
+Here is the list of adapted formatters:
+
+- format_datetime
+- format_date
+- format_time
+- format_timedelta
+- format_interval
+- format_number
+- format_currency
+- format_percent
+- format_scientific
+
+Consult [Babel documentation](https://babel.pocoo.org/en/latest/index.html) for more information.
+
+### Usage
+
+```python
+import datetime
+
+from starlette_babel import format_datetime, set_locale, set_timezone
+
+set_locale('be')
+set_timezone('Europe/Minsk')
+now = datetime.datetime.now()
+local_time = format_datetime(now)  # <-- this
+```
+
+### Jinja integration
+
+There formatters are automatically exposed to templates after applying `configure_jinja_env` on Jinja environment.
+
+## Timezone support
+
+To enable timezone support add `TimezoneMiddleware`. The middleware behaves much like `LocaleMiddleware` and shares same
+concepts.
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+
+from starlette_babel import TimezoneMiddleware
+
+app = Starlette(
+    middleware=[
+        Middleware(TimezoneMiddleware, fallback='Europe/London')
+    ]
+)
+```
+
+By default, the middleware will try these selectors:
+
+1. from `tz` query parameter
+2. from `timezone` cookie
+2. from `get_timezone` user method
+
+### Retrieving timezone information
+
+#### Reading timezone from request object
+
+```python
+from pytz import BaseTzInfo
+
+
+def index_view(request):
+    timezone: BaseTzInfo = request.state.timezone
+```
+
+#### Using `get_timezone` helper
+
+Use `get_timezone` helper to get the timezone information set by the middleware.
+If middleware not used it will return UTC zone info.
+
+```python
+from pytz import BaseTzInfo
+
+from starlette_babel import get_timezone
+
+tz: BaseTzInfo = get_timezone()
+```
+
+### Customizing selectors or changing their order
+
+You can change selectors set or the order they are defined by configuring `selectors` option of the middleware:
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+
+from starlette_babel import TimezoneFromCookie, TimezoneFromQuery, TimezoneMiddleware
+
+app = Starlette(
+    middleware=[
+        Middleware(TimezoneMiddleware, fallback='Europe/London', selectors=[
+            TimezoneFromQuery(), TimezoneFromCookie(),
+        ])
+    ]
+)
+```
+
+### Custom timezone selectors
+
+A selector is a callable that accepts `HTTPConnection` and returns timezone code as a string:
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+
+from starlette_babel import TimezoneMiddleware
+
+
+def my_timezone_selector(conn):
+    return 'Europe/Minsk'
+
+
+app = Starlette(
+    middleware=[
+        Middleware(TimezoneMiddleware, fallback='Europe/London', selectors=[
+            my_timezone_selector,
+        ])
+    ]
+)
+```
+
+### Setting timezone manually
+
+Use `set_timezone` to set the timezone.
+
+```python
+from starlette_babel import set_timezone
+
+set_timezone('Europe/Minsk')
+```
+
+### Temporary switch timezone
+
+Use `set_timezone` to set the timezone.
+
+```python
+from starlette_babel import switch_timezone
+
+set_timezone('Europe/Minsk')
+# time in +03
+
+with switch_timezone('Europe/Warsaw'):
+    # time in +02
+    ...
+
+# time in +03 again
+```
+
+### Convert datetime into user local time
+
+You can apply currently active timezone to any datetime instance using `to_user_timezone` helper.
+
+```python
+import datetime
+from starlette_babel import to_user_timezone, set_timezone
+
+set_timezone('Europe/Minsk')
+now = datetime.datetime.utcnow()  # time in UTC
+user_now = to_user_timezone(now)  # time in Europe/Minsk
+```
+
+### Convert user local time to UTC
+
+You can also convert datetime instance back to UTC using `to_utc` helper.
+
+```python
+import datetime
+
+from starlette_babel import set_timezone, to_user_timezone, to_utc
+
+set_timezone('Europe/Minsk')
+now = datetime.datetime.now()  # time in UTC
+user_now = to_user_timezone(now)  # time in Europe/Minsk
+utc_now = to_utc(user_now)  # time in UTC again
+```
+
+### Getting current time in user timezone
+
+To get current user time use `now` helper.
+
+```python
+from starlette_babel import set_timezone, now
+
+set_timezone('Europe/Minsk')
+user_now = now()  # time in Europe/Minsk
+```
 
-setup(**setup_kwargs)
```


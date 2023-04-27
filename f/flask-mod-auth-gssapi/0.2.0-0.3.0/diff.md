# Comparing `tmp/flask-mod-auth-gssapi-0.2.0.tar.gz` & `tmp/flask-mod-auth-gssapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-mod-auth-gssapi-0.2.0.tar", max compression
+gzip compressed data, was "flask-mod-auth-gssapi-0.3.0.tar", max compression
```

## Comparing `flask-mod-auth-gssapi-0.2.0.tar` & `flask-mod-auth-gssapi-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1104 2020-07-22 13:16:22.023603 flask-mod-auth-gssapi-0.2.0/LICENSE
--rw-r--r--   0        0        0      260 2022-01-03 11:38:11.403330 flask-mod-auth-gssapi-0.2.0/README.md
--rw-r--r--   0        0        0      295 2020-07-22 12:51:10.153480 flask-mod-auth-gssapi-0.2.0/config/gssproxy.conf
--rw-r--r--   0        0        0     1072 2020-07-22 12:50:51.060262 flask-mod-auth-gssapi-0.2.0/config/httpd.conf
--rw-r--r--   0        0        0      140 2020-07-22 12:52:06.868000 flask-mod-auth-gssapi-0.2.0/config/systemd-httpd-service.conf
--rw-r--r--   0        0        0      113 2020-07-22 13:00:34.203000 flask-mod-auth-gssapi-0.2.0/config/tmpfiles.conf
--rw-r--r--   0        0        0      501 2022-01-03 11:24:52.726912 flask-mod-auth-gssapi-0.2.0/flask_mod_auth_gssapi/__init__.py
--rw-r--r--   0        0        0     1671 2022-01-03 10:57:25.763948 flask-mod-auth-gssapi-0.2.0/flask_mod_auth_gssapi/ext.py
--rw-r--r--   0        0        0     1761 2022-01-03 11:34:10.435607 flask-mod-auth-gssapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-07-22 07:55:46.936005 flask-mod-auth-gssapi-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      330 2020-07-22 12:55:32.258431 flask-mod-auth-gssapi-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     2740 2020-07-22 13:07:40.102651 flask-mod-auth-gssapi-0.2.0/tests/test_ext.py
--rw-r--r--   0        0        0      840 2022-01-03 11:28:19.074539 flask-mod-auth-gssapi-0.2.0/tox.ini
--rw-r--r--   0        0        0     1071 2022-01-03 11:38:45.387436 flask-mod-auth-gssapi-0.2.0/setup.py
--rw-r--r--   0        0        0     1398 2022-01-03 11:38:45.387694 flask-mod-auth-gssapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1104 2020-07-22 13:16:22.023603 flask-mod-auth-gssapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0      260 2022-01-03 11:38:11.403330 flask-mod-auth-gssapi-0.3.0/README.md
+-rw-r--r--   0        0        0      295 2020-07-22 12:51:10.153480 flask-mod-auth-gssapi-0.3.0/config/gssproxy.conf
+-rw-r--r--   0        0        0     1072 2020-07-22 12:50:51.060262 flask-mod-auth-gssapi-0.3.0/config/httpd.conf
+-rw-r--r--   0        0        0      140 2020-07-22 12:52:06.868000 flask-mod-auth-gssapi-0.3.0/config/systemd-httpd-service.conf
+-rw-r--r--   0        0        0      113 2020-07-22 13:00:34.203000 flask-mod-auth-gssapi-0.3.0/config/tmpfiles.conf
+-rw-r--r--   0        0        0      501 2022-01-03 11:24:52.726912 flask-mod-auth-gssapi-0.3.0/flask_mod_auth_gssapi/__init__.py
+-rw-r--r--   0        0        0     1799 2023-04-27 09:28:28.527820 flask-mod-auth-gssapi-0.3.0/flask_mod_auth_gssapi/ext.py
+-rw-r--r--   0        0        0     1684 2023-04-27 10:15:04.273934 flask-mod-auth-gssapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-07-22 07:55:46.936005 flask-mod-auth-gssapi-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      330 2020-07-22 12:55:32.258431 flask-mod-auth-gssapi-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     3535 2023-04-27 09:37:03.735528 flask-mod-auth-gssapi-0.3.0/tests/test_ext.py
+-rw-r--r--   0        0        0     1074 2023-04-27 09:33:52.422894 flask-mod-auth-gssapi-0.3.0/tox.ini
+-rw-r--r--   0        0        0     1071 2023-04-27 10:16:22.604150 flask-mod-auth-gssapi-0.3.0/setup.py
+-rw-r--r--   0        0        0     1399 2023-04-27 10:16:22.604493 flask-mod-auth-gssapi-0.3.0/PKG-INFO
```

### Comparing `flask-mod-auth-gssapi-0.2.0/LICENSE` & `flask-mod-auth-gssapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-mod-auth-gssapi-0.2.0/config/httpd.conf` & `flask-mod-auth-gssapi-0.3.0/config/httpd.conf`

 * *Files identical despite different names*

### Comparing `flask-mod-auth-gssapi-0.2.0/flask_mod_auth_gssapi/ext.py` & `flask-mod-auth-gssapi-0.3.0/flask_mod_auth_gssapi/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,18 @@
                 usage="initiate", name=gss_name, store={"ccache": ccache}
             )
         except gssapi.exceptions.GSSError as e:
             self.abort(
                 403,
                 f"Invalid credentials ({e})",
             )
-        if creds.lifetime <= 0:
+        try:
+            lifetime = creds.lifetime
+        except gssapi.exceptions.ExpiredCredentialsError:
+            lifetime = 0
+        if lifetime <= 0:
             self.abort(401, "Credential lifetime has expired")
 
         g.gss_name = gss_name
         g.gss_creds = creds
         g.principal = gss_name.display_as(gssapi.NameType.kerberos_principal)
         g.username = g.principal.split("@")[0]
```

### Comparing `flask-mod-auth-gssapi-0.2.0/pyproject.toml` & `flask-mod-auth-gssapi-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-mod-auth-gssapi"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Flask extention to make use of the authentication provided by the mod_auth_gssapi extention of Apache's HTTPd."
 
 license = "MIT"
 
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
@@ -28,27 +28,27 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.8.0"
 flask = "<3.0.0"
 gssapi = "^1.6.2"
 
 [tool.poetry.dev-dependencies]
-flake8 = "^4.0.1"
-pytest = "^6.2.5"
-pytest-mock = "^3.6.1"
-pytest-cov = "^3.0.0"
-bandit = "^1.6"
-black = {version = "^21.12b0", allow-prereleases = true}
-isort = "^5.10.1"
-coverage = {extras = ["toml"], version = "^6.2"}
+flake8 = "*"
+pytest = "*"
+pytest-mock = "*"
+pytest-cov = "*"
+bandit = "*"
+black = "*"
+isort = "*"
+coverage = {extras = ["toml"], version = "*"}
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
 force_alphabetical_sort_within_sections = true
 
 [tool.pytest.ini_options]
```

### Comparing `flask-mod-auth-gssapi-0.2.0/tox.ini` & `flask-mod-auth-gssapi-0.3.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 [tox]
-envlist = lint,format,security,covclean,{py36,py37,py38,py39}-unittest,covreport
+envlist = lint,format,security,covclean,{py38,py39,py310,py311}-unittest,covreport
 isolated_build = true
-requires =
-    poetry
-    tox-poetry
 
 [testenv]
 passenv = HOME
 sitepackages = false
+skip_install = true
+# Use allowlist for poetry when poetry 1.2+ is more widespread
+# allowlist_externals =
+#     poetry
+deps =
+    poetry>=1.2
+commands_pre =
+    poetry install
 commands =
-    unittest: pytest -vv --cov --cov-append --cov-report= tests {posargs}
+    unittest: poetry run pytest -vv --cov --cov-append --cov-report= tests {posargs}
 depends =
-    {py36,py37,py38,py39}: covclean
-    covreport: py36-unittest,py37-unittest,py38-unittest,py39-unittest
+    {py38,py39,py310,py311}: covclean
+    covreport: py38-unittest,py39-unittest,py310-unittest,py311-unittest
 
 [testenv:covreport]
 basepython = python3.9
 commands =
-    -coverage html
-    coverage report -m
+    -poetry run coverage html
+    poetry run coverage report -m
 
 [testenv:covclean]
-commands = coverage erase
+commands = poetry run coverage erase
 
 
 [testenv:lint]
 commands =
-    flake8 {posargs}
+    poetry run flake8 {posargs}
 
 [testenv:format]
 commands =
-    black --check {posargs:.}
-    isort --check {posargs:.}
+    poetry run black --check {posargs:.}
+    poetry run isort --check {posargs:.}
 
 [testenv:security]
 commands =
-    bandit -r flask_mod_auth_gssapi/ -x tests/ -ll
+    poetry run bandit -r flask_mod_auth_gssapi/ -x tests/ -ll
 
 
 [flake8]
 show-source = True
 max-line-length = 100
 exclude = .git,.tox,dist,*egg
```

### Comparing `flask-mod-auth-gssapi-0.2.0/setup.py` & `flask-mod-auth-gssapi-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['flask<3.0.0', 'gssapi>=1.6.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'flask-mod-auth-gssapi',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': "A Flask extention to make use of the authentication provided by the mod_auth_gssapi extention of Apache's HTTPd.",
     'long_description': "# Flask Mod Auth GSSAPI\n\n\nA Flask extention to make use of the authentication provided by the\n[mod_auth_gssapi](https://github.com/gssapi/mod_auth_gssapi) extention of\nApache's HTTPd. See [FASJSON](https://github.com/fedora-infra/fasjson) for a\nusage example.\n",
     'author': 'Fedora Infrastructure',
     'author_email': 'admin@fedoraproject.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fedora-infra/flask-mod-auth-gssapi',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
+    'python_requires': '>=3.8.0,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `flask-mod-auth-gssapi-0.2.0/PKG-INFO` & `flask-mod-auth-gssapi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: flask-mod-auth-gssapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Flask extention to make use of the authentication provided by the mod_auth_gssapi extention of Apache's HTTPd.
 Home-page: https://github.com/fedora-infra/flask-mod-auth-gssapi
 License: MIT
 Keywords: security,web
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: flask (<3.0.0)
 Requires-Dist: gssapi (>=1.6.2,<2.0.0)
 Project-URL: Repository, https://github.com/fedora-infra/flask-mod-auth-gssapi
```


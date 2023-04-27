# Comparing `tmp/Flask-HTTPAuth-4.7.0.tar.gz` & `tmp/Flask-HTTPAuth-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-HTTPAuth-4.7.0.tar", last modified: Sun May 29 14:32:23 2022, max compression
+gzip compressed data, was "Flask-HTTPAuth-4.8.0.tar", last modified: Thu Apr 27 09:23:58 2023, max compression
```

## Comparing `Flask-HTTPAuth-4.7.0.tar` & `Flask-HTTPAuth-4.8.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.309747 Flask-HTTPAuth-4.7.0/
--rw-r--r--   0 mgrinberg   (502) staff       (20)       96 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/AUTHORS
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       80 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2862 2022-05-29 14:32:23.309990 Flask-HTTPAuth-4.7.0/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2158 2021-02-21 13:13:02.000000 Flask-HTTPAuth-4.7.0/README.md
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.205614 Flask-HTTPAuth-4.7.0/docs/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6794 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/Makefile
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.193558 Flask-HTTPAuth-4.7.0/docs/_build/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.207851 Flask-HTTPAuth-4.7.0/docs/_build/doctrees/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    20237 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 mgrinberg   (502) staff       (20)   109607 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/doctrees/index.doctree
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.216812 Flask-HTTPAuth-4.7.0/docs/_build/html/
--rw-r--r--   0 mgrinberg   (502) staff       (20)      230 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/.buildinfo
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.217748 Flask-HTTPAuth-4.7.0/docs/_build/html/_sources/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    21113 2020-04-26 16:46:49.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.237899 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    12261 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/basic.css
--rw-r--r--   0 mgrinberg   (502) staff       (20)     9354 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)      350 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)      286 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/file.png
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4534 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/flasky.css
--rw-r--r--   0 mgrinberg   (502) staff       (20)      550 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/index.html
--rw-r--r--   0 mgrinberg   (502) staff       (20)   280364 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/jquery-3.4.1.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)    88145 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/jquery.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10847 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5848 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/logo.png
--rw-r--r--   0 mgrinberg   (502) staff       (20)       90 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 mgrinberg   (502) staff       (20)       90 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4395 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 mgrinberg   (502) staff       (20)    16323 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)    35168 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)    12140 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/_static/underscore.js
--rw-r--r--   0 mgrinberg   (502) staff       (20)     8280 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/genindex.html
--rw-r--r--   0 mgrinberg   (502) staff       (20)    61059 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/index.html
--rw-r--r--   0 mgrinberg   (502) staff       (20)      531 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/objects.inv
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1822 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1921 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/search.html
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5152 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.7.0/docs/_build/html/searchindex.js
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.240757 Flask-HTTPAuth-4.7.0/docs/_static/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      550 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_static/index.html
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     5848 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_static/logo.png
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.246624 Flask-HTTPAuth-4.7.0/docs/_themes/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     1789 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/LICENSE
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     1093 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/README
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.256111 Flask-HTTPAuth-4.7.0/docs/_themes/flask/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      693 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask/layout.html
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      590 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask/relations.html
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.257921 Flask-HTTPAuth-4.7.0/docs/_themes/flask/static/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     9062 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask/static/flasky.css_t
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      164 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.260290 Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      683 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.261542 Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/static/
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     4609 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/static/flasky.css_t
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)      184 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/theme.conf
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)     4875 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/_themes/flask_theme_support.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     8168 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/conf.py
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)    20031 2022-04-20 23:33:23.000000 Flask-HTTPAuth-4.7.0/docs/index.rst
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6717 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/docs/make.bat
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-07 11:04:02.000000 Flask-HTTPAuth-4.7.0/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      821 2022-05-29 14:32:23.311262 Flask-HTTPAuth-4.7.0/setup.cfg
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-07 11:04:02.000000 Flask-HTTPAuth-4.7.0/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.263218 Flask-HTTPAuth-4.7.0/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.272248 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2862 2022-05-29 14:32:22.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2207 2022-05-29 14:32:23.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2022-05-29 14:32:22.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 10:54:57.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)        6 2022-05-29 14:32:23.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       15 2022-05-29 14:32:23.000000 Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/top_level.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)    15820 2022-05-26 22:45:50.000000 Flask-HTTPAuth-4.7.0/src/flask_httpauth.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-05-29 14:32:23.308356 Flask-HTTPAuth-4.7.0/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/tests/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2418 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/tests/test_basic_custom_realm.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2280 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/tests/test_basic_get_password.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2215 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/tests/test_basic_hashed_password.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3749 2022-05-26 22:59:19.000000 Flask-HTTPAuth-4.7.0/tests/test_basic_verify_password.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3325 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.7.0/tests/test_basic_verify_password_async.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2224 2022-04-20 10:45:22.000000 Flask-HTTPAuth-4.7.0/tests/test_digest_custom_realm.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10478 2022-04-20 23:24:14.000000 Flask-HTTPAuth-4.7.0/tests/test_digest_get_password.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2425 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.7.0/tests/test_digest_ha1_password.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     7910 2022-04-20 10:45:22.000000 Flask-HTTPAuth-4.7.0/tests/test_digest_no_qop.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1355 2020-11-16 10:28:40.000000 Flask-HTTPAuth-4.7.0/tests/test_error_responses.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6107 2021-05-01 14:19:05.000000 Flask-HTTPAuth-4.7.0/tests/test_multi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6268 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.7.0/tests/test_multi_async.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5321 2020-04-22 23:14:09.000000 Flask-HTTPAuth-4.7.0/tests/test_roles.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5470 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.7.0/tests/test_roles_async.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6036 2020-04-26 17:46:00.000000 Flask-HTTPAuth-4.7.0/tests/test_token.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6185 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.7.0/tests/test_token_async.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.643485 Flask-HTTPAuth-4.8.0/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       96 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/AUTHORS
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       80 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/MANIFEST.in
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2862 2023-04-27 09:23:58.643731 Flask-HTTPAuth-4.8.0/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2158 2021-02-21 13:13:02.000000 Flask-HTTPAuth-4.8.0/README.md
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.504001 Flask-HTTPAuth-4.8.0/docs/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6794 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/Makefile
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.492710 Flask-HTTPAuth-4.8.0/docs/_build/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.506204 Flask-HTTPAuth-4.8.0/docs/_build/doctrees/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    20237 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 mgrinberg   (502) staff       (20)   109607 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/doctrees/index.doctree
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.514191 Flask-HTTPAuth-4.8.0/docs/_build/html/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      230 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/.buildinfo
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.515215 Flask-HTTPAuth-4.8.0/docs/_build/html/_sources/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    21113 2020-04-26 16:46:49.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.534274 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    12261 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/basic.css
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     9354 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      350 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      286 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4534 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/flasky.css
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      550 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/index.html
+-rw-r--r--   0 mgrinberg   (502) staff       (20)   280364 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/jquery-3.4.1.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    88145 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10847 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5848 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/logo.png
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       90 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       90 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4395 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    16323 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    35168 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    12140 2020-04-26 16:30:59.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     8280 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/genindex.html
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    61059 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/index.html
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      531 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/objects.inv
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1822 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/py-modindex.html
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1921 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/search.html
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5152 2020-04-26 16:47:02.000000 Flask-HTTPAuth-4.8.0/docs/_build/html/searchindex.js
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.536553 Flask-HTTPAuth-4.8.0/docs/_static/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      550 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_static/index.html
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     5848 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_static/logo.png
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.539763 Flask-HTTPAuth-4.8.0/docs/_themes/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     1789 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/LICENSE
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     1093 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/README
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.544014 Flask-HTTPAuth-4.8.0/docs/_themes/flask/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      693 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask/layout.html
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      590 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask/relations.html
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.547090 Flask-HTTPAuth-4.8.0/docs/_themes/flask/static/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     9062 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask/static/flasky.css_t
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      164 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.559464 Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      683 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.561649 Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/static/
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     4609 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/static/flasky.css_t
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)      184 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/theme.conf
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)     4875 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     8168 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/conf.py
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)    20172 2023-02-11 11:54:52.000000 Flask-HTTPAuth-4.8.0/docs/index.rst
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6717 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/docs/make.bat
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-07 11:04:02.000000 Flask-HTTPAuth-4.8.0/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      821 2023-04-27 09:23:58.644735 Flask-HTTPAuth-4.8.0/setup.cfg
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-07 11:04:02.000000 Flask-HTTPAuth-4.8.0/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.563179 Flask-HTTPAuth-4.8.0/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.574359 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2862 2023-04-27 09:23:58.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2207 2023-04-27 09:23:58.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-27 09:23:58.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 10:54:57.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        6 2023-04-27 09:23:58.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       15 2023-04-27 09:23:58.000000 Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/top_level.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    15836 2023-04-27 08:56:16.000000 Flask-HTTPAuth-4.8.0/src/flask_httpauth.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-27 09:23:58.642517 Flask-HTTPAuth-4.8.0/tests/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/tests/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2418 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/tests/test_basic_custom_realm.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2280 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/tests/test_basic_get_password.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2215 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/tests/test_basic_hashed_password.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3749 2022-05-26 22:59:19.000000 Flask-HTTPAuth-4.8.0/tests/test_basic_verify_password.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3325 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.8.0/tests/test_basic_verify_password_async.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2224 2022-04-20 10:45:22.000000 Flask-HTTPAuth-4.8.0/tests/test_digest_custom_realm.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10478 2022-04-20 23:24:14.000000 Flask-HTTPAuth-4.8.0/tests/test_digest_get_password.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2425 2020-04-19 16:49:09.000000 Flask-HTTPAuth-4.8.0/tests/test_digest_ha1_password.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     7910 2022-04-20 10:45:22.000000 Flask-HTTPAuth-4.8.0/tests/test_digest_no_qop.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1355 2020-11-16 10:28:40.000000 Flask-HTTPAuth-4.8.0/tests/test_error_responses.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6101 2023-04-26 23:15:46.000000 Flask-HTTPAuth-4.8.0/tests/test_multi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6262 2023-04-26 23:16:04.000000 Flask-HTTPAuth-4.8.0/tests/test_multi_async.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5321 2020-04-22 23:14:09.000000 Flask-HTTPAuth-4.8.0/tests/test_roles.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5470 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.8.0/tests/test_roles_async.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6036 2023-04-26 23:35:54.000000 Flask-HTTPAuth-4.8.0/tests/test_token.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6185 2022-01-22 19:18:14.000000 Flask-HTTPAuth-4.8.0/tests/test_token_async.py
```

### Comparing `Flask-HTTPAuth-4.7.0/LICENSE` & `Flask-HTTPAuth-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/PKG-INFO` & `Flask-HTTPAuth-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-HTTPAuth
-Version: 4.7.0
+Version: 4.8.0
 Summary: HTTP authentication for Flask routes
 Home-page: https://github.com/miguelgrinberg/flask-httpauth
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-httpauth/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-HTTPAuth-4.7.0/README.md` & `Flask-HTTPAuth-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/Makefile` & `Flask-HTTPAuth-4.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/doctrees/environment.pickle` & `Flask-HTTPAuth-4.8.0/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/doctrees/index.doctree` & `Flask-HTTPAuth-4.8.0/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_sources/index.rst.txt` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/basic.css` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/doctools.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/flasky.css` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/flasky.css`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/index.html` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/index.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/jquery-3.4.1.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/jquery.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/language_data.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/logo.png` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/pygments.css` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/searchtools.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/underscore-1.3.1.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/_static/underscore.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/genindex.html` & `Flask-HTTPAuth-4.8.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/index.html` & `Flask-HTTPAuth-4.8.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/objects.inv` & `Flask-HTTPAuth-4.8.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/py-modindex.html` & `Flask-HTTPAuth-4.8.0/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/search.html` & `Flask-HTTPAuth-4.8.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_build/html/searchindex.js` & `Flask-HTTPAuth-4.8.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_static/index.html` & `Flask-HTTPAuth-4.8.0/docs/_static/index.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_static/logo.png` & `Flask-HTTPAuth-4.8.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/LICENSE` & `Flask-HTTPAuth-4.8.0/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/README` & `Flask-HTTPAuth-4.8.0/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask/layout.html` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask/relations.html` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask/static/flasky.css_t` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/layout.html` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask_small/static/flasky.css_t` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/_themes/flask_theme_support.py` & `Flask-HTTPAuth-4.8.0/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/conf.py` & `Flask-HTTPAuth-4.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/docs/index.rst` & `Flask-HTTPAuth-4.8.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
     If this callback is defined, it is also invoked when the request does not have the ``Authorization`` header with user credentials, and in this case both the ``username`` and ``password`` arguments are set to empty strings. The application can opt to return ``True`` in this case and that will allow anonymous users access to the route. The callback function can indicate that the user is anonymous by writing a state variable to ``flask.g`` or by checking if ``auth.current_user()`` is ``None``.
 
     Note that when a ``verify_password`` callback is provided the ``get_password`` and ``hash_password`` callbacks are not used.
 
   .. method:: get_user_roles(roles_callback)
 
-    If defined, this callback function will be called by the framework to obtain the roles assigned to a given user. The callback function takes a single argument, the user for which roles are requested. The user object passed to this function will be the one returned by the ``verify_callback`` function. The function should return the role or list of roles that belong to the user. Example::
+    If defined, this callback function will be called by the framework to obtain the roles assigned to a given user. The callback function takes a single argument, the user for which roles are requested. The user object passed to this function will be the one returned by the "verify" callback. If the verify callback returned ``True`` instead of a user object, then the ``Authorization`` object provided by Flask will be passed to this function. The function should return the role or list of roles that belong to the user. Example::
 
       @auth.get_user_roles
       def get_user_roles(user):
           return user.get_roles()
 
   .. method:: get_password(password_callback)
```

### Comparing `Flask-HTTPAuth-4.7.0/docs/make.bat` & `Flask-HTTPAuth-4.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/setup.cfg` & `Flask-HTTPAuth-4.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Flask-HTTPAuth
-version = 4.7.0
+version = 4.8.0
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = HTTP authentication for Flask routes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/flask-httpauth
 project_urls =
```

### Comparing `Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/PKG-INFO` & `Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-HTTPAuth
-Version: 4.7.0
+Version: 4.8.0
 Summary: HTTP authentication for Flask routes
 Home-page: https://github.com/miguelgrinberg/flask-httpauth
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-httpauth/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-HTTPAuth-4.7.0/src/Flask_HTTPAuth.egg-info/SOURCES.txt` & `Flask-HTTPAuth-4.8.0/src/Flask_HTTPAuth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/src/flask_httpauth.py` & `Flask-HTTPAuth-4.8.0/src/flask_httpauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,30 +72,32 @@
     def authenticate_header(self):
         return '{0} realm="{1}"'.format(self.scheme, self.realm)
 
     def get_auth(self):
         auth = None
         if self.header is None or self.header == 'Authorization':
             auth = request.authorization
-            if auth is None and 'Authorization' in request.headers:
-                # Flask/Werkzeug do not recognize any authentication types
-                # other than Basic or Digest, so here we parse the header by
-                # hand
+            if auth is None and \
+                    'Authorization' in request.headers:  # pragma: no cover
+                # Flask/Werkzeug versions before 2.3 do not recognize any
+                # authentication types other than Basic or Digest, so here we
+                # parse the header by hand
                 try:
                     auth_type, token = request.headers['Authorization'].split(
                         None, 1)
-                    auth = Authorization(auth_type, {'token': token})
+                    auth = Authorization(auth_type)
+                    auth.token = token
                 except (ValueError, KeyError):
                     # The Authorization header is either empty or has no token
                     pass
         elif self.header in request.headers:
             # using a custom header, so the entire value of the header is
             # assumed to be a token
-            auth = Authorization(self.scheme,
-                                 {'token': request.headers[self.header]})
+            auth = Authorization(self.scheme)
+            auth.token = request.headers[self.header]
 
         # if the auth type does not match, we act as if there is no auth
         # this is better than failing directly, as it allows the callback
         # to handle special cases, like supporting multiple auth types
         if auth is not None and auth.type.lower() != self.scheme.lower():
             auth = None
 
@@ -351,16 +353,16 @@
                 opaque)
 
     def authenticate(self, auth, stored_password_or_ha1):
         if not auth or not auth.username or not auth.realm or not auth.uri \
                 or not auth.nonce or not auth.response \
                 or not stored_password_or_ha1:
             return False
-        if not(self.verify_nonce_callback(auth.nonce)) or \
-                not(self.verify_opaque_callback(auth.opaque)):
+        if not self.verify_nonce_callback(auth.nonce) or \
+                not self.verify_opaque_callback(auth.opaque):
             return False
         if auth.qop and auth.qop not in self.qop:  # pragma: no cover
             return False
         if self.use_ha1_pw:
             ha1 = stored_password_or_ha1
         else:
             a1 = auth.username + ":" + auth.realm + ":" + \
@@ -387,18 +389,15 @@
         self.verify_token_callback = None
 
     def verify_token(self, f):
         self.verify_token_callback = f
         return f
 
     def authenticate(self, auth, stored_password):
-        if auth:
-            token = auth['token']
-        else:
-            token = ""
+        token = getattr(auth, 'token', '')
         if self.verify_token_callback:
             return self.ensure_sync(self.verify_token_callback)(token)
 
 
 class MultiAuth(object):
     def __init__(self, main_auth, *args):
         self.main_auth = main_auth
```

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_basic_custom_realm.py` & `Flask-HTTPAuth-4.8.0/tests/test_basic_custom_realm.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_basic_get_password.py` & `Flask-HTTPAuth-4.8.0/tests/test_basic_get_password.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_basic_hashed_password.py` & `Flask-HTTPAuth-4.8.0/tests/test_basic_hashed_password.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_basic_verify_password.py` & `Flask-HTTPAuth-4.8.0/tests/test_basic_verify_password.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_basic_verify_password_async.py` & `Flask-HTTPAuth-4.8.0/tests/test_basic_verify_password_async.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_digest_custom_realm.py` & `Flask-HTTPAuth-4.8.0/tests/test_digest_custom_realm.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_digest_get_password.py` & `Flask-HTTPAuth-4.8.0/tests/test_digest_get_password.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_digest_ha1_password.py` & `Flask-HTTPAuth-4.8.0/tests/test_digest_ha1_password.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_digest_no_qop.py` & `Flask-HTTPAuth-4.8.0/tests/test_digest_no_qop.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_error_responses.py` & `Flask-HTTPAuth-4.8.0/tests/test_error_responses.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_multi.py` & `Flask-HTTPAuth-4.8.0/tests/test_multi.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,29 +26,29 @@
 
         @token_auth.verify_token
         def verify_token(token):
             return token == 'this-is-the-token!'
 
         @token_auth.get_user_roles
         def get_token_role(auth):
-            if auth['token'] == 'this-is-the-token!':
+            if auth.token == 'this-is-the-token!':
                 return 'foo'
             return
 
         @token_auth.error_handler
         def error_handler():
             return 'error', 401, {'WWW-Authenticate': 'MyToken realm="Foo"'}
 
         @custom_token_auth.verify_token
         def verify_custom_token(token):
             return token == 'this-is-the-custom-token!'
 
         @custom_token_auth.get_user_roles
         def get_custom_token_role(auth):
-            if auth['token'] == 'this-is-the-custom-token!':
+            if auth.token == 'this-is-the-custom-token!':
                 return 'foo'
             return
 
         @app.route('/')
         def index():
             return 'index'
```

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_multi_async.py` & `Flask-HTTPAuth-4.8.0/tests/test_multi_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,29 +29,29 @@
 
         @token_auth.verify_token
         async def verify_token(token):
             return token == 'this-is-the-token!'
 
         @token_auth.get_user_roles
         async def get_token_role(auth):
-            if auth['token'] == 'this-is-the-token!':
+            if auth.token == 'this-is-the-token!':
                 return 'foo'
             return
 
         @token_auth.error_handler
         async def error_handler():
             return 'error', 401, {'WWW-Authenticate': 'MyToken realm="Foo"'}
 
         @custom_token_auth.verify_token
         async def verify_custom_token(token):
             return token == 'this-is-the-custom-token!'
 
         @custom_token_auth.get_user_roles
         async def get_custom_token_role(auth):
-            if auth['token'] == 'this-is-the-custom-token!':
+            if auth.token == 'this-is-the-custom-token!':
                 return 'foo'
             return
 
         @app.route('/')
         async def index():
             return 'index'
```

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_roles.py` & `Flask-HTTPAuth-4.8.0/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_roles_async.py` & `Flask-HTTPAuth-4.8.0/tests/test_roles_async.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_token.py` & `Flask-HTTPAuth-4.8.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `Flask-HTTPAuth-4.7.0/tests/test_token_async.py` & `Flask-HTTPAuth-4.8.0/tests/test_token_async.py`

 * *Files identical despite different names*


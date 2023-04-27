# Comparing `tmp/edgetest-conda-2022.7.1.tar.gz` & `tmp/edgetest-conda-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-conda-2022.7.1.tar", last modified: Mon Jul 18 17:06:27 2022, max compression
+gzip compressed data, was "edgetest-conda-2023.4.0.tar", last modified: Thu Apr 27 15:46:39 2023, max compression
```

## Comparing `edgetest-conda-2022.7.1.tar` & `edgetest-conda-2023.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 17:06:27.574059 edgetest-conda-2022.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-07-18 17:06:27.574059 edgetest-conda-2022.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 17:06:27.574059 edgetest-conda-2022.7.1/edgetest_conda/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/edgetest_conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/edgetest_conda/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 17:06:27.574059 edgetest-conda-2022.7.1/edgetest_conda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 17:06:21.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-18 17:06:27.000000 edgetest-conda-2022.7.1/edgetest_conda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-07-18 17:06:27.578059 edgetest-conda-2022.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 17:06:27.574059 edgetest-conda-2022.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11576 2022-07-18 17:05:47.000000 edgetest-conda-2022.7.1/tests/test_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:46:39.159855 edgetest-conda-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-27 15:46:39.159855 edgetest-conda-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:46:39.155856 edgetest-conda-2023.4.0/edgetest_conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/edgetest_conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/edgetest_conda/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:46:39.159855 edgetest-conda-2023.4.0/edgetest_conda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:46:12.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 15:46:39.000000 edgetest-conda-2023.4.0/edgetest_conda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-27 15:46:39.159855 edgetest-conda-2023.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:46:39.159855 edgetest-conda-2023.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-04-27 15:46:06.000000 edgetest-conda-2023.4.0/tests/test_hook.py
```

### Comparing `edgetest-conda-2022.7.1/LICENSE` & `edgetest-conda-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-conda-2022.7.1/PKG-INFO` & `edgetest-conda-2023.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest-conda
-Version: 2022.7.1
+Version: 2023.4.0
 Summary: Conda edgetest plugin
 Home-page: https://github.com/capitalone/edgetest-conda
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 Project-URL: Documentation, https://capitalone.github.io/edgetest-conda
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `edgetest-conda-2022.7.1/README.md` & `edgetest-conda-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `edgetest-conda-2022.7.1/edgetest_conda/plugin.py` & `edgetest-conda-2023.4.0/edgetest_conda/plugin.py`

 * *Files identical despite different names*

### Comparing `edgetest-conda-2022.7.1/edgetest_conda.egg-info/PKG-INFO` & `edgetest-conda-2023.4.0/edgetest_conda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest-conda
-Version: 2022.7.1
+Version: 2023.4.0
 Summary: Conda edgetest plugin
 Home-page: https://github.com/capitalone/edgetest-conda
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 Project-URL: Documentation, https://capitalone.github.io/edgetest-conda
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `edgetest-conda-2022.7.1/setup.cfg` & `edgetest-conda-2023.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	edgetest
+	edgetest>=2022.3.0
 
 [options.extras_require]
 docs = 
 	furo
 	sphinx
 	sphinx-copybutton
 	sphinx-tabs
@@ -79,15 +80,15 @@
 	bumpver
 
 [options.entry_points]
 edgetest = 
 	conda = edgetest_conda.plugin
 
 [bumpver]
-current_version = "2022.7.1"
+current_version = "2023.4.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
@@ -112,15 +113,15 @@
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 88
 
 [mypy]
-python_version = 3.7
+python_version = 3.9
 warn_return_any = True
 warn_unused_configs = True
 ignore_missing_imports = True
 allow_redefinition = True
 
 [pylint]
 pylint_minimum_score = 9.5
```

### Comparing `edgetest-conda-2022.7.1/tests/test_hook.py` & `edgetest-conda-2023.4.0/tests/test_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 """
 
 
 @pytest.mark.parametrize("config", [CFG, CFG_NOCONDA])
 def test_addoption(config, tmpdir):
     """Test the addoption hook."""
     location = tmpdir.mkdir("mylocation")
-    conf_loc = Path(str(location), "myconfig.ini")
+    conf_loc = Path(str(location), "myconfig.cfg")
     with open(conf_loc, "w") as outfile:
         outfile.write(config)
 
     schema = Schema()
     addoption(schema=schema)
 
     cfg = parse_cfg(filename=conf_loc)
@@ -121,18 +121,18 @@
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
 
     runner = CliRunner()
 
     with runner.isolated_filesystem() as loc:
-        with open("config.ini", "w") as outfile:
+        with open("config.cfg", "w") as outfile:
             outfile.write(CFG)
 
-        result = runner.invoke(cli, ["--config=config.ini"])
+        result = runner.invoke(cli, ["--config=config.cfg"])
 
     assert result.exit_code == 0
 
     env_loc = str(Path(loc) / ".edgetest" / "myenv")
     if platform.system() == "Windows":
         py_loc = str(Path(env_loc) / "Scripts" / "python")
     else:
@@ -194,18 +194,18 @@
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
 
     runner = CliRunner()
 
     with runner.isolated_filesystem() as loc:
-        with open("config.ini", "w") as outfile:
+        with open("config.cfg", "w") as outfile:
             outfile.write(CFG)
 
-        result = runner.invoke(cli, ["--config=config.ini"])
+        result = runner.invoke(cli, ["--config=config.cfg"])
 
     assert result.exit_code == 0
 
     env_loc = str(Path(loc) / ".edgetest" / "myenv")
     if platform.system() == "Windows":
         py_loc = str(Path(env_loc) / "Scripts" / "python")
     else:
@@ -261,18 +261,18 @@
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
 
     runner = CliRunner()
 
     with runner.isolated_filesystem() as loc:
-        with open("config.ini", "w") as outfile:
+        with open("config.cfg", "w") as outfile:
             outfile.write(CFG)
 
-        result = runner.invoke(cli, ["--config=config.ini"])
+        result = runner.invoke(cli, ["--config=config.cfg"])
 
     assert result.exit_code == 0
 
     env_loc = str(Path(loc) / ".edgetest" / "myenv")
     if platform.system() == "Windows":
         py_loc = str(Path(env_loc) / "Scripts" / "python")
     else:
@@ -334,18 +334,18 @@
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
 
     runner = CliRunner()
 
     with runner.isolated_filesystem() as loc:
-        with open("config.ini", "w") as outfile:
+        with open("config.cfg", "w") as outfile:
             outfile.write(CFG)
 
-        result = runner.invoke(cli, ["--config=config.ini"])
+        result = runner.invoke(cli, ["--config=config.cfg"])
 
     assert result.exit_code == 0
 
     env_loc = str(Path(loc) / ".edgetest" / "myenv")
     if platform.system() == "Windows":
         py_loc = str(Path(env_loc) / "Scripts" / "python")
     else:
```


# Comparing `tmp/miss_hit_core-0.9.37.tar.gz` & `tmp/miss_hit_core-0.9.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miss_hit_core-0.9.37.tar", last modified: Thu Mar 23 13:30:40 2023, max compression
+gzip compressed data, was "miss_hit_core-0.9.38.tar", last modified: Thu Apr 27 13:22:02 2023, max compression
```

## Comparing `miss_hit_core-0.9.37.tar` & `miss_hit_core-0.9.38.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.37/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.37/LICENSE.AGPL
--rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     6013 2022-09-18 09:39:54.000000 miss_hit_core-0.9.37/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-23 13:30:40.331223 miss_hit_core-0.9.37/miss_hit_core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.37/miss_hit_core/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.37/miss_hit_core/cfg_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21616 2022-08-21 10:02:24.000000 miss_hit_core-0.9.37/miss_hit_core/cfg_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.37/miss_hit_core/cfg_tree.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18585 2023-03-23 13:17:08.000000 miss_hit_core-0.9.37/miss_hit_core/command_line.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18974 2022-08-21 08:54:39.000000 miss_hit_core-0.9.37/miss_hit_core/config.py
--rw-r--r--   0 florian   (1000) florian   (1000)    28769 2022-09-18 10:39:23.000000 miss_hit_core-0.9.37/miss_hit_core/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)   112055 2022-09-18 10:38:40.000000 miss_hit_core-0.9.37/miss_hit_core/m_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.37/miss_hit_core/m_entity_root.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.37/miss_hit_core/m_language.py
--rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.37/miss_hit_core/m_language_builtins.py
--rw-r--r--   0 florian   (1000) florian   (1000)    63616 2022-09-18 10:33:17.000000 miss_hit_core-0.9.37/miss_hit_core/m_lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.37/miss_hit_core/m_parse_utils.py
--rw-r--r--   0 florian   (1000) florian   (1000)    81627 2022-09-18 10:33:45.000000 miss_hit_core-0.9.37/miss_hit_core/m_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.37/miss_hit_core/m_types.py
--rw-r--r--   0 florian   (1000) florian   (1000)    43076 2022-09-18 10:28:55.000000 miss_hit_core-0.9.37/miss_hit_core/mh_metric.py
--rw-r--r--   0 florian   (1000) florian   (1000)    52025 2022-09-18 10:05:58.000000 miss_hit_core-0.9.37/miss_hit_core/mh_style.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.37/miss_hit_core/pathutil.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/miss_hit_core/resources/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/miss_hit_core/resources/assets/
--rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/alert-triangle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/bar-chart-2.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/check-square.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/download.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/edit.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/external-link.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/file-text.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/help-circle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/package.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/settings.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/assets/terminal.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core/resources/style.css
--rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.37/miss_hit_core/resources.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9734 2023-03-23 13:17:08.000000 miss_hit_core-0.9.37/miss_hit_core/s_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    20285 2023-03-23 13:17:08.000000 miss_hit_core-0.9.37/miss_hit_core/s_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-03-23 13:27:17.000000 miss_hit_core-0.9.37/miss_hit_core/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8074 2023-03-23 13:17:08.000000 miss_hit_core-0.9.37/miss_hit_core/work_package.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/miss_hit_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/miss_hit_core.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-03-23 13:30:40.335223 miss_hit_core-0.9.37/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-03-23 13:30:40.000000 miss_hit_core-0.9.37/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.38/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.38/LICENSE.AGPL
+-rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     6013 2022-09-18 09:39:54.000000 miss_hit_core-0.9.38/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.38/miss_hit_core/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21616 2022-08-21 10:02:24.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_tree.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18733 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/command_line.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18974 2022-08-21 08:54:39.000000 miss_hit_core-0.9.38/miss_hit_core/config.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    28769 2022-09-18 10:39:23.000000 miss_hit_core-0.9.38/miss_hit_core/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)   112055 2022-09-18 10:38:40.000000 miss_hit_core-0.9.38/miss_hit_core/m_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.38/miss_hit_core/m_entity_root.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.38/miss_hit_core/m_language.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.38/miss_hit_core/m_language_builtins.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    63616 2022-09-18 10:33:17.000000 miss_hit_core-0.9.38/miss_hit_core/m_lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.38/miss_hit_core/m_parse_utils.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    81627 2022-09-18 10:33:45.000000 miss_hit_core-0.9.38/miss_hit_core/m_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.38/miss_hit_core/m_types.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    43076 2022-09-18 10:28:55.000000 miss_hit_core-0.9.38/miss_hit_core/mh_metric.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    52025 2022-09-18 10:05:58.000000 miss_hit_core-0.9.38/miss_hit_core/mh_style.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.38/miss_hit_core/pathutil.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core/resources/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/miss_hit_core/resources/assets/
+-rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/alert-triangle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/bar-chart-2.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/check-square.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/download.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/edit.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/external-link.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/file-text.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/help-circle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/package.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/settings.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/terminal.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/style.css
+-rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.38/miss_hit_core/resources.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9895 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/s_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    23398 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/s_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-04-27 13:21:29.000000 miss_hit_core-0.9.38/miss_hit_core/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8074 2023-03-23 13:17:08.000000 miss_hit_core-0.9.38/miss_hit_core/work_package.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/setup.py
```

### Comparing `miss_hit_core-0.9.37/LICENSE` & `miss_hit_core-0.9.38/LICENSE`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/LICENSE.AGPL` & `miss_hit_core-0.9.38/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/PKG-INFO` & `miss_hit_core-0.9.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss_hit_core
-Version: 0.9.37
+Version: 0.9.38
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.AGPL
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967056.svg)](https://doi.org/10.5281/zenodo.3967056)
 
 # MATLAB Independent, Small & Safe, High Integrity Tools
```

### Comparing `miss_hit_core-0.9.37/README.md` & `miss_hit_core-0.9.38/README.md`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/cfg_ast.py` & `miss_hit_core-0.9.38/miss_hit_core/cfg_ast.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/cfg_parser.py` & `miss_hit_core-0.9.38/miss_hit_core/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/cfg_tree.py` & `miss_hit_core-0.9.38/miss_hit_core/cfg_tree.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/command_line.py` & `miss_hit_core-0.9.38/miss_hit_core/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,19 @@
     try:
         if not wp.cfg.enabled:
             wp.mh.register_exclusion(wp.filename)
             results.append(work_package.Result(wp, False))
 
         elif isinstance(wp, work_package.SIMULINK_File_WP):
             wp.register_file()
-            wp.parse_simulink()
+            try:
+                wp.parse_simulink()
+            except errors.Error:
+                results.append(work_package.Result(wp, False))
+                return results
             if wp.n_content:
                 for block in wp.n_content.iter_all_blocks():
                     if isinstance(block, s_ast.Matlab_Function):
                         block_wp = work_package.Embedded_MATLAB_WP(wp, block)
                         block_wp.register_file()
                         results.append(process_m_fn(block_wp))
             results.append(process_s_fn(wp))
```

### Comparing `miss_hit_core-0.9.37/miss_hit_core/config.py` & `miss_hit_core-0.9.38/miss_hit_core/config.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/errors.py` & `miss_hit_core-0.9.38/miss_hit_core/errors.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_ast.py` & `miss_hit_core-0.9.38/miss_hit_core/m_ast.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_entity_root.py` & `miss_hit_core-0.9.38/miss_hit_core/m_entity_root.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_language.py` & `miss_hit_core-0.9.38/miss_hit_core/m_language.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_language_builtins.py` & `miss_hit_core-0.9.38/miss_hit_core/m_language_builtins.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_lexer.py` & `miss_hit_core-0.9.38/miss_hit_core/m_lexer.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_parse_utils.py` & `miss_hit_core-0.9.38/miss_hit_core/m_parse_utils.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_parser.py` & `miss_hit_core-0.9.38/miss_hit_core/m_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/m_types.py` & `miss_hit_core-0.9.38/miss_hit_core/m_types.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/mh_metric.py` & `miss_hit_core-0.9.38/miss_hit_core/mh_metric.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/mh_style.py` & `miss_hit_core-0.9.38/miss_hit_core/mh_style.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/pathutil.py` & `miss_hit_core-0.9.38/miss_hit_core/pathutil.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/resources/assets/package.svg` & `miss_hit_core-0.9.38/miss_hit_core/resources/assets/package.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/resources/assets/settings.svg` & `miss_hit_core-0.9.38/miss_hit_core/resources/assets/settings.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/resources/style.css` & `miss_hit_core-0.9.38/miss_hit_core/resources/style.css`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/resources.py` & `miss_hit_core-0.9.38/miss_hit_core/resources.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core/s_ast.py` & `miss_hit_core-0.9.38/miss_hit_core/s_ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,15 +289,21 @@
         super().__init__()
         assert isinstance(sid, str), "expected string, got %s" % type(sid)
         assert isinstance(text, str)
         self.sid  = sid
         self.text = text
 
     def dump_hierarchy(self, indent=0):
-        print(" " * indent, "Annotation (%s)" % repr(self.text))
+        if len(self.text) > 40:
+            text = self.text[:40] + "..."
+        else:
+            text = self.text
+        if "\n" in text:
+            text = repr(text)
+        print(" " * indent, "Annotation (%s)" % text)
 
 
 class Connector(Node):
     # This is a line, but it doesn't do anything, i.e. a comment. It
     # is used to connect an annotation to some block.
 
     # pylint: disable=abstract-method
```

### Comparing `miss_hit_core-0.9.37/miss_hit_core/s_parser.py` & `miss_hit_core-0.9.38/miss_hit_core/s_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,25 +31,57 @@
 """
 
 import os.path
 import zipfile
 import xml.etree.ElementTree as ET
 
 from abc import ABCMeta, abstractmethod
+from io import StringIO
+from html.parser import HTMLParser
 
 from miss_hit_core.config import Config
 from miss_hit_core.s_ast import *
 from miss_hit_core.errors import Message_Handler, ICE
 from miss_hit_core.m_language import MATLAB_Latest_Language
 
 # pylint: disable=invalid-name
 anatomy = {}
 # pylint: enable=invalid-name
 
 
+class HTML_Text_Extractor(HTMLParser):
+    def __init__(self):
+        super().__init__()
+        self.reset()
+        self.strict = False
+        self.convert_charrefs = True
+        self.text = ""
+        self.processing = False
+
+    def handle_starttag(self, tag, attrs):
+        if tag == "body":
+            self.processing = True
+        if not self.processing:
+            return
+        if tag == "br":
+            self.text += "\n"
+
+    def handle_endtag(self, tag):
+        if tag == "body":
+            self.processing = False
+        if not self.processing:
+            return
+        if tag in ("p", "div"):
+            self.text += "\n"
+
+    def handle_data(self, d):
+        if self.processing:
+            self.text += d
+
+
 class Simulink_Parser(metaclass=ABCMeta):
     def __init__(self, mh, filename, cfg):
         assert isinstance(mh, Message_Handler)
         assert isinstance(filename, str)
         assert isinstance(cfg, Config)
 
         self.mh       = mh
@@ -69,31 +101,41 @@
 class Simulink_SLX_Parser(Simulink_Parser):
     def __init__(self, mh, filename, cfg):
         super().__init__(mh, filename, cfg)
 
         self.xml_blockdiagram   = None
         self.xml_stateflow      = None
         self.xml_coreproperties = None
+        self.xml_ref_systems    = {}
+        self.xml_ref_stateflow  = {}
         # ETree nodes for the relevant files
 
         self.other_content = {}
         with zipfile.ZipFile(self.filename) as zfd:
             for name in zfd.namelist():
                 with zfd.open(name) as fd:
                     if name == "metadata/coreProperties.xml":
                         self.xml_coreproperties = ET.parse(fd)
                     elif name == "simulink/blockdiagram.xml":
                         self.xml_blockdiagram = ET.parse(fd)
                     elif name == "simulink/stateflow.xml":
                         self.xml_stateflow = ET.parse(fd)
+                    elif name.startswith("simulink/systems/") and \
+                         name.endswith(".xml"):
+                        sys_id = name[17:-4]
+                        self.xml_ref_systems[sys_id] = ET.parse(fd)
+                    elif name.startswith("simulink/stateflow/") and \
+                         name.endswith(".xml"):
+                        sf_id = name[19:-4]
+                        self.xml_ref_stateflow[sf_id] = ET.parse(fd)
                     else:
                         self.other_content[name] = fd.read()
-        # Read entire zipfile, storing content here. The two XML files
-        # we're interested in we already parse with ETree. The rest of
-        # the parsing happens in parse_file.
+        # Read entire zipfile, storing content here. We parse the XML
+        # files we're interested in with ETree. The rest of the
+        # parsing happens in parse_file.
 
         self.sf_names = {}
         # Dictionary for Stateflow items mapping from string names to
         # ET.Element nodes for the Stateflow charts.
 
         self.is_external_harness = False
         # Set to true once if we determine that this an external
@@ -127,14 +169,20 @@
         return properties
 
     def parse_file(self):
         # Parse stateflow XML first, since we want to refer to it from
         # the blockdiagram.
         if self.xml_stateflow:
             self.parse_stateflow(self.xml_stateflow.getroot())
+        for item in self.xml_ref_stateflow.values():
+            et_item = item.getroot()
+            if et_item.tag == "Stateflow":
+                self.parse_stateflow(et_item)
+            else:
+                self.parse_partial_stateflow(et_item)
 
         # Parse blockdiagram and return the AST.
         return self.parse_blockdiagram(self.xml_blockdiagram.getroot())
 
     def save_and_close(self):
         # Write back the (potentially modified) tree.
         with zipfile.ZipFile(self.filename, mode="w") as zfd:
@@ -143,26 +191,38 @@
                     self.xml_blockdiagram.write(fd)
             if self.xml_stateflow:
                 with zfd.open("simulink/stateflow.xml", mode="w") as fd:
                     self.xml_stateflow.write(fd)
             if self.xml_coreproperties:
                 with zfd.open("metadata/coreProperties.xml", mode="w") as fd:
                     self.xml_coreproperties.write(fd)
+            for sys_id in self.xml_ref_systems:
+                with zfd.open("simulink/systems/%s.xml" % sys_id,
+                              mode="w") as fd:
+                    self.xml_ref_systems[sys_id].write(fd)
+            for sf_id in self.xml_ref_stateflow:
+                with zfd.open("simulink/systems/%s.xml" % sf_id,
+                              mode="w") as fd:
+                    self.xml_ref_stateflow[sf_id].write(fd)
             for name in sorted(self.other_content):
                 with zfd.open(name, mode="w") as fd:
                     fd.write(self.other_content[name])
 
     def loc(self):
         return Location(self.filename,
                         blockname = "/".join(self.name_stack))
 
     ######################################################################
     # Stateflow parsing
     ######################################################################
 
+    def parse_partial_stateflow(self, et_node):
+        assert isinstance(et_node, ET.Element)
+        assert et_node.tag == "chart"
+
     def parse_stateflow(self, et_stateflow):
         assert isinstance(et_stateflow, ET.Element)
         assert et_stateflow.tag == "Stateflow"
 
         d_instances = {}
         # A dictionary for name_str -> (machine, chart)
 
@@ -224,16 +284,21 @@
                               "Unknown item %s in machine" % et_item.tag)
 
         for et_item in et_children:
             if et_item.tag == "target":
                 # TODO: Unclear what exactly this does right now.
                 pass
             elif et_item.tag == "chart":
-                chart_id = int(et_item.attrib["id"])
-                d_machine[chart_id] = et_item
+                if "Ref" in et_item.attrib:
+                    chart_node = \
+                        self.xml_ref_stateflow[et_item.attrib["Ref"]].getroot()
+                else:
+                    chart_node = et_item
+                chart_id = int(chart_node.attrib["id"])
+                d_machine[chart_id] = chart_node
             else:
                 self.mh.error(self.loc(),
                               "Unknown item %s in Children" % et_item.tag)
 
         return d_machine
 
     ######################################################################
@@ -351,22 +416,39 @@
 
         content = None
         for et_item in et_anno:
             if et_item.tag == "P" and et_item.attrib["Name"] == "Name":
                 content = et_item.text
         assert content is not None
 
+        if content.startswith("<!DOCTYPE HTML"):
+            html_parser = HTML_Text_Extractor()
+            html_parser.feed(content)
+            content = html_parser.text.strip()
+
         n_anno = Annotation(et_anno.attrib["SID"],
                             content)
         return n_anno
 
     def parse_system(self, et_system):
         assert isinstance(et_system, ET.Element)
         assert et_system.tag == "System"
 
+        if "Ref" in et_system.attrib:
+            sys_id = et_system.attrib["Ref"]
+            for et_item in et_system:
+                self.mh.error(self.loc(),
+                              "Referenced system %s contains items" %
+                              sys_id)
+            if sys_id not in self.xml_ref_systems:
+                self.mh.error(self.loc(),
+                              "Referenced system %s not contained in slx" %
+                              sys_id)
+            return self.parse_system(self.xml_ref_systems[sys_id].getroot())
+
         n_system = System()
 
         block_items = []
         line_items = []
         anno_items = []
 
         # First we go over all items, but we need to process them in a
```

### Comparing `miss_hit_core-0.9.37/miss_hit_core/version.py` & `miss_hit_core-0.9.38/miss_hit_core/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 ##                                                                          ##
 ##############################################################################
 
 # Some constants we use for tool version and URLs
 
 GITHUB_ISSUES = "https://github.com/florianschanda/miss_hit/issues"
 
-VERSION_TUPLE = (0, 9, 37)
+VERSION_TUPLE = (0, 9, 38)
 VERSION_SUFFIX = ""
 
 VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
           ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "MISS_HIT %s" % VERSION
```

### Comparing `miss_hit_core-0.9.37/miss_hit_core/work_package.py` & `miss_hit_core-0.9.38/miss_hit_core/work_package.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/miss_hit_core.egg-info/PKG-INFO` & `miss_hit_core-0.9.38/miss_hit_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss-hit-core
-Version: 0.9.37
+Version: 0.9.38
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.AGPL
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3967056.svg)](https://doi.org/10.5281/zenodo.3967056)
 
 # MATLAB Independent, Small & Safe, High Integrity Tools
```

### Comparing `miss_hit_core-0.9.37/miss_hit_core.egg-info/SOURCES.txt` & `miss_hit_core-0.9.38/miss_hit_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.37/setup.py` & `miss_hit_core-0.9.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     project_urls={
         "Bug Tracker"   : "https://github.com/florianschanda/miss_hit/issues",
         "Documentation" : "https://florianschanda.github.io/miss_hit/",
         "Source Code"   : "https://github.com/florianschanda/miss_hit",
     },
     license="GNU General Public License v3",
     packages=["miss_hit_core"],
-    python_requires=">=3.6, <4",
+    python_requires=">=3.7, <4",
     package_data = {
         "miss_hit_core": ["resources/*.css", "resources/assets/*"],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```


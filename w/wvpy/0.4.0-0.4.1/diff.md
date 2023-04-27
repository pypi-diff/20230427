# Comparing `tmp/wvpy-0.4.0.tar.gz` & `tmp/wvpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wvpy-0.4.0.tar", last modified: Tue Apr 11 19:43:16 2023, max compression
+gzip compressed data, was "wvpy-0.4.1.tar", last modified: Thu Apr 27 00:11:11 2023, max compression
```

## Comparing `wvpy-0.4.0.tar` & `wvpy-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.691479 wvpy-0.4.0/
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.687221 wvpy-0.4.0/Doc/
--rw-r--r--   0 johnmount   (501) staff       (20)      108 2019-07-23 14:11:39.000000 wvpy-0.4.0/Doc/documentation.txt
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:35:20.000000 wvpy-0.4.0/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)       82 2019-07-23 14:11:39.000000 wvpy-0.4.0/MANIFEST.in
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-11 19:43:16.691229 wvpy-0.4.0/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      373 2022-12-29 19:46:58.000000 wvpy-0.4.0/README.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-11 19:43:16.691553 wvpy-0.4.0/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-01-22 23:07:22.000000 wvpy-0.4.0/setup.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.689203 wvpy-0.4.0/wvpy/
--rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-01-22 23:07:08.000000 wvpy-0.4.0/wvpy/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)    19223 2023-04-10 19:24:30.000000 wvpy-0.4.0/wvpy/jtools.py
--rw-r--r--   0 johnmount   (501) staff       (20)     5898 2022-12-29 19:46:58.000000 wvpy-0.4.0/wvpy/pysheet.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3234 2022-12-29 19:46:58.000000 wvpy-0.4.0/wvpy/render_workbook.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.690815 wvpy-0.4.0/wvpy.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      272 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/top_level.txt
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.150036 wvpy-0.4.1/
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.145807 wvpy-0.4.1/Doc/
+-rw-r--r--   0 johnmount   (501) staff       (20)      108 2019-07-23 14:11:39.000000 wvpy-0.4.1/Doc/documentation.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:35:20.000000 wvpy-0.4.1/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)       82 2019-07-23 14:11:39.000000 wvpy-0.4.1/MANIFEST.in
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-27 00:11:11.149743 wvpy-0.4.1/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      373 2022-12-29 19:46:58.000000 wvpy-0.4.1/README.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-27 00:11:11.150116 wvpy-0.4.1/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-04-11 19:46:06.000000 wvpy-0.4.1/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.147225 wvpy-0.4.1/wvpy/
+-rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-04-11 19:46:02.000000 wvpy-0.4.1/wvpy/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    20444 2023-04-26 23:33:57.000000 wvpy-0.4.1/wvpy/jtools.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     5898 2022-12-29 19:46:58.000000 wvpy-0.4.1/wvpy/pysheet.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3234 2022-12-29 19:46:58.000000 wvpy-0.4.1/wvpy/render_workbook.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.149308 wvpy-0.4.1/wvpy.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      272 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/top_level.txt
```

### Comparing `wvpy-0.4.0/LICENSE` & `wvpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.0/PKG-INFO` & `wvpy-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `wvpy-0.4.0/setup.py` & `wvpy-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION = "Convert Jupyter notebooks to and from Python files."
 LONG_DESCRIPTION = """
 Convert Jupyter notebooks to and from Python files.
 """
 
 setuptools.setup(
     name="wvpy",
-    version="0.4.0",
+    version="0.4.1",
     author="John Mount",
     author_email="jmount@win-vector.com",
     url="https://github.com/WinVector/wvpy",
     packages=setuptools.find_packages(exclude=['tests', 'Examples']),
     install_requires=[
         "IPython",
         "nbformat",
```

### Comparing `wvpy-0.4.0/wvpy/jtools.py` & `wvpy-0.4.1/wvpy/jtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 """Jupyter tools"""
 
 import re
 import datetime
 import os
 import nbformat
-import nbconvert.preprocessors
+from nbconvert import HTMLExporter
+from nbconvert.preprocessors import ExecutePreprocessor
 from multiprocessing import Pool
 import sys
 
-from typing import Iterable, Optional
+from typing import Iterable, List, Optional
 from functools import total_ordering
 
 have_pdf_kit = False
 try:
     import pdfkit
     have_pdf_kit = True
 except ModuleNotFoundError:
@@ -241,14 +242,44 @@
     with open(ipynb_file, "rb") as f:
         nb = nbformat.read(f, as_version=4)
     py_source = convert_notebook_code_to_py(nb, use_black=use_black)
     with open(py_file, 'w') as f:
         f.write(py_source)        
 
 
+class OurExecutor(ExecutePreprocessor):
+    """Catch exception in notebook processing"""
+    def __init__(self, **kw):
+        """Initialize the preprocessor."""
+        ExecutePreprocessor.__init__(self, **kw)
+        self.caught_exception = None
+    
+    def preprocess_cell(self, cell, resources, index):
+        """
+        Override if you want to apply some preprocessing to each cell.
+        Must return modified cell and resource dictionary.
+
+        Parameters
+        ----------
+        cell : NotebookNode cell
+            Notebook cell being processed
+        resources : dictionary
+            Additional resources used in the conversion process.  Allows
+            preprocessors to pass variables into the Jinja engine.
+        index : int
+            Index of the cell being processed
+        """
+        if self.caught_exception is None:
+            try:
+                return ExecutePreprocessor.preprocess_cell(self, cell, resources, index)
+            except Exception as ex:
+                self.caught_exception = ex
+        return cell, self.resources
+
+
 # https://nbconvert.readthedocs.io/en/latest/execute_api.html
 # https://nbconvert.readthedocs.io/en/latest/nbconvert_library.html
 # HTML element we are trying to delete: 
 #   <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[5]:</div>
 def render_as_html(
     notebook_file_name: str,
     *,
@@ -325,35 +356,36 @@
     caught = None
     try:
         if verbose:
             print(
                 f'start render_as_html "{notebook_file_name}" {exec_note} {datetime.datetime.now()}'
             )
         if kernel_name is not None:
-            ep = nbconvert.preprocessors.ExecutePreprocessor(
+            ep = OurExecutor(
                 timeout=timeout, kernel_name=kernel_name
             )
         else:
-            ep = nbconvert.preprocessors.ExecutePreprocessor(timeout=timeout)
+            ep = OurExecutor(timeout=timeout)
         nb_res, nb_resources = ep.preprocess(nb)
-        html_exporter = nbconvert.HTMLExporter(exclude_input=exclude_input)
+        html_exporter = HTMLExporter(exclude_input=exclude_input)
         html_body, html_resources = html_exporter.from_notebook_node(nb_res)
         if exclude_input and (prompt_strip_regexp is not None):
             # strip output prompts
             html_body = re.sub(
                 prompt_strip_regexp,
                 ' ',
                 html_body)
         if not convert_to_pdf:
             with open(html_name, "wt") as f:
                 f.write(html_body)
         else:
             assert have_pdf_kit
             pdf_name = html_name.removesuffix('.html') + '.pdf'
             pdfkit.from_string(html_body, pdf_name)
+        caught = ep.caught_exception
     except Exception as e:
         caught = e
     if caught is not None:
         raise caught
     if verbose:
         print(f'\tdone render_as_html "{html_name}" {datetime.datetime.now()}')
 
@@ -452,42 +484,43 @@
         ])
         return 'JTask(\n' + args_str + ",\n)"
 
     def __repr__(self) -> str:
         return self.__str__()
 
 
-def job_fn(arg: JTask) -> None:
+def job_fn(arg: JTask):
     """
-    Function to run a JTask job
+    Function to run a JTask job. Exceptions pass through
     """
     assert isinstance(arg, JTask)
     # render notebook
-    arg.render_as_html()
+    return arg.render_as_html()
 
 
-def job_fn_eat_exception(arg: JTask) -> None:
+def job_fn_eat_exception(arg: JTask):
     """
-    Function to run a JTask job, eating any exception
+    Function to run a JTask job, catching any exception and returning it as a value
     """
     assert isinstance(arg, JTask)
     # render notebook
     try:
-        arg.render_as_html()
+        return arg.render_as_html()
     except Exception as e:
         print(f"{arg} caught {e}")
+        return (arg, e)
 
 
 def run_pool(
         tasks: Iterable, 
         *, 
         njobs: int = 4,
         verbose: bool = True,
         stop_on_error: bool = True,
-        ) -> None:
+        ) -> List:
     """
     Run a pool of tasks.
 
     :param tasks: iterable of tasks
     :param njobs: degree of parallelism
     :param verbose: if True, print on failure
     :param stop_on_error: if True, stop pool on error
@@ -502,23 +535,24 @@
     for task in tasks:
         assert isinstance(task, JTask)
     if stop_on_error:
         # # complex way, allowing a stop on job failure
         # https://stackoverflow.com/a/25791961/6901725
         with Pool(njobs) as pool:
             try:
-                list(pool.imap_unordered(job_fn, tasks))  # list is forcing iteration over tasks for side-effects
+                res = list(pool.imap_unordered(job_fn, tasks))  # list is forcing iteration over tasks for side-effects
             except Exception:
                 if verbose:
                     sys.stdout.flush()
                     print("!!! run_pool: a worker raised an Exception, aborting...")
                     sys.stdout.flush()
                 pool.close()
                 pool.terminate()
                 raise  # re-raise Exception
             else:
                 pool.close()
                 pool.join()
     else:
         # simple way, but doesn't exit until all jobs succeed or fail
         with Pool(njobs) as pool:
-            pool.map(job_fn_eat_exception, tasks)
+            res = list(pool.map(job_fn_eat_exception, tasks))
+        return res
```

### Comparing `wvpy-0.4.0/wvpy/pysheet.py` & `wvpy-0.4.1/wvpy/pysheet.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.0/wvpy/render_workbook.py` & `wvpy-0.4.1/wvpy/render_workbook.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.0/wvpy.egg-info/PKG-INFO` & `wvpy-0.4.1/wvpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```


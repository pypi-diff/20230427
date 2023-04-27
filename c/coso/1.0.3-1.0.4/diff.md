# Comparing `tmp/coso-1.0.3.tar.gz` & `tmp/coso-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.0.3.tar", last modified: Wed Apr 19 14:00:04 2023, max compression
+gzip compressed data, was "coso-1.0.4.tar", last modified: Wed Apr 26 13:34:46 2023, max compression
```

## Comparing `coso-1.0.3.tar` & `coso-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.718850 coso-1.0.3/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-19 14:00:04.718500 coso-1.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.710328 coso-1.0.3/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      559 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-19 14:00:04.000000 coso-1.0.3/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-19 14:00:04.719054 coso-1.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1078 2023-04-19 13:58:42.000000 coso-1.0.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.716443 coso-1.0.3/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 14:00:04.717553 coso-1.0.3/src/VisCoSo/
--rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.3/src/VisCoSo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.0.3/src/VisCoSo/header.html
--rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.0.3/src/VisCoSo/viscoso.css
--rwxrwxrwx   0 root         (0) root         (0)   113187 2023-04-19 13:32:47.000000 coso-1.0.3/src/VisCoSo/viscoso.html
--rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.3/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.3/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.3/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.3/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15930 2023-04-12 10:50:48.000000 coso-1.0.3/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)     2003 2023-04-19 13:48:19.000000 coso-1.0.3/src/launcher.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.3/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.3/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8708 2023-04-12 10:37:47.000000 coso-1.0.3/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.3/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.3/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.3/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.3/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.3/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14336 2023-04-19 12:40:45.000000 coso-1.0.3/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.3/src/venn.py
--rwxrwxrwx   0 root         (0) root         (0)    20228 2023-04-19 13:59:50.000000 coso-1.0.3/src/viscoso.py
--rwxrwxrwx   0 root         (0) root         (0)     3394 2023-04-19 12:40:33.000000 coso-1.0.3/src/viscoso_widget.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-26 13:34:46.586231 coso-1.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-26 13:34:46.584858 coso-1.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-26 13:34:46.519569 coso-1.0.4/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-26 13:34:46.000000 coso-1.0.4/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      559 2023-04-26 13:34:46.000000 coso-1.0.4/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-26 13:34:46.000000 coso-1.0.4/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-26 13:34:46.000000 coso-1.0.4/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-26 13:34:46.000000 coso-1.0.4/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.4/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-26 13:34:46.586725 coso-1.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1078 2023-04-26 13:32:28.000000 coso-1.0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-26 13:34:46.569650 coso-1.0.4/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-26 13:34:46.578419 coso-1.0.4/src/VisCoSo/
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.4/src/VisCoSo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.0.4/src/VisCoSo/header.html
+-rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.0.4/src/VisCoSo/viscoso.css
+-rwxrwxrwx   0 root         (0) root         (0)   113187 2023-04-19 13:32:47.000000 coso-1.0.4/src/VisCoSo/viscoso.html
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.4/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.4/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.4/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.4/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15930 2023-04-12 10:50:48.000000 coso-1.0.4/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)     2003 2023-04-19 13:48:19.000000 coso-1.0.4/src/launcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.4/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.4/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8708 2023-04-12 10:37:47.000000 coso-1.0.4/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.4/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.4/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.4/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.4/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.4/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14336 2023-04-19 12:40:45.000000 coso-1.0.4/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.4/src/venn.py
+-rwxrwxrwx   0 root         (0) root         (0)    20228 2023-04-19 13:59:50.000000 coso-1.0.4/src/viscoso.py
+-rwxrwxrwx   0 root         (0) root         (0)     3784 2023-04-21 10:17:00.000000 coso-1.0.4/src/viscoso_widget.py
```

### Comparing `coso-1.0.3/LICENSE` & `coso-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/PKG-INFO` & `coso-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.3
+Version: 1.0.4
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.3/README.md` & `coso-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/coso.egg-info/PKG-INFO` & `coso-1.0.4/coso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.3
+Version: 1.0.4
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.3/coso.egg-info/SOURCES.txt` & `coso-1.0.4/coso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/setup.py` & `coso-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='coso',
-    version='1.0.3',    
+    version='1.0.4',    
     url='https://github.com/PietroTotis/CoSo',
     author='Pietro Totis',
     author_email='pietro.totis@kuleuven.be',
     license='GNU General Public License (GPL)',
 
     # packages=find_packages(),
     packages=['coso'],
```

### Comparing `coso-1.0.3/src/VisCoSo/__init__.py` & `coso-1.0.4/src/VisCoSo/__init__.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/VisCoSo/header.html` & `coso-1.0.4/src/VisCoSo/header.html`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/VisCoSo/viscoso.css` & `coso-1.0.4/src/VisCoSo/viscoso.css`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/VisCoSo/viscoso.html` & `coso-1.0.4/src/VisCoSo/viscoso.html`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/__init__.py` & `coso-1.0.4/src/__init__.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/cola_parser.py` & `coso-1.0.4/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/configuration.py` & `coso-1.0.4/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/count.py` & `coso-1.0.4/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/gen_plots.py` & `coso-1.0.4/src/gen_plots.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/launcher.py` & `coso-1.0.4/src/launcher.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/level_1.py` & `coso-1.0.4/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/level_2.py` & `coso-1.0.4/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/logger.py` & `coso-1.0.4/src/logger.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/parsetab.py` & `coso-1.0.4/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/problem.py` & `coso-1.0.4/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/sharpCSP.py` & `coso-1.0.4/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/solver.py` & `coso-1.0.4/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/tester.py` & `coso-1.0.4/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/util.py` & `coso-1.0.4/src/util.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/venn.py` & `coso-1.0.4/src/venn.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/viscoso.py` & `coso-1.0.4/src/viscoso.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.3/src/viscoso_widget.py` & `coso-1.0.4/src/viscoso_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import anywidget
 import traitlets
 import ipywidgets as widgets
-from IPython.display import display
+from IPython.display import display, clear_output
 
 from .cola_parser import Parser
 from .problem import EmptyException
 from .util import *
 
 
-def viscoso():
+def show_widget():
     Widget()
 
 
 class Widget(object):
     def __init__(self):
 
-        self.program = None
+        self.program = "A CoLa program"
         self.text_area = None
+        self.current_output = None
 
         text = widgets.HTML(
             """
             <script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
             <script type="text/x-mathjax-config">
                 MathJax.Hub.Config({TeX: {extensions: ["action.js"] }});
             </script>
@@ -30,18 +31,19 @@
 
         self.input_layout()
         self.output_layout()
 
     def input_layout(self):
 
         self.text_area = widgets.Textarea(
-            value="A CoLa program",
+            value=self.program,
             placeholder="Type a CoLa program",
             description="",
             disabled=False,
+            layout=widgets.Layout( height='200px', min_height='100px', width='50%')
         )
         msg = widgets.Label("Or write a CoLa program in the textbox:")
         ub = self.upload_button()
         input_layout = widgets.VBox([ub, msg, self.text_area])
         display(input_layout)
 
     def output_layout(self):
@@ -53,26 +55,32 @@
             icon="check",
         )
 
         display(solve_button)
         output = widgets.Output()
 
         def on_button_solve(b):
-            if self.program is None:
-                self.program = self.text_area.value
+            self.program = self.text_area.value
+            if self.current_output is not None:
+                self.current_output.close()
+                # with self.current_output:
+                clear_output()
+                self.input_layout()
+                display(solve_button)
 
             parser = Parser(cola=self.program)
             try:
                 parser.parse()
                 sol = parser.problem.solve(debug=False)
                 self.viscoso_widget(sol)
+                self.current_output = output
+                display(output)
             except EmptyException:
                 with output:
                     print("Could not find a problem :(")
-                display(output)
 
         solve_button.on_click(on_button_solve)
 
     def upload_button(self):
         upload_button = widgets.FileUpload(
             accept="",  # Accepted file extension e.g. '.txt', '.pdf', 'image/*', 'image/*,.pdf'
             multiple=False,  # True to accept multiple files upload else False
```


# Comparing `tmp/lognflow-0.6.5.tar.gz` & `tmp/lognflow-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.6.5.tar", last modified: Wed Apr 26 02:34:03 2023, max compression
+gzip compressed data, was "lognflow-0.6.6.tar", last modified: Thu Apr 27 10:35:39 2023, max compression
```

## Comparing `lognflow-0.6.5.tar` & `lognflow-0.6.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 02:33:52.000000 lognflow-0.6.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-26 02:33:52.000000 lognflow-0.6.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-26 02:33:52.000000 lognflow-0.6.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-26 02:33:52.000000 lognflow-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 02:33:52.000000 lognflow-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-26 02:34:03.827967 lognflow-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-26 02:33:52.000000 lognflow-0.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70379 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 02:34:03.827967 lognflow-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 02:33:52.000000 lognflow-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 10:35:28.000000 lognflow-0.6.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-27 10:35:28.000000 lognflow-0.6.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-27 10:35:28.000000 lognflow-0.6.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 10:35:28.000000 lognflow-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 10:35:28.000000 lognflow-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-27 10:35:39.400457 lognflow-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-27 10:35:28.000000 lognflow-0.6.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69493 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 10:35:39.404457 lognflow-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 10:35:28.000000 lognflow-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_printprogress.py
```

### Comparing `lognflow-0.6.5/CONTRIBUTING.rst` & `lognflow-0.6.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/HISTORY.rst` & `lognflow-0.6.6/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -59,8 +59,13 @@
 * Better documentation and examples for readme
 * get_var is added to lognflow to get buffered variables logged by log_var
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
-* added end keyword argument to log_text
+* added end keyword argument to log_text
+
+0.6.6 (2023-05-01)
+------------------
+* Better documentation
+* added tifffile imread to logviewer and imwrite to lognflow
```

### Comparing `lognflow-0.6.5/LICENSE` & `lognflow-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/PKG-INFO` & `lognflow-0.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.5
+Version: 0.6.6
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -170,7 +170,12 @@
 * get_var is added to lognflow to get buffered variables logged by log_var
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
 * added end keyword argument to log_text
+
+0.6.6 (2023-05-01)
+------------------
+* Better documentation
+* added tifffile imread to logviewer and imwrite to lognflow
```

### Comparing `lognflow-0.6.5/README.rst` & `lognflow-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/docs/Makefile` & `lognflow-0.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/docs/conf.py` & `lognflow-0.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/docs/installation.rst` & `lognflow-0.6.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/docs/make.bat` & `lognflow-0.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/lognflow/lognflow.py` & `lognflow-0.6.6/lognflow/lognflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,17 +75,14 @@
         
         it will try to open a dialog to select a directory, except, it will
         get a temp directory from the os and continue. 
         
         The lognflow construction can allow setting global settings that can
         be overridden later by calling each of its methods as follows.
         
-        Parameters
-        ----------
-    
         .. note::
             One of the variables ``logs_root`` or ``log_dir`` must be given.
             if ``log_dir`` is given, ``logs_root`` is disregarded.
     
         :param logs_root: 
             This is the root directory for all logs.
             We will use the time.time() to create a log directory for each 
@@ -145,14 +142,17 @@
                     pass
             
             new_log_dir_found = False
             while(not new_log_dir_found):
                 log_dir_name = ''
                 if(log_prefix is not None):
                     log_dir_name = str(log_prefix)
+                    if len(log_dir_name) > 0:
+                        if log_dir_name[-1] != '_':
+                            log_dir_name += '_'
                 log_dir_name += f'{self._init_time}/'
                 self.log_dir = \
                     pathlib.Path(logs_root) / log_dir_name
                 if(not self.log_dir.is_dir()):
                     new_log_dir_found = True
                 else:
                     self._init_time = time.time()
@@ -167,25 +167,23 @@
         self._loggers_dict = {}
         self._vars_dict = {}
         self._single_var_call_cnt = 0
 
         self.log_name = main_log_name
         self.log_flush_period = log_flush_period
     
-    def rename(self, new_name:str, append : bool = False):
+    def rename(self, new_name:str, append: bool = False):
         """ renaming the log directory
             It is possible to rename the log directory while logging is going
             on. This is particulary useful when at the end of an experiment,
             it is necessary to put some variables in the name of the directory,
             which is very realistic in the eyes of an experimentalist.
             
             There is only one input and that is the new name of the directory.
 
-            Parameters
-            ----------
             :param new_name: The new name of the directory (without parent path)
             :type new_name: str
             
             :param append: keep the time tag for the folder. Default: False.
             :type append: bool
             
         """
@@ -203,27 +201,28 @@
             self.log_text(None, 'Could not rename the log_dir from:')
             self.log_text(None, f'{self.log_dir.name}')
             self.log_text(None, 'into:')
             self.log_text(None, f'{new_name}')
             self.log_text(None, 'Most probably a file was open.')
         return self.log_dir
     
-    def _prepare_param_dir(self, parameter_name : str):
+    def _prepare_param_dir(self, parameter_name: str):
         try:
             _ = parameter_name.split()
         except:
             self.log_text(
                 self.log_name,
-                'The parameter name is not a string. ' \
-                + f'Its type is {type(parameter_name)}. It is {parameter_name}')
+                f'The parameter name {parameter_name} is not a string.' \
+                + f' Its type is {type(parameter_name)}.')
         assert len(parameter_name.split()) == 1, \
             self.log_text(self.log_name,\
-                  f'The variable name {parameter_name} you chose is splitable' \
+                  f'The variable name {parameter_name} you chose, is splitable'\
                 + f' I can split it into {parameter_name.split()}'             \
-                + ' Make sure you dont use space, tab, or ....'                \
+                + ' Make sure you dont use space, tab, or backslash with known'\
+                + ' small letters such as f, t, ...'                           \
                 + ' If you are using single backslash, e.g. for windows'       \
                 + ' folders, replace it with \\ or make it a literal string'   \
                 + ' by putting an r before the variable name.')
         
         is_dir = (parameter_name[-1] == '/') | (parameter_name[-1] == '\\') \
                  | (parameter_name[-1] == r'/') | (parameter_name[-1] == r'\\')
         param_dir = self.log_dir /  parameter_name
@@ -235,16 +234,16 @@
             param_dir = param_dir.parent
         if(not param_dir.is_dir()):
             self.log_text(self.log_name,
                           f'Creating directory: {param_dir.absolute()}')
             param_dir.mkdir(parents = True, exist_ok = True)
         return(param_dir, param_name)
 
-    def _get_fpath(self, param_dir : pathlib.Path, param_name : str, 
-                   save_as : str, time_tag : bool = None) -> pathlib.Path:
+    def _get_fpath(self, param_dir: pathlib.Path, param_name: str, 
+                   save_as: str, time_tag: bool = None) -> pathlib.Path:
         
         time_time = time.time() - self._init_time
         time_tag = self.time_tag if (time_tag is None) else time_tag
         
         if(save_as == 'mat'):
             if(len(param_name) == 0):
                 param_name = param_dir.name
@@ -256,15 +255,15 @@
         else:
             fname = f'{time_time:>6.6f}'
             
         return(param_dir / f'{fname}.{save_as}')
         
     def _log_text_handler(self, log_name = None, 
                          log_size_limit: int = int(1e+7),
-                         time_tag : bool = None,
+                         time_tag: bool = None,
                          log_flush_period = None):
         
         if (log_flush_period is None):
             log_flush_period = self.log_flush_period
             
         param_dir, param_name = self._prepare_param_dir(log_name)
         fpath = self._get_fpath(param_dir, param_name, 'txt', time_tag)
@@ -274,26 +273,21 @@
             log_size_limit=log_size_limit,    
             log_size=0,          
             last_log_flush_time=0,
             log_flush_period=log_flush_period)  
 
     def log_text_flush(self, log_name = None, 
                        flush = False):
-        """
-        Keep str as a list of lines to be logged. This function must take the 
-        log name too. Then put the str in the log file.
-        """
         """ Flush the text logs
             Writing text to open(file, 'a') does not constantly happen on HDD.
             There is an OS buffer in between. This funciton should be called
             regularly. lognflow calls it once in a while when log_text is
             called multiple times. but use needs to also call it once in a
             while.
             In later versions, a timer will be used to call it automatically.
-            
             :param flush:
                 force the flush regardless of when the last time was.
                 default: False
             :type flush: bool
         """
         time_time = time.time() - self._init_time
 
@@ -307,60 +301,58 @@
             with open(curr_textinlog.log_fpath, 'a+') as f:
                 f.writelines(curr_textinlog.to_be_logged)
                 f.flush()
             curr_textinlog.to_be_logged = []
             curr_textinlog.last_log_flush_time = time_time
 
     def log_text(self, 
-                 log_name : str = None,
+                 log_name: str = None,
                  to_be_logged = '', 
                  log_time_stamp = True,
                  print_text = None,
                  log_size_limit: int = int(1e+7),
-                 time_tag : bool = None,
-                 log_flush_period : int = None,
+                 time_tag: bool = None,
+                 log_flush_period: int = None,
                  flush = False,
                  end = '\n',
                  new_file = False):
         """ log a string into a text file
             You can shose a name for the log and give the text to put in it.
             Also you can pass a small numpy array. You can ask it to put time
             stamp in the log and in the log file name, you can disable
             printing the text. You can set the log size limit to split it into
             another file with a new time stamp.
             
-            Parameters
-            ----------
-            :param log_name : str
-                    examples: mylog or myscript/mylog
-                    log_name can be just a name e.g. mylog, or could be a
-                    pathlike name such as myscript/mylog.
-            :param to_be_logged : str, nd.array, list, dict
-                    the string to be logged, could be a list
-                    or numpy array or even a dictionary. It uses str(...).
-            :param log_time_stamp : bool
-                    Put time stamp for every entry of the log
-            :param print_text : bool
-                    if False, what is logged will not be printed.
-            :param log_size_limit : int
-                    log size limit in bytes.
-            :param time_tag : bool
-                    put time stamp in file names.
-            :param log_flush_period : int
-                    How often flush the log in seconds, if time passes this
-                    given period, it will flush the first time a text is logged,
-                    or if the logger is finilized.
-            :param flush : bool
-                    force flush into the log file
+            :param log_name: str
+                   examples: mylog or myscript/mylog
+                   log_name can be just a name e.g. mylog, or could be a
+                   pathlike name such as myscript/mylog.
+            :param to_be_logged: str, nd.array, list, dict
+                   the string to be logged, could be a list
+                   or numpy array or even a dictionary. It uses str(...).
+            :param log_time_stamp: bool
+                   Put time stamp for every entry of the log
+            :param print_text: bool
+                   if False, what is logged will not be printed.
+            :param log_size_limit: int
+                   log size limit in bytes.
+            :param time_tag: bool
+                   put time stamp in file names.
+            :param log_flush_period: int
+                   How often flush the log in seconds, if time passes this
+                   given period, it will flush the first time a text is logged,
+                   or if the logger is finilized.
+            :param flush: bool
+                   force flush into the log file
             :param end: str
-                    The last charachter for this call.
+                   The last charachter for this call.
             :param new_file: bool
-                    if a new file is needed. If time_tag is True, it will make
-                    a new file with a new name that has a time tag. If False,
-                    it closees the current text file and overwrites on it.
+                   if a new file is needed. If time_tag is True, it will make
+                   a new file with a new name that has a time tag. If False,
+                   it closees the current text file and overwrites on it.
         """
         time_time = time.time() - self._init_time
 
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
         log_name = self.log_name if (log_name is None) else log_name
@@ -407,40 +399,38 @@
         return curr_textinlog.log_fpath
                         
 
     def _get_log_counter_limit(self, param, log_size_limit):
         cnt_limit = int(log_size_limit/(param.size*param.itemsize))
         return cnt_limit
 
-    def log_var(self, parameter_name : str, parameter_value, 
+    def log_var(self, parameter_name: str, parameter_value, 
                 save_as='npz', log_size_limit: int = int(1e+7)):
         """log a numpy array in buffer then dump
             It can be the case that we need to take snapshots of a numpy array
             over time. The size of the array would not change and this is hoing
             to happen frequently.
             This log_ver makes a buffer in RAM and keeps many instances of the
             array along with their time stamp and then when the size of the 
             array reaches a threhshold flushes it into HDD with a file that
             has an initial time stamp.
             The benefit of using this function over log_single is that it
             does not use the connection to the directoy all time and if that is
             on a network, there will be less overhead.
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array whose size doesn't change
-            :param save_as : str
+            :param save_as: str
                     can be 'npz' or 'txt' which will save it as text.
             :param log_size_limit: int
-                    log_size_limit in bytes, default : 1e+7.
+                    log_size_limit in bytes, default: 1e+7.
                     
         """
         
         time_time = time.time() - self._init_time
         
         try:
             _ = parameter_value.shape
@@ -489,23 +479,23 @@
         self._vars_dict[parameter_name] = varinlog(data_array, 
                                                    time_array, 
                                                    curr_index,
                                                    file_start_time,
                                                    save_as,
                                                    log_counter_limit)
 
-    def log_var_flush(self, parameter_name : str):
+    def log_var_flush(self, parameter_name: str):
         """ Flush the buffered numpy arrays
             If you have been using log_ver, this will flush all the buffered
             arrays. It is called using log_size_limit for a variable and als
             when the code that made the logger ends.
-        :param parameter_name : str
-            examples: myvar or myscript/myvar
-                parameter_name can be just a name e.g. myvar, or could be a
-                path like name such as myscript/myvar.
+            :param parameter_name: str
+                examples: myvar or myscript/myvar
+                    parameter_name can be just a name e.g. myvar, or could be a
+                    path like name such as myscript/myvar.
         """
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         
         _var = self._vars_dict[parameter_name]
         _var_data_array = _var.data_array[_var.time_array > 0]
         _var_time_array = _var.time_array[_var.time_array > 0]
         if(_var.save_as == 'npz'):
@@ -516,56 +506,56 @@
         elif(_var.save_as == 'txt'):
             fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_time_array)
             fpath = param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_data_array)
         return fpath
     
-    def get_var(self, parameter_name : str):
+    def get_var(self, parameter_name: str) -> tuple:
         """ Get the buffered numpy arrays
             If you need the buffered variable back.
-        :param parameter_name : str
-            examples: myvar or myscript/myvar
-                parameter_name can be just a name e.g. myvar, or could be a
-                path like name such as myscript/myvar.
-        
-        :return: A tuple including two np.ndarray. The first on is 1d time
-            and the second one is nd buffered data.
-        :rtype: tuple of two nd.arrays
+            :param parameter_name: str
+                examples: myvar or myscript/myvar
+                    parameter_name can be just a name e.g. myvar, or could be a
+                    path like name such as myscript/myvar.
+            
+            :return: 
+                A tuple including two np.ndarray. The first on is 1d time
+                and the second one is nd buffered data.
+            :rtype: 
+                tuple of two nd.arrays
         
         """
         _var = self._vars_dict[parameter_name]
         data_array = _var.data_array[_var.time_array>0].copy()
         time_array = _var.time_array[_var.time_array>0].copy()
         return(time_array, data_array)
 
-    def log_single(self, parameter_name : str, 
+    def log_single(self, parameter_name: str, 
                          parameter_value,
                          save_as = None,
                          mat_field = None,
-                         time_tag : bool = None):
+                         time_tag: bool = None):
         """log a single variable
             The most frequently used function would probably be this one.
             
             if you call the logger object as a function and give it a parameter
             name and something to be logged, the __call__ referes to this
             function.
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array whose size doesn't change
-            :param save_as : str
+            :param save_as: str
                     can be 'npz', 'npy', 'mat', 'torch' for pytorch models
                     or 'txt' which will save it as text.
-            :param mat_field : str
+            :param mat_field: str
                     when saving as 'mat' file, the field can be set.
                     otherwise it will be the parameter_name
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
@@ -580,38 +570,39 @@
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
             
         if(save_as == 'npy'):
             np.save(fpath, parameter_value)
         elif(save_as == 'npz'):
             np.savez(fpath, **parameter_value)
+        elif((save_as == '.tif') | (save_as == '.tiff')):
+            from tifffile import imwrite
+            imwrite(fpath, parameter_value)
         elif(save_as == 'txt'):
             with open(fpath,'a') as fdata: 
                 fdata.write(str(parameter_value))
         elif(save_as == 'mat'):
             from scipy.io import savemat
             if(mat_field is None):
                 mat_field = param_name
-            savemat(fpath, {f'{mat_field}' :parameter_value})
+            savemat(fpath, {f'{mat_field}':parameter_value})
         elif(save_as == 'torch'):
             from torch import save as torch_save
             torch_save(parameter_value.state_dict(), fpath)
         return fpath
     
     def log_plt(self, 
-                parameter_name : str, 
+                parameter_name: str, 
                 image_format='jpeg', dpi=1200,
-                time_tag : bool = None,
+                time_tag: bool = None,
                 close_plt = True):
         """log a single plt
             log a plt that you have on the screen.
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
@@ -642,32 +633,30 @@
         fig = ax.figure
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         cbar = fig.colorbar(mappable, cax=cax)
         # cbar.ax.tick_params(size=0.01)
 
     def log_multichannel_by_subplots(self, 
-        parameter_name : str, 
-        parameter_value : np.ndarray,
+        parameter_name: str, 
+        parameter_value: np.ndarray,
         image_format='jpeg', 
         dpi=1200, 
-        time_tag : bool = None,
+        time_tag: bool = None,
         add_colorbar = False,
         remove_axis_ticks = True,
         **kwargs):
         """log multiple images as a tiled square
             The image is logged using plt.imshow
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array of size n_r, n_c, n_ch, to be shown by imshow
                     as a square tile of side length of n_ch**0.5
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         
@@ -676,42 +665,40 @@
         n_r, n_c, n_ch = parameter_value.shape
         n_ch_sq = int(np.ceil(n_ch ** 0.5))
         _, ax = plt.subplots(n_ch_sq,n_ch_sq)
         if(remove_axis_ticks):
             plt.setp(ax, xticks=[], yticks=[])
         for rcnt in range(n_ch_sq):
             for ccnt in range(n_ch_sq):
-                im = parameter_value[:, :, ccnt + rcnt * n_ch_sq]
+                im = parameter_value[:,:, ccnt + rcnt * n_ch_sq]
                 im_ch = ax[rcnt, ccnt].imshow(im, **kwargs)
                 if(add_colorbar):
                     self.add_colorbar(im_ch)
         return self.log_plt(parameter_name = parameter_name,
                      image_format=image_format, dpi=dpi,
                      time_tag = time_tag)
             
-    def log_plot(self, parameter_name : str, 
+    def log_plot(self, parameter_name: str, 
                        parameter_value_list,
                        x_values = None,
                        image_format='jpeg', dpi=1200,
-                       time_tag : bool = None,
+                       time_tag: bool = None,
                        **kwargs):
         """log a single plot
             If you have a numpy array or a list of arrays (or indexable by
             first dimension, an array of 1D arrays), use this to log a plot 
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value_list : np.array
+            :param parameter_value_list: np.array
                     An np array or a list of np arrays or indexable-by-0th-dim
                     np arrays
-            :param x_values : np.array
+            :param x_values: np.array
                     if set, must be an np.array of same size of all y values
                     or a list for each vector in y values where every element
                     of x-values list is the same as the y-values element in 
                     their list
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
@@ -750,39 +737,37 @@
                         
             return fpath
         except:
             self.log_text(self.log_name,
                           f'Cannot plot variable {parameter_name}.')
             return None
     
-    def log_hist(self, parameter_name : str, 
+    def log_hist(self, parameter_name: str, 
                        parameter_value_list,
                        n_bins = 10,
                        alpha = 0.5,
                        image_format='jpeg', dpi=1200,
-                       time_tag : bool = None, 
+                       time_tag: bool = None, 
                        **kwargs):
         """log a single histogram
             If you have a numpy array or a list of arrays (or indexable by
             first dimension, an array of 1D arrays), use this to log a hist
             if multiple inputs are given they will be plotted on top of each
             other using the alpha opacity. 
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value_list : np.array
+            :param parameter_value_list: np.array
                     An np array or a list of np arrays or indexable-by-0th-dim
                     np arrays
-            :param n_bins : number or np.array
+            :param n_bins: number or np.array
                     used to set the bins for making of the histogram
-            :param alpha : float 
+            :param alpha: float 
                     the opacity of histograms, a flot between 0 and 1. If you
                     have multiple histograms on top of each other,
                     use 1/number_of_your_variables.
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
@@ -804,27 +789,25 @@
                 time_tag = time_tag)
             return fpath
         except:
             self.log_text(self.log_name,
                 f'Cannot make the histogram for variable {parameter_name}.')
             return None
     
-    def log_scatter3(self, parameter_name : str,
+    def log_scatter3(self, parameter_name: str,
                        parameter_value, image_format='jpeg', dpi=1200,
-                       time_tag : bool = None):
+                       time_tag: bool = None):
         """log a single scatter in 3D
             Scatter plotting in 3D
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array of size 3 x n, to sctter n data points in 3D
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
@@ -840,27 +823,25 @@
                 time_tag = time_tag)
             return fpath
         except:
             self.log_text(self.log_name,
                 f'Cannot make the scatter3 for variable {parameter_name}.')
             return None
     
-    def log_surface(self, parameter_name : str,
+    def log_surface(self, parameter_name: str,
                        parameter_value, image_format='jpeg', dpi=1200,
-                       time_tag : bool = None, **kwargs):
+                       time_tag: bool = None, **kwargs):
         """log a surface in 3D
             surface plotting in 3D exactly similar to imshow but in 3D
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array of size n x m, to plot surface in 3D
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
             rest of the parameters (**kwargs) will be passed to plot_surface() 
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
@@ -877,29 +858,27 @@
                 time_tag = time_tag)
             return fpath
         except:
             self.log_text(self.log_name,
                 f'Cannot make the surface plot for variable {parameter_name}.')
             return None
         
-    def log_hexbin(self, parameter_name : str, parameter_value,
+    def log_hexbin(self, parameter_name: str, parameter_value,
                    gridsize = 20, image_format='jpeg', dpi=1200,
-                   time_tag : bool = None):
+                   time_tag: bool = None):
         """log a 2D histogram 
             The 2D histogram is made out of hexagonals
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array of size 2 x n, to make the 2D histogram
-            :param gridsize : int
+            :param gridsize: int
                     grid size is the number of bins in 2D
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
 
@@ -914,29 +893,27 @@
                     time_tag = time_tag)
             return fpath
         except:
             self.log_text(self.log_name,
                 f'Cannot make the hexbin for variable {parameter_name}.')
             return None
         
-    def log_imshow(self, parameter_name : str, 
+    def log_imshow(self, parameter_name: str, 
                    parameter_value,
                    image_format='jpeg', dpi=1200, cmap = 'jet',
-                   time_tag : bool = None, nan_borders = np.nan,
+                   time_tag: bool = None, nan_borders = np.nan,
                    **kwargs):
         """log an image
             The image is logged using plt.imshow
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param parameter_value : np.array
+            :param parameter_value: np.array
                     An np array of shape amongst the following:
                     * (n, m) 
                     * (n, m, 3)
                     * (n, m, ch)
                     * (1, n, m, ch)
                     * (n, m, 3, ch)
             :param time_tag: bool
@@ -987,17 +964,15 @@
             return
 
     def multichannel_to_square(self, stack, nan_borders = np.nan):
         """ turn a stack of multi-channel images into stack of square images
             This is very useful when lots of images need to be tiled
             against each other.
         
-            Parameters
-            ----------
-            :param stack : np.ndarray
+            :param stack: np.ndarray
                     It must have the shape of either
                     n_r x n_c x n_ch
                     n_r x n_c x  3  x n_ch
                     n_f x n_r x n_c x n_ch
                     n_f x n_r x n_c x  3  x n_ch
                     
                 In both cases n_ch will be turned into a square tile
@@ -1044,16 +1019,16 @@
             stack[:, -1:       ] = nan_borders
             stack[:,   : , -1: ] = nan_borders
             
             for rcnt in range(square_side):
                 for ccnt in range(square_side):
                     ch_cnt = rcnt + square_side*ccnt
                     if (ch_cnt<n_ch):
-                        canv[:, rcnt*n_R : (rcnt + 1)*n_R,
-                                ccnt*n_C : (ccnt + 1)*n_C] = \
+                        canv[:, rcnt*n_R: (rcnt + 1)*n_R,
+                                ccnt*n_C: (ccnt + 1)*n_C] = \
                             stack[..., used_ch_cnt]
                         used_ch_cnt += 1
         else:
             return None
         return canv
 
     def _handle_images_stack(self, stack, nan_borders = np.nan):
@@ -1085,43 +1060,41 @@
             n_frm x n_row x n_clm if there are n_frm images 
                                   for all elements of stack
             n_frm x n_row x n_clm x n_ch if there are multiple images to be
                                          shown. 
                                          Channels will be tiled into square
             n_frm x n_row x n_clm x n_ch x 3 if channels are in RGB
     
-            Parameters
-            ----------
             :param list_of_stacks
                     list_of_stacks would include arrays iteratable by their
                     first dimension.
-            :param nan_borders : float
+            :param nan_borders: float
                     borders between tiles will be filled with this variable
                     default: np.nan
         """        
         if (not isinstance(list_of_stacks, list)):
             list_of_stacks = [list_of_stacks]
         for cnt, stack in enumerate(list_of_stacks):
             stack = self._handle_images_stack(stack, nan_borders = nan_borders)
             if(stack is None):
                 return
             list_of_stacks[cnt] = stack
         return(list_of_stacks)
 
     def log_canvas(self, 
-                   parameter_name : str,
-                   list_of_stacks : list,
+                   parameter_name: str,
+                   list_of_stacks: list,
                    list_of_masks = None,
                    figsize_ratio = 1,
                    text_as_colorbar = False,
                    use_colorbar = False,
                    image_format='jpeg', 
                    cmap = 'jet',
                    dpi=1200,
-                   time_tag : bool = None):
+                   time_tag: bool = None):
         """log a cavas of stacks of images
             One way to show many images and how they change is to make
             stacks of images and put them in a list. Then each
             element of the list is supposed to be iteratable by the first
             dimension, which should be the same sie for all elements in the list.
             This function will start putting them in coloumns of a canvas.
             If you have an image with many channels, call 
@@ -1133,31 +1106,29 @@
             n_frm x n_row x n_clm if there are n_frm images 
                                   for all elements of stack
             n_frm x n_row x n_clm x 3 if channels are in RGB
             
             if you have multiple images as channels such as the following,
             call the prepare_stack_of_images.
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param list_of_stacks : list
+            :param list_of_stacks: list
                     List of stack of images, each of which can be a
                     n_F x n_r x n_c. Notice that n_F should be the same for all
                     elements of the list.
-            :param list_of_masks : list
+            :param list_of_masks: list
                     the same as the list_of_stacks and will be used to make
                     accurate colorbars
-            :param text_as_colorbar : bool
+            :param text_as_colorbar: bool
                     if True, max and mean and min of each image will be written
                     on it.
-            :param use_colorbar : bool
+            :param use_colorbar: bool
                     actual colorbar for each iamge will be shown
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
@@ -1235,60 +1206,58 @@
         fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
         return fpath
 
     def log_confusion_matrix(self,
-                             parameter_name : str,
+                             parameter_name: str,
                              cm,
                              target_names = None,
                              title='Confusion matrix',
                              cmap=None,
                              figsize = None,
                              image_format = 'jpeg',
                              dpi = 1200,
                              time_tag = False):
-        """
+        """log a confusion matrix
             given a sklearn confusion matrix (cm), make a nice plot
         
-            Parameters
-            ---------
-            :param cm:           confusion matrix from sklearn.metrics.confusion_matrix
-            
-            :param target_names: given classification classes such as [0, 1, 2]
-                              the class names, for example: ['high', 'medium', 'low']
+            :param cm:
+                confusion matrix from sklearn.metrics.confusion_matrix
             
-            :param title:        the text to display at the top of the matrix
-            
-            :param cmap: the gradient of the values displayed from matplotlib.pyplot.cm
-                         (http://matplotlib.org/examples/color/colormaps_reference.html)
-                         plt.get_cmap('jet') or plt.cm.Blues
+            :param target_names: 
+                given classification classes such as [0, 1, 2]
+                the class names, for example: ['high', 'medium', 'low']
+            
+            :param title:        
+                the text to display at the top of the matrix
+            
+            :param cmap: 
+                the gradient of the values displayed from matplotlib.pyplot.cm
+                (http://matplotlib.org/examples/color/colormaps_reference.html)
+                plt.get_cmap('jet') or plt.cm.Blues
                 
-            :param time_tag: if True, the file name will be stamped with time
+            :param time_tag: 
+                if True, the file name will be stamped with time
         
-            Usage
+            Usage::
             -----
-            .. highlight:: python
-               :linenothreshold: 5
-               
-            .. code-block:: python
                 from lognflow import lognflow
                 logger = lognflow(log_roots or log_dir)
                 logger.plot_confusion_matrix(\
                     cm           = cm,                  # confusion matrix created by
                                                         # sklearn.metrics.confusion_matrix
                     target_names = y_labels_vals,       # list of names of the classes
                     title        = best_estimator_name) # title of graph
                         
         
-            Citiation
-            ---------
-            http://scikit-learn.org/stable/auto_examples/model_selection/
-                                                           plot_confusion_matrix.html
+            Credit
+            ------
+                http://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html
     
         """
         accuracy = np.trace(cm) / np.sum(cm).astype('float')
         misclass = 1 - accuracy
     
         if figsize is None:
             figsize = np.ceil(cm.shape[0]/3)
@@ -1322,28 +1291,26 @@
         plt.tight_layout()
         fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
         return fpath
 
-    def log_animation(self, parameter_name : str, stack, 
+    def log_animation(self, parameter_name: str, stack, 
                          interval=50, blit=False, 
                          repeat_delay = None, dpi=100,
-                         time_tag : bool = None):
+                         time_tag: bool = None):
         
         """Make an animation from a stack of images
             
-            Parameters
-            ----------
-            :param parameter_name : str
+            :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
-            :param stack : np.array of shape 
+            :param stack: np.array of shape 
                     n_f x n_r x n_c or n_f x n_r x n_c x 3
                     stack[cnt] needs to be plotable by plt.imshow()
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
@@ -1385,16 +1352,14 @@
             return txt
 
     def get_single(self, var_name, single_shot_index = -1, 
                      suffix = '.np*'):
         """ get a single variable
             return the value of a saved variable.
 
-            Parameters
-            ----------
             :param var_name:
                 variable name
             :param single_shot_index:
                 If there are many snapshots of a variable, this input can
                 limit the returned to a set of indices.
             :param suffix:
                 If there are different suffixes availble for a variable
@@ -1457,37 +1422,35 @@
             if(var_path.suffix == '.npy'):
                 return(np.load(var_path))
             if(var_path.suffix == '.mat'):
                 return(loadmat(var_path))
             if(var_path.suffix == '.txt'):
                 with open(var_path) as f_txt:
                     return(f_txt.read())
+            if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
+                from tifffile import imread
+                return(imread(var_path))                
             if(var_path.suffix == '.torch'):      
                 from torch import load as torch_load 
                 return(torch_load(var_path))
             try:
                 img = imread(var_path)
                 return(img)
             except:
                 pass
-        else:
-            # self.log_text(None, f'{var_name} not found.')
-            return
     
     def get_stack_of_files(self, 
         var_name = None, flist = [], suffix = '*',
-        return_data = False, return_flist = True):
+        return_data = False, return_flist = True) -> tuple:
         
         """ Get list or data of all files in a directory
         
             This function gives the list of paths of all files in a directory
             for a single variable. 
 
-            Parameters
-            ----------
             :param var_name:
                 The directory or variable name to look for the files
             :type var_name: str
             
             :param flist:
                 list of Paths, if data is returned, this flist input can limit 
                 the data requested to this list.
@@ -1500,21 +1463,21 @@
             :param return_data: 
                     with flist you can limit the data that is returned.
                     Otherwise the data for all files in the directory will be
                     returned
             :param return_flist
                     Maybe you are only intrested in the flist.
                     
-            Output
-            ----------
-            
+            :return:
                 It returns a tuple, (dataset, flist),
                 dataset will be a numpy array in case all files produce same
                 shape numpy arrays.
                 flist is type pathlib.Path
+            :rtype: tuple
+            
             
         """
         suffix = suffix.strip('.')
         if not flist:
             assert var_name is not None, \
                 ' The file list is empty. Please provide the ' \
                 + 'variable name or a non-empty file list.'
@@ -1567,16 +1530,14 @@
     def get_common_files(self, var_name_A, var_name_B):
         """ get common files in two directories
         
             It happens often in ML that there are two directories, A and B,
             and we are interested to get the flist in both that is common 
             between them. returns a tuple of two lists of files.
             
-            Parameters
-            ----------
             :param var_name_A:
                 directory A name
             :param var_name_B:
                 directory B name
         """
         flist_A = self.get_stack_of_files(
             var_name_A, return_data = False, return_flist = True)
@@ -1605,16 +1566,14 @@
     def replace_time_with_index(self, var_name):
         """ index in file names
             lognflow uses time stamps to make new log files for a variable.
             That is done by putting _time_stamp after the name of the variable.
             This function changes all of the time stamps, sorted ascendingly,
             by indices.
             
-            Parameters
-            ----------
             :param var_name:
                 variable name
         """
         var_dir = self.log_dir / var_name
         if(var_dir.is_dir()):
             var_fname = None
             flist = list(var_dir.glob(f'*.*'))
@@ -1666,17 +1625,15 @@
     def __bool__(self):
         return self.log_dir.is_dir()
 
 def select_directory(default_directory = './'):
     """ Open dialog to select a directory
         It works for windows and Linux using PyQt5.
     
-        Parameters
-        ----------
-        :param default_directory: pathlib.Path
+       :param default_directory: pathlib.Path
                 When dialog opens, it starts from this default directory.
     """
     from PyQt5.QtWidgets import QFileDialog, QApplication
     _ = QApplication([])
     log_dir = QFileDialog.getExistingDirectory(
         None, "Select a directory", default_directory, QFileDialog.ShowDirsOnly)
     return(log_dir)
```

### Comparing `lognflow-0.6.5/lognflow/logviewer.py` & `lognflow-0.6.6/lognflow/logviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,17 @@
             if(var_path.suffix == '.npy'):
                 return(np.load(var_path))
             if(var_path.suffix == '.mat'):
                 return(loadmat(var_path))
             if(var_path.suffix == '.txt'):
                 with open(var_path) as f_txt:
                     return(f_txt.read())
+            if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
+                from tifffile import imread
+                return(imread(var_path))
             if(var_path.suffix == '.torch'):      
                 from torch import load as torch_load 
                 return(torch_load(var_path))
             try:
                 img = imread(var_path)
                 return(img)
             except:
```

### Comparing `lognflow-0.6.5/lognflow/printprogress.py` & `lognflow-0.6.6/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/lognflow.egg-info/PKG-INFO` & `lognflow-0.6.6/lognflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.5
+Version: 0.6.6
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -170,7 +170,12 @@
 * get_var is added to lognflow to get buffered variables logged by log_var
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
 * added end keyword argument to log_text
+
+0.6.6 (2023-05-01)
+------------------
+* Better documentation
+* added tifffile imread to logviewer and imwrite to lognflow
```

### Comparing `lognflow-0.6.5/lognflow.egg-info/SOURCES.txt` & `lognflow-0.6.6/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/setup.py` & `lognflow-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.6.5'
+__version__ = '0.6.6'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.6.5/tests/test_lognflow.py` & `lognflow-0.6.6/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/tests/test_logviewer.py` & `lognflow-0.6.6/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.5/tests/test_printprogress.py` & `lognflow-0.6.6/tests/test_printprogress.py`

 * *Files identical despite different names*


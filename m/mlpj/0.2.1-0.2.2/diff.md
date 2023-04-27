# Comparing `tmp/mlpj-0.2.1.tar.gz` & `tmp/mlpj-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpj-0.2.1.tar", last modified: Tue Apr 25 16:54:59 2023, max compression
+gzip compressed data, was "mlpj-0.2.2.tar", last modified: Thu Apr 27 11:07:31 2023, max compression
```

## Comparing `mlpj-0.2.1.tar` & `mlpj-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.610810 mlpj-0.2.1/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.1/LICENSE
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-25 16:54:59.610810 mlpj-0.2.1/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.1/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.607477 mlpj-0.2.1/mlpj/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-04-25 16:50:02.000000 mlpj-0.2.1/mlpj/__init__.py
--rw-------   0 bruno     (1000) bruno     (1000)    30221 2023-04-23 10:31:40.000000 mlpj-0.2.1/mlpj/actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7743 2023-04-23 17:34:32.000000 mlpj-0.2.1/mlpj/ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1190 2023-04-22 15:20:30.000000 mlpj-0.2.1/mlpj/numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    23146 2023-04-23 16:17:57.000000 mlpj-0.2.1/mlpj/pandas_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    28573 2023-04-24 10:47:07.000000 mlpj-0.2.1/mlpj/plot_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)     7593 2023-04-23 16:30:36.000000 mlpj-0.2.1/mlpj/project_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7860 2023-04-25 16:48:41.000000 mlpj-0.2.1/mlpj/python_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    18232 2023-04-23 11:06:21.000000 mlpj-0.2.1/mlpj/result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.1/mlpj/result_template.html
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1630 2023-04-25 13:13:57.000000 mlpj-0.2.1/mlpj/timeseries_utils.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.607477 mlpj-0.2.1/mlpj.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      562 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-04-25 16:54:59.610810 mlpj-0.2.1/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1223 2023-04-25 16:49:37.000000 mlpj-0.2.1/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.610810 mlpj-0.2.1/test/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    10983 2023-04-23 10:38:17.000000 mlpj-0.2.1/test/test_actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      483 2023-04-22 15:22:38.000000 mlpj-0.2.1/test/test_numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13448 2023-04-22 17:43:03.000000 mlpj-0.2.1/test/test_pandas_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3686 2023-04-22 16:30:49.000000 mlpj-0.2.1/test/test_python_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2978 2023-04-24 07:28:36.000000 mlpj-0.2.1/test/test_result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1515 2023-04-22 17:44:08.000000 mlpj-0.2.1/test/test_timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 11:07:31.464141 mlpj-0.2.2/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.2/LICENSE
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-27 11:07:31.464141 mlpj-0.2.2/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.2/README.md
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 11:07:31.460808 mlpj-0.2.2/mlpj/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-04-26 14:37:21.000000 mlpj-0.2.2/mlpj/__init__.py
+-rw-------   0 bruno     (1000) bruno     (1000)    31419 2023-04-26 13:32:13.000000 mlpj-0.2.2/mlpj/actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    12131 2023-04-27 10:49:14.000000 mlpj-0.2.2/mlpj/ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1280 2023-04-26 12:56:20.000000 mlpj-0.2.2/mlpj/numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    24925 2023-04-26 13:58:50.000000 mlpj-0.2.2/mlpj/pandas_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    29704 2023-04-26 12:54:56.000000 mlpj-0.2.2/mlpj/plot_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)     7792 2023-04-26 13:31:12.000000 mlpj-0.2.2/mlpj/project_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     8449 2023-04-26 13:42:35.000000 mlpj-0.2.2/mlpj/python_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    18778 2023-04-26 13:30:54.000000 mlpj-0.2.2/mlpj/result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.2/mlpj/result_template.html
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1882 2023-04-26 14:13:05.000000 mlpj-0.2.2/mlpj/timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 11:07:31.460808 mlpj-0.2.2/mlpj.egg-info/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-27 11:07:31.000000 mlpj-0.2.2/mlpj.egg-info/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      584 2023-04-27 11:07:31.000000 mlpj-0.2.2/mlpj.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-04-27 11:07:31.000000 mlpj-0.2.2/mlpj.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-04-27 11:07:31.000000 mlpj-0.2.2/mlpj.egg-info/requires.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-04-27 11:07:31.000000 mlpj-0.2.2/mlpj.egg-info/top_level.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-04-27 11:07:31.464141 mlpj-0.2.2/setup.cfg
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1223 2023-04-26 14:37:12.000000 mlpj-0.2.2/setup.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 11:07:31.460808 mlpj-0.2.2/test/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    11486 2023-04-26 14:07:56.000000 mlpj-0.2.2/test/test_actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     5476 2023-04-27 10:47:47.000000 mlpj-0.2.2/test/test_ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      499 2023-04-26 12:33:47.000000 mlpj-0.2.2/test/test_numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    13724 2023-04-26 12:35:55.000000 mlpj-0.2.2/test/test_pandas_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3807 2023-04-26 12:55:06.000000 mlpj-0.2.2/test/test_python_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3102 2023-04-26 14:00:27.000000 mlpj-0.2.2/test/test_result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1531 2023-04-26 14:00:51.000000 mlpj-0.2.2/test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2.1/LICENSE` & `mlpj-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.1/PKG-INFO` & `mlpj-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2.1/README.md` & `mlpj-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.1/mlpj/actions_looper.py` & `mlpj-0.2.2/mlpj/actions_looper.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,58 +63,59 @@
 import sys
 import re
 import argparse
 import collections
 import pickle
 import inspect
 import types
+from typing import Optional, List, Union, Type, Tuple, Dict, Any
 
 from . import python_utils as pu
 from . import plot_utils as pltu
 
 
 class PicklingStepsStorage(object):
     """Stores the results of steps of your program in pickled form.
 
     Args:
         storage_dir (str): directory for storing your results
     """
-    def __init__(self, storage_dir):
+    def __init__(self, storage_dir: str):
         self.storage_dir = storage_dir
         pu.makedir_unless_exists(self.storage_dir)
 
-    def get_filepath(self, action, step):
+    def get_filepath(self, action: str, step: int) -> str:
         """filepath for the result of the given step of the given action in your
         program
 
         Args:
             action (str): name of an action in your program
             step (str): name of a step within that action
 
         Returns:
             str: path to the pickling file for that step of that action
         """
         return os.path.join(self.storage_dir, f"{action}_step{step}")
 
-    def delegate_ifn(self, result):
+    def delegate_ifn(self, result: Any) -> Any:
         """If the result is an ActionResultProxy, look up the action and step
         within it.
 
         Args:
             result (object): result of a step of an action
 
         Returns:
             object: the ultimate result of the given step of the given action
         """
         if isinstance(result, ActionResultProxy):
             return self.read(result.action, result.step)
         else:
             return result
         
-    def read(self, action, step):
+    def read(self, action: str, step: int) -> Any:
         """Reads the result of the given step of the given action in your
         program
 
         Args:
             action (str): name of an action in your program
             step (str): name of a step within that action
 
@@ -124,15 +125,15 @@
         """
         filepath = self.get_filepath(action, step)
         with open(filepath, 'rb') as fin:
             #return pickle.load(fin)
             result = pickle.load(fin)
         return self.delegate_ifn(result)
 
-    def write(self, action, step, result):
+    def write(self, action: str, step: int, result: Any) -> Any:
         """Write the result of the given step of the given action in your
         program
 
         Args:
             action (str): name of an action in your program
             step (str): name of a step within that action
             result (object): result to write
@@ -161,15 +162,17 @@
         steps_storage (PicklingStepsStorage): object to handle the storage of
             step results
         doc (str, optional): project docstring to be printed in the command
             line help
         with_termseq (bool): whether to color the command line output of actions
             and steps when they are executed
     """
-    def __init__(self, steps_storage, doc='', with_termseq=True):
+    def __init__(self, steps_storage: PicklingStepsStorage, doc: str = '',
+        with_termseq: bool = True
+    ):
         self.steps_storage = steps_storage
         
         self._available_actions = {}
         self.add_available(TestAction, 'test')
         self.doc = doc
         self.with_termseq = with_termseq
 
@@ -177,15 +180,15 @@
         #   are implamented as stacks.
         self._curr_action_stack = []
         self._curr_step_stack = []
         self._curr_step_method_stack = []
         self._curr_step_specs_stack = []
         self.actions_level = 0
         
-    def as_action(self, name=None):
+    def as_action(self, name: Optional[str] = None) -> Any:
         """Decorator to add the decorated class or function as an available action.
 
         Args:
             decorated (class or function): class or function to be decorated
             name (str, optional): if given, supersedes the wrapped function or
                 class name
         Returns:
@@ -196,15 +199,18 @@
                 name1 = decorated.__name__
             else:
                 name1 = name
             self.add_available(decorated, name=name1)
             return decorated
         return action
 
-    def add_available(self, obj, name=None, name_prefix='', tolerate_empty=False):
+    def add_available(
+            self, obj: Any, name: str = None, name_prefix: str = '',
+            tolerate_empty: bool = False
+    ) -> bool:
         """Add an object or a class or function as an available action if it contains
         steps.
 
         Args:
             obj: object or class or function representing an action
             name (str, optional): If omitted, the result of `_name_of_obj_or_cls`
                 is taken.
@@ -231,15 +237,17 @@
             return True
         elif not tolerate_empty:
             raise ValueError(
                 f"no step methods found in this object or class: {name}")
         return False
 
     def add_available_from_module(
-            self, module, name_prefix='', pattern_for_funcs=None, tolerate_empty=False):
+            self, module: types.ModuleType, name_prefix: str = '',
+            pattern_for_funcs: Optional[str] = None, tolerate_empty: bool = False
+    ) -> None:
         """Add all classes with step methods in the module as available actions.
 
         Args:
             module (python module object): Classes with step methods will be
                 searched here.
             name_prefix (str, optional): name prefix for all actions in this module
             pattern_for_funcs (str, optional): a regular expression, is provided,
@@ -259,15 +267,17 @@
                     anything_added |= self.add_available(obj, obj.__name__)
                 
         if not tolerate_empty and not anything_added:
             raise ValueError(
                 f"no suitable classes found in module {module.__name__}")
 
     def add_available_from_main_module(
-            self, name_prefix='', pattern_for_funcs=None, tolerate_empty=False):
+            self, name_prefix: str = '', pattern_for_funcs: Optional[str] = None,
+            tolerate_empty: bool = False
+    ) -> None:
         """Convenience function for calling `add_available_from_module` for
         the `sys.modules['__main__']`.
 
         Args:
             name_prefix (str, optional): name prefix for all actions in this module
             pattern_for_funcs (str, optional): a regular expression, is provided,
                 functions with names matching that pattern (using `re.search`)
@@ -275,16 +285,18 @@
             tolerate_empty (bool): Unless `True`, an exception is raised if no
                 streps are found
         """
         return self.add_available_from_module(
             sys.modules['__main__'], name_prefix=name_prefix,
             pattern_for_funcs=pattern_for_funcs, tolerate_empty=tolerate_empty)
 
-    def actions_loop(self, args=None, add_main=True, pattern_for_funcs=None, tolerate_empty=True
-                   ):
+    def actions_loop(
+            self, args: Optional[List[str]] = None, add_main: bool = True,
+            pattern_for_funcs: Optional[str] = None, tolerate_empty: bool = True
+    ) -> None:
         """Execute the actions as specified in the "-a", "--action" args in
         args.
 
         Args:
             args (list of str, optional): programmatic command line arguments,
                 defaulting to `sys.argv[1:]`
             add_main (bool): If yes, call `add_available_from_module` with
@@ -301,50 +313,50 @@
                 pattern_for_funcs=pattern_for_funcs)
             
         parser = self.action_parser()
         self._parse_sys_args()
         self.execute(self.args.actions)
 
     @property
-    def curr_action(self):
+    def curr_action(self) -> str:
         """The currently executed action.
 
         Returns:
             str: action name
         """
         return self._curr_action_stack[-1]
         
     @property
-    def curr_step(self):
+    def curr_step(self) -> int:
         """The currently executed step.
 
         Returns:
             int: step number
         """
         return self._curr_step_stack[-1]
 
     @property
-    def curr_step_method(self):
+    def curr_step_method(self) -> str:
         """The currently executed step method.
 
         Returns:
             str: method name
         """
         return self._curr_step_method_stack[-1]
 
     @property
-    def curr_astep(self):
+    def curr_astep(self) -> str:
         """Action and method name of the currently executed step method
 
         Returns:
             str: `<action>_<method_name>`
         """
         return f"{self.curr_action}_{self.curr_step_method}"
 
-    def execute(self, requested_action_specs):
+    def execute(self, requested_action_specs: Union[str, List[str]]) -> None:
         """Execute the registered actions and steps selected by the arguments.
 
         Args:
             requested_action_specs (str or list): either a list of arguments as produced
                 by the "-a" command line option or a single string which is then
                 split to create such a list
         """
@@ -358,15 +370,15 @@
                 else:
                     obj = obj_or_cls
 
                 self._execute1(obj, step_methods, req_steps)
             finally:
                 self._curr_action_stack.pop()
                 
-    def execute_fct_steps(self, locs):
+    def execute_fct_steps(self, locs: Dict[str, Any]) -> None:
         """Callback to be used from within function actions. It executes the
         requested steps among the steps found in the passed `locals()` dict.
         
         A function can also be an actions. Declare its steps as inner functions
         and call `execute_fct_steps(locals())` in the last line of the function
         body.
         
@@ -376,27 +388,27 @@
         """
         step_methods = self.step_methods_of_obj_cls_or_locs(locs)
         req_steps = self._translate_requested_steps(
             self.curr_action, step_methods,
             self._curr_step_specs_stack[-1])
         self._execute_steps_of_action(locs, step_methods, req_steps)
 
-    def read_result(self, action, step):
+    def read_result(self, action: str, step: int) -> Any:
         """Read the result for the given action and step from the storage.
 
         Args:
             action (str): name of an action in your program
             step (str): name of a step within that action
 
         Returns:
             object: the ultimate result of the given step of the given action
         """
         return self.steps_storage.read(action, step)
         
-    def action_parser(self):
+    def action_parser(self) -> argparse.ArgumentParser:
         """Generates the command line argument parser for the "-a", "--actions"
         arguments.
 
         This can be overridden in subclasses if this superclass method is
         called.
 
         Returns:
@@ -407,64 +419,68 @@
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
         parser.add_argument(
             '-a', "--actions", type=str, nargs='*', required=True,
             help="List of actions to execute")
         self.argparse = parser
         return parser
 
-    def _cls_of_obj_or_cls(self, obj_or_cls):
+    def _cls_of_obj_or_cls(self, obj_or_cls: Any) -> Type[Any]:
         """If the passed object is already a class, return it, otherwise return its
         class.
 
         Args:
             obj_or_cls: object or class representing an action
 
         Returns:
             class for the object
         """
         if inspect.isclass(obj_or_cls):
             return obj_or_cls
         else:
             return obj_or_cls.__class__
 
-    def _name_of_obj_or_cls(self, obj_or_cls):
+    def _name_of_obj_or_cls(self, obj_or_cls: Any) -> str:
         """Class name of the result of `_cls_of_obj_or_cls`.
 
         Args:
             obj_or_cls: object or class representing an action
 
         Returns:
             class name of the object
         """
         return self._cls_of_obj_or_cls(obj_or_cls).__name__
 
-    def _is_locals(self, obj_cls_or_locs):
+    def _is_locals(self, obj_cls_or_locs: Any) -> bool:
         """Is the argument is a locals dictionary?
 
         Args:
             obj_cls_or_locs: object or class or locals dict representing an action
         Returns:
             bool: True if it's a dictionary
         """
         return type(obj_cls_or_locs) is dict
 
-    def _entry_of_obj_cls_or_locs(self, obj_cls_or_locs, name):
+    def _entry_of_obj_cls_or_locs(
+            self, obj_cls_or_locs: Any, name: str
+    ) -> types.FunctionType:
         """The step entry for the given name in the argument.
 
         Args:
             obj_cls_or_locs: object or class or locals dict representing an action
         Returns:
             function or method corresponding to the step name
         """
         if self._is_locals(obj_cls_or_locs):
             return obj_cls_or_locs[name]
         else:
             return getattr(obj_cls_or_locs, name)
 
-    def step_methods_of_obj_cls_or_locs(self, obj_cls_or_locs):
+    def step_methods_of_obj_cls_or_locs(
+            self, obj_cls_or_locs: Any
+    ) -> collections.OrderedDict:
         """The step methods for the argument.
         
         Args:
             obj_cls_or_locs: object or class or locals dict representing an action
         Returns:
             `collections.OrderedDict`: mapping the step number to the step
             function
@@ -492,15 +508,17 @@
         step_nos.sort()
         step_methods = collections.OrderedDict([
             (step_no, step_methods[step_no]) for step_no in step_nos])
         return step_methods
     
     RE_STEP_NOT_ACTION = r'^(\d+)?(\.\.|:)?(\d+)?$'
     
-    def _translate_requested_actions(self, requested_action_specs):
+    def _translate_requested_actions(
+            self, requested_action_specs: Union[str, List[str]]
+    ) -> List[Tuple[str, List[Any]]]:
         """Translate the action specifications into a list of actions and requested
         steps.
 
         Args:
             requested_action_specs: either a string which is then split into
                 a list first; or a list of command line action specs or an action
 
@@ -562,16 +580,17 @@
                         "must be preceded by a an action.")
                 cur_step_specs[0].append(req_action)
                 
         add_requested_steps()
         return to_execute
             
     def _translate_requested_steps(
-            self, cur_action, step_methods, requested_step_specs
-    ):
+            self, cur_action: str, step_methods: Dict[int, str],
+            requested_step_specs: List[Any]
+    ) -> List[int]:
         """Translate step specifications into a list of steps.
 
         Args:
             cur_action (str): name of curr action
             step_methods (dict): mapping step number to method name
             requested_step_specs: list of integers or integer ranges built with
                 ":" or ".."
@@ -618,25 +637,25 @@
                             steps_to_add.append(stepno)
                 if not steps_to_add:
                     raise ValueError("no steps found matching the range "
                                      f"{req_action} in action {cur_action}")
                 cur_steps.extend(steps_to_add)
         return cur_steps
 
-    def _is_step_with_result(self, step_methods, step):
+    def _is_step_with_result(self, step_methods: Dict[int, str], step: int) -> bool:
         """Does the given step method produce a result?
 
         That is, does its name start with "step_r"?
         
         Returns:
             bool: True for step methods producing results
         """
         return step_methods[step].startswith('step_r')
 
-    def _method_has_params_to_read(self, obj, method_name, step):
+    def _method_has_params_to_read(self, obj: Any, method_name: str, step: int) -> bool:
         """Has the step method positional or varargs params to read?
 
         Args:
             obj: object, class or `locals()` dict representing an action
             method_name (str): method name
             step (int): step number
         Returns:
@@ -647,25 +666,27 @@
         n_positional = len(argspec.args)
         if n_positional > 0 and argspec.args[0] == 'self':
             n_positional -= 1
         if argspec.defaults is not None:
             n_positional -= len(argspec.defaults)
         return n_positional > 0 or argspec.varargs is not None
     
-    def _steps_to_read(self, obj, step_methods, req_steps):
+    def _steps_to_read(
+            self, obj: Any, step_methods: Dict[int, str], req_steps: List[int]
+    ) -> List[int]:
         """Returns the step numbers of the requested steps that have an
         positional or varargs params to read.
 
         No need to read any data if the requested methods have no input params
         to read from earlier steps.
         
         Args:
             obj: object, class or `locals()` dict representing an action
             step_methods (dict): mapping step number to method name
-            req_steps (sequence of int): requested step numbers
+            req_steps (list of int): requested step numbers
         Returns:
             list of ints: step numbers
         """
         req_steps_with_inputs = [
             step for step in req_steps
             if self._method_has_params_to_read(obj, step_methods[step], step)]
         if not req_steps_with_inputs:
@@ -675,15 +696,18 @@
         req_steps = set(req_steps)
         return [
             step for step, method_name in step_methods.items()
             if (step < max_req_step and step not in req_steps
                 and self._is_step_with_result(step_methods, step))
         ]
 
-    def _call_step_method(self, obj, method_name, cur_step, data):
+    def _call_step_method(
+            self, obj: Any, method_name: str, cur_step: int,
+            data: Dict[int, Any]
+    ) -> Any:
         """Call a step method with the required inputs.
 
         Args:
             obj: object, class or `locals()` dict representing an action
             method_name (str): method name
             cur_step (int): step number
             data (dict): mapping step number to step result
@@ -701,42 +725,46 @@
                     args.extend(result)
                 else:
                     args.append(result)
             else:
                 break
         return mthd(*args)
     
-    def _execute1(self, obj, step_methods, req_steps):
+    def _execute1(
+            self, obj: Any, step_methods: Dict[int, str], req_steps: List[int]
+    ) -> None:
         """Execute the requested steps for the given action.
 
         Args:
             obj: object, class or `locals()` dict representing an action
             step_methods (dict): mapping step number to method name
-            req_steps (sequence of int): requested step numbers
+            req_steps (list of int): requested step numbers
         """
         if step_methods is None:
             # If there are no step methods, the object must be a
             #   function. Call it. It may call {⠠d execute_fct_steps}
             #   back.
             self._curr_step_specs_stack.append(req_steps)
             try:
                 obj()
             finally:
                 self._curr_step_specs_stack.pop()
         else:
             self._execute_steps_of_action(obj, step_methods, req_steps)
 
-    def _execute_steps_of_action(self, obj, step_methods, req_steps):
+    def _execute_steps_of_action(
+            self, obj: Any, step_methods: Dict[int, str], req_steps: List[int]
+    ) -> None:
         """Execute the requested steps for the given action which mustn't be a
         function.
 
         Args:
             obj: object, class representing an action
             step_methods (dict): mapping step number to method name
-            req_steps (sequence of int): requested step numbers
+            req_steps (list of int): requested step numbers
         """
         action = self.curr_action
         # Since a requested step can be mentioned multiple times and in any
         #   order, we must first read the required results and then loop
         #   over the requested steps. A loop over all steps using a set of
         #   requested steps wouldn't do.
         data = collections.OrderedDict()
@@ -761,43 +789,42 @@
                     if self._is_step_with_result(step_methods, req_step):
                         result = self.steps_storage.write(action, req_step, result)
                         data[req_step] = result
             finally:
                 self._curr_step_method_stack.pop()
                 self._curr_step_stack.pop()
     
-    def _parse_sys_args(self, args=None):
+    def _parse_sys_args(self, args: Optional[List[str]] = None) -> None:
         """Call `action_parser`, lets it act on `args` and saves the result in
         `self.args`.
 
         Args:
             args (list of str, optional): programmatic command line arguments,
                 defaulting to `sys.argv[1:]`
         """
         if not hasattr(self, 'argparse'):
             self.action_parser()
         self.args = self.argparse.parse_args(args=args)
-        return self
 
 
 class TestAction(object):
     """Special action to call `pytest` on the module of the script used in
     the command line
     """
-    def step_0(self):
+    def step_0(self) -> None:
         with pltu.libstyle():
             pytest.cmdline.main(args=sys.argv[:1] + ['-s'])
 
 
 class ActionResultProxy:
     """Special result serving as a proxy for another result saved for a given step
     of a given action.
     
     Use this to avoid saving the same big result multiple time.
 
     Args:
         action (str): The action to refer to.
         step (str): The step of the above action to refer to.
     """
-    def __init__(self, action, step):
+    def __init__(self, action: str, step: int):
         self.action = action
         self.step = step
```

### Comparing `mlpj-0.2.1/mlpj/numpy_utils.py` & `mlpj-0.2.2/mlpj/numpy_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Utilities and convenience functions for using `numpy`.
 """
 import numpy as np
+from numpy.typing import ArrayLike
 
 
-def anynan(x):
+def anynan(x: ArrayLike) -> bool:
     """Does the input contain any NaN values?
 
     Args:
         x (array-like): input array
     Returns:
         bool: whether any NaNs were found
     """
     return np.isnan(x).any()
 
 
-def digitize(x, bins):
+def digitize(x: ArrayLike, bins: ArrayLike) -> np.ndarray:
     """An alternative version `np.digitize`. It puts x values greater or
     equal to `bins.max()` on the last index of `bins`. Values smaller than
     `bins.min()` are put on the first index of `bins`.
 
     If values in `x` are such that they fall outside the bin range,
     attempting to index `bins` with the indices that `digitize` returns
     would result in an IndexError.
```

### Comparing `mlpj-0.2.1/mlpj/pandas_utils.py` & `mlpj-0.2.2/mlpj/pandas_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 Utilities and convenience functions for using `pandas`.
 """
 import re
 import contextlib
 import collections
+from typing import Optional, Union, List, Tuple, Any, Dict
+from collections.abc import Sequence, Generator
+import types
 
 import numpy as np
+from numpy.typing import ArrayLike
 import pandas as pd
 import pandas.testing as pd_testing
 import numba
 
 from . import python_utils as pu
 
 
-def from_items(items, index=None):
+def from_items(
+        items: Sequence[Tuple[str, Any]], index: ArrayLike = None
+) -> pd.DataFrame:
     """Convert a sequence of (key, value) pairs to a DataFrame.
 
     This is similar to `pandas.DataFrame.from_items`, but with support for
     the `index` argument.
 
     In contrast to the `pandas.DataFrame` constructor using dictionaries,
     the order of the columns in the resulting dataframe will be as specified
@@ -25,50 +31,54 @@
 
     Args:
         items (seq of key-value pairs): Keys are the column names. Values
             should be array-like. All arrays have to be of equal length.
         index (array-like, optional): index to use for resulting dataframe.
             Will default to `np.arange()` if no indexing information is
             part of input data and no index is provided, see `pd.DataFrame`.
+    Returns:
+        `pd.DataFrame`
     """
     dframe = pd.DataFrame.from_dict(collections.OrderedDict(items))
     if index is not None:
         dframe.index = index
     return dframe
 
 
 @contextlib.contextmanager
-def wide_display(width=250, max_columns=75, max_rows=500):
+def wide_display(
+        width: int = 250, max_columns: int = 75, max_rows: int = 500
+) -> Generator[None]:
     """Use this for a wide and long output of `pd.DataFrame`s.
 
     Args:
         width (int): terminal width in characters
         max_columns (int): maximum number of dataframe columns
         max_rows (int): maximum number of dataframe rows
     """
     with pd.option_context("display.width", width,
                            "display.max_columns", max_columns,
                            "display.max_rows", max_rows,
                            'max_colwidth', 80):
         yield
 
 
-def is_numerical(ser):
+def is_numerical(ser: pd.Series) -> bool:
     """Does a series contain numerical values?
 
     Args:
       ser (pd.Series): input series
 
     Returns:
       bool: whether the series can be used for numerical purposes
     """
     return ser.dtype.kind in "bif"
 
 
-def get_colnames(X_or_names):
+def get_colnames(X_or_names: Any) -> List[str]:
     """Get columns from an object carrying column names
     
     Args:
         X_or_names (`pd.DataFrame` or `DataFrameGroupBy` or seq of str):
             input carrying column names
     Returns:
         list of str: list of column names
@@ -77,33 +87,37 @@
         return X_or_names.columns
     elif isinstance(X_or_names, pd.core.groupby.DataFrameGroupBy):
         return X_or_names.obj.columns
     else:
         return X_or_names
 
 
-def all_colnames_except(X_or_names, colnames):
+def all_colnames_except(
+        X_or_names: Any, colnames: Union[str, Sequence[str]]
+) -> List[str]:
     """All column names except the ones given in `colnames`.
 
     Args:
         X_or_names (`pd.DataFrame` or `DataFrameGroupBy` or seq of str):
             input carrying column names
         colnames (str or seq of str): column names to exclude
     Returns:
         list of str: remaining column names
     """
     return pu.all_except(get_colnames(X_or_names), colname_list(colnames))
 
 
-def category_colnames(df, feature_list=None):
+def category_colnames(
+        df: pd.DataFrame, feature_list: Optional[Sequence[str]] = None
+) -> List[str]:
     """The list of columns of category type
 
     Args:
         df (`pd.DataFrame`): input dataframe
-        feature_list (list of str, optional): If specified, consider only these
+        feature_list (seq of str, optional): If specified, consider only these
             columns of the dataframe.
     Returns:
         list of str: the category column names
     """
     selected = []
     for colname in df.columns:
         if df[colname].dtype.name == 'category':
@@ -111,15 +125,15 @@
     if feature_list is not None:
         selected = set(selected)
         return [feature for feature in feature_list if feature in selected]
     else:
         return selected
 
     
-def rename_column(X, old_name, new_name):
+def rename_column(X: pd.DataFrame, old_name: str, new_name: str) -> None:
     """Rename a column in the passed dataframe (in place).
 
     Args:
         X (`pd.DataFrame): input dataframe
         old_name (str): old column name
         new_name (str): new column name
 
@@ -127,40 +141,42 @@
         `ValueError` if the `old_name` isn't found among the columns.
     """
     if old_name not in X.columns:
         raise KeyError('column {} not found'.format(old_name))
     X.rename(columns={old_name: new_name}, inplace=True)
 
     
-def drop_index(X):
+def drop_index(X: pd.DataFrame) -> pd.DataFrame:
     """Drop the index from a dataframe in place.
 
     Args:
         X (`pd.DataFrame`): input dataframe
     Returns:
         X: changed in place
     """
     X.reset_index(drop=True, inplace=True)
     return X
 
 
-def drop_columns(X, columns):
+def drop_columns(X: pd.DataFrame, columns: Union[str, Sequence[str]]
+               ) -> pd.DataFrame:
     """Drop columns of a dataframe in place.
 
     Args:
         columns (str or list of str): column names to remove; don't use tuples in but
         lists.
     Returns:
         X: changed in place
     """
     X.drop(columns, axis=1, inplace=True)
     return X
 
 
-def columns_to_right(df, colnames):
+def columns_to_right(df: pd.DataFrame, colnames: Union[str, Sequence[str]]
+                   ) -> pd.DataFrame:
     """Move some column names to the right.
 
     Due to a Pandas bug, columns with texts in right-to-left writing order
     are always printed on the right end of a table. Circumvent this by
     moving these columns to the right. Then the values will be consistent
     with the headline output.
 
@@ -171,82 +187,87 @@
         `pd.DataFrame` with the columns rearranged as described
     """
     colnames = colname_list(colnames)
     colnames_set = set(colnames)
     return df[[colname for colname in df.columns if colname not in colnames_set] + colnames]
 
 
-def shuffle_df_drop_index(df):
+def shuffle_df_drop_index(df: pd.DataFrame) -> pd.DataFrame:
     """Shuffle the rows of a dataframe and drop the index.
 
     Args:
         df (`pd.DataFrame`): input dataframe
     Returns:
         `pd.DataFrame`: new dataframe
     """
     import sklearn.utils
     
     df = sklearn.utils.shuffle(df)
     drop_index(df)
     return df
 
 
-def assert_frame_contents_equal(df1, df2, **kwargs):
+def assert_frame_contents_equal(
+        df1: pd.DataFrame, df2: pd.DataFrame, **kwargs
+) -> None:
     """Convenience function to assert that the contents of two datframes is
     equal.
 
     That is, the indices of the dataframes are ignored.
 
     Args:
         df1 (`pd.DataFrame`): first input dataframe
         df2 (`pd.DataFrame`): second input dataframe
         kwargs: See `pd.testing.assert_frame_equal`.
     """
     pd_testing.assert_frame_equal(
         df1.reset_index(drop=True), df2.reset_index(drop=True), **kwargs)
 
         
-def ser_where_defined(ser):
+def ser_where_defined(ser: pd.Series) -> pd.Series:
     """Select non-null entries of a series.
 
     Args:
         ser (`pd.Series`): input series
     Returns:
         `pd.Series`: a new series containing the non-null entries.
     """
     return ser[ser.notnull()]
 
 
-def n_undefined_and_percentage(ser):
+def n_undefined_and_percentage(ser: pd.Series) -> Tuple[int, float]:
     """Number of undefined values and their percentage
 
     Args:
        ser (`pd.Series`): input series
     Returns:
        n, perc: the number of undefined values in the series and their
            percentage (scaled to 100)
     """
     return pu.wi_perc(ser.isnull().sum(), len(ser))
 
 
-def colname_list(colnames):
+def colname_list(colnames: Union[str, Sequence[str]]) -> Sequence[str]:
     """If the input is a string, turn it into a one-element list, otherwise just
     return the input.
 
     Args:
         colnames (str or list of str): input column names
     Returns:
         list of str: list of oclumn names
     """
     if pu.isstring(colnames):
         return [colnames]
     return colnames
     
 
-def sort(X, colnames=None, inplace=False, kind='stable', ascending=True):
+def sort(
+        X: pd.DataFrame, colnames: Union[str, Sequence[str]] = None,
+        inplace: bool = False, kind: str = 'stable', ascending: bool = True
+) -> pd.DataFrame:
     """Convenience function to sort a dataframe with a stable sort and ignoring
     the index.
 
     For some applications, the resorted original index is harmful.
 
     Args:
         X (`pd.DataFrame`): input dataframe
@@ -265,28 +286,28 @@
     X1 = X.sort_values(colnames, inplace=inplace, kind=kind,
                        ascending=ascending, ignore_index=True)
     if not inplace:
         X = X1
     return X
 
 
-def sorted_unique_1dim(ser):
+def sorted_unique_1dim(ser: ArrayLike) -> pd.Series:
     """The sorted series of unique values within the given series or index.
 
     Args:
         ser (`pd.Series` | `pd.Index`): input series or index
     Returns:
         `pd.Series`: unique values of the original series as a series with the
             original name
     """
     arr = np.unique(ser.values)
     return pd.Series(arr, name=ser.name)
 
 
-def left_merge(left, right, **kwargs):
+def left_merge(left: pd.DataFrame, right: pd.DataFrame, **kwargs) -> pd.DataFrame:
     """Convience function for a left merge in Pandas.
     
     `pd.DataFrame.merge` may produce result columns to in a different order
     if the left dataframe is empty. The (empty) index is also of a different
     type than for nonempty dataframes. This causes problems in `dask`. This
     wrapper function fixes the bug.
 
@@ -316,15 +337,17 @@
     if len(df) != len(left):
         raise ValueError("The left merge has a different number of rows ({}) "
                          "from the original ({})".format(len(df), len(left)))
     df.index = left.index
     return df
 
 
-def _fast_groupby_multi_transform1(igroup, work_columns, f):
+def _fast_groupby_multi_transform1(
+        igroup: np.ndarray, work_columns: np.ndarray, f: types.FunctionType
+) -> None:
     """Backend for fast_groupby_multi_transform
 
     Args:
         igroup (`np.ndarray` of int): array containing the group numbers
         nrows (int): number of rows
         work_columns (`np.ndarray` of shape `(n, d)`): the work columns
             to read and write, the result columns among them
@@ -349,17 +372,20 @@
         row_of_group_start = row_of_group_end
         
 
 _fast_groupby_multi_transform1_jit = numba.njit(_fast_groupby_multi_transform1)
 
 
 def fast_groupby_multi_transform(
-        df, group_colnames, work_colnames, result_colnames,
-        f, further_sort_colnames=[], already_sorted=False
-):
+        df: pd.DataFrame, group_colnames: Union[str, Sequence[str]],
+        work_colnames: Union[str, Sequence[str]],
+        result_colnames: Union[str, Sequence[str]],
+        f: types.FunctionType,
+        further_sort_colnames: Sequence[str] = [], already_sorted: bool = False
+) -> None:
     """Efficiently transform multiple columns as a whole for each row group.
 
     In contrast to Pandas's groupby-transform, the work columns are transformed
     as a whole rather than independently of each other. The dataframe is changed
     in place.
 
     Args:
@@ -414,26 +440,29 @@
     backend(igroup, work_columns, f)
 
     for result_colname in result_colnames:
         i = work_colnames.index(result_colname)
         df[result_colname] = work_columns[:, i]
 
 
-def flatten_multi_columns(df):
+def flatten_multi_columns(df: pd.DataFrame) -> None:
     """A multi-index for the column is flattened in place.
 
     The column levels are combined with underscores.
 
     Args:
         df (`pd.DataFrame`): input dataframe
     """
     df.columns = ['_'.join(colname).strip() for colname in df.columns.values]
 
 
-def rename_groupby_colnames(df, name_for_count=None, renamings=()):
+def rename_groupby_colnames(
+        df: pd.DataFrame, name_for_count: Optional[str] = None,
+        renamings: Union[Sequence[Tuple[str, str]], Dict[str, str]] = ()
+) -> None:
     """Rename column names as they arise from groupby-calls.
 
     The dataframe is changed in place.
     
     If a column has multiple aggregations, the tuple column names are combined
     with underscores. Otherwise just the column is used.
 
@@ -477,15 +506,18 @@
                 if name in renamings:
                     df.index.levels[i_level].name = renamings[name]
         else:
             if df.index.name in renamings:
                 df.index.name = renamings[df.index.name]
 
 
-def print_column_info(col, table_name=None, ignored_columns=(), n_value_counts=50):
+def print_column_info(
+        col: pd.Series, table_name: str = None,
+        ignored_columns: Sequence[str] = (), n_value_counts: int = 50
+) -> None:
     """Print information about a column
     
     For a column, print its `dtype`, call `describe`, count the missing
     values, count the distinct values and print the `value_counts` of up to
     `n_value_counts` most frequent values.
 
     Args:
@@ -521,15 +553,18 @@
         print(f"value counts")
         print(value_counts)
     else:
         print("value counts of the 50 most frequent values:")
         print(value_counts.iloc[:50])
 
         
-def print_table_info(df, table_name, ignored_columns=(), n_value_counts=50):
+def print_table_info(
+        df: pd.DataFrame, table_name: str,
+        ignored_columns: Sequence[str] = (), n_value_counts: int = 50
+) -> None:
     """Print information about a dataframe's columns.
     
     For a dataframe, print its shape, column dtypes and call
     `print_column_info` for each column (except the ones in `ignored_columns`).
 
     Args:
         df (`pd.DataFrame`): the input dataframe
@@ -543,15 +578,18 @@
     print(df.dtypes)
     for colname in df.columns:
         print_column_info(
             df[colname], table_name=table_name, ignored_columns=ignored_columns,
             n_value_counts=n_value_counts)
 
 
-def consistency_check(df, colname_a, colname_b, n_examples=50, extra_colnames=[]):
+def consistency_check(
+        df: pd.DataFrame, colname_a: str, colname_b: str,
+        n_examples: int = 50, extra_colnames: Sequence[str] = []
+) -> None:
     """Print a report about inconsistencies between two columns.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         colname_a (str): first column name to compare
         colname_b (str): second column name to compare
         n_examples (int): number of inconsistency examples to show
@@ -578,65 +616,65 @@
             print("all inconsistencies:")
         else:
             examples = examples.iloc[-n_examples:]
             print(f"the last {len(examples)} inconsistencies:")
         print(examples)
 
         
-def keys_of_dict_column(ser):
+def keys_of_dict_column(ser: pd.Series) -> pd.Series:
     """Transform a series with dict values into a series with the lists of their
     keys.
 
     Args:
         ser (`pd.Series`): input series with `dict` entries
     Returns:
         `pd.Series`: a new series containing the list of keys for each entry
     """
     return ser.transform(lambda   dic: list(dic.keys()))
 
 
-def distinct_keys_of_dict_column(ser):
+def distinct_keys_of_dict_column(ser: pd.Series) -> np.ndarray:
     """For a series with dict values, extract the distinct lists of keys
     these dicts.
 
     Args:
         ser (`pd.Series`): input series with `dict` entries
     Returns:
         `np.ndarray`: array of distinct lists of keys
     """
     return np.unique(keys_of_dict_column(ser))
 
 
-def truncate_datetime_to_freq(ser, freq):
+def truncate_datetime_to_freq(ser: pd.Series, freq: str) -> pd.Series:
     """Truncate datetime values to the specified period.
 
     Args:
         ser (`pd.Series`): input series
         freq (str): Pandas frequency or frequency alias
     Returns:
         `pd.Series` with truncated datetime values
     """
     return ser.dt.to_period(freq).dt.start_time
 
 
-def truncate_datetime_to_month(ser):
+def truncate_datetime_to_month(ser: pd.Series) -> pd.Series:
     """Truncate datetime values to the beginning of the month.
 
     Special case of `truncate_datetime_to_freq` with frequency 'M'.
     
     Args:
         ser (`pd.Series`): input series
     Returns:
         `pd.Series` with datetime values truncated to the beginning of the
         respective month
     """
     return truncate_datetime_to_freq(ser, 'M')
 
 
-def truncate_datetime_to_week(ser, sunday_first=False):
+def truncate_datetime_to_week(ser: pd.Series, sunday_first: bool = False) -> pd.Series:
     """Truncate datetime values to the beginning of the week.
 
     Special case of `truncate_datetime_to_freq`.
     
     Args:
         ser (`pd.Series`): input series
         sunday_first (bool): whether to consider Sunday the beginning of the week;
@@ -651,29 +689,29 @@
         freq = 'W'
     return truncate_datetime_to_freq(ser, freq)
 
 
 MIN_DATETIME = pd.to_datetime("1970-01-01")
 
 
-def datetime_to_epoch(ser):
+def datetime_to_epoch(ser: pd.Series) -> pd.Series:
     """Convert a Pandas datetime series to a float epoch, including the
     nanoseconds.
     
     NaT values are converted to NaT values.
 
     Args:
         ser (`pd.Series`): input deries
     Returns:
         `pd.Series`: output series containing float epochs
     """
     return (ser - MIN_DATETIME).dt.total_seconds()
 
 
-def to_csv(df, filepath, **kwargs):
+def to_csv(df: pd.DataFrame, filepath: str, **kwargs) -> None:
     """Convenience function to call `pd.DataFrame.to_csv` with common
     defaults.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         file (str or stream): CSV filepath to create or stream to write to
         kwargs: See `pd.DataFrame.to_csv`.
```

### Comparing `mlpj-0.2.1/mlpj/plot_utils.py` & `mlpj-0.2.2/mlpj/plot_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Utilities and convenience functions for `matplotlib`
 """
 import collections
 import warnings
+from typing import Optional, Any, Tuple
 
 import contextlib
 import numpy as np
+from numpy.typing import ArrayLike
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 from matplotlib import gridspec
 
 from . import numpy_utils as npu
 from . import pandas_utils as pdu
 
 
 LOWER_1_SIGMA_QUANTILE = (1. - 0.6827) / 2
 LOWER_2_SIGMA_QUANTILE = (1. - 0.9545) / 2
 
 
 @contextlib.contextmanager
-def libstyle():
+def libstyle() -> None:
     """Context manager to set some `matplotlib` styles temporarily"""
     orig_params = list(mpl.rcParams.items())
     try:
         mpl.rcParams['grid.color'] = '#000000'
         mpl.rcParams['grid.alpha'] = 0.1
         mpl.rcParams['grid.linestyle'] = '-'
         mpl.rcParams['lines.markersize'] = 3.0
@@ -46,15 +48,15 @@
     finally:
         mpl.rcParams.clear()
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             mpl.rcParams.update(orig_params)
 
 
-def xytitle(xlabel=None, ylabel=None, title=None):
+def xytitle(xlabel: str = None, ylabel: str = None, title: str = None) -> None:
     """Add labels for the x-axis, y-axis and / or the whole plot.
     
     Args:
         xlabel (str, optional): label for the x-axis
         ylabel (str, optional): label for the y-axis
         title (str, optional): label for the plot
     """
@@ -62,29 +64,30 @@
         plt.xlabel(xlabel)
     if ylabel is not None:
         plt.ylabel(ylabel)
     if title is not None:
         plt.title(title)
 
 
-def histogram_of_col(col):
+def histogram_of_col(col: pd.Series) -> None:
     """Plot a histogram of the given column and add titles.
 
     Args:
         col (`pd.Series`): the data column to plot
     """
     colname = col.name
     #n_notnull = len(col[col.notnull()].drop_duplicates())
     #col.hist(bins=min(n_bins, n_notnull), backend='seaborn')
     #plt.hist(col.values, bins=min(n_bins, n_notnull), #align='right')
     plt.hist(col.values, bins='sqrt')
     xytitle(colname, "n", f"histogram of {colname}")
 
 
-def plot_all_numerical_histograms(pj, df, table_name):
+def plot_all_numerical_histograms(pj, df: pd.DataFrame, table_name: str
+) -> None:
     """Plot the histograms of all numerical columns.
 
     Each plot will be generated unter the key
     `<table_name>_<colname>_histogram`.
     
     Args:
         pj (`project_utils.Manager`): project manager to handle the plots
@@ -115,16 +118,17 @@
         n_plots (int, optional) number of subplots to put in the grid; either
             this or `n_rows` must be specified
         n_rows (int, optional): number of rows to put in the grid; either this
             or `n_plots` must be specified
         n_cols (int): number of subplots per row
         For the other parameters, see `matplotlib.gridspec.GridSpec`.
     """
-    def __init__(self, n_plots=None, n_rows=None, n_cols=None, width_ratios=None, height_ratios=None,
-        wspace=None, hspace=None
+    def __init__(self, n_plots: int = None, n_rows: int = None, n_cols: int = None,
+        width_ratios: ArrayLike = None, height_ratios: ArrayLike = None,
+        wspace: Optional[float] =None, hspace: Optional[float] =None
     ):
         if n_cols is None:
             raise ValueError('n_cols is mandatory')
 
         if n_plots is not None and n_rows is None:
             n_rows = int(np.ceil(n_plots / n_cols))
         elif n_rows is not None and n_plots is None:
@@ -143,26 +147,26 @@
             axes.set_xticks([])
             axes.set_yticks([])
             self.gridspec = gridspec.GridSpecFromSubplotSpec(
                 self.n_rows, self.n_cols, subplot_spec=self.containing_gridspec,
                 width_ratios=width_ratios, height_ratios=height_ratios,
                 wspace=wspace, hspace=hspace)
 
-    def subplot(self, i_plot):
+    def subplot(self, i_plot: int) -> mpl.axes.Axes:
         """Go to the i-th subplot and return the corresponding axes object.
 
         The attribute `containing_gridspec` is set in the `axes` object.
         This way, `get_containing_gridspec` can determine whether an
         `axes` object is contained in a `PlotGrid` or not and what its
         corresponding `gridspec` is.
 
         Args:
             i_plot (int): plot number
         Returns:
-            `matplotlib.axes.AxesSubplot`: axes object of the i-th subplot in
+            `matplotlib.axes.Axes`: axes object of the i-th subplot in
             the grid
         """
         gridspec = self.gridspec[i_plot]
         if self.containing_gridspec is None:
             axes = plt.subplot(gridspec)
         else:
             figure = plt.gcf()
@@ -177,22 +181,22 @@
 
         This method delegates to `matplotlib.gridspec.GridSpec.update` of the
         internal `matplotlib.gridspec.GridSpec` object.
         """
         self.gridspec.update(**kwargs)
         
 
-def get_containing_gridspec(axes):
+def get_containing_gridspec(axes: mpl.axes.Axes) -> mpl.gridspec.SubplotSpec:
     """Return the gridspec containing this axes object, if applicable.
 
     `PlotGrid.subplot` sets the attribute `containing_gridspec` in the
     subplot axes object to the corresponding gridspec item.
 
     Args:
-        axes (`matplotlib.axes.AxesSubplot`): axes object of a subplot
+        axes (`matplotlib.axes.Axes`): axes object of a subplot
     Returns:
         `matplotlib.gridspec.SubplotSpec` or `None`:
         If the axes object hasn't been created by `PlotGrid.subplot`,
         the result is None, otherwise it's the corresponding `gridspec` item.
     """
     if not hasattr(axes, 'containing_gridspec'):
         return None
@@ -200,16 +204,18 @@
         return axes.containing_gridspec
 
         
 LOWER_1_SIGMA_QUANTILE = (1. - 0.6827) / 2
 LOWER_2_SIGMA_QUANTILE = (1. - 0.9545) / 2
 
 
-def histogram_plot(bin_contents, bin_boundaries, yscale='linear',
-                 orientation='vertical'):
+def histogram_plot(
+        bin_contents: ArrayLike, bin_boundaries: ArrayLike,
+        yscale: str = 'linear', orientation: str = 'vertical'
+) -> None:
     """Plot a histogram for the given bin boundaries and bin contents.
 
     Args:
         bin_contents (series-like of shape `(n,)`): count for each bin.
         bin_boundaries (series-like of shape `(n + 1,)`): left and right
             boundaries for all bins
         yscale ('linear' | 'log'):
@@ -259,17 +265,20 @@
             plt.ylim(count_min, count_max)
         else:
             plt.xlim(count_max, count_min)
             locs, labels = plt.xticks()
             plt.setp(labels, rotation=70)
     
     
-def profile_plot(x, y, n_bins=100, equal_n_datapoints=False, n_ticks=10,
-               is_continuous_x=True, errorbars='quantile', histogram='linear',
-               density=None, with_median=True):
+def profile_plot(
+        x: ArrayLike, y: ArrayLike, n_bins: int = 100, equal_n_datapoints: bool = False,
+        n_ticks: int = 10, is_continuous_x: bool = True,
+        errorbars: str = 'quantile', histogram: str = 'linear',
+        density: Optional[str] = None, with_median: bool = True
+) -> None:
     """Profile plot of one column versus another.
     
     The x-axis represents the values of `x`, the y-axis the values of `y`.
     For each x-bin, the distribution of y-values is visualized by this plot:
     the mean y (in blue), optionally the median y (in green), the 1-sigma error
     bar (in green) and the 2-sigma error bar (in yellow).
     
@@ -432,18 +441,19 @@
                 axes_right.set_xticklabels(
                     reduce_labels(axes_right.get_xticklabels()))
     
         plt.sca(axes_main)
 
 
 def diagonal_plot_for_prediction(
-        pred, y, n_bins=100, n_ticks=10, errorbars='quantile',
-        xlabel="Prediction", ylabel="Truth", histogram='linear',
-        with_median=True
-):
+        pred: ArrayLike, y: ArrayLike, n_bins: int = 100, n_ticks: int = 10,
+        errorbars: str = 'quantile', xlabel: str = "Prediction",
+        ylabel: str = "Truth", histogram: str ='linear',
+        with_median: bool = True
+) -> None:
     """Diagonal plot of a prediction on test data with median and error bars
     for 1 sigma ranges and 2 sigma ranges in each bin.
 
     The x-axis represents the predictions, the y-axis the true values in
     training or test data. For each prediction bin, the distribution of true
     values is visualized by this plot: the mean target (in blue), optionally
     the median target (in green), the 1-sigma error bar (in green) and the 2-sigma
@@ -489,15 +499,17 @@
         xmin, xmax = plt.xlim()
         plt.plot([xmin, xmax], [xmin, xmax], 'k', linewidth=0.4)
         # Axis labels:
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
 
 
-def _calc_statistics(x, y, errorbars):
+def _calc_statistics(
+        x: ArrayLike, y: ArrayLike, errorbars: str
+) -> Tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike]:
     """Calculate means, medians, errors, counts for each bin.
     
     Args:
         x (series-like): binned x-values
         y (series-like): y-values
         errorbars (str): See the same param in `profile_plot`.
     Returns:
@@ -532,15 +544,18 @@
         n = groupby.size()
         k = groupby.aggregate(np.sum)  # y = 1 or y = 0
         prior = 1
         errors = npu.beta_posterior_uncertainty(k, n, prior, prior)
     return means, medians, errors, counts
     
 
-def _profile_plot_discrete(x, y, errorbars, with_median=True):
+def _profile_plot_discrete(
+        x: ArrayLike, y: ArrayLike, errorbars: str,
+        with_median: bool = True
+) -> None:
     """Profile plot implementation for discrete x-values.
 
     Args:
         x (series-like): x-values
         y (series-like): y-values
         errorbars (str): See the same param in `profile_plot`.
     """
@@ -555,15 +570,17 @@
         xmax = len(means) + 0.5
         plt.xlim(xmin, xmax)
         _plot_bin_results(bin_centers, means.values, medians.values,
                           np.asarray(errors), errorbars, with_median=with_median)
         return bin_boundaries, np.asarray(counts)
 
 
-def _reduce_xticks(locations, labels, n_ticks):
+def _reduce_xticks(
+        locations: ArrayLike, labels: ArrayLike, n_ticks: int
+) -> Tuple[ArrayLike, ArrayLike]:
     """Recduce the number of ticks to plot.
 
     Args:
         locations (series-like): locations of the bins
         labels (series-like): tick labels for the bins
         n_ticks (int, optional): number of ticks
 
@@ -595,16 +612,18 @@
         chosen_labels.pop()
         chosen_labels.append('')
         add_entry(n - 1)
 
     return chosen_locations, chosen_labels
 
 
-def _profile_plot_continuous(x, y, n_bins, equal_n_datapoints, n_ticks,
-                           errorbars, with_median=True):
+def _profile_plot_continuous(
+        x: ArrayLike, y: ArrayLike, n_bins: int, equal_n_datapoints: bool,
+        n_ticks: int, errorbars: str, with_median: bool = True
+) -> None:
     """Profile plot implementation for continuous x-values.
 
     Args:
         See `profile_plot` for the params with the same names.
     """
     with libstyle():
         if equal_n_datapoints:
@@ -642,24 +661,29 @@
                   2 * bin_boundaries[-1] - bin_centers[-1]])
         
         if not equal_n_datapoints:
             assert len(bin_boundaries) == len(counts) + 1
         return bin_boundaries, np.asarray(counts)
 
     
-def _create_bottom_right_axes(equal_n_datapoints, histogram_x, histogram_y):
+def _create_bottom_right_axes(
+        equal_n_datapoints: bool, histogram_x: str, histogram_y: bool
+) -> Tuple[mpl.axes.Axes, mpl.axes.Axes, mpl.axes.Axes,
+     mpl.axes.Axes] :
     """Create axes objects for the bottom and/or the right of the current axes.
 
     Args:
         equal_n_datapoints (bool): If `True`, bins with approximately equal
             number of data points are chosen instead of equidistant bins.
         histogram_x (str or `None`): the kind of histogram to plot for the x-axis;
             see param `histogram` in `profile_plot`.
         histogram_y (str or `None`): the kind of histogram to plot for the y-axis;
             see param `histogram` in `profile_plot`.
+    Returns:
+        axes_main, axes_bottom, axes_right, original_axes
     """
     original_axes = plt.gca()
 
     if histogram_x is None and histogram_y is None:
         return original_axes, None, None, original_axes
 
     if histogram_x is not None:
@@ -697,26 +721,30 @@
     else:
         axes_bottom = None
 
     plt.sca(axes_main)
     return axes_main, axes_bottom, axes_right, original_axes
 
 
-def _set_yticks_and_labels(axis, y_ticks, y_ticklabels):
+def _set_yticks_and_labels(axis: mpl.axes.Axes, y_ticks: ArrayLike,
+                         y_ticklabels: ArrayLike) -> None:
     """Workaround to set yticks and labels.
     
     https://stackoverflow.com/questions/63723514/userwarning-fixedformatter-should-only-be-used-together-with-fixedlocator
     """
     if y_ticks is None:
         y_ticks = axis.get_yticks()
     axis.set_yticks(y_ticks)
     axis.set_yticklabels(y_ticklabels)
 
 
-def _plot_bin_results(x, means, medians, errors, errorbars, with_median=True):
+def _plot_bin_results(
+        x: ArrayLike, means: ArrayLike, medians: ArrayLike,
+        errors: ArrayLike, errorbars: str, with_median: bool = True
+) -> None:
     """Plot results for each bin
 
     Args:
         x (array-like, shape `(n,)): binned x-values
         means (array-like, shape `(n,)): mean of y for each x-bin
         medians (array-like, shape `(n,)): median of y for each x-bin
         errors (array-like, shape `(n, 4)): boundaries of 1-sigma and 2-sigma
```

### Comparing `mlpj-0.2.1/mlpj/project_utils.py` & `mlpj-0.2.2/mlpj/project_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import os
 import sys
 import re
 import random
 import contextlib
 import tempfile
+from typing import Optional, Any, List, Union
+from collections.abc import Generator
 
 import numpy as np
 
 from . import python_utils as pu
 from . import result_display, actions_looper
 
 
@@ -36,15 +38,15 @@
       commands like (`savefig`, `printer`), linking to the images in the image
       directory above
     * `<project_path>/html/index.html`: the default HTML page generated by
       `result_display` commands
     * `<project_path>/contents.db`: Sqlite database used by `result_display`
       commands
     """
-    def __init__(self, project_path, seed=None, doc=None):
+    def __init__(self, project_path: str, seed: Optional[int] = None, doc: Optional[str] = None):
         self.project_dir = os.path.abspath(os.path.expanduser(project_path))
         pu.makedir_unless_exists(self.project_dir)
         self.name = os.path.basename(self.project_dir)
         
         self.db_path = os.path.join(self.project_dir, "contents.db")
         self.html_path = os.path.join(self.project_dir, "html")
         self.htmlind_path = os.path.join(self.html_path, "index.html")
@@ -63,144 +65,140 @@
         doc = f"{self.name}\n{doc}"
         
         steps_storage = actions_looper.PicklingStepsStorage(
             os.path.join(self.project_dir, "steps"))
 
         self.actions_looper = actions_looper.ActionsLooper(steps_storage, doc=doc)
     
-    def as_action(self, *args, **kwargs):
+    def as_action(self, *args, **kwargs) -> Any:
         """delegates to `actions_looper.ActionsLooper.action`"""
         return self.actions_looper.as_action(*args, **kwargs)
 
-    def add_available(self, *args, **kwargs):
+    def add_available(self, *args, **kwargs) -> bool:
         """delegates to `actions_looper.ActionsLooper.add_available`"""
         return self.actions_looper.add_available(*args, **kwargs)
     
-    def add_available_from_module(self, *args, **kwargs):
+    def add_available_from_module(self, *args, **kwargs) -> None:
         """delegates to `actions_looper.ActionsLooper.add_available_from_module`
         """
         return self.actions_looper.add_available_from_module(*args, **kwargs)
     
-    def add_available_from_main_module(self, *args, **kwargs):
+    def add_available_from_main_module(self, *args, **kwargs) -> None:
         """delegates to
         `actions_looper.ActionsLooper.add_available_from_main_module`
         """
         return self.actions_looper.add_available_from_main_module(*args, **kwargs)
 
     
-    def actions_loop(self, *args, **kwargs):
+    def actions_loop(self, *args, **kwargs) -> None:
         """delegates to `actions_looper.ActionsLooper.actions_loop`"""
         return self.actions_looper.actions_loop(*args, **kwargs)
 
     
     @property
-    def curr_action(self):
+    def curr_action(self) -> str:
         """delegates to `actions_looper.ActionsLooper.curr_action`"""
         return self.actions_looper.curr_action
         
     @property
-    def curr_step(self):
+    def curr_step(self) -> int:
         """delegates to `actions_looper.ActionsLooper.curr_step`"""
         return self.actions_looper.curr_step
         
     @property
-    def curr_astep(self):
-        """delegates to `actions_looper.ActionsLooper.curr_astep`"""
-        return self.actions_looper.curr_astep
-        
-    @property
-    def curr_step_method(self):
+    def curr_step_method(self) -> str:
         """delegates to `actions_looper.ActionsLooper.curr_step_method`"""
         return self.actions_looper.curr_step_method
+        
+    @property
+    def curr_astep(self) -> str:
+        """delegates to `actions_looper.ActionsLooper.curr_astep`"""
+        return self.actions_looper.curr_astep
     
-    def execute(self, *args, **kwargs):
+    def execute(self, *args, **kwargs) -> None:
         """delegates to `actions_looper.ActionsLooper.execute`"""
         return self.actions_looper.execute(*args, **kwargs)
     
-    def execute_fct_steps(self, *args, **kwargs):
+    def execute_fct_steps(self, *args, **kwargs) -> None:
         """delegates to `actions_looper.ActionsLooper.execute_fct_steps`"""
         return self.actions_looper.execute_fct_steps(*args, **kwargs)
     
-    def read_result(self, action, step):
+    def read_result(self, action: str, step: int) -> Any:
         """delegates to `actions_looper.ActionsLooper.read_result`"""
         return self.actions_looper.read_result(action, step)
 
     
-    def printer(self, *args, **kwargs):
+    def printer(self, *args, **kwargs) -> None:
         """delegates to `result_display.HTMLDisplay.printer`"""
         return self.display.printer(*args, **kwargs)
 
-    def print(self, *args, **kwargs):
+    def print(self, *args, **kwargs) -> None:
         """delegates to `result_display.HTMLDisplay.print`"""
         return self.display.print(*args, **kwargs)
         
-    def savefig(self, *args, **kwargs):
+    def savefig(self, *args, **kwargs) -> None:
         """delegates to `result_display.HTMLDisplay.savefig`"""
         return self.display.savefig(*args, **kwargs)
     
-    def add_db_entry(self, *args, **kwargs):
+    def add_db_entry(self, *args, **kwargs) -> None:
         """delegates to `result_display.HTMLDisplay.add_db_entry`"""
         return self.display.add_db_entry(*args, **kwargs)
         
-    def link_text(self, *args, **kwargs):
+    def link_text(self, *args, **kwargs) -> str:
         """delegates to `result_display.HTMLDisplay.link_text`"""
         return self.display.link_text(*args, **kwargs)
     
-    def print_link_and_return_filepath(self, filename, remark=''):
+    def print_link_and_return_filepath(self, filename: str, remark: str = '') -> str:
         """Create a filepath for the given filename in the image directory and
         print an HTML link to it.
 
         Args:
             filename (str): filename (no directory)
             remark (str, optional): remark to print before the link text
         Returns:
             str: filepath in the image directory
         """
         filepath = os.path.join(self.image_path, filename)
         link_text = self.display.link_text(filepath, link_text=filename)
         print(f'{remark}{link_text}')
         return filepath
 
-    def get_analysis_pdf_filepath(self, model_name, iteration=-1):
+    def get_analysis_pdf_filepath(self, model_name: str, iteration: int =-1) -> str:
         """Filepath to save a Cyclic Boosting analysis PDF in.
         
         Args:
             model_name (str): model name
             iteration (int): Cyclic Boosting iteration
         Returns:
             str: filepath in the image directory
         """
         if iteration == -1:
             suffix = ""
         else:
             suffix = f"_{iteration}"
         return os.path.join(self.image_path, f"{model_name}{suffix}.pdf")
     
-    def get_keys(self):
+    def get_keys(self) -> List[str]:
         """delegates to `result_display.HTMLDisplay.get_keys`"""
         return self.display.get_keys()
 
-    def del_keys(self, keys):
+    def del_keys(self, keys: Union[str, List[str]]) -> None:
         """delegates to `result_display.HTMLDisplay.del_keys`"""
         return self.display.del_keys(keys)
 
-    def del_keys_like(self, regex):
+    def del_keys_like(self, regex: str) -> None:
         """delegates to `result_display.HTMLDisplay.del_keys_like`"""
         return self.display.del_keys_like(regex)
 
-    def get_findings(self):
+    def get_findings(self) -> List[Any]:
         """delegates to `result_display.HTMLDisplay.db_findings"""
         return self.display.get_findings()
-    
-    def generate_htmlpage(self, *args, **kwargs):
-        """delegates to `result_display.HTMLDisplay.generate_htmlpage`"""
-        return self.display.generate_htmlpage(*args, **kwargs)
 
 
 @contextlib.contextmanager
-def temp_project():
+def temp_project() -> Generator[Manager]:
     """Context manager offering a temporary project
 
     For example for testing purposes.
     """
     with tempfile.TemporaryDirectory() as tmpdir:
         yield Manager(tmpdir)
```

### Comparing `mlpj-0.2.1/mlpj/python_utils.py` & `mlpj-0.2.2/mlpj/python_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,43 @@
 import os
 import sys
 import sqlite3
 import datetime
 import contextlib
 import tempfile
 import logging
+from typing import Any, List, Tuple, Union, TextIO, BinaryIO
+from collections.abc import Sequence, Generator
 
 
-def all_except(seq, omissions):
+def all_except(seq: Sequence[Any], omissions: Sequence[Any]) -> List[Any]:
     """All entries of a list except the one mentioned in `omissions`.
 
     Args:
         seq (seq): sequence of objects
         omissions (seq): sequence of omissions
     Returns:
         list of remaining objects
     """
     omissions = set(omissions)
     return [entry for entry in seq if entry not in omissions]
 
 
-def isstring(s):
+def isstring(s: Any) -> bool:
     """Is the argument a string?
 
     Args:
         s: object
     Returns:
         bool: whether it is of type `str` or `bytes`
     """
     return isinstance(s, (str, bytes))
 
 
-def if_true(flag, value, default=''):
+def if_true(flag: bool, value: Any, default: str = '') -> Any:
     """If the flag is true, return the value, otherwise the default.
 
     Args:
         flag (bool): control flag
         value (object): value to return if the flag is true
         default (object): value to return if the flag is false
     Returns:
@@ -46,62 +48,62 @@
     """
     if flag:
         return value
     else:
         return default
     
 
-def wi_perc(value, reference):
+def wi_perc(value: float, reference: float) -> Tuple[float, float]:
     """Return the value and the percentage of the value in the reference.
 
     Args:
         value (number): value to compare
         reference (number): total amount
     Returns:
         value, perc: The original value and the percentage (scaled to 100)
     """
     return value, value / reference * 100.
 
 
-def perc_str(value, reference):
+def perc_str(value: float, reference: float) -> str:
     """Return a string with the value and the percentage of the value in
     the reference.
 
     Args:
         value (number): value to compare
         reference (number): total amount
     Returns:
         str: value with percentage
     """
     _, perc = wi_perc(value, reference)
     return f"{value} ({perc:.2f} %)"
 
 
-def first_of_each_item(items):
+def first_of_each_item(items: Sequence[Any]) -> List[Any]:
     """The first subitem of each item in the input
 
     Args:
-        items (list of indexable objects): input list of items
+        items (sequence of indexable objects): input list of items
     Returns:
         list of objects: For each item in the input, `item[0]`.
     """
     return [item[0] for item in items]
 
 
-def makedir_unless_exists(dirpath):
+def makedir_unless_exists(dirpath: str) -> None:
     """Create a directory path unless it already exists.
 
     Args:
         dirpath (str): directory path
     """
     if not os.path.isdir(dirpath):
         os.makedirs(dirpath)
 
 
-def make_path_relative_to(filepath, reference_path):
+def make_path_relative_to(filepath: str, reference_path: str) -> str:
     """Make a filepath relative to a given reference path.
 
     This is needed for HTML links to images, for example.
 
     Args:
         filepath (str): input filepath
         reference_path (str): reference filepath
@@ -115,15 +117,15 @@
     for i, part in enumerate(parts):
         if i >= n_ref or part != parts_ref[i]:
             break
     return os.path.join(*(['..'] * (n_ref - i) + parts[i:]))
 
 
 @contextlib.contextmanager
-def redirect_stdouterr(outfp, errfp):
+def redirect_stdouterr(outfp: TextIO, errfp: TextIO) -> Generator[None]:
     """Context manager for temporary redirection of `sys.stdout` and
     `sys.stderr`.
     
     Args:
         outfp (output stream): output stream to redirect the standard output
             stream to (default=`os.devnull`)
         errfp (output stream): path or output stream to redirect
@@ -147,39 +149,41 @@
         
 class BranchedOutputStreams:
     """Output stream that delegates to multiple other output streams
 
     Args:
         streams (seq of output streams): output streams to delegate to
     """
-    def __init__(self, streams):
+    def __init__(self, streams: Sequence[TextIO]):
         self.streams = streams
 
-    def write(self, message):
+    def write(self, message: str) -> None:
         """Write a message to all output streams.
 
         Args:
             message (str): message to write
         """
         for stream in self.streams:
             stream.write(message)
 
-    def flush(self):
+    def flush(self) -> None:
         """Flush all output streams."""
         for stream in self.streams:
             stream.flush()
 
-    def close(self):
+    def close(self) -> None:
         """Close all output streams."""
         for stream in self.streams:
             stream.close()
 
         
 @contextlib.contextmanager
-def open_overwriting_safely(filepath, mode):
+def open_overwriting_safely(
+        filepath: str, mode: int
+) -> Generator[Union[TextIO, BinaryIO]]:
     """Open a temporary file and rename it in the end.
 
     Instead of overwriting the given file directly, open a temporary file
     in the same directory, write into it and rename the temporary file to the
     given filepath in the end.
 
     This way, if an exception occurs, the original file contents is preserved.
@@ -198,15 +202,15 @@
         os.rename(filepath_tmp, filepath)
         filepath_tmp = None
     finally:
         if filepath_tmp is not None and os.path.exists(filepath_tmp):
             os.remove(filepath_tmp)
 
 
-def ansiicol(color_num, is_bright=False):
+def ansiicol(color_num: int, is_bright: bool = False) -> str:
     """ANSI escape code for the given color number
     https://en.wikipedia.org/wiki/ANSI_escape_code
 
     Args:
         color_num (int): color number
         is_bold (bool): whether to use bold face
     Returns:
@@ -232,15 +236,15 @@
     'br_blue[': ansiicol(34, True),
     #'bold[': "\x1b[30;1m",
     ']': "\x1b[0m",
 }
 
 
 @contextlib.contextmanager
-def sqlite3_conn(filepath):
+def sqlite3_conn(filepath) -> Generator[Tuple[sqlite3.Connection, sqlite3.Cursor]]:
     """Context manager for a connection to a Sqlite3 database file
 
     Args:
         filepath (str): filepath to the database file
     Yielding:
         db, cursor; the database connection and the cursor
     """
@@ -258,35 +262,35 @@
 
 
 SECONDS_IN_HOUR = 3600
 
 SECONDS_IN_DAY = 24 * SECONDS_IN_HOUR
 
     
-def n_days_ago(n_days):
+def n_days_ago(n_days: int) -> datetime.datetime:
     """The datetime object for the day n_days days ago
 
     Args:
         n_days (int): number of days to go into the past
     Returns:
         `datetime.datetime`: datetime object for that day in the past
     """
     return datetime.date.today() - datetime.timedelta(n_days)
 
 
-def today_isoformat():
+def today_isoformat() -> str:
     """Today in ISO date format
 
     Returns:
         str: in ISO date format
     """
     return datetime.date.today().isoformat()
 
 
-def create_console_logger(module, level=logging.DEBUG):
+def create_console_logger(module: str, level: int = logging.DEBUG) -> logging.Logger:
     """Create a default console logger for a given module.
 
     Args:
         module (str): module name
         level (int): logging level
     Returns:
         `logging.Logger`
```

### Comparing `mlpj-0.2.1/mlpj/result_display.py` & `mlpj-0.2.2/mlpj/result_display.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 import os
 import sys
 import re
 import logging
 import time
 import io
+import sqlite3
+from typing import Tuple, Optional, List, Union, Any
 
 import contextlib
 import jinja2
 import markupsafe
 import numpy as np
 import pandas as pd
 
@@ -66,18 +68,18 @@
         further_html_headers (str, optional): further headers to add to the
             generated HTML pages
         refresh_how_long (float): upper limit for the number of seconds to run the
             refresh loop (only used if plots request refreshing)
         refresh_not_started_after (float): upper limit for the number of seconds
             after creating the plot to ignore requests for refreshing
     """
-    def __init__(self, db_path, project_name, html_dir, image_dir,
-        default_figsize=(8, 6), further_html_headers='',
-        refresh_how_long=pu.SECONDS_IN_HOUR // 2,
-        refresh_not_started_after=pu.SECONDS_IN_DAY // 2,
+    def __init__(self, db_path: str, project_name: str, html_dir: str, image_dir: str,
+        default_figsize: Tuple[float, float] = (8, 6), further_html_headers: str = '',
+        refresh_how_long: float = pu.SECONDS_IN_HOUR // 2,
+        refresh_not_started_after: float = pu.SECONDS_IN_DAY // 2,
     ):
         self.db_path = os.path.abspath(db_path)
 
         with open(os.path.join(os.path.dirname(__file__), "result_template.html")
         ) as fin:
             self.html_template = jinja2.Template(fin.read())
 
@@ -98,15 +100,16 @@
         self.html_index_filename = 'index.html'
         self.default_figsize = default_figsize
         self.further_html_headers = further_html_headers
         self.refresh_how_long = refresh_how_long
         self.refresh_not_started_after = refresh_not_started_after
     
     @contextlib.contextmanager
-    def printer(self, key, suppl=False, silence_stdout=False, preformatted=True):
+    def printer(self, key: str, suppl: bool = False, silence_stdout: bool = False,
+              preformatted: bool = True) -> None:
         """Context manager to add the output printed in the context manager's
         block to the database under the given key and regenerate the
         corresponding HTML page.
 
         If there's an exception in the user block, the outputs printed so far
         are preserved.
         
@@ -126,23 +129,24 @@
                 with pdu.wide_display():
                     yield key
         finally:
             content = out.getvalue().rstrip()
             self.print(key, content, suppl=suppl, silence_stdout=silence_stdout,
                     preformatted=preformatted)
 
-    def print(self, key, content, suppl=False, silence_stdout=False, preformatted=False):
+    def print(self, key: str, content: str, suppl: bool = False,
+            silence_stdout: bool = False, preformatted: bool = False) -> None:
         """Print and add the output to the database under the given key and
         regenerate the corresponding HTML page.
 
         Do nothing if the content is blank.
         
         Args:
             key (str): result key
-            content: positional arguments for `print`
+            content (str): to be printed
             suppl (bool): If `True`, the database entry isn't replaced but
                 supplemented.
             silence_stdout (bool): If `True`, the content won't be printed but
                 only registered in the database.
             preformatted (bool): If `True`, wrap the content in HTML pre-tags.
         """
         if not content.strip():
@@ -150,17 +154,19 @@
         if not silence_stdout:
             print('####', key, content)
         if preformatted:
             content = f"<pre>{content}</pre>"
         self.add_db_entry(key, content, suppl=suppl)
         
     @contextlib.contextmanager
-    def savefig(self, key, tool='matplotlib', with_printer=True, with_libstyle=True,
-              figsize=None, refresh_millisec=None, tight_layout=True, close_all=True
-    ):
+    def savefig(self, key: str, tool: str = 'matplotlib', with_printer: bool = True,
+              with_libstyle: bool = True, figsize: Optional[Tuple[float, float]] = None,
+              refresh_millisec: Optional[float] = None, tight_layout: bool = True,
+              close_all: bool = True
+    ) -> None:
         """Context manager to convert the plot created in the context manager's
         block into a PNG file
 
         The PNG file will be saved under the key in the image directory and
         linked under the key in the corresponding HTML file and the database.
         Printed output will also be added if `with_printer=True`.
 
@@ -267,15 +273,15 @@
         contents = (f'<img src="{path}"><pre>{description}</pre>'
                     f'{refresh_code}')
             
         self.add_db_entry(key, contents)
         if close_all:
             plt.close('all')
 
-    def add_db_entry(self, key, contents, suppl=False):
+    def add_db_entry(self, key: str, contents: str, suppl: bool = False) -> None:
         """Add an entry to the Sqlite3 database file for the given key.
 
         After adding the entry, regenerate the result HTML page.
         
         Args:
             key (str): result key
             contents (str): result string (HTML)
@@ -295,42 +301,42 @@
                         ind = 0
                     ind += 1
             cursor.execute("insert into findings values (?, ?, ?, ?)",
                            (key, ind, time.time(), contents))
             db.commit()
             self._regenerate_html(cursor)
 
-    def link_text(self, filepath, link_text=''):
+    def link_text(self, filepath: str, link_text: str= '') -> str:
         """HTML text for a link to a given filepath.
 
         The filepath is made relative to the HTML directory for the link.
 
         Args:
             filepath (str): filepath for the link
             link_text (str, optional): link text to display, defaults to given
                 filepath
         Returns:
             str: HTML link text
         """
         filepath = pu.make_path_relative_to(filepath, self.html_dir)
         return f'<a target="_blank" href="{filepath}">{link_text}</a>'
             
-    def get_keys(self):
+    def get_keys(self) -> List[str]:
         """Get all distinct result keys from the database, reverse-ordered by
         timestamp.
         
         Returns:
             list of str: list of result keys
         """
         with pu.sqlite3_conn(self.db_path) as (db, cursor):
             return pu.first_of_each_item(
                 cursor.execute('select distinct key from findings '
                                'order by timestamp desc'))
 
-    def del_keys(self, keys):
+    def del_keys(self, keys: Union[str, List[str]]) -> None:
         """Delete the given result keys from the database.
 
         Args:
             keys (list of str): result keys to delete
         """
         if pu.isstring(keys):
             keys = [keys]
@@ -338,54 +344,54 @@
             for key in keys:
                 cursor.execute('delete from findings where key = ?', (key,))
                 plot_filepath = self._get_image_filepath(key)
                 if os.path.exists(plot_filepath):
                     os.remove(plot_filepath)
             db.commit()
 
-    def del_keys_like(self, regex):
+    def del_keys_like(self, regex: str) -> None:
         """Delete result keys matching the passed regex from the database.
 
         Args:
             regex (str): regular expression for the result keys
         """
         if pu.isstring(regex):
             regex = re.compile(regex)
         selected_keys = []
         for key in self.get_keys():
             if regex.search(key):
                 selected_keys.append(key)
         self.del_keys(selected_keys)
         
-    def get_findings(self):
+    def get_findings(self) -> List[Any]:
         """Get the contents of the findings table in the database,
         reverse-ordered by timestamp.
         
         Returns:
             list of tuples: rows of the database table
         """
         with pu.sqlite3_conn(self.db_path) as (db, cursor):
             return list(cursor.execute(
                 'select * from findings order by timestamp desc'))
 
-    def _init_db_if_necessary(self):
+    def _init_db_if_necessary(self) -> None:
         """Create the Sqlite3 database file and the table "findings" in it
         unless they already exist.
         """
         with pu.sqlite3_conn(self.db_path) as (db, cursor):
             cursor.execute("""
                 create table if not exists findings (
                     key text not null,
                     ind integer not null,
                     timestamp integer not null,
                     contents text not null,
                     primary key (key, ind)
                 )""")
 
-    def _regenerate_html(self, cursor, descending=True):
+    def _regenerate_html(self, cursor: sqlite3.Cursor, descending: bool = True) -> None:
         """Regenerate the result HTML page.
 
         Args:
             cursor: Sqlite3 database cursor
             descending (bool): whether to sort in descending timestamp order
         """
         all_entries = {}
@@ -428,26 +434,26 @@
                         display=self, entries=entries,
                         further_html_headers=self.further_html_headers,
                         html_filepath=html_filepath
                 ))
 
     RE_VALID_FIGURE_KEY = re.compile(r'^[^\s/()\[\]]+$')
 
-    def _get_image_filepath(self, filename_stem):
+    def _get_image_filepath(self, filename_stem: str) -> str:
         """Add the image directory and ".png" to the filename stem.
 
         Args:
             filename_stem (str): filename without directory or extension
         Returns:
             corresponding image filepath
         """
         filename = filename_stem + '.png'
         return os.path.join(self.image_dir, filename)
         
-    def _get_figure_path(self, key):
+    def _get_figure_path(self, key: str) -> str:
         """Check whether the key is valid and determine the filepath for a plot
         file.
 
         Args:
             key (str): result key
         Returns:
             key, plot filepath
@@ -455,13 +461,13 @@
         if self.RE_VALID_FIGURE_KEY.match(key) is None:
             raise ValueError(
                 'Please avoid whitespace, parentheses or slashes in the '
                 f'key for savefig: "{key}"')
         plot_filepath = self._get_image_filepath(key)
         return key, plot_filepath
 
-    def _tight_layout(self):
+    def _tight_layout(self) -> None:
         """Call `plt.tight_layout` and catch `ValueError`s."""
         try:
             plt.tight_layout(pad=0.3)
         except ValueError:
             pass
```

### Comparing `mlpj-0.2.1/mlpj/result_template.html` & `mlpj-0.2.2/mlpj/result_template.html`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.1/mlpj/timeseries_utils.py` & `mlpj-0.2.2/mlpj/timeseries_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """
 Utilities and convenience functions for timeseries models
 """
+import datetime
+from typing import Union, Tuple
+
+import numpy as np
 import pandas as pd
 
 from . import python_utils as pu
 
 
-def remove_last_n_days(df, datetime_colname, n_days):
+def remove_last_n_days(
+        df: pd.DataFrame, datetime_colname: str, n_days: int
+) -> pd.DataFrame:
     """Remove the data later than `n_days` before today from the dataframe.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         datetime_colname (str): column name containing pd-datetime values
         n_days (int): Data up to the date this many days ago will be kept.
     Returns:
         `pd.DataFrame`: filtered dataframe
     """
     last_day = pu.n_days_ago(n_days)
     return df[df[datetime_colname] <= pd.to_datetime(last_day)]
 
 
-def ts_train_test_split(df, train_test_split_date, date_colname, target_colname):
+def ts_train_test_split(
+        df: pd.DataFrame, train_test_split_date: Union[str, datetime.datetime],
+        date_colname: str, target_colname: str
+) -> Tuple[pd.DataFrame, np.ndarray, pd.DataFrame, np.ndarray]:
     """Train-test split for timeseries data
 
     All data before the `train_test_split_date` is taken as training data,
     the data starting from that time is taken as test data.
 
     Args:
         df (`pd.DataFrame`): input dataframe
```

### Comparing `mlpj-0.2.1/mlpj.egg-info/PKG-INFO` & `mlpj-0.2.2/mlpj.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2.1/mlpj.egg-info/SOURCES.txt` & `mlpj-0.2.2/mlpj.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 mlpj/timeseries_utils.py
 mlpj.egg-info/PKG-INFO
 mlpj.egg-info/SOURCES.txt
 mlpj.egg-info/dependency_links.txt
 mlpj.egg-info/requires.txt
 mlpj.egg-info/top_level.txt
 test/test_actions_looper.py
+test/test_ml_utils.py
 test/test_numpy_utils.py
 test/test_pandas_utils.py
 test/test_python_utils.py
 test/test_result_display.py
 test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2.1/setup.py` & `mlpj-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 github_url = 'https://github.com/bdanielby/mlpj'
 
 setup(
     name='mlpj',
-    version='0.2.1',
+    version='0.2.2',
     description='Tools for machine learning projects',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url=github_url,
     author='Bruno Daniel',
     license='MIT',
     packages=['mlpj'],
```

### Comparing `mlpj-0.2.1/test/test_actions_looper.py` & `mlpj-0.2.2/test/test_actions_looper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Unit tests for `mlpj.actions_looper`.
 """
 import collections
+from typing import List, Tuple, Any
 
 import pytest
 
 from mlpj import project_utils, actions_looper
 from mlpj.project_utils import temp_project
 
 
-def contents_of_defaultdict(dic):
+def sorted_items_of_dict(dic: dict) -> List[Tuple[Any, Any]]:
     """Sorted items of a defaultdict
 
     Args:
-        dic (defualtdict): input dictionary
+        dic (defaultdict): input dictionary
     Returns:
         list: sorted list of items
     """
     res = list(dic.items())
     res.sort()
     return res
     
@@ -25,38 +26,38 @@
 class ClassExample:
     """Example for an action implemented as a class
 
     Each step traces its calls in the class attribute `interim_results`.
     """
     interim_results = collections.defaultdict(list)
 
-    def step_r0_init(self):
+    def step_r0_init(self) -> str:
         self.interim_results[0].append("0")
         return "init"
 
-    def step_1_next(self, res0):
+    def step_1_next(self, res0: str) -> None:
         self.interim_results[1].append(f"1:{res0}")
 
-    def step_r5(self, res0):
+    def step_r5(self, res0: str) -> str:
         self.interim_results[5].append(f"5:{res0}")
         return "r2"
 
-    def step_10(self, res0, res2):
+    def step_10(self, res0: str, res2: str) -> None:
         self.interim_results[10].append(f"10:{res0},{res2}")
 
     @classmethod
-    def reset(cls):
+    def reset(cls) -> None:
         cls.interim_results.clear()
 
     @classmethod
-    def contents(cls):
-        return contents_of_defaultdict(cls.interim_results)
+    def contents(cls) -> List[Tuple[int, List[str]]]:
+        return sorted_items_of_dict(cls.interim_results)
     
 
-def test_execute_class_action():
+def test_execute_class_action() -> None:
     with temp_project() as pj:
         pj.add_available(ClassExample)
         ClassExample.reset()
 
         assert ClassExample.contents() == []
         
         # Previous result producing steps must be called first.
@@ -108,33 +109,33 @@
     """Example for an action implemented as an object of a class.
 
     Each step traces its calls in the instance attribute `interim_results`.
     """
     def __init__(self):
         self.interim_results = collections.defaultdict(list)
 
-    def step_r0_init(self):
+    def step_r0_init(self) -> str:
         self.interim_results[0].append("0")
         return "init"
 
-    def step_1_next(self, res0):
+    def step_1_next(self, res0: str) -> None:
         self.interim_results[1].append(f"1:{res0}")
 
-    def step_r5(self, res0):
+    def step_r5(self, res0: str) -> str:
         self.interim_results[5].append(f"5:{res0}")
         return "r2"
 
-    def step_10(self, res0, res2):
+    def step_10(self, res0: str, res2: str) -> None:
         self.interim_results[10].append(f"10:{res0},{res2}")
 
-    def contents(self):
-        return contents_of_defaultdict(self.interim_results)
+    def contents(self) -> List[Tuple[int, List[str]]]:
+        return sorted_items_of_dict(self.interim_results)
 
     
-def test_execute_object_action():
+def test_execute_object_action() -> None:
     with temp_project() as pj:
         obj = ObjExample()
         pj.add_available(obj)
 
         assert obj.contents() == []
         
         # Previous result producing steps must be called first.
@@ -178,15 +179,15 @@
             (5, ['5:init', '5:init', '5:init']), (10, ['10:init,r2'])
         ]
 
         assert pj.read_result("ObjExample", 0) == "init"
         assert pj.read_result("ObjExample", 5) == "r2"
 
         
-def test_execute_two_actions():
+def test_execute_two_actions() -> None:
     with temp_project() as pj:
         obj = ObjExample()
         pj.add_available(obj)
 
         with pytest.raises(ValueError, match=r'action "ClassExample" not found'):
             pj.execute("ObjExample ..1 ClassExample ..1")
             
@@ -194,42 +195,42 @@
         pj.add_available(ClassExample)
         
         pj.execute("ObjExample 0 ClassExample ..1")
         assert obj.contents() == [(0, ['0'])]
         assert ClassExample.contents() == [(0, ['0']), (1, ['1:init'])]
 
 
-def test_execute_fct_action():
+def test_execute_fct_action() -> None:
     interim_results = collections.defaultdict(list)
 
-    def contents():
-        return contents_of_defaultdict(interim_results)
+    def contents() -> List[Tuple[int, List[str]]]:
+        return sorted_items_of_dict(interim_results)
     
     with temp_project() as pj:
-        def fct_example():
+        def fct_example() -> None:
             """Example for an action implemented as a function.
     
             Each step traces its calls in the `defaultdict` `interim_results`.
             """
-            def step_r0_init():
+            def step_r0_init() -> str:
                 interim_results[0].append("0")
                 return "init"
     
-            def step_1_next(res0):
+            def step_1_next(res0: str) -> None:
                 assert pj.curr_action == "fct_example"
                 assert pj.curr_step == 1
                 assert pj.curr_step_method == "step_1_next"
                 assert pj.curr_astep == "fct_example_step_1_next"
                 interim_results[1].append(f"1:{res0}")
     
-            def step_r5(res0):
+            def step_r5(res0: str) -> str:
                 interim_results[5].append(f"5:{res0}")
                 return "r2"
     
-            def step_10(res0, res2):
+            def step_10(res0: str, res2: str) -> None:
                 interim_results[10].append(f"10:{res0},{res2}")
     
             pj.execute_fct_steps(locals())
     
         pj.add_available(fct_example)
         assert contents() == []
         
@@ -274,69 +275,69 @@
             (5, ['5:init', '5:init', '5:init']), (10, ['10:init,r2'])
         ]
 
         assert pj.read_result("fct_example", 0) == "init"
         assert pj.read_result("fct_example", 5) == "r2"
 
         
-def test_as_action():
+def test_as_action() -> None:
     interim_results = collections.defaultdict(list)
 
-    def contents():
-        return contents_of_defaultdict(interim_results)
+    def contents() -> List[Tuple[int, List[str]]]:
+        return sorted_items_of_dict(interim_results)
     
     with temp_project() as pj:
         @pj.as_action('myaction')
-        def fct_example():
+        def fct_example() -> None:
             """Example for an action implemented as a function.
     
             The decorator renames the action to "myaction".
             
             Each step traces its calls in the `defaultdict` `interim_results`.
             """
-            def step_r0_init():
+            def step_r0_init() -> str:
                 assert pj.curr_action == "myaction"
                 assert pj.curr_step == 0
                 assert pj.curr_step_method == "step_r0_init"
                 assert pj.curr_astep == "myaction_step_r0_init"
                 interim_results[0].append("0")
                 return "init"
     
-            def step_1_next(res0):
+            def step_1_next(res0: str) -> None:
                 interim_results[1].append(f"1:{res0}")
     
             pj.execute_fct_steps(locals())
     
         pj.add_available(fct_example)
         pj.execute("myaction ..1")
         assert contents() == [(0, ['0']), (1, ['1:init'])]
         
         pj.execute("myaction 1")
         assert contents() == [(0, ['0']), (1, ['1:init', '1:init'])]
         
         assert pj.read_result("myaction", 0) == "init"
 
 
-def test_ActionResultProxy():
+def test_ActionResultProxy() -> None:
     interim_results = collections.defaultdict(list)
 
-    def contents():
-        return contents_of_defaultdict(interim_results)
+    def contents() -> List[Tuple[int, List[str]]]:
+        return sorted_items_of_dict(interim_results)
     
     with temp_project() as pj:
-        def fct_example():
+        def fct_example() -> None:
             """Example for an action implemented as a function.
     
             Each step traces its calls in the `defaultdict` `interim_results`.
             """
-            def step_r0_init():
+            def step_r0_init() -> actions_looper.ActionResultProxy:
                 interim_results[0].append("0")
                 return actions_looper.ActionResultProxy("ClassExample", 0)
     
-            def step_1_next(res0):
+            def step_1_next(res0: str) -> None:
                 interim_results[1].append(f"1:{res0}")
     
             pj.execute_fct_steps(locals())
     
         pj.add_available(fct_example)
         assert contents() == []
```

### Comparing `mlpj-0.2.1/test/test_pandas_utils.py` & `mlpj-0.2.2/test/test_pandas_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from mlpj import python_utils as pu
 from mlpj import pandas_utils as pdu
 
 nan = np.nan
 
 
-def test_from_items():
+def test_from_items() -> None:
     pd_testing.assert_frame_equal(
         pdu.from_items([
             ('b', np.array([3, 8])),
             ('a', ['first', 'second']),
         ], index=[3, 4]),
         pd.DataFrame([[3, 'first'], [8, 'second']],
                      columns=['b', 'a'], index=[3, 4]))
@@ -40,72 +40,72 @@
     with pytest.raises(ValueError):
         pdu.from_items([
             ('b', np.array([3, 8, 9])),
             ('a', ['first', 'second']),
         ], index=[3, 4])
 
 
-def test_wide_display():
+def test_wide_display() -> None:
     out = io.StringIO()
     with pdu.wide_display():
         n_cols = 50
         df = pd.DataFrame(np.random.randint(low=0, high=3, size=(2, n_cols)),
                           columns=np.arange(n_cols))
         print(df, file=out)
     lines = out.getvalue().splitlines()
     assert len(lines) == 3
 
 
-def test_is_numerical():
+def test_is_numerical() -> None:
     assert pdu.is_numerical(pd.Series([3, 4]))
     assert pdu.is_numerical(pd.Series([3.5, 4]))
     assert pdu.is_numerical(pd.Series([True, False]))
     assert pdu.is_numerical(pd.Series([3.5, 4, nan]))
     assert not pdu.is_numerical(pd.Series(["foo", "bar"]))
 
 
-def test_get_colnames():
+def test_get_colnames() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ])
     np.testing.assert_array_equal(pdu.get_colnames(df), ['a', 'b', 'c'])
 
     dfg = df.groupby('b')
     np.testing.assert_array_equal(pdu.get_colnames(dfg), ['a', 'b', 'c'])
 
     np.testing.assert_array_equal(pdu.get_colnames(['x', 'y']), ['x', 'y'])
 
 
-def test_all_colnames_except():
+def test_all_colnames_except() -> None:
     X = pd.DataFrame(np.eye(4), columns=['x', 'a', 'ba', 'c'])
     assert pdu.all_colnames_except(X, ['a', 'c']) == ['x', 'ba']
 
     X = pd.DataFrame(np.eye(4), columns=list('abcd'))
     assert pdu.all_colnames_except(X, ['c', 'a']) == ['b', 'd']
     assert pdu.all_colnames_except(X, ['c', 'a', 'b', 'd']) == []
 
     
-def test_category_colnames():
+def test_category_colnames() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ])
         
     assert pdu.category_colnames(df) == []
     for colname in ['a', 'b']:
         df[colname] = df[colname].astype('category')
     assert pdu.category_colnames(df) == ['a', 'b']
 
     assert pdu.category_colnames(df, feature_list=('b', 'c')) == ['b']
 
 
-def test_rename_column():
+def test_rename_column() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
     ])
     
     pdu.rename_column(df, 'b', 'b1')
     pd_testing.assert_frame_equal(
@@ -115,15 +115,15 @@
             ('b1', ['a', 'b', 'b', 'a']),
         ]))
 
     with pytest.raises(KeyError):
         pdu.rename_column(df, 'foo', 'bar')
 
 
-def test_drop_index():
+def test_drop_index() -> None:
     df = pdu.from_items([
         ('b', np.array([3, 8])),
         ('a', ['first', 'second']),
     ], index=[3, 4])
 
     pdu.drop_index(df)
 
@@ -131,15 +131,15 @@
         df,
         pdu.from_items([
             ('b', np.array([3, 8])),
             ('a', ['first', 'second'])
         ]))
 
     
-def test_drop_columns():
+def test_drop_columns() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ], index=[3, 4, 5, 8])
     
     df1 = df.copy()
@@ -160,15 +160,15 @@
             ('b', ['a', 'b', 'b', 'a']),
         ], index=[3, 4, 5, 8]))
         
     with pytest.raises(KeyError):
         pdu.drop_columns(df, 'x')
 
 
-def test_columns_to_right():
+def test_columns_to_right() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ], index=[3, 4, 5, 8])
 
     df1 = pdu.columns_to_right(df, ['b', 'a'])
@@ -177,58 +177,58 @@
         pdu.from_items([
             ('c', ['x', 'y', 'z', 'x']),
             ('b', ['a', 'b', 'b', 'a']),
             ('a', [3, 4, 3, 2]),
         ], index=[3, 4, 5, 8]))
 
 
-def test_shuffle_df_drop_index():
+def test_shuffle_df_drop_index() -> None:
     df = pd.DataFrame(np.random.random(size=(3, 3)), columns=['a', 'b', 'c'])
     df1 = pdu.shuffle_df_drop_index(df)
     np.testing.assert_array_equal(df1.index.values, np.arange(len(df)))
     np.testing.assert_allclose(df1.sum(), df.sum())
 
 
-def test_assert_frame_contents_equal():
+def test_assert_frame_contents_equal() -> None:
     df1 = pdu.from_items([
         ('b', np.array([3, 8])),
         ('a', ['first', 'second']),
     ], index=[3, 4])
     
     df2 = pd.DataFrame([[3, 'first'], [8, 'second']],
                        columns=['b', 'a'])
 
     with pytest.raises(AssertionError):
         pd_testing.assert_frame_equal(df1, df2)
 
     pdu.assert_frame_contents_equal(df1, df2)
 
 
-def test_ser_where_defined():
+def test_ser_where_defined() -> None:
     x = pd.Series([4, 5, nan, 2, nan])
 
     pd_testing.assert_series_equal(
         pdu.ser_where_defined(x),
         pd.Series([4., 5, 2], index=[0, 1, 3]))
 
     
-def test_n_undefined_and_percentage():
+def test_n_undefined_and_percentage() -> None:
     x = pd.Series([4, 5, nan, 2, nan])
     
     n, perc = pdu.n_undefined_and_percentage(x)
     assert n == 2
     assert perc == 2 / 5 * 100
 
 
-def test_colname_list():
+def test_colname_list() -> None:
     assert pdu.colname_list('foo') == ['foo']
     assert pdu.colname_list(['foo', 'bar']) == ['foo', 'bar']
 
 
-def test_sort():
+def test_sort() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'c', 'd']),
         ('c', ['x', 'y', 'z', 'w'])
     ], index=[3, 4, 5, 8])
 
     df1 = pdu.sort(df, colnames='a', inplace=True)
@@ -239,22 +239,22 @@
         pdu.from_items([
             ('a', [2, 3, 3, 4]),
             ('b', ['d', 'a', 'c', 'b']),
             ('c', ['w', 'x', 'z', 'y'])
         ], index=[0, 1, 2, 3]))
         
 
-def test_sorted_unique_1dim():
+def test_sorted_unique_1dim() -> None:
     x = pd.Series([4, 3, nan, 8, 4, 3, nan, 2])
     pd_testing.assert_series_equal(
         pdu.sorted_unique_1dim(x),
         pd.Series([2, 3, 4, 8, nan]))
 
 
-def test_left_merge():
+def test_left_merge() -> None:
     df = pdu.from_items([('ITEM', [10, 20, 70, 30]),
                          ('Quantity', [3, 4, 8, 9])])
     dfb = pdu.from_items([('ITEM', [10, 20, 90]),
                           ('Quantity_nrm', [8, 9, 7])])
     dfr = pdu.left_merge(df, dfb, on=['ITEM'])
     pd_testing.assert_frame_equal(
         dfr, pdu.from_items([('ITEM', [10, 20, 70, 30]),
@@ -270,28 +270,28 @@
         dfr, pdu.from_items([('ITEM', np.zeros(0)),
                              ('Quantity', np.zeros(0)),
                              ('Quantity_nrm', np.zeros(0))]
                              ))
 
 
 @numba.njit
-def add_cumsum_a_to_b(X):
+def add_cumsum_a_to_b(X: pd.DataFrame) -> None:
     a = X[:, 0]
     b = X[:, 1]
     b += np.cumsum(a)
     # to test whether overwriting a non-result column has any consequence:
     a[:] = 0.
 
 
 @numba.njit
-def double_a(X):
+def double_a(X: pd.DataFrame) -> None:
     X[:, 0] *= 2
     
 
-def test_fast_groupby_multi_transform():
+def test_fast_groupby_multi_transform() -> None:
     df = pdu.shuffle_df_drop_index(
         pdu.from_items([
             ('g', [0,   0, 0, 0, 1, 1, 1, 1]),
             ('a', [1,   2, 4, 8, 3, 9, 27, 81]),
             ('b', [nan, 2, 5, 4, 4, 0, 3, -1])
         ]))
     
@@ -314,15 +314,15 @@
         pdu.from_items([
             ('g', [0,   0, 0, 0,   1, 1, 1, 1]),
             ('a', [2,   4, 8, 16,  6, 18, 54, 162]),
             ('b', [nan, 5, 12, 19, 7, 12, 42, 119])
         ]))
     
 
-def test_flatten_multi_columns():
+def test_flatten_multi_columns() -> None:
     df = pdu.from_items([
         (('a', '1'), [3, 4, 3, 2]),
         (('b', '2'), ['a', 'b', 'b', 'a']),
         (('c', '1'), ['x', 'y', 'z', 'x'])
     ], index=[3, 4, 5, 8])
     
     pdu.flatten_multi_columns(df)
@@ -331,15 +331,15 @@
         pdu.from_items([
             ('a_1', [3, 4, 3, 2]),
             ('b_2', ['a', 'b', 'b', 'a']),
             ('c_1', ['x', 'y', 'z', 'x'])
         ], index=[3, 4, 5, 8]))
 
 
-def test_rename_groupby_colnames():
+def test_rename_groupby_colnames() -> None:
     df = pdu.from_items([
         ('g', [0, 0, 0, 0, 1, 1, 1]),
         ('a', [2, 3, 0, 1, 4, 2, 1]),
         ('b', [-1, 1, 2, 0, -2, 1, 0]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
     
@@ -373,46 +373,46 @@
             ('a__max', [3, 4]),
             ('b', [2, -1]),
             ('count', [4, 3]),
             ('c', [8, 4])
         ], index=pd.Index([0, 1], name='group')))
 
 
-def test_print_column_info():
+def test_print_column_info() -> None:
     ser = pd.Series([3, 4, nan, 2])
     
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.print_column_info(ser, table_name='X')
 
 
-def test_print_table_info():
+def test_print_table_info() -> None:
     df = pdu.from_items([
         ('a', [2, 3, 0, 1, 4, 2, 1]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
     
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.print_table_info(df, table_name='X')
 
 
-def test_consistency_check():
+def test_consistency_check() -> None:
     df = pdu.from_items([
         ('a', [2, 3,    0, 1, 4.1, 2, 1]),
         ('a1', [2, 3.1, 0, 1, 4,   2, 1]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
     
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.consistency_check(df, 'a', 'a1')
 
 
-def test_truncate_datetime_to_freq():
+def test_truncate_datetime_to_freq() -> None:
     x = pd.Series(pd.to_datetime(['2023-04-22 10:40:22', '2023-03-01']))
     
     pd_testing.assert_series_equal(
         pdu.truncate_datetime_to_freq(x, 'D'),
         pd.Series(pd.to_datetime(['2023-04-22', '2023-03-01'])))
     
     pd_testing.assert_series_equal(
@@ -420,53 +420,53 @@
         pd.Series(pd.to_datetime(['2023-04-01', '2023-03-01'])))
     
     pd_testing.assert_series_equal(
         pdu.truncate_datetime_to_freq(x, 'W'),
         pd.Series(pd.to_datetime(['2023-04-17', '2023-02-27'])))
 
 
-def test_truncate_datetime_to_month():
+def test_truncate_datetime_to_month() -> None:
     df = pd.DataFrame({'dt': pd.to_datetime(['2017-09-12', '2017-10-20'])})
     
     df['dtm'] = pdu.truncate_datetime_to_month(df['dt'])
     
     pd_testing.assert_frame_equal(
         df, pdu.from_items([
         ('dt', pd.to_datetime(['2017-09-12', '2017-10-20'])),
         ('dtm', pd.to_datetime(['2017-09-01', '2017-10-01']))]))
 
 
-def test_truncate_datetime_to_week():
+def test_truncate_datetime_to_week() -> None:
     df = pd.DataFrame({'dt': pd.to_datetime(['2017-09-11', '2017-09-24'])})
     
     df['dtm'] = pdu.truncate_datetime_to_week(df['dt'])
     df['dtm_sun'] = pdu.truncate_datetime_to_week(df['dt'], sunday_first=True)
     
     pd_testing.assert_frame_equal(
         df, pdu.from_items([
             ('dt', pd.to_datetime(['2017-09-11', '2017-09-24'])),
             ('dtm', pd.to_datetime(['2017-09-11', '2017-09-18'])),
             ('dtm_sun', pd.to_datetime(['2017-09-10', '2017-09-24']))
         ]))
 
 
-def test_datetime_to_epoch():
+def test_datetime_to_epoch() -> None:
     pd_testing.assert_series_equal(
         pdu.datetime_to_epoch(
             pd.Series(pd.to_datetime(["1970-01-01", "1970-01-01 0:01:02.345",
                                       "NaT"]))),
         pd.Series([0., 62.345, nan]), check_exact=True)
     
     pd_testing.assert_series_equal(
         pdu.datetime_to_epoch(
             pd.Series([pd.to_datetime("1970-01-01 1:00:00")])),
         pd.Series([3600.]))
 
 
-def test_to_csv():
+def test_to_csv() -> None:
     df = pdu.from_items([
         ('b', np.array([3, 8])),
         ('a', ['first', 'second']),
     ], index=[3, 4])
 
     out = io.StringIO()
     pdu.to_csv(df, out)
```

### Comparing `mlpj-0.2.1/test/test_python_utils.py` & `mlpj-0.2.2/test/test_python_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,96 +7,96 @@
 import io
 import tempfile
 import datetime
 
 from mlpj import python_utils as pu
 
 
-def test_all_except()
+def test_all_except() -> None:
     lst = ['x', 'a', 'ba', 'a', 'c']
     assert pu.all_except(lst, ['a', 'c']) == ['x', 'ba']
 
 
-def test_isstring():
+def test_isstring() -> None:
     assert pu.isstring("foo")
     assert pu.isstring(b"foo")
     assert not pu.isstring(5)
     assert not pu.isstring(None)
 
 
-def test_if_true():
+def test_if_true() -> None:
     assert pu.if_true(True, 5) == 5
     assert pu.if_true(False, 5) == ''
     assert pu.if_true(False, 5, default=6) == 6
 
 
-def test_wi_perc():
+def test_wi_perc() -> None:
     assert pu.wi_perc(6, 10) == (6, 60)
     assert pu.wi_perc(6, 11) == (6, 6 / 11 * 100)
 
 
-def test_perc_str():
+def test_perc_str() -> None:
     assert pu.perc_str(6, 10) == "6 (60.00 %)"
 
 
-def test_first_of_each_item():
+def test_first_of_each_item() -> None:
     assert pu.first_of_each_item([('a', 3, 9), ('b', 4), ('c',)]) == [
         'a', 'b', 'c']
     
     assert (
         pu.first_of_each_item(collections.OrderedDict([('A', 3), ('B', 4)])
                               .items())
         == ['A', 'B'])
 
 
-def test_mkdir_unless_exists():
+def test_mkdir_unless_exists() -> None:
     with tempfile.TemporaryDirectory() as tmpdir:
         dirpath = os.path.join(tmpdir, "foo", "bar")
         assert not os.path.isdir(dirpath)
         pu.makedir_unless_exists(dirpath)
         assert os.path.isdir(dirpath)
         pu.makedir_unless_exists(dirpath)
 
 
-def test_make_path_relative_to():
+def test_make_path_relative_to() -> None:
     assert pu.make_path_relative_to('/ab/cd/d/e', '/ab/cd') == 'd/e'
     assert pu.make_path_relative_to('/ab/cd/d/e', '/ab/cd/d2') == '../d/e'
     assert pu.make_path_relative_to('/abd/cd/d/e', '/ab/cd/d2') == (
         '../../../abd/cd/d/e')
 
     assert pu.make_path_relative_to('/ab//cd//d/e/', '/ab//cd/') == 'd/e'
     assert pu.make_path_relative_to('/ab//cd//d/e/', '/ab//cd//d2') == '../d/e'
     
 
-def test_redirect_stdouterr():
+def test_redirect_stdouterr() -> None:
     out = io.StringIO()
     err = io.StringIO()
     with pu.redirect_stdouterr(out, err):
         print("foo")
         print("bar", file=sys.stderr)
     assert out.getvalue() == "foo\n"
     assert err.getvalue() == "bar\n"
 
 
-def test_BranchedOutputStreams():
+def test_BranchedOutputStreams() -> None:
     out1 = io.StringIO()
     out2 = io.StringIO()
 
     stream = pu.BranchedOutputStreams([out1, out2])
     stream.write("foo ")
     stream.flush()
     stream.write("bar")
 
     for out in (out1, out2):
         assert out.getvalue() == "foo bar"
 
     stream.close()
 
 
-def test_open_overwriting_safely():
+def test_open_overwriting_safely() -> None:
     with tempfile.TemporaryDirectory() as tmpdir:
         filepath = os.path.join(tmpdir, 'foo.txt')
         
         original_output = "foo\nbar\n"
         with open(filepath, 'w') as fout:
             fout.write(original_output)
 
@@ -115,26 +115,26 @@
         assert contents(filepath) == original_output
         
         with pu.open_overwriting_safely(filepath, 'w') as fout:
             fout.write(new_output)
         assert contents(filepath) == new_output
 
 
-def test_ansiicol():
+def test_ansiicol() -> None:
     assert pu.ansiicol(31) == "\x1b[31m"
 
 
-def test_sqlite3_conn():
+def test_sqlite3_conn() -> None:
     with tempfile.TemporaryDirectory() as tmpdir:
         dbpath = os.path.join(tmpdir, "database.db")
         with pu.sqlite3_conn(dbpath) as (db, cursor):
             pass
 
 
-def test_n_days_ago():
+def test_n_days_ago() -> None:
     today = datetime.date.today()
     assert (today - pu.n_days_ago(5)) == datetime.timedelta(days=5)
 
 
-def test_today_isoformat():
+def test_today_isoformat() -> None:
     today = datetime.date.today()
     assert pu.today_isoformat() == today.strftime("%Y-%m-%d")
```

### Comparing `mlpj-0.2.1/test/test_result_display.py` & `mlpj-0.2.2/test/test_result_display.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Unit tests for `mlpj.result_display`.
 """
 import os
 import collections
 import io
+from typing import List, Tuple, Any
 
 import numpy as np
 import pytest
 
 from mlpj import python_utils as pu
 from mlpj import project_utils
 from mlpj import plot_utils as pltu
 from mlpj.project_utils import temp_project
 
 
-def get_keys_and_contents(pj):
+def get_keys_and_contents(pj: project_utils.Manager) -> List[Tuple[str, Any]]:
     return [(key, contents) for (key, ind, timestamp, contents) in pj.get_findings()]
 
 
-def test_printer():
+def test_printer() -> None:
     with temp_project() as pj:
         with pj.printer("key1"):
             print("foo")
             
         with pj.printer("key2"):
             print("bar")
         
@@ -48,15 +49,15 @@
         assert get_keys_and_contents(pj) == [
             ('key2', '<pre>continuation</pre>'),
             ('key10', 'value10'),
             ('key2', '<pre>bar</pre>'),
         ]
 
 
-def test_savefig():
+def test_savefig() -> None:
     with temp_project() as pj:
         with pj.savefig("profile_plot"):
             n = 500
             x = np.random.random(size=n)
             y = x * x + 0.1 * np.random.random(size=n)
 
             pltu.profile_plot(x, y, n_bins=30, histogram=None)
@@ -67,35 +68,35 @@
              '<img src="../image/profile_plot.png">'
              '<pre>profile plot of a noisy x^2\n</pre>')
         ]
 
         assert os.path.exists(os.path.join(pj.image_path, "profile_plot.png"))
 
 
-def test_link_text():
+def test_link_text() -> None:
     with temp_project() as pj:
         assert pj.link_text(
             os.path.join(pj.image_path, "myfile.txt"), 'myfile') == (
                 '<a target="_blank" href="../image/myfile.txt">myfile</a>')
 
 
-def test_print_link_and_return_filepath():
+def test_print_link_and_return_filepath() -> None:
     with temp_project() as pj:
         out = io.StringIO()
         with pu.redirect_stdouterr(out, out):
             filepath = pj.print_link_and_return_filepath(
                 'myfile.txt', 'See: ')
 
         assert out.getvalue() == (
             'See: <a target="_blank" href="../image/myfile.txt">'
             'myfile.txt</a>\n')
         assert filepath == os.path.join(pj.image_path, 'myfile.txt')
 
 
-def test_get_analysis_pdf_filepath():
+def test_get_analysis_pdf_filepath() -> None:
     with temp_project() as pj:
         for iteration in [0, 1, -1]:
             if iteration == -1:
                 suffix = ''
             else:
                 suffix = f'_{iteration}'
             assert (
```

### Comparing `mlpj-0.2.1/test/test_timeseries_utils.py` & `mlpj-0.2.2/test/test_timeseries_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas.testing as pd_testing
 
 from mlpj import python_utils as pu
 from mlpj import pandas_utils as pdu
 from mlpj import timeseries_utils as tsu
 
 
-def test_remove_last_n_days():
+def test_remove_last_n_days() -> None:
     df = pdu.from_items([
         ('date', pd.to_datetime(
             [pu.n_days_ago(20), pu.n_days_ago(5), pu.n_days_ago(10)])),
         ('a', [2, 3, 1])
     ])
     
     df1 = tsu.remove_last_n_days(df, 'date', 10)
@@ -22,15 +22,15 @@
         df1,
         pdu.from_items([
             ('date', pd.to_datetime([pu.n_days_ago(20), pu.n_days_ago(10)])),
             ('a', [2, 1])
         ]))
 
     
-def test_ts_train_test_split():
+def test_ts_train_test_split() -> None:
     df = pdu.from_items([
         ('date', pd.to_datetime(['2023-03-05', '2023-01-15', '2023-02-01'])),
         ('a', [2, 3, 1]),
         ('y', [0, 1, -1]),
     ])
 
     X_train, y_train, X_test, y_test = tsu.ts_train_test_split(
```


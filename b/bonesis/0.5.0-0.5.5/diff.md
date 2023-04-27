# Comparing `tmp/bonesis-0.5.0.tar.gz` & `tmp/bonesis-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonesis-0.5.0.tar", last modified: Thu Mar 30 22:50:11 2023, max compression
+gzip compressed data, was "bonesis-0.5.5.tar", last modified: Thu Apr 27 20:53:00 2023, max compression
```

## Comparing `bonesis-0.5.0.tar` & `bonesis-0.5.5.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:50:11.334487 bonesis-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-03-30 22:49:58.000000 bonesis-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-03-30 22:49:58.000000 bonesis-0.5.0/Licence_CeCILL_V2.1-fr.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 22:49:58.000000 bonesis-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 22:50:11.334487 bonesis-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-30 22:49:58.000000 bonesis-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:50:11.334487 bonesis-0.5.0/bonesis/
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/aeon.py
--rw-r--r--   0 runner    (1001) docker     (123)    27662 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/asp_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/reprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:50:11.334487 bonesis-0.5.0/bonesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 22:50:11.000000 bonesis-0.5.0/bonesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:50:11.334487 bonesis-0.5.0/bonesis0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis0/asp_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis0/diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis0/proxy_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-30 22:49:58.000000 bonesis-0.5.0/bonesis0/subset_portfolio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 22:50:11.334487 bonesis-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-30 22:49:58.000000 bonesis-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.750640 bonesis-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-27 20:52:49.000000 bonesis-0.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-04-27 20:52:49.000000 bonesis-0.5.5/Licence_CeCILL_V2.1-fr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 20:52:49.000000 bonesis-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-27 20:53:00.750640 bonesis-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-27 20:52:49.000000 bonesis-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/aeon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/asp_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/reprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/asp_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/clingo_solving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/gil_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/proxy_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/subset_portfolio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:53:00.750640 bonesis-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-27 20:52:49.000000 bonesis-0.5.5/setup.py
```

### Comparing `bonesis-0.5.0/LICENSE.txt` & `bonesis-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/Licence_CeCILL_V2.1-fr.txt` & `bonesis-0.5.5/Licence_CeCILL_V2.1-fr.txt`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/README.md` & `bonesis-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/__init__.py` & `bonesis-0.5.5/bonesis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 
 settings = {
     "parallel": 1,
     "clingo_options": (),
     "clingo_opt_strategy": "bb",
     "solutions": "all",
     "quiet": False,
+    "timeout": 0,
+    "soft_interrupt": False, # if True, silently end solving
+    "fail_if_timeout": True, # if timeout raise TimeoutError
+    "clingo_gil_workaround": 1,
+        # 0/None: no GIL wrapper for clingo
+        # 1: run clingo in a single background thread
+        # 2: separate thread for each solution
 }
 
 class BoNesis(object):
     def __init__(self, domain, data=None):
         if not isinstance(domain, BonesisDomain):
             if isinstance(domain, minibn.BooleanNetwork):
                 domain = BooleanNetwork(domain)
```

### Comparing `bonesis-0.5.0/bonesis/aeon.py` & `bonesis-0.5.5/bonesis/aeon.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/asp_encoding.py` & `bonesis-0.5.5/bonesis/asp_encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -376,14 +376,21 @@
 
     def encode_some(self, some):
         if some.dtype is None:
             raise TypeError(f"{some} has no type!")
         encoder = getattr(self, f"encode_some_{some.dtype.lower()}")
         return encoder(some.name, some.opts)
 
+    def encode_some_different(self, s1, s2):
+        for some in (s1, s2):
+            if s1.dtype is None:
+                raise TypeError(f"{some} has no type!")
+        encoder = getattr(self, f"encode_some_{s1.dtype.lower()}_different")
+        return encoder(s1, s2)
+
     def encode_some_freeze(self, name, opts):
         opts = SomeFreeze.default_opts | opts
         min_size = opts["min_size"]
         max_size = opts["max_size"]
         #TODO: user-specified domain
         exclude = opts["exclude"] or ()
         name = clingo_encode(name)
@@ -398,25 +405,36 @@
             rules.append(f":- some_freeze({name},{ex},_)")
         if max_size > 1:
             rules += [
                 f":- some_freeze({name},N,V), some_freeze({name},N,-V)"
             ]
         return rules
 
-    def encode_mutant(self, name, mutations, __pred="mutant"):
+    def encode_some_freeze_different(self, s1, s2):
+        n1 = clingo_encode(s1.name)
+        n2 = clingo_encode(s2.name)
+        ns = "some_freeze"
+        return [
+            f"{ns}_diff({n1},{n2}) :- {ns}({n1},N,V), {ns}({n2},N,-V)",
+            f"{ns}_diff({n1},{n2}) :- {ns}({n1},N,_), not {ns}({n2},N,_)",
+            f"{ns}_diff({n1},{n2}) :- not {ns}({n1},N,_), {ns}({n2},N,_)",
+            f":- not {ns}_diff({n1},{n2})"
+        ]
+
+    def encode_mutant(self, name, mutations, pred="mutant"):
         if isinstance(mutations, Some):
             # copy 'Some' mutation
             name = clingo_encode(name)
             some = clingo_encode(mutations.name)
-            return [f"{__pred}({name},N,V) :- some_freeze({some},N,V)"]
-        return [clingo.Function(__pred, symbols(name, node, s2v(b)))
+            return [f"{pred}({name},N,V) :- some_freeze({some},N,V)"]
+        return [clingo.Function(pred, symbols(name, node, s2v(b)))
             for node, b in mutations.items()]
 
     def encode_weak_mutant(self, name, mutations):
-        self.encode_mutant(name, mutatinons, __pred="weak_mutant")
+        return self.encode_mutant(name, mutations, pred="weak_mutant")
 
     def apply_mutant_to_mcfg(self, mutant, mcfg):
         if mutant is None:
             return []
         return [f"clamped({mcfg},N,V) :- mutant({mutant},N,V)"]
 
     def encode_fixpoint(self, cfg, mutant=None):
@@ -449,15 +467,14 @@
         H = clingo_encode(h.name)
         rules = [f"hypercube({H})" ]
         if h.min_dimension >= 1:
             rules.append(f":- #count {{ N: hypercube({H},N,2) }}"
                                         f"{h.min_dimension-1}")
         if h.max_dimension:
             rules.append(f":- {max_dimension+1} #count {{ N: hypercube({H},N,2) }}")
-        print(rules)
         return rules
 
     def encode_in_attractor(self, cfg, mutant=None):
         self.load_template_eval()
 
         X = clingo_encode(cfg.name)
         Z = self.fresh_atom("ts")
```

### Comparing `bonesis-0.5.0/bonesis/cli.py` & `bonesis-0.5.5/bonesis/cli.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/debug.py` & `bonesis-0.5.5/bonesis/debug.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/domains.py` & `bonesis-0.5.5/bonesis/domains.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/language.py` & `bonesis-0.5.5/bonesis/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,19 @@
         else:
             assert self.dtype == dtype, "Some used with incompatible types"
     def __str__(self):
         return f"Some{self.dtype}(\"{self.name}\")"
     def copy(self):
         return self
 
+    def __ne__(left, right):
+        if not isinstance(right, Some):
+            raise TypeError()
+        left.mgr.register_predicate("some_different", left, right)
+
     def assignments(self, solutions="subset-minimal", **kwargs):
         from .views import SomeView
         return SomeView(self, self.mgr.bo, solutions=solutions, **kwargs)
     def complementary_assignments(self, solutions="subset-minimal", **kwargs):
         if self.dtype == "Freeze":
             from .views import SomeFreezeComplementaryView
             return SomeFreezeComplementaryView(self, self.mgr.bo,
```

### Comparing `bonesis-0.5.0/bonesis/manager.py` & `bonesis-0.5.5/bonesis/manager.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/reprogramming.py` & `bonesis-0.5.5/bonesis/reprogramming.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/snippets.py` & `bonesis-0.5.5/bonesis/snippets.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/utils.py` & `bonesis-0.5.5/bonesis/utils.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis/views.py` & `bonesis-0.5.5/bonesis/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 #
 
+from functools import partial
 import itertools
 import multiprocessing
 import os
 from threading import Timer, Lock
 import time
 
 import clingo
@@ -45,14 +46,16 @@
 from .snippets import bn_nocyclic_attractors
 from .utils import OverlayedDict, frozendict
 from bonesis0.asp_encoding import (minibn_of_facts,
         configurations_of_facts,
         parse_nb_threads,
         portfolio_path,
         py_of_symbol, symbol_of_py)
+from bonesis0.clingo_solving import setup_clingo_solve_handler
+from bonesis0.gil_utils import setup_gil_iterator
 from bonesis0 import diversity
 
 
 class BonesisView(object):
     single_shot = True
     def __init__(self, bo, limit=0, mode="auto", extra=None, progress=False, **settings):
         self.bo = bo
@@ -69,14 +72,17 @@
 
         def parse_extra(extra):
             if isinstance(extra, str):
                 if extra == "configurations":
                     return configurations_of_facts
                 elif extra == "boolean-network":
                     return minibn_of_facts
+                elif extra == "somes":
+                    return partial(AllSomeView.allsomes_from_atoms,
+                                       self.bo.manager)
                 raise ValueError(f"Unknown extra '{extra}'")
             return extra
         if isinstance(extra, (tuple, list)):
             extra = tuple(map(parse_extra, extra))
         elif extra is not None:
             extra = (parse_extra(extra),)
         self.extra_model = extra
@@ -120,56 +126,57 @@
                 self.control.add("base", [], f"#show {x}.")
 
     def interrupt(self):
         dbg(f"{self} interrupted")
         self.interrupted = True
         self.control.interrupt()
 
+
     def __iter__(self):
         self.configure()
-        self._iterator = iter(self.control.solve(yield_=True))
+        self._solve_handler = setup_clingo_solve_handler(self.settings,
+                                                     self.control)
+        self._iterator = iter(self._solve_handler)
+        self._iterator = setup_gil_iterator(self.settings, self._iterator,
+                                self._solve_handler, self.control)
         self._counter = 0
         if self.progress:
             self._progressbar = self.progress(desc="Model optimization",
                                           total=float("inf"))
         return self
 
+    def _progress_tick(self):
+        if not self.progress:
+            return
+        if not self.mode.startswith("opt"):
+            return
+        self._progressbar.set_postfix({"score": self.cur_model.cost},
+                                          refresh=False)
+        self._progressbar.update()
+        self._progressbar.refresh()
+
     def __next__(self):
         if self.limit and self._counter >= self.limit:
             raise StopIteration
 
-        t = Timer(self.settings["timeout"], self.interrupt) \
-                if "timeout" in self.settings else None
-        t.start() if t is not None else None
-        try:
-            self.cur_model = next(self._iterator)
+        self.cur_model = next(self._iterator)
+        self._progress_tick()
 
-            def progress():
-                if self.progress:
-                    if self.mode.startswith("opt"):
-                        self._progressbar.set_postfix({"score": self.cur_model.cost},
-                                                      refresh=False)
-                    self._progressbar.update()
-                    self._progressbar.refresh()
-            progress()
-
-            if self.mode == "opt":
-                try:
-                    while True:
-                        self.cur_model = next(self._iterator)
-                        progress()
-                except StopIteration:
-                    if self.progress:
-                        self._progressbar.close()
-            elif self.mode == "optN":
-                while not self.cur_model.optimality_proven:
+        if self.mode == "opt":
+            try:
+                while True:
                     self.cur_model = next(self._iterator)
-                    progress()
-        finally:
-            t.cancel() if t is not None else None
+                    self._progress_tick()
+            except StopIteration:
+                if self.progress:
+                    self._progressbar.close()
+        elif self.mode == "optN":
+            while not self.cur_model.optimality_proven:
+                self.cur_model = next(self._iterator)
+                self._progress_tick()
 
         pmodel = self.parse_model(self.cur_model)
         for func in self.filters:
             if not func(pmodel):
                 print(f"Skipping solution not verifying {func.__name__}")
                 return next(self)
         self._counter += 1
@@ -341,15 +348,16 @@
         self.skip_supersets = skip_supersets
 
     def configure(self, **opts):
         super().configure(**opts)
         self.driver = self.driver_cls(**self.driver_kwargs)
         self.diverse = diversity.solve_diverse(self.control.control, self.driver,
                 limit=self.limit, on_model=super().parse_model,
-                skip_supersets=self.skip_supersets)
+                skip_supersets=self.skip_supersets,
+                settings=self.settings)
 
     def parse_model(self, model):
         return model
 
     def __iter__(self):
         self.configure()
         self._iterator = iter(self.diverse)
@@ -393,28 +401,34 @@
                 v = 0
             pairs.append((n,v))
         return dict(sorted(pairs))
 
 class AllSomeView(BonesisView):
     project = True
     show_templates = ["some"]
-    def format_model(self, model):
+
+    @staticmethod
+    def allsomes_from_atoms(manager, atoms):
         def init_some(dtype):
             if dtype == "Freeze":
                 return {}
             raise NotImplementedError
         somes = {name: init_some(some.dtype)
-            for name, some in self.bo.manager.some.items()}
+            for name, some in manager.some.items()}
 
-        for a in model.symbols(shown=True):
+        for a in atoms:
             if a.name == "some_freeze":
                 name, n, v = py_of_symbol(a)
                 somes[name][n] = max(v,0)
         return somes
 
+    def format_model(self, model):
+        atoms = model.symbols(shown=True)
+        return self.allsomes_from_atoms(self.bo.manager, atoms)
+
 class SomeView(AllSomeView):
     def __init__(self, some, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.some = some
     def configure_show(self):
         if self.some.dtype == "Freeze":
             name = symbol_of_py(self.some.name)
```

### Comparing `bonesis-0.5.0/bonesis.egg-info/SOURCES.txt` & `bonesis-0.5.5/bonesis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,10 +19,12 @@
 bonesis.egg-info/SOURCES.txt
 bonesis.egg-info/dependency_links.txt
 bonesis.egg-info/entry_points.txt
 bonesis.egg-info/requires.txt
 bonesis.egg-info/top_level.txt
 bonesis0/__init__.py
 bonesis0/asp_encoding.py
+bonesis0/clingo_solving.py
 bonesis0/diversity.py
+bonesis0/gil_utils.py
 bonesis0/proxy_control.py
 bonesis0/subset_portfolio.cfg
```

### Comparing `bonesis-0.5.0/bonesis0/asp_encoding.py` & `bonesis-0.5.5/bonesis0/asp_encoding.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis0/diversity.py` & `bonesis-0.5.5/bonesis0/diversity.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,22 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 #
 
 import random
 import time
+from threading import Thread
+from queue import Queue
 
 import clingo
 
 from .asp_encoding import minibn_of_facts
+from .clingo_solving import setup_clingo_solve_handler
+from .gil_utils import setup_gil_iterator
 
 class diversity_driver:
     preds = {("clause", 4), ("constant", 1)}
     def match_pred(self, a):
         return (a.name, len(a.arguments)) in self.preds
     def initialize(self, control):
         self.control = control
@@ -86,21 +90,22 @@
 
 
 def on_model_make_minibn(model):
     return minibn_of_facts(model.symbols(True))
 
 class solve_diverse:
     def __init__(self, control, driver, skip_supersets=False, limit=0,
-                    on_model=on_model_make_minibn):
+                    on_model=on_model_make_minibn, settings={}):
         self.control = control
         self.skip_supersets = skip_supersets
         self.driver = driver
         self.driver.initialize(self.control)
         self.limit = limit
         self.on_model = on_model
+        self.settings = settings
         self.__counter = 0
 
     def inject_solution(self, atoms):
         self.driver.on_solution(atoms)
         self.prepare_next(atoms)
         self.__counter += 1
 
@@ -130,31 +135,31 @@
         self.first_time = None
         return self
 
     def __next__(self):
         if self.limit and self.__counter >= self.limit:
             print()
             raise StopIteration
-        found = False
-        with self.control.solve(yield_=True) as solutions:
-            for model in solutions:
-                found = True
-                self.__counter += 1
-                now = time.time()
-                if self.first_time is None:
-                    self.first_time = now
-                elapsed = now-self.start_time
-                print("\rFound {} solutions in {:.1f}s (first in {:.1f}s; rate {:.1f}s)".format(
+
+        sh = setup_clingo_solve_handler(self.settings, self.control)
+        with sh:
+            it = setup_gil_iterator(self.settings, iter(sh), sh, self.control)
+            model = next(it, None)
+            if model is None:
+                if self.__counter:
+                    print()
+                raise StopIteration
+            atoms = model.symbols(atoms=True)
+            ret = self.on_model(model)
+
+        self.__counter += 1
+        now = time.time()
+        if self.first_time is None:
+            self.first_time = now
+        elapsed = now-self.start_time
+        print("\rFound {} solutions in {:.1f}s (first in {:.1f}s; rate {:.1f}s)".format(
                     self.__counter, elapsed,
                     self.first_time-self.start_time,
                     elapsed/self.__counter), end="", flush=True)
-                atoms = model.symbols(atoms=True)
-                obj = self.on_model(model)
-                self.driver.on_solution(atoms)
-                break
-        if not found:
-            if self.__counter:
-                print()
-            raise StopIteration
+        self.driver.on_solution(atoms)
         self.prepare_next(atoms)
-        return obj
-
+        return ret
```

### Comparing `bonesis-0.5.0/bonesis0/proxy_control.py` & `bonesis-0.5.5/bonesis0/proxy_control.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/bonesis0/subset_portfolio.cfg` & `bonesis-0.5.5/bonesis0/subset_portfolio.cfg`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.0/setup.py` & `bonesis-0.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup, find_packages
 
 NAME = 'bonesis'
-VERSION = '0.5.0'
+VERSION = '0.5.5'
 
 setup(name=NAME,
     version=VERSION,
     description = "Synthesis of Most Permissive Boolean Networks",
     license_files = ('LICENSE.txt', 'Licence_CeCILL_V2.1-fr.txt'),
     install_requires = [
         "boolean.py",
```


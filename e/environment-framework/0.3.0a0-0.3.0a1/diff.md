# Comparing `tmp/environment_framework-0.3.0a0.tar.gz` & `tmp/environment_framework-0.3.0a1.tar.gz`

## Comparing `environment_framework-0.3.0a0.tar` & `environment_framework-0.3.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/CONTRIBUTING.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/makefile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/mypy.ini
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pylintrc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pytest.ini
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/version.py
--rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/example/grid_world.ipynb
--rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/example/grid_world.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/requirements/dev.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/requirements/main.txt
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/__init__.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/estimator.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/game.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/gym.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/ilevel.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/level.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/observer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/py.typed
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/pygame_wrapper.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/simulator.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/src/environment_framework/visualizer.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_gym.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_level.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/tests/test_simulator.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/README.md
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 environment_framework-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/makefile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/mypy.ini
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/pylintrc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/pytest.ini
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/version.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/example/grid_world.ipynb
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/example/grid_world.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/requirements/dev.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/requirements/main.txt
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/estimator.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/game.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/gym.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/ilevel.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/level.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/observer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/py.typed
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/pygame_wrapper.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/simulator.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/src/environment_framework/visualizer.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/tests/test_gym.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/tests/test_level.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/tests/test_simulator.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/LICENSE
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/README.md
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 environment_framework-0.3.0a1/PKG-INFO
```

### Comparing `environment_framework-0.3.0a0/CODE_OF_CONDUCT.md` & `environment_framework-0.3.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/CONTRIBUTING.md` & `environment_framework-0.3.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/makefile` & `environment_framework-0.3.0a1/makefile`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/pylintrc` & `environment_framework-0.3.0a1/pylintrc`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/example/grid_world.ipynb` & `environment_framework-0.3.0a1/example/grid_world.ipynb`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/example/grid_world.py` & `environment_framework-0.3.0a1/example/grid_world.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/requirements/dev.txt` & `environment_framework-0.3.0a1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/requirements/main.txt` & `environment_framework-0.3.0a1/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/game.py` & `environment_framework-0.3.0a1/src/environment_framework/game.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/gym.py` & `environment_framework-0.3.0a1/src/environment_framework/gym.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/ilevel.py` & `environment_framework-0.3.0a1/src/environment_framework/ilevel.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/level.py` & `environment_framework-0.3.0a1/src/environment_framework/level.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/observer.py` & `environment_framework-0.3.0a1/src/environment_framework/observer.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/simulator.py` & `environment_framework-0.3.0a1/src/environment_framework/simulator.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/src/environment_framework/visualizer.py` & `environment_framework-0.3.0a1/src/environment_framework/visualizer.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/tests/test_gym.py` & `environment_framework-0.3.0a1/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/tests/test_level.py` & `environment_framework-0.3.0a1/tests/test_level.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/tests/test_simulator.py` & `environment_framework-0.3.0a1/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/.gitignore` & `environment_framework-0.3.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/LICENSE` & `environment_framework-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/README.md` & `environment_framework-0.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/pyproject.toml` & `environment_framework-0.3.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `environment_framework-0.3.0a0/PKG-INFO` & `environment_framework-0.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-framework
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Loose building blocks to create agent-environment loops.
 Project-URL: Source, https://github.com/crzdg/environment-framework
 Author: Reto Barmettler
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```


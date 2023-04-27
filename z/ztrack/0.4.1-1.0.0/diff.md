# Comparing `tmp/ztrack-0.4.1.tar.gz` & `tmp/ztrack-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztrack-0.4.1.tar", max compression
+gzip compressed data, was "ztrack-1.0.0.tar", max compression
```

## Comparing `ztrack-0.4.1.tar` & `ztrack-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,72 @@
--rw-r--r--   0        0        0     1614 2022-06-23 17:39:30.433026 ztrack-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      742 2022-06-23 17:14:31.588709 ztrack-0.4.1/README.md
--rw-r--r--   0        0        0      181 2022-06-23 17:39:30.433523 ztrack-0.4.1/ztrack/__init__.py
--rw-r--r--   0        0        0       75 2022-06-23 17:14:31.589709 ztrack-0.4.1/ztrack/__main__.py
--rw-r--r--   0        0        0      536 2022-06-23 17:38:37.873032 ztrack-0.4.1/ztrack/_create_config.py
--rw-r--r--   0        0        0       91 2022-06-23 17:14:31.589709 ztrack-0.4.1/ztrack/_run_gui.py
--rw-r--r--   0        0        0     1188 2022-06-23 17:38:37.866575 ztrack-0.4.1/ztrack/_run_tracking.py
--rw-r--r--   0        0        0       92 2022-06-23 17:14:31.590209 ztrack-0.4.1/ztrack/_settings.py
--rw-r--r--   0        0        0     5414 2022-06-23 17:38:37.863098 ztrack-0.4.1/ztrack/_view_results.py
--rw-r--r--   0        0        0     3480 2022-06-23 17:14:31.590709 ztrack-0.4.1/ztrack/cli.py
--rw-r--r--   0        0        0        0 2022-06-23 17:14:31.590709 ztrack-0.4.1/ztrack/gui/__init__.py
--rw-r--r--   0        0        0     5020 2022-06-23 17:14:31.590709 ztrack-0.4.1/ztrack/gui/_control_widget.py
--rw-r--r--   0        0        0     7120 2022-06-23 17:14:31.591209 ztrack-0.4.1/ztrack/gui/_main_window.py
--rw-r--r--   0        0        0     8811 2022-06-23 17:14:31.591209 ztrack-0.4.1/ztrack/gui/_tracking_plot_widget.py
--rw-r--r--   0        0        0        0 2022-06-23 17:14:31.591209 ztrack-0.4.1/ztrack/gui/behavior_analyzer/__init__.py
--rw-r--r--   0        0        0     1561 2022-06-23 17:14:31.591709 ztrack-0.4.1/ztrack/gui/behavior_analyzer/behavior_analyzer.py
--rw-r--r--   0        0        0      763 2022-06-23 17:14:31.591709 ztrack-0.4.1/ztrack/gui/behavior_analyzer/control_widget.py
--rw-r--r--   0        0        0     2399 2022-06-23 17:14:31.591709 ztrack-0.4.1/ztrack/gui/behavior_analyzer/multirow.py
--rw-r--r--   0        0        0     1385 2022-06-23 17:14:31.592209 ztrack-0.4.1/ztrack/gui/behavior_analyzer/plot_widget.py
--rw-r--r--   0        0        0     7389 2022-06-23 17:14:31.592209 ztrack-0.4.1/ztrack/gui/create_config.py
--rw-r--r--   0        0        0     1740 2022-06-23 17:14:31.592709 ztrack-0.4.1/ztrack/gui/img/logo.svg
--rw-r--r--   0        0        0     5284 2022-06-23 17:14:31.592709 ztrack-0.4.1/ztrack/gui/menu_widget.py
--rw-r--r--   0        0        0     4111 2022-06-23 17:14:31.592709 ztrack-0.4.1/ztrack/gui/tracking_viewer.py
--rw-r--r--   0        0        0        0 2022-06-23 17:14:31.592709 ztrack-0.4.1/ztrack/gui/utils/__init__.py
--rw-r--r--   0        0        0     2372 2022-06-23 17:14:31.593209 ztrack-0.4.1/ztrack/gui/utils/file.py
--rw-r--r--   0        0        0     2341 2022-06-23 17:14:31.593209 ztrack-0.4.1/ztrack/gui/utils/frame_bar.py
--rw-r--r--   0        0        0     1327 2022-06-23 17:14:31.593209 ztrack-0.4.1/ztrack/gui/utils/launch.py
--rw-r--r--   0        0        0    10874 2022-06-23 17:14:31.593709 ztrack-0.4.1/ztrack/gui/utils/variable_widgets.py
--rw-r--r--   0        0        0      146 2022-06-23 17:14:31.593709 ztrack-0.4.1/ztrack/metadata.py
--rw-r--r--   0        0        0     1150 2022-06-23 17:14:31.594209 ztrack-0.4.1/ztrack/tracking/__init__.py
--rw-r--r--   0        0        0      314 2022-06-23 17:14:31.594209 ztrack-0.4.1/ztrack/tracking/eye/__init__.py
--rw-r--r--   0        0        0     3605 2022-06-23 17:14:31.594709 ztrack-0.4.1/ztrack/tracking/eye/adaptive_threshold.py
--rw-r--r--   0        0        0     1438 2022-06-23 17:14:31.594709 ztrack-0.4.1/ztrack/tracking/eye/binary.py
--rw-r--r--   0        0        0     4827 2022-06-23 17:14:31.594709 ztrack-0.4.1/ztrack/tracking/eye/eye_tracker.py
--rw-r--r--   0        0        0     2529 2022-06-23 17:14:31.595209 ztrack-0.4.1/ztrack/tracking/eye/multi_threshold.py
--rw-r--r--   0        0        0      210 2022-06-23 17:14:31.595209 ztrack-0.4.1/ztrack/tracking/free/__init__.py
--rw-r--r--   0        0        0     3690 2022-06-23 17:14:31.595209 ztrack-0.4.1/ztrack/tracking/free/base.py
--rw-r--r--   0        0        0     2468 2022-06-23 17:14:31.595709 ztrack-0.4.1/ztrack/tracking/free/contour.py
--rw-r--r--   0        0        0     1593 2022-06-23 17:14:31.595709 ztrack-0.4.1/ztrack/tracking/free/sequential.py
--rw-r--r--   0        0        0        0 2022-06-23 17:14:31.595709 ztrack-0.4.1/ztrack/tracking/mixins/__init__.py
--rw-r--r--   0        0        0      611 2022-06-23 17:14:31.596209 ztrack-0.4.1/ztrack/tracking/mixins/background.py
--rw-r--r--   0        0        0      122 2022-06-23 17:14:31.596209 ztrack-0.4.1/ztrack/tracking/paramecia/__init__.py
--rw-r--r--   0        0        0     3262 2022-06-23 17:14:31.596209 ztrack-0.4.1/ztrack/tracking/paramecia/paramecia.py
--rw-r--r--   0        0        0     1826 2022-06-23 17:14:31.596710 ztrack-0.4.1/ztrack/tracking/params.py
--rw-r--r--   0        0        0      133 2022-06-23 17:14:31.596710 ztrack-0.4.1/ztrack/tracking/tail/__init__.py
--rw-r--r--   0        0        0     3009 2022-06-23 17:14:31.597209 ztrack-0.4.1/ztrack/tracking/tail/sequential.py
--rw-r--r--   0        0        0     2110 2022-06-23 17:14:31.597209 ztrack-0.4.1/ztrack/tracking/tail/tail_tracker.py
--rw-r--r--   0        0        0     4295 2022-06-23 17:14:31.597209 ztrack-0.4.1/ztrack/tracking/tracker.py
--rw-r--r--   0        0        0        0 2022-06-23 17:14:31.597709 ztrack-0.4.1/ztrack/utils/__init__.py
--rw-r--r--   0        0        0     5061 2022-06-23 17:14:31.597709 ztrack-0.4.1/ztrack/utils/cv.py
--rw-r--r--   0        0        0      150 2022-06-23 17:14:31.597709 ztrack-0.4.1/ztrack/utils/exception.py
--rw-r--r--   0        0        0     3567 2022-06-23 17:14:31.597709 ztrack-0.4.1/ztrack/utils/file.py
--rw-r--r--   0        0        0      351 2022-06-23 17:14:31.598209 ztrack-0.4.1/ztrack/utils/geometry.py
--rw-r--r--   0        0        0      119 2022-06-23 17:14:31.598209 ztrack-0.4.1/ztrack/utils/math.py
--rw-r--r--   0        0        0     2653 2022-06-23 17:14:31.598709 ztrack-0.4.1/ztrack/utils/shape.py
--rw-r--r--   0        0        0      171 2022-06-23 17:14:31.598709 ztrack-0.4.1/ztrack/utils/typing.py
--rw-r--r--   0        0        0     4475 2022-06-23 17:14:31.598709 ztrack-0.4.1/ztrack/utils/variable.py
--rw-r--r--   0        0        0     2122 2022-06-23 17:40:11.179374 ztrack-0.4.1/setup.py
--rw-r--r--   0        0        0     2030 2022-06-23 17:40:11.179374 ztrack-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1631 2023-04-27 08:34:27.000298 ztrack-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-04-27 08:28:52.798815 ztrack-1.0.0/README.md
+-rw-r--r--   0        0        0     2188 2023-04-27 08:28:52.799815 ztrack-1.0.0/ztrack/.gitignore
+-rw-r--r--   0        0        0      419 2023-04-27 08:28:52.799815 ztrack-1.0.0/ztrack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      181 2023-04-27 08:34:27.000798 ztrack-1.0.0/ztrack/__init__.py
+-rw-r--r--   0        0        0       75 2023-04-27 08:28:52.800316 ztrack-1.0.0/ztrack/__main__.py
+-rw-r--r--   0        0        0      422 2023-04-27 08:28:52.800815 ztrack-1.0.0/ztrack/_annotate.py
+-rw-r--r--   0        0        0      536 2023-04-27 08:28:52.800815 ztrack-1.0.0/ztrack/_create_config.py
+-rw-r--r--   0        0        0       91 2023-04-27 08:28:52.800815 ztrack-1.0.0/ztrack/_run_gui.py
+-rw-r--r--   0        0        0     1275 2023-04-27 08:28:52.801315 ztrack-1.0.0/ztrack/_run_tracking.py
+-rw-r--r--   0        0        0       92 2023-04-27 08:28:52.801315 ztrack-1.0.0/ztrack/_settings.py
+-rw-r--r--   0        0        0     5414 2023-04-27 08:28:52.801315 ztrack-1.0.0/ztrack/_view_results.py
+-rw-r--r--   0        0        0     3612 2023-04-27 08:28:52.801816 ztrack-1.0.0/ztrack/cli.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:28:52.801816 ztrack-1.0.0/ztrack/gui/__init__.py
+-rw-r--r--   0        0        0     5102 2023-04-27 08:28:52.801816 ztrack-1.0.0/ztrack/gui/_control_widget.py
+-rw-r--r--   0        0        0     7120 2023-04-27 08:28:52.802315 ztrack-1.0.0/ztrack/gui/_main_window.py
+-rw-r--r--   0        0        0     9450 2023-04-27 08:28:52.802315 ztrack-1.0.0/ztrack/gui/_tracking_plot_widget.py
+-rw-r--r--   0        0        0     5566 2023-04-27 08:28:52.802815 ztrack-1.0.0/ztrack/gui/annotator.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:28:52.802815 ztrack-1.0.0/ztrack/gui/behavior_analyzer/__init__.py
+-rw-r--r--   0        0        0     1561 2023-04-27 08:28:52.803315 ztrack-1.0.0/ztrack/gui/behavior_analyzer/behavior_analyzer.py
+-rw-r--r--   0        0        0      763 2023-04-27 08:28:52.803315 ztrack-1.0.0/ztrack/gui/behavior_analyzer/control_widget.py
+-rw-r--r--   0        0        0     2399 2023-04-27 08:28:52.803315 ztrack-1.0.0/ztrack/gui/behavior_analyzer/multirow.py
+-rw-r--r--   0        0        0     1385 2023-04-27 08:28:52.803315 ztrack-1.0.0/ztrack/gui/behavior_analyzer/plot_widget.py
+-rw-r--r--   0        0        0     7527 2023-04-27 08:28:52.803315 ztrack-1.0.0/ztrack/gui/create_config.py
+-rw-r--r--   0        0        0     1740 2023-04-27 08:28:52.804320 ztrack-1.0.0/ztrack/gui/img/logo.svg
+-rw-r--r--   0        0        0     5284 2023-04-27 08:28:52.804320 ztrack-1.0.0/ztrack/gui/menu_widget.py
+-rw-r--r--   0        0        0     4567 2023-04-27 08:28:52.804826 ztrack-1.0.0/ztrack/gui/tracking_viewer.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:28:52.804826 ztrack-1.0.0/ztrack/gui/utils/__init__.py
+-rw-r--r--   0        0        0     2372 2023-04-27 08:28:52.804826 ztrack-1.0.0/ztrack/gui/utils/file.py
+-rw-r--r--   0        0        0     2341 2023-04-27 08:28:52.805326 ztrack-1.0.0/ztrack/gui/utils/frame_bar.py
+-rw-r--r--   0        0        0     1327 2023-04-27 08:28:52.805326 ztrack-1.0.0/ztrack/gui/utils/launch.py
+-rw-r--r--   0        0        0    12353 2023-04-27 08:28:52.805826 ztrack-1.0.0/ztrack/gui/utils/variable_widgets.py
+-rw-r--r--   0        0        0       51 2023-04-27 08:28:52.799815 ztrack-1.0.0/ztrack/MANIFEST.in
+-rw-r--r--   0        0        0      146 2023-04-27 08:28:52.805826 ztrack-1.0.0/ztrack/metadata.py
+-rw-r--r--   0        0        0     1631 2023-04-27 08:35:40.013677 ztrack-1.0.0/ztrack/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-04-27 08:28:52.800316 ztrack-1.0.0/ztrack/README.md
+-rw-r--r--   0        0        0      470 2023-04-27 08:35:40.020175 ztrack-1.0.0/ztrack/setup.cfg
+-rw-r--r--   0        0        0      250 2023-04-27 08:35:40.016674 ztrack-1.0.0/ztrack/setup.py
+-rw-r--r--   0        0        0     1150 2023-04-27 08:28:52.806326 ztrack-1.0.0/ztrack/tracking/__init__.py
+-rw-r--r--   0        0        0      376 2023-04-27 08:28:52.806826 ztrack-1.0.0/ztrack/tracking/eye/__init__.py
+-rw-r--r--   0        0        0     4238 2023-04-27 08:28:52.806826 ztrack-1.0.0/ztrack/tracking/eye/adaptive_threshold.py
+-rw-r--r--   0        0        0     1436 2023-04-27 08:28:52.806826 ztrack-1.0.0/ztrack/tracking/eye/binary.py
+-rw-r--r--   0        0        0     4827 2023-04-27 08:28:52.806826 ztrack-1.0.0/ztrack/tracking/eye/eye_tracker.py
+-rw-r--r--   0        0        0     3905 2023-04-27 08:28:52.806826 ztrack-1.0.0/ztrack/tracking/eye/eyes_only.py
+-rw-r--r--   0        0        0     2527 2023-04-27 08:28:52.807831 ztrack-1.0.0/ztrack/tracking/eye/multi_threshold.py
+-rw-r--r--   0        0        0      210 2023-04-27 08:28:52.807831 ztrack-1.0.0/ztrack/tracking/free/__init__.py
+-rw-r--r--   0        0        0     3690 2023-04-27 08:28:52.808337 ztrack-1.0.0/ztrack/tracking/free/base.py
+-rw-r--r--   0        0        0     2468 2023-04-27 08:28:52.808337 ztrack-1.0.0/ztrack/tracking/free/contour.py
+-rw-r--r--   0        0        0     1593 2023-04-27 08:28:52.808337 ztrack-1.0.0/ztrack/tracking/free/sequential.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:28:52.808837 ztrack-1.0.0/ztrack/tracking/mixins/__init__.py
+-rw-r--r--   0        0        0      611 2023-04-27 08:28:52.808837 ztrack-1.0.0/ztrack/tracking/mixins/background.py
+-rw-r--r--   0        0        0      122 2023-04-27 08:28:52.809337 ztrack-1.0.0/ztrack/tracking/paramecia/__init__.py
+-rw-r--r--   0        0        0     3262 2023-04-27 08:28:52.809337 ztrack-1.0.0/ztrack/tracking/paramecia/paramecia.py
+-rw-r--r--   0        0        0     1826 2023-04-27 08:28:52.809337 ztrack-1.0.0/ztrack/tracking/params.py
+-rw-r--r--   0        0        0      398 2023-04-27 08:28:52.809837 ztrack-1.0.0/ztrack/tracking/tail/__init__.py
+-rw-r--r--   0        0        0     8391 2023-04-27 08:28:52.809837 ztrack-1.0.0/ztrack/tracking/tail/com.py
+-rw-r--r--   0        0        0     3717 2023-04-27 08:28:52.810337 ztrack-1.0.0/ztrack/tracking/tail/gradient.py
+-rw-r--r--   0        0        0     8281 2023-04-27 08:28:52.810337 ztrack-1.0.0/ztrack/tracking/tail/gradient2.py
+-rw-r--r--   0        0        0     1852 2023-04-27 08:28:52.810838 ztrack-1.0.0/ztrack/tracking/tail/sequential.py
+-rw-r--r--   0        0        0     8642 2023-04-27 08:28:52.810838 ztrack-1.0.0/ztrack/tracking/tail/sequential2.py
+-rw-r--r--   0        0        0     2110 2023-04-27 08:28:52.811337 ztrack-1.0.0/ztrack/tracking/tail/tail_tracker.py
+-rw-r--r--   0        0        0     4086 2023-04-27 08:28:52.811337 ztrack-1.0.0/ztrack/tracking/tracker.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:28:52.811337 ztrack-1.0.0/ztrack/utils/__init__.py
+-rw-r--r--   0        0        0     4921 2023-04-27 08:28:52.811838 ztrack-1.0.0/ztrack/utils/cv.py
+-rw-r--r--   0        0        0      150 2023-04-27 08:28:52.811838 ztrack-1.0.0/ztrack/utils/exception.py
+-rw-r--r--   0        0        0     3316 2023-04-27 08:28:52.812339 ztrack-1.0.0/ztrack/utils/file.py
+-rw-r--r--   0        0        0      351 2023-04-27 08:28:52.812339 ztrack-1.0.0/ztrack/utils/geometry.py
+-rw-r--r--   0        0        0      119 2023-04-27 08:28:52.812871 ztrack-1.0.0/ztrack/utils/math.py
+-rw-r--r--   0        0        0     4008 2023-04-27 08:28:52.812871 ztrack-1.0.0/ztrack/utils/shape.py
+-rw-r--r--   0        0        0      171 2023-04-27 08:28:52.813338 ztrack-1.0.0/ztrack/utils/typing.py
+-rw-r--r--   0        0        0     5428 2023-04-27 08:28:52.813338 ztrack-1.0.0/ztrack/utils/variable.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 ztrack-1.0.0/PKG-INFO
```

### Comparing `ztrack-0.4.1/pyproject.toml` & `ztrack-1.0.0/ztrack/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 target-version = ['py38']
-line-length = 79
+line-length = 99
 exclude = '''
 (
   /(
       \.eggs
     | \.git
     | \.mypy_cache
     | \.tox
@@ -19,15 +19,15 @@
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "ztrack"
-version = "0.4.1"
+version = "0.5.0"
 description = ""
 authors = ["Ka Chung Lam <kclamar@connect.ust.hk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kclamar/ztrack"
 repository = "https://github.com/kclamar/ztrack"
 classifiers=[
@@ -42,19 +42,20 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.1"
 decord = "^0.6.0"
 matplotlib = "^3.4.2"
 opencv-python = "^4.5.2"
 pandas = "^1.3.0"
-PyQt5 = "^5.15.4"
+PyQt5 = "^5.10.1"
 pyqtgraph = "^0.12.2"
 qtmodern = "^0.2.0"
 scikit-image = "^0.18.2"
-tables = "^3.6.1"
+superqt = "^0.3"
+tables = "3.6.1"
 tqdm = "^4.61.2"
 
 bump2version = { version = "*", optional = true }
 pandas-stubs = { version = "*", optional = true }
 pre-commit = { version = "*", optional = true }
 PyQt5-stubs = { version = "*", optional = true }
```

### Comparing `ztrack-0.4.1/README.md` & `ztrack-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/_create_config.py` & `ztrack-1.0.0/ztrack/_create_config.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/_view_results.py` & `ztrack-1.0.0/ztrack/_view_results.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/cli.py` & `ztrack-1.0.0/ztrack/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 )
 @my_command
 @overwrite
 @click.option(
     "-i",
     "--ignore-errors",
     is_flag=True,
-    help="Whether to view video in egocentric coordinates.",
+    help="Ignore errors during tracking.",
 )
 def run(**kwargs):
     from ztrack._run_tracking import run_tracking
 
     run_tracking(**kwargs)
 
 
@@ -140,7 +140,15 @@
 @main.command(short_help="Open GUI.")
 @verbose
 @click.option("--style", default="dark", show_default=True)
 def gui(**kwargs):
     from ztrack._run_gui import run_gui
 
     run_gui(**kwargs)
+
+
+@main.command(short_help="Annotate.")
+@my_command
+def annotate(**kwargs):
+    from ztrack._annotate import annotate
+
+    annotate(**kwargs)
```

### Comparing `ztrack-0.4.1/ztrack/gui/_control_widget.py` & `ztrack-1.0.0/ztrack/gui/_control_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,33 @@
     @property
     def trackingPlotWidget(self):
         return self._trackingPlotWidget
 
     def addTrackerGroup(self, groupName: str, trackers: Iterable[Tracker]):
         assert groupName not in self._tabs
         tab = TrackingTab(self, groupName)
-        tab.trackerIndexChanged.connect(
-            lambda index: self.trackerChanged.emit(groupName, index)
-        )
+        tab.trackerIndexChanged.connect(lambda index: self.trackerChanged.emit(groupName, index))
 
         for tracker in trackers:
             tab.addTracker(tracker)
 
         self.addTab(tab, groupName.capitalize())
         self._tabs[groupName] = tab
 
     def getCurrentTrackerIndex(self, groupName: str):
         return self._tabs[groupName].currentIndex
 
     def setStateFromTrackingConfig(self, trackingConfig: config_dict):
-        for groupName, groupDict in trackingConfig.items():
-            self._tabs[groupName].setState(
-                groupDict["method"], groupDict["params"]
-            )
+        for groupName in self._tabs:
+            if groupName in trackingConfig:
+                groupDict = trackingConfig[groupName]
+
+                self._tabs[groupName].setState(groupDict["method"], groupDict["params"])
+            else:
+                self._tabs[groupName].setState("none", {})
 
 
 class TrackingTab(QtWidgets.QWidget):
     def __init__(self, parent: ControlWidget, groupName: str):
         super().__init__(parent)
 
         self._trackingPlotWidget = parent.trackingPlotWidget
@@ -117,17 +118,15 @@
     def __init__(self, parent: TrackingTab, *, tracker: Tracker):
         super().__init__(parent)
         self._trackingPlotWidget = parent.trackingPlotWidget
         self._formLayout = QtWidgets.QFormLayout()
         self.setLayout(self._formLayout)
         self._fields: Dict[str, VariableWidget] = {}
 
-        for name, param in zip(
-            tracker.params.parameter_names, tracker.params.parameter_list
-        ):
+        for name, param in zip(tracker.params.parameter_names, tracker.params.parameter_list):
             label = QtWidgets.QLabel(self)
             label.setText(param.display_name)
             field = VariableWidget.fromVariable(param, self)
 
             if isinstance(field, (PointWidget, RectWidget)):
                 field.setTrackingPlotWidget(self._trackingPlotWidget)
```

### Comparing `ztrack-0.4.1/ztrack/gui/_main_window.py` & `ztrack-1.0.0/ztrack/gui/_main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     def closeEvent(self, a0: QtGui.QCloseEvent):
         self.closedSignal.emit()
         super().closeEvent(a0)
 
     def dragEnterEvent(self, event: QtGui.QDragEnterEvent) -> None:
         if event.mimeData().hasUrls():
-            if all(
+            if any(
                 [
                     Path(u.toLocalFile()).suffix in video_extensions
                     for u in event.mimeData().urls()
                 ]
             ):
                 event.accept()
         else:
```

### Comparing `ztrack-0.4.1/ztrack/gui/_tracking_plot_widget.py` & `ztrack-1.0.0/ztrack/gui/_tracking_plot_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 import pyqtgraph as pg
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-from ztrack.utils.shape import Ellipse, Points, Rectangle
+from ztrack.utils.shape import Ellipse, Line, Points, Rectangle
 from ztrack.utils.variable import Rect
 
 if TYPE_CHECKING:
     from typing import Dict, Iterable, List, Optional
 
     from ztrack.tracking.tracker import Tracker
     from ztrack.utils.shape import Shape
@@ -206,14 +206,16 @@
 def roiFromShape(shape: Shape):
     if isinstance(shape, Ellipse):
         return GuiEllipse(shape)
     elif isinstance(shape, Points):
         return GuiPoints(shape)
     elif isinstance(shape, Rectangle):
         return GuiRectangle(shape)
+    elif isinstance(shape, Line):
+        return GuiLine(shape)
     else:
         raise NotImplementedError
 
 
 class ShapeMixin:
     @abstractmethod
     def refresh(self):
@@ -284,7 +286,27 @@
             theta = self._ellipse.theta
             self.setVisible(True)
             self.setRect(cx - a, cy - b, a * 2, b * 2)
             self.setTransformOriginPoint(cx, cy)
             self.setRotation(theta)
         else:
             self.setVisible(False)
+
+
+class GuiLine(QtWidgets.QGraphicsLineItem, ShapeMixin):
+    def __init__(self, line: Line):
+        super().__init__()
+        self._line = line
+        self.setPen(pg.mkPen(color=line.lc, width=line.lw))
+        self.refresh()
+
+    def setBBox(self, bbox):
+        self._line.set_bbox(bbox)
+
+    def refresh(self):
+        if self._line.visible:
+            self.setVisible(True)
+            self.setLine(
+                self._line.x1, self._line.y1, self._line.x2, self._line.y2
+            )
+        else:
+            self.setVisible(False)
```

### Comparing `ztrack-0.4.1/ztrack/gui/behavior_analyzer/behavior_analyzer.py` & `ztrack-1.0.0/ztrack/gui/behavior_analyzer/behavior_analyzer.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/behavior_analyzer/control_widget.py` & `ztrack-1.0.0/ztrack/gui/behavior_analyzer/control_widget.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/behavior_analyzer/multirow.py` & `ztrack-1.0.0/ztrack/gui/behavior_analyzer/multirow.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/behavior_analyzer/plot_widget.py` & `ztrack-1.0.0/ztrack/gui/behavior_analyzer/plot_widget.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/create_config.py` & `ztrack-1.0.0/ztrack/gui/create_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import json
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 from PyQt5 import QtWidgets
 
 from ztrack._settings import config_extension
 from ztrack.gui.utils.file import selectVideoDirectories, selectVideoPaths
 from ztrack.tracking import get_trackers
 from ztrack.tracking.tracker import NoneTracker
 from ztrack.utils.file import get_config_dict, get_paths_for_config_creation
+from ztrack._settings import video_extensions
 
 from ._control_widget import ControlWidget
 from ._main_window import MainWindow
 
 if TYPE_CHECKING:
     from typing import List, Optional
 
@@ -38,16 +40,15 @@
         self._savePaths: List[List[str]] = savePaths
 
         self._trackerGroups = get_trackers(verbose=verbose, debug=True)
         self._controlWidget = ControlWidget(self)
 
         self._buttonBox = QtWidgets.QDialogButtonBox(self)
         self._buttonBox.setStandardButtons(
-            QtWidgets.QDialogButtonBox.Ok  # type: ignore
-            | QtWidgets.QDialogButtonBox.Cancel
+            QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel  # type: ignore
         )
 
         self._hBoxLayout.addWidget(self._controlWidget)
         self._hBoxLayout.setStretch(0, 50)
         self._hBoxLayout.setStretch(1, 50)
         self._layout.addWidget(self._buttonBox)
 
@@ -57,17 +58,17 @@
         self._trackingPlotWidget.setTrackerGroup(list(self._trackerGroups)[0])
 
         self._controlWidget.currentChanged.connect(self._onTabChanged)
         self._controlWidget.trackerChanged.connect(self._onTrackerChanged)
         self._controlWidget.paramsChanged.connect(self._onParamsChanged)
         self._trackingPlotWidget.roiChanged.connect(self._onRoiChanged)
 
-        self._buttonBox.button(
-            QtWidgets.QDialogButtonBox.Cancel
-        ).clicked.connect(self._onCancelButtonClicked)
+        self._buttonBox.button(QtWidgets.QDialogButtonBox.Cancel).clicked.connect(
+            self._onCancelButtonClicked
+        )
 
         self._buttonBox.button(QtWidgets.QDialogButtonBox.Ok).clicked.connect(
             self._onOkButtonClicked
         )
         self.updateVideo()
 
     @property
@@ -81,41 +82,41 @@
 
         return None
 
     def _saveTrackingConfig(self):
         trackingConfig = {}
 
         for group_name, trackers in self._trackerGroups.items():
-            tracker = trackers[
-                self._controlWidget.getCurrentTrackerIndex(group_name)
-            ]
+            tracker = trackers[self._controlWidget.getCurrentTrackerIndex(group_name)]
             if not isinstance(tracker, NoneTracker):
                 trackingConfig[group_name] = dict(
                     method=tracker.name(),
                     roi=tracker.roi.value,
                     params=tracker.params.to_dict(),
                 )
 
         for savePath in self._currentSavePaths:
-            with open(savePath + config_extension, "w") as fp:
+            with open(Path(savePath).with_suffix(config_extension), "w") as fp:
                 json.dump(trackingConfig, fp)
 
     def _onOkButtonClicked(self):
         self._saveTrackingConfig()
         self.dequeue()
         self.updateVideo()
 
     def _onCancelButtonClicked(self):
         self.dequeue()
         self.updateVideo()
 
     def dropEvent(self, event: QtGui.QDropEvent) -> None:
         paths = [u.toLocalFile() for u in event.mimeData().urls()]
+        paths = [path for path in paths if Path(path).suffix in video_extensions]
+        paths = sorted(paths, key=lambda x: x[::-1])
 
-        for path in paths:
+        for path in paths[::-1]:
             self.enqueue(path, [path], first=True)
 
         self.updateVideo()
 
     def _onFrameChanged(self):
         img = self._currentFrame
 
@@ -193,19 +194,15 @@
 
         for videoPath in reversed(videoPaths):
             self.enqueue(videoPath, [videoPath], first=True)
 
         self.updateVideo()
 
     def _openFolders(self):
-        directories, (
-            recursive,
-            sameConfig,
-            overwrite,
-        ) = selectVideoDirectories(
+        directories, (recursive, sameConfig, overwrite,) = selectVideoDirectories(
             (
                 ("Include subdirectories", True),
                 ("Use one configuration file per directory", True),
                 ("Overwrite existing configuration files", True),
             )
         )
         videoPaths, savePaths = get_paths_for_config_creation(
```

### Comparing `ztrack-0.4.1/ztrack/gui/img/logo.svg` & `ztrack-1.0.0/ztrack/gui/img/logo.svg`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/menu_widget.py` & `ztrack-1.0.0/ztrack/gui/menu_widget.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/tracking_viewer.py` & `ztrack-1.0.0/ztrack/gui/tracking_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,21 +35,38 @@
     ):
         super().__init__(
             parent, videoPaths=videoPaths, verbose=verbose, dock=dock
         )
 
         self._results: Dict[str, pd.DataFrame] = {}
         self._trackers: Dict[str, Tracker] = {}
+
+        self._buttonBox = QtWidgets.QDialogButtonBox(self)
+        self._buttonBox.setStandardButtons(
+            QtWidgets.QDialogButtonBox.Ok  # type: ignore
+        )
+        self._layout.addWidget(self._buttonBox)
+
+        self._buttonBox.button(QtWidgets.QDialogButtonBox.Ok).clicked.connect(
+            self._onOkButtonClicked
+        )
+
         if update:
             self.updateVideo()
 
+    def _onOkButtonClicked(self):
+        self.dequeue()
+        self.updateVideo()
+
     def dropEvent(self, event: QtGui.QDropEvent) -> None:
         paths = [u.toLocalFile() for u in event.mimeData().urls()]
+        paths = [path for path in paths if Path(path).suffix in video_extensions]
+        paths = sorted(paths)
 
-        for path in paths:
+        for path in paths[::-1]:
             self.enqueue(str(path), first=True)
 
         self.updateVideo()
 
     def _onFrameChanged(self):
         img = self._currentFrame
 
@@ -67,15 +84,15 @@
             self._videoPaths.insert(0, videoPath)
         else:
             self._videoPaths.append(videoPath)
 
     def dequeue(self):
         if len(self._videoPaths) > 0:
             self._videoPaths.pop(0)
-            self._savePaths.pop(0)
+            # self._savePaths.pop(0)
 
     def _openFiles(self):
         videoPaths = selectVideoPaths(native=True)
 
         for videoPath in reversed(videoPaths):
             self.enqueue(videoPath, first=True)
 
@@ -123,15 +140,13 @@
     def dragEnterEvent(self, event: QtGui.QDragEnterEvent) -> None:
         if event.mimeData().hasUrls():
             paths = [u.toLocalFile() for u in event.mimeData().urls()]
 
             if all(
                 [
                     Path(path).suffix in video_extensions
-                    and get_config_path(path).exists()
-                    and get_results_path(path).exists()
                     for path in paths
                 ]
             ):
                 event.accept()
         else:
             event.ignore()
```

### Comparing `ztrack-0.4.1/ztrack/gui/utils/file.py` & `ztrack-1.0.0/ztrack/gui/utils/file.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/utils/frame_bar.py` & `ztrack-1.0.0/ztrack/gui/utils/frame_bar.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/utils/launch.py` & `ztrack-1.0.0/ztrack/gui/utils/launch.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/gui/utils/variable_widgets.py` & `ztrack-1.0.0/ztrack/gui/utils/variable_widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from __future__ import annotations
 
 from abc import ABC, ABCMeta, abstractmethod
 from typing import TYPE_CHECKING
 
 from PyQt5 import QtCore, QtWidgets
+from superqt import QLabeledDoubleRangeSlider
 
-from ztrack.utils.variable import Angle, Float, Int, Point, Rect, String
+from ztrack.utils.variable import (
+    Angle,
+    Bool,
+    Float,
+    FloatRange,
+    Int,
+    Point,
+    Rect,
+    String,
+)
 
 if TYPE_CHECKING:
     from ztrack.gui._tracking_plot_widget import TrackingPlotWidget
     from ztrack.utils.typing import point2d, rect
     from ztrack.utils.variable import Variable
 
 
 class AbstractWidgetMeta(type(QtWidgets.QWidget), ABCMeta):  # type: ignore
     pass
 
 
 class VariableWidget(QtWidgets.QWidget, ABC, metaclass=AbstractWidgetMeta):
     valueChanged = QtCore.pyqtSignal()
 
-    def __init__(
-        self, parent: QtWidgets.QWidget = None, *, variable: Variable
-    ):
+    def __init__(self, parent: QtWidgets.QWidget = None, *, variable: Variable):
         super().__init__(parent)
         self._variable = variable
 
     @staticmethod
     def fromVariable(variable: Variable, parent: QtWidgets.QWidget = None):
         if isinstance(variable, Angle):
             return AngleWidget(parent, variable=variable)
@@ -36,14 +44,18 @@
             return IntWidget(parent, variable=variable)
         if isinstance(variable, Point):
             return PointWidget(parent, variable=variable)
         if isinstance(variable, Rect):
             return RectWidget(parent, variable=variable)
         if isinstance(variable, String):
             return StringWidget(parent, variable=variable)
+        if isinstance(variable, Bool):
+            return BoolWidget(parent, variable=variable)
+        if isinstance(variable, FloatRange):
+            return FloatRangeWidget(parent, variable=variable)
         raise NotImplementedError
 
     def _setValue(self, value):
         self._variable.value = value
         self._setGuiValue(self._variable.value)
         self.valueChanged.emit()
 
@@ -52,14 +64,54 @@
         pass
 
     def setValue(self, value):
         self._setValue(value)
         self._setGuiValue(value)
 
 
+class FloatRangeWidget(VariableWidget):
+    _variable: FloatRange
+
+    def __init__(self, parent: QtWidgets.QWidget = None, *, variable: FloatRange):
+        super().__init__(parent, variable=variable)
+        self._slider = QLabeledDoubleRangeSlider(self)
+        self._slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self._slider.setRange(variable.minimum, variable.maximum)
+        self._slider.setValue(variable.value)
+
+        layout = QtWidgets.QHBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.addWidget(self._slider)
+        self.setLayout(layout)
+        self._slider.valueChanged.connect(self._setValue)
+
+    def _setGuiValue(self, value):
+        self._slider.valueChanged.disconnect()
+        self._slider.setValue(value)
+        self._slider.valueChanged.connect(self._setValue)
+
+
+class BoolWidget(VariableWidget):
+    def __init__(self, parent: QtWidgets.QWidget = None, *, variable: Bool):
+        super().__init__(parent, variable=variable)
+
+        self._checkbox = QtWidgets.QCheckBox(self)
+        self._checkbox.setChecked(variable.value)
+
+        layout = QtWidgets.QHBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.addWidget(self._checkbox)
+        self.setLayout(layout)
+
+        self._checkbox.stateChanged.connect(self._setValue)
+
+    def _setGuiValue(self, value: bool):
+        self._checkbox.setChecked(value)
+
+
 class StringWidget(VariableWidget):
     def __init__(self, parent: QtWidgets.QWidget = None, *, variable: String):
         super().__init__(parent, variable=variable)
 
         self._line = QtWidgets.QLineEdit(self)
         layout = QtWidgets.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
@@ -199,63 +251,52 @@
         self._pushButton.setText(self._get_display_str(variable.value))
 
         layout = QtWidgets.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self._pushButton)
         self.setLayout(layout)
 
-        self._pushButton.clicked.connect(
-            lambda: self._setSelectionMode(not self._selectionMode)
-        )
+        self._pushButton.clicked.connect(lambda: self._setSelectionMode(not self._selectionMode))
 
     def _setGuiValue(self, value: point2d):
         self._pushButton.setText(self._get_display_str(value))
 
     @staticmethod
     def _get_display_str(value: point2d):
         x, y = value
         return f"({x}, {y})"
 
     def _setValue(self, value):
-        print(value)
         super()._setValue(value)
         self._setSelectionMode(False)
 
     def _setSelectionMode(self, b: bool):
         self._selectionMode = b
 
         if self._selectionMode:
-            print("link")
             self.link()
             self._pushButton.setText("Cancel")
         else:
-            print("unlink")
             self.unlink()
-            self._pushButton.setText(
-                self._get_display_str(self._variable.value)
-            )
+            self._pushButton.setText(self._get_display_str(self._variable.value))
 
         self._selectionModeChanged.emit(self._selectionMode)
 
     def link(self):
-        self._trackingPlotWidget.pointSelected.connect(
-            lambda x, y: self._setValue((x, y))
-        )
+        self._trackingPlotWidget.pointSelected.connect(lambda x, y: self._setValue((x, y)))
 
     def unlink(self):
         try:
             self._trackingPlotWidget.pointSelected.disconnect()
         except TypeError:
             pass
 
     def setTrackingPlotWidget(self, trackingPlotWidget: TrackingPlotWidget):
         self._trackingPlotWidget = trackingPlotWidget
-        self._selectionModeChanged.connect(
-            self._trackingPlotWidget.setPointSelectionModeEnabled
-        )
+        self._selectionModeChanged.connect(self._trackingPlotWidget.setPointSelectionModeEnabled)
 
 
 class RectWidget(VariableWidget):
     _selectionModeChanged = QtCore.pyqtSignal(bool)
     _trackingPlotWidget: TrackingPlotWidget
 
     def __init__(self, parent: QtWidgets.QWidget = None, *, variable: Rect):
@@ -268,17 +309,15 @@
 
         layout = QtWidgets.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self._pushButton)
         self.setLayout(layout)
 
         self._pushButton.clicked.connect(
-            lambda: self._setSelectionState(
-                -1 if self._selectedPoints >= 0 else 0
-            )
+            lambda: self._setSelectionState(-1 if self._selectedPoints >= 0 else 0)
         )
 
     def _setGuiValue(self, value: rect):
         self._pushButton.setText(self._get_display_str(value))
 
     @staticmethod
     def _get_display_str(value: rect = None):
@@ -307,27 +346,23 @@
         self._selectedPoints = b
 
         if self._selectedPoints >= 0:
             self.link()
             self._pushButton.setText("Cancel")
         else:
             self.unlink()
-            self._pushButton.setText(
-                self._get_display_str(self._variable.value)
-            )
+            self._pushButton.setText(self._get_display_str(self._variable.value))
 
         self._selectionModeChanged.emit(self._selectedPoints >= 0)
 
     def link(self):
         self._trackingPlotWidget.pointSelected.connect(self._setPoint)
 
     def unlink(self):
         try:
             self._trackingPlotWidget.pointSelected.disconnect()
         except TypeError:
             pass
 
     def setTrackingPlotWidget(self, trackingPlotWidget: TrackingPlotWidget):
         self._trackingPlotWidget = trackingPlotWidget
-        self._selectionModeChanged.connect(
-            self._trackingPlotWidget.setPointSelectionModeEnabled
-        )
+        self._selectionModeChanged.connect(self._trackingPlotWidget.setPointSelectionModeEnabled)
```

### Comparing `ztrack-0.4.1/ztrack/tracking/__init__.py` & `ztrack-1.0.0/ztrack/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/eye/adaptive_threshold.py` & `ztrack-1.0.0/ztrack/tracking/tail/gradient.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,117 @@
-import cv2
+from typing import Type
+
 import numpy as np
-from skimage.morphology import remove_small_objects
+import pandas as pd
+from scipy.ndimage import gaussian_filter
 
 import ztrack.utils.cv as zcv
-from ztrack.tracking.eye.eye_tracker import EyeParams, EyeTracker
-from ztrack.utils.shape import Rectangle
-from ztrack.utils.variable import Float, Int, Rect
+from ztrack.tracking.tracker import Params, Tracker
+from ztrack.utils.shape import Points
+from ztrack.utils.variable import Angle, Bool, Float, Int, Point
 
 
-class AdaptiveThresholdEyeTracker(EyeTracker):
-    def __init__(
-        self, roi=None, params: dict = None, *, verbose=0, debug=False
-    ):
-        super().__init__(roi, params, verbose=verbose, debug=debug)
+class GradientTailTracker(Tracker):
+    @property
+    def _Params(self) -> Type[Params]:
+        return self.__Params
+
+    @property
+    def shapes(self):
+        return [self._points]
 
-        self._left_eye_bbox = Rectangle(0, 0, 1, 1, 4, "b")
-        self._right_eye_bbox = Rectangle(0, 0, 1, 1, 4, "r")
-        self._swim_bladder_bbox = Rectangle(0, 0, 1, 1, 4, "g")
-        self._bboxes = [
-            self._left_eye_bbox,
-            self._right_eye_bbox,
-            self._swim_bladder_bbox,
-        ]
+    def annotate_from_series(self, s: pd.Series) -> None:
+        raise NotImplementedError
 
-    class __Params(EyeParams):
+    @classmethod
+    def _results_to_series(cls, results):
+        raise NotImplementedError
+
+    def _transform_from_roi_to_frame(self, results):
+        if self.roi.value is not None:
+            x0, y0 = self.roi.value[:2]
+            results[:, :2] += (x0, y0)
+
+        return results
+
+    class __Params(Params):
         def __init__(self, params: dict = None):
             super().__init__(params)
             self.sigma = Float("Sigma (px)", 2, 0, 100, 0.1)
+            self.n_segments = Int("Number of segments", 10, 3, 20)
+            self.segment_length = Int("Segment length (px)", 10, 5, 50)
+            self.tail_base = Point("Tail base (x, y)", (250, 120))
+            self.angle = Angle("Initial angle (°)", 90)
+            self.theta = Angle("Search angle (°)", 60)
+            self.d_theta = Float("dtheta", 0.05, 0.01, 0.1, 0.01)
+            self.sigma_tail = Float("sigma tail", 0.2, 0.05, 0.4, 0.05)
+            self.invert = Bool("invert", True)
 
-            self.bbox_l = Rect("Left eye", (0, 0, 30, 30))
-            self.block_size_l = Int(
-                "Block size (px)", 11, 1, 299, odd_only=True
-            )
-            self.c_l = Int("C", 0, -100, 100)
-
-            self.bbox_r = Rect("Right eye", (0, 0, 30, 30))
-            self.block_size_r = Int(
-                "Block size (px)", 11, 1, 299, odd_only=True
-            )
-            self.c_r = Int("C", 0, -100, 100)
-
-            self.bbox_sb = Rect("Swim bladder", (0, 0, 30, 30))
-            self.block_size_sb = Int(
-                "Block size (px)", 11, 1, 299, odd_only=True
-            )
-            self.c_sb = Int("C", 0, -100, 100)
+    def __init__(
+        self,
+        roi=None,
+        params: dict = None,
+        *,
+        verbose=0,
+        debug=False,
+    ):
+        super().__init__(roi, params, verbose=verbose, debug=debug)
+        self._points = Points(np.array([[0, 0]]), 1, "m", symbol="+")
 
-            self.min_size = Int("Minimum size (px)", 5, 0, 200)
+    @classmethod
+    def _results_to_dataframe(cls, results):
+        n_segments = results.shape[-2]
+        idx = pd.MultiIndex.from_product(
+            ((f"point{i:02d}" for i in range(n_segments)), ("x", "y", "angle"))
+        )
+        return pd.DataFrame(results.reshape(len(results), -1), idx)
 
-            self.invert = Int("invert", 0, -1, 1)
+    def _track_img(self, img: np.ndarray):
+        p = self.params
 
-    @property
-    def shapes(self):
-        return super().shapes + self._bboxes
+        x, y = p.tail_base
+        if self.roi.value is not None:
+            x0, y0 = self.roi.value[:2]
+            x -= x0
+            y -= y0
+
+        angle = np.deg2rad(p.angle)
+        theta = np.deg2rad(p.theta / 2)
+        img = zcv.rgb2gray_dark_bg_blur(img, p.sigma, p.invert)
+
+        h, w = img.shape
+        n_segments = p.n_segments
+        results = np.empty((n_segments, 3))
+        d_theta = p.d_theta
+        r = p.segment_length
+
+        sigma_tail = p.sigma_tail / d_theta
+
+        for i in range(n_segments):
+            if x - r < 0 or x + r >= w or y - r < 0 or y + r >= h:
+                results[i:] = np.nan
+                break
+
+            angles = np.arange(angle - theta, angle + theta, d_theta)
+            x_ = (r * np.cos(angles)).astype(int) + x
+            y_ = (r * np.sin(angles)).astype(int) + y
+            z = img[y_, x_]
+            z = gaussian_filter(z.astype(float), sigma_tail, 1, mode="nearest")
+            argmax = (z.argmin() + z.argmax()) // 2
+            angle = angles[argmax]
+            x = x_[argmax]
+            y = y_[argmax]
+            results[i] = (x, y, angle)
 
-    @property
-    def _Params(self):
-        return self.__Params
+        return results
 
     @staticmethod
     def name():
-        return "adaptive"
+        return "gradient"
 
     @staticmethod
     def display_name():
-        return "Adaptive threshold"
-
-    def annotate(self, frame: np.ndarray) -> None:
-        super().annotate(frame)
-
-        p = self.params
-
-        for i, j in zip(self._bboxes, (p.bbox_l, p.bbox_r, p.bbox_sb)):
-            i.visible = True
-            x, y, w, h = j
-            x -= self.roi.value[0]
-            y -= self.roi.value[1]
-            i.x, i.y, i.w, i.h = x, y, w, h
-
-    def _track_contours(self, img: np.ndarray):
-        p = self.params
-
-        contours = []
-
-        temp = np.zeros_like(img)
-
-        for part in ("l", "r", "sb"):
-            x, y, w, h = getattr(p, f"bbox_{part}")
-            x -= self.roi.value[0]
-            y -= self.roi.value[1]
-
-            im = img[y : y + h, x : x + w]
-
-            block_size = getattr(p, f"block_size_{part}")
-            c = getattr(p, f"c_{part}")
-            threshold = zcv.adaptive_threshold(im, block_size, c)
-            threshold = (
-                remove_small_objects(threshold > 0, p.min_size) * 255
-            ).astype(np.uint8)
-
-            temp[y : y + h, x : x + w] = threshold
-
-            points = np.concatenate(zcv.find_contours(threshold))
-            contour = cv2.convexHull(points) + np.array([[x, y]])
-
-            # temp = np.zeros_like(im)
-            # ret = cv2.drawContours(temp, [contour], -1, 255, -1)
-            # cv2.imshow(part, ret)
-
-            contours.append(contour)
-
-        if self._debug:
-            cv2.imshow("debug", temp)
+        return "Gradient"
 
-        return contours
+    def annotate_from_results(self, a: np.ndarray) -> None:
+        self._points.visible = True
+        self._points.data = a[:, :2]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ztrack-0.4.1/ztrack/tracking/eye/binary.py` & `ztrack-1.0.0/ztrack/tracking/eye/binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import cv2
 import numpy as np
 
 import ztrack.utils.cv as zcv
 from ztrack.tracking.eye.eye_tracker import EyeParams, EyeTracker
-from ztrack.utils.variable import Float, Int, UInt8
+from ztrack.utils.variable import Bool, Float, UInt8
 
 
 class BinaryEyeTracker(EyeTracker):
     def __init__(
         self, roi=None, params: dict = None, *, verbose=0, debug=False
     ):
         super().__init__(roi, params, verbose=verbose, debug=debug)
 
     class __Params(EyeParams):
         def __init__(self, params: dict = None):
             super().__init__(params)
             self.sigma = Float("Sigma (px)", 2, 0, 100, 0.1)
             self.threshold = UInt8("Threshold", 127)
-            self.invert = Int("invert", 0, -1, 1)
+            self.invert = Bool("invert", True)
 
     @property
     def _Params(self):
         return self.__Params
 
     @staticmethod
     def name():
```

### Comparing `ztrack-0.4.1/ztrack/tracking/eye/eye_tracker.py` & `ztrack-1.0.0/ztrack/tracking/eye/eye_tracker.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/eye/multi_threshold.py` & `ztrack-1.0.0/ztrack/tracking/eye/multi_threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import cv2
 import numpy as np
 
 import ztrack.utils.cv as zcv
 from ztrack.tracking.eye.eye_tracker import EyeParams, EyeTracker
 from ztrack.utils.exception import TrackingError
-from ztrack.utils.variable import Float, Int, UInt8
+from ztrack.utils.variable import Bool, Float, UInt8
 
 
 class MultiThresholdEyeTracker(EyeTracker):
     class __Params(EyeParams):
         def __init__(self, params: dict = None):
             super().__init__(params)
             self.sigma = Float("Sigma (px)", 2, 0, 100, 0.1)
             self.threshold_segmentation = UInt8("Segmentation threshold", 127)
             self.threshold_left_eye = UInt8("Left eye threshold", 127)
             self.threshold_right_eye = UInt8("Right eye threshold", 127)
             self.threshold_swim_bladder = UInt8("Swim bladder threshold", 127)
-            self.invert = Int("invert", 0, -1, 1)
+            self.invert = Bool("invert", True)
 
     def __init__(
         self, roi=None, params: dict = None, *, verbose=0, debug=False
     ):
         super().__init__(roi, params, verbose=verbose, debug=debug)
 
     @property
```

### Comparing `ztrack-0.4.1/ztrack/tracking/free/base.py` & `ztrack-1.0.0/ztrack/tracking/free/base.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/free/contour.py` & `ztrack-1.0.0/ztrack/tracking/free/contour.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/free/sequential.py` & `ztrack-1.0.0/ztrack/tracking/free/sequential.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/mixins/background.py` & `ztrack-1.0.0/ztrack/tracking/mixins/background.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/paramecia/paramecia.py` & `ztrack-1.0.0/ztrack/tracking/paramecia/paramecia.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/params.py` & `ztrack-1.0.0/ztrack/tracking/params.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/tail/sequential.py` & `ztrack-1.0.0/ztrack/tracking/tail/sequential.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 import numpy as np
 
 import ztrack.utils.cv as zcv
-from ztrack.utils.shape import Rectangle
-from ztrack.utils.variable import Angle, Float, Int, Point, Rect, String
+from ztrack.utils.variable import Angle, Bool, Float, Int, Point, String
 
 from .tail_tracker import TailParams, TailTracker
 
 
 class SequentialTailTracker(TailTracker):
     class __Params(TailParams):
         def __init__(self, params: dict = None):
             super().__init__(params)
             self.sigma = Float("Sigma (px)", 2, 0, 100, 0.1)
             self.n_steps = Int("Number of steps", 10, 3, 20)
             self.length = Int("Tail length (px)", 200, 0, 1000)
             self.tail_base = Point("Tail base (x, y)", (250, 120))
             self.angle = Angle("Initial angle (°)", 90)
             self.theta = Angle("Search angle (°)", 60)
-            self.theta2 = Angle("Search angle 2 (°)", 60)
-            self.fraction = Float("Fraction", 0.5, 0, 1, 0.05)
-            self.bbox_l_tail = Rect("Left tail", (0, 0, 30, 30))
-            self.bbox_r_tail = Rect("Right tail", (0, 0, 30, 30))
-            self.step_lengths = String("Step lengths", "")
-            self.invert = Int("invert", 0, -1, 1)
-
-    def __init__(
-        self, roi=None, params: dict = None, *, verbose=0, debug=False
-    ):
-        super().__init__(roi, params, verbose=verbose, debug=debug)
+            self.skips = String("Skips", "")
+            self.invert = Bool("invert", True)
 
-        self._left_tail_bbox = Rectangle(0, 0, 1, 1, 4, "b")
-        self._right_tail_bbox = Rectangle(0, 0, 1, 1, 4, "r")
-        self._bboxes = [self._left_tail_bbox, self._right_tail_bbox]
+    def __init__(self, roi=None, params: dict = None, *, verbose=0, debug=False):
+        super().__init__(roi, params, verbose=verbose, debug=debug)
 
     @property
     def _Params(self):
         return self.__Params
 
     def _track_tail(self, img):
         p = self.params
@@ -45,51 +34,30 @@
             x0, y0 = self.roi.value[:2]
             point = (x - x0, y - y0)
         else:
             point = (x, y)
 
         angle = np.deg2rad(p.angle)
         theta = np.deg2rad(p.theta / 2)
-        theta2 = np.deg2rad(p.theta2 / 2)
         img = zcv.rgb2gray_dark_bg_blur(img, p.sigma, p.invert)
 
-        x, y, w, h = p.bbox_l_tail
-        img[y : y + h, x : x + w] = 0
-
-        x, y, w, h = p.bbox_r_tail
-        img[y : y + h, x : x + w] = 0
-
         return zcv.sequential_track_tail(
             img,
             point,
             angle,
             theta,
-            theta2,
-            p.fraction,
             p.n_steps,
             p.length,
-            p.step_lengths,
+            p.skips,
         )
 
     @staticmethod
     def name():
         return "sequential"
 
     @property
     def shapes(self):
-        return super().shapes + self._bboxes
+        return super().shapes
 
     @staticmethod
     def display_name():
         return "Sequential"
-
-    def annotate(self, frame: np.ndarray) -> None:
-        super().annotate(frame)
-
-        p = self.params
-
-        for i, j in zip(self._bboxes, (p.bbox_l_tail, p.bbox_r_tail)):
-            i.visible = True
-            x, y, w, h = j
-            x -= self.roi.value[0]
-            y -= self.roi.value[1]
-            i.x, i.y, i.w, i.h = x, y, w, h
```

### Comparing `ztrack-0.4.1/ztrack/tracking/tail/tail_tracker.py` & `ztrack-1.0.0/ztrack/tracking/tail/tail_tracker.py`

 * *Files identical despite different names*

### Comparing `ztrack-0.4.1/ztrack/tracking/tracker.py` & `ztrack-1.0.0/ztrack/tracking/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import traceback
 from abc import ABC, abstractmethod
 from typing import Type
 
 import numpy as np
 import pandas as pd
 from decord import VideoReader
@@ -12,17 +13,15 @@
 
 from .params import Params
 
 
 class Tracker(ABC):
     _index: pd.Index
 
-    def __init__(
-        self, roi=None, params: dict = None, *, verbose=0, debug=False
-    ):
+    def __init__(self, roi=None, params: dict = None, *, verbose=0, debug=False):
         self._debug = debug
         self._roi = Rect("", roi)
         self._params = self._Params(params)
         self._verbose = verbose
 
     def __repr__(self):
         return f"{self.__class__.__name__}(roi={self._roi.value}, params={self.params.to_dict()})"
@@ -59,17 +58,15 @@
 
     @abstractmethod
     def annotate_from_series(self, s: pd.Series) -> None:
         pass
 
     def annotate_from_results(self, a: np.ndarray) -> None:
         if a is not None:
-            return self.annotate_from_series(
-                self._results_to_dataframe(a[None]).iloc[0]
-            )
+            return self.annotate_from_series(self._results_to_dataframe(a[None]).iloc[0])
 
     @property
     def params(self) -> Params:
         return self._params
 
     @staticmethod
     @abstractmethod
@@ -102,43 +99,32 @@
         pass
 
     def __track_img(self, img: np.ndarray, i: int, ignore_error=False):
         try:
             return self._track_img(img)
         except Exception:
             if ignore_error:
-                print(f"Tracker {self.name()} failed at frame {i}")
+                logging.error(f"Tracker {self.name()} failed at frame {i}")
                 return np.nan
             raise TrackingError(i)
 
     def track_video(self, video_path, ignore_errors=False):
         self.set_video(video_path)
 
         video_reader = VideoReader(str(video_path))
-        it = (
-            tqdm(range(len(video_reader)))
-            if self._verbose
-            else range(len(video_reader))
-        )
+        it = tqdm(range(len(video_reader))) if self._verbose else range(len(video_reader))
 
         s_ = self.roi.to_slice()
         data = np.asarray(
             np.broadcast_arrays(
-                *[
-                    self.__track_img(
-                        video_reader[i].asnumpy()[s_], i, ignore_errors
-                    )
-                    for i in it
-                ]
+                *[self.__track_img(video_reader[i].asnumpy()[s_], i, ignore_errors) for i in it]
             )
         )
 
-        return self._results_to_dataframe(
-            self._transform_from_roi_to_frame(data)
-        )
+        return self._results_to_dataframe(self._transform_from_roi_to_frame(data))
 
     def set_video(self, video_path):
         pass
 
 
 class NoneTracker(Tracker):
     class __Params(Params):
```

### Comparing `ztrack-0.4.1/ztrack/utils/cv.py` & `ztrack-1.0.0/ztrack/utils/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 import cv2
 import numpy as np
 from decord import VideoReader
 from scipy.interpolate import splev, splprep
 from skimage.draw import circle_perimeter
 from tqdm import tqdm
 
-from .exception import TrackingError
 from .geometry import angle_diff
 from .math import split_int
 
 
+def winsorize(img, qmin, qmax):
+    vmin = np.quantile(img, qmin)
+    vmax = np.quantile(img, qmax)
+    return np.clip((img - vmin) / (vmax - vmin), 0, 1)
+
+
 def binary_threshold(img: np.ndarray, threshold: int) -> np.ndarray:
     return cv2.threshold(img, threshold, 255, cv2.THRESH_BINARY)[1]
 
 
 def find_contours(img: np.ndarray) -> list:
     return cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)[0]
 
@@ -50,79 +55,78 @@
     return x, y, b / 2, a / 2, theta - 90
 
 
 def rgb2gray(img: np.ndarray) -> np.ndarray:
     return cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)
 
 
-def video_median(
-    video_path: str, n_frames_for_bg=300, verbose=False
-) -> np.ndarray:
+def video_median(video_path: str, n_frames_for_bg=300, verbose=False) -> np.ndarray:
     vr = VideoReader(video_path)
     n_frames = len(vr)
     n_frames_for_bg = min(n_frames, n_frames_for_bg)
     idx = np.linspace(0, n_frames - 1, n_frames_for_bg).astype(int)
-    frames = [
-        rgb2gray(vr[i].asnumpy()) for i in (tqdm(idx) if verbose else idx)
-    ]
+    frames = [rgb2gray(vr[i].asnumpy()) for i in (tqdm(idx) if verbose else idx)]
 
     return np.median(frames, axis=0).astype(np.uint8)
 
 
 def interpolate_tail(tail: np.ndarray, n_points: int) -> np.ndarray:
     tck = splprep(tail.T)[0]
     return np.column_stack(splev(np.linspace(0, 1, n_points), tck))
 
 
 def sequential_track_tail(
-    img, point, angle, theta, theta2, fraction, n_steps, length, step_lengths
+    img,
+    point,
+    angle,
+    theta,
+    n_steps,
+    length,
+    skips,
 ):
     h, w = img.shape
-    if step_lengths.strip() != "":
-        try:
-            step_lengths = eval(step_lengths)
-        except Exception:
-            print("invalid step lengths")
-            step_lengths = split_int(round(length), n_steps)
+
+    if skips == "":
+        skips = ()
     else:
-        step_lengths = split_int(round(length), n_steps)
+        skips = np.sort(np.unique(eval(skips)))
 
+    step_lengths = split_int(round(length), n_steps + len(skips))
+
+    for skip in skips[::-1]:
+        step_lengths[skip - 1] += step_lengths[skip]
+
+    step_lengths = np.delete(step_lengths, skips)
     n_steps = len(step_lengths)
 
-    tail = np.zeros((n_steps + 1, 2), dtype=int)
+    tail = np.full((n_steps + 1, 2), -1, dtype=int)
     tail[0] = point
 
     for i in range(n_steps):
-        points = np.column_stack(
-            circle_perimeter(*point, step_lengths[i], shape=(w, h))
-        )
+        points = np.column_stack(circle_perimeter(*point, step_lengths[i], shape=(w, h)))
         angles = np.arctan2(*reversed((points - point).T))
-        lim = theta if i / n_steps < fraction else theta2
+        lim = theta
         idx = angle_diff(angles, angle) < lim
         points, angles = points[idx], angles[idx]
-        x, y = points.T
 
-        try:
-            argmax = img[y, x].argmax()
-        except ValueError:
-            raise TrackingError("Tail tracking failed")
+        if len(points) == 0:
+            break
 
+        x, y = points.T
+        argmax = img[y, x].argmax()
         angle = angles[argmax]
         tail[i + 1] = point = points[argmax]
 
     return tail
 
 
 def rgb2gray_dark_bg_blur(img, sigma=0, invert=0):
     img = cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)
 
-    if invert == 0:
-        if cv2.mean(img)[0] > 127:
-            img = cv2.bitwise_not(img)
-    elif invert == 1:
+    if invert:
         img = cv2.bitwise_not(img)
 
     if sigma > 0:
         img = cv2.GaussianBlur(img, (0, 0), sigma)
 
     return img
 
@@ -133,29 +137,24 @@
     heading_rad = np.deg2rad(heading)
     v = np.array([np.cos(heading_rad), np.sin(heading_rad)])
     bbox_midpoint = midpoint + (f - b) * v
     h = f + b
     rect = (bbox_midpoint, (w, h), heading + 90)
     box = np.int0(cv2.boxPoints(rect))
     src_pts = box.astype("float32")
-    dst_pts = np.array(
-        [[0, h - 1], [0, 0], [w - 1, 0], [w - 1, h - 1]], dtype="float32"
-    )
+    dst_pts = np.array([[0, h - 1], [0, 0], [w - 1, 0], [w - 1, h - 1]], dtype="float32")
 
     T = cv2.getPerspectiveTransform(src_pts, dst_pts)
 
     return cv2.warpPerspective(img, T, (int(w), int(h)))
 
 
 def orientation(src):
     moments = cv2.moments(src)
-    return np.rad2deg(
-        np.arctan2(2 * moments["mu11"], (moments["mu20"] - moments["mu02"]))
-        / 2
-    )
+    return np.rad2deg(np.arctan2(2 * moments["mu11"], (moments["mu20"] - moments["mu02"])) / 2)
 
 
 def fit_ellipse_moments(contour):
     m = cv2.moments(contour)
     cx = m["m10"] / m["m00"]
     cy = m["m01"] / m["m00"]
     b, a = cv2.fitEllipse(contour)[1]
```

### Comparing `ztrack-0.4.1/ztrack/utils/file.py` & `ztrack-1.0.0/ztrack/utils/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 from typing import List, Optional
 
 from ztrack._settings import config_extension, results_extension, video_extensions
 
 
 def get_results_path(video):
-    if Path(str(video)).with_suffix(results_extension).exists():
-        return Path(str(video)).with_suffix(results_extension)
-    return Path(str(video) + results_extension)
+    if Path(str(video) + results_extension).exists():
+        return Path(str(video) + results_extension)
+    return Path(video).with_suffix(results_extension)
 
 
 def get_config_path(video):
-    if Path(str(video)).with_suffix(config_extension).exists():
-        return Path(str(video)).with_suffix(config_extension)
-    return Path(str(video) + config_extension)
+    if Path(str(video) + config_extension).exists():
+        return Path(str(video) + config_extension)
+    return Path(str(video)).with_suffix(config_extension)
 
 
 def get_config_dict(video) -> Optional[dict]:
     path = get_config_path(video)
 
     if path.exists():
         with open(path) as fp:
@@ -27,25 +27,19 @@
             except json.JSONDecodeError:
                 return None
     return None
 
 
 def get_video_paths(inputs, recursive):
     paths: List[Path] = list(map(Path, inputs))
-    videos = [
-        path
-        for path in paths
-        if path.is_file() and path.suffix in video_extensions
-    ]
+    videos = [path for path in paths if path.is_file() and path.suffix in video_extensions]
 
     for path in filter(Path.is_dir, paths):
         for ext in video_extensions:
-            videos.extend(
-                path.rglob(f"*{ext}") if recursive else path.glob(f"*{ext}")
-            )
+            videos.extend(path.rglob(f"*{ext}") if recursive else path.glob(f"*{ext}"))
 
     return videos
 
 
 def get_paths_for_view_results(inputs: List[str], recursive: bool):
     videos = get_video_paths(inputs, recursive)
     videos = [file for file in videos if get_results_path(file).exists()]
@@ -56,65 +50,51 @@
     inputs: List[str], recursive: bool, same_config: bool, overwrite: bool
 ):
     def _str(path: Path):
         return path.resolve().as_posix()
 
     paths: List[Path] = [Path(path) for path in inputs]
     directories = [path for path in paths if path.is_dir()]
-    files = [
-        path
-        for path in paths
-        if path.is_file() and path.suffix in video_extensions
-    ]
+    files = [path for path in paths if path.is_file() and path.suffix in video_extensions]
 
     video_paths: List[str] = []
     save_paths: List[List[str]] = []
 
     for directory in directories:
         for ext in video_extensions:
             if recursive:
                 videos = list(directory.rglob(f"*{ext}"))
             else:
                 videos = list(directory.glob(f"*{ext}"))
 
             if not overwrite:
                 videos = [
-                    video
-                    for video in videos
-                    if not Path(str(video) + config_extension).exists()
+                    video for video in videos if not Path(str(video) + config_extension).exists()
                 ]
 
             if len(videos) > 0:
                 if same_config:
                     video_paths.append(_str(videos[0]))
                     save_paths.append([_str(video) for video in videos])
                 else:
                     for video in videos:
                         video_paths.append(_str(video))
                         save_paths.append([_str(video)])
 
     if not overwrite:
-        files = [
-            file
-            for file in files
-            if not Path(str(file) + config_extension).exists()
-        ]
+        files = [file for file in files if not Path(str(file) + config_extension).exists()]
 
     for file in files:
         video_paths.append(_str(file))
         save_paths.append([_str(file)])
 
     return video_paths, save_paths
 
 
-def get_video_paths_from_inputs(
-    inputs: List[str], recursive: bool, overwrite: bool
-):
+def get_video_paths_from_inputs(inputs: List[str], recursive: bool, overwrite: bool):
     videos = get_video_paths(inputs, recursive)
     videos = [file for file in videos if get_config_path(file).exists()]
 
     if not overwrite:
-        videos = [
-            file for file in videos if not get_results_path(file).exists()
-        ]
+        videos = [file for file in videos if not get_results_path(file).exists()]
 
     return videos
```

### Comparing `ztrack-0.4.1/ztrack/utils/variable.py` & `ztrack-1.0.0/ztrack/utils/variable.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,14 +67,53 @@
         return self._value
 
     @value.setter
     def value(self, value: str):
         self._value = value
 
 
+class FloatRange(Variable):
+    def __init__(self, display_name: str, value, minimum=0.0, maximum=1.0):
+        super().__init__(display_name)
+        vmin, vmax = value
+        assert minimum <= maximum
+        assert vmin <= vmax
+        self._value = (vmin, vmax)
+        self._minimum = minimum
+        self._maximum = maximum
+        # self._step = step
+        # self._strict = strict
+
+    @property
+    def value(self) -> Tuple[float, float]:
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        vmin, vmax = value
+        assert vmin <= vmax
+        self._value = (vmin, vmax)
+
+    @property
+    def minimum(self):
+        return self._minimum
+
+    @property
+    def maximum(self):
+        return self._maximum
+
+    @property
+    def step(self):
+        return self._step
+
+    @property
+    def strict(self):
+        return self._strict
+
+
 class Rect(Variable):
     def __init__(self, display_name: str, bbox=None):
         super().__init__(display_name)
         if bbox is not None:
             x, y, w, h = bbox
             bbox = x, y, w, h
         self._value = bbox
@@ -116,14 +155,18 @@
         return self._value
 
     @value.setter
     def value(self, value):
         self._value = value
 
 
+class Bool(Numerical):
+    pass
+
+
 class Bounded(Numerical, ABC):
     def __init__(self, display_name: str, value, minimum, maximum):
         super().__init__(display_name, value)
         assert minimum <= value <= maximum
         self._minimum = minimum
         self._maximum = maximum
```

### Comparing `ztrack-0.4.1/PKG-INFO` & `ztrack-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: ztrack
-Version: 0.4.1
+Version: 1.0.0
 Summary: 
 Home-page: https://github.com/kclamar/ztrack
 License: MIT
 Author: Ka Chung Lam
 Author-email: kclamar@connect.ust.hk
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
-Requires-Dist: PyQt5 (>=5.15.4,<6.0.0)
-Requires-Dist: PyQt5-stubs; extra == "dev"
-Requires-Dist: bump2version; extra == "dev"
+Requires-Dist: PyQt5 (>=5.10.1,<6.0.0)
+Requires-Dist: PyQt5-stubs ; extra == "dev"
+Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: decord (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.4.2,<4.0.0)
 Requires-Dist: opencv-python (>=4.5.2,<5.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
-Requires-Dist: pandas-stubs; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pandas-stubs ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pyqtgraph (>=0.12.2,<0.13.0)
 Requires-Dist: qtmodern (>=0.2.0,<0.3.0)
 Requires-Dist: scikit-image (>=0.18.2,<0.19.0)
-Requires-Dist: tables (>=3.6.1,<4.0.0)
+Requires-Dist: superqt (>=0.3,<0.4)
+Requires-Dist: tables (==3.6.1)
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
 Project-URL: Repository, https://github.com/kclamar/ztrack
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/ztrack.svg)](https://pypi.python.org/pypi/ztrack)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ztrack.svg)](https://pypi.python.org/pypi/ztrack)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```


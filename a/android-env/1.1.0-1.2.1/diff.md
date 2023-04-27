# Comparing `tmp/android_env-1.1.0.tar.gz` & `tmp/android-env-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/agergely/android_env/dist/tmpz8pcqnn4/android_env-1.1.0.tar", last modified: Thu Oct  7 22:22:56 2021, max compression
+gzip compressed data, was "android-env-1.2.1.tar", last modified: Thu Apr 27 15:13:29 2023, max compression
```

## Comparing `android_env-1.1.0.tar` & `android-env-1.2.1.tar`

### file list

```diff
@@ -1,73 +1,88 @@
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.496801 android_env-1.1.0/
--rw-r--r--   0 agergely (726598) primarygroup (89939)    11357 2021-10-07 22:21:10.000000 android_env-1.1.0/LICENSE
--rw-r--r--   0 agergely (726598) primarygroup (89939)      469 2021-10-07 22:22:56.496361 android_env-1.1.0/PKG-INFO
--rw-r--r--   0 agergely (726598) primarygroup (89939)     7771 2021-10-07 22:21:10.000000 android_env-1.1.0/README.md
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.463819 android_env-1.1.0/android_env/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      703 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/__init__.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.483010 android_env-1.1.0/android_env/components/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      610 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/__init__.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)      828 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/action_type.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    24535 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/adb_controller.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    16068 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/adb_controller_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     1462 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/adb_log_stream.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     1560 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/adb_log_stream_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     8034 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/app_screen_checker.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5955 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/app_screen_checker_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    12533 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/coordinator.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     6308 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/coordinator_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4996 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/dumpsys_thread.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3567 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/dumpsys_thread_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3098 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/errors.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     1535 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/log_stream.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2485 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/log_stream_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5667 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/logcat_thread.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4370 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/logcat_thread_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    11720 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/setup_step_interpreter.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    14297 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/setup_step_interpreter_test.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.484628 android_env-1.1.0/android_env/components/simulators/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      888 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/__init__.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     8645 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/base_simulator.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5734 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/base_simulator_test.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.487392 android_env-1.1.0/android_env/components/simulators/emulator/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      610 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/emulator/__init__.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     8287 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/emulator/emulator_launcher.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5734 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/emulator/emulator_launcher_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     6588 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/emulator/emulator_simulator.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     9058 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/emulator/emulator_simulator_test.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.489833 android_env-1.1.0/android_env/components/simulators/fake/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      610 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/fake/__init__.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5030 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/fake/fake_simulator.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2586 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/simulators/fake/fake_simulator_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4768 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/specs.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5002 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/specs_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    13481 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/task_manager.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)    12689 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/task_manager_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3815 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/thread_function.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2153 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/thread_function_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     1831 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/utils.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2787 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/components/utils_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4381 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/environment.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     6499 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/environment_test.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2719 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/loader.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3591 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/loader_test.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.490440 android_env-1.1.0/android_env/proto/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      610 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/proto/__init__.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.495663 android_env-1.1.0/android_env/wrappers/
--rw-r--r--   0 agergely (726598) primarygroup (89939)     1356 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/__init__.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2134 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/base_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     5901 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/discrete_action_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4177 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/flat_interface_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2565 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/float_pixels_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2968 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/gym_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4212 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/image_rescale_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     4312 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/last_action_wrapper.py
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3517 2021-10-07 22:21:10.000000 android_env-1.1.0/android_env/wrappers/tap_action_wrapper.py
-drwxr-xr-x   0 agergely (726598) primarygroup (89939)        0 2021-10-07 22:22:56.466743 android_env-1.1.0/android_env.egg-info/
--rw-r--r--   0 agergely (726598) primarygroup (89939)      469 2021-10-07 22:22:56.000000 android_env-1.1.0/android_env.egg-info/PKG-INFO
--rw-r--r--   0 agergely (726598) primarygroup (89939)     2524 2021-10-07 22:22:56.000000 android_env-1.1.0/android_env.egg-info/SOURCES.txt
--rw-r--r--   0 agergely (726598) primarygroup (89939)        1 2021-10-07 22:22:56.000000 android_env-1.1.0/android_env.egg-info/dependency_links.txt
--rw-r--r--   0 agergely (726598) primarygroup (89939)      171 2021-10-07 22:22:56.000000 android_env-1.1.0/android_env.egg-info/requires.txt
--rw-r--r--   0 agergely (726598) primarygroup (89939)       12 2021-10-07 22:22:56.000000 android_env-1.1.0/android_env.egg-info/top_level.txt
--rw-r--r--   0 agergely (726598) primarygroup (89939)      103 2021-06-09 18:28:55.000000 android_env-1.1.0/pyproject.toml
--rw-r--r--   0 agergely (726598) primarygroup (89939)       38 2021-10-07 22:22:56.496968 android_env-1.1.0/setup.cfg
--rw-r--r--   0 agergely (726598) primarygroup (89939)     3746 2021-10-07 22:22:27.000000 android_env-1.1.0/setup.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.576698 android-env-1.2.1/
+-rw-rw-r--   0 kenjitoyama (156877) primarygroup (89939)    11357 2021-01-19 09:11:58.000000 android-env-1.2.1/LICENSE
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    13727 2023-04-27 15:13:29.572697 android-env-1.2.1/PKG-INFO
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     7771 2023-04-27 13:42:56.000000 android-env-1.2.1/README.md
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.560696 android-env-1.2.1/android_env/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/__init__.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.568697 android-env-1.2.1/android_env/components/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      882 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/action_type.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    31189 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_call_parser.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    55184 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_call_parser_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4116 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_controller.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2160 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_controller_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     1462 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_log_stream.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     1574 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/adb_log_stream_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     9714 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/app_screen_checker.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     7664 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/app_screen_checker_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    20069 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/coordinator.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    16569 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/coordinator_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4730 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/dumpsys_thread.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3866 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/dumpsys_thread_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     1696 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/errors.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2037 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/log_stream.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3494 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/log_stream_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4728 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/logcat_thread.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4291 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/logcat_thread_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6536 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/setup_step_interpreter.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    11752 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/setup_step_interpreter_test.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.568697 android-env-1.2.1/android_env/components/simulators/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4565 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/base_simulator.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2122 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/base_simulator_test.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.568697 android-env-1.2.1/android_env/components/simulators/emulator/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/emulator/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6561 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/emulator/emulator_launcher.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6604 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/emulator/emulator_launcher_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    11928 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/emulator/emulator_simulator.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    11220 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/emulator/emulator_simulator_test.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.568697 android-env-1.2.1/android_env/components/simulators/fake/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/fake/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4282 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/fake/fake_simulator.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3747 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/simulators/fake/fake_simulator_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5192 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/specs.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5600 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/specs_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    13311 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/task_manager.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    17100 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/task_manager_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2619 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/utils.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3889 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/components/utils_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2879 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/env_interface.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5296 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/environment.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     8949 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/environment_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2682 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/loader.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3565 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/loader_test.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.572697 android-env-1.2.1/android_env/proto/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/proto/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    12046 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/proto/adb.proto
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    41044 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/proto/emulator_controller.proto
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     1327 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/proto/raw_observation.proto
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6597 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/proto/task.proto
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.572697 android-env-1.2.1/android_env/wrappers/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      610 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/__init__.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2988 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/base_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5180 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/base_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5901 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/discrete_action_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    14363 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/discrete_action_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4177 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/flat_interface_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6173 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/flat_interface_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2597 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/float_pixels_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     5266 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/float_pixels_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     2968 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/gym_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4026 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/gym_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4214 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/image_rescale_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4024 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/image_rescale_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4312 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/last_action_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     6117 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/last_action_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4092 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/rate_limit_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     8387 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/rate_limit_wrapper_test.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3504 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/tap_action_wrapper.py
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     4717 2023-04-27 13:42:56.000000 android-env-1.2.1/android_env/wrappers/tap_action_wrapper_test.py
+drwxr-x---   0 kenjitoyama (156877) primarygroup (89939)        0 2023-04-27 15:13:29.560696 android-env-1.2.1/android_env.egg-info/
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)    13727 2023-04-27 15:13:29.000000 android-env-1.2.1/android_env.egg-info/PKG-INFO
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3171 2023-04-27 15:13:29.000000 android-env-1.2.1/android_env.egg-info/SOURCES.txt
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)        1 2023-04-27 15:13:29.000000 android-env-1.2.1/android_env.egg-info/dependency_links.txt
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)      187 2023-04-27 15:13:29.000000 android-env-1.2.1/android_env.egg-info/requires.txt
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)       12 2023-04-27 15:13:29.000000 android-env-1.2.1/android_env.egg-info/top_level.txt
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     1048 2023-04-27 15:13:15.000000 android-env-1.2.1/pyproject.toml
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)       38 2023-04-27 15:13:29.576698 android-env-1.2.1/setup.cfg
+-rw-r-----   0 kenjitoyama (156877) primarygroup (89939)     3112 2023-04-27 14:43:44.000000 android-env-1.2.1/setup.py
```

### Comparing `android_env-1.1.0/LICENSE` & `android-env-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `android_env-1.1.0/README.md` & `android-env-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `android_env-1.1.0/android_env/__init__.py` & `android-env-1.2.1/android_env/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Init file for android_env package."""
-
-from android_env import loader
-
-load = loader.load
```

### Comparing `android_env-1.1.0/android_env/components/__init__.py` & `android-env-1.2.1/android_env/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/components/action_type.py` & `android-env-1.2.1/android_env/components/action_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,12 +14,16 @@
 # limitations under the License.
 
 """The different kinds of actions that AndroidEnv supports."""
 
 import enum
 
 
+@enum.unique
 class ActionType(enum.IntEnum):
   """Integer values to describe each supported action in AndroidEnv."""
   TOUCH = 0
   LIFT = 1
   REPEAT = 2
+  KEYDOWN = 3
+  KEYUP = 4
+  KEYPRESS = 5
```

### Comparing `android_env-1.1.0/android_env/components/adb_log_stream.py` & `android-env-1.2.1/android_env/components/adb_log_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/components/adb_log_stream_test.py` & `android-env-1.2.1/android_env/components/adb_log_stream_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for adb_log_stream."""
 
 import subprocess
+from unittest import mock
 
 from absl.testing import absltest
 from android_env.components import adb_log_stream
-import mock
 
 
 class FakeAdbSubprocess():
 
   @property
   def stdout(self):
     return [f'line_{i}' for i in range(100)]
```

### Comparing `android_env-1.1.0/android_env/components/app_screen_checker.py` & `android-env-1.2.1/android_env/components/app_screen_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,49 +13,52 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Determines if the current app screen matches an expected app screen."""
 
 import enum
 import re
+import time
 from typing import Callable, List, Optional, Sequence, Pattern
 
 from absl import logging
 
-from android_env.components import adb_controller as adb_control
+from android_env.components import adb_call_parser as adb_call_parser_lib
+from android_env.components import errors
+from android_env.proto import adb_pb2
 from android_env.proto import task_pb2
 
 
-class DumpsysNode():
+class _DumpsysNode():
   """A node in a dumpsys tree."""
 
   def __init__(self, data: Optional[str] = None):
     self._children = []
     self._data = data
 
   @property
   def data(self) -> str:
     return self._data
 
   @property
-  def children(self) -> List['DumpsysNode']:
+  def children(self) -> List['_DumpsysNode']:
     return self._children
 
   def find_child(self,
-                 predicate: Callable[['DumpsysNode'], bool],
-                 max_levels: int = 0) -> Optional['DumpsysNode']:
+                 predicate: Callable[['_DumpsysNode'], bool],
+                 max_levels: int = 0) -> Optional['_DumpsysNode']:
     """Returns the first direct child that matches `predicate`, None otherwise.
 
     Args:
-      predicate: Function-like that accepts a DumpsysNode and returns boolean.
+      predicate: Function-like that accepts a _DumpsysNode and returns boolean.
       max_levels: Maximum number of levels down the tree to search for a child.
         If non-positive, only direct children will be searched for.
 
     Returns:
-      A DumpsysNode or None.
+      A _DumpsysNode or None.
     """
     if not self.children:
       return None
 
     try:
       return next(x for x in self.children if predicate(x))
     except StopIteration:
@@ -75,35 +78,35 @@
   def print_tree(self, indent: int = 2):
     """Prints this tree in logging.info()."""
     logging.info(' ' * indent + self.data)
     for c in self.children:
       c.print_tree(indent + 2)
 
 
-def build_tree_from_dumpsys_output(dumpsys_output: str) -> DumpsysNode:
+def build_tree_from_dumpsys_output(dumpsys_output: str) -> _DumpsysNode:
   """Constructs a tree from a dumpsys string output.
 
   Args:
     dumpsys_output: string Verbatim output from adb dumpsys. The expected format
       is a list where each line is a node and the indentation marks the
       relationship with its parent or sibling.
 
   Returns:
-    DumpsysNode The root of the tree.
+    _DumpsysNode The root of the tree.
   """
   lines = dumpsys_output.split('\n')  # Split by lines.
   lines = [x.rstrip(' \r') for x in lines]
   lines = [x for x in lines if len(x)]  # Remove empty lines.
 
-  root = DumpsysNode('___root___')  # The root of all nodes.
+  root = _DumpsysNode('___root___')  # The root of all nodes.
   parents_stack = [root]
   for line in lines:
     stripped_line = line.lstrip(' ')
     indent = len(line) - len(stripped_line)  # Number of indent spaces.
-    new_node = DumpsysNode(stripped_line)  # Create a node without indentation.
+    new_node = _DumpsysNode(stripped_line)  # Create a node without indentation.
 
     parent = parents_stack.pop()
     if parent.data == '___root___':  # The root is an exception for indentation.
       parent_indent = -2
     else:
       parent_indent = (len(parents_stack) - 1) * 2
 
@@ -180,47 +183,85 @@
     # We were unable to determine the current activity.
     FAILED_ACTIVITY_EXTRACTION = 2
     # The current activity does not match the expected activity.
     UNEXPECTED_ACTIVITY = 3
     # The current view hierarchy does not match the expected view hierarchy.
     UNEXPECTED_VIEW_HIERARCHY = 4
 
-  def __init__(self,
-               adb_controller: adb_control.AdbController,
+  def __init__(self, adb_call_parser: adb_call_parser_lib.AdbCallParser,
                expected_app_screen: task_pb2.AppScreen):
-    self._adb_controller = adb_controller
+    self._adb_call_parser = adb_call_parser
+    self._expected_app_screen = expected_app_screen
     self._expected_activity = expected_app_screen.activity
     self._expected_view_hierarchy_path = [
         re.compile(regex) for regex in expected_app_screen.view_hierarchy_path
     ]
 
   # Return type is AppScreenChecker.Outcome, but pytype doesn't understand that.
   def matches_current_app_screen(self) -> enum.IntEnum:
     """Determines whether the current app screen matches `expected_app_screen`."""
     if not self._expected_activity:
       return AppScreenChecker.Outcome.EMPTY_EXPECTED_ACTIVITY
 
     # Check if we are still on the expected Activity.
-    current_activity = self._adb_controller.get_current_activity()
-    if current_activity is None:
+    response = self._adb_call_parser.parse(
+        adb_pb2.AdbRequest(
+            get_current_activity=adb_pb2.AdbRequest.GetCurrentActivity()))
+    if response.status != adb_pb2.AdbResponse.OK:
       return AppScreenChecker.Outcome.FAILED_ACTIVITY_EXTRACTION
 
+    current_activity = response.get_current_activity.full_activity
     if current_activity != self._expected_activity:
       logging.error('current_activity: %s,  expected_activity: %s',
                     current_activity, self._expected_activity)
       return AppScreenChecker.Outcome.UNEXPECTED_ACTIVITY
 
     # Extract just the package name from the full activity name.
     package_name = self._expected_activity.split('/')[0]
 
     # Check if we are in the expected view hierarchy path.
     if self._expected_view_hierarchy_path:
-      dumpsys_activity_output = self._adb_controller.get_activity_dumpsys(
-          package_name)
-      if dumpsys_activity_output:
+      dumpsys_response = self._adb_call_parser.parse(
+          adb_pb2.AdbRequest(
+              dumpsys=adb_pb2.AdbRequest.DumpsysRequest(
+                  service='activity', args=[package_name, package_name])))
+      if dumpsys_response.status != adb_pb2.AdbResponse.OK:
+        return AppScreenChecker.Outcome.FAILED_ACTIVITY_EXTRACTION
+
+      if dumpsys_response.dumpsys.output:
         if not matches_path(
-            dumpsys_activity_output,
+            dumpsys_response.dumpsys.output.decode('utf-8'),
             self._expected_view_hierarchy_path,
             max_levels=3):
           return AppScreenChecker.Outcome.UNEXPECTED_VIEW_HIERARCHY
 
     return AppScreenChecker.Outcome.SUCCESS
+
+  def wait_for_app_screen(self, timeout_sec: float) -> float:
+    """Waits for `self._expected_app_screen` to be the current screen.
+
+    Args:
+      timeout_sec: Maximum total time to wait for the screen to pop up.
+
+    Returns:
+      The total amount of time in seconds spent waiting for the screen to pop
+      up.
+    Raises:
+      errors.WaitForAppScreenError if the screen does not pop up within
+      `timeout_sec`.
+    """
+
+    logging.info('Waiting for app screen...')
+    start_time = time.time()
+    while time.time() - start_time < timeout_sec:
+      if self.matches_current_app_screen() == AppScreenChecker.Outcome.SUCCESS:
+        wait_time = time.time() - start_time
+        logging.info('Successfully waited for app screen in %r seconds: [%r]',
+                     wait_time, self._expected_app_screen)
+        return wait_time
+      time.sleep(0.1)
+
+    wait_time = time.time() - start_time
+    logging.error('Failed to wait for app screen in %r seconds: [%r].',
+                  wait_time, self._expected_app_screen)
+
+    raise errors.WaitForAppScreenError()
```

### Comparing `android_env-1.1.0/android_env/components/app_screen_checker_test.py` & `android-env-1.2.1/android_env/components/app_screen_checker_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,20 +13,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for android_env.components.app_screen_checker."""
 
 import re
 from typing import Sequence
+from unittest import mock
 
 from absl.testing import absltest
+from android_env.components import adb_call_parser
 from android_env.components import app_screen_checker
+from android_env.components import errors
+from android_env.proto import adb_pb2
+from android_env.proto import task_pb2
 
 
-def flatten_tree(tree: app_screen_checker.DumpsysNode,
+def flatten_tree(tree: app_screen_checker._DumpsysNode,
                  flat_tree: Sequence[str],
                  indent: int = 2):
   """Appends a list of strings to `flat_tree` from `tree`."""
   flat_tree.append(' ' * indent + tree.data)
   for c in tree.children:
     flatten_tree(c, flat_tree, indent + 2)
 
@@ -221,10 +226,42 @@
     expected_view_hierarchy_path = [
         re.compile(regex) for regex in expected_path
     ]
     self.assertFalse(
         app_screen_checker.matches_path(
             dumpsys_output, expected_view_hierarchy_path, max_levels=2))
 
+  def test_wait_for_app_screen_zero_timeout(self):
+    """Ensures that an exception is raised if the timeout is passed."""
+    app_screen = task_pb2.AppScreen(activity='whatever.MyActivity')
+    call_parser = mock.create_autospec(adb_call_parser.AdbCallParser)
+    screen_checker = app_screen_checker.AppScreenChecker(
+        adb_call_parser=call_parser,
+        expected_app_screen=app_screen)
+    # With a zero timeout, the method should never be able to wait for the
+    # screen to pop up and an exception should be raised.
+    self.assertRaises(
+        errors.WaitForAppScreenError,
+        screen_checker.wait_for_app_screen,
+        timeout_sec=0.0)
+
+  def test_wait_for_app_screen_successful(self):
+    """Ensures that with the right conditions, the app screen should pop up."""
+    app_screen = task_pb2.AppScreen(activity='my.favorite.AwesomeActivity')
+    call_parser = mock.create_autospec(adb_call_parser.AdbCallParser)
+    call_parser.parse.return_value = adb_pb2.AdbResponse(
+        status=adb_pb2.AdbResponse.Status.OK,
+        get_current_activity=adb_pb2.AdbResponse.GetCurrentActivityResponse(
+            full_activity='my.favorite.AwesomeActivity'))
+
+    screen_checker = app_screen_checker.AppScreenChecker(
+        call_parser, app_screen)
+    timeout = 1.0
+    wait_time = screen_checker.wait_for_app_screen(timeout_sec=timeout)
+
+    # The call should not generate an exception and the return value should be
+    # less than the timeout given.
+    self.assertLess(wait_time, timeout)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `android_env-1.1.0/android_env/components/dumpsys_thread.py` & `android-env-1.2.1/android_env/components/dumpsys_thread.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,117 +11,116 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A ThreadFunction that runs and parses adb dumpsys."""
 
-import enum
+import concurrent.futures
+from typing import Optional
 
 from absl import logging
+from android_env.components import app_screen_checker as app_screen_checker_lib
 
-from android_env.components import app_screen_checker as screen_checker
-from android_env.components import thread_function
+_Outcome = app_screen_checker_lib.AppScreenChecker.Outcome
 
-AppScreenChecker = screen_checker.AppScreenChecker
 
-
-class DumpsysThread(thread_function.ThreadFunction):
-  """A class that executes dumpsys in a separate thread."""
-
-  class Signal(enum.IntEnum):
-    """Defines commands we can use to communicate with the dumpsys thread."""
-    # To ask the thread to fetch dumpsys from Android.
-    FETCH_DUMPSYS = 0
-    # The user has left the activity that contains the AndroidEnv task.
-    USER_EXITED_ACTIVITY = 1
-    # The user exited the view hierarchy that we expect.
-    USER_EXITED_VIEW_HIERARCHY = 2
-    # App screen checker determined none of the errors above happened.
-    OK = 3
-    # App screen checker was not queried.
-    DID_NOT_CHECK = 4
+class DumpsysThread:
+  """A thread that checks if the user is in the expected app screen."""
 
   def __init__(
       self,
-      app_screen_checker: AppScreenChecker,
-      check_frequency: int,
-      max_failed_current_activity: int,
-      block_input: bool,
-      block_output: bool,
-      name: str = 'dumpsys',
+      app_screen_checker: app_screen_checker_lib.AppScreenChecker,
+      check_frequency: int = 10,
+      max_failed_current_activity: int = 10,
   ):
     """Initializes the dumpsys reader thread.
 
-    This loops forever waiting for inputs from the main thread and outputting
-    its analyses of the output of ADB dumpsys. These analyses are too expensive
-    to be in the critical path of AndroidEnv::step() so we consume them async
-    from this separate thread.
+    This loops forever checking if the user is in the expected screen dictated
+    by `app_screen_checker`. These analyses are too expensive to be in the
+    critical path of AndroidEnv::step() so we consume them async from this
+    separate thread.
 
     Args:
       app_screen_checker: The class that actually determines if the current
           screen matches the expected screen.
       check_frequency: Integer. We only call dumpsys 1/check_frequency times in
           each iteration of the while loop below.
       max_failed_current_activity: Integer. We try to fetch the current activity
           but sometimes it fails. If it fails more than
           `max_failed_current_activity` consecutive times, we declare that the
           user has exited `expected_activity`.
-      block_input: Whether to block this thread when reading its input queue.
-      block_output: Whether to block this thread when writing to its output
-        queue.
-      name: Name of the thread.
     """
 
     self._app_screen_checker = app_screen_checker
     self._main_loop_counter = 0
     self._check_frequency = check_frequency
     self._max_failed_activity_extraction = max_failed_current_activity
     self._num_failed_activity_extraction = 0
-    super().__init__(
-        block_input=block_input, block_output=block_output, name=name)
+    self._latest_check: Optional[concurrent.futures.Future] = None
 
-  def main(self):
-    v = self._read_value()
-    if v != DumpsysThread.Signal.FETCH_DUMPSYS:
-      self._write_value(DumpsysThread.Signal.DID_NOT_CHECK)
-      return
+  def check_user_exited(self, timeout: Optional[float] = None) -> bool:
+    """Returns True if the user is not in the expected screen.
+
+    Args:
+      timeout: An optional time in seconds to block waiting for the result of
+        the (expensive) checking operation. If None, the function will return
+        immediately with `False`.
+
+    Returns:
+      Whether the user of the Android device has exited the expected screen
+      determined by `AppScreenChecker` given at __init__().
+    """
 
     # Update and check loop_counter against check_frequency.
     self._main_loop_counter += 1
     if (self._check_frequency <= 0 or
         self._main_loop_counter < self._check_frequency):
-      self._write_value(DumpsysThread.Signal.DID_NOT_CHECK)
-      return
+      return False
     self._main_loop_counter = 0
 
+    # If the latest check is None, perform a check and return.
+    if self._latest_check is None:
+      with concurrent.futures.ThreadPoolExecutor() as executor:
+        self._latest_check = executor.submit(self._check_impl)
+      return False
+
+    # If there's a check in flight, continue only if it's finished.
+    if not timeout and not self._latest_check.done():
+      return False
+
+    v = self._latest_check.result(timeout=timeout)
+    self._latest_check = None  # Reset the check.
+    return v
+
+  def _check_impl(self) -> bool:
+    """The synchronous implementation of Dumpsys."""
+
     outcome = self._app_screen_checker.matches_current_app_screen()
 
     # We were unable to determine the current activity.
-    if outcome == AppScreenChecker.Outcome.FAILED_ACTIVITY_EXTRACTION:
+    if outcome == _Outcome.FAILED_ACTIVITY_EXTRACTION:
       self._num_failed_activity_extraction += 1
       logging.info('self._num_failed_activity_extraction: %s',
                    self._num_failed_activity_extraction)
       if (self._num_failed_activity_extraction >=
           self._max_failed_activity_extraction):
         logging.error('Maximum number of failed activity extraction reached.')
         self._num_failed_activity_extraction = 0
-        self._write_value(DumpsysThread.Signal.USER_EXITED_ACTIVITY)
-        return
+        return True
     else:
       self._num_failed_activity_extraction = 0
 
     # The current app screen matches all expectations.
-    if (outcome == AppScreenChecker.Outcome.SUCCESS or
-        outcome == AppScreenChecker.Outcome.EMPTY_EXPECTED_ACTIVITY):
-      self._write_value(DumpsysThread.Signal.OK)
-      return
+    if (outcome == _Outcome.SUCCESS or
+        outcome == _Outcome.EMPTY_EXPECTED_ACTIVITY):
+      return False
 
     # Player has exited the app. Terminate the episode.
-    elif outcome == AppScreenChecker.Outcome.UNEXPECTED_ACTIVITY:
-      self._write_value(DumpsysThread.Signal.USER_EXITED_ACTIVITY)
-      return
+    elif outcome == _Outcome.UNEXPECTED_ACTIVITY:
+      return True
 
     # Player has exited the main game. Terminate the episode.
-    elif outcome == AppScreenChecker.Outcome.UNEXPECTED_VIEW_HIERARCHY:
-      self._write_value(DumpsysThread.Signal.USER_EXITED_VIEW_HIERARCHY)
-      return
+    elif outcome == _Outcome.UNEXPECTED_VIEW_HIERARCHY:
+      return True
+
+    return False
```

### Comparing `android_env-1.1.0/android_env/components/log_stream.py` & `android-env-1.2.1/android_env/components/log_stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,38 +12,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Abstract class for handling a stream of logs from a simulator."""
 
 import abc
-from typing import List
+import threading
+from typing import Generator, List
 from absl import logging
 
 
 class LogStream(metaclass=abc.ABCMeta):
   """Manages the stream of logs output by a simulator."""
 
   def __init__(self, verbose: bool = False):
     self._verbose = verbose
     self._filters = []
+    self._should_stream = threading.Event()
 
-  def get_stream_output(self):
+  def get_stream_output(self) -> Generator[str, None, None]:
     """Starts log process and returns the stream of logs."""
     for line in self._get_stream_output():
       if self._verbose:
         logging.info('line: %r', line)
-      yield line
+      if self._should_stream.is_set():
+        yield line
 
   @abc.abstractmethod
   def _get_stream_output(self):
     """Starts log process and returns the stream of logs."""
     pass
 
   @abc.abstractmethod
-  def stop_stream(self):
-    """Stops the log stream from the simulator."""
+  def stop_stream(self) -> None:
+    """Terminates log stream process from the simulator."""
     pass
 
+  def pause_stream(self) -> None:
+    """No lines are yielded while the event is not set."""
+    logging.info('Pausing LogStream.')
+    self._should_stream.clear()
+
+  def resume_stream(self) -> None:
+    """The stream will continue yielding lines if the event is set."""
+    logging.info('Resuming LogStream.')
+    self._should_stream.set()
+
   def set_log_filters(self, log_filters: List[str]):
     """Sets the filters for the log stream."""
     self._filters = list(log_filters) + ['*:S']
```

### Comparing `android_env-1.1.0/android_env/components/logcat_thread_test.py` & `android-env-1.2.1/android_env/components/logcat_thread_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -51,33 +51,26 @@
         continue
       else:
         with self._lock:
           next_value = self._values.pop(0)
         yield next_value
 
 
-def _log_parsing_config():
-  """Returns log_parsing_config object for testing."""
-
-  return task_pb2.LogParsingConfig(
-      filters=['AndroidRLTask:V'])
-
-
 def make_stdout(data):
   """Returns a valid log output with given data as message."""
   return '         1553110400.424  5583  5658 D Tag: %s' % data
 
 
 class FakeLogStream(log_stream.LogStream):
-  """Add doc string."""
+  """FakeLogStream class that wraps a FakeStream."""
 
   def __init__(self):
+    super().__init__(verbose=False)
     self.logs = FakeStream()
     self.stream_is_alive = True
-    self._verbose = False
 
   def _get_stream_output(self):
     return self.logs
 
   def stop_stream(self):
     self.stream_is_alive = False
     self.logs.kill()
@@ -90,61 +83,59 @@
     self.fake_log_stream = FakeLogStream()
 
   def tearDown(self):
     self.fake_log_stream.stop_stream()
     super().tearDown()
 
   def test_set_filters(self):
-    _ = logcat_thread.LogcatThread(
-        log_stream=self.fake_log_stream,
-        log_parsing_config=_log_parsing_config())
+    log_parsing_config = task_pb2.LogParsingConfig(filters=['AndroidRLTask:V'])
+    self.fake_log_stream.set_log_filters(log_parsing_config.filters)
+    _ = logcat_thread.LogcatThread(log_stream=self.fake_log_stream)
     expected_filters = ['AndroidRLTask:V', '*:S']
     self.assertEqual(expected_filters, self.fake_log_stream._filters)
 
   def test_kill(self):
-    logcat = logcat_thread.LogcatThread(
-        log_stream=self.fake_log_stream,
-        log_parsing_config=_log_parsing_config())
+    logcat = logcat_thread.LogcatThread(log_stream=self.fake_log_stream)
     self.assertTrue(self.fake_log_stream.stream_is_alive)
     logcat.kill()
     self.assertFalse(self.fake_log_stream.stream_is_alive)
 
   def test_listeners(self):
     """Ensures that we can wait for a specific message without polling."""
-    logcat = logcat_thread.LogcatThread(
-        log_stream=self.fake_log_stream,
-        log_parsing_config=_log_parsing_config())
+    logcat = logcat_thread.LogcatThread(log_stream=self.fake_log_stream)
+    # Start yielding lines from LogStream.
+    logcat.resume()
 
     # Set up a listener that modifies an arbitrary state.
-    some_state = False
+    some_state = threading.Event()
 
     def my_handler(event: Pattern[str], match: Match[str]):
       del event, match
       nonlocal some_state
-      some_state = True
+      some_state.set()
 
     # Create a desired event and hook up the listener.
     my_event = re.compile('Hello world')
     listener = logcat_thread.EventListener(my_event, my_handler)
     logcat.add_event_listener(listener)
     self.fake_log_stream.logs.send_value('Hi there!')  # This should not match.
-    self.assertFalse(some_state)
+    self.assertFalse(some_state.is_set())
     self.fake_log_stream.logs.send_value(make_stdout('Hello world'))
-    logcat.wait(event=my_event, timeout_sec=1.0)
-    self.assertTrue(some_state)
+    some_state.wait(timeout=1.0)
+    self.assertTrue(some_state.is_set())
 
     # Waiting for any events should also trigger the listener.
-    some_state = False
+    some_state.clear()
     self.fake_log_stream.logs.send_value(make_stdout('Hello world'))
-    logcat.wait(event=None, timeout_sec=1.0)
-    self.assertTrue(some_state)
+    some_state.wait(timeout=1.0)
+    self.assertTrue(some_state.is_set())
 
     # After removing the listener, it should not be called anymore.
-    some_state = False
+    some_state.clear()
     logcat.remove_event_listener(listener)
     self.fake_log_stream.logs.send_value(make_stdout('Hello world'))
-    logcat.wait(event=my_event, timeout_sec=1.0)
-    self.assertFalse(some_state)
+    some_state.wait(timeout=1.0)
+    self.assertFalse(some_state.is_set())
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `android_env-1.1.0/android_env/components/simulators/emulator/__init__.py` & `android-env-1.2.1/android_env/components/simulators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/components/simulators/emulator/emulator_launcher.py` & `android-env-1.2.1/android_env/components/simulators/emulator/emulator_simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,225 +1,305 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Prepares and launches the emulator."""
+"""A class that manages an Android Emulator."""
 
 import os
-import subprocess
 import time
-from typing import Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 from absl import logging
+from android_env.components import adb_controller
+from android_env.components import adb_log_stream
 from android_env.components import errors
+from android_env.components import log_stream
+from android_env.components.simulators import base_simulator
+from android_env.components.simulators.emulator import emulator_launcher
 import grpc
+import numpy as np
+import portpicker
 
 from android_env.proto import emulator_controller_pb2
 from android_env.proto import emulator_controller_pb2_grpc
 from google.protobuf import empty_pb2
 
-# Period in milliseconds to ping the Emulator gRPC server to keep the connection
-# alive. If too frequent, we may get errors such as "Too many pings.", which can
-# bring down the process.
-_GRPC_KEEPALIVE_MS = 100000
 
-
-class EmulatorLauncher():
-  """Handles launching the emulator."""
-
-  def __init__(
-      self,
-      local_tmp_dir: str = '/tmp',
-      adb_port: Optional[int] = None,
-      adb_server_port: Optional[int] = None,
-      emulator_console_port: Optional[int] = None,
-      grpc_port: int = -1,
-      emulator_path: str = '',
-      android_sdk_root: str = '',
-      avd_name: str = '',
-      run_headless: bool = False,
-      kvm_device: str = '/dev/kvm',
-      gpu_mode: str = 'swiftshader_indirect',
-      android_avd_home: str = '',
-      startup_wait_time_sec: int = 300,
-  ):
-    """Installs required files locally and launches the emulator.
+def is_existing_emulator_provided(launcher_args: Dict[str, Any]) -> bool:
+  """Returns true if all necessary args were provided."""
+  return bool(launcher_args.get('adb_port') and
+              launcher_args.get('emulator_console_port') and
+              launcher_args.get('grpc_port'))
+
+
+def _reconnect_on_grpc_error(func):
+  """Decorator function for reconnecting to emulator upon grpc errors."""
+  def wrapper(*args, **kwargs):
+    try:
+      return func(*args, **kwargs)
+    except grpc.RpcError:
+      logging.exception('RpcError caught. Reconnecting to emulator...')
+      emu = args[0]  # The first arg of the function is "self"
+      emu._emulator_stub = emu._connect_to_emulator(emu._grpc_port)  # pylint: disable=protected-access
+      return func(*args, **kwargs)
+  return wrapper
+
+
+class EmulatorBootError(errors.SimulatorError):
+  """Raised when an emulator failed to boot."""
+
+
+class EmulatorCrashError(errors.SimulatorError):
+  """Raised when a simulator crashed."""
+
+
+class EmulatorSimulator(base_simulator.BaseSimulator):
+  """Controls an Android Emulator."""
+
+  def __init__(self,
+               emulator_launcher_args: Dict[str, Any],
+               adb_controller_args: Dict[str, Any],
+               tmp_dir: str = '/tmp/android_env/simulator',
+               logfile_path: Optional[str] = None,
+               **kwargs):
+    """Instantiates an EmulatorSimulator.
 
     Args:
-      local_tmp_dir: Local directory for logs and maybe installing the AVD.
-      adb_port: ADB port for the Android device.
-      adb_server_port: Port of the ADB server deamon.
-      emulator_console_port: Port for telnet communication with the emulator.
-      grpc_port: Port for gRPC communication with the emulator.
-      emulator_path: Path to the emulator binary.
-      android_sdk_root: Root directory of the Android SDK.
-      avd_name: Name of the AVD.
-      run_headless: Whether to run in headless mode.
-      kvm_device: Path to the KVM device.
-      gpu_mode: GPU mode override. Supported values are listed at:
-        https://developer.android.com/studio/run/emulator-acceleration#accel-graphics
-      android_avd_home: Local directory for AVDs.
-      startup_wait_time_sec: Timeout for booting the emulator.
+      emulator_launcher_args: Arguments for EmulatorLauncher.
+      adb_controller_args: Arguments for AdbController.
+      tmp_dir: Temporary directory to hold simulator files.
+      logfile_path: Path to file which holds emulator logs. If not provided,
+        it will be determined by the EmulatorLauncher.
+      **kwargs: keyword arguments for base class.
     """
-    self._local_tmp_dir = local_tmp_dir
-    self._adb_port = adb_port
-    self._adb_server_port = adb_server_port
-    self._emulator_console_port = emulator_console_port
-    self._emulator_path = emulator_path
-    self._android_sdk_root = android_sdk_root
-    self._avd_name = avd_name
-    self._run_headless = run_headless
-    self._kvm_device = kvm_device
-    self._gpu_mode = gpu_mode
-    self._android_avd_home = android_avd_home
-    self._startup_wait_time_sec = startup_wait_time_sec
-    self._grpc_port = grpc_port
 
-    self._emulator = None
-    self._emulator_output = None
+    # If adb_port, console_port and grpc_port are all already provided,
+    # we assume the emulator already exists and there's no need to launch.
+    if is_existing_emulator_provided(emulator_launcher_args):
+      self._existing_emulator_provided = True
+      self._adb_port = emulator_launcher_args['adb_port']
+      self._console_port = emulator_launcher_args['emulator_console_port']
+      self._grpc_port = emulator_launcher_args['grpc_port']
+      logging.info('Connecting to existing emulator "%r"', self._adb_port)
+    else:
+      self._existing_emulator_provided = False
+      self._adb_port = portpicker.pick_unused_port()
+      self._console_port = portpicker.pick_unused_port()
+      self._grpc_port = portpicker.pick_unused_port()
+
+    self._channel = None
     self._emulator_stub = None
-    self._is_closed = False
+    # Set the image format to RGBA. The width and height of the returned
+    # screenshots will use the device's width and height.
+    self._image_format = emulator_controller_pb2.ImageFormat(
+        format=emulator_controller_pb2.ImageFormat.ImgFormat.RGBA8888)
+
+    super().__init__(**kwargs)
+
+    # Initialize own ADB controller.
+    self._adb_controller_args = adb_controller_args
+    self._adb_controller = self.create_adb_controller()
+    self._adb_controller.init_server()
+    logging.info('Initialized simulator with ADB server port %r.',
+                 self._adb_controller_args['adb_server_port'])
+
+    # If necessary, create EmulatorLauncher.
+    if self._existing_emulator_provided:
+      self._logfile_path = logfile_path or None
+      self._launcher = None
+    else:
+      emulator_launcher_args.update({
+          'adb_port': self._adb_port,
+          'adb_server_port': self._adb_controller_args['adb_server_port'],
+          'emulator_console_port': self._console_port,
+          'grpc_port': self._grpc_port,
+          'tmp_dir': tmp_dir,
+      })
+      logging.info('emulator_launcher_args: %r', emulator_launcher_args)
+      self._launcher = emulator_launcher.EmulatorLauncher(
+          **emulator_launcher_args)
+      self._logfile_path = logfile_path or self._launcher.logfile_path()
+
+  def get_logs(self) -> str:
+    """Returns logs recorded by the emulator."""
+    if self._logfile_path and os.path.exists(self._logfile_path):
+      with open(self._logfile_path, 'rb') as f:
+        return f.read().decode('utf-8')
+    else:
+      return f'Logfile does not exist: {self._logfile_path}.'
+
+  def adb_device_name(self) -> str:
+    return 'emulator-%s' % (self._adb_port - 1)
 
-  def launch(self) -> None:
-    """Launches the emulator."""
+  def create_adb_controller(self):
+    """Returns an ADB controller which can communicate with this simulator."""
+    return adb_controller.AdbController(
+        device_name=self.adb_device_name(),
+        **self._adb_controller_args)
+
+  def create_log_stream(self) -> log_stream.LogStream:
+    return adb_log_stream.AdbLogStream(
+        adb_command_prefix=self._adb_controller.command_prefix(),
+        verbose=self._verbose_logs)
+
+  def _restart_impl(self) -> None:
+    if self._launcher is not None:
+      logging.info('Restarting the emulator...')
+      self._shutdown_emulator()
+      self._launcher.launch_emulator_process()
+      self._emulator_stub = self._connect_to_emulator(self._grpc_port)
+      self._confirm_booted()
+      logging.info('Done restarting the emulator.')
+
+  def _launch_impl(self) -> None:
+    """Establishes a grpc connection to an emulator process."""
+
+    # If required, launch an emulator process.
+    if self._launcher is not None:
+      self._launcher.launch_emulator_process()
+
+    # Establish grpc connection to emulator process.
+    self._emulator_stub = self._connect_to_emulator(self._grpc_port)
+
+    # Confirm booted status.
+    try:
+      self._confirm_booted()
+    except EmulatorCrashError:
+      logging.exception(
+          'Failed to confirm booted status of emulator. Restarting...')
+      self.restart()
+
+  def _connect_to_emulator(
+      self,
+      grpc_port: int,
+      timeout_sec: int = 30,
+  ) -> emulator_controller_pb2_grpc.EmulatorControllerStub:
+    """Connects to an emulator and returns a corresponsing stub."""
+
+    logging.info('Creating gRPC channel to the emulator on port %r', grpc_port)
+    port = f'localhost:{grpc_port}'
+    options = [('grpc.max_send_message_length', -1),
+               ('grpc.max_receive_message_length', -1)]
+    creds = grpc.local_channel_credentials()
 
-    logging.info('Booting the emulator [%s]', self._emulator_path)
+    try:
+      self._channel = grpc.secure_channel(port, creds, options=options)
+      grpc.channel_ready_future(self._channel).result(timeout=timeout_sec)
+    except (grpc.RpcError, grpc.FutureTimeoutError) as grpc_error:
+      logging.exception('Failed to connect to the emulator.')
+      raise EmulatorBootError(
+          'Failed to connect to the emulator.') from grpc_error
 
-    # Set necessary environment variables.
-    base_lib_dir = self._emulator_path[:-8] + 'lib64/'
-    ld_library_path = ':'.join([
-        base_lib_dir + 'x11/',
-        base_lib_dir + 'qt/lib/',
-        base_lib_dir + 'gles_swiftshader/',
-        base_lib_dir
-    ])
-    extra_env_vars = {
-        'ANDROID_HOME': '',
-        'ANDROID_SDK_ROOT': self._android_sdk_root,
-        'ANDROID_AVD_HOME': self._android_avd_home,
-        'ANDROID_EMULATOR_KVM_DEVICE': self._kvm_device,
-        'ANDROID_ADB_SERVER_PORT': str(self._adb_server_port),
-        'LD_LIBRARY_PATH': ld_library_path,
-        'QT_DEBUG_PLUGINS': '1',
-        'QT_XKB_CONFIG_ROOT': str(self._emulator_path[:-8] + 'qt_config/'),
-    }
-    logging.info('extra_env_vars: %s', str(extra_env_vars))
-    env_vars = dict(os.environ).copy()
-    env_vars.update(extra_env_vars)
-
-    # Compile command.
-    grpc_port = ['-grpc', str(self._grpc_port)] if self._grpc_port >= 0 else []
-    run_headless = ['-no-skin', '-no-window'] if self._run_headless else []
-    ports = ['-ports', '%s,%s' % (self._emulator_console_port, self._adb_port)]
-    command = [
-        self._emulator_path,
-        '-no-snapshot',
-        '-gpu', self._gpu_mode,
-        '-no-audio',
-        '-verbose',
-        '-avd', self._avd_name,
-    ] + grpc_port + run_headless + ports
-    logging.info('Emulator launch command: %s', ' '.join(command))
-
-    # Prepare logfile.
-    emulator_logfile = os.path.join(self._local_tmp_dir, 'emulator_output')
-    self._emulator_output = open(emulator_logfile, 'wb')
-
-    # Spawn the emulator process.
-    self._emulator = subprocess.Popen(
-        command,
-        env=env_vars,
-        stdout=self._emulator_output,
-        stderr=self._emulator_output)
+    logging.info('Added gRPC channel for the Emulator on port %s', port)
+    return emulator_controller_pb2_grpc.EmulatorControllerStub(self._channel)
 
-    self._emulator_stub = EmulatorLauncher.create_emulator_stub(self._grpc_port)
+  @_reconnect_on_grpc_error
+  def _confirm_booted(self, startup_wait_time_sec: int = 300):
+    """Waits until the emulator is fully booted."""
 
-    # Wait for the emulator to boot.
     start_time = time.time()
-    deadline = start_time + self._startup_wait_time_sec
+    deadline = start_time + startup_wait_time_sec
     success = False
     while time.time() < deadline:
       emu_status = self._emulator_stub.getStatus(empty_pb2.Empty())
-      logging.info('Waiting for emulator to start. Emulator uptime: %rms',
-                   emu_status.uptime)
+      logging.info('Waiting for emulator to start... (%rms)', emu_status.uptime)
       if emu_status.booted:
         success = True
         break
-      time.sleep(1.0)
+      time.sleep(5.0)
 
     elapsed_time = time.time() - start_time
     if not success:
-      raise errors.SimulatorCrashError(
-          'The emulator failed to boot after %r seconds' %
-          self._startup_wait_time_sec)
+      raise EmulatorCrashError(
+          f'The emulator failed to boot after {startup_wait_time_sec} seconds')
 
     logging.info('Done booting the emulator (in %f seconds).', elapsed_time)
+    logging.info('********** Emulator logs (last 20 lines) **********')
+    for line in self.get_logs().splitlines()[-20:]:
+      logging.info(line)
+    logging.info('******* End of emulator logs *******')
+    logging.info('See the full emulator logs at %r', self._logfile_path)
+
+  @_reconnect_on_grpc_error
+  def send_touch(self, touches: List[Tuple[int, int, bool, int]]) -> None:
+    """Sends a touch event to be executed on the simulator.
 
-  def restart(self) -> None:
-    logging.info('Restarting the emulator...')
-    self._kill_emulator_process()
-    self.launch()
-    logging.info('Done restarting the emulator.')
-
-  @classmethod
-  def create_emulator_stub(
-      cls,
-      grpc_port: int,
-      use_async: bool = False,
-  ) -> emulator_controller_pb2_grpc.EmulatorControllerStub:
-    """Returns a stub to the EmulatorController service."""
-    logging.info('Creating gRPC channel to the emulator on port %r', grpc_port)
-    port = f'localhost:{grpc_port}'
-    options = [('grpc.max_send_message_length', -1),
-               ('grpc.max_receive_message_length', -1),
-               ('grpc.keepalive_time_ms', _GRPC_KEEPALIVE_MS)]
-    creds = grpc.local_channel_credentials()
-    if use_async:
-      channel = grpc.aio.secure_channel(port, creds, options=options)
-    else:
-      channel = grpc.secure_channel(port, creds, options=options)
-    grpc.channel_ready_future(channel).result()  # Wait for channel to be ready.
-    logging.info('Added gRPC channel for the Emulator on port %s', port)
-    return emulator_controller_pb2_grpc.EmulatorControllerStub(channel)
+    Args:
+      touches: A list of touch events. Each elemet in the list corresponds to a
+          single touch event. Each touch event tuple should have:
+          0 x: The horizontal coordinate of this event.
+          1 y: The vertical coordinate of this event.
+          2 is_down: Whether the finger is touching or not the screen.
+          3 identifier: Identifies a particular finger in a multitouch event.
+    """
 
-  def get_emulator_stub(
-      self) -> emulator_controller_pb2_grpc.EmulatorControllerStub:
-    """Returns the EmulatorController stub for the launched emulator."""
-    return self._emulator_stub
-
-  def _kill_emulator_process(self) -> None:
-    if self._emulator:
-      logging.info('Killing the emulator process...')
-      self._emulator_stub.setVmState(
-          emulator_controller_pb2.VmRunState(
-              state=emulator_controller_pb2.VmRunState.RunState.SHUTDOWN))
-      logging.info('Will wait 30s for it to finish gracefully...')
-      try:
-        self._emulator.wait(timeout=30.0)
-      except subprocess.TimeoutExpired:
-        logging.exception('The emulator process did not finish after 30s. '
-                          f'returncode: {self._emulator.returncode}. '
-                          'Will now try to kill() it.')
-        self._emulator.kill()
-      self._emulator = None
-      self._emulator_output.close()
-      logging.info('Done killing the emulator process.')
+    assert self._emulator_stub, 'Emulator stub has not been initialized yet.'
+    touch_events = [
+        emulator_controller_pb2.Touch(
+            x=t[0], y=t[1], pressure=int(t[2]), identifier=t[3])
+        for t in touches
+    ]
+    self._emulator_stub.sendTouch(
+        emulator_controller_pb2.TouchEvent(touches=touch_events))
+
+  @_reconnect_on_grpc_error
+  def send_key(self, keycode: np.int32, event_type: str) -> None:
+    """Sends a key event to the emulator.
 
-  def close(self):
-    """Clean up launcher files and processes."""
-    if not self._is_closed:
-      self._kill_emulator_process()
-      self._is_closed = True
+    Args:
+      keycode: Code representing the desired key press in XKB format.
+        See the emulator_controller_pb2 for details.
+      event_type: Type of key event to be sent.
+    """
+    event_types = emulator_controller_pb2.KeyboardEvent.KeyEventType.keys()
+    if event_type not in event_types:
+      raise ValueError(
+          f'Event type must be one of {event_types} but is {event_type}.')
+
+    self._emulator_stub.sendKey(
+        emulator_controller_pb2.KeyboardEvent(
+            codeType=emulator_controller_pb2.KeyboardEvent.KeyCodeType.XKB,
+            eventType=emulator_controller_pb2.KeyboardEvent
+            .KeyEventType.Value(event_type),
+            keyCode=np.int32(keycode),
+        ))
+
+  @_reconnect_on_grpc_error
+  def get_screenshot(self) -> np.ndarray:
+    """Fetches the latest screenshot from the emulator."""
+    assert self._emulator_stub, 'Emulator stub has not been initialized yet.'
+    assert self._image_format, 'ImageFormat has not been initialized yet.'
+    image_proto = self._emulator_stub.getScreenshot(self._image_format)
+    h, w = image_proto.format.height, image_proto.format.width
+    image = np.frombuffer(image_proto.image, dtype='uint8', count=h * w * 4)
+    image.shape = (h, w, 4)
+    return image[:, :, :3]
+
+  @_reconnect_on_grpc_error
+  def _shutdown_emulator(self):
+    """Sends a signal to trigger emulator shutdown."""
+    logging.info('Shutting down the emulator...')
+    self._emulator_stub.setVmState(
+        emulator_controller_pb2.VmRunState(
+            state=emulator_controller_pb2.VmRunState.RunState.SHUTDOWN))
+    self._launcher.confirm_shutdown()
 
-  def __del__(self):
-    self.close()
+  def close(self):
+    if self._launcher is not None:
+      self._shutdown_emulator()
+      self._launcher.close()
+    if hasattr(self, '_emulator_stub'):
+      del self._emulator_stub
+    if self._channel is not None:
+      self._channel.close()
+    super().close()
```

### Comparing `android_env-1.1.0/android_env/components/simulators/emulator/emulator_simulator.py` & `android-env-1.2.1/android_env/components/simulators/emulator/emulator_launcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,179 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A class that manages an Android Emulator."""
+"""Prepares and launches an emulator process."""
 
-import functools
+import os
+import subprocess
 import tempfile
-from typing import Any, Dict, List, Optional
+from typing import Optional
 
 from absl import logging
-from android_env.components import adb_controller
-from android_env.components import adb_log_stream
-from android_env.components import errors
-from android_env.components import log_stream
-from android_env.components.simulators import base_simulator
-from android_env.components.simulators.emulator import emulator_launcher
-import numpy as np
-import portpicker
-
-from android_env.proto import emulator_controller_pb2
-
-
-def is_existing_emulator_provided(launcher_args: Dict[str, Any]) -> bool:
-  """Returns true if all necessary args were provided."""
-  return bool(launcher_args.get('adb_port') and
-              launcher_args.get('emulator_console_port') and
-              launcher_args.get('grpc_port'))
-
-
-class EmulatorSimulator(base_simulator.BaseSimulator):
-  """Controls an Android Emulator."""
-
-  def __init__(self,
-               emulator_launcher_args: Dict[str, Any],
-               adb_controller_args: Dict[str, Any],
-               tmp_dir: Optional[str] = None,
-               **kwargs):
-
-    # If adb_port, console_port and grpc_port are all already provided,
-    # we assume the emulator already exists and there's no need to launch.
-    if is_existing_emulator_provided(emulator_launcher_args):
-      self._existing_emulator_provided = True
-      self._adb_port = emulator_launcher_args['adb_port']
-      self._console_port = emulator_launcher_args['emulator_console_port']
-      self._grpc_port = emulator_launcher_args['grpc_port']
-      logging.info('Connecting to existing emulator "%r"', self._adb_port)
-    else:
-      self._existing_emulator_provided = False
-      self._adb_port = portpicker.pick_unused_port()
-      self._console_port = portpicker.pick_unused_port()
-      self._grpc_port = portpicker.pick_unused_port()
 
-    self._emulator_stub = None
-    self._image_format = None
 
-    super().__init__(**kwargs)
+class EmulatorLauncher():
+  """Handles launching an emulator."""
+
+  def __init__(
+      self,
+      adb_port: Optional[int] = None,
+      adb_server_port: Optional[int] = None,
+      emulator_console_port: Optional[int] = None,
+      grpc_port: int = -1,
+      emulator_path: str = '',
+      android_sdk_root: str = '',
+      avd_name: str = '',
+      android_avd_home: str = '',
+      run_headless: bool = False,
+      kvm_device: str = '/dev/kvm',
+      gpu_mode: str = 'swiftshader_indirect',
+      tmp_dir: str = '',
+      snapshot_name: str = '',
+      restrict_network: bool = False):
+    """Launches an emulator.
+
+    Args:
+      adb_port: ADB port for the Android device.
+      adb_server_port: Port of the ADB server deamon.
+      emulator_console_port: Port for telnet communication with the emulator.
+      grpc_port: Port for gRPC communication with the emulator.
+      emulator_path: Path to the emulator binary.
+      android_sdk_root: Root directory of the Android SDK.
+      avd_name: Name of the AVD.
+      android_avd_home: Local directory for AVDs.
+      run_headless: Whether to run in headless mode.
+      kvm_device: Path to the KVM device.
+      gpu_mode: GPU mode override. Supported values are listed at:
+        https://developer.android.com/studio/run/emulator-acceleration#accel-graphics
+      tmp_dir: Path to directory which will hold temporary files.
+      snapshot_name: Name of the snapshot to load.
+      restrict_network: if True, will disable networking on the device. This
+        option is only available for emulator version > 31.3.9 (June 2022).
+    """
+    self._adb_port = adb_port
+    self._adb_server_port = adb_server_port
+    self._emulator_console_port = emulator_console_port
+    self._grpc_port = grpc_port
+    self._emulator_path = emulator_path
+    self._android_sdk_root = android_sdk_root
+    self._avd_name = avd_name
+    self._android_avd_home = android_avd_home
+    self._run_headless = run_headless
+    self._kvm_device = kvm_device
+    self._gpu_mode = gpu_mode
+    self._snapshot_name = snapshot_name
+    self._restrict_network = restrict_network
+
+    self._emulator = None
+    self._emulator_output = None
+    self._is_closed = False
 
     # Create directory for tmp files.
-    self._tmp_dir = tmp_dir or tempfile.gettempdir()
-    self._local_tmp_dir_handle = tempfile.TemporaryDirectory(dir=self._tmp_dir)
+    # Note: this will be deleted once EmulatorLauncher instance is cleaned up.
+    os.makedirs(tmp_dir, exist_ok=True)
+    self._local_tmp_dir_handle = tempfile.TemporaryDirectory(
+        dir=tmp_dir, prefix='simulator_instance_')
     self._local_tmp_dir = self._local_tmp_dir_handle.name
+    self._logfile_path = os.path.join(self._local_tmp_dir, 'emulator_output')
     logging.info('Simulator local_tmp_dir: %s', self._local_tmp_dir)
 
-    # Initialize own ADB controller
-    self._adb_controller_args = adb_controller_args
-    self._adb_controller = self.create_adb_controller()
-    self._adb_controller.init_server()
-    logging.info('Initialized simulator with ADB server port %r.',
-                 self._adb_controller_args['adb_server_port'])
-
-    # Create EmulatorLauncher.
-    emulator_launcher_args.update({
-        'adb_port': self._adb_port,
-        'adb_server_port': self._adb_controller_args['adb_server_port'],
-        'emulator_console_port': self._console_port,
-        'local_tmp_dir': self._local_tmp_dir,
-        'grpc_port': self._grpc_port,
-    })
-    logging.info('emulator_launcher_args: %r', emulator_launcher_args)
-    if not self._existing_emulator_provided:
-      self._launcher = emulator_launcher.EmulatorLauncher(
-          **emulator_launcher_args)
-      self._get_emulator_stub = self._launcher.get_emulator_stub
-    else:
-      self._get_emulator_stub = functools.partial(
-          emulator_launcher.EmulatorLauncher.create_emulator_stub,
-          grpc_port=self._grpc_port)
-
-  def adb_device_name(self) -> str:
-    return 'emulator-%s' % (self._adb_port - 1)
-
-  def create_adb_controller(self):
-    """Returns an ADB controller which can communicate with this simulator."""
-    return adb_controller.AdbController(
-        device_name=self.adb_device_name(),
-        **self._adb_controller_args)
-
-  def _restart_impl(self) -> None:
-    if not self._existing_emulator_provided:
-      self._launcher.restart()
-
-  def _launch_impl(self) -> None:
-    try:
-      if not self._existing_emulator_provided:
-        self._launcher.launch()
-    except errors.SimulatorCrashError:
-      # If the simulator crashes on the initial launch, we try to restart once.
-      self.restart()
-
-  def _post_launch_setup(self):
-    super()._post_launch_setup()
-    self._emulator_stub = self._get_emulator_stub()
-    self._image_format = emulator_controller_pb2.ImageFormat(
-        format=emulator_controller_pb2.ImageFormat.ImgFormat.RGB888,
-        height=self._screen_dimensions[0],
-        width=self._screen_dimensions[1],
-    )
-
-  def send_action(self, action: Dict[str, np.ndarray]) -> None:
-    """Sends touch events to the emulator."""
-    assert self._emulator_stub, 'Emulator stub has not been initialized yet.'
-    touches = []
-    for i, finger_action in enumerate(self._split_action(action)):
-      x, y, down = self._prepare_action(finger_action)
-      touches.append(emulator_controller_pb2.Touch(
-          x=x, y=y, pressure=int(down), identifier=i))
-    self._emulator_stub.sendTouch(
-        emulator_controller_pb2.TouchEvent(touches=touches))
-
-  def _get_observation(self) -> Optional[List[np.ndarray]]:
-    """Fetches the latest observation from the emulator."""
-    assert self._emulator_stub, 'Emulator stub has not been initialized yet.'
-    assert self._image_format, 'ImageFormat has not been initialized yet.'
-    image_proto = self._emulator_stub.getScreenshot(self._image_format)
-    h, w = image_proto.format.height, image_proto.format.width
-    image = np.frombuffer(image_proto.image, dtype='uint8', count=h * w * 3)
-    image.shape = (h, w, 3)
-    return [image, np.int64(image_proto.timestampUs)]
-
-  def _create_log_stream(self) -> log_stream.LogStream:
-    return adb_log_stream.AdbLogStream(
-        adb_command_prefix=self._adb_controller.command_prefix(),
-        verbose=self._verbose_logs)
+  def logfile_path(self) -> str:
+    return self._logfile_path
+
+  def launch_emulator_process(self) -> None:
+    """Launches the emulator."""
+
+    logging.info('Booting new emulator [%s]', self._emulator_path)
+
+    # Set necessary environment variables.
+    base_lib_dir = self._emulator_path[:-8] + 'lib64/'
+    ld_library_path = ':'.join([
+        base_lib_dir + 'x11/', base_lib_dir + 'qt/lib/',
+        base_lib_dir + 'gles_swiftshader/', base_lib_dir
+    ])
+    extra_env_vars = {
+        'ANDROID_HOME': '',
+        'ANDROID_SDK_ROOT': self._android_sdk_root,
+        'ANDROID_AVD_HOME': self._android_avd_home,
+        'ANDROID_EMULATOR_KVM_DEVICE': self._kvm_device,
+        'ANDROID_ADB_SERVER_PORT': str(self._adb_server_port),
+        'LD_LIBRARY_PATH': ld_library_path,
+        'QT_XKB_CONFIG_ROOT': str(self._emulator_path[:-8] + 'qt_config/'),
+    }
+    logging.info('extra_env_vars: %s',
+                 ' '.join(f'{k}={v}' for k, v in extra_env_vars.items()))
+    env_vars = dict(os.environ).copy()
+    env_vars.update(extra_env_vars)
+
+    # Compile command.
+    grpc_port = ['-grpc', str(self._grpc_port)] if self._grpc_port >= 0 else []
+    run_headless = ['-no-skin', '-no-window'] if self._run_headless else []
+    ports = ['-ports', '%s,%s' % (self._emulator_console_port, self._adb_port)]
+    snapshot = [
+        '-snapshot', self._snapshot_name, '-feature',
+        'AllowSnapshotMigration,MigratableSnapshotSave'
+    ]
+    snapshot = snapshot if self._snapshot_name else ['-no-snapshot']
+    restrict_network_args = [
+        '-network-user-mode-options', 'restrict=y', '-wifi-user-mode-options',
+        'restrict=y'
+    ]
+    network_args = restrict_network_args if self._restrict_network else []
+    command = [
+        self._emulator_path,
+        '-gpu',
+        self._gpu_mode,
+        '-no-audio',
+        '-show-kernel',
+        '-verbose',
+        '-avd',
+        self._avd_name,
+    ] + grpc_port + run_headless + ports + snapshot + network_args
+    logging.info('Emulator launch command: %s', ' '.join(command))
+
+    # Prepare logfile.
+    self._emulator_output = open(self._logfile_path, 'wb')
+
+    # Spawn the emulator process.
+    self._emulator = subprocess.Popen(
+        command,
+        env=env_vars,
+        stdout=self._emulator_output,
+        stderr=self._emulator_output)
+
+  def confirm_shutdown(self) -> None:
+    """Shuts down the emulator process."""
+    if self._emulator is not None:
+      logging.info('Checking if emulator process has finished...')
+      try:
+        self._emulator.wait(timeout=30.0)
+      except subprocess.TimeoutExpired:
+        logging.exception(
+            'The emulator process did not finish after 30s. '
+            'returncode: %s. Will now try to kill() it.',
+            self._emulator.returncode)
+        self._emulator.kill()
+      self._emulator = None
+      self._emulator_output.close()
+      logging.info('The emulator process has finished.')
 
   def close(self):
-    if hasattr(self, '_channel'):
-      self._channel.close()
-    if hasattr(self, '_emulator_stub'):
-      del self._emulator_stub
-    if hasattr(self, '_launcher') and not self._existing_emulator_provided:
-      self._launcher.close()
-    super().close()
+    """Clean up launcher files and processes."""
+    if not self._is_closed:
+      self.confirm_shutdown()
+      self._is_closed = True
+
+  def __del__(self):
+    self.close()
```

### Comparing `android_env-1.1.0/android_env/components/simulators/fake/__init__.py` & `android-env-1.2.1/android_env/components/simulators/emulator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/components/simulators/fake/fake_simulator.py` & `android-env-1.2.1/android_env/components/simulators/fake/fake_simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # limitations under the License.
 
 """Fake Simulator for testing AndroidEnv infrastructure."""
 
 import random
 import threading
 import time
-from typing import Dict, List, Optional, Tuple
+from typing import List, Optional, Tuple
 
 from absl import logging
 from android_env.components import adb_controller
 from android_env.components import log_stream
 from android_env.components.simulators import base_simulator
 import numpy as np
 
@@ -31,15 +31,15 @@
   """This class simulates the logs coming from ADB."""
 
   def __init__(self):
     self._values = [
         '',
         self._make_stdout('reward: 0.5'),
         self._make_stdout('reward: 1.0'),
-        self._make_stdout('extra: my_extra: [1.0]'),
+        self._make_stdout('extra: my_extra [1.0]'),
         self._make_stdout('episode end'),
     ]
     self._kill = False
     self._lock = threading.Lock()
 
   def _make_stdout(self, data):
     """Returns a valid log output with given data as message."""
@@ -60,109 +60,87 @@
         yield next_value
 
 
 class FakeLogStream(log_stream.LogStream):
   """FakeLogStream class that wraps a FakeStream."""
 
   def __init__(self):
+    super().__init__(verbose=False)
     self.stream = FakeStream()
-    self.stream_is_alive = True
-    self._verbose = False
 
   def _get_stream_output(self):
     return self.stream
 
   def stop_stream(self):
-    self.stream_is_alive = False
     self.stream.kill()
 
 
 class FakeAdbController(adb_controller.AdbController):
   """Fake adb controller for FakeSimulator."""
 
-  def __init__(self,
-               screen_dimensions: Tuple[int, int],
-               fake_activity: str,
-               *args, **kwargs):
-    super().__init__(*args, **kwargs)
-    self._screen_dimensions = screen_dimensions
-    self._fake_activity = fake_activity
-
-  def _execute_command(
-      self,
-      args: List[str],
-      timeout: Optional[float] = None) -> Optional[bytes]:
-    del args, timeout
-    return bytes('fake output', 'utf-8')
-
-  def _wait_for_device(
-      self,
-      max_tries: int = 20,
-      sleep_time: float = 1.0,
-      timeout: Optional[float] = None) -> None:
-    """Fake adb controller does not have to wait for a device."""
-    pass
+  def execute_command(self,
+                      args: List[str],
+                      timeout: Optional[float] = None) -> bytes:
+    """Returns fake output for adb commands."""
+
+    del timeout
+
+    # Fake "service is ready" output.
+    if args[:3] == ['shell', 'service', 'check']:
+      return f'Service {args[-1]}: found'.encode('utf-8')
+
+    # Fake dumpsys output for getting orientation.
+    if args == ['shell', 'dumpsys', 'input']:
+      return b' SurfaceOrientation: 0'
+
+    # app_screen_checker: fake_task expects 'fake_activity'.
+    if args[:4] == ['shell', 'am', 'stack', 'list']:
+      return (b'taskId=0 fake_activity visible=true '
+              b'topActivity=ComponentInfo{fake_activity}')
 
-  def get_screen_dimensions(
-      self, timeout: Optional[float] = None) -> Tuple[int, int]:
-    return self._screen_dimensions
-
-  def get_current_activity(
-      self, timeout: Optional[float] = None) -> Optional[str]:
-    return self._fake_activity
-
-  def is_package_installed(
-      self, package_name: str, timeout: Optional[float] = None) -> bool:
-    return True
-
-  def start_screen_pinning(
-      self, full_activity: str, timeout: Optional[float] = None):
-    pass
+    return b'fake output'
 
 
 class FakeSimulator(base_simulator.BaseSimulator):
   """FakeSimulator class."""
 
   def __init__(self,
                screen_dimensions: Tuple[int, int] = (480, 320),
-               fake_activity: str = '',
                **kwargs):
     """FakeSimulator class that can replace EmulatorSimulator in AndroidEnv.
 
     Args:
-      screen_dimensions: desired screen dimensions in pixels.
-      fake_activity: if FakeSimulator is used in combination with a
-        task_pb2.Task() that has an expected_activity, we can mock an
-        activity here. If this activity does not match the expected_activity,
-        an error will be raised.
+      screen_dimensions: desired screen dimensions in pixels. This determines
+        the shape of the screenshots returned by get_screenshot().
       **kwargs: other keyword arguments for the base class.
     """
     super().__init__(**kwargs)
-    self._screen_dimensions = screen_dimensions
-    self._fake_activity = fake_activity
-    self._adb_controller = self.create_adb_controller()
+    self._screen_dimensions = np.array(screen_dimensions)
     logging.info('Created FakeSimulator.')
 
+  def get_logs(self) -> str:
+    return 'FakeSimulator: fake logs'
+
   def adb_device_name(self) -> str:
     return 'fake_simulator'
 
   def create_adb_controller(self):
-    return FakeAdbController(
-        screen_dimensions=self._screen_dimensions,
-        fake_activity=self._fake_activity)
+    return FakeAdbController()
+
+  def create_log_stream(self) -> log_stream.LogStream:
+    return FakeLogStream()
 
   def _restart_impl(self) -> None:
     pass
 
   def _launch_impl(self) -> None:
     pass
 
-  def send_action(self, action: Dict[str, np.ndarray]) -> None:
-    del action
+  def send_touch(self, touches: List[Tuple[int, int, bool, int]]) -> None:
+    del touches
 
-  def _get_observation(self) -> Optional[List[np.ndarray]]:
-    image = np.zeros(shape=(*self._screen_dimensions, 3), dtype=np.uint8)
-    timestamp = np.random.randint(100, dtype=np.int64)
-    return [image, timestamp]
+  def send_key(self, keycode: np.int32, event_type: str) -> None:
+    del keycode, event_type
 
-  def _create_log_stream(self) -> log_stream.LogStream:
-    return FakeLogStream()
+  def get_screenshot(self) -> np.ndarray:
+    return np.random.randint(
+        low=0, high=255, size=(*self._screen_dimensions, 3), dtype=np.uint8)
```

### Comparing `android_env-1.1.0/android_env/components/simulators/fake/fake_simulator_test.py` & `android-env-1.2.1/android_env/components/simulators/fake/fake_simulator_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for fake_simulator."""
 
+import re
 from absl.testing import absltest
 from android_env.components.simulators.fake import fake_simulator
 import numpy as np
 
 
 class FakeSimulatorTest(absltest.TestCase):
 
@@ -26,44 +27,71 @@
     simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
     self.assertEqual(simulator.adb_device_name(), 'fake_simulator')
 
   def test_launch_close(self):
     # The simulator should launch and not crash.
     simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
     simulator.launch()
-    # After a successful launch(), screen_dimensions() should return something.
-    np.testing.assert_equal(simulator.screen_dimensions(), [320, 480])
     # Closing the simulator should also not crash.
     simulator.close()
 
-  def test_get_observation(self):
+  def test_get_screenshot(self):
     simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
     simulator.launch()
 
-    observation = simulator.get_observation()
-    np.testing.assert_equal(
-        observation['pixels'].shape, [320, 480, 3])
-    np.testing.assert_array_equal(
-        observation['pixels'], np.zeros((320, 480, 3), dtype=np.uint8))
-    np.testing.assert_equal(
-        observation['timedelta'].dtype, np.int64)
-    np.testing.assert_array_equal(
-        observation['orientation'], np.zeros((4,), dtype=np.uint8))
+    screenshot = simulator.get_screenshot()
+    np.testing.assert_equal(screenshot.shape, [320, 480, 3])
+    np.testing.assert_equal(screenshot.dtype, np.uint8)
 
   def test_log_stream(self):
     simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
     simulator.launch()
-    log_stream = simulator.get_log_stream()
+    log_stream = simulator.create_log_stream()
+    # Start yielding lines from LogStream.
+    log_stream.resume_stream()
     lines = [
         '',
         '         1553110400.424  5583  5658 D Tag: reward: 0.5',
         '         1553110400.424  5583  5658 D Tag: reward: 1.0',
-        '         1553110400.424  5583  5658 D Tag: extra: my_extra: [1.0]',
+        '         1553110400.424  5583  5658 D Tag: extra: my_extra [1.0]',
         '         1553110400.424  5583  5658 D Tag: episode end',
     ]
     for i, line in enumerate(log_stream.get_stream_output()):
       self.assertIn(line, lines)
       if i > 10:
         break
 
+  def test_adb_output(self):
+    simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
+    simulator.launch()
+    adb_controller = simulator.create_adb_controller()
+    line = adb_controller.execute_command(['shell', 'dumpsys', 'input'])
+    line = line.decode('utf-8')
+    orientation = re.match(r'\s+SurfaceOrientation:\s+(\d)', line).group(1)
+    self.assertEqual(orientation, '0')
+    line = adb_controller.execute_command(['shell', 'service', 'check', 'foo'])
+    line = line.decode('utf-8')
+    self.assertEqual(line, 'Service foo: found')
+    line = adb_controller.execute_command(['shell', 'am', 'stack', 'list'])
+    line = line.decode('utf-8')
+    self.assertEqual(line, 'taskId=0 fake_activity visible=true '
+                     'topActivity=ComponentInfo{fake_activity}')
+
+  def test_send_touch(self):
+    simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
+    simulator.launch()
+    simulator.send_touch([(0, 1, True, 0)])
+    simulator.send_touch([(0, 1, False, 0)])
+    # No assertions, we just want to ensure that `send_touch()` can be called
+    # without crashing anything.
+
+  def test_send_key(self):
+    simulator = fake_simulator.FakeSimulator(screen_dimensions=(320, 480))
+    simulator.launch()
+    simulator.send_key(123, 'keydown')
+    simulator.send_key(123, 'keyup')
+    simulator.send_key(123, 'keypress')
+    # No assertions, we just want to ensure that `send_key()` can be called
+    # without crashing anything.
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `android_env-1.1.0/android_env/components/specs.py` & `android-env-1.2.1/android_env/components/specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,37 +36,41 @@
     task_pb2.ArraySpec.DataType.UINT32: np.uint32,
     task_pb2.ArraySpec.DataType.UINT64: np.uint64,
     task_pb2.ArraySpec.DataType.BOOL: np.bool_,
     task_pb2.ArraySpec.DataType.STRING_U1: np.dtype(('U1')),
     task_pb2.ArraySpec.DataType.STRING_U16: np.dtype(('<U16')),
     task_pb2.ArraySpec.DataType.STRING_U25: np.dtype(('<U25')),
     task_pb2.ArraySpec.DataType.STRING_U250: np.dtype(('<U250')),
+    task_pb2.ArraySpec.DataType.STRING: np.dtype(('<U0')),
 }
 
 
-def base_action_spec(num_fingers: int = 1) -> Dict[str, specs.Array]:
+def base_action_spec(num_fingers: int = 1,
+                     enable_key_events: bool = False) -> Dict[str, specs.Array]:
   """Default action spec for AndroidEnv.
 
   Args:
     num_fingers: Number of virtual fingers of the agent.
+    enable_key_events: Whether keyboard key events are enabled.
+
   Returns:
     A dict of action specs, each item corresponding to a virtual finger.
     action_type: An integer of type ActionType: TOUCH=0, LIFT=1, REPEAT=2
     touch_position: Position [x, y] of the touch action, where x, y are float
       values between 0.0 and 1.0 corresponding to the relative position on the
       screen. IGNORED when (action_type != ActionType.TOUCH).
     action_type_i: Action type for additional fingers (i>1).
     touch_position_i: Touch position for additional fingers (i>1).
   """
 
+  num_actions = len(action_type.ActionType) if enable_key_events else 3
+
   action_spec = {
       'action_type':
-          specs.DiscreteArray(
-              num_values=len(action_type.ActionType),
-              name='action_type'),
+          specs.DiscreteArray(num_values=num_actions, name='action_type'),
       'touch_position':
           specs.BoundedArray(
               shape=(2,),
               dtype=np.float32,
               minimum=[0.0, 0.0],
               maximum=[1.0, 1.0],
               name='touch_position'),
@@ -83,26 +87,33 @@
                 shape=(2,),
                 dtype=np.float32,
                 minimum=[0.0, 0.0],
                 maximum=[1.0, 1.0],
                 name=f'touch_position_{i}'),
     })
 
+  if enable_key_events:
+    action_spec['keycode'] = specs.DiscreteArray(
+        num_values=(1 << 16) - 1, name='keycode')
+
   return action_spec
 
 
 def base_observation_spec(height: int, width: int) -> Dict[str, specs.Array]:
   """Default observation spec for AndroidEnv.
 
   Args:
     height: Height of the device screen in pixels.
     width: Width of the device screen in pixels.
+
   Returns:
     pixels: Spec for the RGB screenshot of the device. Has shape (H, W, 3)
     timedelta: Spec for time delta since the last observation (in microseconds).
+        The first timestep immediately after reset() will have this value set to
+        0.
     orientation: Spec for the latest orientation in a one-hot representation:
         [1, 0, 0, 0]: PORTRAIT  (0 degrees)
         [0, 1, 0, 0]: LANDSCAPE (90 degrees clockwise)
         [0, 0, 1, 0]: PORTRAIT  (180 degrees) ("upside down")
         [0, 0, 0, 1]: LANDSCAPE (270 degrees clockwise)
   """
```

### Comparing `android_env-1.1.0/android_env/components/specs_test.py` & `android-env-1.2.1/android_env/components/specs_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,14 +30,25 @@
     for spec in action_spec.values():
       self.assertIsInstance(spec, dm_env_specs.Array)
     self.assertEqual(action_spec['action_type'].shape, ())
     self.assertEqual(action_spec['action_type'].dtype, np.int32)
     self.assertEqual(action_spec['touch_position'].shape, (2,))
     self.assertEqual(action_spec['touch_position'].dtype, np.float32)
 
+  def test_base_action_spec_with_key_events(self):
+    action_spec = specs.base_action_spec(num_fingers=1, enable_key_events=True)
+    for spec in action_spec.values():
+      self.assertIsInstance(spec, dm_env_specs.Array)
+    self.assertEqual(action_spec['action_type'].shape, ())
+    self.assertEqual(action_spec['action_type'].dtype, np.int32)
+    self.assertEqual(action_spec['touch_position'].shape, (2,))
+    self.assertEqual(action_spec['touch_position'].dtype, np.float32)
+    self.assertEqual(action_spec['keycode'].shape, ())
+    self.assertEqual(action_spec['keycode'].dtype, np.int32)
+
   def test_base_action_spec_multitouch(self):
     action_spec = specs.base_action_spec(num_fingers=3)
     self.assertLen(action_spec.keys(), 6)
     for spec in action_spec.values():
       self.assertIsInstance(spec, dm_env_specs.Array)
     self.assertEqual(action_spec['action_type'].shape, ())
     self.assertEqual(action_spec['action_type'].dtype, np.int32)
```

### Comparing `android_env-1.1.0/android_env/components/task_manager.py` & `android-env-1.2.1/android_env/components/task_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,28 +15,27 @@
 
 """TaskManager handles all events and information related to the task."""
 
 import ast
 import copy
 import datetime
 import json
-import queue
 import re
 import threading
-from typing import Any, Dict
+from typing import Any, Callable, Dict
 
 from absl import logging
-from android_env.components import adb_controller as adb_control
+from android_env.components import adb_call_parser as adb_call_parser_lib
 from android_env.components import app_screen_checker
 from android_env.components import dumpsys_thread
-from android_env.components import errors
 from android_env.components import log_stream as log_stream_lib
 from android_env.components import logcat_thread
 from android_env.components import setup_step_interpreter
 from android_env.proto import task_pb2
+import dm_env
 import numpy as np
 
 
 class TaskManager():
   """Handles all events and information related to the task."""
 
   def __init__(
@@ -60,29 +59,31 @@
     self._task = task
     self._max_bad_states = max_bad_states
     self._dumpsys_check_frequency = dumpsys_check_frequency
     self._max_failed_current_activity = max_failed_current_activity
 
     self._lock = threading.Lock()
     self._extras_max_buffer_size = 100
-    self._adb_controller = None
+    self._logcat_thread = None
+    self._dumpsys_thread = None
     self._setup_step_interpreter = None
 
-    # Logging settings
-    self._log_dict = {
+    # Initialize stats.
+    self._stats = {
+        'episode_steps': 0,
         'reset_count_step_timeout': 0,
-        'reset_count_player_exited': 0,
+        'reset_count_user_exited': 0,
         'reset_count_episode_end': 0,
         'reset_count_max_duration_reached': 0,
         'restart_count_max_bad_states': 0,
+        'task_updates': 0,
     }
 
     # Initialize internal state
     self._task_start_time = None
-    self._episode_steps = 0
     self._bad_state_counter = 0
     self._is_bad_episode = False
 
     self._latest_values = {
         'reward': 0.0,
         'score': 0.0,
         'extra': {},
@@ -90,175 +91,172 @@
     }
 
     logging.info('Task config: %s', self._task)
 
   def task(self) -> task_pb2.Task:
     return self._task
 
-  def increment_steps(self):
-    self._episode_steps += 1
+  def update_task(self, task: task_pb2.Task) -> None:
+    self._stats['task_updates'] += 1
+    self._task = task
+
+  def stats(self) -> Dict[str, Any]:
+    """Returns a dictionary of stats.
+
+    This method is expected to be called after setup_task() has been called.
+    """
+    output = copy.deepcopy(self._stats)
+    if self._setup_step_interpreter is not None:
+      output.update(self._setup_step_interpreter.stats())
+    return output
 
-  def log_dict(self) -> Dict[str, Any]:
-    log_dict = copy.deepcopy(self._log_dict)
-    log_dict.update(self._setup_step_interpreter.log_dict())
-    return log_dict
+  def setup_task(
+      self,
+      adb_call_parser_factory: Callable[[], adb_call_parser_lib.AdbCallParser],
+      log_stream: log_stream_lib.LogStream) -> None:
+    """Performs one-off task setup.."""
+
+    self._start_logcat_thread(log_stream=log_stream)
+    self._start_dumpsys_thread(adb_call_parser_factory())
+    self._start_setup_step_interpreter(adb_call_parser_factory())
+    self._setup_step_interpreter.interpret(self._task.setup_steps)
 
-  def _reset_counters(self):
-    """Reset counters at the end of an RL episode."""
+  def stop_task(self) -> None:
+    """Suspends task processing."""
 
+    self._stop_logcat_thread()
+
+  def reset_task(self) -> None:
+    """Resets a task for a new run."""
+
+    self._logcat_thread.pause()
+    self._setup_step_interpreter.interpret(self._task.reset_steps)
+    self._logcat_thread.resume()
+
+    # Reset some other variables.
     if not self._is_bad_episode:
       self._bad_state_counter = 0
     self._is_bad_episode = False
 
-    self._episode_steps = 0
     self._task_start_time = datetime.datetime.now()
     with self._lock:
       self._latest_values = {
           'reward': 0.0,
           'score': 0.0,
           'extra': {},
           'episode_end': False,
       }
 
-  def setup_task(self,
-                 adb_controller: adb_control.AdbController,
-                 log_stream: log_stream_lib.LogStream) -> None:
-    """Starts the given task along with all relevant processes."""
+  def rl_reset(self, observation: Dict[str, Any]) -> dm_env.TimeStep:
+    """Performs one RL step."""
 
-    self._adb_controller = adb_controller
-    self._start_logcat_thread(log_stream=log_stream)
-    self._start_setup_step_interpreter()
-    self._setup_step_interpreter.interpret(self._task.setup_steps)
+    self._stats['episode_steps'] = 0
 
-  def reset_task(self) -> None:
-    """Resets a task at the end of an RL episode."""
+    self._logcat_thread.line_ready().wait()
+    with self._lock:
+      extras = self._get_current_extras()
 
-    self.pause_task()
-    self._setup_step_interpreter.interpret(self._task.reset_steps)
-    self._resume_task()
-    self._reset_counters()
+    observation['extras'] = extras
 
-  def pause_task(self) -> None:
-    self._stop_dumpsys_thread()
+    return dm_env.TimeStep(
+        step_type=dm_env.StepType.FIRST,
+        reward=0.0,
+        discount=0.0,
+        observation=observation)
 
-  def _resume_task(self) -> None:
-    self._start_dumpsys_thread()
+  def rl_step(self, observation: Dict[str, Any]) -> dm_env.TimeStep:
+    """Performs one RL step."""
 
-  def get_current_reward(self) -> float:
-    """Returns total reward accumulated since the last step."""
+    self._stats['episode_steps'] += 1
 
+    self._logcat_thread.line_ready().wait()
     with self._lock:
-      reward = self._latest_values['reward']
-      self._latest_values['reward'] = 0.0
+      reward = self._get_current_reward()
+      extras = self._get_current_extras()
+      transition_fn = self._determine_transition_fn()
+
+    observation['extras'] = extras
+
+    return transition_fn(reward=reward, observation=observation)
+
+  def _get_current_reward(self) -> float:
+    """Returns total reward accumulated since the last step."""
+    reward = self._latest_values['reward']
+    self._latest_values['reward'] = 0.0
     return reward
 
-  def get_current_extras(self) -> Dict[str, Any]:
+  def _get_current_extras(self) -> Dict[str, Any]:
     """Returns task extras accumulated since the last step."""
-
-    with self._lock:
-      extras = {}
-      for name, values in self._latest_values['extra'].items():
-        extras[name] = np.stack(values)
-      self._latest_values['extra'] = {}
-      return extras
-
-  def check_if_episode_ended(self) -> bool:
-    """Determines whether the episode should be terminated and reset."""
-
-    # Check if player existed the task
-    if self._check_player_exited():
-      self._log_dict['reset_count_player_exited'] += 1
-      logging.warning('Player exited the game. Ending episode.')
+    extras = {}
+    for name, values in self._latest_values['extra'].items():
+      extras[name] = np.stack(values)
+    self._latest_values['extra'] = {}
+    return extras
+
+  def _determine_transition_fn(self) -> Callable[..., dm_env.TimeStep]:
+    """Determines the type of RL transition will be used."""
+
+    # Check if user existed the task
+    if self._dumpsys_thread.check_user_exited():
+      self._increment_bad_state()
+      self._stats['reset_count_user_exited'] += 1
+      logging.warning('User exited the task. Truncating the episode.')
       logging.info('************* END OF EPISODE *************')
-      return True
+      return dm_env.truncation
 
     # Check if episode has ended
-    with self._lock:
-      if self._latest_values['episode_end']:
-        self._log_dict['reset_count_episode_end'] += 1
-        logging.info('End of episode from logcat! Ending episode.')
-        logging.info('************* END OF EPISODE *************')
-        return True
+    if self._latest_values['episode_end']:
+      self._stats['reset_count_episode_end'] += 1
+      logging.info('End of episode from logcat! Ending episode.')
+      return dm_env.termination
 
     # Check if step limit or time limit has been reached
-    if self._task.max_num_steps > 0:
-      if self._episode_steps > self._task.max_num_steps:
-        self._log_dict['reset_count_max_duration_reached'] += 1
-        logging.info('Maximum task duration (steps) reached. Ending episode.')
-        logging.info('************* END OF EPISODE *************')
-        return True
+    if self._task.max_episode_steps > 0:
+      if self._stats['episode_steps'] > self._task.max_episode_steps:
+        self._stats['reset_count_max_duration_reached'] += 1
+        logging.info('Maximum task duration (steps) reached. '
+                     'Truncating the episode.')
+        return dm_env.truncation
 
-    if self._task.max_duration_sec > 0.0:
+    if self._task.max_episode_sec > 0.0:
       task_duration = datetime.datetime.now() - self._task_start_time
-      max_duration_sec = self._task.max_duration_sec
-      if task_duration > datetime.timedelta(seconds=int(max_duration_sec)):
-        self._log_dict['reset_count_max_duration_reached'] += 1
-        logging.info('Maximum task duration (sec) reached. Ending episode.')
-        logging.info('************* END OF EPISODE *************')
-        return True
-
-    return False
-
-  def _check_player_exited(self) -> bool:
-    """Returns whether the player has exited the game."""
-    try:
-      self._check_player_exited_impl()
-      return False
-    except errors.NotAllowedError:
-      return True
-
-  def _check_player_exited_impl(self):
-    """Raises an error if the OS is not in an allowed state."""
-
-    if not hasattr(self, '_dumpsys_thread'):
-      return
-
-    self._dumpsys_thread.write(
-        dumpsys_thread.DumpsysThread.Signal.FETCH_DUMPSYS)
-
-    try:
-      v = self._dumpsys_thread.read(block=False)
-      if v == dumpsys_thread.DumpsysThread.Signal.USER_EXITED_ACTIVITY:
-        self._increment_bad_state()
-        raise errors.PlayerExitedActivityError()
-      elif v == dumpsys_thread.DumpsysThread.Signal.USER_EXITED_VIEW_HIERARCHY:
-        self._increment_bad_state()
-        raise errors.PlayerExitedViewHierarchyError()
-    except queue.Empty:
-      pass  # Don't block here, just ignore if we have nothing.
+      max_episode_sec = self._task.max_episode_sec
+      if task_duration > datetime.timedelta(seconds=int(max_episode_sec)):
+        self._stats['reset_count_max_duration_reached'] += 1
+        logging.info('Maximum task duration (sec) reached. '
+                     'Truncating the episode.')
+        return dm_env.truncation
+
+    return dm_env.transition
 
-  def _start_setup_step_interpreter(self):
+  def _start_setup_step_interpreter(
+      self, adb_call_parser: adb_call_parser_lib.AdbCallParser):
     self._setup_step_interpreter = setup_step_interpreter.SetupStepInterpreter(
-        adb_controller=self._adb_controller,
-        logcat=self._logcat_thread)
+        adb_call_parser=adb_call_parser)
 
   def _start_logcat_thread(self, log_stream: log_stream_lib.LogStream):
-    self._logcat_thread = logcat_thread.LogcatThread(
-        log_stream=log_stream,
-        log_parsing_config=self._task.log_parsing_config)
+    log_stream.set_log_filters(list(self._task.log_parsing_config.filters))
+    self._logcat_thread = logcat_thread.LogcatThread(log_stream=log_stream)
 
     for event_listener in self._logcat_listeners():
       self._logcat_thread.add_event_listener(event_listener)
 
-  def _start_dumpsys_thread(self):
+  def _start_dumpsys_thread(self,
+                            adb_call_parser: adb_call_parser_lib.AdbCallParser):
     self._dumpsys_thread = dumpsys_thread.DumpsysThread(
         app_screen_checker=app_screen_checker.AppScreenChecker(
-            self._adb_controller, self._task.expected_app_screen),
+            adb_call_parser=adb_call_parser,
+            expected_app_screen=self._task.expected_app_screen),
         check_frequency=self._dumpsys_check_frequency,
-        max_failed_current_activity=self._max_failed_current_activity,
-        block_input=True,
-        block_output=True)
+        max_failed_current_activity=self._max_failed_current_activity)
 
   def _stop_logcat_thread(self):
-    if hasattr(self, '_logcat_thread'):
+    if self._logcat_thread is not None:
       self._logcat_thread.kill()
-
-  def _stop_dumpsys_thread(self):
-    if hasattr(self, '_dumpsys_thread'):
-      self._dumpsys_thread.kill()
+      self._logcat_thread = None
 
   def _increment_bad_state(self) -> None:
     """Increments the bad state counter.
 
     Bad states are errors that shouldn't happen and that trigger an
     episode reset. If enough bad states have been seen consecutively,
     we restart the simulation in the hope of returning the simulation
@@ -267,15 +265,15 @@
     logging.warning('Bad state detected.')
     if self._max_bad_states:
       self._is_bad_episode = True
       self._bad_state_counter += 1
       logging.warning('Bad state counter: %d.', self._bad_state_counter)
       if self._bad_state_counter >= self._max_bad_states:
         logging.error('Too many consecutive bad states. Restarting simulator.')
-        self._log_dict['restart_count_max_bad_states'] += 1
+        self._stats['restart_count_max_bad_states'] += 1
         self._should_restart = True
     else:
       logging.warning('Max bad states not set, bad states will be ignored.')
 
   def _logcat_listeners(self):
     """Creates list of EventListeners for logcat thread."""
 
@@ -381,13 +379,7 @@
             latest_extras[extra_name].pop(0)
           latest_extras[extra_name].append(extra)
         else:
           latest_extras[extra_name] = [extra]
         self._latest_values['extra'] = latest_extras
 
     return listeners
-
-  def close(self):
-    if hasattr(self, '_logcat_thread'):
-      self._logcat_thread.kill()
-    if hasattr(self, '_dumpsys_thread'):
-      self._dumpsys_thread.kill()
```

### Comparing `android_env-1.1.0/android_env/environment.py` & `android-env-1.2.1/android_env/environment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,30 +13,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Android environment implementation."""
 
 from typing import Any, Dict
 from absl import logging
+from android_env import env_interface
 from android_env.components import coordinator as coordinator_lib
+from android_env.proto import adb_pb2
+from android_env.proto import task_pb2
 import dm_env
 import numpy as np
 
 
-class AndroidEnv(dm_env.Environment):
+class AndroidEnv(env_interface.AndroidEnvInterface):
   """An RL environment that interacts with Android apps."""
 
   def __init__(self, coordinator: coordinator_lib.Coordinator):
     """Initializes the state of this AndroidEnv object."""
 
     self._coordinator = coordinator
     self._latest_action = {}
     self._latest_observation = {}
     self._latest_extras = {}
     self._reset_next_step = True
+    self._is_closed = False
 
     logging.info('Action spec: %s', self.action_spec())
     logging.info('Observation spec: %s', self.observation_spec())
     logging.info('Task extras spec: %s', self.task_extras_spec())
 
   def action_spec(self) -> Dict[str, dm_env.specs.Array]:
     return self._coordinator.action_spec()
@@ -45,89 +49,110 @@
     return self._coordinator.observation_spec()
 
   def task_extras_spec(self) -> Dict[str, dm_env.specs.Array]:
     return self._coordinator.task_extras_spec()
 
   @property
   def raw_action(self):
-    return self._latest_action
+    return self._latest_action.copy()
 
   @property
   def raw_observation(self):
-    return self._latest_observation
+    return self._latest_observation.copy()
 
-  def android_logs(self) -> Dict[str, Any]:
-    return self._coordinator.get_logs()
+  def stats(self) -> Dict[str, Any]:
+    return self._coordinator.stats()
 
   def reset(self) -> dm_env.TimeStep:
     """Resets the environment for a new RL episode."""
 
     logging.info('Resetting AndroidEnv...')
 
-    # Reset state of the environment.
-    self._coordinator.reset_environment_state()
-
-    # Execute selected action (None when resetting).
-    obs, _, extras, _ = self._coordinator.execute_action(action=None)
+    # Execute a reset. Timestep will be of type FIRST.
+    timestep = self._coordinator.rl_reset()
 
     # Process relevant information.
-    if obs is not None:
-      self._latest_observation = obs.copy()
-    self._latest_extras = extras.copy()
+    if timestep.observation is not None:
+      self._latest_extras = timestep.observation.pop('extras')
+      self._latest_observation = timestep.observation.copy()
+    else:
+      # If the observation is None, we return the latest observation again.
+      timestep = timestep._replace(observation=self._latest_observation.copy())
+
     self._latest_action = {}
     self._reset_next_step = False
 
     logging.info('Done resetting AndroidEnv.')
     logging.info('************* NEW EPISODE *************')
 
-    return dm_env.TimeStep(
-        step_type=dm_env.StepType.FIRST,
-        observation=self._latest_observation,
-        reward=0.0,
-        discount=0.0)
+    return timestep
 
   def step(self, action: Dict[str, np.ndarray]) -> dm_env.TimeStep:
     """Takes a step in the environment."""
 
     # Check if it's time to reset the episode.
     if self._reset_next_step:
       return self.reset()
 
     # Execute selected action.
-    obs, reward, extras, episode_end = self._coordinator.execute_action(action)
+    timestep = self._coordinator.rl_step(action)
 
     # Process relevant information.
-    if obs is not None:
-      self._latest_observation = obs.copy()
-    self._latest_extras = extras.copy()
+    if timestep.observation is not None:
+      self._latest_extras = timestep.observation.pop('extras')
+      self._latest_observation = timestep.observation.copy()
+    else:
+      # If the observation is None, we return the latest observation again.
+      timestep = timestep._replace(observation=self._latest_observation.copy())
+
     self._latest_action = action.copy()
-    self._reset_next_step = episode_end
 
-    # Return timestep with reward and observation just computed.
-    if episode_end:
-      return dm_env.termination(
-          observation=self._latest_observation, reward=reward)
-    else:
-      return dm_env.transition(
-          observation=self._latest_observation, reward=reward, discount=0.0)
+    if timestep.last():
+      self._reset_next_step = True
+      logging.info('************* END OF EPISODE *************')
+
+    return timestep
 
   def task_extras(self, latest_only: bool = True) -> Dict[str, np.ndarray]:
     """Returns latest task extras."""
 
     task_extras = {}
     for key, spec in self.task_extras_spec().items():
       if key in self._latest_extras:
         extra_values = self._latest_extras[key].astype(spec.dtype)
         for extra in extra_values:
-          spec.validate(extra)
+          self._validate_type(spec, extra)
         task_extras[key] = extra_values[-1] if latest_only else extra_values
     return task_extras
 
+  def _validate_type(self, spec: dm_env.specs.Array, data: np.ndarray):
+    # Handling of spec data type of string of arbitary length.
+    if spec.dtype.str == '<U0' and data.dtype.str.startswith(
+        '<U') and spec.shape == data.shape:
+      return
+    spec.validate(data)
+
+  def execute_adb_call(self, call: adb_pb2.AdbRequest) -> adb_pb2.AdbResponse:
+    return self._coordinator.execute_adb_call(call)
+
+  def update_task(self, task: task_pb2.Task) -> bool:
+    """Replaces the current task with a new task.
+
+    Args:
+      task: A new task to replace the current one.
+
+    Returns:
+      A bool indicating the success of the task setup.
+    """
+    return self._coordinator.update_task(task)
+
   def close(self) -> None:
     """Cleans up running processes, threads and local files."""
-    logging.info('Cleaning up AndroidEnv...')
-    if hasattr(self, '_coordinator'):
-      self._coordinator.close()
-    logging.info('Done cleaning up AndroidEnv.')
+    if not self._is_closed:
+      logging.info('Cleaning up AndroidEnv...')
+      if hasattr(self, '_coordinator'):
+        self._coordinator.close()
+      logging.info('Done cleaning up AndroidEnv.')
+      self._is_closed = True
 
   def __del__(self) -> None:
     self.close()
```

### Comparing `android_env-1.1.0/android_env/environment_test.py` & `android-env-1.2.1/android_env/environment_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,23 +11,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for AndroidEnv."""
 
+from unittest import mock
+
 from absl.testing import absltest
 from android_env import environment
 from android_env.components import coordinator as coordinator_lib
+from android_env.proto import adb_pb2
+from android_env.proto import task_pb2
 import dm_env
-import mock
 import numpy as np
 
 
-def _create_mock_env():
+def _create_mock_coordinator() -> coordinator_lib.Coordinator:
   coordinator = mock.create_autospec(coordinator_lib.Coordinator)
   coordinator.action_spec.return_value = {
       'action_type':
           dm_env.specs.DiscreteArray(num_values=3),
       'touch_position':
           dm_env.specs.BoundedArray(
               shape=(2,), dtype=np.float32, minimum=0.0, maximum=1.0),
@@ -36,21 +39,21 @@
       'pixels': dm_env.specs.Array(shape=(123, 456, 3), dtype=np.uint8),
       'timedelta': dm_env.specs.Array(shape=(), dtype=np.int64),
       'orientation': dm_env.specs.Array(shape=(4,), dtype=np.uint8),
   }
   coordinator.task_extras_spec.return_value = {
       'click': dm_env.specs.Array(shape=(), dtype=np.int64),
   }
-  return environment.AndroidEnv(coordinator)
+  return coordinator
 
 
 class AndroidEnvTest(absltest.TestCase):
 
   def test_specs(self):
-    env = _create_mock_env()
+    env = environment.AndroidEnv(_create_mock_coordinator())
 
     # Check action spec.
     self.assertNotEmpty(env.action_spec())
     self.assertIn('action_type', env.action_spec())
     self.assertIsInstance(env.action_spec()['action_type'],
                           dm_env.specs.DiscreteArray)
     self.assertIn('touch_position', env.action_spec())
@@ -95,25 +98,26 @@
         'timedelta': dm_env.specs.Array(shape=(), dtype=np.int64),
         'orientation': dm_env.specs.Array(shape=(4,), dtype=np.uint8),
     }
     coordinator.task_extras_spec.return_value = {
         'click': dm_env.specs.Array(shape=(1,), dtype=np.int64),
     }
     env = environment.AndroidEnv(coordinator)
-    coordinator.execute_action.return_value = (
-        {
+    coordinator.rl_reset.return_value = dm_env.TimeStep(
+        step_type=dm_env.StepType.FIRST,
+        reward=0.0,
+        discount=0.0,
+        observation={
             'pixels': np.random.rand(987, 654, 3),
             'timedelta': 123456,
             'orientation': np.array((1, 0, 0, 0)),
-        },  # Observation
-        0.0,  # Reward.
-        {
-            'click': np.array([[246]], dtype=np.int64)
-        },  # Task extras.
-        False  # Episode ended?
+            'extras': {
+                'click': np.array([[246]], dtype=np.int64)
+            }
+        },
     )
 
     ts = env.reset()
     self.assertIsInstance(ts, dm_env.TimeStep)
     # After a `reset()` the TimeStep should follow some expectations.
     self.assertTrue(ts.first())
     self.assertEqual(ts.reward, 0.0)
@@ -128,19 +132,33 @@
     np.testing.assert_equal(obs['orientation'], (1, 0, 0, 0))
 
     # Extras should also be provided.
     extras = env.task_extras()
     self.assertIn('click', extras)
     self.assertEqual(extras['click'], np.array([246], dtype=np.int64))
 
-    coordinator.get_logs.return_value = {
+    coordinator.stats.return_value = {
         'my_measurement': 135,
     }
 
     # Step again in the environment and check expectations again.
+    pixels = np.random.rand(987, 654, 3)
+    latest_observation = {
+        'pixels': pixels,
+        'timedelta': 123456,
+        'orientation': np.array((1, 0, 0, 0)),
+        'extras': {
+            'click': np.array([[246]], dtype=np.int64)
+        }
+    }
+    coordinator.rl_step.return_value = dm_env.transition(
+        reward=0.0,
+        discount=0.0,
+        observation=latest_observation,
+    )
     ts = env.step({'action_type': 1, 'touch_position': (10, 20)})
     self.assertIsInstance(ts, dm_env.TimeStep)
     # The StepType now should NOT be FIRST.
     self.assertFalse(ts.first())
     self.assertEqual(ts.reward, 0.0)
     self.assertEqual(ts.discount, 0.0)
     obs = ts.observation
@@ -154,14 +172,63 @@
 
     # Extras should still be provided.
     extras = env.task_extras()
     self.assertIn('click', extras)
     self.assertEqual(extras['click'], np.array([246], dtype=np.int64))
 
     # At this point these methods and properties should return something.
-    self.assertNotEmpty(env.android_logs())
+    self.assertNotEmpty(env.stats())
     self.assertNotEmpty(env.raw_observation)
+    self.assertNotIn('extras', env.raw_observation)
     self.assertNotEmpty(env.raw_action)
 
+    # If the observation is None, we want to return the latest observation.
+    coordinator.rl_step.return_value = dm_env.truncation(
+        reward=0.0,
+        observation=None,
+    )
+    ts = env.step({'action_type': 1, 'touch_position': (10, 20)})
+    self.assertIsInstance(ts, dm_env.TimeStep)
+    # Assert the observation matches the latest observation.
+    obs = ts.observation
+    self.assertIn('pixels', obs)
+    self.assertEqual(obs['pixels'].shape, (987, 654, 3))
+    np.testing.assert_equal(obs['pixels'], pixels)
+    self.assertIn('timedelta', obs)
+    self.assertEqual(obs['timedelta'], 123456)
+    self.assertIn('orientation', obs)
+    self.assertEqual(obs['orientation'].shape, (4,))
+    np.testing.assert_equal(obs['orientation'], (1, 0, 0, 0))
+
+  def test_adb_call(self):
+    coordinator = _create_mock_coordinator()
+    env = environment.AndroidEnv(coordinator)
+    call = adb_pb2.AdbRequest(
+        force_stop=adb_pb2.AdbRequest.ForceStop(package_name='blah'))
+    expected_response = adb_pb2.AdbResponse(
+        status=adb_pb2.AdbResponse.Status.OK)
+    coordinator.execute_adb_call.return_value = expected_response
+
+    response = env.execute_adb_call(call)
+
+    self.assertEqual(response, expected_response)
+    coordinator.execute_adb_call.assert_called_once_with(call)
+
+  def test_update_task(self):
+    coordinator = _create_mock_coordinator()
+    env = environment.AndroidEnv(coordinator)
+    task = task_pb2.Task()
+    coordinator.update_task.return_value = True
+    response = env.update_task(task)
+    self.assertEqual(response, True)
+    coordinator.update_task.assert_called_once_with(task)
+
+  def test_double_close(self):
+    coordinator = _create_mock_coordinator()
+    env = environment.AndroidEnv(coordinator)
+    env.close()
+    env.close()
+    coordinator.close.assert_called_once()
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `android_env-1.1.0/android_env/loader.py` & `android-env-1.2.1/android_env/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -48,15 +48,14 @@
   """
 
   # Create simulator.
   simulator = emulator_simulator.EmulatorSimulator(
       adb_controller_args=dict(
           adb_path=os.path.expanduser(adb_path),
           adb_server_port=5037,
-          prompt_regex=r'\w*:\/ \$',
       ),
       emulator_launcher_args=dict(
           avd_name=avd_name,
           android_avd_home=os.path.expanduser(android_avd_home),
           android_sdk_root=os.path.expanduser(android_sdk_root),
           emulator_path=os.path.expanduser(emulator_path),
           run_headless=run_headless,
```

### Comparing `android_env-1.1.0/android_env/loader_test.py` & `android-env-1.2.1/android_env/loader_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,22 +13,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for loader."""
 
 import builtins
 import os
+from unittest import mock
+
 from absl.testing import absltest
 from android_env import environment
 from android_env import loader
 from android_env.components import coordinator as coordinator_lib
 from android_env.components import task_manager as task_manager_lib
 from android_env.components.simulators.emulator import emulator_simulator
 from android_env.proto import task_pb2
-import mock
 
 
 class LoaderTest(absltest.TestCase):
 
   @mock.patch.object(task_manager_lib, 'TaskManager', autospec=True)
   @mock.patch.object(emulator_simulator, 'EmulatorSimulator', autospec=True)
   @mock.patch.object(coordinator_lib, 'Coordinator', autospec=True)
@@ -49,15 +50,14 @@
     )
 
     self.assertIsInstance(env, environment.AndroidEnv)
     simulator.assert_called_with(
         adb_controller_args=dict(
             adb_path=os.path.expanduser('~/Android/Sdk/platform-tools/adb'),
             adb_server_port=5037,
-            prompt_regex=r'\w*:\/ \$',
         ),
         emulator_launcher_args=dict(
             avd_name='my_avd',
             android_avd_home=os.path.expanduser('~/.android/avd'),
             android_sdk_root=os.path.expanduser('~/Android/Sdk'),
             emulator_path=os.path.expanduser('~/Android/Sdk/emulator/emulator'),
             run_headless=False,
@@ -76,27 +76,27 @@
 
     del coordinator, simulator
     mock_open.return_value.__enter__ = mock_open
     mock_open.return_value.read.return_value = r'''
 id: "fake_task"
 name: "Fake Task"
 description: "Task for testing loader."
-max_duration_sec: 0
+max_episode_sec: 0
 '''
 
     env = loader.load(
         task_path='some/path/',
         avd_name='my_avd',
     )
 
     expected_task = task_pb2.Task()
     expected_task.id = 'fake_task'
     expected_task.name = 'Fake Task'
     expected_task.description = 'Task for testing loader.'
-    expected_task.max_duration_sec = 0
+    expected_task.max_episode_sec = 0
 
     task_manager.assert_called_with(expected_task)
     assert isinstance(env, environment.AndroidEnv)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `android_env-1.1.0/android_env/proto/__init__.py` & `android-env-1.2.1/android_env/components/simulators/fake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/wrappers/base_wrapper.py` & `android-env-1.2.1/android_env/wrappers/base_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,33 +12,43 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base class for AndroidEnv wrappers."""
 
 from typing import Any, Dict
+
+from absl import logging
+from android_env import env_interface
+from android_env.proto import adb_pb2
+from android_env.proto import task_pb2
 import dm_env
 from dm_env import specs
+import numpy as np
 
 
-class BaseWrapper(dm_env.Environment):
+class BaseWrapper(env_interface.AndroidEnvInterface):
   """AndroidEnv wrapper."""
 
   def __init__(self, env):
     self._env = env
+    logging.info('Wrapping with %s', self.__class__.__name__)
 
   def reset(self) -> dm_env.TimeStep:
     self._reset_state()
     timestep = self._process_timestep(self._env.reset())
     return timestep
 
   def step(self, action: Any) -> dm_env.TimeStep:
     action = self._process_action(action)
     return self._process_timestep(self._env.step(action))
 
+  def task_extras(self, latest_only: bool = True) -> Dict[str, np.ndarray]:
+    return self._env.task_extras(latest_only=latest_only)
+
   def _reset_state(self):
     pass
 
   def _process_action(self, action: Any) -> Any:
     return action
 
   def _process_timestep(self, timestep: dm_env.TimeStep) -> dm_env.TimeStep:
@@ -46,23 +56,41 @@
 
   def observation_spec(self) -> Dict[str, specs.Array]:
     return self._env.observation_spec()
 
   def action_spec(self) -> Dict[str, specs.Array]:
     return self._env.action_spec()
 
-  def _wrapper_logs(self) -> Dict[str, Any]:
+  def task_extras_spec(self) -> Dict[str, specs.Array]:
+    return self._env.task_extras_spec()
+
+  def _wrapper_stats(self) -> Dict[str, Any]:
     """Add wrapper specific logging here."""
     return {}
 
-  def android_logs(self) -> Dict[str, Any]:
-    info = self._env.android_logs()
-    info.update(self._wrapper_logs())
+  def stats(self) -> Dict[str, Any]:
+    info = self._env.stats()
+    info.update(self._wrapper_stats())
     return info
 
+  def execute_adb_call(self,
+                       adb_call: adb_pb2.AdbRequest) -> adb_pb2.AdbResponse:
+    return self._env.execute_adb_call(adb_call)
+
+  def update_task(self, task: task_pb2.Task) -> bool:
+    return self._env.update_task(task)
+
+  @property
+  def raw_action(self):
+    return self._env.raw_action
+
+  @property
+  def raw_observation(self):
+    return self._env.raw_observation
+
   @property
   def raw_env(self):
     """Recursively unwrap until we reach the true 'raw' env."""
     wrapped = self._env
     if hasattr(wrapped, 'raw_env'):
       return wrapped.raw_env
     return wrapped
```

### Comparing `android_env-1.1.0/android_env/wrappers/discrete_action_wrapper.py` & `android-env-1.2.1/android_env/wrappers/discrete_action_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/wrappers/flat_interface_wrapper.py` & `android-env-1.2.1/android_env/wrappers/flat_interface_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/wrappers/float_pixels_wrapper.py` & `android-env-1.2.1/android_env/wrappers/float_pixels_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,43 +25,40 @@
 
 
 class FloatPixelsWrapper(base_wrapper.BaseWrapper):
   """Wraps AndroidEnv for Panultimate agent."""
 
   def __init__(self, env: dm_env.Environment):
     super().__init__(env)
-    self._should_convert_int_to_float = np.issubdtype(
-        self._env.observation_spec()['pixels'].dtype, np.integer)
+    self._input_spec = self._env.observation_spec()['pixels']
+    self._should_convert_int_to_float = np.issubdtype(self._input_spec.dtype,
+                                                      np.integer)
 
   def _process_observation(
       self, observation: Dict[str, np.ndarray]
   ) -> Dict[str, np.ndarray]:
     if self._should_convert_int_to_float:
-      float_pixels = utils.convert_int_to_float(
-          observation['pixels'],
-          self._env.observation_spec()['pixels'],
-          np.float32)
+      float_pixels = utils.convert_int_to_float(observation['pixels'],
+                                                self._input_spec, np.float32)
       observation['pixels'] = float_pixels
     return observation
 
   def _process_timestep(self, timestep: dm_env.TimeStep) -> dm_env.TimeStep:
     step_type, reward, discount, observation = timestep
     return dm_env.TimeStep(
         step_type=step_type,
         reward=reward,
         discount=discount,
         observation=self._process_observation(observation))
 
   def reset(self) -> dm_env.TimeStep:
-    timestep = self._env.reset()
-    return self._process_timestep(timestep)
+    return self._process_timestep(self._env.reset())
 
   def step(self, action: Dict[str, np.ndarray]) -> dm_env.TimeStep:
-    timestep = self._env.step(action)
-    return self._process_timestep(timestep)
+    return self._process_timestep(self._env.step(action))
 
   def observation_spec(self) -> Dict[str, specs.Array]:
     if self._should_convert_int_to_float:
       observation_spec = self._env.observation_spec()
       observation_spec['pixels'] = specs.BoundedArray(
           shape=self._env.observation_spec()['pixels'].shape,
           dtype=np.float32,
```

### Comparing `android_env-1.1.0/android_env/wrappers/gym_wrapper.py` & `android-env-1.2.1/android_env/wrappers/gym_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/wrappers/image_rescale_wrapper.py` & `android-env-1.2.1/android_env/wrappers/image_rescale_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -65,15 +65,15 @@
         observation['pixels'])
     return timestep._replace(observation=processed_observation)
 
   def _process_pixels(self, raw_observation: np.ndarray) -> np.ndarray:
     # We expect `raw_observation` to have shape (W, H, 3) - 3 for RGB
     new_shape = np.array(
         self._zoom_factors[0:2] * np.array(raw_observation.shape[0:2]),
-        dtype=np.int)[::-1]
+        dtype=np.int32)[::-1]
     if self._grayscale:
       # When self._grayscale == True, we squash the RGB into a single layer
       image = np.dot(raw_observation, RGB_TO_GRAYSCALE_COEFFICIENTS)
     else:
       image = raw_observation
     return self._resize_image_array(image, new_shape)
```

### Comparing `android_env-1.1.0/android_env/wrappers/last_action_wrapper.py` & `android-env-1.2.1/android_env/wrappers/last_action_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `android_env-1.1.0/android_env/wrappers/tap_action_wrapper.py` & `android-env-1.2.1/android_env/wrappers/tap_action_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,17 +35,17 @@
                touch_only: bool = False):
     super().__init__(env)
     assert 'action_type' in env.action_spec()
     self._touch_only = touch_only
     self._num_frames = num_frames
     self._env_steps = 0
 
-  def android_logs(self):
+  def stats(self):
     """Returns a dictionary of metrics logged by the environment."""
-    logs = self._env.android_logs()
+    logs = self._env.stats()
     logs.update({'env_steps': self._env_steps})
     return logs
 
   def _process_action(
       self, action: Dict[str, np.ndarray]
   ) -> Sequence[Dict[str, np.ndarray]]:
 
@@ -72,15 +72,15 @@
 
     return actions
 
   def step(self, action: Dict[str, np.ndarray]) -> dm_env.TimeStep:
     """Takes a step in the environment."""
     self._env_steps += self._num_frames + 1
     actions = self._process_action(action)
-    total_reward = 0
+    total_reward = 0.0
     for idx in range(len(actions)):
       step_type, reward, discount, observation = self._env.step(actions[idx])
       if reward:
         total_reward += reward
       if step_type == dm_env.StepType.LAST:
         return dm_env.TimeStep(
             step_type=step_type,
@@ -99,8 +99,7 @@
           'action_type':
               dm_env.specs.DiscreteArray(num_values=1, name='action_type'),
           'touch_position':
               self._env.action_spec()['touch_position'],
       }
     else:
       return self._env.action_spec()
-
```

### Comparing `android_env-1.1.0/android_env.egg-info/SOURCES.txt` & `android-env-1.2.1/android_env.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 android_env/__init__.py
+android_env/env_interface.py
 android_env/environment.py
 android_env/environment_test.py
 android_env/loader.py
 android_env/loader_test.py
 android_env.egg-info/PKG-INFO
 android_env.egg-info/SOURCES.txt
 android_env.egg-info/dependency_links.txt
 android_env.egg-info/requires.txt
 android_env.egg-info/top_level.txt
 android_env/components/__init__.py
 android_env/components/action_type.py
+android_env/components/adb_call_parser.py
+android_env/components/adb_call_parser_test.py
 android_env/components/adb_controller.py
 android_env/components/adb_controller_test.py
 android_env/components/adb_log_stream.py
 android_env/components/adb_log_stream_test.py
 android_env/components/app_screen_checker.py
 android_env/components/app_screen_checker_test.py
 android_env/components/coordinator.py
@@ -31,32 +34,44 @@
 android_env/components/logcat_thread_test.py
 android_env/components/setup_step_interpreter.py
 android_env/components/setup_step_interpreter_test.py
 android_env/components/specs.py
 android_env/components/specs_test.py
 android_env/components/task_manager.py
 android_env/components/task_manager_test.py
-android_env/components/thread_function.py
-android_env/components/thread_function_test.py
 android_env/components/utils.py
 android_env/components/utils_test.py
 android_env/components/simulators/__init__.py
 android_env/components/simulators/base_simulator.py
 android_env/components/simulators/base_simulator_test.py
 android_env/components/simulators/emulator/__init__.py
 android_env/components/simulators/emulator/emulator_launcher.py
 android_env/components/simulators/emulator/emulator_launcher_test.py
 android_env/components/simulators/emulator/emulator_simulator.py
 android_env/components/simulators/emulator/emulator_simulator_test.py
 android_env/components/simulators/fake/__init__.py
 android_env/components/simulators/fake/fake_simulator.py
 android_env/components/simulators/fake/fake_simulator_test.py
 android_env/proto/__init__.py
+android_env/proto/adb.proto
+android_env/proto/emulator_controller.proto
+android_env/proto/raw_observation.proto
+android_env/proto/task.proto
 android_env/wrappers/__init__.py
 android_env/wrappers/base_wrapper.py
+android_env/wrappers/base_wrapper_test.py
 android_env/wrappers/discrete_action_wrapper.py
+android_env/wrappers/discrete_action_wrapper_test.py
 android_env/wrappers/flat_interface_wrapper.py
+android_env/wrappers/flat_interface_wrapper_test.py
 android_env/wrappers/float_pixels_wrapper.py
+android_env/wrappers/float_pixels_wrapper_test.py
 android_env/wrappers/gym_wrapper.py
+android_env/wrappers/gym_wrapper_test.py
 android_env/wrappers/image_rescale_wrapper.py
+android_env/wrappers/image_rescale_wrapper_test.py
 android_env/wrappers/last_action_wrapper.py
-android_env/wrappers/tap_action_wrapper.py
+android_env/wrappers/last_action_wrapper_test.py
+android_env/wrappers/rate_limit_wrapper.py
+android_env/wrappers/rate_limit_wrapper_test.py
+android_env/wrappers/tap_action_wrapper.py
+android_env/wrappers/tap_action_wrapper_test.py
```

### Comparing `android_env-1.1.0/setup.py` & `android-env-1.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 DeepMind Technologies Limited.
+# Copyright 2022 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,18 +19,14 @@
 
 import pkg_resources
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 
-description = """AndroidEnv
-Read the README at https://github.com/deepmind/android_env for more information.
-"""
-
 _ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 # Tuple of proto message definitions to build Python bindings for. Paths must
 # be relative to root directory.
 _ANDROID_ENV_PROTOS = (
     'android_env/proto/emulator_controller.proto',
     'android_env/proto/raw_observation.proto',
@@ -39,14 +35,15 @@
 )
 
 testing_requirements = [
     'attrs==20.3.0',  # temporary pin to fix pytype issue.
     'pillow',
     'pytype',
     'pytest-xdist',
+    'gym',
 ]
 
 
 class _GenerateProtoFiles(cmd.Command):
   """Command to generate protobuf bindings for AndroidEnv protos."""
 
   descriptions = 'Generates Python protobuf bindings for AndroidEnv protos.'
@@ -91,41 +88,18 @@
   """Generate protobuf bindings in build_py stage."""
 
   def run(self):
     self.run_command('generate_protos')
     build_py.run(self)
 
 setup(
-    name='android_env',
-    version='1.1.0',
-    description='AndroidEnv environment and library for training agents.',
-    long_description=description,
-    author='DeepMind',
-    license='Apache License, Version 2.0',
-    keywords='Android OS reinforcement-learning',
     url='https://github.com/deepmind/android_env',
     packages=find_packages(exclude=['examples']),
-    setup_requires=[
-        'grpcio-tools',
-    ],
-    install_requires=[
-        'absl-py>=0.1.0',
-        'dm_env',
-        'grpcio',
-        'mock',
-        'numpy<1.20',
-        'pexpect',
-        'portpicker>=1.2.0',
-        'protobuf>=2.6',
-        'pygame',
-    ],
-    extras_require={
-        'acme': ['dm-acme'],
-        'gym': ['gym'],
-        'testing': testing_requirements,
-    },
+    package_data={'': ['proto/*.proto']},  # Copy protobuf files.
+    include_package_data=True,
+    setup_requires=['grpcio-tools'],
     cmdclass={
         'build_ext': _BuildExt,
         'build_py': _BuildPy,
         'generate_protos': _GenerateProtoFiles,
     },
 )
```


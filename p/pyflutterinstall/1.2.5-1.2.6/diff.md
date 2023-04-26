# Comparing `tmp/pyflutterinstall-1.2.5.tar.gz` & `tmp/pyflutterinstall-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflutterinstall-1.2.5.tar", last modified: Wed Apr  5 06:02:15 2023, max compression
+gzip compressed data, was "pyflutterinstall-1.2.6.tar", last modified: Wed Apr 26 22:13:34 2023, max compression
```

## Comparing `pyflutterinstall-1.2.5.tar` & `pyflutterinstall-1.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.109635 pyflutterinstall-1.2.5/
--rw-rw-rw-   0        0        0     1064 2022-09-27 06:03:03.000000 pyflutterinstall-1.2.5/LICENSE
--rw-rw-rw-   0        0        0       24 2022-09-27 06:03:03.000000 pyflutterinstall-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3918 2023-04-05 06:02:15.108639 pyflutterinstall-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3168 2023-04-05 06:00:43.000000 pyflutterinstall-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.066637 pyflutterinstall-1.2.5/pyflutterinstall/
--rw-rw-rw-   0        0        0       14 2023-01-14 03:41:26.000000 pyflutterinstall-1.2.5/pyflutterinstall/__init__.py
--rw-rw-rw-   0        0        0     5301 2023-03-24 08:25:28.000000 pyflutterinstall-1.2.5/pyflutterinstall/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.097641 pyflutterinstall-1.2.5/pyflutterinstall/cmds/
--rw-rw-rw-   0        0        0       14 2023-01-14 03:41:26.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/__init__.py
--rw-rw-rw-   0        0        0      599 2023-03-25 11:54:46.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/adb.py
--rw-rw-rw-   0        0        0      607 2023-03-25 11:54:56.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/avdmanager.py
--rw-rw-rw-   0        0        0      582 2023-03-25 11:54:59.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/emulator.py
--rw-rw-rw-   0        0        0      996 2023-03-24 09:30:28.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/gradle.py
--rw-rw-rw-   0        0        0      731 2023-03-24 09:10:58.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/java.py
--rw-rw-rw-   0        0        0      604 2023-03-25 11:55:44.000000 pyflutterinstall-1.2.5/pyflutterinstall/cmds/sdkmanager.py
--rw-rw-rw-   0        0        0      909 2023-03-24 08:26:30.000000 pyflutterinstall-1.2.5/pyflutterinstall/config.py
--rw-rw-rw-   0        0        0      546 2023-02-18 22:32:44.000000 pyflutterinstall-1.2.5/pyflutterinstall/flutter_doctor.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.103638 pyflutterinstall-1.2.5/pyflutterinstall/install/
--rw-rw-rw-   0        0        0       14 2023-02-03 04:33:07.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/__init__.py
--rw-rw-rw-   0        0        0     3778 2023-03-24 10:39:37.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/android_sdk.py
--rw-rw-rw-   0        0        0     1619 2023-03-08 00:25:48.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/ant_sdk.py
--rw-rw-rw-   0        0        0     1317 2023-02-18 22:32:44.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/chrome.py
--rw-rw-rw-   0        0        0     2700 2023-02-18 22:32:53.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/flutter_sdk.py
--rw-rw-rw-   0        0        0      755 2023-02-18 22:32:44.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/gradle.py
--rw-rw-rw-   0        0        0     2599 2023-04-05 06:01:04.000000 pyflutterinstall-1.2.5/pyflutterinstall/install/java_sdk.py
--rw-rw-rw-   0        0        0      522 2023-02-03 04:33:07.000000 pyflutterinstall-1.2.5/pyflutterinstall/outstream.py
--rw-rw-rw-   0        0        0     2124 2023-03-23 08:25:30.000000 pyflutterinstall-1.2.5/pyflutterinstall/postrun.py
--rw-rw-rw-   0        0        0     4462 2023-04-05 06:01:33.000000 pyflutterinstall-1.2.5/pyflutterinstall/resources.py
--rw-rw-rw-   0        0        0     2328 2023-02-18 22:32:44.000000 pyflutterinstall-1.2.5/pyflutterinstall/setenv.py
--rw-rw-rw-   0        0        0     1459 2023-03-24 10:09:27.000000 pyflutterinstall-1.2.5/pyflutterinstall/trampoline.py
--rw-rw-rw-   0        0        0     1867 2023-02-18 22:32:53.000000 pyflutterinstall-1.2.5/pyflutterinstall/util.py
--rw-rw-rw-   0        0        0     3142 2023-03-24 09:40:09.000000 pyflutterinstall-1.2.5/pyflutterinstall/which_all.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.090636 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/
--rw-rw-rw-   0        0        0     3918 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      447 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-05 06:02:14.000000 pyflutterinstall-1.2.5/pyflutterinstall.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-03-24 09:49:25.000000 pyflutterinstall-1.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 06:02:15.109635 pyflutterinstall-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     3088 2023-04-05 06:00:58.000000 pyflutterinstall-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:02:15.107637 pyflutterinstall-1.2.5/tests/
--rw-rw-rw-   0        0        0      577 2023-03-24 09:54:39.000000 pyflutterinstall-1.2.5/tests/test_cmd_java.py
--rw-rw-rw-   0        0        0     1877 2023-03-24 09:54:39.000000 pyflutterinstall-1.2.5/tests/test_cmds.py
--rw-rw-rw-   0        0        0      367 2023-01-13 13:38:00.000000 pyflutterinstall-1.2.5/tests/test_pyflutterinstall.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.065523 pyflutterinstall-1.2.6/
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-01-27 19:14:46.000000 pyflutterinstall-1.2.6/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)       24 2023-01-27 19:14:46.000000 pyflutterinstall-1.2.6/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     3874 2023-04-26 22:13:34.065315 pyflutterinstall-1.2.6/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     3213 2023-04-25 20:00:58.000000 pyflutterinstall-1.2.6/README.md
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.059477 pyflutterinstall-1.2.6/pyflutterinstall/
+-rw-r--r--   0 niteris    (501) staff       (20)       14 2023-01-27 19:14:46.000000 pyflutterinstall-1.2.6/pyflutterinstall/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     5301 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cli.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.062667 pyflutterinstall-1.2.6/pyflutterinstall/cmds/
+-rw-r--r--   0 niteris    (501) staff       (20)       14 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)      599 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/adb.py
+-rw-r--r--   0 niteris    (501) staff       (20)      607 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/avdmanager.py
+-rw-r--r--   0 niteris    (501) staff       (20)      582 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/emulator.py
+-rw-r--r--   0 niteris    (501) staff       (20)      996 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/gradle.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1056 2023-04-25 18:42:16.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/java.py
+-rw-r--r--   0 niteris    (501) staff       (20)      604 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/cmds/sdkmanager.py
+-rw-r--r--   0 niteris    (501) staff       (20)      998 2023-04-25 18:34:15.000000 pyflutterinstall-1.2.6/pyflutterinstall/config.py
+-rw-r--r--   0 niteris    (501) staff       (20)      546 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/flutter_doctor.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.064273 pyflutterinstall-1.2.6/pyflutterinstall/install/
+-rw-r--r--   0 niteris    (501) staff       (20)       14 2023-01-27 19:14:46.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3778 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/android_sdk.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1619 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/ant_sdk.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1317 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/chrome.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2700 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/flutter_sdk.py
+-rw-r--r--   0 niteris    (501) staff       (20)      979 2023-04-26 21:59:25.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/gradle.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2599 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/install/java_sdk.py
+-rw-r--r--   0 niteris    (501) staff       (20)      522 2023-01-28 00:03:57.000000 pyflutterinstall-1.2.6/pyflutterinstall/outstream.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2124 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/postrun.py
+-rw-r--r--   0 niteris    (501) staff       (20)     4462 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/resources.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2328 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/setenv.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1504 2023-04-26 19:45:45.000000 pyflutterinstall-1.2.6/pyflutterinstall/trampoline.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1867 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/util.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3142 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/pyflutterinstall/which_all.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.060891 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     3874 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     1177 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      447 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/entry_points.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      105 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/requires.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       17 2023-04-26 22:13:34.000000 pyflutterinstall-1.2.6/pyflutterinstall.egg-info/top_level.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       95 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/requirements.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-04-26 22:13:34.065576 pyflutterinstall-1.2.6/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     3088 2023-04-25 19:59:33.000000 pyflutterinstall-1.2.6/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-04-26 22:13:34.065005 pyflutterinstall-1.2.6/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)      577 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/tests/test_cmd_java.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1877 2023-04-25 17:35:31.000000 pyflutterinstall-1.2.6/tests/test_cmds.py
+-rw-r--r--   0 niteris    (501) staff       (20)      367 2023-01-27 19:14:46.000000 pyflutterinstall-1.2.6/tests/test_pyflutterinstall.py
```

### Comparing `pyflutterinstall-1.2.5/LICENSE` & `pyflutterinstall-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/PKG-INFO` & `pyflutterinstall-1.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,90 @@
-Metadata-Version: 2.1
-Name: pyflutterinstall
-Version: 1.2.5
-Summary: Installs the flutter sdk and dependencies
-Home-page: https://github.com/zackees/pyflutterinstall
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# pyflutterinstall
-
-[![Win_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml)
-[![Win_FullInstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml)
-[![MacOS_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml)
-[![MacOS_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml)
-[![Ubuntu_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml)
-[![Ubuntu_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml)
-
-Installs all dependencies for pyflutter/AndroidSDK on Windows.
-
-```bash
-pip install pyflutterinstall
-cd <DIRECTORY YOU WANT TO INSTALL>
-pyflutterinstall
-```
-The SDK will be installed at `FlutterSDK`
-
-Use this tool if you need to:
-  * Install FlutterSDK
-  * -or- Install the AndroidSDK
-  
-Your path will be updated with the dependencies so that you can execute `sdkmanager`, `adb`, `emulator` and the like.
-  
-# Why?
-
-Installing the Android SDK toolchain is **hard**! This tool takes care of all of this for
-Windows/Linux/MacOS and does it in a fully automated way. This is great for reproducabilty of tool chain install across your
-team.
-
-
-#### Versions
-
-  * Android API: 33
-  * Java: 8
-  * Flutter: <TODO>
-
-Usage
-```bash
-> pip install pyflutterinstall
-> pyflutterinstall
-```
-
-# Releases
-  * 1.2.5: Java is now jdk v17 by default
-  * 1.2.4: Java v11.0.2 -> v11.0.18 (fixes OkHttp3 bug)
-  * 1.2.2: Fixes for sdkmanager.
-  * 1.2.1: Fixes for avdmanager.
-  * 1.2.0: Now uses shims for adb, avdmanager, emulator, gradle, java, sdkmanager
-  * 1.1.3: Fix 1.1.2
-  * 1.1.2: Adds --install-dir option to install to a specific directory.
-  * 1.1.1: Expose the post_run testing function to test environments.
-  * 1.1.0: Adds ant install.
-  * 1.0.10: Emulator tools now installed on path.
-  * 1.0.9: adb is now installed on the path.
-  * 1.0.8: Gradle upgrade to 7.5, JDK is downgraded to 9.
-  * 1.0.7: Windows now uses user environment variables to avoid elevated privileges.
-  * 1.0.6: Fix macos install.
-  * 1.0.5: Gradle is now installed as well.
-  * 1.0.3: Uses pexpect to run commands.
-  * 1.0.2: MacOS: now installs cocoapods dependency.
-  * 1.0.1: Update setenvironment to 1.0.9 to get expanded paths.
-  * 1.0.0: Windows, Mac and Linux now supported and all tests pass.
-  * 0.0.2: Automated tests for windows.
-  * 0.0.1: Initial release - windows supported.
-
-# TODO
-  * [ ] Integrate the Windows Universal bridge driver for devices:
-    * https://adb.clockworkmod.com/
+Metadata-Version: 2.1
+Name: pyflutterinstall
+Version: 1.2.6
+Summary: Installs the flutter sdk and dependencies
+Home-page: https://github.com/zackees/pyflutterinstall
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# pyflutterinstall
+
+[![Win_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml)
+[![Win_FullInstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml)
+[![MacOS_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml)
+[![MacOS_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml)
+[![Ubuntu_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml)
+[![Ubuntu_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml)
+
+Installs all dependencies for pyflutter/AndroidSDK on Windows.
+
+```bash
+pip install pyflutterinstall
+cd <DIRECTORY YOU WANT TO INSTALL>
+pyflutterinstall
+```
+The SDK will be installed at `FlutterSDK`
+
+Use this tool if you need to:
+  * Install FlutterSDK
+  * -or- Install the AndroidSDK
+  
+Your path will be updated with the dependencies so that you can execute `sdkmanager`, `adb`, `emulator` and the like.
+  
+# Why?
+
+Installing the Android SDK toolchain is **hard**! This tool takes care of all of this for
+Windows/Linux/MacOS and does it in a fully automated way. This is great for reproducabilty of tool chain install across your
+team.
+
+
+#### Versions
+
+  * Android API: 33
+  * Java: 8
+  * Flutter: <TODO>
+
+Usage
+```bash
+> pip install pyflutterinstall
+> pyflutterinstall
+```
+
+# Releases
+  * 1.2.6: Java trampoline fixed for Mac OSX
+  * 1.2.5: Java is now jdk v17 by default
+  * 1.2.4: Java v11.0.2 -> v11.0.18 (fixes OkHttp3 bug)
+  * 1.2.2: Fixes for sdkmanager.
+  * 1.2.1: Fixes for avdmanager.
+  * 1.2.0: Now uses shims for adb, avdmanager, emulator, gradle, java, sdkmanager
+  * 1.1.3: Fix 1.1.2
+  * 1.1.2: Adds --install-dir option to install to a specific directory.
+  * 1.1.1: Expose the post_run testing function to test environments.
+  * 1.1.0: Adds ant install.
+  * 1.0.10: Emulator tools now installed on path.
+  * 1.0.9: adb is now installed on the path.
+  * 1.0.8: Gradle upgrade to 7.5, JDK is downgraded to 9.
+  * 1.0.7: Windows now uses user environment variables to avoid elevated privileges.
+  * 1.0.6: Fix macos install.
+  * 1.0.5: Gradle is now installed as well.
+  * 1.0.3: Uses pexpect to run commands.
+  * 1.0.2: MacOS: now installs cocoapods dependency.
+  * 1.0.1: Update setenvironment to 1.0.9 to get expanded paths.
+  * 1.0.0: Windows, Mac and Linux now supported and all tests pass.
+  * 0.0.2: Automated tests for windows.
+  * 0.0.1: Initial release - windows supported.
+
+# TODO
+  * [ ] Integrate the Windows Universal bridge driver for devices:
+    * https://adb.clockworkmod.com/
```

### Comparing `pyflutterinstall-1.2.5/README.md` & `pyflutterinstall-1.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 Usage
 ```bash
 > pip install pyflutterinstall
 > pyflutterinstall
 ```
 
 # Releases
+  * 1.2.6: Java trampoline fixed for Mac OSX
   * 1.2.5: Java is now jdk v17 by default
   * 1.2.4: Java v11.0.2 -> v11.0.18 (fixes OkHttp3 bug)
   * 1.2.2: Fixes for sdkmanager.
   * 1.2.1: Fixes for avdmanager.
   * 1.2.0: Now uses shims for adb, avdmanager, emulator, gradle, java, sdkmanager
   * 1.1.3: Fix 1.1.2
   * 1.1.2: Adds --install-dir option to install to a specific directory.
```

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cli.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cli.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/adb.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/adb.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/avdmanager.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/avdmanager.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/emulator.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/emulator.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/gradle.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/gradle.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/java.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/java.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,30 +4,39 @@
 
 import os
 import sys
 
 from pyflutterinstall.config import config_load
 from pyflutterinstall.trampoline import trampoline
 
-JAVA_DIR = config_load().get("JAVA_DIR", "INVALID")
+JAVA_DIR = config_load().get("JAVA_DIR", None)
 
 COMMAND = "java"
 
 
 def find_default_path_or_none() -> str | None:
     """Find default path"""
+    if JAVA_DIR is None:
+        return None
     jdk_folders = os.listdir(JAVA_DIR)
     if not jdk_folders:
         return None
     if len(jdk_folders) > 1:
         jdk_folders.sort()
         jdk_folders.reverse()
-    return os.path.join(JAVA_DIR, jdk_folders[0], "bin")
+    base_java_dir = os.path.join(JAVA_DIR, jdk_folders[0])
+    if sys.platform == "darwin":
+        java_bin = os.path.join(base_java_dir, "Contents", "Home", "bin")
+    else:
+        java_bin = os.path.join(base_java_dir, "bin")
+    return java_bin
 
 
 def main(argv: list[str] | None = None) -> int:
     """Main"""
-    return trampoline(COMMAND, args=argv, default_path=find_default_path_or_none())
+    java_bin = trampoline(COMMAND, args=argv, default_path=find_default_path_or_none())
+    assert os.path.exists(java_bin), f"java_bin {java_bin} does not exist"
+    return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/cmds/sdkmanager.py` & `pyflutterinstall-1.2.6/pyflutterinstall/cmds/sdkmanager.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/config.py` & `pyflutterinstall-1.2.6/pyflutterinstall/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,14 @@
     with open(CONFIG_FILE, encoding="utf-8", mode="r") as filed:
         return json.load(filed)
 
 
 def print_config() -> int:
     """Endpoint for printing the current configuration."""
     config = config_load()
+    print(f"Config file: {CONFIG_FILE}")
     print(json.dumps(config, indent=4))
     return 0
+
+
+if __name__ == "__main__":
+    print_config()
```

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/flutter_doctor.py` & `pyflutterinstall-1.2.6/pyflutterinstall/flutter_doctor.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/install/android_sdk.py` & `pyflutterinstall-1.2.6/pyflutterinstall/install/android_sdk.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/install/ant_sdk.py` & `pyflutterinstall-1.2.6/pyflutterinstall/install/ant_sdk.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/install/chrome.py` & `pyflutterinstall-1.2.6/pyflutterinstall/install/chrome.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/install/flutter_sdk.py` & `pyflutterinstall-1.2.6/pyflutterinstall/install/flutter_sdk.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/install/java_sdk.py` & `pyflutterinstall-1.2.6/pyflutterinstall/install/java_sdk.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/outstream.py` & `pyflutterinstall-1.2.6/pyflutterinstall/outstream.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/postrun.py` & `pyflutterinstall-1.2.6/pyflutterinstall/postrun.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/resources.py` & `pyflutterinstall-1.2.6/pyflutterinstall/resources.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/setenv.py` & `pyflutterinstall-1.2.6/pyflutterinstall/setenv.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/trampoline.py` & `pyflutterinstall-1.2.6/pyflutterinstall/trampoline.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,12 +36,12 @@
         paths = which_all(command, filter_package_exes=True)
         if paths:
             cmd_list = [paths[0]] + args
             if "--which" in sys.argv:
                 print("Real tool is at:", paths[0])
                 return 0
             return subprocess.call(cmd_list, env=env)
-        print(f"{command} not installed on system paths.")
+        print(f"Trampoline {command} could not find the real {command} installed on the system paths.")
         return 1
     finally:
         if prev_path:
             os.environ["PATH"] = prev_path
```

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/util.py` & `pyflutterinstall-1.2.6/pyflutterinstall/util.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall/which_all.py` & `pyflutterinstall-1.2.6/pyflutterinstall/which_all.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall.egg-info/PKG-INFO` & `pyflutterinstall-1.2.6/pyflutterinstall.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,90 @@
-Metadata-Version: 2.1
-Name: pyflutterinstall
-Version: 1.2.5
-Summary: Installs the flutter sdk and dependencies
-Home-page: https://github.com/zackees/pyflutterinstall
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# pyflutterinstall
-
-[![Win_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml)
-[![Win_FullInstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml)
-[![MacOS_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml)
-[![MacOS_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml)
-[![Ubuntu_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml)
-[![Ubuntu_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml)
-
-Installs all dependencies for pyflutter/AndroidSDK on Windows.
-
-```bash
-pip install pyflutterinstall
-cd <DIRECTORY YOU WANT TO INSTALL>
-pyflutterinstall
-```
-The SDK will be installed at `FlutterSDK`
-
-Use this tool if you need to:
-  * Install FlutterSDK
-  * -or- Install the AndroidSDK
-  
-Your path will be updated with the dependencies so that you can execute `sdkmanager`, `adb`, `emulator` and the like.
-  
-# Why?
-
-Installing the Android SDK toolchain is **hard**! This tool takes care of all of this for
-Windows/Linux/MacOS and does it in a fully automated way. This is great for reproducabilty of tool chain install across your
-team.
-
-
-#### Versions
-
-  * Android API: 33
-  * Java: 8
-  * Flutter: <TODO>
-
-Usage
-```bash
-> pip install pyflutterinstall
-> pyflutterinstall
-```
-
-# Releases
-  * 1.2.5: Java is now jdk v17 by default
-  * 1.2.4: Java v11.0.2 -> v11.0.18 (fixes OkHttp3 bug)
-  * 1.2.2: Fixes for sdkmanager.
-  * 1.2.1: Fixes for avdmanager.
-  * 1.2.0: Now uses shims for adb, avdmanager, emulator, gradle, java, sdkmanager
-  * 1.1.3: Fix 1.1.2
-  * 1.1.2: Adds --install-dir option to install to a specific directory.
-  * 1.1.1: Expose the post_run testing function to test environments.
-  * 1.1.0: Adds ant install.
-  * 1.0.10: Emulator tools now installed on path.
-  * 1.0.9: adb is now installed on the path.
-  * 1.0.8: Gradle upgrade to 7.5, JDK is downgraded to 9.
-  * 1.0.7: Windows now uses user environment variables to avoid elevated privileges.
-  * 1.0.6: Fix macos install.
-  * 1.0.5: Gradle is now installed as well.
-  * 1.0.3: Uses pexpect to run commands.
-  * 1.0.2: MacOS: now installs cocoapods dependency.
-  * 1.0.1: Update setenvironment to 1.0.9 to get expanded paths.
-  * 1.0.0: Windows, Mac and Linux now supported and all tests pass.
-  * 0.0.2: Automated tests for windows.
-  * 0.0.1: Initial release - windows supported.
-
-# TODO
-  * [ ] Integrate the Windows Universal bridge driver for devices:
-    * https://adb.clockworkmod.com/
+Metadata-Version: 2.1
+Name: pyflutterinstall
+Version: 1.2.6
+Summary: Installs the flutter sdk and dependencies
+Home-page: https://github.com/zackees/pyflutterinstall
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# pyflutterinstall
+
+[![Win_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win.yml)
+[![Win_FullInstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_win_fullinstall.yml)
+[![MacOS_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos.yml)
+[![MacOS_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_macos_fullinstall.yml)
+[![Ubuntu_Tests](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu.yml)
+[![Ubuntu_Fullinstall](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml/badge.svg)](https://github.com/zackees/pyflutterinstall/actions/workflows/push_ubuntu_fullinstall.yml)
+
+Installs all dependencies for pyflutter/AndroidSDK on Windows.
+
+```bash
+pip install pyflutterinstall
+cd <DIRECTORY YOU WANT TO INSTALL>
+pyflutterinstall
+```
+The SDK will be installed at `FlutterSDK`
+
+Use this tool if you need to:
+  * Install FlutterSDK
+  * -or- Install the AndroidSDK
+  
+Your path will be updated with the dependencies so that you can execute `sdkmanager`, `adb`, `emulator` and the like.
+  
+# Why?
+
+Installing the Android SDK toolchain is **hard**! This tool takes care of all of this for
+Windows/Linux/MacOS and does it in a fully automated way. This is great for reproducabilty of tool chain install across your
+team.
+
+
+#### Versions
+
+  * Android API: 33
+  * Java: 8
+  * Flutter: <TODO>
+
+Usage
+```bash
+> pip install pyflutterinstall
+> pyflutterinstall
+```
+
+# Releases
+  * 1.2.6: Java trampoline fixed for Mac OSX
+  * 1.2.5: Java is now jdk v17 by default
+  * 1.2.4: Java v11.0.2 -> v11.0.18 (fixes OkHttp3 bug)
+  * 1.2.2: Fixes for sdkmanager.
+  * 1.2.1: Fixes for avdmanager.
+  * 1.2.0: Now uses shims for adb, avdmanager, emulator, gradle, java, sdkmanager
+  * 1.1.3: Fix 1.1.2
+  * 1.1.2: Adds --install-dir option to install to a specific directory.
+  * 1.1.1: Expose the post_run testing function to test environments.
+  * 1.1.0: Adds ant install.
+  * 1.0.10: Emulator tools now installed on path.
+  * 1.0.9: adb is now installed on the path.
+  * 1.0.8: Gradle upgrade to 7.5, JDK is downgraded to 9.
+  * 1.0.7: Windows now uses user environment variables to avoid elevated privileges.
+  * 1.0.6: Fix macos install.
+  * 1.0.5: Gradle is now installed as well.
+  * 1.0.3: Uses pexpect to run commands.
+  * 1.0.2: MacOS: now installs cocoapods dependency.
+  * 1.0.1: Update setenvironment to 1.0.9 to get expanded paths.
+  * 1.0.0: Windows, Mac and Linux now supported and all tests pass.
+  * 0.0.2: Automated tests for windows.
+  * 0.0.1: Initial release - windows supported.
+
+# TODO
+  * [ ] Integrate the Windows Universal bridge driver for devices:
+    * https://adb.clockworkmod.com/
```

### Comparing `pyflutterinstall-1.2.5/pyflutterinstall.egg-info/SOURCES.txt` & `pyflutterinstall-1.2.6/pyflutterinstall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/setup.py` & `pyflutterinstall-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 NAME = "pyflutterinstall"
 DESCRIPTION = "Installs the flutter sdk and dependencies"
 URL = "https://github.com/zackees/pyflutterinstall"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9"
-VERSION = "1.2.5"
+VERSION = "1.2.6"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fd:
     LONG_DESCRIPTION = fd.read()
 
 with open(os.path.join(HERE, "requirements.txt")) as fd:
     REQUIREMENTS = [line.strip() for line in fd.readlines() if line.strip()]
@@ -76,26 +76,25 @@
         "Programming Language :: Python :: 3.9",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Environment :: Console",
     ],
     install_requires=REQUIREMENTS,
-
     entry_points={
         "console_scripts": [
             "pyflutterinstall = pyflutterinstall.cli:main",
             "pyflutteractivate = pyflutterinstall.setenv:init_dotenv",
             "pyflutterprintconfig = pyflutterinstall.config:print_config",
             "sdkmanager = pyflutterinstall.cmds.sdkmanager:main",
             "avdmanager = pyflutterinstall.cmds.avdmanager:main",
             "adb = pyflutterinstall.cmds.adb:main",
             "gradle = pyflutterinstall.cmds.gradle:main",
             "emulator = pyflutterinstall.cmds.emulator:main",
-            "java = pyflutterinstall.cmds.java:main"
+            "java = pyflutterinstall.cmds.java:main",
         ],
     },
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     package_data={},
     include_package_data=True,
     extras_require={
         "test": ["pytest"],
```

### Comparing `pyflutterinstall-1.2.5/tests/test_cmd_java.py` & `pyflutterinstall-1.2.6/tests/test_cmd_java.py`

 * *Files identical despite different names*

### Comparing `pyflutterinstall-1.2.5/tests/test_cmds.py` & `pyflutterinstall-1.2.6/tests/test_cmds.py`

 * *Files identical despite different names*


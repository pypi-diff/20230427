# Comparing `tmp/buildapp-1.1.0.tar.gz` & `tmp/buildapp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildapp-1.1.0.tar", last modified: Mon Apr 10 21:08:37 2023, max compression
+gzip compressed data, was "buildapp-1.1.1.tar", last modified: Thu Apr 27 18:48:41 2023, max compression
```

## Comparing `buildapp-1.1.0.tar` & `buildapp-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.641981 buildapp-1.1.0/
--rw-rw-rw-   0        0        0      153 2023-04-10 21:08:37.640973 buildapp-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2503 2023-04-10 19:54:01.000000 buildapp-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.622974 buildapp-1.1.0/buildapp/
--rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.1.0/buildapp/__init__.py
--rw-rw-rw-   0        0        0     3419 2023-04-10 21:01:25.000000 buildapp-1.1.0/buildapp/buildapp.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:08:37.639022 buildapp-1.1.0/buildapp.egg-info/
--rw-rw-rw-   0        0        0      153 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 21:08:37.000000 buildapp-1.1.0/buildapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:08:37.641981 buildapp-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      349 2023-04-10 21:04:15.000000 buildapp-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.092253 buildapp-1.1.1/
+-rw-rw-rw-   0        0        0      153 2023-04-27 18:48:41.092253 buildapp-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2567 2023-04-11 09:31:12.000000 buildapp-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.076629 buildapp-1.1.1/buildapp/
+-rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.1.1/buildapp/__init__.py
+-rw-rw-rw-   0        0        0     3381 2023-04-27 06:46:32.000000 buildapp-1.1.1/buildapp/buildapp.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.092253 buildapp-1.1.1/buildapp.egg-info/
+-rw-rw-rw-   0        0        0      153 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:48:41.092253 buildapp-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-04-27 18:46:12.000000 buildapp-1.1.1/setup.py
```

### Comparing `buildapp-1.1.0/README.md` & `buildapp-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Corss-Platform script used to recompile APK that was decompiled by apktool <br/>
 That way, you can decompile an application, patch it's smali-source / resources / manifest / libs / ... <br />
 And rebuild it into a new apk you may install in your devices <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only!
 
 ## Installation
-Simply
-> pip install buildapp
+After having all [requirements](#Requirements), simply
+> pip install buildapp --upgrade
 
-Make sure to have python scripts folder in your path,
+Make sure to have python scripts folder in your path, <br/>
 And use the correct version of pip for python3
 
 ## Decompilation process
 Use [`apktool`](https://ibotpeaches.github.io/Apktool/install/) to decompile your application.
 
 Apktool decompilation syntax:
 > apktool d <apk_path> -o <output_folder>
```

### Comparing `buildapp-1.1.0/buildapp/buildapp.py` & `buildapp-1.1.1/buildapp/buildapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import argparse
 import subprocess
 
 KEYSTORE_ALIAS = 'defkeystorealias'
 KEYSTORE_PASSWORD = 'defkeystorepass'
-KEYSTORE_PATH = os.path.expanduser('~/buildapp-keystore.jks')
+KEYSTORE_PATH = os.path.expanduser('~/.buildapp-keystore.jks')
 
 
 class CompileApp:
     def __init__(self, decompiled_path, output_apk_path):
         self.prealigned_file = f'{output_apk_path}_prealign'
         self.decompiled_path = decompiled_path
 
@@ -45,15 +45,15 @@
         run_process(f'apksigner sign --ks-key-alias {KEYSTORE_ALIAS} --ks {KEYSTORE_PATH} {output_apk_path}', input_string=f'{KEYSTORE_PASSWORD}\n')
 
     def __del__(self):
         os.unlink(f'{self.output_apk_path}.idsig')
 
 class InstallApk:
     def __init__(self, apk_path):
-        run_process(f'adb install {apk_path}')
+        run_process(f'adb install -r {apk_path}')
 
 
 def run_process(cmdline, input_string='', ignore_stderr=False):
     print(f'Executing `{cmdline}`')
 
     subprocess.run(
         cmdline,
@@ -77,21 +77,19 @@
 
 def build_app(output_apk_path, decompiled_folder, keystore_path=None, install_after_build=False):
     with CompileApp(decompiled_folder, output_apk_path):
         AlignApk(output_apk_path)
         ObtainKeystore(keystore_path)
         SignApk(output_apk_path)
 
-        print('Compiled successfully!')
-
         if install_after_build:
             InstallApk(output_apk_path)
-            print('Installed successfully!')
 
 
 def main():
     args = parse_arguments()
     build_app(args.output_apk_path, args.decompiled_path, args.keystore_path, args.install)
 
+    print('buildapp completed successfully!')
 
 if __name__ == "__main__":
     main()
```


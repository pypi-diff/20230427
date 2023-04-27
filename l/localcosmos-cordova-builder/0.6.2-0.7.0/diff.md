# Comparing `tmp/localcosmos_cordova_builder-0.6.2.tar.gz` & `tmp/localcosmos_cordova_builder-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_cordova_builder-0.6.2.tar", last modified: Tue Feb 28 19:09:01 2023, max compression
+gzip compressed data, was "localcosmos_cordova_builder-0.7.0.tar", last modified: Thu Apr 27 08:10:41 2023, max compression
```

## Comparing `localcosmos_cordova_builder-0.6.2.tar` & `localcosmos_cordova_builder-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/
--rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/
--rw-r--r--   0 tom       (1000) tom       (1000)     8690 2023-01-31 15:32:09.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/AppImageCreator.py
--rw-r--r--   0 tom       (1000) tom       (1000)    29703 2023-02-28 18:25:16.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/CordovaAppBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    19752 2023-01-31 15:32:09.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/JobManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/MetaAppDefinition.py
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4257 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/image_utils.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/logger.py
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/required_assets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 19:09:01.082448 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/resources/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/resources/images/
--rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/urllib_request_upload_files.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-02-28 19:09:01.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      862 2023-02-28 19:09:01.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-02-28 19:09:01.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-02-28 19:09:01.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       28 2023-02-28 19:09:01.000000 localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-02-28 19:09:01.086448 localcosmos_cordova_builder-0.6.2/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1007 2023-02-28 19:08:42.000000 localcosmos_cordova_builder-0.6.2/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.676923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9443 2023-04-26 15:54:18.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/AppImageCreator.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31637 2023-04-26 16:14:22.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/CordovaAppBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    19752 2023-01-31 15:32:09.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/JobManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/MetaAppDefinition.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4257 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/image_utils.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/logger.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/required_assets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.672923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4077 2023-04-26 15:23:50.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/urllib_request_upload_files.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.676923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      927 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       28 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1007 2023-04-27 08:10:06.000000 localcosmos_cordova_builder-0.7.0/setup.py
```

### Comparing `localcosmos_cordova_builder-0.6.2/LICENSE` & `localcosmos_cordova_builder-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/PKG-INFO` & `localcosmos_cordova_builder-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_cordova_builder
-Version: 0.6.2
+Version: 0.7.0
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/AppImageCreator.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/AppImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # - varying dimensions: use the shorter side to create png, cut afterwards
 # - the extension might differ from the existing_image_diskpath
 # - android adaptive launchers (foreground + background)
 
 
 FALLBACK_IMAGES = {
     'appLauncherBackground' : 'resources/images/adaptive_launcher_background.svg', # relative to this file
+    'appLauncherIcon' : 'resources/images/appLauncherIcon.svg', # relative to this file
 }
 
 
 class AppImageCreator:
 
     def __init__(self, meta_app_definition, app_cordova_folder, app_build_sources_path):
         
@@ -140,21 +141,21 @@
         'appLauncherBackground' : {
             'subfolders_startwith' : 'mipmap-',
             'folder' : 'platforms/android/app/src/main/res',
             'filenames' : ['ic_launcher_background.png'],
             'varying_ratios' : False,
             'remove_alpha_channel' : False,
         },
-        'appSplashscreen' : {
-            'subfolders_startwith' : 'drawable-',
-            'folder' : 'platforms/android/app/src/main/res',
-            'filenames' : ['screen.png'],
-            'varying_ratios' : True,
-            'remove_alpha_channel' : False,
-        }
+        #'appSplashscreen' : {
+        #    'subfolders_startwith' : 'drawable-',
+        #    'folder' : 'platforms/android/app/src/main/res',
+        #    'filenames' : ['screen.png'],
+        #    'varying_ratios' : True,
+        #    'remove_alpha_channel' : False,
+        #}
     }
 
 
     def iterate_over_default_image_files(self, image_type):
         icon_parent_folder = os.path.join(self.app_cordova_folder, self.definitions[image_type]['folder'])
         
         # iterate over all subfolders named mipmap-*
@@ -239,7 +240,30 @@
             target_image_filepath = os.path.join(screen_folder, storyboard_filename)
             width = size[0]
             height = size[1]
             
             create_resized_png_from_svg(source_image_filepath, width, height, target_image_filepath)
         
         
+class BrowserAppImageCreator(AppImageCreator):
+
+    def create_favicon(self):
+
+        launcher_source = self._get_source_image_diskpath('appLauncherIcon')
+
+        app_www_folder = os.path.join(self.app_cordova_folder, 'www')
+
+        ico_target_path = os.path.join(app_www_folder, 'lcfavicon.ico')
+
+        largest_size = 48
+
+        png_filename = 'ico_{0}.png'.format(largest_size)
+        destination_filepath = os.path.join(app_www_folder, png_filename)
+
+        create_png_from_svg(launcher_source, largest_size, largest_size, destination_filepath)
+
+        icon = Image.open(destination_filepath)
+
+        icon.save(ico_target_path, format='ICO')
+
+
+
```

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/CordovaAppBuilder.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/CordovaAppBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from localcosmos_cordova_builder.logger import get_logger
 
 # WORKDIR is the directory where node_modules and the cordova binary are installed
 WORKDIR = os.getenv('LOCALCOSMOS_CORDOVA_BUILDER_WORKDIR', None)
 if not WORKDIR:
     raise ValueError('LOCALCOSMOS_CORDOVA_BUILDER_WORKDIR environment variable not found')
 
-CORDOVA_CLI_VERSION = '11.0.0'
+CORDOVA_CLI_VERSION = '11.1.0'
 
 DEFAULT_CORDOVA_PLATFORM_VERSIONS = {
     "android" : "android@11.0.0",
-    "ios" : "ios@6.2.0",
+    "ios" : "ios@6.3.0",
     "browser" : "browser@6.0.0",
 }
 
 PLATFORM_IOS = 'ios'
 PLATFORM_ANDROID = 'android'
 PLATFORM_BROWSER = 'browser'
 
@@ -25,15 +25,15 @@
     pass
 
 
 import subprocess, os, shutil, zipfile, json
 from subprocess import CalledProcessError, PIPE
 
 
-from .AppImageCreator import AndroidAppImageCreator, IOSAppImageCreator
+from .AppImageCreator import AndroidAppImageCreator, IOSAppImageCreator, BrowserAppImageCreator
 
 from lxml import etree
 
 
 '''
     has to be independant from django model instances and app builder instances, as it also runs on a mac
 
@@ -103,31 +103,48 @@
         return self.meta_app_definition.package_name
 
     # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/sources/www
     @property
     def _app_build_sources_www_path(self):
         return os.path.join(self._app_build_sources_path, 'www')
 
+    # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/sources/www
+    @property
+    def _app_build_sources_cordova_assets_path(self):
+        return os.path.join(self._app_build_sources_path, 'cordova')
+
     # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/cordova/{package_name}/
     @property
     def _app_cordova_path(self):
         return os.path.join(self._cordova_build_path, self._app_folder_name)
 
     # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/cordova/{package_name}/www/
     @property
     def _cordova_www_path(self):
         return os.path.join(self._app_cordova_path, 'www')
 
+    # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/cordova/{package_name}/config.xml
     @property
     def config_xml_path(self):
         return os.path.join(self._app_cordova_path, 'config.xml')
 
+    # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/sources/cordova/config.xml
     @property
     def _custom_config_xml_path(self):
-        return os.path.join(self._app_build_sources_path, 'config.xml')
+        return os.path.join(self._app_build_sources_cordova_assets_path, 'config.xml')
+
+    # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/sources/cordova/res
+    @property
+    def _app_cordova_res_source_folder_path(self):
+        return os.path.join(self._app_build_sources_cordova_assets_path, 'res')
+
+    # {settings.APP_KIT_ROOT}/{meta_app.uuid}/{meta_app.current_version}/release/cordova/{package_name}/res/
+    @property
+    def _cordova_res_folder_path(self):
+        return os.path.join(self._app_cordova_path, 'res')
 
     # installing the cordova CLI
     def load_cordova(self):
 
         self.logger.info('Loading cordova environment')
 
         # setup cordova
@@ -263,15 +280,15 @@
         # add stuff to config
         # <preference name="SplashMaintainAspectRatio" value="true" />
         # <preference name="StatusBarStyle" value="blackopaque" />
         # <preference name="StatusBarOverlaysWebView" value="false" />
         # <preference name="StatusBarBackgroundColor" value="#000000" />
 
         preferences = [
-            {'name' : 'SplashMaintainAspectRatio', 'value' : 'true'},
+            #{'name' : 'SplashMaintainAspectRatio', 'value' : 'true'},
             {'name' : 'StatusBarStyle', 'value' : 'blackopaque'},
             {'name' : 'StatusBarOverlaysWebView', 'value' : 'false'},
             {'name' : 'StatusBarBackgroundColor', 'value' : '#000000'},
             {'name' : 'DisallowOverscroll', 'value': 'true'},
         ]
 
         for tag_attributes in preferences:
@@ -358,14 +375,27 @@
 
         root.set('version', version_string)
         
         with open(self.config_xml_path, 'wb') as config_file:
             config_xml_tree.write(config_file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
 
+    def _copy_cordova_res_folder(self):
+
+        if os.path.isdir(self._app_cordova_res_source_folder_path):
+
+            if not os.path.isdir(self._cordova_res_folder_path):
+                self.logger.info('Copying res folder: {0} to {1}'.format(self._app_cordova_res_source_folder_path, self._cordova_res_folder_path))
+                shutil.copytree(self._app_cordova_res_source_folder_path, self._cordova_res_folder_path)
+            else:
+                self.logger.info('res folder already present, not copying res folder.')
+        else:
+            self.logger.info('No res folder found, not copying res folder.')
+
+
     ##############################################################################################################
     # BUILD CONFIG
     ##############################################################################################################
     def _get_build_config_path(self):
         return os.path.join(WORKDIR, 'build_config.json')
 
             
@@ -383,14 +413,16 @@
 
         self.load_cordova()
 
         self._build_blank_cordova_app(rebuild=rebuild)
 
         self._update_config_xml()
 
+        self._copy_cordova_res_folder()
+
         self._install_cordova_plugins()
 
         # set app version
         self.set_config_xml_app_version(self.meta_app_definition.current_version, self.build_number)
 
         platform_version = self._get_cordova_platform_version(PLATFORM_ANDROID)
 
@@ -404,15 +436,15 @@
         if add_android_completed_process.returncode != 0:
             raise CordovaBuildError(add_android_completed_process.stderr)
         
         # replace cordova default www with android www
         self._add_cordova_www_folder()
 
         # build android images
-        self.logger.info('building Android launcher and splashscreen images')
+        self.logger.info('building Android launcher images')
         image_creator = AndroidAppImageCreator(self.meta_app_definition, self._app_cordova_path,
                                                 self._app_build_sources_path)
         
         for image_type, image_filename in REQUIRED_ASSETS.items():
             image_creator.generate_images_from_svg(image_type)
         
 
@@ -671,14 +703,16 @@
 
         self.load_cordova()
 
         self._build_blank_cordova_app(rebuild=rebuild)
 
         self._update_config_xml()
 
+        self._copy_cordova_res_folder()
+
         self._install_cordova_plugins()
 
         # set app version
         self.set_config_xml_app_version(self.meta_app_definition.current_version, self.build_number)
 
         self.logger.info('Adding browser platform')
         platform_version = self._get_cordova_platform_version(PLATFORM_BROWSER)
@@ -689,14 +723,21 @@
 
         if add_browser_completed_process.returncode != 0:
             raise CordovaBuildError(add_browser_completed_process.stderr)
 
         # replace cordova default www with android www
         self._add_cordova_www_folder()
 
+        # add ico
+        self.logger.info('Creating favicon')
+        image_creator = BrowserAppImageCreator(self.meta_app_definition, self._app_cordova_path,
+                                                self._app_build_sources_path)
+
+        image_creator.create_favicon()
+
         # build ios release
         self.logger.info('initiating cordova build browser')
 
         build_browser_command = [self.cordova_bin, 'build', 'browser', '--release']
 
         build_browser_process_completed = subprocess.run(build_browser_command, stdout=PIPE, stderr=PIPE,
                                                      cwd=self._app_cordova_path)
```

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/JobManager.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/JobManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/MetaAppDefinition.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/MetaAppDefinition.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/image_utils.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/image_utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/logger.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/logger.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder/urllib_request_upload_files.py` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/urllib_request_upload_files.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/PKG-INFO` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos-cordova-builder
-Version: 0.6.2
+Version: 0.7.0
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.6.2/localcosmos_cordova_builder.egg-info/SOURCES.txt` & `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 localcosmos_cordova_builder/urllib_request_upload_files.py
 localcosmos_cordova_builder.egg-info/PKG-INFO
 localcosmos_cordova_builder.egg-info/SOURCES.txt
 localcosmos_cordova_builder.egg-info/dependency_links.txt
 localcosmos_cordova_builder.egg-info/requires.txt
 localcosmos_cordova_builder.egg-info/top_level.txt
 localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
-localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
+localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
+localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
```

### Comparing `localcosmos_cordova_builder-0.6.2/setup.py` & `localcosmos_cordova_builder-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'lxml>=4.3.4',
     'tendo',
     'Pillow',
 ]
 
 setup(
     name='localcosmos_cordova_builder',
-    version='0.6.2',
+    version='0.7.0',
     description='Create android and ios app packages for Local Cosmos apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='localcosmos, app kit, cordova builder',
     author='Thomas Uher',
```


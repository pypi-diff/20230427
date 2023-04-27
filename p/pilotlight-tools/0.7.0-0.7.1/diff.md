# Comparing `tmp/pilotlight_tools-0.7.0.tar.gz` & `tmp/pilotlight_tools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilotlight_tools-0.7.0.tar", last modified: Fri Apr 21 03:53:16 2023, max compression
+gzip compressed data, was "pilotlight_tools-0.7.1.tar", last modified: Wed Apr 26 14:44:17 2023, max compression
```

## Comparing `pilotlight_tools-0.7.0.tar` & `pilotlight_tools-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/
--rw-rw-rw-   0        0        0     1087 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     3766 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2721 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/pilotlight_tools/
--rw-rw-rw-   0        0        0        7 2023-04-21 03:52:55.000000 pilotlight_tools-0.7.0/pilotlight_tools/__init__.py
--rw-rw-rw-   0        0        0   103746 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/pilotlight_tools/pl_build.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/
--rw-rw-rw-   0        0        0     3766 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       96 2023-04-21 03:52:55.000000 pilotlight_tools-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1811 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:44:17.092717 pilotlight_tools-0.7.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 14:43:32.000000 pilotlight_tools-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     3766 2023-04-26 14:44:17.092717 pilotlight_tools-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2721 2023-04-26 14:43:32.000000 pilotlight_tools-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 14:44:17.092717 pilotlight_tools-0.7.1/pilotlight_tools/
+-rw-rw-rw-   0        0        0        7 2023-04-26 14:44:02.000000 pilotlight_tools-0.7.1/pilotlight_tools/__init__.py
+-rw-rw-rw-   0        0        0   104506 2023-04-26 14:43:32.000000 pilotlight_tools-0.7.1/pilotlight_tools/pl_build.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:44:17.092717 pilotlight_tools-0.7.1/pilotlight_tools.egg-info/
+-rw-rw-rw-   0        0        0     3766 2023-04-26 14:44:17.000000 pilotlight_tools-0.7.1/pilotlight_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-26 14:44:17.000000 pilotlight_tools-0.7.1/pilotlight_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:44:17.000000 pilotlight_tools-0.7.1/pilotlight_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-26 14:44:17.000000 pilotlight_tools-0.7.1/pilotlight_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       96 2023-04-26 14:44:02.000000 pilotlight_tools-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:44:17.092717 pilotlight_tools-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2023-04-26 14:43:32.000000 pilotlight_tools-0.7.1/setup.py
```

### Comparing `pilotlight_tools-0.7.0/LICENSE` & `pilotlight_tools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pilotlight_tools-0.7.0/PKG-INFO` & `pilotlight_tools-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight_tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.7.0 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.7.1 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pilotlight_tools-0.7.0/README.md` & `pilotlight_tools-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pilotlight_tools-0.7.0/pilotlight_tools/pl_build.py` & `pilotlight_tools-0.7.1/pilotlight_tools/pl_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 ###############################################################################
 #                                  Info                                       #
 ###############################################################################
 
 # very poorly written & dirty system, to be cleaned up later
 
@@ -628,15 +628,15 @@
                 for plat in config._platforms:
                     for settings in plat._compiler_settings:   
                         if settings._output_binary_extension is None:
                             if target._target_type == TargetType.STATIC_LIBRARY:
                                 if settings._compiler_type == CompilerType.MSVC:
                                     settings._output_binary_extension = ".lib"
                                 else :
-                                    settings._output_binary_extension = ".o"
+                                    settings._output_binary_extension = ".a"
                             elif target._target_type == TargetType.DYNAMIC_LIBRARY:
                                 if settings._compiler_type == CompilerType.MSVC:
                                     settings._output_binary_extension = ".dll"
                                 elif settings._compiler_type == CompilerType.CLANG:
                                     settings._output_binary_extension = ".dylib"
                                 else :
                                     settings._output_binary_extension = ".so"
@@ -882,28 +882,31 @@
                                                         for target2 in project._targets:
                                                             if target2._name == _target_link:
                                                                 for config2 in target2._configurations:
                                                                     if config2._name == config._name:
                                                                         for platform2 in config2._platforms:
                                                                             if platform2._platform_type == PlatformType.MACOS:
                                                                                 for settings2 in platform2._compiler_settings:
-                                                                                    settings._source_files.append(settings2._output_directory + "/" + settings2._output_binary + ".o")
+                                                                                    settings._source_files.append(settings2._output_directory + "/" + settings2._output_binary + ".a")
 
                                                 if target._target_type == TargetType.STATIC_LIBRARY:
                     
                                                     buffer += '# run compiler only\n'
                                                     buffer += "echo\n"
                                                     buffer += 'echo ${YELLOW}Step: ' + target._name +'${NC}\n'
                                                     buffer += 'echo ${YELLOW}~~~~~~~~~~~~~~~~~~~${NC}\n'
                                                     buffer += 'echo ${CYAN}Compiling...${NC}\n'
                                                 
                                                     buffer += '\n# each file must be compiled separately\n'
                                                     for source in settings._source_files:
                                                         source_as_path = PurePath(source)
                                                         buffer += 'clang -c -fPIC $PL_INCLUDE_DIRECTORIES $PL_DEFINES $PL_COMPILER_FLAGS ' + source + ' -o "./' + settings._output_directory + '/' + source_as_path.stem + '.o"\n'
+                                                    buffer += '\n# combine object files into a static lib\n'
+                                                    buffer += 'ar rcs ./' + settings._output_directory + '/' + settings._output_binary + '.a ./' + settings._output_directory + '/*.o\n'
+                                                    buffer += 'rm ./' + settings._output_directory + '/*.o\n'
 
                                                 elif target._target_type == TargetType.DYNAMIC_LIBRARY:
 
                                                     buffer += '# source files\n'
                                                     if project._collapse:
                                                         buffer += 'PL_SOURCES="'    
                                                         for source in settings._source_files:
@@ -1187,29 +1190,31 @@
                                                         for target2 in project._targets:
                                                             if target2._name == _target_link:
                                                                 for config2 in target2._configurations:
                                                                     if config2._name == config._name:
                                                                         for platform2 in config2._platforms:
                                                                             if platform2._platform_type == PlatformType.LINUX:
                                                                                 for settings2 in platform2._compiler_settings:
-                                                                                    settings._source_files.append(settings2._output_directory + "/" + settings2._output_binary + ".o")
+                                                                                    settings._source_files.append(settings2._output_directory + "/" + settings2._output_binary + ".a")
                                                 
                                                 if target._target_type == TargetType.STATIC_LIBRARY:
                     
                                                     buffer += '# run compiler only\n'
                                                     buffer += "echo\n"
                                                     buffer += 'echo ${YELLOW}Step: ' + target._name +'${NC}\n'
                                                     buffer += 'echo ${YELLOW}~~~~~~~~~~~~~~~~~~~${NC}\n'
                                                     buffer += 'echo ${CYAN}Compiling...${NC}\n'
                                                 
                                                     buffer += '\n# each file must be compiled separately\n'
                                                     for source in settings._source_files:
                                                         source_as_path = PurePath(source)
                                                         buffer += 'gcc -c -fPIC $PL_INCLUDE_DIRECTORIES $PL_DEFINES $PL_COMPILER_FLAGS ' + source + ' -o "./' + settings._output_directory + '/' + source_as_path.stem + '.o"\n'
-                                                    
+                                                    buffer += '\n# combine object files into a static lib\n'
+                                                    buffer += 'ar rcs ./' + settings._output_directory + '/' + settings._output_binary + '.a ./' + settings._output_directory + '/*.o\n'
+                                                    buffer += 'rm ./' + settings._output_directory + '/*.o\n'
                                                 elif target._target_type == TargetType.DYNAMIC_LIBRARY:
 
                                                     buffer += '# source files\n'
                                                     if project._collapse:
                                                         buffer += 'PL_SOURCES="'    
                                                         for source in settings._source_files:
                                                             buffer += source + ' '
```

### Comparing `pilotlight_tools-0.7.0/pilotlight_tools.egg-info/PKG-INFO` & `pilotlight_tools-0.7.1/pilotlight_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.7.0 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.7.1 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pilotlight_tools-0.7.0/setup.py` & `pilotlight_tools-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from codecs import open
 import os
 
-wip_version = "0.6.1"
+wip_version = "0.7.1"
 
 def version_number():
     """This function reads the version number which is populated by github actions"""
 
     if os.environ.get('READTHEDOCS') == 'True':
         return wip_version
     try:
```


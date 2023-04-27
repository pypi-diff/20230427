# Comparing `tmp/optilibre-1.2.0.tar.gz` & `tmp/optilibre-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optilibre-1.2.0.tar", last modified: Thu Apr 27 07:42:14 2023, max compression
+gzip compressed data, was "optilibre-1.2.1.tar", last modified: Thu Apr 27 08:34:51 2023, max compression
```

## Comparing `optilibre-1.2.0.tar` & `optilibre-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911842 optilibre-1.2.0/
--rw-r--r--   0 sydney     (501) staff       (20)      126 2023-04-26 14:48:40.000000 optilibre-1.2.0/.gitignore
--rw-r--r--   0 sydney     (501) staff       (20)      159 2023-04-26 15:01:42.000000 optilibre-1.2.0/CHANGELOG.md
--rw-r--r--   0 sydney     (501) staff       (20)    34454 2022-05-22 13:42:28.000000 optilibre-1.2.0/LICENSE
--rw-r--r--   0 sydney     (501) staff       (20)      190 2023-04-26 14:46:30.000000 optilibre-1.2.0/Makefile
--rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 07:42:14.911950 optilibre-1.2.0/PKG-INFO
--rw-r--r--   0 sydney     (501) staff       (20)     1655 2022-05-22 13:42:28.000000 optilibre-1.2.0/README.md
--rw-r--r--   0 sydney     (501) staff       (20)      409 2022-05-30 08:28:22.000000 optilibre-1.2.0/optilibre.example.conf
--rw-r--r--   0 sydney     (501) staff       (20)      908 2022-05-31 08:48:39.000000 optilibre-1.2.0/optilibre.example.toml
--rw-r--r--   0 sydney     (501) staff       (20)      469 2023-04-26 15:06:54.000000 optilibre-1.2.0/pyproject.toml
--rw-r--r--   0 sydney     (501) staff       (20)       31 2022-05-22 13:42:28.000000 optilibre-1.2.0/requirements.txt
--rw-r--r--   0 sydney     (501) staff       (20)      654 2023-04-27 07:42:14.912266 optilibre-1.2.0/setup.cfg
--rwxr-xr-x   0 sydney     (501) staff       (20)      497 2022-05-22 13:42:28.000000 optilibre-1.2.0/setup.sh
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.905139 optilibre-1.2.0/src/
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.910207 optilibre-1.2.0/src/optilibre/
--rw-r--r--   0 sydney     (501) staff       (20)      489 2023-04-26 14:39:18.000000 optilibre-1.2.0/src/optilibre/__init__.py
--rw-r--r--   0 sydney     (501) staff       (20)      200 2023-04-26 14:39:18.000000 optilibre-1.2.0/src/optilibre/__main__.py
--rw-r--r--   0 sydney     (501) staff       (20)      160 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre/_version.py
--rw-r--r--   0 sydney     (501) staff       (20)     2134 2022-05-22 14:24:54.000000 optilibre-1.2.0/src/optilibre/cli.py
--rw-r--r--   0 sydney     (501) staff       (20)     4141 2023-04-26 08:18:28.000000 optilibre-1.2.0/src/optilibre/core.py
--rw-r--r--   0 sydney     (501) staff       (20)      838 2023-04-25 12:43:08.000000 optilibre-1.2.0/src/optilibre/enums.py
--rw-r--r--   0 sydney     (501) staff       (20)     5230 2023-04-26 08:19:48.000000 optilibre-1.2.0/src/optilibre/helpers.py
--rw-r--r--   0 sydney     (501) staff       (20)     3178 2023-04-26 06:54:49.000000 optilibre-1.2.0/src/optilibre/models.py
--rw-r--r--   0 sydney     (501) staff       (20)     7794 2023-04-26 13:25:59.000000 optilibre-1.2.0/src/optilibre/runner.py
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911243 optilibre-1.2.0/src/optilibre/utils/
--rw-r--r--   0 sydney     (501) staff       (20)        0 2022-05-27 11:05:59.000000 optilibre-1.2.0/src/optilibre/utils/__init__.py
--rw-r--r--   0 sydney     (501) staff       (20)     2122 2022-07-20 14:11:59.000000 optilibre-1.2.0/src/optilibre/utils/parsers.py
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911032 optilibre-1.2.0/src/optilibre.egg-info/
--rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/PKG-INFO
--rw-r--r--   0 sydney     (501) staff       (20)      703 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/SOURCES.txt
--rw-r--r--   0 sydney     (501) staff       (20)        1 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/dependency_links.txt
--rw-r--r--   0 sydney     (501) staff       (20)       54 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/entry_points.txt
--rw-r--r--   0 sydney     (501) staff       (20)       32 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/requires.txt
--rw-r--r--   0 sydney     (501) staff       (20)       10 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/top_level.txt
-drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911704 optilibre-1.2.0/systemd/
--rw-r--r--   0 sydney     (501) staff       (20)      364 2022-05-22 13:42:28.000000 optilibre-1.2.0/systemd/opti_libre.service
--rw-r--r--   0 sydney     (501) staff       (20)       90 2022-05-22 13:42:28.000000 optilibre-1.2.0/systemd/opti_libre.timer
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.077700 optilibre-1.2.1/
+-rw-r--r--   0 sydney     (501) staff       (20)      126 2023-04-27 08:34:31.000000 optilibre-1.2.1/.gitignore
+-rw-r--r--   0 sydney     (501) staff       (20)      251 2023-04-27 08:34:31.000000 optilibre-1.2.1/CHANGELOG.md
+-rw-r--r--   0 sydney     (501) staff       (20)    34454 2022-05-22 13:42:28.000000 optilibre-1.2.1/LICENSE
+-rw-r--r--   0 sydney     (501) staff       (20)      190 2023-04-27 08:34:31.000000 optilibre-1.2.1/Makefile
+-rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 08:34:51.078160 optilibre-1.2.1/PKG-INFO
+-rw-r--r--   0 sydney     (501) staff       (20)     1655 2022-05-22 13:42:28.000000 optilibre-1.2.1/README.md
+-rw-r--r--   0 sydney     (501) staff       (20)      409 2023-04-27 08:34:31.000000 optilibre-1.2.1/optilibre.example.conf
+-rw-r--r--   0 sydney     (501) staff       (20)      908 2023-04-27 08:34:31.000000 optilibre-1.2.1/optilibre.example.toml
+-rw-r--r--   0 sydney     (501) staff       (20)      469 2023-04-27 08:34:31.000000 optilibre-1.2.1/pyproject.toml
+-rw-r--r--   0 sydney     (501) staff       (20)       31 2022-05-22 13:42:28.000000 optilibre-1.2.1/requirements.txt
+-rw-r--r--   0 sydney     (501) staff       (20)      654 2023-04-27 08:34:51.078591 optilibre-1.2.1/setup.cfg
+-rwxr-xr-x   0 sydney     (501) staff       (20)      497 2022-05-22 13:42:28.000000 optilibre-1.2.1/setup.sh
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.070842 optilibre-1.2.1/src/
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.075745 optilibre-1.2.1/src/optilibre/
+-rw-r--r--   0 sydney     (501) staff       (20)      489 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/__init__.py
+-rw-r--r--   0 sydney     (501) staff       (20)      200 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/__main__.py
+-rw-r--r--   0 sydney     (501) staff       (20)      160 2023-04-27 08:34:50.000000 optilibre-1.2.1/src/optilibre/_version.py
+-rw-r--r--   0 sydney     (501) staff       (20)     2134 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/cli.py
+-rw-r--r--   0 sydney     (501) staff       (20)     4141 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/core.py
+-rw-r--r--   0 sydney     (501) staff       (20)      838 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/enums.py
+-rw-r--r--   0 sydney     (501) staff       (20)     5230 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/helpers.py
+-rw-r--r--   0 sydney     (501) staff       (20)     3726 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/models.py
+-rw-r--r--   0 sydney     (501) staff       (20)     8227 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/runner.py
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.076872 optilibre-1.2.1/src/optilibre/utils/
+-rw-r--r--   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/utils/__init__.py
+-rw-r--r--   0 sydney     (501) staff       (20)     2122 2023-04-27 08:34:31.000000 optilibre-1.2.1/src/optilibre/utils/parsers.py
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.076625 optilibre-1.2.1/src/optilibre.egg-info/
+-rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/PKG-INFO
+-rw-r--r--   0 sydney     (501) staff       (20)      703 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/SOURCES.txt
+-rw-r--r--   0 sydney     (501) staff       (20)        1 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/dependency_links.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       54 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/entry_points.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       32 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/requires.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       10 2023-04-27 08:34:51.000000 optilibre-1.2.1/src/optilibre.egg-info/top_level.txt
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 08:34:51.077376 optilibre-1.2.1/systemd/
+-rw-r--r--   0 sydney     (501) staff       (20)      364 2022-05-22 13:42:28.000000 optilibre-1.2.1/systemd/opti_libre.service
+-rw-r--r--   0 sydney     (501) staff       (20)       90 2022-05-22 13:42:28.000000 optilibre-1.2.1/systemd/opti_libre.timer
```

### Comparing `optilibre-1.2.0/LICENSE` & `optilibre-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/PKG-INFO` & `optilibre-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optilibre
-Version: 1.2.0
+Version: 1.2.1
 Summary: Video and Image optimizer
 Home-page: https://gitlab.com/daufinsyd/optilibre
 Author: Sydney Gems
 Author-email: sydney@gems.technology
 Project-URL: Bug Tracker, https://gitlab.com/daufinsyd/optilibre/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `optilibre-1.2.0/README.md` & `optilibre-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/optilibre.example.toml` & `optilibre-1.2.1/optilibre.example.toml`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/setup.cfg` & `optilibre-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre/cli.py` & `optilibre-1.2.1/src/optilibre/cli.py`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre/core.py` & `optilibre-1.2.1/src/optilibre/core.py`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre/enums.py` & `optilibre-1.2.1/src/optilibre/enums.py`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre/helpers.py` & `optilibre-1.2.1/src/optilibre/helpers.py`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre/models.py` & `optilibre-1.2.1/src/optilibre/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,26 @@
 
     def get_in_path(self) -> Path:
         return self.in_path
 
     def get_out_path(self) -> Path:
         return self.out_path
 
+    def get_on_success_path(self) -> [Path, None]:
+        if 'src_on_success_dest' not in self.config:
+            logging.debug("src_on_success_dest is not defined for {}".format(self.name))
+            return None
+        return Path(self.config['src_on_success_dest'])
+
+    def get_on_failure_path(self) -> [Path, None]:
+        if 'src_on_failure_dest' not in self.config:
+            logging.debug("src_on_failure_dest is not defined for {}".format(self.name))
+            return None
+        return Path(self.config['src_on_failure_dest'])
+
 
 class ImageFolder(Folder):
     def get_codec(self):
         codec_str = self.get_config()["codec"]
         try:
             codec = enums.ImageCodec[codec_str.lower()]
         except KeyError:
```

### Comparing `optilibre-1.2.0/src/optilibre/runner.py` & `optilibre-1.2.1/src/optilibre/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,23 +35,24 @@
     subdir_msg = ""
     if subdir:
         subdir_msg = "(subdir: {})".format(subdir.relative_to(in_path))
     logging.info("Treating folder: {} {}".format(folder.get_name(), subdir_msg))
 
     local_config = folder.get_config()
     out_path = folder.get_out_path()
+    success_dest_path = folder.get_on_success_path()
+    failure_dest_path = folder.get_on_failure_path()
     codec = folder.get_codec()
 
     relative_subdir = None
     if subdir:
         # If we are working with a sub dir. Append it to out_path.
         relative_subdir = subdir.relative_to(in_path)  # for src_on_done
         out_path = out_path.joinpath(relative_subdir)  # get subdir from absolute path and join it with out_path
         in_path = subdir
-        helpers.ensure_folder_exists(path=out_path)
 
     # Set default options for JPEGoptim
     if codec == enums.ImageCodec.jpeg:
         # Remove dest if provided (otherwise subdir won't work because of arg as reference)
         local_config[codec.name.lower()].pop('d', None)
         local_config[codec.name.lower()].pop('dest', None)
         #if "d" not in local_config[codec.name.lower()] and "dest" not in local_config[codec.name.lower()]:
@@ -63,14 +64,20 @@
         for opt in local_config[codec.name.lower()].items():
             cmdline_codec_opts += " -" + str(opt[0]) + " " + str(opt[1])
     else:
         logging.debug("No config for %s found. Using default codec values." % codec.name)
 
     arg_list = []  # [(file1, shell1, local_config, subdir), (...)] we split arg_list to processes
     for file in Path(in_path).glob('*'):
+        # Check if we're processing a in/out/success/failure dest.
+        if file in [in_path, out_path, success_dest_path, failure_dest_path]:
+            logging.critical("Ignoring in/out folder ({})".format(file))
+            continue
+
+        # FILE
         if file.is_file():
             kind = filetype.guess_mime(str(file))
             if bool(re.match("image/+", str(kind))):
                 logging.debug("Building cmd line for: %s" % str(file))
                 file_mime = filetype.guess_mime(str(file))
 
                 if file.suffix not in optilibre.supported_img_ext or not bool(re.match('image/+', str(file_mime))):
@@ -97,22 +104,25 @@
                 shell_cmdline = "{encoder} {in_file} {options} {outfile}".format(
                     encoder=encoder_cmdline, in_file=helpers.get_path_as_escaped_str(file), options=cmdline_codec_opts, outfile=out_file)
 
                 arg_list.append((file, shell_cmdline, local_config, relative_subdir))
             else:
                 # Changing suffix
                 logging.debug("Filetype: %s for file: %s isn't an image file." % (str(kind), str(file)))
+
+        # DIRECTORY
         elif file.is_dir():
             logging.debug("{} is a directory. Recursively entering it.".format(str(file)))
             process_image_folder(folder=folder, subdir=Path(file))
         else:
             logging.debug("{} is not a file neither a dir. Ignoring it.".format(str(file)))
 
     # multiprocess call
     if arg_list:
+        helpers.ensure_folder_exists(path=out_path)  # only create folder if there is files to convert
         with Pool() as p:
             p.starmap(convert_img, arg_list)
 
 
 def process_video_folder(folder: models.VideoFolder, subdir: Path = None):
     """
     This function recursively process an "optilibre" folder and its subdir.
```

### Comparing `optilibre-1.2.0/src/optilibre/utils/parsers.py` & `optilibre-1.2.1/src/optilibre/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `optilibre-1.2.0/src/optilibre.egg-info/PKG-INFO` & `optilibre-1.2.1/src/optilibre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optilibre
-Version: 1.2.0
+Version: 1.2.1
 Summary: Video and Image optimizer
 Home-page: https://gitlab.com/daufinsyd/optilibre
 Author: Sydney Gems
 Author-email: sydney@gems.technology
 Project-URL: Bug Tracker, https://gitlab.com/daufinsyd/optilibre/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `optilibre-1.2.0/src/optilibre.egg-info/SOURCES.txt` & `optilibre-1.2.1/src/optilibre.egg-info/SOURCES.txt`

 * *Files identical despite different names*


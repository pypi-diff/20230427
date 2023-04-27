# Comparing `tmp/ocp_tessellate-1.0.1.tar.gz` & `tmp/ocp_tessellate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.1.tar", last modified: Sun Apr 23 16:08:07 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.0.2.tar", last modified: Thu Apr 27 18:57:05 2023, max compression
```

## Comparing `ocp_tessellate-1.0.1.tar` & `ocp_tessellate-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998796 ocp_tessellate-1.0.1/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-23 16:08:07.998848 ocp_tessellate-1.0.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998112 ocp_tessellate-1.0.1/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.1/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-04-23 16:07:54.000000 ocp_tessellate-1.0.1/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.1/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    26909 2023-04-23 16:07:04.000000 ocp_tessellate-1.0.1/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-21 16:07:20.000000 ocp_tessellate-1.0.1/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.1/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.1/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.1/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.1/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.1/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6137 2023-04-07 10:44:39.000000 ocp_tessellate-1.0.1/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:08:07.998702 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.1/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-04-23 16:08:07.999096 ocp_tessellate-1.0.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-04-23 16:07:54.000000 ocp_tessellate-1.0.1/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.745693 ocp_tessellate-1.0.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-27 18:57:05.745747 ocp_tessellate-1.0.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.744843 ocp_tessellate-1.0.2/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.2/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-04-27 18:56:38.000000 ocp_tessellate-1.0.2/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.2/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    27010 2023-04-27 18:53:29.000000 ocp_tessellate-1.0.2/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-27 18:53:44.000000 ocp_tessellate-1.0.2/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.2/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.2/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.2/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.2/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.2/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-27 16:19:21.000000 ocp_tessellate-1.0.2/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.745597 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-04-27 18:57:05.745992 ocp_tessellate-1.0.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-04-27 18:56:38.000000 ocp_tessellate-1.0.2/setup.py
```

### Comparing `ocp_tessellate-1.0.1/PKG-INFO` & `ocp_tessellate-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/__init__.py` & `ocp_tessellate-1.0.2/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/_version.py` & `ocp_tessellate-1.0.2/ocp_tessellate/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.0.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.0.2/ocp_tessellate/cad_objects.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/convert.py` & `ocp_tessellate-1.0.2/ocp_tessellate/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         cad_objs = [cad_obj]
 
     elif is_topods_shape(cad_obj):
         _debug(f"        conv: CAD Obj TopoDS Shape")
         cad_objs = [downcast(cad_obj)]
 
     else:
-        raise RuntimeError(f"Cannot transform {cad_objs}({type(cad_objs)}) to OCP")
+        raise RuntimeError(f"Cannot transform {cad_obj}({type(cad_obj)}) to OCP")
 
     if is_compound_list(cad_objs):
         cad_objs = get_downcasted_shape(cad_objs[0])
 
     # Convert to PartGroup
 
     if is_solid_list(cad_objs):
@@ -661,14 +661,17 @@
                 for child in cad_obj:
                     part = conv(child.wrapped, obj_name, color, alpha)
                     pg.add(part)
 
             else:
                 _debug("  to_assembly: generic case", obj_name)
                 if hasattr(cad_obj, "_dim") and cad_obj._dim == 3:
+                    if obj_name is None or obj_name == "":
+                        obj_name = "Solid"
+
                     if not isinstance(cad_obj, Iterable):
                         _debug("    to_assembly: no iterable", obj_name)
                         part = get_instance(
                             cad_obj, obj_name, rgba, instances, progress
                         )
 
                     elif isinstance(cad_obj, Iterable) and len(cad_obj.solids()) == 1:
```

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/defaults.py` & `ocp_tessellate-1.0.2/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.0.2/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.0.2/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.0.2/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.0.2/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.0.2/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate/utils.py` & `ocp_tessellate-1.0.2/ocp_tessellate/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,19 @@
     warnings.simplefilter("ignore", warning)
 
 
 def make_unique(names):
     found = {}
     unique_names = []
     for name in names:
+        if name is None:
+            unique_names.append(None)
+            continue
+
         if found.get(name) is None:
             found[name] = 1
             unique_names.append(name)
         else:
             found[name] += 1
             unique_names.append(f"{name}({found[name]})")
+
     return unique_names
```

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.0.2/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.1/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.0.2/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.1/setup.cfg` & `ocp_tessellate-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.1
+current_version = 1.0.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.1/setup.py` & `ocp_tessellate-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.1",
+    "version": "1.0.2",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```


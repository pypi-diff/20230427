# Comparing `tmp/pyaogmaneo-2.0.3.tar.gz` & `tmp/pyaogmaneo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.3.tar", last modified: Wed Mar 22 23:49:03 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.4.tar", last modified: Thu Apr 27 21:18:55 2023, max compression
```

## Comparing `pyaogmaneo-2.0.3.tar` & `pyaogmaneo-2.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-03-22 23:49:03.727977 pyaogmaneo-2.0.3/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-03-22 23:49:03.724643 pyaogmaneo-2.0.3/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.3/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-03-22 23:48:23.000000 pyaogmaneo-2.0.3/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.3/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.3/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-03-22 23:49:03.727977 pyaogmaneo-2.0.3/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-03-22 20:21:56.000000 pyaogmaneo-2.0.3/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-03-22 23:49:03.724643 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-03-22 23:49:03.000000 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-03-22 23:49:03.000000 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-03-22 23:49:03.000000 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-03-22 23:49:03.000000 pyaogmaneo-2.0.3/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.3/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-03-22 23:49:03.727977 pyaogmaneo-2.0.3/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-03-22 23:48:30.000000 pyaogmaneo-2.0.3/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-03-22 23:49:03.724643 pyaogmaneo-2.0.3/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-03-22 23:49:03.727977 pyaogmaneo-2.0.3/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-03-22 19:14:03.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-03-22 20:22:39.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9781 2023-03-22 23:23:39.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6544 2023-03-22 22:28:21.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     5880 2023-03-22 19:13:42.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3014 2023-03-22 20:22:46.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8391 2023-03-22 22:18:15.000000 pyaogmaneo-2.0.3/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.4/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-04-27 21:17:42.000000 pyaogmaneo-2.0.4/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.4/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.4/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.4/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-04-27 21:16:13.000000 pyaogmaneo-2.0.4/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9352 2023-04-23 00:53:41.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6430 2023-04-27 21:16:02.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     5920 2023-04-22 23:35:15.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3029 2023-04-27 21:15:53.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8641 2023-04-27 19:20:12.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.3/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.4/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.3/CMakeLists.txt` & `pyaogmaneo-2.0.4/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 63b9593fccf964e0383650256e337e6ffb8435d9
+        GIT_TAG 7332a07731274779cf476b5810101f5aec2d20a3
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.3/LICENSE.md` & `pyaogmaneo-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.3/PKG-INFO` & `pyaogmaneo-2.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.3/README.md` & `pyaogmaneo-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.3/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.4/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.3/setup.py` & `pyaogmaneo-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.3",
+    version="2.0.4",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -52,54 +52,24 @@
     if (temporal_horizon < 1)
         throw std::runtime_error("error: temporal_horizon < 1 is not allowed!");
 
     if (ticks_per_update > temporal_horizon)
         throw std::runtime_error("error: ticks_per_update > temporal_horizon is not allowed!");
 }
 
-void Hierarchy::enc_get_set_index_check(
-    int l
-) const {
-    if (l < 0 || l >= h.get_num_layers())
-        throw std::runtime_error("error: " + std::to_string(l) + " is not a valid layer index!");
-}
-
-void Hierarchy::dec_get_set_index_check(
-    int l, int i
-) const {
-    if (l < 0 || l >= h.get_num_layers())
-        throw std::runtime_error("error: " + std::to_string(l) + " is not a valid layer index!");
-
-    if (l == 0 && (i < 0 || i >= h.get_num_io()))
-        throw std::runtime_error("error: " + std::to_string(i) + " is not a valid input index!");
-
-    if (l == 0 && (!h.io_layer_exists(i) || h.get_io_type(i) != aon::prediction))
-        throw std::runtime_error("error: index " + std::to_string(i) + " does not have a decoder!");
-}
-
-void Hierarchy::act_get_set_index_check(
-    int i
-) const {
-    if (i < 0 || i >= h.get_num_io())
-        throw std::runtime_error("error: " + std::to_string(i) + " is not a valid input index!");
-
-    if (!h.io_layer_exists(i) || h.get_io_type(i) != aon::action)
-        throw std::runtime_error("error: index " + std::to_string(i) + " does not have an actor!");
-}
-
 Hierarchy::Hierarchy(
     const std::vector<IO_Desc> &io_descs,
     const std::vector<Layer_Desc> &layer_descs,
-    const std::string &name,
+    const std::string &file_name,
     const std::vector<unsigned char> &buffer
 ) {
     if (!buffer.empty())
         init_from_buffer(buffer);
-    else if (!name.empty())
-        init_from_file(name);
+    else if (!file_name.empty())
+        init_from_file(file_name);
     else {
         if (io_descs.empty() || layer_descs.empty())
             throw std::runtime_error("error: Hierarchy constructor requires some non-empty arguments!");
 
         init_random(io_descs, layer_descs);
     }
 
@@ -148,24 +118,24 @@
         );
     }
 
     h.init_random(c_io_descs, c_layer_descs);
 }
 
 void Hierarchy::init_from_file(
-    const std::string &name
+    const std::string &file_name
 ) {
     File_Reader reader;
-    reader.ins.open(name, std::ios::binary);
+    reader.ins.open(file_name, std::ios::binary);
 
     int magic;
     reader.read(&magic, sizeof(int));
 
     if (magic != hierarchy_magic)
-        throw std::runtime_error("attempted to initialize Hierarchy from incompatible file - " + name);
+        throw std::runtime_error("attempted to initialize Hierarchy from incompatible file - " + file_name);
 
     h.read(reader);
 }
 
 void Hierarchy::init_from_buffer(
     const std::vector<unsigned char> &buffer
 ) {
@@ -178,18 +148,18 @@
     if (magic != hierarchy_magic)
         throw std::runtime_error("attempted to initialize Hierarchy from incompatible buffer!");
 
     h.read(reader);
 }
 
 void Hierarchy::save_to_file(
-    const std::string &name
+    const std::string &file_name
 ) {
     File_Writer writer;
-    writer.outs.open(name, std::ios::binary);
+    writer.outs.open(file_name, std::ios::binary);
 
     writer.write(&hierarchy_magic, sizeof(int));
 
     h.write(writer);
 }
 
 std::vector<unsigned char> Hierarchy::serialize_to_buffer() {
@@ -275,14 +245,31 @@
 
     for (int j = 0; j < predictions.size(); j++)
         predictions[j] = h.get_prediction_cis(i)[j];
 
     return predictions;
 }
 
+std::vector<float> Hierarchy::get_prediction_acts(
+    int i
+) const {
+    if (i < 0 || i >= h.get_num_io())
+        throw std::runtime_error("prediction index " + std::to_string(i) + " out of range [0, " + std::to_string(h.get_num_io() - 1) + "]!");
+
+    if (!h.io_layer_exists(i) || h.get_io_type(i) == aon::none)
+        throw std::runtime_error("no decoder exists at index " + std::to_string(i) + " - did you set it to the correct type?");
+
+    std::vector<float> predictions(h.get_prediction_acts(i).size());
+
+    for (int j = 0; j < predictions.size(); j++)
+        predictions[j] = h.get_prediction_acts(i)[j];
+
+    return predictions;
+}
+
 void Hierarchy::copy_params_to_h() {
     if (params.ios.size() != h.params.ios.size())
         throw std::runtime_error("ios parameter size mismatch - did you modify the length of params.ios?");
 
     if (params.layers.size() != h.params.layers.size())
         throw std::runtime_error("layers parameter size mismatch - did you modify the length of params.layers?");
```

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.h`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace pyaon {
-const int hierarchy_magic = 3188325;
+const int hierarchy_magic = 1188221;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -79,54 +79,41 @@
     std::vector<aon::Hierarchy::IO_Params> ios;
 };
 
 class Hierarchy {
 private:
     aon::Hierarchy h;
 
-    void enc_get_set_index_check(
-        int l
-    ) const;
-
-    void dec_get_set_index_check(
-        int l,
-        int i
-    ) const;
-
-    void act_get_set_index_check(
-        int i
-    ) const;
-
     void init_random(
         const std::vector<IO_Desc> &io_descs,
         const std::vector<Layer_Desc> &layer_descs
     );
 
     void init_from_file(
-        const std::string &name
+        const std::string &file_name
     );
 
     void init_from_buffer(
         const std::vector<unsigned char> &buffer
     );
 
     void copy_params_to_h();
 
 public:
     Params params;
 
     Hierarchy(
         const std::vector<IO_Desc> &io_descs,
         const std::vector<Layer_Desc> &layer_descs,
-        const std::string &name,
+        const std::string &file_name,
         const std::vector<unsigned char> &buffer
     );
 
     void save_to_file(
-        const std::string &name
+        const std::string &file_name
     );
 
     std::vector<unsigned char> serialize_to_buffer();
 
     void set_state_from_buffer(
         const std::vector<unsigned char> &buffer
     );
@@ -148,14 +135,18 @@
         return h.get_num_layers();
     }
 
     std::vector<int> get_prediction_cis(
         int i
     ) const;
 
+    std::vector<float> get_prediction_acts(
+        int i
+    ) const;
+
     std::vector<int> get_hidden_cis(
         int l
     ) {
         if (l < 0 || l >= h.get_num_layers())
             throw std::runtime_error("error: " + std::to_string(l) + " is not a valid layer index!");
 
         std::vector<int> hidden_cis(h.get_encoder(l).get_hidden_cis().size());
```

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     if (radius < 0)
         throw std::runtime_error("error: radius < 0 is not allowed!");
 }
 
 Image_Encoder::Image_Encoder(
     const std::tuple<int, int, int> &hidden_size,
     const std::vector<Image_Visible_Layer_Desc> &visible_layer_descs,
-    const std::string &name,
+    const std::string &file_name,
     const std::vector<unsigned char> &buffer
 ) {
     if (!buffer.empty())
         init_from_buffer(buffer);
-    else if (!name.empty())
-        init_from_file(name);
+    else if (!file_name.empty())
+        init_from_file(file_name);
     else {
         if (visible_layer_descs.empty())
             throw std::runtime_error("error: Image_Encoder constructor requires some non-empty arguments!");
 
         init_random(hidden_size, visible_layer_descs);
     }
 
@@ -72,24 +72,24 @@
     if (!all_in_range)
         throw std::runtime_error(" - Image_Encoder: some parameters out of range!");
 
     enc.init_random(aon::Int3(std::get<0>(hidden_size), std::get<1>(hidden_size), std::get<2>(hidden_size)), c_visible_layer_descs);
 }
 
 void Image_Encoder::init_from_file(
-    const std::string &name
+    const std::string &file_name
 ) {
     File_Reader reader;
-    reader.ins.open(name, std::ios::binary);
+    reader.ins.open(file_name, std::ios::binary);
 
     int magic;
     reader.read(&magic, sizeof(int));
 
     if (magic != image_encoder_magic)
-        throw std::runtime_error("attempted to initialize Image_Encoder from incompatible file - " + name);
+        throw std::runtime_error("attempted to initialize Image_Encoder from incompatible file - " + file_name);
 
     enc.read(reader);
 }
 
 void Image_Encoder::init_from_buffer(
     const std::vector<unsigned char> &buffer
 ) {
@@ -102,18 +102,18 @@
     if (magic != image_encoder_magic)
         throw std::runtime_error("attempted to initialize Image_Encoder from incompatible buffer!");
 
     enc.read(reader);
 }
 
 void Image_Encoder::save_to_file(
-    const std::string &name
+    const std::string &file_name
 ) {
     File_Writer writer;
-    writer.outs.open(name, std::ios::binary);
+    writer.outs.open(file_name, std::ios::binary);
 
     writer.write(&image_encoder_magic, sizeof(int));
 
     enc.write(writer);
 }
 
 std::vector<unsigned char> Image_Encoder::serialize_to_buffer() {
```

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace pyaon {
-const int image_encoder_magic = 6221138;
+const int image_encoder_magic = 6121137;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
@@ -37,33 +37,33 @@
 
     void init_random(
         const std::tuple<int, int, int> &hidden_size,
         const std::vector<Image_Visible_Layer_Desc> &visible_layer_descs
     );
 
     void init_from_file(
-        const std::string &name
+        const std::string &file_name
     );
 
     void init_from_buffer(
         const std::vector<unsigned char> &buffer
     );
 
 public:
     aon::Image_Encoder::Params params;
 
     Image_Encoder(
         const std::tuple<int, int, int> &hidden_size,
         const std::vector<Image_Visible_Layer_Desc> &visible_layer_descs,
-        const std::string &name,
+        const std::string &file_name,
         const std::vector<unsigned char> &buffer
     );
 
     void save_to_file(
-        const std::string &name
+        const std::string &file_name
     );
 
     std::vector<unsigned char> serialize_to_buffer();
 
     void step(
         const std::vector<std::vector<unsigned char>> &inputs,
         bool learn_enabled
```

### Comparing `pyaogmaneo-2.0.3/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.4/source/pyaogmaneo/py_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,27 @@
         .def_readwrite("down_radius", &pyaon::Layer_Desc::down_radius)
         .def_readwrite("ticks_per_update", &pyaon::Layer_Desc::ticks_per_update)
         .def_readwrite("temporal_horizon", &pyaon::Layer_Desc::temporal_horizon);
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("scale", &aon::Encoder::Params::scale)
-        .def_readwrite("lr", &aon::Encoder::Params::lr);
+        .def_readwrite("code_iters", &aon::Encoder::Params::code_iters)
+        .def_readwrite("lr", &aon::Encoder::Params::lr)
+        .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
-        .def_readwrite("scale", &aon::Decoder::Params::scale)
-        .def_readwrite("lr", &aon::Decoder::Params::lr);
+        .def_readwrite("lr", &aon::Decoder::Params::lr)
+        .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
 
     py::class_<aon::Actor::Params>(m, "Actorparams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
-        .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
         .def_readwrite("temperature", &aon::Actor::Params::temperature)
         .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
         .def_readwrite("history_iters", &aon::Actor::Params::history_iters);
 
     py::class_<aon::Hierarchy::Layer_Params>(m, "LayerParams")
         .def(py::init<>())
@@ -109,15 +109,15 @@
                 const std::vector<pyaon::IO_Desc>&,
                 const std::vector<pyaon::Layer_Desc>&,
                 const std::string&,
                 const std::vector<unsigned char>&
             >(),
             py::arg("io_descs") = std::vector<pyaon::IO_Desc>(),
             py::arg("layer_descs") = std::vector<pyaon::Layer_Desc>(),
-            py::arg("name") = std::string(),
+            py::arg("file_name") = std::string(),
             py::arg("buffer") = std::vector<unsigned char>()
         )
         .def_readwrite("params", &pyaon::Hierarchy::params)
         .def("save_to_file", &pyaon::Hierarchy::save_to_file)
         .def("serialize_to_buffer", &pyaon::Hierarchy::serialize_to_buffer)
         .def("set_state_from_buffer", &pyaon::Hierarchy::set_state_from_buffer)
         .def("serialize_state_to_buffer", &pyaon::Hierarchy::serialize_state_to_buffer)
@@ -126,14 +126,15 @@
             py::arg("learn_enabled") = true,
             py::arg("reward") = 0.0f,
             py::arg("mimic") = 0.0f
         )
         .def("clear_state", &pyaon::Hierarchy::clear_state)
         .def("get_num_layers", &pyaon::Hierarchy::get_num_layers)
         .def("get_prediction_cis", &pyaon::Hierarchy::get_prediction_cis)
+        .def("get_prediction_acts", &pyaon::Hierarchy::get_prediction_acts)
         .def("get_hidden_cis", &pyaon::Hierarchy::get_hidden_cis)
         .def("get_hidden_size", &pyaon::Hierarchy::get_hidden_size)
         .def("get_num_encoder_visible_layers", &pyaon::Hierarchy::get_num_encoder_visible_layers)
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
         .def("get_io_size", &pyaon::Hierarchy::get_io_size)
@@ -152,26 +153,28 @@
         )
         .def_readwrite("size", &pyaon::Image_Visible_Layer_Desc::size)
         .def_readwrite("radius", &pyaon::Image_Visible_Layer_Desc::radius);
 
     // bind params
     py::class_<aon::Image_Encoder::Params>(m, "ImageEncoderParams")
         .def(py::init<>())
+        .def_readwrite("choice", &aon::Image_Encoder::Params::choice)
+        .def_readwrite("vigilance", &aon::Image_Encoder::Params::vigilance)
         .def_readwrite("lr", &aon::Image_Encoder::Params::lr);
 
     py::class_<pyaon::Image_Encoder>(m, "ImageEncoder")
         .def(py::init<
                 const std::tuple<int, int, int>&,
                 const std::vector<pyaon::Image_Visible_Layer_Desc>&,
                 const std::string&,
                 const std::vector<unsigned char>&
             >(),
             py::arg("hidden_size") = std::tuple<int, int, int>({ 4, 4, 16 }),
             py::arg("visible_layer_descs") = std::vector<pyaon::Image_Visible_Layer_Desc>(),
-            py::arg("name") = std::string(),
+            py::arg("file_name") = std::string(),
             py::arg("buffer") = std::vector<unsigned char>()
         )
         .def_readwrite("params", &pyaon::Image_Encoder::params)
         .def("save_to_file", &pyaon::Image_Encoder::save_to_file)
         .def("serialize_to_buffer", &pyaon::Image_Encoder::serialize_to_buffer)
         .def("step", &pyaon::Image_Encoder::step,
             py::arg("inputs"),
```


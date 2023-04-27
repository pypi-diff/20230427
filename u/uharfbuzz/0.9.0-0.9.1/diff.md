# Comparing `tmp/uharfbuzz-0.9.0.zip` & `tmp/uharfbuzz-0.9.1.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 28770 bytes, number of entries: 32
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/src/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/tests/
--rw-r--r--  2.0 unx      909 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/.coveragerc
--rw-r--r--  2.0 unx      347 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/.gitignore
--rw-r--r--  2.0 unx     1901 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/.travis.yml
--rw-r--r--  2.0 unx     1067 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/appveyor.yml
--rw-r--r--  2.0 unx     2367 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/CMakeLists.txt
--rw-r--r--  2.0 unx    11357 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/LICENSE
--rw-r--r--  2.0 unx     1996 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/PKG-INFO
--rw-r--r--  2.0 unx      217 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/pyproject.toml
--rw-r--r--  2.0 unx     1243 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/README.md
--rw-r--r--  2.0 unx      140 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/requirements-dev.txt
--rw-r--r--  2.0 unx       96 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/setup.cfg
--rw-r--r--  2.0 unx     1841 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/setup.py
--rw-r--r--  2.0 unx     1961 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/tox.ini
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/
--rw-r--r--  2.0 unx       25 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/src/uharfbuzz/__init__.py
--rw-r--r--  2.0 unx    22735 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/src/uharfbuzz/_harfbuzz.pyx
--rw-r--r--  2.0 unx     9869 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/src/uharfbuzz/charfbuzz.pxd
--rw-r--r--  2.0 unx     1316 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/src/uharfbuzz/CMakeLists.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/not-zip-safe
--rw-r--r--  2.0 unx     1996 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      555 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       10 b- defN 20-Mar-28 08:05 uharfbuzz-0.9.0/src/uharfbuzz.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-28 08:05 uharfbuzz-0.9.0/tests/data/
--rw-r--r--  2.0 unx    10247 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/tests/test_uharfbuzz.py
--rw-r--r--  2.0 unx       85 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/tests/data/AdobeBlank.fea
--rw-r--r--  2.0 unx     1892 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/tests/data/AdobeBlank.subset.ttf
--rw-r--r--  2.0 unx     4301 b- defN 20-Mar-28 07:57 uharfbuzz-0.9.0/tests/data/LICENSE_AdobeBlank.txt
-32 files, 78475 bytes uncompressed, 24098 bytes compressed:  69.3%
+Zip file size: 28851 bytes, number of entries: 32
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/src/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/tests/
+-rw-r--r--  2.0 unx      909 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/.coveragerc
+-rw-r--r--  2.0 unx      347 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/.gitignore
+-rw-r--r--  2.0 unx     1901 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/.travis.yml
+-rw-r--r--  2.0 unx     1067 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/appveyor.yml
+-rw-r--r--  2.0 unx     2367 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/CMakeLists.txt
+-rw-r--r--  2.0 unx    11357 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/LICENSE
+-rw-r--r--  2.0 unx     1996 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/PKG-INFO
+-rw-r--r--  2.0 unx      217 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/pyproject.toml
+-rw-r--r--  2.0 unx     1243 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/README.md
+-rw-r--r--  2.0 unx      140 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/requirements-dev.txt
+-rw-r--r--  2.0 unx       96 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/setup.cfg
+-rw-r--r--  2.0 unx     1841 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/setup.py
+-rw-r--r--  2.0 unx     1961 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/tox.ini
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/
+-rw-r--r--  2.0 unx       25 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/src/uharfbuzz/__init__.py
+-rw-r--r--  2.0 unx    22849 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/src/uharfbuzz/_harfbuzz.pyx
+-rw-r--r--  2.0 unx     9869 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/src/uharfbuzz/charfbuzz.pxd
+-rw-r--r--  2.0 unx     1316 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/src/uharfbuzz/CMakeLists.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx     1996 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      555 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       10 b- defN 20-Apr-01 15:13 uharfbuzz-0.9.1/src/uharfbuzz.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 20-Apr-01 15:13 uharfbuzz-0.9.1/tests/data/
+-rw-r--r--  2.0 unx    10624 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/tests/test_uharfbuzz.py
+-rw-r--r--  2.0 unx       85 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/tests/data/AdobeBlank.fea
+-rw-r--r--  2.0 unx     1892 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/tests/data/AdobeBlank.subset.ttf
+-rw-r--r--  2.0 unx     4301 b- defN 20-Apr-01 15:05 uharfbuzz-0.9.1/tests/data/LICENSE_AdobeBlank.txt
+32 files, 78966 bytes uncompressed, 24179 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,97 +1,97 @@
-Filename: uharfbuzz-0.9.0/
+Filename: uharfbuzz-0.9.1/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/
+Filename: uharfbuzz-0.9.1/src/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/
+Filename: uharfbuzz-0.9.1/tests/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/.coveragerc
+Filename: uharfbuzz-0.9.1/.coveragerc
 Comment: 
 
-Filename: uharfbuzz-0.9.0/.gitignore
+Filename: uharfbuzz-0.9.1/.gitignore
 Comment: 
 
-Filename: uharfbuzz-0.9.0/.travis.yml
+Filename: uharfbuzz-0.9.1/.travis.yml
 Comment: 
 
-Filename: uharfbuzz-0.9.0/appveyor.yml
+Filename: uharfbuzz-0.9.1/appveyor.yml
 Comment: 
 
-Filename: uharfbuzz-0.9.0/CMakeLists.txt
+Filename: uharfbuzz-0.9.1/CMakeLists.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/LICENSE
+Filename: uharfbuzz-0.9.1/LICENSE
 Comment: 
 
-Filename: uharfbuzz-0.9.0/PKG-INFO
+Filename: uharfbuzz-0.9.1/PKG-INFO
 Comment: 
 
-Filename: uharfbuzz-0.9.0/pyproject.toml
+Filename: uharfbuzz-0.9.1/pyproject.toml
 Comment: 
 
-Filename: uharfbuzz-0.9.0/README.md
+Filename: uharfbuzz-0.9.1/README.md
 Comment: 
 
-Filename: uharfbuzz-0.9.0/requirements-dev.txt
+Filename: uharfbuzz-0.9.1/requirements-dev.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/setup.cfg
+Filename: uharfbuzz-0.9.1/setup.cfg
 Comment: 
 
-Filename: uharfbuzz-0.9.0/setup.py
+Filename: uharfbuzz-0.9.1/setup.py
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tox.ini
+Filename: uharfbuzz-0.9.1/tox.ini
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz/
+Filename: uharfbuzz-0.9.1/src/uharfbuzz/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz/__init__.py
+Filename: uharfbuzz-0.9.1/src/uharfbuzz/__init__.py
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz/_harfbuzz.pyx
+Filename: uharfbuzz-0.9.1/src/uharfbuzz/_harfbuzz.pyx
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz/charfbuzz.pxd
+Filename: uharfbuzz-0.9.1/src/uharfbuzz/charfbuzz.pxd
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz/CMakeLists.txt
+Filename: uharfbuzz-0.9.1/src/uharfbuzz/CMakeLists.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/dependency_links.txt
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/dependency_links.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/not-zip-safe
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/not-zip-safe
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/PKG-INFO
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/PKG-INFO
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/SOURCES.txt
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/SOURCES.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/src/uharfbuzz.egg-info/top_level.txt
+Filename: uharfbuzz-0.9.1/src/uharfbuzz.egg-info/top_level.txt
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/data/
+Filename: uharfbuzz-0.9.1/tests/data/
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/test_uharfbuzz.py
+Filename: uharfbuzz-0.9.1/tests/test_uharfbuzz.py
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/data/AdobeBlank.fea
+Filename: uharfbuzz-0.9.1/tests/data/AdobeBlank.fea
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/data/AdobeBlank.subset.ttf
+Filename: uharfbuzz-0.9.1/tests/data/AdobeBlank.subset.ttf
 Comment: 
 
-Filename: uharfbuzz-0.9.0/tests/data/LICENSE_AdobeBlank.txt
+Filename: uharfbuzz-0.9.1/tests/data/LICENSE_AdobeBlank.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `uharfbuzz-0.9.0/.coveragerc` & `uharfbuzz-0.9.1/.coveragerc`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/.travis.yml` & `uharfbuzz-0.9.1/.travis.yml`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/appveyor.yml` & `uharfbuzz-0.9.1/appveyor.yml`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/CMakeLists.txt` & `uharfbuzz-0.9.1/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/LICENSE` & `uharfbuzz-0.9.1/LICENSE`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/PKG-INFO` & `uharfbuzz-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uharfbuzz
-Version: 0.9.0
+Version: 0.9.1
 Summary: Streamlined Cython bindings for the harfbuzz shaping engine
 Home-page: https://github.com/trufont/uharfbuzz
 Author: Adrien Tétar
 Author-email: adri-from-59@hotmail.fr
 License: Apache License 2.0
 Description: [![Travis Build Status](https://travis-ci.org/harfbuzz/uharfbuzz.svg?branch=master)](https://travis-ci.org/harfbuzz/uharfbuzz)
         [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/k52t0vwqb9rhcl9v/branch/master?svg=true)](https://ci.appveyor.com/project/fonttools/uharfbuzz/branch/master)
```

## Comparing `uharfbuzz-0.9.0/README.md` & `uharfbuzz-0.9.1/README.md`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/setup.py` & `uharfbuzz-0.9.1/setup.py`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/tox.ini` & `uharfbuzz-0.9.1/tox.ini`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/src/uharfbuzz/_harfbuzz.pyx` & `uharfbuzz-0.9.1/src/uharfbuzz/_harfbuzz.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -73,19 +73,21 @@
     @property
     def y_offset(self):
         return self._hb_glyph_position.y_offset
 
 
 cdef class Buffer:
     cdef hb_buffer_t* _hb_buffer
+    cdef object _message_callback
 
     def __cinit__(self):
         self._hb_buffer = hb_buffer_create()
         if not hb_buffer_allocation_successful(self._hb_buffer):
             raise MemoryError()
+        self._message_callback = None
 
     def __dealloc__(self):
         if self._hb_buffer is not NULL:
             hb_buffer_destroy(self._hb_buffer)
 
     # DEPRECATED: use the normal constructor
     @classmethod
@@ -234,14 +236,15 @@
         else:
             raise AssertionError(kind)
 
     def guess_segment_properties(self) -> None:
         hb_buffer_guess_segment_properties(self._hb_buffer)
 
     def set_message_func(self, callback) -> None:
+        self._message_callback = callback
         hb_buffer_set_message_func(self._hb_buffer, msgcallback, <void*>callback, NULL)
 
 
 cdef hb_user_data_key_t k
 
 
 cdef hb_blob_t* _reference_table_func(
```

## Comparing `uharfbuzz-0.9.0/src/uharfbuzz/charfbuzz.pxd` & `uharfbuzz-0.9.1/src/uharfbuzz/charfbuzz.pxd`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/src/uharfbuzz/CMakeLists.txt` & `uharfbuzz-0.9.1/src/uharfbuzz/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/src/uharfbuzz.egg-info/PKG-INFO` & `uharfbuzz-0.9.1/src/uharfbuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uharfbuzz
-Version: 0.9.0
+Version: 0.9.1
 Summary: Streamlined Cython bindings for the harfbuzz shaping engine
 Home-page: https://github.com/trufont/uharfbuzz
 Author: Adrien Tétar
 Author-email: adri-from-59@hotmail.fr
 License: Apache License 2.0
 Description: [![Travis Build Status](https://travis-ci.org/harfbuzz/uharfbuzz.svg?branch=master)](https://travis-ci.org/harfbuzz/uharfbuzz)
         [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/k52t0vwqb9rhcl9v/branch/master?svg=true)](https://ci.appveyor.com/project/fonttools/uharfbuzz/branch/master)
```

## Comparing `uharfbuzz-0.9.0/src/uharfbuzz.egg-info/SOURCES.txt` & `uharfbuzz-0.9.1/src/uharfbuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/tests/test_uharfbuzz.py` & `uharfbuzz-0.9.1/tests/test_uharfbuzz.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,14 +228,29 @@
         gids_trace = [[g.codepoint for g in infos] for infos in infos_trace]
         assert gids_trace == [[5, 4, 3, 2, 1], [5, 4, 1, 2, 1],
                               [5, 4, 1, 2, 1], [5, 4, 1, 2, 1]]
         advances_trace = [[g.x_advance for g in pos] for pos in positions_trace]
         assert advances_trace == [[0, 0, 0, 0, 0], [0, 0, 0, 0, 0],
                                   [0, 0, 0, 0, 0], [0, 0, 0, 100, 0]]
 
+    def test_message_func_crash(self, blankfont):
+        string = "edcba"
+        buf = hb.Buffer()
+        buf.add_str(string)
+        buf.guess_segment_properties()
+        message_collector = MessageCollector()
+        buf.set_message_func(message_collector.message)
+        hb.shape(blankfont, buf)
+
+
+class MessageCollector:
+    def message(self, message):
+        pass
+
+
 class TestGetBaseline:
     # The test font contains a BASE table with some test values
     def test_ot_layout_get_baseline_invalid_tag(self, blankfont):
         with pytest.raises(ValueError):
             # invalid baseline tag
             baseline = hb.ot_layout_get_baseline(blankfont, "xxxx", "LTR", "", "")
```

## Comparing `uharfbuzz-0.9.0/tests/data/AdobeBlank.subset.ttf` & `uharfbuzz-0.9.1/tests/data/AdobeBlank.subset.ttf`

 * *Files identical despite different names*

## Comparing `uharfbuzz-0.9.0/tests/data/LICENSE_AdobeBlank.txt` & `uharfbuzz-0.9.1/tests/data/LICENSE_AdobeBlank.txt`

 * *Files identical despite different names*


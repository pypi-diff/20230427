# Comparing `tmp/SpiNNakerTestBase-1!7.0.0a4.tar.gz` & `tmp/SpiNNakerTestBase-1!7.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiNNakerTestBase-1!7.0.0a4.tar", last modified: Wed Apr 19 15:14:16 2023, max compression
+gzip compressed data, was "SpiNNakerTestBase-1!7.0.0a5.tar", last modified: Wed Apr 26 12:08:54 2023, max compression
```

## Comparing `SpiNNakerTestBase-1!7.0.0a4.tar` & `SpiNNakerTestBase-1!7.0.0a5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:16.390962 SpiNNakerTestBase-1!7.0.0a4/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5054 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a4/CITATION.cff
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:37:33.000000 SpiNNakerTestBase-1!7.0.0a4/LICENSE
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      957 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a4/LICENSE_POLICY.md
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       56 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a4/MANIFEST.in
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-19 15:14:16.390962 SpiNNakerTestBase-1!7.0.0a4/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      167 2023-04-19 15:14:13.000000 SpiNNakerTestBase-1!7.0.0a4/README.md
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:16.390962 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      630 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/SOURCES.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/dependency_links.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       92 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/requires.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       19 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/top_level.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:14:16.000000 SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/zip-safe
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:30:41.000000 SpiNNakerTestBase-1!7.0.0a4/pyproject.toml
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1380 2023-04-19 15:14:16.390962 SpiNNakerTestBase-1!7.0.0a4/setup.cfg
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1319 2023-04-13 14:09:56.000000 SpiNNakerTestBase-1!7.0.0a4/setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:14:16.390962 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      798 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-19 15:14:13.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/_version.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3359 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/base_test_case.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     6113 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/root_script_builder.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4903 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/root_test_case.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2822 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/script_checker.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1033 2023-04-14 09:55:13.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/test_no_job_destroy.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1022 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/test_scripts_header
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5054 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a5/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:37:33.000000 SpiNNakerTestBase-1!7.0.0a5/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      957 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a5/LICENSE_POLICY.md
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       56 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a5/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      167 2023-04-26 12:06:32.000000 SpiNNakerTestBase-1!7.0.0a5/README.md
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.222593 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      630 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       92 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       19 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/zip-safe
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:30:41.000000 SpiNNakerTestBase-1!7.0.0a5/pyproject.toml
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1380 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1319 2023-04-13 14:09:56.000000 SpiNNakerTestBase-1!7.0.0a5/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      798 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-26 12:06:32.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3359 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/base_test_case.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     6113 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_script_builder.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4903 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_test_case.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2822 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/script_checker.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1033 2023-04-14 09:55:13.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_no_job_destroy.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1022 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_scripts_header
```

### Comparing `SpiNNakerTestBase-1!7.0.0a4/CITATION.cff` & `SpiNNakerTestBase-1!7.0.0a5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/LICENSE` & `SpiNNakerTestBase-1!7.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/LICENSE_POLICY.md` & `SpiNNakerTestBase-1!7.0.0a5/LICENSE_POLICY.md`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/PKG-INFO` & `SpiNNakerTestBase-1!7.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiNNakerTestBase
-Version: 1!7.0.0a4
+Version: 1!7.0.0a5
 Summary: Tools for testing SpiNNaker platform
 Home-page: https://github.com/SpiNNakerManchester/Testbase
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,test support
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/PKG-INFO` & `SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiNNakerTestBase
-Version: 1!7.0.0a4
+Version: 1!7.0.0a5
 Summary: Tools for testing SpiNNaker platform
 Home-page: https://github.com/SpiNNakerManchester/Testbase
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,test support
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SpiNNakerTestBase-1!7.0.0a4/SpiNNakerTestBase.egg-info/SOURCES.txt` & `SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/pyproject.toml` & `SpiNNakerTestBase-1!7.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/setup.cfg` & `SpiNNakerTestBase-1!7.0.0a5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [options]
 python_requires = >=3.7, <4
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
-	SpiNNFrontEndCommon == 1!7.0.0.a4
+	SpiNNFrontEndCommon == 1!7.0.0-a5
 	matplotlib
 
 [options.packages.find]
 include = 
 	spinnaker_testbase
 	spinnaker_testbase.*
```

### Comparing `SpiNNakerTestBase-1!7.0.0a4/setup.py` & `SpiNNakerTestBase-1!7.0.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/__init__.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/_version.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1!7.0.0.a4"
+__version__ = "1!7.0.0-a5"
 __version_month__ = "April"
 __version_year__ = "2023"
 __version_day__ = "17"
 __version_name__ = "Revisionist"
```

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/base_test_case.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/base_test_case.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/root_script_builder.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_script_builder.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/root_test_case.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_test_case.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/script_checker.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/script_checker.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/test_no_job_destroy.py` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_no_job_destroy.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a4/spinnaker_testbase/test_scripts_header` & `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_scripts_header`

 * *Files identical despite different names*


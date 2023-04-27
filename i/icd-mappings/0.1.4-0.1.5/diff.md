# Comparing `tmp/icd_mappings-0.1.4.tar.gz` & `tmp/icd_mappings-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icd_mappings-0.1.4.tar", max compression
+gzip compressed data, was "icd_mappings-0.1.5.tar", max compression
```

## Comparing `icd_mappings-0.1.4.tar` & `icd_mappings-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,29 @@
--rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.1.4/README.md
--rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.4/icdmappings/__init__.py
--rw-r--r--   0        0        0     2132 2023-04-26 14:04:37.870674 icd_mappings-0.1.4/icdmappings/icdmappings.py
--rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.4/icdmappings/mappers/__init__.py
--rw-r--r--   0        0        0     1916 2023-04-26 14:01:46.741546 icd_mappings-0.1.4/icdmappings/mappers/icd10_to_icd9.py
--rw-r--r--   0        0        0     2465 2023-04-26 14:02:22.394668 icd_mappings-0.1.4/icdmappings/mappers/icd9_to_cci.py
--rw-r--r--   0        0        0     4793 2023-04-26 14:02:40.764706 icd_mappings-0.1.4/icdmappings/mappers/icd9_to_ccs.py
--rw-r--r--   0        0        0     3351 2023-04-26 14:00:55.494895 icd_mappings-0.1.4/icdmappings/mappers/icd9_to_chapters.py
--rw-r--r--   0        0        0     1987 2023-04-26 14:01:15.042461 icd_mappings-0.1.4/icdmappings/mappers/icd9_to_icd10.py
--rw-r--r--   0        0        0      760 2023-04-26 14:01:27.386173 icd_mappings-0.1.4/icdmappings/mappers/icd9_to_level3.py
--rw-r--r--   0        0        0     1096 2023-03-15 14:45:47.834508 icd_mappings-0.1.4/icdmappings/mappers/lol.ipynb
--rw-r--r--   0        0        0      491 2023-04-26 14:00:22.255137 icd_mappings-0.1.4/icdmappings/mappers/mapper_interface.py
--rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.4/icdmappings/validators/__init__.py
--rw-r--r--   0        0        0     3264 2023-04-26 14:04:23.901528 icd_mappings-0.1.4/icdmappings/validators/icd9_validator.py
--rw-r--r--   0        0        0      735 2023-04-26 14:32:56.238228 icd_mappings-0.1.4/icdmappings/validators/icd_validator_interface.py
--rw-r--r--   0        0        0      600 2023-04-26 14:32:50.891198 icd_mappings-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 icd_mappings-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.1.5/README.md
+-rw-r--r--   0        0        0     6148 2023-03-13 09:43:51.822806 icd_mappings-0.1.5/data_sources/.DS_Store
+-rw-r--r--   0        0        0   106285 2021-07-12 11:47:18.000000 icd_mappings-0.1.5/data_sources/CCS-SingleDiagnosisGrouper.txt
+-rw-r--r--   0        0        0   897559 2023-04-26 11:30:37.278877 icd_mappings-0.1.5/data_sources/ICD-9-CM-v32-master-descriptions/CMS32_DESC_LONG_DX.txt
+-rw-r--r--   0        0        0   182309 2023-03-31 16:11:55.490825 icd_mappings-0.1.5/data_sources/ICD-9-CM-v32-master-descriptions/CMS32_DESC_LONG_SG.txt
+-rw-r--r--   0        0        0   418158 2013-06-13 10:42:38.000000 icd_mappings-0.1.5/data_sources/ICD-9-CM-v32-master-descriptions/CMS32_DESC_SHORT_DX.txt
+-rw-r--r--   0        0        0   107145 2013-06-26 12:34:24.000000 icd_mappings-0.1.5/data_sources/ICD-9-CM-v32-master-descriptions/CMS32_DESC_SHORT_SG.txt
+-rw-r--r--   0        0        0      311 2023-03-13 09:49:16.855619 icd_mappings-0.1.5/data_sources/ICD-9-CM-v32-master-descriptions/readme.md
+-rw-r--r--   0        0        0        0 2023-03-13 11:37:06.004050 icd_mappings-0.1.5/data_sources/__init__.py
+-rw-r--r--   0        0        0   629547 2022-06-20 16:29:42.984515 icd_mappings-0.1.5/data_sources/cci2015.csv
+-rw-r--r--   0        0        0  2766948 2022-09-21 16:12:43.000000 icd_mappings-0.1.5/data_sources/icd10cmtoicd9gem.csv
+-rw-r--r--   0        0        0     1087 2021-07-19 15:30:56.000000 icd_mappings-0.1.5/data_sources/icd9-CM-code-chapter-en=PT.csv
+-rw-r--r--   0        0        0  1427817 2022-06-23 13:00:01.514335 icd_mappings-0.1.5/data_sources/icd9dx2015.csv
+-rw-r--r--   0        0        0   821109 2022-06-21 13:09:55.045319 icd_mappings-0.1.5/data_sources/icd9toicd10cmgem.csv
+-rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.5/icdmappings/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-26 14:04:37.870674 icd_mappings-0.1.5/icdmappings/icdmappings.py
+-rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.5/icdmappings/mappers/__init__.py
+-rw-r--r--   0        0        0     1973 2023-04-27 15:33:19.770238 icd_mappings-0.1.5/icdmappings/mappers/icd10_to_icd9.py
+-rw-r--r--   0        0        0     2521 2023-04-27 15:33:25.171671 icd_mappings-0.1.5/icdmappings/mappers/icd9_to_cci.py
+-rw-r--r--   0        0        0     4847 2023-04-27 15:28:55.683724 icd_mappings-0.1.5/icdmappings/mappers/icd9_to_ccs.py
+-rw-r--r--   0        0        0     3408 2023-04-27 15:31:56.787678 icd_mappings-0.1.5/icdmappings/mappers/icd9_to_chapters.py
+-rw-r--r--   0        0        0     2044 2023-04-27 15:32:58.934201 icd_mappings-0.1.5/icdmappings/mappers/icd9_to_icd10.py
+-rw-r--r--   0        0        0      760 2023-04-27 15:23:41.254667 icd_mappings-0.1.5/icdmappings/mappers/icd9_to_level3.py
+-rw-r--r--   0        0        0      491 2023-04-26 14:00:22.255137 icd_mappings-0.1.5/icdmappings/mappers/mapper_interface.py
+-rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.5/icdmappings/validators/__init__.py
+-rw-r--r--   0        0        0     3363 2023-04-27 15:36:03.890673 icd_mappings-0.1.5/icdmappings/validators/icd9_validator.py
+-rw-r--r--   0        0        0      735 2023-04-26 14:39:04.763355 icd_mappings-0.1.5/icdmappings/validators/icd_validator_interface.py
+-rw-r--r--   0        0        0      652 2023-04-27 15:38:41.347187 icd_mappings-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 icd_mappings-0.1.5/PKG-INFO
```

### Comparing `icd_mappings-0.1.4/README.md` & `icd_mappings-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.4/icdmappings/icdmappings.py` & `icd_mappings-0.1.5/icdmappings/icdmappings.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd10_to_icd9.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd10_to_icd9.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import csv
 from typing import Union
+import pkg_resources
 
 class ICD10toICD9(MapperInterface):
     """
     Maps icd10 codes to icd9.
     
     Source of mapping: https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings
     """
     def __init__(self):
         self.path2file = "data_sources/icd10cmtoicd9gem.csv"
         self._setup()
 
     def _setup(self):
+        current_file_path = pkg_resources.resource_filename(__name__, '')
         filepath = os.path.join(
             os.path.dirname(
-            os.path.dirname(
-            os.path.dirname(os.path.abspath(__file__)))),
+            os.path.dirname(current_file_path)),
                 self.path2file
         )
         
         self.icd10_to_icd9 = self._parse_file(filepath)
 
 
     def _map_single(self, icd10code : str):
```

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd9_to_cci.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd9_to_cci.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import List, Union
 import os
 from collections.abc import Iterable
 import csv
+import pkg_resources
 
 class ICD9toCCI:
         """
         Maps icd9 diagnostic codes to chronic or not chronic (that is the question).
         
         source of mapping: https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp
         """
         def __init__(self):
             self.path2file = "data_sources/cci2015.csv"
-
             self.icd9_to_cci = None # will be filled by self._setup() {icd9code:cci,...icd9code:cci}
             self._setup()
 
 
         def _setup(self):
+            current_file_path = pkg_resources.resource_filename(__name__, '')
             filepath = os.path.join(
                 os.path.dirname(
-                os.path.dirname(
-                os.path.dirname(os.path.abspath(__file__)))),
+                os.path.dirname(current_file_path)),
                   self.path2file
             )
 
             # creates self.chapters_num, self.chapters_char, self.bins
             self.icd9_to_cci = self._parse_file(filepath)
```

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd9_to_ccs.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd9_to_ccs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from typing import List, Union
 import os
 from collections.abc import Iterable
 import re
-
+import pkg_resources
 from .mapper_interface import MapperInterface
 
 class ICD9toCCS(MapperInterface):
         """
         Maps icd9 codes to CCS groups
         
         source of mapping: https://www.hcup-us.ahrq.gov/toolssoftware/ccs/ccs.jsp
         """
         def __init__(self):
-
             self.path2file = "data_sources/CCS-SingleDiagnosisGrouper.txt"
             self._setup()
 
 
         def _setup(self):
+            current_file_path = pkg_resources.resource_filename(__name__, '')
             self.path2file = os.path.join(
                 os.path.dirname(
-                os.path.dirname(
-                os.path.dirname(os.path.abspath(__file__)))),
+                os.path.dirname(current_file_path)),
                   self.path2file
             )
-             
+            
             # {ccs:[icd9,...],..., ccs:[icd9,...]}
             self.ccs_to_icd9 = self._parse_file(self.path2file)
 
             # (inverse mapping): {icd9:ccs,..., icd9:ccs}
             self.icd9_to_ccs = self.ccs_to_icd9 = {self.ccs_to_icd9[ccs][i]:ccs for ccs in self.ccs_to_icd9 for i in range(len(self.ccs_to_icd9[ccs]))} 
         
         def _parse_file(self, filepath : str):
```

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd9_to_chapters.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd9_to_chapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import List,Union
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import bisect
 import csv
+import pkg_resources
 
 class ICD9toChapters(MapperInterface):
         """
         Maps icd9 diagnostic codes to icd9 chapters.
         
         source of mapping: https://icd.codes/icd9cm
         """
         def __init__(self):
             self.path2file = "data_sources/icd9-CM-code-chapter-en=PT.csv"
             self._setup()
 
         def _setup(self):
+            current_file_path = pkg_resources.resource_filename(__name__, '')
             filepath = os.path.join(
                 os.path.dirname(
-                os.path.dirname(
-                os.path.dirname(os.path.abspath(__file__)))),
+                os.path.dirname(current_file_path)),
                   self.path2file
             )
 
             # creates self.chapters_num, self.chapters_char, self.bins
             self.bins, self.char_mapping = self._parse_file(filepath)
```

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd9_to_icd10.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd9_to_icd10.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import csv
 from typing import Union
+import pkg_resources
 
 
 class ICD9toICD10(MapperInterface):
     """
     Maps icd9 codes into icd10.
     
     
     Source of mapping: https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings
     """
     def __init__(self):
         self.path2file = "data_sources/icd9toicd10cmgem.csv"
         self._setup()
 
     def _setup(self):
+        current_file_path = pkg_resources.resource_filename(__name__, '')
         filepath = os.path.join(
             os.path.dirname(
-            os.path.dirname(
-            os.path.dirname(os.path.abspath(__file__)))),
+            os.path.dirname(current_file_path)),
                 self.path2file
         )
 
         # creates self.chapters_num, self.chapters_char, self.bins
         self.icd9_to_icd10 = self._parse_file(filepath)
 
     def map(self,icd9code : Union[str, Iterable]):
```

### Comparing `icd_mappings-0.1.4/icdmappings/mappers/icd9_to_level3.py` & `icd_mappings-0.1.5/icdmappings/mappers/icd9_to_level3.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.4/icdmappings/validators/icd9_validator.py` & `icd_mappings-0.1.5/icdmappings/validators/icd9_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from .icd_validator_interface import ICDValidatorInterface
 from typing import List, Union
 import os
 from collections.abc import Iterable
+import pkg_resources
 
 
 class ICD9Validator(ICDValidatorInterface):
         """
         Checks if a code is icd9-cm version 32 compliant.
         """
         
         def __init__(self):
             self.path2folder = "data_sources/ICD-9-CM-v32-master-descriptions"
             self._setup()
         
         def _setup(self):
-             self.path2folder = os.path.join(
-                 os.path.dirname(
+            current_file_path = pkg_resources.resource_filename(__name__, '')
+            self.path2folder = os.path.join(
                    os.path.dirname(
-                   os.path.dirname(os.path.abspath(__file__)))
-                 ), self.path2folder)
-             self.diagnostics = self._parse_diagnostics()
-             self.procedures = self._parse_procedures()
-             pass
+                    os.path.dirname(
+                        current_file_path)
+                   ),
+                   self.path2folder)
+            self.diagnostics = self._parse_diagnostics()
+            self.procedures = self._parse_procedures()
+            pass
         
 
         def validate_diagnostics(self, 
                                 codes : Union[str,Iterable],
                                 ) -> Union[bool, Iterable]:
             """validates if a code or iterable of codes are valid diagnostics.
             If iterable is numpy or pd.Series, returns the same type. ALl other iterables are returned as List.
```

### Comparing `icd_mappings-0.1.4/icdmappings/validators/icd_validator_interface.py` & `icd_mappings-0.1.5/icdmappings/validators/icd_validator_interface.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.4/pyproject.toml` & `icd_mappings-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "icd-mappings"
-version = "0.1.4"
+version = "0.1.5"
 description = "This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))"
 authors = ["Simao Novais <snovaisg.97@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/snovaisg/ICDMappings"
 packages = [{include = "icdmappings"}]
+include = ["data_sources/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+setuptools = "^67.7.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `icd_mappings-0.1.4/PKG-INFO` & `icd_mappings-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: icd-mappings
-Version: 0.1.4
+Version: 0.1.5
 Summary: This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))
 Home-page: https://github.com/snovaisg/ICDMappings
 License: MIT
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Project-URL: Repository, https://github.com/snovaisg/ICDMappings
 Description-Content-Type: text/markdown
 
 # ICDMappings
 
 This tool helps working with ICD codes. It maps between ICD versions (such as between ICD9 and ICD10). Also maps to other codings such as CCS (Computer Software Classification), and CCI (Chronic Condition Indicator).
```


# Comparing `tmp/pytsv-0.1.67.tar.gz` & `tmp/pytsv-0.1.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsv-0.1.67.tar", last modified: Sun Sep 12 17:18:17 2021, max compression
+gzip compressed data, was "pytsv-0.1.68.tar", last modified: Thu Apr 27 08:15:05 2023, max compression
```

## Comparing `pytsv-0.1.67.tar` & `pytsv-0.1.68.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-09-12 17:18:17.668350 pytsv-0.1.67/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2017-11-26 05:05:03.000000 pytsv-0.1.67/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1394 2021-09-12 17:18:17.668350 pytsv-0.1.67/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      298 2021-09-12 17:18:03.000000 pytsv-0.1.67/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-09-12 17:18:17.667350 pytsv-0.1.67/pytsv/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:56:13.000000 pytsv-0.1.67/pytsv/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     8327 2021-09-08 17:44:47.000000 pytsv-0.1.67/pytsv/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    10675 2021-09-08 18:35:44.000000 pytsv-0.1.67/pytsv/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)    28582 2021-09-12 17:17:47.000000 pytsv-0.1.67/pytsv/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2021-09-12 17:18:03.000000 pytsv-0.1.67/pytsv/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-09-12 17:18:17.668350 pytsv-0.1.67/pytsv.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1394 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      296 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       51 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2021-09-12 17:18:17.000000 pytsv-0.1.67/pytsv.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2021-09-12 17:18:17.668350 pytsv-0.1.67/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1678 2021-09-12 17:18:03.000000 pytsv-0.1.67/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:15:05.534929 pytsv-0.1.68/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:14:51.000000 pytsv-0.1.68/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1344 2023-04-27 08:15:05.534929 pytsv-0.1.68/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      397 2023-04-27 08:14:51.000000 pytsv-0.1.68/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:15:05.533929 pytsv-0.1.68/pytsv/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:56:13.000000 pytsv-0.1.68/pytsv/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     8432 2022-06-18 06:36:22.000000 pytsv-0.1.68/pytsv/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    10640 2023-04-22 07:36:46.000000 pytsv-0.1.68/pytsv/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    28521 2023-04-27 08:14:36.000000 pytsv-0.1.68/pytsv/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-27 08:14:51.000000 pytsv-0.1.68/pytsv/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:15:05.534929 pytsv-0.1.68/pytsv.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1344 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      292 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       51 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-27 08:15:05.000000 pytsv-0.1.68/pytsv.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:15:05.534929 pytsv-0.1.68/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1598 2023-04-27 08:14:51.000000 pytsv-0.1.68/setup.py
```

### Comparing `pytsv-0.1.67/PKG-INFO` & `pytsv-0.1.68/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pytsv
-Version: 0.1.67
-Summary: pytsv is a module to help with all things TSV
+Version: 0.1.68
+Summary: Pytsv is a the Swiss army knife for TSV files
 Home-page: https://veltzer.github.io/pytsv
+Download-URL: https://github.com/veltzer/pytsv
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pytsv
-Description: =======
-        *pytsv*
-        =======
-        
-        .. image:: https://img.shields.io/pypi/v/pytsv
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pytsv
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pytsv
-        
-        author: Mark Veltzer
-        
-        version: 0.1.67
-        
-        
-        
 Keywords: python,tsv,format,csv
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=======
+*pytsv*
+=======
+
+.. image:: https://img.shields.io/pypi/v/pytsv
+
+.. image:: https://img.shields.io/github/license/veltzer/pytsv
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pytsv
+
+author: Mark Veltzer
+
+version: 0.1.68
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytsv-0.1.67/pytsv/configs.py` & `pytsv-0.1.68/pytsv/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+""" configuration for this project """
+
+
 import multiprocessing
 
 from pytconf import ParamCreator, Config
 
 CHECK_NON_ASCII = False
 SKIP_COMMENTS = False
 VALIDATE_ALL_LINES_SAME_NUMBER_OF_FIELDS = True
@@ -14,14 +17,16 @@
 CHECK_NUM_FIELDS = True
 CONVERT_TO_STRING = True
 DO_GZIP = False
 FILENAME_DETECT = True
 DEFAULT_ENCODING = 'utf-8'
 ATTACH_ENCODER = False
 
+# pylint: disable=too-few-public-methods
+
 
 class ConfigInputFiles(Config):
     """
     Parameters to specify input files
     """
     input_files = ParamCreator.create_list_str(
         help_string="input files",
@@ -172,15 +177,16 @@
 
 
 class ConfigCsvToTsv(Config):
     """
     Parameters to control the CSV to TSV conversion process
     """
     set_max = ParamCreator.create_bool(
-        help_string="do you want to unset the limit on csv fields (good for large fielded csv files)",
+        help_string="""do you want to unset the limit on csv fields \
+                (good for large fielded csv files)""",
         default=True,
     )
     replace_tabs_with_spaces = ParamCreator.create_bool(
         help_string="do you want to replace tabs with spaces?",
         default=True,
     )
     check_num_fields = ParamCreator.create_bool(
```

### Comparing `pytsv-0.1.67/pytsv/core.py` & `pytsv-0.1.68/pytsv/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gzip
 import itertools
 import logging
 import re
 from collections import defaultdict
-from typing import Iterable, List, Tuple, Dict, IO, Text, Union, Sequence
+from typing import Iterable, List, Dict, Union, Sequence, Optional, Any, IO, Generator, TextIO
 
 import pyanyzip.core
 
 from pytsv.configs import SANITIZE, CLEAN_EDGES, SUB_TRAILING, REMOVE_NON_ASCII, LOWER_CASE, CHECK_NUM_FIELDS, \
     CONVERT_TO_STRING, FILENAME_DETECT, DO_GZIP, USE_ANY_FORMAT, SKIP_COMMENTS, \
     CHECK_NON_ASCII, VALIDATE_ALL_LINES_SAME_NUMBER_OF_FIELDS
 
@@ -45,41 +45,41 @@
     :param input_file_names:
     :param match_columns:
     :param aggregate_columns:
     :param output_file_name:
     :param floating_point:
     :return:
     """
-    counts: Dict[Tuple[str], List[Union[int, float]]] = {}
+    counts: Dict[str, List[Union[int, float]]] = {}
     logger = logging.getLogger(__name__)
     for input_file_name in input_file_names:
         logger.debug(f"working on file [{input_file_name}]")
         with TsvReader(filename=input_file_name) as input_handle:
             for fields in input_handle:
-                match: Tuple[str] = tuple(fields[i] for i in match_columns)
-                if match not in counts:
+                m = "-".join(str(fields[i]) for i in match_columns)
+                if m not in counts:
                     if floating_point:
-                        counts[match] = [float(0)] * len(aggregate_columns)
+                        counts[m] = [float(0)] * len(aggregate_columns)
                     else:
-                        counts[match] = [int(0)] * len(aggregate_columns)
+                        counts[m] = [int(0)] * len(aggregate_columns)
                 for i, aggregate_column in enumerate(aggregate_columns):
                     if floating_point:
-                        counts[match][i] += float(fields[aggregate_column])
+                        counts[m][i] += float(fields[aggregate_column])
                     else:
-                        counts[match][i] += int(fields[aggregate_column])
+                        counts[m][i] += int(fields[aggregate_column])
     # notice that we create a writer that does not check the number
     # of fields because the check requires a len(fields) to be available
     # and it is not in this case because of itertools.chain
     with TsvWriter(
         filename=output_file_name,
         check_num_fields=False,
         sanitize=False,
     ) as output_file_handle:
-        for match, aggregates in counts.items():
-            to_write = list(itertools.chain(match, aggregates))
+        for m, aggregates in counts.items():
+            to_write = list(itertools.chain(m, aggregates))
             output_file_handle.write(to_write)
 
 
 def write_data(data: List[List[str]], output_file_name: str) -> None:
     with TsvWriter(
         filename=output_file_name,
         mode="at",
@@ -99,77 +99,81 @@
     logger = logging.getLogger(__name__)
     for input_file_name in input_file_names:
         logger.debug(f"working on file [{input_file_name}]")
         with open(input_file_name, 'rt') as file_handle:
             for line in file_handle:
                 line = line.rstrip()
                 parts: List[str] = line.split("\t")
-                match_tup: Tuple[str] = tuple(parts[i] for i in group_by_columns)
-                match = "_".join(match_tup)
+                m = "-".join(parts[i] for i in group_by_columns)
                 data_to_append = [parts[i] for i in collect_columns]
-                all_data[match].append(data_to_append)
-                if len(all_data[match]) > limit:
-                    write_data(all_data[match], output_file_template.format(match=match))
-                    all_data[match] = []
+                all_data[m].append(data_to_append)
+                if len(all_data[m]) > limit:
+                    write_data(all_data[m], output_file_template.format(m=m))
+                    all_data[m] = []
     # write the rest for the data
-    for match, data in all_data.items():
-        write_data(data, output_file_template.format(match=match))
-    return [output_file_template.format(match=match) for match in all_data]
+    for m, data in all_data.items():
+        write_data(data, output_file_template.format(m=m))
+    return [output_file_template.format(m=m) for match in all_data]
 
 
 def is_ascii(s: str) -> bool:
     return all(ord(c) < 128 for c in s)
 
 
 class TsvWriter:
     def __init__(
         self,
         filename: str,
         mode: str = "wt",
         throw_exceptions: bool = False,
 
         sanitize: bool = SANITIZE,
-        fields_to_clean: List[int] = None,
+        fields_to_clean: Optional[List[int]] = None,
         clean_edges: bool = CLEAN_EDGES,
         sub_trailing: bool = SUB_TRAILING,
         remove_non_ascii: bool = REMOVE_NON_ASCII,
         lower_case: bool = LOWER_CASE,
 
         check_num_fields: bool = CHECK_NUM_FIELDS,
-        num_fields: int = None,
+        num_fields: Optional[int] = None,
         convert_to_string: bool = CONVERT_TO_STRING,
 
         do_gzip: bool = DO_GZIP,
         filename_detect: bool = FILENAME_DETECT,
     ) -> None:
+        self.io: IO[Any]
+        self.io_text: TextIO
         if filename_detect:
             found = False
             if filename.endswith(".tsv.gz"):
-                self.io: IO[str] = gzip.open(filename, mode=mode)
+                self.io_gzip = gzip.open(filename, mode=mode)
                 found = True
             if filename.endswith(".tsv"):
                 # pylint: disable=consider-using-with
-                self.io: IO[str] = open(filename, mode=mode)
+                self.io = open(filename, mode=mode)
                 found = True
             if not found:
                 # treat as tsv
                 # pylint: disable=consider-using-with
-                self.io: IO[str] = open(filename, mode=mode)
+                self.io = open(filename, mode=mode)
             # old code, be more strict
             # assert found, "file name unknown"
         else:
             if do_gzip:
-                self.io: IO[str] = gzip.open(filename, mode=mode)
+                self.io_gzip = gzip.open(filename, mode=mode)
             else:
                 # pylint: disable=consider-using-with
-                self.io: IO[str] = open(filename, mode=mode)
+                self.io = open(filename, mode=mode)
         self.throw_exceptions = throw_exceptions
 
         self.sanitize = sanitize
-        self.fields_to_clean = fields_to_clean
+        if fields_to_clean is None:
+            self.fields_to_clean = []
+        else:
+            self.fields_to_clean = fields_to_clean
         if self.fields_to_clean is None:
             self.fields_to_clean = []
         self.clean_edges = clean_edges
         self.sub_trailing = sub_trailing
         self.remove_non_ascii = remove_non_ascii
         self.lower_case = lower_case
 
@@ -187,15 +191,15 @@
                     sub_trailing=self.sub_trailing,
                     remove_non_ascii=self.remove_non_ascii,
                     lower_case=self.lower_case,
                 )
             return r
         return seq
 
-    def _convert(self, seq: Sequence[str]) -> Sequence[str]:
+    def _convert(self, seq: Sequence[str]) -> Generator[str, None, None]:
         if self.convert_to_string:
             for t in seq:
                 if type(t) in (int, float, type(None)):
                     yield str(t)
                 else:
                     yield t
         else:
@@ -204,16 +208,18 @@
 
     def write(self, input_list: Sequence[str]) -> None:
         sanitized_list = self._sanitize(input_list)
         if self.check_num_fields:
             if self.num_fields is None:
                 self.num_fields = len(sanitized_list)
             else:
-                assert len(sanitized_list) == self.num_fields, "wrong number of fields in {}".format(sanitized_list)
-        print("\t".join(self._convert(sanitized_list)), file=self.io)
+                assert len(sanitized_list) == self.num_fields, f"wrong number of fields in {sanitized_list}"
+        buf = "\t".join(self._convert(sanitized_list))
+        self.io.write(buf.encode())
+        # print("\t".join(self._convert(sanitized_list)), file=self.io)
 
     def close(self) -> None:
         self.io.close()
 
     def __enter__(self):
         """ method needed to be a context manager """
         return self
@@ -243,42 +249,36 @@
         self.validate_all_lines_same_number_of_fields = validate_all_lines_same_number_of_fields
         self.num_fields = num_fields
         self.skip_comments = skip_comments
         self.check_non_ascii = check_non_ascii
 
         self.line_number = -1
 
-    def next(self):
-        return self.__next__()
-
-    def __next__(self) -> List[Text]:
+    def __next__(self) -> List[str]:
         """ method needed to be an iterator """
         self.line_number += 1
         line = self.io.readline()
         if not line:
             raise StopIteration
         if self.skip_comments:
             while line.startswith("#"):
                 self.line_number += 1
                 line = self.io.readline()
                 if not line:
                     raise StopIteration
         line = line.rstrip('\r\n')
         if self.check_non_ascii:
-            assert is_ascii(line), "non ascii characters in line [{}]".format(self.line_number)
+            assert is_ascii(line), f"non ascii characters in line [{self.line_number}]"
         fields = line.split('\t')
         if self.validate_all_lines_same_number_of_fields:
             if self.num_fields is None:
                 self.num_fields = len(fields)
             else:
-                assert len(fields) == self.num_fields, "wrong number of fields in line number {} {} {}".format(
-                    self.line_number,
-                    self.num_fields,
-                    len(fields),
-                )
+                assert len(fields) == self.num_fields, f"""wrong number of fields in line\
+                        number {self.line_number} {self.num_fields} {len(fields)}"""
         if self.check_non_ascii:
             assert is_ascii(line)
         return fields
 
     def __iter__(self):
         """ method needed to be an iterator """
         return self
@@ -291,11 +291,11 @@
         """ method needed to be a context manager """
         self.close()
 
     def close(self) -> None:
         self.io.close()
 
 
-def write_dict(filename: str = None, d: Dict[str, str] = None) -> None:
+def write_dict(filename: str, d: Dict[str, str]) -> None:
     with TsvWriter(filename=filename, num_fields=2, fields_to_clean=[0]) as output_handle:
         for k, v in d.items():
             output_handle.write([k, v])
```

### Comparing `pytsv-0.1.67/pytsv/main.py` & `pytsv-0.1.68/pytsv/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 import numpy.random
 import pandas
 import pyanyzip.core
 import pylogconf.core
 import tqdm
 from pytconf import register_endpoint, register_main, config_arg_parse_and_launch
 
-from pytsv.configs import ConfigInputFiles, ConfigFloatingPoint, ConfigAggregateColumns, ConfigMatchColumns, \
-    ConfigOutputFile, ConfigProgress, ConfigParallel, ConfigNumFields, ConfigTsvReader, ConfigColumns, \
-    ConfigInputFile, ConfigFixTypes, ConfigColumn, ConfigBucketNumber, ConfigMajority, ConfigCsvToTsv, ConfigJoin, \
+from pytsv.configs import ConfigInputFiles, ConfigFloatingPoint, ConfigAggregateColumns, \
+    ConfigMatchColumns, ConfigOutputFile, ConfigProgress, ConfigParallel, ConfigNumFields, \
+    ConfigTsvReader, ConfigColumns, ConfigInputFile, ConfigFixTypes, ConfigColumn, \
+    ConfigBucketNumber, ConfigMajority, ConfigCsvToTsv, ConfigJoin, \
     ConfigTree, ConfigSampleByColumnOld, ConfigSampleByTwoColumns, ConfigPattern, \
-    ConfigSampleSize, ConfigReplace, ConfigSampleColumn, ConfigWeightValue, ConfigCheckUnique
+    ConfigSampleSize, ConfigReplace, ConfigWeightValue, ConfigCheckUnique
 from pytsv.core import TsvReader, TsvWriter, clean, do_aggregate
-from pytsv.static import APP_NAME, VERSION_STR
+from pytsv.static import APP_NAME, VERSION_STR, DESCRIPTION
 
 # The next line is because pylint complains about pandas objects
 # pylint: disable=unsubscriptable-object,no-member
 
 
 @register_endpoint(
     description="aggregate TSV files",
@@ -54,15 +55,15 @@
         self.num_fields = None
         self.validate_all_lines_same_number_of_fields = None
         self.check_non_ascii = None
         self.progress = None
 
 
 def check_file(params_for_job: ParamsForJob) -> bool:
-    print('checking [{}]...'.format(params_for_job.input_file))
+    print(f"checking [{params_for_job.input_file}]...")
     with TsvReader(filename=params_for_job.input_file,
                    num_fields=params_for_job.num_fields,
                    validate_all_lines_same_number_of_fields=params_for_job.validate_all_lines_same_number_of_fields,
                    check_non_ascii=params_for_job.check_non_ascii) as input_file_handle:
         if params_for_job.progress:
             input_file_handle = tqdm.tqdm(input_file_handle)
         for _ in input_file_handle:
@@ -116,32 +117,28 @@
     configs=[
         ConfigProgress,
         ConfigInputFiles,
         ConfigColumns,
     ],
 )
 def check_columns_unique() -> None:
-    dicts = [{} for _ in range(len(ConfigColumns.columns))]
+    dicts: List[Dict[str, int]] = [{} for _ in range(len(ConfigColumns.columns))]
     errors = False
     for input_file in ConfigInputFiles.input_files:
         with TsvReader(
             filename=input_file,
         ) as input_file_handle:
             if ConfigProgress.progress:
                 input_file_handle = tqdm.tqdm(input_file_handle, desc=input_file)
             for line_number, fields in enumerate(input_file_handle):
                 for i, column in enumerate(ConfigColumns.columns):
                     value = fields[column]
                     if value in dicts[i]:
                         line = dicts[i][value]
-                        print("value [{}] is duplicate on lines [{}, {}]".format(
-                            value,
-                            line,
-                            line_number,
-                        ))
+                        print(f"value [{value}] is duplicate on lines [{line}, {line_number}]")
                         errors = True
                     else:
                         dicts[i][value] = line_number
     assert errors is False, "found errors"
 
 
 @register_endpoint(
@@ -281,28 +278,29 @@
 )
 def majority() -> None:
     """
     This means that if x1 appears more
     with y2 than any other values in column Y then x1, y2 will be in the output
     and no other entry with x1 will appear
     """
-    d: Dict[Dict[str, int]] = defaultdict(dict)
+    d: Dict[str, Dict[int, int]] = defaultdict(dict)
     with TsvReader(filename=ConfigInputFile.input_file) as input_file_handle:
         if ConfigProgress.progress:
             input_file_handle = tqdm.tqdm(input_file_handle)
         for fields in input_file_handle:
             p_first = fields[ConfigMajority.input_first_column]
-            p_second = fields[ConfigMajority.input_second_column]
+            p_second = int(fields[ConfigMajority.input_second_column])
             p_multiplication = int(fields[ConfigMajority.input_multiplication_column])
             if p_second not in d[p_first]:
                 d[p_first][p_second] = 0
             d[p_first][p_second] += p_multiplication
     with TsvWriter(filename=ConfigOutputFile.output_file) as output_file_handle:
         for p_first, p_dict in d.items():
-            p_second = max(p_dict.keys(), key=lambda x, closure_dict=p_dict: closure_dict[x])
+            # p_second = max(p_dict.keys(), key=lambda x: x, closure_dict=p_dict: closure_dict[x])
+            p_second = max(p_dict.keys())
             p_count = p_dict[p_second]
             output_file_handle.write([
                 p_first,
                 p_second,
                 str(p_count),
             ])
 
@@ -429,17 +427,17 @@
             else:
                 if ConfigJoin.output_add_unknown:
                     event_unknown_added += 1
                     fields.insert(ConfigJoin.output_insert_column, "unknown")
                     output_file_handle.write(fields)
                 else:
                     event_discarded += 1
-    print("event_found {}".format(event_found))
-    print("event_unknown_added {}".format(event_unknown_added))
-    print("event_discarded {}".format(event_discarded))
+    print(f"event_found {event_found}")
+    print(f"event_unknown_added {event_unknown_added}")
+    print(f"event_discarded {event_discarded}")
 
 
 @register_endpoint(
     description="lower case some columns",
     configs=[
         ConfigInputFile,
         ConfigOutputFile,
@@ -463,15 +461,15 @@
     configs=[
         ConfigInputFile,
         ConfigColumns,
         ConfigProgress,
     ],
 )
 def sum_columns() -> None:
-    sums = [0] * len(ConfigColumns.columns)
+    sums: List[float] = [0] * len(ConfigColumns.columns)
     with TsvReader(filename=ConfigInputFile.input_file) as input_file_handle:
         if ConfigProgress.progress:
             input_file_handle = tqdm.tqdm(input_file_handle)
         for fields in input_file_handle:
             for n, i in enumerate(ConfigColumns.columns):
                 sums[n] += float(fields[i])
     print(sums)
@@ -558,15 +556,15 @@
         ConfigTree,
     ],
 )
 def tree() -> None:
     """
     You can also see only parts of the tree
     """
-    children_dict: Dict[Set] = defaultdict(set)
+    children_dict: Dict[str, Set] = defaultdict(set)
     parents_dict = defaultdict(set)
     with TsvReader(filename=ConfigInputFile.input_file) as input_file_handle:
         for fields in input_file_handle:
             p_parent = fields[ConfigTree.parent_column]
             p_child = fields[ConfigTree.child_column]
             children_dict[p_parent].add(p_child)
             parents_dict[p_child].add(p_parent)
@@ -590,15 +588,15 @@
     # lets draw the tree
     while len(stack) > 0:
         name, depth, last, print_list = stack.pop()
         if last:
             special_string = "└──"
         else:
             special_string = "├──"
-        print("{}{}".format(print_list + special_string, name))
+        print(f"{print_list+special_string}{name}")
         first = True
         list_to_append = []
         for p_child in children_dict[name]:
             if last:
                 special_string = "   "
             else:
                 special_string = "│  "
@@ -644,15 +642,15 @@
         header=None,
     )
     if ConfigCheckUnique.check_unique:
         logger.info("checking that the values are unique")
         unique_values_count = df[ConfigWeightValue.value_column].nunique()
         if unique_values_count != df.shape[0]:
             logger.error("your data is not unique in the value_column")
-            logger.error("unique values {} != number of rows {}".format(unique_values_count, df.shape[0]))
+            logger.error(f"unique values {unique_values_count} != number of rows {df.shape[0]}")
             return
     logger.info("sampling")
     sample = df.sample(
         n=ConfigSampleSize.size,
         replace=ConfigReplace.replace,
         weights=df[ConfigWeightValue.weight_column],
     )
@@ -671,47 +669,47 @@
         ConfigInputFile,
         ConfigOutputFile,
         ConfigProgress,
         ConfigSampleByColumnOld,
     ],
 )
 def sample_by_column_old() -> None:
-    weights = []
-    elements = []
+    weights: List[float] = []
+    elements: List[List[str]] = []
     sum_weights = float(0)
     with TsvReader(ConfigInputFile.input_file) as input_handle:
         if ConfigProgress.progress:
             input_handle = tqdm.tqdm(input_handle)
         for fields in input_handle:
             elements.append(fields)
-            weight = float(fields[ConfigSampleColumn.sample_column])
+            weight = float(fields[ConfigSampleByColumnOld.sample_column])
             sum_weights += weight
             weights.append(weight)
     # the following code will only work on python3.6 because the
     # random.choices API was only introduced then
     # from random import choices
     # results = choices(lines, weights, k=size)
 
     # this is the same code with numpy
     weights = [w / sum_weights for w in weights]
     if ConfigSampleByColumnOld.hits_mode:
-        results_dict = defaultdict(int)
+        results_dict: Dict[int, int] = defaultdict(int)
         for _ in range(ConfigSampleSize.size):
-            current_result = numpy.random.choice(
+            current_results = numpy.random.choice(
                 a=len(elements),
                 replace=ConfigReplace.replace,
                 size=1,
                 p=weights,
             )
-            current_result = current_result[0]
+            current_result = current_results[0]
             results_dict[current_result] += 1
         with TsvWriter(ConfigOutputFile.output_file) as output_handle:
             for result, hits in results_dict.items():
                 record = list(elements[result])
-                record.append(hits)
+                record.append(str(hits))
                 output_handle.write(record)
     else:
         results = numpy.random.choice(
             a=len(elements),
             replace=ConfigReplace.replace,
             size=ConfigSampleSize.size,
             p=weights,
@@ -738,15 +736,15 @@
         sep='\t',
         header=None,
     )
     logger.info("checking that the values are unique")
     unique_values_count = df[ConfigWeightValue.value_column].nunique()
     if ConfigCheckUnique.check_unique and unique_values_count != df.shape[0]:
         logger.error("your data is not unique in the value_column")
-        logger.error("unique values {} != number of rows {}".format(unique_values_count, df.shape[0]))
+        logger.error(f"unique values {unique_values_count} != number of rows {df.shape[0]}")
         return
     logger.info("finding clusters")
     clusters = df[ConfigSampleByTwoColumns.group_column].unique()
     if ConfigProgress.progress:
         clusters = tqdm.tqdm(clusters)
     if os.path.isfile(ConfigOutputFile.output_file):
         os.unlink(ConfigOutputFile.output_file)
@@ -797,15 +795,15 @@
                 output_handle.write(fields)
     # close all writers
     for v in tsv_writers_dict.values():
         v.close()
 
 
 @register_main(
-    main_description="Pytsv is the Swiss Army Knife for TSV",
+    main_description=DESCRIPTION,
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     pylogconf.core.setup()
     config_arg_parse_and_launch()
```

### Comparing `pytsv-0.1.67/pytsv.egg-info/PKG-INFO` & `pytsv-0.1.68/pytsv.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pytsv
-Version: 0.1.67
-Summary: pytsv is a module to help with all things TSV
+Version: 0.1.68
+Summary: Pytsv is a the Swiss army knife for TSV files
 Home-page: https://veltzer.github.io/pytsv
+Download-URL: https://github.com/veltzer/pytsv
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pytsv
-Description: =======
-        *pytsv*
-        =======
-        
-        .. image:: https://img.shields.io/pypi/v/pytsv
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pytsv
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pytsv
-        
-        author: Mark Veltzer
-        
-        version: 0.1.67
-        
-        
-        
 Keywords: python,tsv,format,csv
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=======
+*pytsv*
+=======
+
+.. image:: https://img.shields.io/pypi/v/pytsv
+
+.. image:: https://img.shields.io/github/license/veltzer/pytsv
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pytsv
+
+author: Mark Veltzer
+
+version: 0.1.68
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


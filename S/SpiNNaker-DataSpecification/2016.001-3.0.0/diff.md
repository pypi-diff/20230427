# Comparing `tmp/SpiNNaker_DataSpecification-2016.001.zip` & `tmp/SpiNNaker_DataSpecification-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,35 +1,35 @@
-Zip file size: 55927 bytes, number of entries: 33
--rw-rw-rw-  2.0 fat      290 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/PKG-INFO
--rw-rw-rw-  2.0 fat     1452 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/README
--rw-rw-rw-  2.0 fat       64 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/setup.cfg
--rw-rw-rw-  2.0 fat      613 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/setup.py
--rw-rw-rw-  2.0 fat      873 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/constants.py
--rw-rw-rw-  2.0 fat     8651 b- defN 16-Apr-19 10:49 SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor.py
--rw-rw-rw-  2.0 fat    19448 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor_functions.py
--rw-rw-rw-  2.0 fat   150594 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_generator.py
--rw-rw-rw-  2.0 fat    17909 b- defN 16-Apr-19 10:49 SpiNNaker_DataSpecification-2016.001/data_specification/exceptions.py
--rw-rw-rw-  2.0 fat     2311 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/memory_region.py
--rw-rw-rw-  2.0 fat     2231 b- defN 16-Apr-01 15:18 SpiNNaker_DataSpecification-2016.001/data_specification/memory_region_collection.py
--rw-rw-rw-  2.0 fat      491 b- defN 16-Apr-19 10:49 SpiNNaker_DataSpecification-2016.001/data_specification/utility_calls.py
--rw-rw-rw-  2.0 fat     2180 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-2016.001/data_specification/__init__.py
--rw-rw-rw-  2.0 fat      261 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/command.py
--rw-rw-rw-  2.0 fat     1272 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/commands.py
--rw-rw-rw-  2.0 fat      256 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/constants.py
--rw-rw-rw-  2.0 fat    26340 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_executor.aplx
--rw-rw-rw-  2.0 fat     1596 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender.py
--rw-rw-rw-  2.0 fat     1580 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender_functions.py
--rw-rw-rw-  2.0 fat     3295 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/spec_sender.py
--rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/__init__.py
--rw-rw-rw-  2.0 fat      558 b- defN 16-Apr-01 15:18 SpiNNaker_DataSpecification-2016.001/data_specification/enums/arithemetic_operation.py
--rw-rw-rw-  2.0 fat     5448 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/enums/commands.py
--rw-rw-rw-  2.0 fat      948 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/enums/condition.py
--rw-rw-rw-  2.0 fat     6867 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-2016.001/data_specification/enums/data_type.py
--rw-rw-rw-  2.0 fat      638 b- defN 16-Apr-01 15:18 SpiNNaker_DataSpecification-2016.001/data_specification/enums/logic_operation.py
--rw-rw-rw-  2.0 fat      388 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-2016.001/data_specification/enums/random_number_generator.py
--rw-rw-rw-  2.0 fat       24 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-2016.001/data_specification/enums/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat      290 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       44 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     1393 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       19 b- defN 16-Apr-28 13:51 SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/top_level.txt
-33 files, 258325 bytes uncompressed, 48195 bytes compressed:  81.3%
+Zip file size: 56631 bytes, number of entries: 33
+-rw-rw-rw-  2.0 fat      287 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/PKG-INFO
+-rw-rw-rw-  2.0 fat     1452 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/README
+-rw-rw-rw-  2.0 fat       64 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/setup.cfg
+-rw-rw-rw-  2.0 fat      616 b- defN 16-Sep-01 19:32 SpiNNaker_DataSpecification-3.0.0/setup.py
+-rw-rw-rw-  2.0 fat      873 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/constants.py
+-rw-rw-rw-  2.0 fat     9205 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor.py
+-rw-rw-rw-  2.0 fat    20568 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor_functions.py
+-rw-rw-rw-  2.0 fat   151330 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_generator.py
+-rw-rw-rw-  2.0 fat    17909 b- defN 16-Apr-19 10:49 SpiNNaker_DataSpecification-3.0.0/data_specification/exceptions.py
+-rw-rw-rw-  2.0 fat     2825 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region.py
+-rw-rw-rw-  2.0 fat     2383 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region_collection.py
+-rw-rw-rw-  2.0 fat      491 b- defN 16-Apr-19 10:49 SpiNNaker_DataSpecification-3.0.0/data_specification/utility_calls.py
+-rw-rw-rw-  2.0 fat     2180 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-3.0.0/data_specification/__init__.py
+-rw-rw-rw-  2.0 fat      342 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/command.py
+-rw-rw-rw-  2.0 fat     1272 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/commands.py
+-rw-rw-rw-  2.0 fat      256 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/constants.py
+-rw-rw-rw-  2.0 fat    26340 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_executor.aplx
+-rw-rw-rw-  2.0 fat     1961 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender.py
+-rw-rw-rw-  2.0 fat     1809 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender_functions.py
+-rw-rw-rw-  2.0 fat     3580 b- defN 16-Sep-01 15:01 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/spec_sender.py
+-rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/__init__.py
+-rw-rw-rw-  2.0 fat      558 b- defN 16-Apr-01 15:18 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/arithemetic_operation.py
+-rw-rw-rw-  2.0 fat     5448 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/commands.py
+-rw-rw-rw-  2.0 fat      948 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/condition.py
+-rw-rw-rw-  2.0 fat     6867 b- defN 16-Apr-01 15:20 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/data_type.py
+-rw-rw-rw-  2.0 fat      638 b- defN 16-Apr-01 15:18 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/logic_operation.py
+-rw-rw-rw-  2.0 fat      388 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/random_number_generator.py
+-rw-rw-rw-  2.0 fat       24 b- defN 15-Jun-24 21:22 SpiNNaker_DataSpecification-3.0.0/data_specification/enums/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat      287 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       49 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat     1393 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat       19 b- defN 16-Sep-02 09:02 SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/top_level.txt
+33 files, 262363 bytes uncompressed, 49097 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -1,100 +1,100 @@
-Filename: SpiNNaker_DataSpecification-2016.001/PKG-INFO
+Filename: SpiNNaker_DataSpecification-3.0.0/PKG-INFO
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/README
+Filename: SpiNNaker_DataSpecification-3.0.0/README
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/setup.cfg
+Filename: SpiNNaker_DataSpecification-3.0.0/setup.cfg
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/setup.py
+Filename: SpiNNaker_DataSpecification-3.0.0/setup.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/constants.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/constants.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor_functions.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor_functions.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_generator.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_generator.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/exceptions.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/exceptions.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/memory_region.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/memory_region_collection.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region_collection.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/utility_calls.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/utility_calls.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/__init__.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/__init__.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/command.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/command.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/commands.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/commands.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/constants.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/constants.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_executor.aplx
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_executor.aplx
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender_functions.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender_functions.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/spec_sender.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/spec_sender.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/__init__.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/__init__.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/arithemetic_operation.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/arithemetic_operation.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/commands.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/commands.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/condition.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/condition.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/data_type.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/data_type.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/logic_operation.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/logic_operation.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/random_number_generator.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/random_number_generator.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/data_specification/enums/__init__.py
+Filename: SpiNNaker_DataSpecification-3.0.0/data_specification/enums/__init__.py
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/dependency_links.txt
+Filename: SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/dependency_links.txt
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/PKG-INFO
+Filename: SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/PKG-INFO
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/requires.txt
+Filename: SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/requires.txt
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/SOURCES.txt
+Filename: SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/SOURCES.txt
 Comment: 
 
-Filename: SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/top_level.txt
+Filename: SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `SpiNNaker_DataSpecification-2016.001/README` & `SpiNNaker_DataSpecification-3.0.0/README`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/constants.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/constants.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,36 @@
 
 
 class DataSpecificationExecutor(object):
     """ Used to execute a data specification language file to produce a memory\
         image
     """
 
+    __slots__ = [
+        # The object to read the specification language file
+        "spec_reader",
+
+        # The object to write the memory image to
+        "mem_writer",
+
+        # The object to write the report of the data specification executor
+        "report_writer",
+
+        # The amount of space used by the dsg script.
+        "space_used",
+
+        # the amount of space written by the dsg script (different from used,
+        # as empty data regions are not counted as written)
+        "space_written",
+
+        # ???????????
+        "dsef"
+
+    ]
+
     def __init__(self, spec_reader, mem_writer, memory_space,
                  report_writer=None):
         """
         :param spec_reader: The object to read the specification language file\
                     from
         :type spec_reader:\
                     :py:class:`data_specification.abstract_data_reader.\
@@ -68,20 +90,20 @@
 
             opcode = (cmd >> 20) & 0xFF
 
             try:
                 # noinspection PyArgumentList
                 return_value = \
                     commands.Commands(opcode).exec_function(self.dsef, cmd)
-            except ValueError as e:
+            except ValueError:
                 traceback.print_exc()
                 raise exceptions.DataSpecificationException(
                     "Invalid command 0x{0:X} while reading file {1:s}".format(
                         cmd, self.spec_reader.filename))
-            except TypeError as e:
+            except TypeError:
                 traceback.print_exc()
                 raise exceptions.DataSpecificationException(
                     "Invalid command 0x{0:X} while reading file {1:s}".format(
                         cmd, self.spec_reader.filename))
 
             if return_value == constants.END_SPEC_EXECUTOR:
                 break
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_executor_functions.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_executor_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,71 @@
 from data_specification import constants, exceptions, memory_region_collection
 import struct
 from data_specification.memory_region import MemoryRegion
 
 
-class DataSpecificationExecutorFunctions:
+class DataSpecificationExecutorFunctions(object):
     """ This class includes the function related to each of the commands\
         of the data specification file.
     """
 
+    __slots__ = [
+
+        # ????????????
+        "spec_reader",
+
+        # ????????????
+        "mem_writer",
+
+        # ????????????
+        "memory_space",
+
+        # ????????????
+        "space_allocated",
+
+        # ????????????
+        "current_region",
+
+        # ????????????
+        "registers",
+
+        # ????????????
+        "mem_regions",
+
+        # ????????????
+        "struct_slots",
+
+        # ????????????
+        "_cmd_size",
+
+        # ????????????
+        "opcode",
+
+        # ????????????
+        "use_dest_reg",
+
+        # ????????????
+        "use_src1_reg",
+
+        # ????????????
+        "use_src2_reg",
+
+        # ????????????
+        "dest_reg",
+
+        # ????????????
+        "src1_reg",
+
+        # ????????????
+        "src2_reg",
+
+        # ????????????
+        "data_len"
+    ]
+
     def __init__(self, spec_reader, mem_writer, memory_space):
         """
 
         :param spec_reader: The object to read the specification language file\
             from
         :type spec_reader:\
             :py:class:`data_specification.abstract_data_reader.\
@@ -32,14 +86,25 @@
         self.current_region = None
 
         self.registers = [0] * constants.MAX_REGISTERS
         self.mem_regions = memory_region_collection.MemoryRegionCollection(
             constants.MAX_MEM_REGIONS)
         self.struct_slots = [0] * constants.MAX_STRUCT_SLOTS
 
+        # storage objects
+        self._cmd_size = None
+        self.opcode = None
+        self.use_dest_reg = None
+        self.use_src1_reg = None
+        self.use_src2_reg = None
+        self.dest_reg = None
+        self.src1_reg = None
+        self.src2_reg = None
+        self.data_len = None
+
     def __unpack_cmd__(self, cmd):
         """ Routine to unpack the command read from the data spec file. The\
         parameters of the command are stored in the class data
 
         :param cmd: The command read form the data spec file
         :type cmd: int
         :return: No value returned
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_specification_generator.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_specification_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,56 @@
 logger = logging.getLogger(__name__)
 
 
 class DataSpecificationGenerator(object):
     """ Used to generate a data specification language file that can be\
         executed to produce a memory image
     """
+
+    __slots__ = [
+        # The object to write the specification to
+        "spec_writer",
+
+        # the writer for the human readable report
+        "report_writer",
+
+        # ????????
+        "txt_indent",
+
+        # how many instructions has been executed ?????
+        "instruction_counter",
+
+        # ???????
+        "mem_slot",
+
+        # ???????
+        "function",
+
+        # ???????
+        "struct_slot",
+
+        # ????????
+        "rng",
+
+        # ????????
+        "random_distribution",
+
+        # ???????
+        "conditionals",
+
+        # the current dsg region we're writing to
+        "current_region",
+
+        # ?????????
+        "ongoing_function_definition",
+
+        # ????????
+        "ongoing_loop"
+    ]
+
     MAGIC_NUMBER = 0xAD130AD6
     VERSION = 1
 
     def __init__(self, spec_writer, report_writer=None):
         """
         :param spec_writer: The object to write the specification to
         :type spec_writer: Implementation of\
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/exceptions.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/exceptions.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/memory_region.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 
 class MemoryRegion(object):
     """ Memory region storage object
 
     """
 
+    __slots__ = [
+        # the write pointer position
+        "_mem_pointer",
+
+        # flag that states if the region is filled or not
+        "_unfilled",
+
+        # the amount of memory allocated to this dsg
+        "_allocated_size",
+
+        # the region address map????
+        "_region_data",
+
+        # the position in the memory where the writing is currently occurring
+        "_write_pointer",
+
+        # the max point where if written over, it will cause an error
+        "_max_write_pointer"
+    ]
+
     def __init__(self, memory_pointer, unfilled, size):
         """
 
         :param memory_pointer: the write pointer position
         :param unfilled: if the region needs to be filled when written
         :return: None
         :rtype: None
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/memory_region_collection.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/memory_region_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from data_specification import exceptions
 
 
 class MemoryRegionCollection(object):
     """Collection of memory regions.
     """
+
+    __slots__ = [
+
+        # the max number of regions available
+        "_n_regions",
+
+        # map of region id to region data
+        "_regions"
+    ]
+
     def __init__(self, n_regions):
         """Create a new MemoryRegionCollection with the given number of regions.
         """
         self._n_regions = n_regions
         self._regions = [None] * n_regions
 
     def __len__(self):
@@ -52,18 +62,18 @@
         :rtype: boolean
         :raise DataSpecificationNoRegionSelectedException: when the id is \
         beyond the expected region range
         """
         if region_id > self._n_regions:
             raise exceptions.DataSpecificationNoRegionSelectedException(
                 "the region id requested is beyond the supported number of"
-                "avilable region ids")
+                "available region ids")
         if not self._regions[region_id].unfilled:
             return True
         else:
             needs_writing = False
             for region in range(region_id, self._n_regions):
-                if (self._regions[region_id] is not None
-                        and not self._regions[region_id].unfilled):
+                if (self._regions[region] is not None and
+                        not self._regions[region].unfilled):
                     needs_writing = True
         return needs_writing
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/__init__.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/__init__.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/commands.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/commands.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_executor.aplx` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_executor.aplx`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,48 @@
 
 
 class DataSpecificationSender(object):
     """ Used to send a data specification language file to SpiNNaker to\
         produce a memory image
     """
 
-    """
-    :param spec_reader: Reads from the DSG file.
-    :type spec_reader: FileDataReader
-    :param spec_sender: Buffer used to send reliably data specification\
-                        commands to the SpiNNaker board.
-    :type spec_sender: SpecSender
-    :param report_writer: DSE report writer.
-    :return:
-    """
+    __slots__ = [
+        # reader for the spec file
+        "spec_reader",
+
+        # Buffer used to send reliably data specification commands to the
+        #  SpiNNaker board.
+        "spec_sender",
+
+        # report writer for human consumption
+        "report_writer",
+
+        # ?????????
+        "dssf"
+    ]
+
     def __init__(self, spec_reader, spec_sender, report_writer=None):
+        """
+        :param spec_reader: Reads from the DSG file.
+        :type spec_reader: FileDataReader
+        :param spec_sender: Buffer used to send reliably data specification\
+                            commands to the SpiNNaker board.
+        :type spec_sender: SpecSender
+        :param report_writer: DSE report writer.
+        :return:
+        """
         self.spec_reader = spec_reader
         self.spec_sender = spec_sender
         self.report_writer = report_writer
         self.dssf = Dssf(self.spec_reader, self.spec_sender)
 
-    """ Parse the data specification form self.spec_reader, split it into\
-        atomic chunks and send it using the spec_sender.
-    """
     def sendSpec(self):
+        """ Parse the data specification form self.spec_reader, split it into\
+            atomic chunks and send it using the spec_sender.
+        """
 
         # read a new command
         instruction_spec = self.spec_reader.read(4)
         while len(instruction_spec) != 0:
             # process the received command
             cmd = Command(struct.unpack("<I", str(instruction_spec))[0])
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/data_specification_sender_functions.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/data_specification_sender_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import struct
 import constants
 from command import Command
 from data_specification.data_spec_sender.commands import Commands
 
 
-class DataSpecificationSenderFunctions:
+class DataSpecificationSenderFunctions(object):
+
+    __slots__ = [
+        
+        # the reader for the spec file
+        "spec_reader",
+
+        # Buffer used to send reliably data specification commands to the
+        #  SpiNNaker board.
+        "spec_sender"
+    ]
 
     def __init__(self, spec_reader, spec_sender):
         self.spec_reader = spec_reader
         self.spec_sender = spec_sender
 
     def send_break(self, cmd):
         self.spec_sender.add(cmd.get_value())
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/data_spec_sender/spec_sender.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/data_spec_sender/spec_sender.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,35 @@
 from spinnman.messages.sdp.sdp_flag import SDPFlag
 
 import struct
 import constants
 import time
 
 
-class SpecSender:
+class SpecSender(object):
     """ Class for sending a data spec to a core.
         The data is added to a buffer using the add method and then sent using
         the send method.
     """
 
+    __slots__ = [
+        
+        # The transceiver used to communicate with the board.
+        "transceiver",
+
+        # The destination of the data specification.
+        "placement",
+
+        # ???????????
+        "header",
+
+        # ???????????
+        "msg_data"
+    ]
+
     def __init__(self, transceiver, placement):
         """ Create a new SpecSender
         :param transceiver: The transceiver used to communicate with the board.
         :type transceiver: Transceiver
         :param placement: The destination of the data specification.
         :type placement: Placement
         :return:
```

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/enums/arithemetic_operation.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/enums/arithemetic_operation.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/enums/commands.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/enums/commands.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/enums/condition.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/enums/condition.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/enums/data_type.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/enums/data_type.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/data_specification/enums/logic_operation.py` & `SpiNNaker_DataSpecification-3.0.0/data_specification/enums/logic_operation.py`

 * *Files identical despite different names*

## Comparing `SpiNNaker_DataSpecification-2016.001/SpiNNaker_DataSpecification.egg-info/SOURCES.txt` & `SpiNNaker_DataSpecification-3.0.0/SpiNNaker_DataSpecification.egg-info/SOURCES.txt`

 * *Files identical despite different names*


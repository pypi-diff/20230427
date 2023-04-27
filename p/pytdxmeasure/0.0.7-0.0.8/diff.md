# Comparing `tmp/pytdxmeasure-0.0.7-py3-none-any.whl.zip` & `tmp/pytdxmeasure-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 16576 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-25 03:05 pytdxmeasure/__init__.py
--rw-r--r--  2.0 unx     6498 b- defN 23-Feb-25 03:05 pytdxmeasure/actor.py
--rw-r--r--  2.0 unx     2827 b- defN 23-Feb-25 03:05 pytdxmeasure/binaryblob.py
--rw-r--r--  2.0 unx     3231 b- defN 23-Feb-25 03:05 pytdxmeasure/ccel.py
--rw-r--r--  2.0 unx     1816 b- defN 23-Feb-25 03:05 pytdxmeasure/cli.py
--rw-r--r--  2.0 unx      632 b- defN 23-Feb-25 03:05 pytdxmeasure/rtmr.py
--rw-r--r--  2.0 unx     8841 b- defN 23-Feb-25 03:05 pytdxmeasure/tdeventlog.py
--rw-r--r--  2.0 unx     7133 b- defN 23-Feb-25 03:05 pytdxmeasure/tdreport.py
--rwxr-xr-x  2.0 unx      108 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.data/scripts/tdx_eventlogs
--rwxr-xr-x  2.0 unx       78 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.data/scripts/tdx_tdreport
--rwxr-xr-x  2.0 unx       74 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.data/scripts/tdx_verify_rtmr
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1445 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1346 b- defN 23-Feb-25 03:05 pytdxmeasure-0.0.7.dist-info/RECORD
-16 files, 45491 bytes uncompressed, 14338 bytes compressed:  68.5%
+Zip file size: 21280 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 12:52 pytdxmeasure/__init__.py
+-rw-r--r--  2.0 unx     6498 b- defN 23-Feb-28 12:52 pytdxmeasure/actor.py
+-rw-r--r--  2.0 unx     2827 b- defN 23-Feb-28 12:52 pytdxmeasure/binaryblob.py
+-rw-r--r--  2.0 unx     3231 b- defN 23-Feb-28 12:52 pytdxmeasure/ccel.py
+-rw-r--r--  2.0 unx     2473 b- defN 23-Apr-26 12:45 pytdxmeasure/cli.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-Apr-26 12:45 pytdxmeasure/rtmr.py
+-rw-r--r--  2.0 unx     8841 b- defN 23-Feb-28 12:52 pytdxmeasure/tdeventlog.py
+-rw-r--r--  2.0 unx     8155 b- defN 23-Apr-27 07:19 pytdxmeasure/tdreport.py
+-rw-r--r--  2.0 unx     7914 b- defN 23-Apr-27 07:19 pytdxmeasure/utility.py
+-rwxr-xr-x  2.0 unx      108 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.data/scripts/tdx_eventlogs
+-rwxr-xr-x  2.0 unx      902 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.data/scripts/tdx_extend_rtmr
+-rwxr-xr-x  2.0 unx       78 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.data/scripts/tdx_tdreport
+-rwxr-xr-x  2.0 unx       74 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.data/scripts/tdx_verify_rtmr
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2971 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-27 07:19 pytdxmeasure-0.0.8.dist-info/RECORD
+18 files, 60416 bytes uncompressed, 18750 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -18,32 +18,38 @@
 
 Filename: pytdxmeasure/tdeventlog.py
 Comment: 
 
 Filename: pytdxmeasure/tdreport.py
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.data/scripts/tdx_eventlogs
+Filename: pytdxmeasure/utility.py
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.data/scripts/tdx_tdreport
+Filename: pytdxmeasure-0.0.8.data/scripts/tdx_eventlogs
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.data/scripts/tdx_verify_rtmr
+Filename: pytdxmeasure-0.0.8.data/scripts/tdx_extend_rtmr
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.dist-info/LICENSE
+Filename: pytdxmeasure-0.0.8.data/scripts/tdx_tdreport
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.dist-info/METADATA
+Filename: pytdxmeasure-0.0.8.data/scripts/tdx_verify_rtmr
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.dist-info/WHEEL
+Filename: pytdxmeasure-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.dist-info/top_level.txt
+Filename: pytdxmeasure-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pytdxmeasure-0.0.7.dist-info/RECORD
+Filename: pytdxmeasure-0.0.8.dist-info/WHEEL
+Comment: 
+
+Filename: pytdxmeasure-0.0.8.dist-info/top_level.txt
+Comment: 
+
+Filename: pytdxmeasure-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytdxmeasure/cli.py

```diff
@@ -3,15 +3,15 @@
 """
 
 from abc import abstractmethod
 import logging
 import logging.config
 from .actor import VerifyActor, TDEventLogActor
 from .tdreport import TdReport
-
+from .rtmr import RTMR
 from .ccel import CCEL
 
 __author__ = "cpio"
 
 LOG = logging.getLogger(__name__)
 
 
@@ -82,7 +82,28 @@
     def run(self):
         """
         Run cmd
         """
 
         LOG.info("=> Dump TD Report")
         TdReport.get_td_report().dump()
+
+class TDXRTMRExtendCmd():
+    """
+    Cmd executor to extend RTMR register
+    """
+
+    def __init__(self):
+        logging.basicConfig(level=logging.DEBUG, format='%(message)s')
+
+    @staticmethod
+    def run(extend_raw_data, extend_str_data, extend_digest_data, extend_rtmr_index):
+        """
+        Run cmd
+        """
+
+        LOG.info("=> Extend RTMR")
+        res = RTMR.extend_rtmr(extend_raw_data, extend_str_data,
+                               extend_digest_data, extend_rtmr_index)
+        if res == RTMR.EXTEND_SUCCESS:
+            LOG.info("Changed RTMR value in TD Report")
+            TdReport.get_td_report().dump()
```

## pytdxmeasure/rtmr.py

```diff
@@ -1,24 +1,90 @@
 """
 RTMR data structures
 """
 
+import os
+import fcntl
+import struct
+import logging
+import hashlib
 from .binaryblob import BinaryBlob
 
+__author__ = 'cpio'
+LOG = logging.getLogger(__name__)
 
 class RTMR(BinaryBlob):
     """
     Data structure for RTMR registers.
     A RTMR register manages a 48-bytes (384-bits) hash value.
     """
     RTMR_COUNT = 4
     RTMR_LENGTH_BY_BYTES = 48
+    TDX_ATTEST_FILE = '/dev/tdx_guest'
+    EXTEND_SUCCESS = 'RTMR_EXTEND_SUCCESS'
+    EXTEND_FAILURE = 'RTMR_EXTEND_FAILURE'
+    EXTEND_FAILURE_WITH_WRONG_INPUT = 'RTMR_EXTEND_FAILURE_WITH_WRONG_INPUT'
 
     def __init__(self, data: bytearray = bytearray(RTMR_LENGTH_BY_BYTES),
         base_addr=0):
         super().__init__(data, base_addr)
 
     def __eq__(self, other):
         bytearray_1, _ = self.get_bytes(0, RTMR.RTMR_LENGTH_BY_BYTES)
         bytearray_2, _ = other.get_bytes(0, RTMR.RTMR_LENGTH_BY_BYTES)
 
         return bytearray(bytearray_1) == bytearray(bytearray_2)
+
+    @staticmethod
+    def extend_rtmr(raw_extend_data, str_extend_data, digest_extend_data, extend_rtmr_index):
+        """
+        Perform ioctl on the device file /dev/tdx_guest to extend rtmr
+        """
+        if not os.path.exists(RTMR.TDX_ATTEST_FILE):
+            LOG.error("Could not find device node %s. Kernel version 6.2 above supports RTMR write",
+                      RTMR.TDX_ATTEST_FILE)
+            return None
+
+        try:
+            fd_tdx_attest = os.open(RTMR.TDX_ATTEST_FILE, os.O_RDWR)
+        except (PermissionError, IOError, OSError):
+            LOG.error("Fail to open file %s", RTMR.TDX_ATTEST_FILE)
+            return None
+
+        #Perform extend through ioctl call
+        #Reference: Structure of tdx_extend_rtmr_req in /include/uapi/linux/tdx-guest.h
+        #struct tdx_extend_rtmr_req {
+        #    __u8 data[TDX_EXTEND_RTMR_DATA_LEN];
+        #    __u8 index;
+        #};
+
+        extend_data = bytearray(64)
+
+        if str_extend_data is not None:
+            data_digest = hashlib.sha384(str_extend_data.encode())
+            extend_data = bytearray(data_digest.digest())
+        elif digest_extend_data is not None:
+            extend_data = bytearray.fromhex(digest_extend_data)
+            if len(extend_data) != RTMR.RTMR_LENGTH_BY_BYTES:
+                LOG.error("Invalid length for the extend data. Should be 48B length.")
+                return RTMR.EXTEND_FAILURE_WITH_WRONG_INPUT
+        else:
+            extend_data = bytearray(raw_extend_data.encode())
+            if len(extend_data) != RTMR.RTMR_LENGTH_BY_BYTES:
+                LOG.error("Invalid length for the extend data. Should be 48B length.")
+                return RTMR.EXTEND_FAILURE_WITH_WRONG_INPUT
+
+        req = struct.pack("@48sB", extend_data, int(extend_rtmr_index))
+
+        #Reference: command used for tdx rtmr extend defined in /include/uapi/linux/tdx-guest.h
+        #define TDX_CMD_EXTEND_RTMR		_IOR('T', 3, struct tdx_extend_rtmr_req)
+        try:
+            fcntl.ioctl(fd_tdx_attest,
+                        int.from_bytes(struct.pack('Hcb', 0x3180, b'T', 3), 'big'), req)
+        except OSError:
+            LOG.info("Fail to execute ioctl for file %s", RTMR.TDX_ATTEST_FILE)
+            os.close(fd_tdx_attest)
+            return RTMR.EXTEND_FAILURE
+
+        os.close(fd_tdx_attest)
+        LOG.info("RTMR extend success.")
+        return RTMR.EXTEND_SUCCESS
```

## pytdxmeasure/tdreport.py

```diff
@@ -1,20 +1,20 @@
 """
 Parse td report struct, see:
 https://software.intel.com/content/dam/develop/external/us/en/documents/tdx-module-1eas-v0.85.039.pdf  # pylint: disable=line-too-long
 https://software.intel.com/content/dam/develop/external/us/en/documents-tps/intel-tdx-cpu-architectural-specification.pdf  # pylint: disable=line-too-long
 """
 
-import os
 import logging
-import ctypes
-import struct
-import fcntl
-from .binaryblob import BinaryBlob
 
+from .utility import DeviceNode, \
+        DEVICE_NODE_NAME_DEPRECATED as DEV_DEPRECATED, \
+        DEVICE_NODE_NAME_1_0 as DEV_1_0, \
+        DEVICE_NODE_NAME_1_5 as DEV_1_5
+from .binaryblob import BinaryBlob
 
 __author__ = "cpio"
 
 LOG = logging.getLogger(__name__)
 
 
 class ReportMacStruct(BinaryBlob):
@@ -56,70 +56,95 @@
         self.cpusvn, offset = self.get_bytes(offset, 0x10)
         self.tee_tcb_info_hash, offset = self.get_bytes(offset, 0x30)
         self.tee_info_hash, offset = self.get_bytes(offset, 0x30)
         self.report_data, offset = self.get_bytes(offset, 0x40)
         self.reserverd2, offset = self.get_bytes(offset, 0x20)
         self.mac, offset = self.get_bytes(offset, 0x20)
 
-
 class TeeTcbInfo(BinaryBlob):
     """
     Struct TEE_TCB_INFO
     """
 
-    def __init__(self, data):
+    def __init__(self, data, device):
         super().__init__(data)
+        # auxiliary fileds
+        self.device = device
+        # real fields
         self.valid = None
         self.tee_tcb_svn = None
         self.mrseam = None
         self.mrsignerseam = None
         self.attributes = None
+        self.tee_tcb_svn2 = None
         self.reserved = None
         self.parse()
 
     def parse(self):
         """
         parse the raw data for Struct TEE_TCB_INFO
 
         Struct TEE_TCB_INFO's layout:
         offset, len
-        0x0,    0x8     valid
+        0x0,    0x08    valid
         0x8,    0x10    tee_tcb_svn
         0x18,   0x30    mrseam
         0x48,   0x30    mrsignerseam
-        0x78,   0x8     attributes
+        0x78,   0x08    attributes
+
+        # fileds in tdx v1.0
         0x80,   0x6f    reserved
+
+        # fileds in tdx v1.5
+        0x80,   0x10    tee_tcb_svn2
+        0x90,   0x5f    reserved
+
+        FIXME:  need spec reference to update info # pylint: disable=fixme
+                about new field tee_tcb_svn2
         """
+        if self.device == DEV_DEPRECATED:
+            LOG.error("Deprecated device node %s, please upgrade to use %s or %s",
+                      DEV_DEPRECATED, DEV_1_0, DEV_1_5)
+            return
+
         offset = 0
 
         self.valid, offset = self.get_bytes(offset, 0x8)
         self.tee_tcb_svn, offset = self.get_bytes(offset, 0x10)
         self.mrseam, offset = self.get_bytes(offset, 0x30)
         self.mrsignerseam, offset = self.get_bytes(offset, 0x30)
         self.attributes, offset = self.get_bytes(offset, 0x8)
-        self.reserved, offset = self.get_bytes(offset, 0x6f)
 
+        if  self.device == DEV_1_0:
+            self.reserved, offset = self.get_bytes(offset, 0x6f)
+        elif self.device == DEV_1_5:
+            self.tee_tcb_svn2, offset = self.get_bytes(offset, 0x10)
+            self.reserved, offset = self.get_bytes(offset, 0x5f)
 
 class TdInfo(BinaryBlob):
     """
     Struct TDINFO_STRUCT
     """
 
-    def __init__(self, data):
+    def __init__(self, data, device):
         super().__init__(data)
+        # auxiliary fileds
+        self.device = device
+        # read fields
         self.attributes = None
         self.xfam = None
         self.mrtd = None
         self.mrconfigid = None
         self.mrowner = None
         self.mrownerconfig = None
         self.rtmr_0 = None
         self.rtmr_1 = None
         self.rtmr_2 = None
         self.rtmr_3 = None
+        self.servtd_hash = None
         self.reserved = None
         self.parse()
 
     def parse(self):
         '''
         parse the raw data for Struct TDINFO_STRUCT
 
@@ -131,37 +156,63 @@
         0x40,   0x30    mrconfigid
         0x70,   0x30    mrowner
         0xa0,   0x30    mrownerconfig
         0xd0,   0x30    rtmr_0
         0x100,  0x30    rtmr_1
         0x130,  0x30    rtmr_2
         0x160,  0x30    rtmr_3
+
+        # fields in tdx v1.0
         0x190,  0x70    reserved
+
+        # fields in tdx v1.5
+        0x190,  0x30    servtd_hash
+        0x1c0,  0x40    reserved
+
+        ref:
+            Page 40 of Intel® TDX Module v1.5 ABI Specification
+            from https://www.intel.com/content/www/us/en/developer/articles/technical/
+            intel-trust-domain-extensions.html
         '''
+
+        if self.device == DEV_DEPRECATED:
+            LOG.error("Deprecated device node %s, please upgrade to use %s or %s",
+                      DEV_DEPRECATED, DEV_1_0, DEV_1_5)
+            return
+
         offset = 0
 
         self.attributes, offset = self.get_bytes(offset, 0x8)
         self.xfam, offset = self.get_bytes(offset, 0x8)
         self.mrtd, offset = self.get_bytes(offset, 0x30)
         self.mrconfigid, offset = self.get_bytes(offset, 0x30)
         self.mrowner, offset = self.get_bytes(offset, 0x30)
         self.mrownerconfig, offset = self.get_bytes(offset, 0x30)
         self.rtmr_0, offset = self.get_bytes(offset, 0x30)
         self.rtmr_1, offset = self.get_bytes(offset, 0x30)
         self.rtmr_2, offset = self.get_bytes(offset, 0x30)
         self.rtmr_3, offset = self.get_bytes(offset, 0x30)
 
+        if  self.device == DEV_1_0:
+            self.reserved, offset = self.get_bytes(offset, 0x70)
+        elif self.device == DEV_1_5:
+            self.servtd_hash, offset = self.get_bytes(offset, 0x30)
+            self.reserved, offset = self.get_bytes(offset, 0x40)
 
 class TdReport(BinaryBlob):
     """
     Struct TDREPORT_STRUCT
     """
-
-    def __init__(self, data):
+    def __init__(self, data, device_node=None):
         super().__init__(data)
+        # auxiliary fileds
+        if device_node is None:
+            device_node = DeviceNode()
+        self.device_node = device_node
+        # real fields in TDREPORT_STRUCT
         self.report_mac_struct = None
         self.tee_tcb_info = None
         self.reserved = None
         self.td_info = None
         self.parse()
 
     def parse(self):
@@ -171,68 +222,35 @@
         Struct TDREPORT_STRUCT's layout:
         offset, len
         0x0,    0x100   ReportMacStruct
         0x100,  0xef    TeeTcbInfo
         0x1ef,  0x11    Reserved
         0x200,  0x200   TdInfo
         '''
+        if self.device_node == DEV_DEPRECATED:
+            LOG.error("Deprecated device node %s, please upgrade to use %s or %s",
+                      DEV_DEPRECATED, DEV_1_0, DEV_1_5)
+            return
+
         offset = 0
 
         data, offset = self.get_bytes(offset, 0x100)
         self.report_mac_struct = ReportMacStruct(data)
-        self.report_mac_struct.parse()
 
         data, offset = self.get_bytes(offset, 0xef)
-        self.tee_tcb_info = TeeTcbInfo(data)
-        self.tee_tcb_info.parse()
+        self.tee_tcb_info = TeeTcbInfo(data, self.device_node.device_node_name)
 
         data, offset = self.get_bytes(offset, 0x11)
         self.reserved = data
 
         data, offset = self.get_bytes(offset, 0x200)
-        self.td_info = TdInfo(data)
-        self.td_info.parse()
+        self.td_info = TdInfo(data, self.device_node.device_node_name)
 
     @staticmethod
-    def get_td_report():
+    def get_td_report(report_data=None):
         """
-        Perform ioctl on the device file /dev/tdx-attes, to get td-report
+        Perform ioctl on the device file, to get td-report
         """
-        tdx_attest_file = '/dev/tdx-guest'
-        if not os.path.exists(tdx_attest_file):
-            LOG.error("Could not find device node %s", tdx_attest_file)
-            return None
-
-        try:
-            fd_tdx_attest = os.open(tdx_attest_file, os.O_RDWR)
-        except (PermissionError, IOError, OSError):
-            LOG.error("Fail to open file %s", tdx_attest_file)
-            return None
-
-        #
-        # Reference: Structure of tdx_report_req
-        #
-        # struct tdx_report_req {
-        #        __u8  subtype;
-        #        __u64 reportdata;
-        #        __u32 rpd_len;
-        #        __u64 tdreport;
-        #        __u32 tdr_len;
-        # };
-        #
-        reportdata = ctypes.create_string_buffer(64)
-        tdreport = ctypes.create_string_buffer(1024)
-
-        req = struct.pack("BQLQL", 0, ctypes.addressof(reportdata), 64,
-                          ctypes.addressof(tdreport), 1024)
-        try:
-            fcntl.ioctl(fd_tdx_attest,
-                int.from_bytes(struct.pack('Hcb', 0x08c0, b'T', 1), 'big'),
-                req)
-        except OSError:
-            LOG.error("Fail to execute ioctl for file %s", tdx_attest_file)
-            os.close(fd_tdx_attest)
-            return None
-        os.close(fd_tdx_attest)
-        report = TdReport(bytearray(tdreport))
-        report.parse()
+        device_node = DeviceNode()
+        tdreport_bytes = device_node.get_tdreport_bytes(report_data)
+        report = TdReport(tdreport_bytes, device_node)
         return report
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pytdxmeasure-0.0.7.dist-info/LICENSE` & `pytdxmeasure-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytdxmeasure-0.0.7.dist-info/RECORD` & `pytdxmeasure-0.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 pytdxmeasure/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytdxmeasure/actor.py,sha256=rMPWP28_GBmcxxprmKX0d5SCzEdlSsAG2irJf-G3ZVo,6498
 pytdxmeasure/binaryblob.py,sha256=bprsbPHjFTMYMyCU53ZFznBKS0yxeLHIdUueQV4D0sc,2827
 pytdxmeasure/ccel.py,sha256=wb4qEdiffnqXaPQao0iR0NwiXovQ3hasLsMXhFcRBRw,3231
-pytdxmeasure/cli.py,sha256=YNq8pvmFio-INCOQfQKxifjA9nmza3PdpAe03X0W4eU,1816
-pytdxmeasure/rtmr.py,sha256=-v1ZRivXAZYfdFRJIqpWw9NvdQUEWHhqm9ab8lFpOGI,632
+pytdxmeasure/cli.py,sha256=NwZ-LOKxfQE5gsB_fIxihJNupESbnl2E2swSxjP91vM,2473
+pytdxmeasure/rtmr.py,sha256=6ID1sRPxPtzxjAf2_dAucuRc3lwuPlpbXZQyrseLTrQ,3352
 pytdxmeasure/tdeventlog.py,sha256=fo2J2uEZb1QM_DZitIIz5DZm380fU-BlM9gyWDkVgKU,8841
-pytdxmeasure/tdreport.py,sha256=AfpCBzuOMxeGnga3H2xbnT_PJon5Oz8AJ4WNTgFaxg0,7133
-pytdxmeasure-0.0.7.data/scripts/tdx_eventlogs,sha256=1AwUMK9CXUjorwq2mvgz_W3_fDPkcpvxHXn3TiDVRUc,108
-pytdxmeasure-0.0.7.data/scripts/tdx_tdreport,sha256=SYLB1z5Tvd0YiKs4611jpad6am3CJPa4y1iI7r1-AJc,78
-pytdxmeasure-0.0.7.data/scripts/tdx_verify_rtmr,sha256=Sjb1YovSFqwR3ItIl4_tAWaNe5ToTIiVyN_mIyxUduE,74
-pytdxmeasure-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytdxmeasure-0.0.7.dist-info/METADATA,sha256=-WjDc58FmCLVlVNmB-jAN73wGQCws3U3bck8y1tXq6s,1445
-pytdxmeasure-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pytdxmeasure-0.0.7.dist-info/top_level.txt,sha256=lmm5CpLm0znxqki6CtGDeEv3-18ohYpxcUB4qpYJFp8,13
-pytdxmeasure-0.0.7.dist-info/RECORD,,
+pytdxmeasure/tdreport.py,sha256=3-fTuqlwyMS877FfFvlWJjvTACT2qtwVLryqpXR5TMc,8155
+pytdxmeasure/utility.py,sha256=V9jEfJRJxGgkJBBhOXyYClG1byeDYAKoq8wLmh2WNvQ,7914
+pytdxmeasure-0.0.8.data/scripts/tdx_eventlogs,sha256=1AwUMK9CXUjorwq2mvgz_W3_fDPkcpvxHXn3TiDVRUc,108
+pytdxmeasure-0.0.8.data/scripts/tdx_extend_rtmr,sha256=T9NAqgOjy_g8u647DFuPFSadn6MM_91i3AxVGRoi4xk,902
+pytdxmeasure-0.0.8.data/scripts/tdx_tdreport,sha256=SYLB1z5Tvd0YiKs4611jpad6am3CJPa4y1iI7r1-AJc,78
+pytdxmeasure-0.0.8.data/scripts/tdx_verify_rtmr,sha256=Sjb1YovSFqwR3ItIl4_tAWaNe5ToTIiVyN_mIyxUduE,74
+pytdxmeasure-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytdxmeasure-0.0.8.dist-info/METADATA,sha256=dXlWbYyrZO4slgKJkCiBniHVdllGxIgEf6u2AS6UtjY,2971
+pytdxmeasure-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytdxmeasure-0.0.8.dist-info/top_level.txt,sha256=lmm5CpLm0znxqki6CtGDeEv3-18ohYpxcUB4qpYJFp8,13
+pytdxmeasure-0.0.8.dist-info/RECORD,,
```


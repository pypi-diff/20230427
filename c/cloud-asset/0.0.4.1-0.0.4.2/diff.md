# Comparing `tmp/cloud_asset-0.0.4.1-py3-none-any.whl.zip` & `tmp/cloud_asset-0.0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 39077 bytes, number of entries: 34
+Zip file size: 40955 bytes, number of entries: 36
 -rw-rw-rw-  2.0 fat      102 b- defN 23-Jan-11 08:03 asset/__init__.py
 -rw-rw-rw-  2.0 fat      863 b- defN 23-Apr-24 03:08 asset/asset_register.py
 -rw-rw-rw-  2.0 fat     3680 b- defN 23-Feb-09 07:04 asset/asset_table.py
 -rw-rw-rw-  2.0 fat    16941 b- defN 23-Apr-27 03:27 asset/base.py
 -rw-rw-rw-  2.0 fat     3179 b- defN 23-Apr-26 06:24 asset/cli.py
 -rw-rw-rw-  2.0 fat     3068 b- defN 23-Apr-27 07:03 asset/commands.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 23-Apr-26 09:11 asset/conf.py
@@ -16,21 +16,23 @@
 -rw-rw-rw-  2.0 fat      167 b- defN 23-Apr-10 10:58 asset/aws/__init__.py
 -rw-rw-rw-  2.0 fat     4878 b- defN 23-Apr-10 10:58 asset/aws/cloudwatch.py
 -rw-rw-rw-  2.0 fat    11132 b- defN 23-Apr-14 07:50 asset/aws/ec2.py
 -rw-rw-rw-  2.0 fat     3055 b- defN 23-Apr-10 10:58 asset/aws/elb.py
 -rw-rw-rw-  2.0 fat     8620 b- defN 23-Apr-10 10:58 asset/aws/elb_v2.py
 -rw-rw-rw-  2.0 fat     9638 b- defN 23-Feb-10 09:11 asset/aws/rds.py
 -rw-rw-rw-  2.0 fat     3172 b- defN 23-Feb-09 08:29 asset/aws/s3.py
+-rw-rw-rw-  2.0 fat      134 b- defN 23-Apr-24 03:11 asset/huawei/__init__.py
+-rw-rw-rw-  2.0 fat     7068 b- defN 23-Apr-27 02:40 asset/huawei/ecs.py
 -rw-rw-rw-  2.0 fat      170 b- defN 23-Apr-10 10:58 asset/tencent/__init__.py
 -rw-rw-rw-  2.0 fat     2901 b- defN 23-Apr-10 10:58 asset/tencent/cdb_mysql.py
 -rw-rw-rw-  2.0 fat     2309 b- defN 23-Apr-10 10:58 asset/tencent/clb.py
 -rw-rw-rw-  2.0 fat     1804 b- defN 23-Apr-10 10:58 asset/tencent/cos.py
 -rw-rw-rw-  2.0 fat     2242 b- defN 23-Apr-10 10:58 asset/tencent/cvm.py
 -rw-rw-rw-  2.0 fat     3279 b- defN 23-Apr-10 10:58 asset/tencent/monitor.py
 -rw-rw-rw-  2.0 fat    11514 b- defN 23-Apr-17 06:58 asset/tencent/vpc.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1100 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2623 b- defN 23-Apr-27 09:11 cloud_asset-0.0.4.1.dist-info/RECORD
-34 files, 135605 bytes uncompressed, 34975 bytes compressed:  74.2%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1100 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2779 b- defN 23-Apr-27 09:23 cloud_asset-0.0.4.2.dist-info/RECORD
+36 files, 142963 bytes uncompressed, 36615 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -57,14 +57,20 @@
 
 Filename: asset/aws/rds.py
 Comment: 
 
 Filename: asset/aws/s3.py
 Comment: 
 
+Filename: asset/huawei/__init__.py
+Comment: 
+
+Filename: asset/huawei/ecs.py
+Comment: 
+
 Filename: asset/tencent/__init__.py
 Comment: 
 
 Filename: asset/tencent/cdb_mysql.py
 Comment: 
 
 Filename: asset/tencent/clb.py
@@ -78,26 +84,26 @@
 
 Filename: asset/tencent/monitor.py
 Comment: 
 
 Filename: asset/tencent/vpc.py
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/LICENSE
+Filename: cloud_asset-0.0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/METADATA
+Filename: cloud_asset-0.0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/WHEEL
+Filename: cloud_asset-0.0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/entry_points.txt
+Filename: cloud_asset-0.0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/top_level.txt
+Filename: cloud_asset-0.0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloud_asset-0.0.4.1.dist-info/RECORD
+Filename: cloud_asset-0.0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cloud_asset-0.0.4.1.dist-info/LICENSE` & `cloud_asset-0.0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cloud_asset-0.0.4.1.dist-info/METADATA` & `cloud_asset-0.0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-asset
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Cloud Asset - Asset For Postgres
 Author: Cloud Asset Authors
 Author-email: 
 License: Apache-2.0
 Requires-Python: >=3.7.1,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `cloud_asset-0.0.4.1.dist-info/RECORD` & `cloud_asset-0.0.4.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 asset/aws/__init__.py,sha256=iZDKcu1UVff75M_C5lcXNRMY3LaWBI2Pf7GPyRVqxwg,167
 asset/aws/cloudwatch.py,sha256=i06mf37R7wMn8bJZxflapOM3GHXTTZs1XNaQqr5xXmM,4878
 asset/aws/ec2.py,sha256=zgYBqNykB4ru5aECglT1EUss_e7xzUL0pdsp-n5Gca0,11132
 asset/aws/elb.py,sha256=b2sdi-XLiQ0f8p4sPCtC1mWAsGXAcrZ1XLoWiAcHi9Y,3055
 asset/aws/elb_v2.py,sha256=lnExSX3Fv06nrZPociCv5sEAewajDXqLX9Hdvme1kcg,8620
 asset/aws/rds.py,sha256=QOSIu3HJM44Ib28pbSHzt9BtBYx8ceN_bILBPAg0rTI,9638
 asset/aws/s3.py,sha256=lxBcZP8mh1dILGC4txB7chqu2ClA6sPB4U2xXeZxmpM,3172
+asset/huawei/__init__.py,sha256=9MHRH27pM6wItPM1NKxQNRYn0U-ZEu1LzXfac7x_0t0,134
+asset/huawei/ecs.py,sha256=WY1LI_oB7mNI_pg1iGl_nSPqGPAAGfO8p2awjLdcOLo,7068
 asset/tencent/__init__.py,sha256=_MsiCfmMqtiYhCoTa8Sj_hfOWme6me6fwr3v4uI0Hos,170
 asset/tencent/cdb_mysql.py,sha256=YJJqU8zyV33nE0TMUdFafg1Ata8y8pQL2A1989EiBJ8,2901
 asset/tencent/clb.py,sha256=AXSqB1BtSrW2RNhQtdGfJlAIWfpvUdVFoqALiPT3aio,2309
 asset/tencent/cos.py,sha256=muWkfEdF0mHAGPTXw5MkBc13FrK8UMt9-QxPcy6QsMw,1804
 asset/tencent/cvm.py,sha256=QKj4PKvxJrjffT0Vr6H9eS_m65EmZxidsba-Yqqteag,2242
 asset/tencent/monitor.py,sha256=gEnGh0QxESqp5aZZ-LzLT6nQADsfCqZJPFI5QKNqJyc,3279
 asset/tencent/vpc.py,sha256=3XKDVm1fu0Egrc0wv3jbH-n2nxSLLSBzxxcS69VaR_Y,11514
-cloud_asset-0.0.4.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-cloud_asset-0.0.4.1.dist-info/METADATA,sha256=_0ucCQgYhktACdFjvBQ39srbmWbzkAt7dI6ojPJVcls,1100
-cloud_asset-0.0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cloud_asset-0.0.4.1.dist-info/entry_points.txt,sha256=E98BNjat-vzRmq_JOsUw1BEUB8gGDXTCrge_EcO1ItQ,47
-cloud_asset-0.0.4.1.dist-info/top_level.txt,sha256=OOL4Q5O665etnevbCwltTM6xLZ_EIE3w81HrT-kZli8,6
-cloud_asset-0.0.4.1.dist-info/RECORD,,
+cloud_asset-0.0.4.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+cloud_asset-0.0.4.2.dist-info/METADATA,sha256=AV9EBTAR2-j4BnYnFMrQxPmsSRHgByYANamUC7uQg9I,1100
+cloud_asset-0.0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cloud_asset-0.0.4.2.dist-info/entry_points.txt,sha256=E98BNjat-vzRmq_JOsUw1BEUB8gGDXTCrge_EcO1ItQ,47
+cloud_asset-0.0.4.2.dist-info/top_level.txt,sha256=OOL4Q5O665etnevbCwltTM6xLZ_EIE3w81HrT-kZli8,6
+cloud_asset-0.0.4.2.dist-info/RECORD,,
```


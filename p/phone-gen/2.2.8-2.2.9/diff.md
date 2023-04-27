# Comparing `tmp/phone_gen-2.2.8-py3-none-any.whl.zip` & `tmp/phone_gen-2.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 34475 bytes, number of entries: 14
+Zip file size: 34507 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx     1030 b- defN 21-Dec-27 20:05 phone_gen/__init__.py
--rw-rw-r--  2.0 unx       34 b- defN 22-May-06 15:14 phone_gen/__version__.py
+-rw-rw-r--  2.0 unx       34 b- defN 22-Jun-14 00:27 phone_gen/__version__.py
 -rw-rw-r--  2.0 unx    10602 b- defN 22-Jan-05 19:28 phone_gen/_generator.py
 -rw-rw-r--  2.0 unx      562 b- defN 22-Jan-05 19:28 phone_gen/alt_patterns.py
 -rw-rw-r--  2.0 unx     1478 b- defN 22-Jan-05 19:28 phone_gen/cli.py
 -rw-rw-r--  2.0 unx    16602 b- defN 22-Jan-05 19:28 phone_gen/country_name.py
 -rw-rw-r--  2.0 unx     6932 b- defN 22-Jan-05 19:28 phone_gen/iso3.py
--rw-rw-r--  2.0 unx    87120 b- defN 22-May-31 13:27 phone_gen/patterns.py
--rw-rw-r--  2.0 unx     1067 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4223 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1121 b- defN 22-May-31 13:34 phone_gen-2.2.8.dist-info/RECORD
-14 files, 130923 bytes uncompressed, 32623 bytes compressed:  75.1%
+-rw-rw-r--  2.0 unx    87211 b- defN 22-Jun-14 00:27 phone_gen/patterns.py
+-rw-rw-r--  2.0 unx     1067 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4223 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1121 b- defN 22-Jun-14 00:27 phone_gen-2.2.9.dist-info/RECORD
+14 files, 131014 bytes uncompressed, 32655 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: phone_gen/iso3.py
 Comment: 
 
 Filename: phone_gen/patterns.py
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/LICENSE
+Filename: phone_gen-2.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/METADATA
+Filename: phone_gen-2.2.9.dist-info/METADATA
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/WHEEL
+Filename: phone_gen-2.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/entry_points.txt
+Filename: phone_gen-2.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/top_level.txt
+Filename: phone_gen-2.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: phone_gen-2.2.8.dist-info/RECORD
+Filename: phone_gen-2.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phone_gen/__version__.py

```diff
@@ -1,2 +1,2 @@
 # coding: utf-8
-version = "2.2.7"
+version = "2.2.9"
```

## phone_gen/patterns.py

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2022-05-31 13:07:51 UTC
-Resource: https://github.com/google/libphonenumber v8.12.49
+Auto-generated file 2022-06-13 23:22:41 UTC
+Resource: https://github.com/google/libphonenumber v8.12.50
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.12.49",
+    "info": "libphonenumber v8.12.50",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -51,16 +51,16 @@
         "AO": {
             "code": "244",
             "pattern": "((2[\\d]([0134][25-9])|([25-9][\\d])[\\d]{5}))",
             "mobile": "((9[1-59][\\d]{7}))",
         },
         "AR": {
             "code": "54",
-            "pattern": "((3888[013-9][\\d]{5})|((29(54)|(66))|(3(777)|(865))[2-8][\\d]{5})|(3(7(1[15])|(81))|(8(21)|(4[16])|(69)|(9[12]))[46][\\d]{5})|((2(2(2[59])|(44)|(52))|(3(26)|(44))|(473)|(9([07]2)|(2[26])|(34)|(46)))|(3327)[45][\\d]{5})|((2(284)|(302)|(657)|(920))|(3(4(8[27])|(92))|(541)|(755)|(878))[2-7][\\d]{5})|((2((26)|(62)2)|(32[03])|(477)|(9(42)|(83)))|(3(329)|(4([47]6)|(62)|(89))|(564))[2-6][\\d]{5})|(((11[1-8])|(670)[\\d])|(2(2(0[45])|(1[2-6])|(3[3-6]))|(3([06]4)|(7[45]))|(494)|(6(04)|(1[2-8])|([36][45])|(4[3-6]))|(80[45])|(9([17][4-6])|([48][45])|(9[3-6])))|(3(364)|(4(1[2-7])|([235][4-6])|(84))|(5(1[2-8])|([38][4-6]))|(6(2[45])|(44))|(7[069][45])|(8([03][45])|([17][2-6])|([58][3-6])))[\\d]{6})|(2(2(21)|(4[23])|(6[145])|(7[1-4])|(8[356])|(9[267]))|(3(16)|(3[13-8])|(43)|(5[346-8])|(9[3-5]))|(475)|(6(2[46])|(4[78])|(5[1568]))|(9(03)|(2[1457-9])|(3[1356])|(4[08])|([56][23])|(82))4[\\d]{5})|((2(2(57)|(81))|(3(24)|(46)|(92))|(9(01)|(23)|(64)))|(3(4(42)|(71))|(5(25)|(37)|(4[347])|(71))|(7(18)|(5[17])))[3-6][\\d]{5})|((2(2(02)|(2[3467])|(4[156])|(5[45])|(6[6-8])|(91))|(3(1[47])|(25)|([45][25])|(96))|(47[48])|(625)|(932))|(3(38[2578])|(4(0[0-24-9])|(3[78])|(4[457])|(58)|(6[03-9])|(72)|(83)|(9[136-8]))|(5(2[124])|([368][23])|(4[2689])|(7[2-6]))|(7(16)|(2[15])|(3[145])|(4[13])|(5[468])|(7[2-5])|(8[26]))|(8(2[5-7])|(3[278])|(4[3-5])|(5[78])|(6[1-378])|([78]7)|(94)))[4-6][\\d]{5}))",
-            "mobile": "((93888[013-9][\\d]{5})|(9(29(54)|(66))|(3(777)|(865))[2-8][\\d]{5})|(93(7(1[15])|(81))|(8(21)|(4[16])|(69)|(9[12]))[46][\\d]{5})|(9(2(2(2[59])|(44)|(52))|(3(26)|(44))|(473)|(9([07]2)|(2[26])|(34)|(46)))|(3327)[45][\\d]{5})|(9(2(284)|(302)|(657)|(920))|(3(4(8[27])|(92))|(541)|(755)|(878))[2-7][\\d]{5})|(9(2((26)|(62)2)|(32[03])|(477)|(9(42)|(83)))|(3(329)|(4([47]6)|(62)|(89))|(564))[2-6][\\d]{5})|((675[\\d])|(9(11[1-8][\\d])|(2(2(0[45])|(1[2-6])|(3[3-6]))|(3([06]4)|(7[45]))|(494)|(6(04)|(1[2-8])|([36][45])|(4[3-6]))|(80[45])|(9([17][4-6])|([48][45])|(9[3-6])))|(3(364)|(4(1[2-7])|([235][4-6])|(84))|(5(1[2-8])|([38][4-6]))|(6(2[45])|(44))|(7[069][45])|(8([03][45])|([17][2-6])|([58][3-6]))))[\\d]{6})|(92(2(21)|(4[23])|(6[145])|(7[1-4])|(8[356])|(9[267]))|(3(16)|(3[13-8])|(43)|(5[346-8])|(9[3-5]))|(475)|(6(2[46])|(4[78])|(5[1568]))|(9(03)|(2[1457-9])|(3[1356])|(4[08])|([56][23])|(82))4[\\d]{5})|(9(2(2(57)|(81))|(3(24)|(46)|(92))|(9(01)|(23)|(64)))|(3(4(42)|(71))|(5(25)|(37)|(4[347])|(71))|(7(18)|(5[17])))[3-6][\\d]{5})|(9(2(2(02)|(2[3467])|(4[156])|(5[45])|(6[6-8])|(91))|(3(1[47])|(25)|([45][25])|(96))|(47[48])|(625)|(932))|(3(38[2578])|(4(0[0-24-9])|(3[78])|(4[457])|(58)|(6[03-9])|(72)|(83)|(9[136-8]))|(5(2[124])|([368][23])|(4[2689])|(7[2-6]))|(7(16)|(2[15])|(3[145])|(4[13])|(5[468])|(7[2-5])|(8[26]))|(8(2[5-7])|(3[278])|(4[3-5])|(5[78])|(6[1-378])|([78]7)|(94)))[4-6][\\d]{5}))",
+            "pattern": "((3888[013-9][\\d]{5})|(3(7(1[15])|(81))|(8(21)|(4[16])|(69)|(9[12]))[46][\\d]{5})|((29(54)|(66))|(3(7(55)|(77))|(865))[2-8][\\d]{5})|((2(2(2[59])|(44)|(52))|(3(26)|(44))|(473)|(9([07]2)|(2[26])|(34)|(46)))|(3327)[45][\\d]{5})|((2(284)|(3(02)|(23))|(657)|(920))|(3(4(8[27])|(92))|(541)|(878))[2-7][\\d]{5})|((2((26)|(62)2)|(320)|(477)|(9(42)|(83)))|(3(329)|(4([47]6)|(62)|(89))|(564))[2-6][\\d]{5})|(((11[1-8])|(670)[\\d])|(2(2(0[45])|(1[2-6])|(3[3-6]))|(3([06]4)|(7[45]))|(494)|(6(04)|(1[2-8])|([36][45])|(4[3-6]))|(80[45])|(9([17][4-6])|([48][45])|(9[3-6])))|(3(364)|(4(1[2-7])|([235][4-6])|(84))|(5(1[2-9])|([38][4-6]))|(6(2[45])|(44))|(7[069][45])|(8(0[45])|([17][2-6])|(3[4-6])|([58][3-6])))[\\d]{6})|(2(2(21)|(4[23])|(6[145])|(7[1-4])|(8[356])|(9[267]))|(3(16)|(3[13-8])|(43)|(5[346-8])|(9[3-5]))|(475)|(6(2[46])|(4[78])|(5[1568]))|(9(03)|(2[1457-9])|(3[1356])|(4[08])|([56][23])|(82))4[\\d]{5})|((2(2(57)|(81))|(3(24)|(46)|(92))|(9(01)|(23)|(64)))|(3(4(42)|(71))|(5(25)|(37)|(4[347])|(71))|(7(18)|(5[17])))[3-6][\\d]{5})|((2(2(02)|(2[3467])|(4[156])|(5[45])|(6[6-8])|(91))|(3(1[47])|(25)|([45][25])|(96))|(47[48])|(625)|(932))|(3(38[2578])|(4(0[0-24-9])|(3[78])|(4[457])|(58)|(6[03-9])|(72)|(83)|(9[136-8]))|(5(2[124])|([368][23])|(4[2689])|(7[2-6]))|(7(16)|(2[15])|(3[145])|(4[13])|(5[468])|(7[2-5])|(8[26]))|(8(2[5-7])|(3[278])|(4[3-5])|(5[78])|(6[1-378])|([78]7)|(94)))[4-6][\\d]{5}))",
+            "mobile": "((93(7(1[15])|(81)[46])|(8((21)|(4[16])|(69)|(9[12])[46])|(88[013-9]))[\\d]{5})|(9(29(54)|(66))|(3(7(55)|(77))|(865))[2-8][\\d]{5})|(9(2(2(2[59])|(44)|(52))|(3(26)|(44))|(473)|(9([07]2)|(2[26])|(34)|(46)))|(3327)[45][\\d]{5})|(9(2(284)|(3(02)|(23))|(657)|(920))|(3(4(8[27])|(92))|(541)|(878))[2-7][\\d]{5})|(9(2((26)|(62)2)|(320)|(477)|(9(42)|(83)))|(3(329)|(4([47]6)|(62)|(89))|(564))[2-6][\\d]{5})|((675[\\d])|(9(11[1-8][\\d])|(2(2(0[45])|(1[2-6])|(3[3-6]))|(3([06]4)|(7[45]))|(494)|(6(04)|(1[2-8])|([36][45])|(4[3-6]))|(80[45])|(9([17][4-6])|([48][45])|(9[3-6])))|(3(364)|(4(1[2-7])|([235][4-6])|(84))|(5(1[2-9])|([38][4-6]))|(6(2[45])|(44))|(7[069][45])|(8(0[45])|([17][2-6])|(3[4-6])|([58][3-6]))))[\\d]{6})|(92(2(21)|(4[23])|(6[145])|(7[1-4])|(8[356])|(9[267]))|(3(16)|(3[13-8])|(43)|(5[346-8])|(9[3-5]))|(475)|(6(2[46])|(4[78])|(5[1568]))|(9(03)|(2[1457-9])|(3[1356])|(4[08])|([56][23])|(82))4[\\d]{5})|(9(2(2(57)|(81))|(3(24)|(46)|(92))|(9(01)|(23)|(64)))|(3(4(42)|(71))|(5(25)|(37)|(4[347])|(71))|(7(18)|(5[17])))[3-6][\\d]{5})|(9(2(2(02)|(2[3467])|(4[156])|(5[45])|(6[6-8])|(91))|(3(1[47])|(25)|([45][25])|(96))|(47[48])|(625)|(932))|(3(38[2578])|(4(0[0-24-9])|(3[78])|(4[457])|(58)|(6[03-9])|(72)|(83)|(9[136-8]))|(5(2[124])|([368][23])|(4[2689])|(7[2-6]))|(7(16)|(2[15])|(3[145])|(4[13])|(5[468])|(7[2-5])|(8[26]))|(8(2[5-7])|(3[278])|(4[3-5])|(5[78])|(6[1-378])|([78]7)|(94)))[4-6][\\d]{5}))",
         },
         "AS": {
             "code": "1",
             "pattern": "((6846(22)|(33)|(44)|(55)|(77)|(88)|(9[19])[\\d]{4}))",
             "mobile": "((684(2(48)|(5[2468])|(72))|(7(3[13])|(70)|(82))[\\d]{4}))",
         },
         "AT": {
@@ -226,16 +226,16 @@
         "CK": {
             "code": "682",
             "pattern": "(((2[\\d])|(3[13-7])|(4[1-5])[\\d]{3}))",
             "mobile": "(([578][\\d]{4}))",
         },
         "CL": {
             "code": "56",
-            "pattern": "((2(1982[0-6])|(3314[05-9])[\\d]{3})|((2(1(160)|(962))|(3(2[\\d][\\d])|(3([034][\\d])|(1[0-35-9])|(2[1-9])|(5[0-2]))|(600))|(6469))|(80[1-9][\\d][\\d])|(9(3([0-57-9][\\d][\\d])|(6(0[02-9])|([1-9][\\d])))|(6([0-8][\\d][\\d])|(9([02-79][\\d])|(1[05-9])))|(7[1-9][\\d][\\d])|(9([03-9][\\d][\\d])|(1([0235-9][\\d])|(4[0-24-9]))|(2([0-79][\\d])|(8[0-46-9]))))[\\d]{4})|((22)|(3[2-5])|([47][1-35])|(5[1-3578])|(6[13-57])|(8[1-9])|(9[2458])[\\d]{7}))",
-            "mobile": "((2(1982[0-6])|(3314[05-9])[\\d]{3})|((2(1(160)|(962))|(3(2[\\d][\\d])|(3([034][\\d])|(1[0-35-9])|(2[1-9])|(5[0-2]))|(600))|(6469))|(80[1-9][\\d][\\d])|(9(3([0-57-9][\\d][\\d])|(6(0[02-9])|([1-9][\\d])))|(6([0-8][\\d][\\d])|(9([02-79][\\d])|(1[05-9])))|(7[1-9][\\d][\\d])|(9([03-9][\\d][\\d])|(1([0235-9][\\d])|(4[0-24-9]))|(2([0-79][\\d])|(8[0-46-9]))))[\\d]{4})|((22)|(3[2-5])|([47][1-35])|(5[1-3578])|(6[13-57])|(8[1-9])|(9[2458])[\\d]{7}))",
+            "pattern": "((2(1982[0-6])|(3314[05-9])[\\d]{3})|((2(1(160)|(962))|(3(2[\\d][\\d])|(3([034][\\d])|(1[0-35-9])|(2[1-9])|(5[0-2]))|(600))|(646[59]))|(80[1-9][\\d][\\d])|(9(3([0-57-9][\\d][\\d])|(6(0[02-9])|([1-9][\\d])))|(6([0-8][\\d][\\d])|(9([02-79][\\d])|(1[05-9])))|(7[1-9][\\d][\\d])|(9([03-9][\\d][\\d])|(1([0235-9][\\d])|(4[0-24-9]))|(2([0-79][\\d])|(8[0-46-9]))))[\\d]{4})|((22)|(3[2-5])|([47][1-35])|(5[1-3578])|(6[13-57])|(8[1-9])|(9[2458])[\\d]{7}))",
+            "mobile": "((2(1982[0-6])|(3314[05-9])[\\d]{3})|((2(1(160)|(962))|(3(2[\\d][\\d])|(3([034][\\d])|(1[0-35-9])|(2[1-9])|(5[0-2]))|(600))|(646[59]))|(80[1-9][\\d][\\d])|(9(3([0-57-9][\\d][\\d])|(6(0[02-9])|([1-9][\\d])))|(6([0-8][\\d][\\d])|(9([02-79][\\d])|(1[05-9])))|(7[1-9][\\d][\\d])|(9([03-9][\\d][\\d])|(1([0235-9][\\d])|(4[0-24-9]))|(2([0-79][\\d])|(8[0-46-9]))))[\\d]{4})|((22)|(3[2-5])|([47][1-35])|(5[1-3578])|(6[13-57])|(8[1-9])|(9[2458])[\\d]{7}))",
         },
         "CM": {
             "code": "237",
             "pattern": "((2(22)|(33)[\\d]{6}))",
             "mobile": "(((24[23])|(6[25-9][\\d])[\\d]{6}))",
         },
         "CN": {
@@ -281,15 +281,15 @@
         "CZ": {
             "code": "420",
             "pattern": "(((2[\\d])|(3[1257-9])|(4[16-9])|(5[13-9])[\\d]{7}))",
             "mobile": "(((60[1-8])|(7(0[2-5])|([2379][\\d]))[\\d]{6}))",
         },
         "DE": {
             "code": "49",
-            "pattern": "((32[\\d]{9:11})|(49[2-6][\\d]{10})|(49[0-7][\\d]{3:9})|(([34]0)|([68]9)[\\d]{3:13})|((2(0[1-689])|([1-3569][\\d])|(4[0-8])|(7[1-7])|(8[0-7]))|(3([3569][\\d])|(4[0-79])|(7[1-7])|(8[1-8]))|(4(1[02-9])|([2-48][\\d])|(5[0-6])|(6[0-8])|(7[0-79]))|(5(0[2-8])|([124-6][\\d])|([38][0-8])|([79][0-7]))|(6(0[02-9])|([1-358][\\d])|([47][0-8])|(6[1-9]))|(7(0[2-8])|(1[1-9])|([27][0-7])|(3[\\d])|([4-6][0-8])|(8[0-5])|(9[013-7]))|(8(0[2-9])|(1[0-79])|(2[\\d])|(3[0-46-9])|(4[0-6])|(5[013-9])|(6[1-8])|(7[0-8])|(8[0-24-6]))|(9(0[6-9])|([1-4][\\d])|([589][0-7])|(6[0-8])|(7[0-467]))[\\d]{3:12}))",
+            "pattern": "((32[\\d]{9:11})|(49[2-6][\\d]{10})|(322[\\d]{6})|(49[0-7][\\d]{3:9})|(([34]0)|([68]9)[\\d]{3:13})|((2(0[1-689])|([1-3569][\\d])|(4[0-8])|(7[1-7])|(8[0-7]))|(3([3569][\\d])|(4[0-79])|(7[1-7])|(8[1-8]))|(4(1[02-9])|([2-48][\\d])|(5[0-6])|(6[0-8])|(7[0-79]))|(5(0[2-8])|([124-6][\\d])|([38][0-8])|([79][0-7]))|(6(0[02-9])|([1-358][\\d])|([47][0-8])|(6[1-9]))|(7(0[2-8])|(1[1-9])|([27][0-7])|(3[\\d])|([4-6][0-8])|(8[0-5])|(9[013-7]))|(8(0[2-9])|(1[0-79])|(2[\\d])|(3[0-46-9])|(4[0-6])|(5[013-9])|(6[1-8])|(7[0-8])|(8[0-24-6]))|(9(0[6-9])|([1-4][\\d])|([589][0-7])|(6[0-8])|(7[0-467]))[\\d]{3:12}))",
             "mobile": "((15[0-25-9][\\d]{8})|(1(6[023])|(7[\\d])[\\d]{7:8}))",
         },
         "DJ": {
             "code": "253",
             "pattern": "((2(1[2-5])|(7[45])[\\d]{5}))",
             "mobile": "((77[\\d]{6}))",
         },
@@ -327,15 +327,15 @@
             "code": "20",
             "pattern": "((13[23][\\d]{6})|((15)|(57)[\\d]{6:7})|((2[2-4])|(3)|(4[05-8])|(5[05])|(6[24-689])|(8[2468])|(9[235-7])[\\d]{7}))",
             "mobile": "((1[0-25][\\d]{8}))",
         },
         "EH": {
             "code": "212",
             "pattern": "((528[89][\\d]{5}))",
-            "mobile": "(((6([0-79][\\d])|(8[0-247-9]))|(7([017][\\d])|(6[0-367]))[\\d]{6}))",
+            "mobile": "(((6([0-79][\\d])|(8[0-247-9]))|(7([017][\\d])|(2[0-2])|(6[0-367]))[\\d]{6}))",
         },
         "ER": {
             "code": "291",
             "pattern": "(((1(1[12568])|([24]0)|(55)|(6[146]))|(8[\\d][\\d])[\\d]{4}))",
             "mobile": "(((17[1-3])|(7[\\d][\\d])[\\d]{4}))",
         },
         "ES": {
@@ -381,15 +381,15 @@
         "GA": {
             "code": "241",
             "pattern": "(([01]1[\\d]{6}))",
             "mobile": "((((0[2-7])|(7[467])[\\d])|(6(0[0-4])|(10)|([256][\\d]))[\\d]{5})|([2-7][\\d]{6}))",
         },
         "GB": {
             "code": "44",
-            "pattern": "(((1(1(3([0-58][\\d][\\d])|(73[0235]))|(4([0-5][\\d][\\d])|(69[7-9])|(70[01359]))|((5[0-26-9])|([78][0-49])[\\d][\\d])|(6([0-4][\\d][\\d])|(50[0-79])))|(2((0[024-9])|(2[3-9])|(3[3-79])|(4[1-689])|([58][02-9])|(6[0-47-9])|(7[013-9])|(9[\\d])[\\d][\\d])|(1([0-7][\\d][\\d])|(8([02][\\d])|(1[0-27-9]))))|((3(0[\\d])|(1[0-8])|([25][02-9])|(3[02-579])|([468][0-46-9])|(7[1-35-79])|(9[2-578]))|(4(0[03-9])|([137][\\d])|([28][02-57-9])|(4[02-69])|(5[0-8])|([69][0-79]))|(5(0[1-35-9])|([16][\\d])|(2[024-9])|(3[015689])|(4[02-9])|(5[03-9])|(7[0-35-9])|(8[0-468])|(9[0-57-9]))|(6(0[034689])|(1[\\d])|(2[0-35689])|([38][013-9])|(4[1-467])|(5[0-69])|(6[13-9])|(7[0-8])|(9[0-24578]))|(7(0[0246-9])|(2[\\d])|(3[0236-8])|(4[03-9])|(5[0-46-9])|(6[013-9])|(7[0-35-9])|(8[024-9])|(9[02-9]))|(8(0[35-9])|(2[1-57-9])|(3[02-578])|(4[0-578])|(5[124-9])|(6[2-69])|(7[\\d])|(8[02-9])|(9[02569]))|(9(0[02-589])|([18][\\d])|(2[02-689])|(3[1-57-9])|(4[2-9])|(5[0-579])|(6[2-47-9])|(7[0-24578])|(9[2-57]))[\\d][\\d]))|(2(0[013478])|(3[0189])|(4[017])|(8[0-46-9])|(9[0-2])[\\d]{3})[\\d]{4})|(1(2(0(46[1-4])|(87[2-9]))|(545[1-79])|(76(2[\\d])|(3[1-8])|(6[1-6]))|(9(7(2[0-4])|(3[2-5]))|(8(2[2-8])|(7[0-47-9])|(8[3-5]))))|(3(6(38[2-5])|(47[23]))|(8(47[04-9])|(64[0157-9])))|(4(044[1-7])|(20(2[23])|(8[\\d]))|(6(0(30)|(5[2-57])|(6[1-8])|(7[2-8]))|(140))|(8(052)|(87[1-3])))|(5(2(4(3[2-79])|(6[\\d]))|(76[\\d]))|(6(26[06-9])|(686)))|(6(06(4[\\d])|(7[4-79]))|(295[5-7])|(35[34][\\d])|(47(24)|(61))|(59(5[08])|(6[67])|(74))|(9(55[0-4])|(77[23])))|(7(26(6[13-9])|(7[0-7]))|((442)|(688)[\\d])|(50(2[0-3])|([3-68]2)|(76)))|(8(27[56][\\d])|(37(5[2-5])|(8[239]))|(843[2-58]))|(9(0(0(6[1-8])|(85))|(52[\\d]))|(3583)|(4(66[1-8])|(9(2[01])|(81)))|(63(23)|(3[1-4]))|(9561))[\\d]{3}))",
+            "pattern": "(((1(1(3([0-58][\\d][\\d])|(73[0235]))|(4([0-5][\\d][\\d])|(69[7-9])|(70[01359]))|((5[0-26-9])|([78][0-49])[\\d][\\d])|(6([0-4][\\d][\\d])|(50[0-79])))|(2((0[024-9])|(2[3-9])|(3[3-79])|(4[1-689])|([58][02-9])|(6[0-47-9])|(7[013-9])|(9[\\d])[\\d][\\d])|(1([0-7][\\d][\\d])|(8([02][\\d])|(1[0-26-9]))))|((3(0[\\d])|(1[0-8])|([25][02-9])|(3[02-579])|([468][0-46-9])|(7[1-35-79])|(9[2-578]))|(4(0[03-9])|([137][\\d])|([28][02-57-9])|(4[02-69])|(5[0-8])|([69][0-79]))|(5(0[1-35-9])|([16][\\d])|(2[024-9])|(3[015689])|(4[02-9])|(5[03-9])|(7[0-35-9])|(8[0-468])|(9[0-57-9]))|(6(0[034689])|(1[\\d])|(2[0-35689])|([38][013-9])|(4[1-467])|(5[0-69])|(6[13-9])|(7[0-8])|(9[0-24578]))|(7(0[0246-9])|(2[\\d])|(3[0236-8])|(4[03-9])|(5[0-46-9])|(6[013-9])|(7[0-35-9])|(8[024-9])|(9[02-9]))|(8(0[35-9])|(2[1-57-9])|(3[02-578])|(4[0-578])|(5[124-9])|(6[2-69])|(7[\\d])|(8[02-9])|(9[02569]))|(9(0[02-589])|([18][\\d])|(2[02-689])|(3[1-57-9])|(4[2-9])|(5[0-579])|(6[2-47-9])|(7[0-24578])|(9[2-57]))[\\d][\\d]))|(2(0[013478])|(3[0189])|(4[017])|(8[0-46-9])|(9[0-2])[\\d]{3})[\\d]{4})|(1(2(0(46[1-4])|(87[2-9]))|(545[1-79])|(76(2[\\d])|(3[1-8])|(6[1-6]))|(9(7(2[0-4])|(3[2-5]))|(8(2[2-8])|(7[0-47-9])|(8[3-5]))))|(3(6(38[2-5])|(47[23]))|(8(47[04-9])|(64[0157-9])))|(4(044[1-7])|(20(2[23])|(8[\\d]))|(6(0(30)|(5[2-57])|(6[1-8])|(7[2-8]))|(140))|(8(052)|(87[1-3])))|(5(2(4(3[2-79])|(6[\\d]))|(76[\\d]))|(6(26[06-9])|(686)))|(6(06(4[\\d])|(7[4-79]))|(295[5-7])|(35[34][\\d])|(47(24)|(61))|(59(5[08])|(6[67])|(74))|(9(55[0-4])|(77[23])))|(7(26(6[13-9])|(7[0-7]))|((442)|(688)[\\d])|(50(2[0-3])|([3-68]2)|(76)))|(8(27[56][\\d])|(37(5[2-5])|(8[239]))|(843[2-58]))|(9(0(0(6[1-8])|(85))|(52[\\d]))|(3583)|(4(66[1-8])|(9(2[01])|(81)))|(63(23)|(3[1-4]))|(9561))[\\d]{3}))",
             "mobile": "((7(457[0-57-9])|(700[01])|(911[028])[\\d]{5})|(7([1-3][\\d][\\d])|(4([0-46-9][\\d])|(5[0-689]))|(5(0[0-8])|([13-9][\\d])|(2[0-35-9]))|(7(0[1-9])|([1-7][\\d])|(8[02-9])|(9[0-689]))|(8([014-9][\\d])|([23][0-8]))|(9([024-9][\\d])|(1[02-9])|(3[0-689]))[\\d]{6}))",
         },
         "GD": {
             "code": "1",
             "pattern": "((473(2(3[0-2])|(69))|(3(2[89])|(86))|(4([06]8)|(3[5-9])|(4[0-49])|(5[5-79])|(73)|(90))|(63[68])|(7(58)|(84))|(800)|(938)[\\d]{4}))",
             "mobile": "((473(4(0[2-79])|(1[04-9])|(2[0-5])|(58))|(5(2[01])|(3[3-8]))|(901)[\\d]{4}))",
         },
@@ -467,25 +467,25 @@
             "code": "592",
             "pattern": "(((2(1[6-9])|(2[0-35-9])|(3[1-4])|(5[3-9])|(6[\\d])|(7[0-24-79]))|(3(2[25-9])|(3[\\d]))|(4(4[0-24])|(5[56]))|(77[1-57])[\\d]{4}))",
             "mobile": "(((6[\\d][\\d])|(70[015-7])[\\d]{4}))",
         },
         "HK": {
             "code": "852",
             "pattern": "(((2([13-9][\\d])|(2[013-9])[\\d])|(3(([1569][0-24-9])|(4[0-246-9])|(7[0-24-69])[\\d])|(8(4[0-8])|(5[0-5])|(9[\\d])))|(58(0[1-8])|(1[2-9]))[\\d]{4}))",
-            "mobile": "(((46(0[0-7])|(1[0-6])|(4[0-57-9])|(6[0-4])|(7[0-8]))|(573[0-6])|(6(26[013-8])|(66[0-3]))|(70(7[1-5])|(8[0-4]))|(848[015-9])|(929[013-9])[\\d]{4})|((4(40)|(6[2358]))|(5([1-59][0-46-9])|(6[0-4689])|(7[0-24679]))|(6(0[1-9])|([13-59][\\d])|([268][0-57-9])|(7[0-79]))|(84[09])|(9(0[1-9])|(1[02-9])|([2358][0-8])|([467][\\d]))[\\d]{5}))",
+            "mobile": "(((4(44[5-9])|(6(0[0-7])|(1[0-6])|(4[0-57-9])|(6[0-4])|(7[0-8])))|(573[0-6])|(6(26[013-8])|(66[0-3]))|(70(7[1-5])|(8[0-4]))|(848[015-9])|(9(29[013-9])|(59[0-4]))[\\d]{4})|((4(40)|(6[2358]))|(5([1-59][0-46-9])|(6[0-4689])|(7[0-24679]))|(6(0[1-9])|([13-59][\\d])|([268][0-57-9])|(7[0-79]))|(84[09])|(9(0[1-9])|(1[02-9])|([2358][0-8])|([467][\\d]))[\\d]{5}))",
         },
         "HN": {
             "code": "504",
             "pattern": "((2(2(0[0-39])|(1[1-367])|([23][\\d])|(4[03-6])|(5[57])|(6[245])|(7[0135689])|(8[01346-9])|(9[0-2]))|(4(0[78])|(2[3-59])|(3[13-9])|(4[0-68])|(5[1-35]))|(5(0[7-9])|(16)|(4[03-5])|(5[\\d])|(6[014-6])|(7[04])|(80))|(6([056][\\d])|(17)|(2[067])|(3[04])|(4[0-378])|([78][0-8])|(9[01]))|(7(6[46-9])|(7[02-9])|(8[034])|(91))|(8(79)|(8[0-357-9])|(9[1-57-9]))[\\d]{4}))",
             "mobile": "(([37-9][\\d]{7}))",
         },
         "HR": {
             "code": "385",
             "pattern": "((1[\\d]{7})|((2[0-3])|(3[1-5])|(4[02-47-9])|(5[1-3])[\\d]{6:7}))",
-            "mobile": "((98[\\d]{6:7})|(975(1[\\d])|(96)[\\d]{4})|(9(0[1-9])|([1259][\\d])|(7[0679])[\\d]{6}))",
+            "mobile": "((98[\\d]{6:7})|(975(1[\\d])|(9[67])[\\d]{4})|(9(0[1-9])|([1259][\\d])|(7[0679])[\\d]{6}))",
         },
         "HT": {
             "code": "509",
             "pattern": "((2(2[\\d])|(5[1-5])|(81)|(9[149])[\\d]{5}))",
             "mobile": "(([34][\\d]{7}))",
         },
         "HU": {
@@ -523,15 +523,15 @@
             "code": "964",
             "pattern": "((1[\\d]{7})|((2[13-5])|(3[02367])|(4[023])|(5[03])|(6[026])[\\d]{6:7}))",
             "mobile": "((7[3-9][\\d]{8}))",
         },
         "IR": {
             "code": "98",
             "pattern": "(((1[137])|(2[13-68])|(3[1458])|(4[145])|(5[1468])|(6[16])|(7[1467])|(8[13467])([03-57][\\d]{7})|([16][\\d]{3}([\\d]{4})?)|([289][\\d]{3}([\\d]([\\d]{3})?)?))|(94(000[09])|(2(121)|([2689]0[\\d]))|(30[0-2][\\d])|(4(111)|(40[\\d]))[\\d]{4}))",
-            "mobile": "((9((0([0-35][\\d])|(4[4-6]))|(([13][\\d])|(2[0-3])[\\d])[\\d])|(9([0-46][\\d][\\d])|(5[15]0)|(8(1[\\d])|(88))|(9(0[013])|([19][\\d])|(21)|(77)|(8[7-9])))[\\d]{5}))",
+            "mobile": "((9((0([0-35][\\d])|(4[4-6]))|(([13][\\d])|(2[0-3])[\\d])[\\d])|(9([0-46][\\d][\\d])|(5[15]0)|(8(1[\\d])|(88))|(9(0[0-3])|([19][\\d])|(21)|(77)|(8[7-9])))[\\d]{5}))",
         },
         "IS": {
             "code": "354",
             "pattern": "(((4(1[0-24-69])|(2[0-7])|([37][0-8])|(4[0-24589])|(5[0-68])|(6[\\d])|(8[0-36-8]))|(5(05)|([156][\\d])|(2[02578])|(3[0-579])|(4[03-7])|(7[0-2578])|(8[0-35-9])|(9[013-689]))|(872)[\\d]{4}))",
             "mobile": "(((38[589][\\d][\\d])|(6(1[1-8])|(2[0-6])|(3[026-9])|(4[014679])|(5[0159])|(6[0-69])|(70)|(8[06-8])|(9[\\d]))|(7(5[057])|([6-9][\\d]))|(8(2[0-59])|([3-69][\\d])|(8[238]))[\\d]{4}))",
         },
         "IT": {
@@ -660,15 +660,15 @@
             "code": "218",
             "pattern": "(((2(0[56])|([1-6][\\d])|(7[124579])|(8[124]))|(3(1[\\d])|(2[2356]))|(4([17][\\d])|(2[1-357])|(5[2-4])|(8[124]))|(5([1347][\\d])|(2[1-469])|(5[13-5])|(8[1-4]))|(6([1-479][\\d])|(5[2-57])|(8[1-5]))|(7([13][\\d])|(2[13-79]))|(8([124][\\d])|(5[124])|(84))[\\d]{6}))",
             "mobile": "((9[1-6][\\d]{7}))",
         },
         "MA": {
             "code": "212",
             "pattern": "((5(29([189][05])|(2[29])|(3[01]))|(389[05])[\\d]{4})|(5(2([0-25-7][\\d])|(3[1-578])|(4[02-46-8])|(8[0235-7])|(90))|(3([0-47][\\d])|(5[02-9])|(6[02-8])|(8[08])|(9[3-9]))|((4[067])|(5[03])[\\d])[\\d]{5}))",
-            "mobile": "(((6([0-79][\\d])|(8[0-247-9]))|(7([017][\\d])|(6[0-367]))[\\d]{6}))",
+            "mobile": "(((6([0-79][\\d])|(8[0-247-9]))|(7([017][\\d])|(2[0-2])|(6[0-367]))[\\d]{6}))",
         },
         "MC": {
             "code": "377",
             "pattern": "(((870)|(9[2-47-9][\\d])[\\d]{5}))",
             "mobile": "((4([46][\\d])|(5[1-9])[\\d]{5})|((3)|(6[\\d])[\\d]{7}))",
         },
         "MD": {
@@ -690,15 +690,15 @@
             "code": "261",
             "pattern": "((2072[29][\\d]{4})|(20(2[\\d])|(4[47])|(5[3467])|(6[279])|(7[35])|(8[268])|(9[245])[\\d]{5}))",
             "mobile": "((3[2-489][\\d]{7}))",
         },
         "MH": {
             "code": "692",
             "pattern": "(((247)|(528)|(625)[\\d]{4}))",
-            "mobile": "((((23)|(54)5)|(329)|(45[56])[\\d]{4}))",
+            "mobile": "((((23)|(54)5)|(329)|(45[356])[\\d]{4}))",
         },
         "MK": {
             "code": "389",
             "pattern": "((((2(62)|(77)0)|(3444)[\\d])|(4[56]440)[\\d]{3})|((34)|(4[357])700[\\d]{3})|((2([23][\\d])|(5[0-578])|(6[01])|(82))|(3(1[3-68])|([23][2-68])|(4[23568]))|(4([23][2-68])|(4[3-68])|(5[2568])|(6[25-8])|(7[24-68])|(8[4-68]))[\\d]{5}))",
             "mobile": "((7(3555)|(4(60[\\d])|(747))|(94([01][\\d])|(2[0-4]))[\\d]{3})|(7([0-25-8][\\d])|(3[1-4])|(42)|(9[23])[\\d]{5}))",
         },
         "ML": {
@@ -1095,15 +1095,15 @@
         "TR": {
             "code": "90",
             "pattern": "(((2([13][26])|([28][2468])|([45][268])|([67][246]))|(3([13][28])|([24-6][2468])|([78][02468])|(92))|(4([16][246])|([23578][2468])|(4[26]))[\\d]{7}))",
             "mobile": "((56161[\\d]{5})|(5(0[15-7])|(1[06])|(24)|([34][\\d])|(5[1-59])|(9[46])[\\d]{7}))",
         },
         "TT": {
             "code": "1",
-            "pattern": "((868(2(0[13])|(1[89])|([23][\\d])|(4[0-2]))|(6(0[7-9])|(1[02-8])|(2[1-9])|([3-69][\\d])|(7[0-79]))|(82[124])[\\d]{4}))",
+            "pattern": "((868(2(0[13])|(1[5-9])|([23][\\d])|(4[0-2]))|(6(0[7-9])|(1[02-8])|(2[1-9])|([3-69][\\d])|(7[0-79]))|(82[124])[\\d]{4}))",
             "mobile": "((868((2[5-9])|(3[\\d])[\\d])|(4(3[0-6])|([6-9][\\d]))|(6(20)|(78)|(8[\\d]))|(7(0[1-9])|(1[02-9])|([2-9][\\d]))[\\d]{4}))",
         },
         "TV": {
             "code": "688",
             "pattern": "((2[02-9][\\d]{3}))",
             "mobile": "(((7[01][\\d])|(90)[\\d]{4}))",
         },
@@ -1116,25 +1116,25 @@
             "code": "255",
             "pattern": "((2[2-8][\\d]{7}))",
             "mobile": "((77[2-9][\\d]{6})|((6[1-9])|(7[1-689])[\\d]{7}))",
         },
         "UA": {
             "code": "380",
             "pattern": "(((3[1-8])|(4[13-8])|(5[1-7])|(6[12459])[\\d]{7}))",
-            "mobile": "(((50)|(6[36-8])|(7[1-3])|(9[1-9])[\\d]{7}))",
+            "mobile": "(((39)|(50)|(6[36-8])|(7[1-3])|(9[1-9])[\\d]{7}))",
         },
         "UG": {
             "code": "256",
             "pattern": "((20(((24)|(81)0)|(30[67])[\\d])|(6(00[0-2])|(30[0-4]))[\\d]{3})|((20([017][\\d])|(2[5-9])|(32)|(5[0-4])|(6[15-9]))|([34][\\d]{3})[\\d]{5}))",
             "mobile": "((726[01][\\d]{5})|(7([01578][\\d])|(20)|(36)|([46][0-4])|(9[89])[\\d]{6}))",
         },
         "US": {
             "code": "1",
-            "pattern": "((5(05([2-57-9][\\d][\\d])|(6([0-35-9][\\d])|(44)))|(82(2(0[0-3])|([268]2))|(3(0[02])|(22)|(33))|(4(00)|(4[24])|(65)|(82))|(5(00)|(29)|(58)|(83))|(6(00)|(66)|(82))|(7(58)|(77))|(8(00)|(42)|(88))|(9(00)|(9[89])))[\\d]{4})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[12])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[19])|(6[1-47])|(7[0-5])|(8[056]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[08])|(3[0-289])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[0157-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
-            "mobile": "((5(05([2-57-9][\\d][\\d])|(6([0-35-9][\\d])|(44)))|(82(2(0[0-3])|([268]2))|(3(0[02])|(22)|(33))|(4(00)|(4[24])|(65)|(82))|(5(00)|(29)|(58)|(83))|(6(00)|(66)|(82))|(7(58)|(77))|(8(00)|(42)|(88))|(9(00)|(9[89])))[\\d]{4})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[12])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[19])|(6[1-47])|(7[0-5])|(8[056]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[08])|(3[0-289])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[0157-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
+            "pattern": "((5(05([2-57-9][\\d][\\d])|(6([0-35-9][\\d])|(44)))|(82(2(0[0-3])|([268]2))|(3(0[02])|(22)|(33))|(4(00)|(4[24])|(65)|(82))|(5(00)|(29)|(58)|(83))|(6(00)|(66)|(82))|(7(58)|(77))|(8(00)|(42)|(88))|(9(00)|(9[89])))[\\d]{4})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[12])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[19])|(6[1-47])|(7[0-5])|(8[056]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[068])|(3[0-289])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[0157-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
+            "mobile": "((5(05([2-57-9][\\d][\\d])|(6([0-35-9][\\d])|(44)))|(82(2(0[0-3])|([268]2))|(3(0[02])|(22)|(33))|(4(00)|(4[24])|(65)|(82))|(5(00)|(29)|(58)|(83))|(6(00)|(66)|(82))|(7(58)|(77))|(8(00)|(42)|(88))|(9(00)|(9[89])))[\\d]{4})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[12])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[19])|(6[1-47])|(7[0-5])|(8[056]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[068])|(3[0-289])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[0157-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
         },
         "UY": {
             "code": "598",
             "pattern": "(((1(770)|(987))|((2[\\d])|(4[2-7])[\\d][\\d])[\\d]{4}))",
             "mobile": "((9[1-9][\\d]{6}))",
         },
         "UZ": {
```

## Comparing `phone_gen-2.2.8.dist-info/LICENSE` & `phone_gen-2.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phone_gen-2.2.8.dist-info/METADATA` & `phone_gen-2.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.2.8
+Version: 2.2.9
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Platform: UNKNOWN
```

## Comparing `phone_gen-2.2.8.dist-info/RECORD` & `phone_gen-2.2.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 phone_gen/__init__.py,sha256=Wy9sBhYYGJP-cbm6OOFDMB8pVLSe4dykwNJwmjsP6O8,1030
-phone_gen/__version__.py,sha256=0UaZPYyQpOweR3m8VBEg2-sRpVNXWT33mZ-4AxzDQrU,34
+phone_gen/__version__.py,sha256=TPPGsmYP-hNc1YtqRV6qFI8G7GmWhZMF2F1ADX3TrcA,34
 phone_gen/_generator.py,sha256=5n3xAwSVf1GpYxbC47vQjTowxqhrh2bwL38RF_OgbRI,10602
 phone_gen/alt_patterns.py,sha256=gE9k33zvsMv3T8mYGAvf3NTYufpwE1mFSVHck1GHzKU,562
 phone_gen/cli.py,sha256=brzMtp-t239RILDyHncnrjPzSW1AbC63-EOBFOaloxU,1478
 phone_gen/country_name.py,sha256=GOyQSjxM5G28D83tJn5uGQnK-7Pn1HJnjBU3V6X1DGM,16602
 phone_gen/iso3.py,sha256=cVwoh2nbY2wGzcTAkrV2P5ISpGgtRHCExrWsq9Gl1vY,6932
-phone_gen/patterns.py,sha256=d0buWIFaATejxc7RGqRLTyuHJPre7evmhyziBxUTSrQ,87120
-phone_gen-2.2.8.dist-info/LICENSE,sha256=rIUWZBoK2vPxnSn6Gm25N4HK7E9aKf97fMlmimBBioM,1067
-phone_gen-2.2.8.dist-info/METADATA,sha256=DgLiBdEXTWWgh4jFeVIyPIWAkxI9zpg2uBqxUKwN-VQ,4223
-phone_gen-2.2.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-phone_gen-2.2.8.dist-info/entry_points.txt,sha256=ZuUmmqkOGL9fX9p0CYL4NB7WhC0Bedx85V1kJchO6tw,50
-phone_gen-2.2.8.dist-info/top_level.txt,sha256=cX_kXxByWyh_ur7NKWya4UviV7vSqkVhZrJrFi4637s,10
-phone_gen-2.2.8.dist-info/RECORD,,
+phone_gen/patterns.py,sha256=WmCuCSJZ1Wv8Fxx-Q3po58RQDW6Izw5voGtY6ewhntI,87211
+phone_gen-2.2.9.dist-info/LICENSE,sha256=rIUWZBoK2vPxnSn6Gm25N4HK7E9aKf97fMlmimBBioM,1067
+phone_gen-2.2.9.dist-info/METADATA,sha256=15p7-OvFVMMwylyI9xGX5hAmPPdRxj66jsi-SfKAXME,4223
+phone_gen-2.2.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+phone_gen-2.2.9.dist-info/entry_points.txt,sha256=ZuUmmqkOGL9fX9p0CYL4NB7WhC0Bedx85V1kJchO6tw,50
+phone_gen-2.2.9.dist-info/top_level.txt,sha256=cX_kXxByWyh_ur7NKWya4UviV7vSqkVhZrJrFi4637s,10
+phone_gen-2.2.9.dist-info/RECORD,,
```

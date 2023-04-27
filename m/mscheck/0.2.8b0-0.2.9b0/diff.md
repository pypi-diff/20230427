# Comparing `tmp/mscheck-0.2.8b0.tar.gz` & `tmp/mscheck-0.2.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscheck-0.2.8b0.tar", last modified: Thu Apr 27 20:57:39 2023, max compression
+gzip compressed data, was "mscheck-0.2.9b0.tar", last modified: Thu Apr 27 21:14:52 2023, max compression
```

## Comparing `mscheck-0.2.8b0.tar` & `mscheck-0.2.9b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:39.561399 mscheck-0.2.8b0/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:57:39.561399 mscheck-0.2.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:39.557399 mscheck-0.2.8b0/mscheck/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/mscheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/mscheck/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/mscheck/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/mscheck/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/mscheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:39.557399 mscheck-0.2.8b0/mscheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:57:39.000000 mscheck-0.2.8b0/mscheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 20:57:39.000000 mscheck-0.2.8b0/mscheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:57:39.000000 mscheck-0.2.8b0/mscheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 20:57:39.000000 mscheck-0.2.8b0/mscheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 20:57:39.000000 mscheck-0.2.8b0/mscheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 20:57:39.561399 mscheck-0.2.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:39.561399 mscheck-0.2.8b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 20:57:36.000000 mscheck-0.2.8b0/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/mscheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/mscheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/mscheck/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/mscheck/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/mscheck/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/mscheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/mscheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-27 21:14:52.000000 mscheck-0.2.9b0/mscheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 21:14:52.000000 mscheck-0.2.9b0/mscheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:14:52.000000 mscheck-0.2.9b0/mscheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 21:14:52.000000 mscheck-0.2.9b0/mscheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 21:14:52.000000 mscheck-0.2.9b0/mscheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:14:52.311721 mscheck-0.2.9b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 21:14:50.000000 mscheck-0.2.9b0/tests/test_spectrum.py
```

### Comparing `mscheck-0.2.8b0/PKG-INFO` & `mscheck-0.2.9b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d73 6368  : 2.1.Name: msch
 00000020: 6563 6b0a 5665 7273 696f 6e3a 2030 2e32  eck.Version: 0.2
-00000030: 2e38 6230 0a53 756d 6d61 7279 3a20 4175  .8b0.Summary: Au
+00000030: 2e39 6230 0a53 756d 6d61 7279 3a20 4175  .9b0.Summary: Au
 00000040: 746f 204d 5320 6d61 7373 2063 6865 636b  to MS mass check
 00000050: 6572 0a48 6f6d 652d 7061 6765 3a20 6874  er.Home-page: ht
 00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000070: 2f57 617a 746f 6d2f 6d73 6368 6563 6b0a  /Waztom/mscheck.
 00000080: 4175 7468 6f72 3a20 5761 7272 656e 2054  Author: Warren T
 00000090: 686f 6d70 736f 6e0a 4175 7468 6f72 2d65  hompson.Author-e
 000000a0: 6d61 696c 3a20 7761 7a74 6f6d 4067 6d61  mail: waztom@gma
@@ -145,97 +145,104 @@
 00000900: 6520 2d6e 204d 5363 6865 636b 2070 7974  e -n MScheck pyt
 00000910: 686f 6e3d 332e 3131 600a 0a32 2e20 4163  hon=3.11`..2. Ac
 00000920: 7469 7661 7465 2074 6865 204d 5363 6865  tivate the MSche
 00000930: 636b 2063 6f6e 6461 2065 6e76 6972 6f6e  ck conda environ
 00000940: 6d65 6e74 2063 7265 6174 6564 0a0a 2020  ment created..  
 00000950: 203e 2060 636f 6e64 6120 6163 7469 7661   > `conda activa
 00000960: 7465 204d 5363 6865 636b 600a 0a33 2e20  te MScheck`..3. 
-00000970: 5069 7020 696e 7374 616c 6c20 4d53 6368  Pip install MSch
-00000980: 6563 6b0a 2020 203e 2060 7069 7020 696e  eck.   > `pip in
-00000990: 7374 616c 6c20 6d73 6368 6563 6b60 0a0a  stall mscheck`..
-000009a0: 2320 3c61 206e 616d 653d 2250 7265 7061  # <a name="Prepa
-000009b0: 7269 6e67 2076 656e 646f 7220 6669 6c65  ring vendor file
-000009c0: 7322 3e3c 2f61 3e2a 2a50 7265 7061 7269  s"></a>**Prepari
-000009d0: 6e67 2076 656e 646f 7220 6669 6c65 732a  ng vendor files*
-000009e0: 2a0a 0a4d 5363 6865 636b 2068 6173 2062  *..MScheck has b
-000009f0: 6565 6e20 7465 7374 6564 206f 6e20 7573  een tested on us
-00000a00: 696e 6720 4167 696c 656e 7420 4c43 4d53  ing Agilent LCMS
-00000a10: 2066 696c 6573 2028 2e44 2920 6173 2074   files (.D) as t
-00000a20: 6865 2073 7461 7274 696e 6720 6669 6c65  he starting file
-00000a30: 2066 6f72 6d61 742e 204f 6e65 2063 6861   format. One cha
-00000a40: 6c6c 656e 6765 2069 7320 746f 2063 6f6e  llenge is to con
-00000a50: 7665 7274 2076 656e 646f 7220 6669 6c65  vert vendor file
-00000a60: 2066 6f72 6d61 7473 2069 6e74 6f0a 6120   formats into.a 
-00000a70: 666f 726d 6174 2077 6974 6820 7468 6520  format with the 
-00000a80: 6269 6e61 7279 2064 6563 6f64 6564 2e0a  binary decoded..
-00000a90: 0a31 2e20 436f 6e76 6572 7420 2e44 2041  .1. Convert .D A
-00000aa0: 6769 6c65 6e74 2066 6f6c 6465 7220 746f  gilent folder to
-00000ab0: 2061 202e 6420 4d61 7373 4875 6e74 6572   a .d MassHunter
-00000ac0: 2066 6f72 6d61 7420 7573 696e 6720 4167   format using Ag
-00000ad0: 696c 656e 7427 7320 4368 656d 5374 6174  ilent's ChemStat
-00000ae0: 696f 6e20 746f 204d 6173 7348 756e 7465  ion to MassHunte
-00000af0: 7220 5472 616e 736c 6174 6f72 2028 422e  r Translator (B.
-00000b00: 3034 2e30 3029 0a32 2e20 436f 6e76 6572  04.00).2. Conver
-00000b10: 7420 2e64 2066 6f72 6d61 7420 696e 746f  t .d format into
-00000b20: 202e 6d7a 4d4c 2066 6f72 6d61 7420 7573   .mzML format us
-00000b30: 696e 6720 5b50 726f 7465 6f57 697a 6172  ing [ProteoWizar
-00000b40: 6427 735d 2868 7474 703a 2f2f 7072 6f74  d's](http://prot
-00000b50: 656f 7769 7a61 7264 2e73 6f75 7263 6566  eowizard.sourcef
-00000b60: 6f72 6765 2e6e 6574 2f29 204d 5343 6f6e  orge.net/) MSCon
-00000b70: 7665 7274 2074 6f6f 6c0a 332e 2046 696e  vert tool.3. Fin
-00000b80: 616c 6c79 202d 2077 6520 6861 7665 2061  ally - we have a
-00000b90: 6e20 6669 6c65 2066 6f72 6d61 7420 7468  n file format th
-00000ba0: 6174 2077 6520 6361 6e20 7573 6521 0a34  at we can use!.4
-00000bb0: 2e20 496e 2079 6f75 7220 6661 766f 7572  . In your favour
-00000bc0: 6974 6520 4944 4520 6f72 204a 7570 7974  ite IDE or Jupyt
-00000bd0: 6572 206e 6f74 6562 6f6f 6b20 2d20 6120  er notebook - a 
-00000be0: 6261 7369 6320 6578 616d 706c 6520 6f66  basic example of
-00000bf0: 2075 7369 6e67 204d 5343 6865 636b 2069   using MSCheck i
-00000c00: 7320 7072 6f76 6964 6564 2062 656c 6f77  s provided below
-00000c10: 3a3c 6272 3e0a 0a60 6060 0a66 726f 6d20  :<br>..```.from 
-00000c20: 6d73 6368 6563 6b2e 616e 616c 7973 6520  mscheck.analyse 
-00000c30: 696d 706f 7274 2041 6e61 6c79 7365 5370  import AnalyseSp
-00000c40: 6563 7472 756d 0a0a 2320 4372 6561 7465  ectrum..# Create
-00000c50: 204d 5320 7363 7074 7275 6d20 6f62 6a65   MS scptrum obje
-00000c60: 6374 2061 6e64 2066 696e 6420 7065 616b  ct and find peak
-00000c70: 730a 7465 7374 203d 2041 6e61 6c79 7365  s.test = Analyse
-00000c80: 5370 6563 7472 756d 2822 3c70 6174 6820  Spectrum("<path 
-00000c90: 746f 202e 6d7a 4d4c 2066 696c 653e 222c  to .mzML file>",
-00000ca0: 206d 6f64 653d 2250 6f73 6974 6976 6522   mode="Positive"
-00000cb0: 290a 0a23 2053 6574 2053 4d49 4c45 5320  )..# Set SMILES 
-00000cc0: 6f66 2074 6172 6765 7420 746f 2073 6561  of target to sea
-00000cd0: 7263 6820 666f 720a 7461 7267 6574 5f53  rch for.target_S
-00000ce0: 4d49 4c45 5320 3d20 2243 434f 4328 3d4f  MILES = "CCOC(=O
-00000cf0: 294e 3143 434e 2843 283d 4f29 4e32 4343  )N1CCN(C(=O)N2CC
-00000d00: 4e28 4328 3d4f 2963 3363 6363 6f33 2943  N(C(=O)c3ccco3)C
-00000d10: 4332 2943 4331 220a 0a23 2041 6e61 6c79  C2)CC1"..# Analy
-00000d20: 7365 2074 6573 7420 7370 6563 7472 756d  se test spectrum
-00000d30: 2073 6561 7263 6869 6e67 2066 6f72 2074   searching for t
-00000d40: 6172 6765 7420 534d 494c 4553 0a74 6573  arget SMILES.tes
-00000d50: 742e 616e 616c 7973 6528 636f 6d70 6f75  t.analyse(compou
-00000d60: 6e64 736d 696c 6573 3d74 6172 6765 745f  ndsmiles=target_
-00000d70: 534d 494c 4553 2c0a 2020 2020 2020 2020  SMILES,.        
-00000d80: 2020 2020 2069 6f6e 7374 6f61 6464 3d5b       ionstoadd=[
-00000d90: 225b 485d 222c 2022 5b4e 615d 222c 2022  "[H]", "[Na]", "
-00000da0: 5b4b 5d22 2c20 225b 4e48 342b 5d22 5d2c  [K]", "[NH4+]"],
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 746f  .             to
-00000dc0: 6c65 7261 6e63 653d 3129 0a0a 2320 4372  lerance=1)..# Cr
-00000dd0: 6561 7465 2061 202e 7376 6720 7265 706f  eate a .svg repo
-00000de0: 7274 202d 2069 6620 796f 7520 646f 206e  rt - if you do n
-00000df0: 6f74 2067 6976 6520 6120 636f 6d70 6f75  ot give a compou
-00000e00: 6e64 5f6e 616d 650a 2320 7468 6520 656e  nd_name.# the en
-00000e10: 6469 6e67 206c 6561 6620 6f66 2074 6865  ding leaf of the
-00000e20: 2066 696c 6520 6e61 6d65 2077 696c 6c20   file name will 
-00000e30: 6265 2075 7365 640a 7465 7374 2e63 7265  be used.test.cre
-00000e40: 6174 655f 7265 706f 7274 2863 6f6d 706f  ate_report(compo
-00000e50: 756e 645f 6e61 6d65 3d22 5465 7374 2229  und_name="Test")
-00000e60: 0a60 6060 0a0a 203c 6272 3e0a 0a54 6865  .```.. <br>..The
-00000e70: 202e 7376 6720 7265 706f 7274 2077 696c   .svg report wil
-00000e80: 6c20 6265 2069 6e20 6120 666f 6c64 6572  l be in a folder
-00000e90: 2063 616c 6c65 6420 5265 706f 7274 730a   called Reports.
-00000ea0: 0a45 7861 6d70 6c65 206f 6620 7265 706f  .Example of repo
-00000eb0: 7274 206f 7574 7075 743a 3c62 723e 0a0a  rt output:<br>..
-00000ec0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000ed0: 223e 0a3c 696d 6720 7372 633d 2269 6d61  ">.<img src="ima
-00000ee0: 6765 732f 7265 706f 7274 2e73 7667 2220  ges/report.svg" 
-00000ef0: 7769 6474 683d 2236 3030 7078 223e 0a3c  width="600px">.<
-00000f00: 2f70 3e0a 0a0a                           /p>...
+00000970: 5069 7020 696e 7374 616c 6c20 7079 4f70  Pip install pyOp
+00000980: 656e 4d53 0a0a 2020 203e 2060 7069 7020  enMS..   > `pip 
+00000990: 696e 7374 616c 6c20 2d2d 696e 6465 782d  install --index-
+000009a0: 7572 6c20 6874 7470 733a 2f2f 7079 7069  url https://pypi
+000009b0: 2e63 732e 756e 692d 7475 6562 696e 6765  .cs.uni-tuebinge
+000009c0: 6e2e 6465 2f73 696d 706c 652f 2070 796f  n.de/simple/ pyo
+000009d0: 7065 6e6d 7360 0a0a 342e 2050 6970 2069  penms`..4. Pip i
+000009e0: 6e73 7461 6c6c 204d 5363 6865 636b 0a0a  nstall MScheck..
+000009f0: 2020 203e 2060 7069 7020 696e 7374 616c     > `pip instal
+00000a00: 6c20 6d73 6368 6563 6b60 0a0a 2320 3c61  l mscheck`..# <a
+00000a10: 206e 616d 653d 2250 7265 7061 7269 6e67   name="Preparing
+00000a20: 2076 656e 646f 7220 6669 6c65 7322 3e3c   vendor files"><
+00000a30: 2f61 3e2a 2a50 7265 7061 7269 6e67 2076  /a>**Preparing v
+00000a40: 656e 646f 7220 6669 6c65 732a 2a0a 0a4d  endor files**..M
+00000a50: 5363 6865 636b 2068 6173 2062 6565 6e20  Scheck has been 
+00000a60: 7465 7374 6564 206f 6e20 7573 696e 6720  tested on using 
+00000a70: 4167 696c 656e 7420 4c43 4d53 2066 696c  Agilent LCMS fil
+00000a80: 6573 2028 2e44 2920 6173 2074 6865 2073  es (.D) as the s
+00000a90: 7461 7274 696e 6720 6669 6c65 2066 6f72  tarting file for
+00000aa0: 6d61 742e 204f 6e65 2063 6861 6c6c 656e  mat. One challen
+00000ab0: 6765 2069 7320 746f 2063 6f6e 7665 7274  ge is to convert
+00000ac0: 2076 656e 646f 7220 6669 6c65 2066 6f72   vendor file for
+00000ad0: 6d61 7473 2069 6e74 6f0a 6120 666f 726d  mats into.a form
+00000ae0: 6174 2077 6974 6820 7468 6520 6269 6e61  at with the bina
+00000af0: 7279 2064 6563 6f64 6564 2e0a 0a31 2e20  ry decoded...1. 
+00000b00: 436f 6e76 6572 7420 2e44 2041 6769 6c65  Convert .D Agile
+00000b10: 6e74 2066 6f6c 6465 7220 746f 2061 202e  nt folder to a .
+00000b20: 6420 4d61 7373 4875 6e74 6572 2066 6f72  d MassHunter for
+00000b30: 6d61 7420 7573 696e 6720 4167 696c 656e  mat using Agilen
+00000b40: 7427 7320 4368 656d 5374 6174 696f 6e20  t's ChemStation 
+00000b50: 746f 204d 6173 7348 756e 7465 7220 5472  to MassHunter Tr
+00000b60: 616e 736c 6174 6f72 2028 422e 3034 2e30  anslator (B.04.0
+00000b70: 3029 0a32 2e20 436f 6e76 6572 7420 2e64  0).2. Convert .d
+00000b80: 2066 6f72 6d61 7420 696e 746f 202e 6d7a   format into .mz
+00000b90: 4d4c 2066 6f72 6d61 7420 7573 696e 6720  ML format using 
+00000ba0: 5b50 726f 7465 6f57 697a 6172 6427 735d  [ProteoWizard's]
+00000bb0: 2868 7474 703a 2f2f 7072 6f74 656f 7769  (http://proteowi
+00000bc0: 7a61 7264 2e73 6f75 7263 6566 6f72 6765  zard.sourceforge
+00000bd0: 2e6e 6574 2f29 204d 5343 6f6e 7665 7274  .net/) MSConvert
+00000be0: 2074 6f6f 6c0a 332e 2046 696e 616c 6c79   tool.3. Finally
+00000bf0: 202d 2077 6520 6861 7665 2061 6e20 6669   - we have an fi
+00000c00: 6c65 2066 6f72 6d61 7420 7468 6174 2077  le format that w
+00000c10: 6520 6361 6e20 7573 6521 0a34 2e20 496e  e can use!.4. In
+00000c20: 2079 6f75 7220 6661 766f 7572 6974 6520   your favourite 
+00000c30: 4944 4520 6f72 204a 7570 7974 6572 206e  IDE or Jupyter n
+00000c40: 6f74 6562 6f6f 6b20 2d20 6120 6261 7369  otebook - a basi
+00000c50: 6320 6578 616d 706c 6520 6f66 2075 7369  c example of usi
+00000c60: 6e67 204d 5343 6865 636b 2069 7320 7072  ng MSCheck is pr
+00000c70: 6f76 6964 6564 2062 656c 6f77 3a3c 6272  ovided below:<br
+00000c80: 3e0a 0a60 6060 0a66 726f 6d20 6d73 6368  >..```.from msch
+00000c90: 6563 6b2e 616e 616c 7973 6520 696d 706f  eck.analyse impo
+00000ca0: 7274 2041 6e61 6c79 7365 5370 6563 7472  rt AnalyseSpectr
+00000cb0: 756d 0a0a 2320 4372 6561 7465 204d 5320  um..# Create MS 
+00000cc0: 7363 7074 7275 6d20 6f62 6a65 6374 2061  scptrum object a
+00000cd0: 6e64 2066 696e 6420 7065 616b 730a 7465  nd find peaks.te
+00000ce0: 7374 203d 2041 6e61 6c79 7365 5370 6563  st = AnalyseSpec
+00000cf0: 7472 756d 2822 3c70 6174 6820 746f 202e  trum("<path to .
+00000d00: 6d7a 4d4c 2066 696c 653e 222c 206d 6f64  mzML file>", mod
+00000d10: 653d 2250 6f73 6974 6976 6522 290a 0a23  e="Positive")..#
+00000d20: 2053 6574 2053 4d49 4c45 5320 6f66 2074   Set SMILES of t
+00000d30: 6172 6765 7420 746f 2073 6561 7263 6820  arget to search 
+00000d40: 666f 720a 7461 7267 6574 5f53 4d49 4c45  for.target_SMILE
+00000d50: 5320 3d20 2243 434f 4328 3d4f 294e 3143  S = "CCOC(=O)N1C
+00000d60: 434e 2843 283d 4f29 4e32 4343 4e28 4328  CN(C(=O)N2CCN(C(
+00000d70: 3d4f 2963 3363 6363 6f33 2943 4332 2943  =O)c3ccco3)CC2)C
+00000d80: 4331 220a 0a23 2041 6e61 6c79 7365 2074  C1"..# Analyse t
+00000d90: 6573 7420 7370 6563 7472 756d 2073 6561  est spectrum sea
+00000da0: 7263 6869 6e67 2066 6f72 2074 6172 6765  rching for targe
+00000db0: 7420 534d 494c 4553 0a74 6573 742e 616e  t SMILES.test.an
+00000dc0: 616c 7973 6528 636f 6d70 6f75 6e64 736d  alyse(compoundsm
+00000dd0: 696c 6573 3d74 6172 6765 745f 534d 494c  iles=target_SMIL
+00000de0: 4553 2c0a 2020 2020 2020 2020 2020 2020  ES,.            
+00000df0: 2069 6f6e 7374 6f61 6464 3d5b 225b 485d   ionstoadd=["[H]
+00000e00: 222c 2022 5b4e 615d 222c 2022 5b4b 5d22  ", "[Na]", "[K]"
+00000e10: 2c20 225b 4e48 342b 5d22 5d2c 0a20 2020  , "[NH4+]"],.   
+00000e20: 2020 2020 2020 2020 2020 746f 6c65 7261            tolera
+00000e30: 6e63 653d 3129 0a0a 2320 4372 6561 7465  nce=1)..# Create
+00000e40: 2061 202e 7376 6720 7265 706f 7274 202d   a .svg report -
+00000e50: 2069 6620 796f 7520 646f 206e 6f74 2067   if you do not g
+00000e60: 6976 6520 6120 636f 6d70 6f75 6e64 5f6e  ive a compound_n
+00000e70: 616d 650a 2320 7468 6520 656e 6469 6e67  ame.# the ending
+00000e80: 206c 6561 6620 6f66 2074 6865 2066 696c   leaf of the fil
+00000e90: 6520 6e61 6d65 2077 696c 6c20 6265 2075  e name will be u
+00000ea0: 7365 640a 7465 7374 2e63 7265 6174 655f  sed.test.create_
+00000eb0: 7265 706f 7274 2863 6f6d 706f 756e 645f  report(compound_
+00000ec0: 6e61 6d65 3d22 5465 7374 2229 0a60 6060  name="Test").```
+00000ed0: 0a0a 203c 6272 3e0a 0a54 6865 202e 7376  .. <br>..The .sv
+00000ee0: 6720 7265 706f 7274 2077 696c 6c20 6265  g report will be
+00000ef0: 2069 6e20 6120 666f 6c64 6572 2063 616c   in a folder cal
+00000f00: 6c65 6420 5265 706f 7274 730a 0a45 7861  led Reports..Exa
+00000f10: 6d70 6c65 206f 6620 7265 706f 7274 206f  mple of report o
+00000f20: 7574 7075 743a 3c62 723e 0a0a 3c70 2061  utput:<br>..<p a
+00000f30: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+00000f40: 696d 6720 7372 633d 2269 6d61 6765 732f  img src="images/
+00000f50: 7265 706f 7274 2e73 7667 2220 7769 6474  report.svg" widt
+00000f60: 683d 2236 3030 7078 223e 0a3c 2f70 3e0a  h="600px">.</p>.
+00000f70: 0a0a                                     ..
```

### Comparing `mscheck-0.2.8b0/README.md` & `mscheck-0.2.9b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,20 @@
 
    > `conda create -c conda-forge -n MScheck python=3.11`
 
 2. Activate the MScheck conda environment created
 
    > `conda activate MScheck`
 
-3. Pip install MScheck
+3. Pip install pyOpenMS
+
+   > `pip install --index-url https://pypi.cs.uni-tuebingen.de/simple/ pyopenms`
+
+4. Pip install MScheck
+
    > `pip install mscheck`
 
 # <a name="Preparing vendor files"></a>**Preparing vendor files**
 
 MScheck has been tested on using Agilent LCMS files (.D) as the starting file format. One challenge is to convert vendor file formats into
 a format with the binary decoded.
```

### Comparing `mscheck-0.2.8b0/mscheck/analyse.py` & `mscheck-0.2.9b0/mscheck/analyse.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.8b0/mscheck/report.py` & `mscheck-0.2.9b0/mscheck/report.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.8b0/mscheck/spectrum.py` & `mscheck-0.2.9b0/mscheck/spectrum.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.8b0/mscheck/utils.py` & `mscheck-0.2.9b0/mscheck/utils.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.8b0/mscheck.egg-info/PKG-INFO` & `mscheck-0.2.9b0/mscheck.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d73 6368  : 2.1.Name: msch
 00000020: 6563 6b0a 5665 7273 696f 6e3a 2030 2e32  eck.Version: 0.2
-00000030: 2e38 6230 0a53 756d 6d61 7279 3a20 4175  .8b0.Summary: Au
+00000030: 2e39 6230 0a53 756d 6d61 7279 3a20 4175  .9b0.Summary: Au
 00000040: 746f 204d 5320 6d61 7373 2063 6865 636b  to MS mass check
 00000050: 6572 0a48 6f6d 652d 7061 6765 3a20 6874  er.Home-page: ht
 00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000070: 2f57 617a 746f 6d2f 6d73 6368 6563 6b0a  /Waztom/mscheck.
 00000080: 4175 7468 6f72 3a20 5761 7272 656e 2054  Author: Warren T
 00000090: 686f 6d70 736f 6e0a 4175 7468 6f72 2d65  hompson.Author-e
 000000a0: 6d61 696c 3a20 7761 7a74 6f6d 4067 6d61  mail: waztom@gma
@@ -145,97 +145,104 @@
 00000900: 6520 2d6e 204d 5363 6865 636b 2070 7974  e -n MScheck pyt
 00000910: 686f 6e3d 332e 3131 600a 0a32 2e20 4163  hon=3.11`..2. Ac
 00000920: 7469 7661 7465 2074 6865 204d 5363 6865  tivate the MSche
 00000930: 636b 2063 6f6e 6461 2065 6e76 6972 6f6e  ck conda environ
 00000940: 6d65 6e74 2063 7265 6174 6564 0a0a 2020  ment created..  
 00000950: 203e 2060 636f 6e64 6120 6163 7469 7661   > `conda activa
 00000960: 7465 204d 5363 6865 636b 600a 0a33 2e20  te MScheck`..3. 
-00000970: 5069 7020 696e 7374 616c 6c20 4d53 6368  Pip install MSch
-00000980: 6563 6b0a 2020 203e 2060 7069 7020 696e  eck.   > `pip in
-00000990: 7374 616c 6c20 6d73 6368 6563 6b60 0a0a  stall mscheck`..
-000009a0: 2320 3c61 206e 616d 653d 2250 7265 7061  # <a name="Prepa
-000009b0: 7269 6e67 2076 656e 646f 7220 6669 6c65  ring vendor file
-000009c0: 7322 3e3c 2f61 3e2a 2a50 7265 7061 7269  s"></a>**Prepari
-000009d0: 6e67 2076 656e 646f 7220 6669 6c65 732a  ng vendor files*
-000009e0: 2a0a 0a4d 5363 6865 636b 2068 6173 2062  *..MScheck has b
-000009f0: 6565 6e20 7465 7374 6564 206f 6e20 7573  een tested on us
-00000a00: 696e 6720 4167 696c 656e 7420 4c43 4d53  ing Agilent LCMS
-00000a10: 2066 696c 6573 2028 2e44 2920 6173 2074   files (.D) as t
-00000a20: 6865 2073 7461 7274 696e 6720 6669 6c65  he starting file
-00000a30: 2066 6f72 6d61 742e 204f 6e65 2063 6861   format. One cha
-00000a40: 6c6c 656e 6765 2069 7320 746f 2063 6f6e  llenge is to con
-00000a50: 7665 7274 2076 656e 646f 7220 6669 6c65  vert vendor file
-00000a60: 2066 6f72 6d61 7473 2069 6e74 6f0a 6120   formats into.a 
-00000a70: 666f 726d 6174 2077 6974 6820 7468 6520  format with the 
-00000a80: 6269 6e61 7279 2064 6563 6f64 6564 2e0a  binary decoded..
-00000a90: 0a31 2e20 436f 6e76 6572 7420 2e44 2041  .1. Convert .D A
-00000aa0: 6769 6c65 6e74 2066 6f6c 6465 7220 746f  gilent folder to
-00000ab0: 2061 202e 6420 4d61 7373 4875 6e74 6572   a .d MassHunter
-00000ac0: 2066 6f72 6d61 7420 7573 696e 6720 4167   format using Ag
-00000ad0: 696c 656e 7427 7320 4368 656d 5374 6174  ilent's ChemStat
-00000ae0: 696f 6e20 746f 204d 6173 7348 756e 7465  ion to MassHunte
-00000af0: 7220 5472 616e 736c 6174 6f72 2028 422e  r Translator (B.
-00000b00: 3034 2e30 3029 0a32 2e20 436f 6e76 6572  04.00).2. Conver
-00000b10: 7420 2e64 2066 6f72 6d61 7420 696e 746f  t .d format into
-00000b20: 202e 6d7a 4d4c 2066 6f72 6d61 7420 7573   .mzML format us
-00000b30: 696e 6720 5b50 726f 7465 6f57 697a 6172  ing [ProteoWizar
-00000b40: 6427 735d 2868 7474 703a 2f2f 7072 6f74  d's](http://prot
-00000b50: 656f 7769 7a61 7264 2e73 6f75 7263 6566  eowizard.sourcef
-00000b60: 6f72 6765 2e6e 6574 2f29 204d 5343 6f6e  orge.net/) MSCon
-00000b70: 7665 7274 2074 6f6f 6c0a 332e 2046 696e  vert tool.3. Fin
-00000b80: 616c 6c79 202d 2077 6520 6861 7665 2061  ally - we have a
-00000b90: 6e20 6669 6c65 2066 6f72 6d61 7420 7468  n file format th
-00000ba0: 6174 2077 6520 6361 6e20 7573 6521 0a34  at we can use!.4
-00000bb0: 2e20 496e 2079 6f75 7220 6661 766f 7572  . In your favour
-00000bc0: 6974 6520 4944 4520 6f72 204a 7570 7974  ite IDE or Jupyt
-00000bd0: 6572 206e 6f74 6562 6f6f 6b20 2d20 6120  er notebook - a 
-00000be0: 6261 7369 6320 6578 616d 706c 6520 6f66  basic example of
-00000bf0: 2075 7369 6e67 204d 5343 6865 636b 2069   using MSCheck i
-00000c00: 7320 7072 6f76 6964 6564 2062 656c 6f77  s provided below
-00000c10: 3a3c 6272 3e0a 0a60 6060 0a66 726f 6d20  :<br>..```.from 
-00000c20: 6d73 6368 6563 6b2e 616e 616c 7973 6520  mscheck.analyse 
-00000c30: 696d 706f 7274 2041 6e61 6c79 7365 5370  import AnalyseSp
-00000c40: 6563 7472 756d 0a0a 2320 4372 6561 7465  ectrum..# Create
-00000c50: 204d 5320 7363 7074 7275 6d20 6f62 6a65   MS scptrum obje
-00000c60: 6374 2061 6e64 2066 696e 6420 7065 616b  ct and find peak
-00000c70: 730a 7465 7374 203d 2041 6e61 6c79 7365  s.test = Analyse
-00000c80: 5370 6563 7472 756d 2822 3c70 6174 6820  Spectrum("<path 
-00000c90: 746f 202e 6d7a 4d4c 2066 696c 653e 222c  to .mzML file>",
-00000ca0: 206d 6f64 653d 2250 6f73 6974 6976 6522   mode="Positive"
-00000cb0: 290a 0a23 2053 6574 2053 4d49 4c45 5320  )..# Set SMILES 
-00000cc0: 6f66 2074 6172 6765 7420 746f 2073 6561  of target to sea
-00000cd0: 7263 6820 666f 720a 7461 7267 6574 5f53  rch for.target_S
-00000ce0: 4d49 4c45 5320 3d20 2243 434f 4328 3d4f  MILES = "CCOC(=O
-00000cf0: 294e 3143 434e 2843 283d 4f29 4e32 4343  )N1CCN(C(=O)N2CC
-00000d00: 4e28 4328 3d4f 2963 3363 6363 6f33 2943  N(C(=O)c3ccco3)C
-00000d10: 4332 2943 4331 220a 0a23 2041 6e61 6c79  C2)CC1"..# Analy
-00000d20: 7365 2074 6573 7420 7370 6563 7472 756d  se test spectrum
-00000d30: 2073 6561 7263 6869 6e67 2066 6f72 2074   searching for t
-00000d40: 6172 6765 7420 534d 494c 4553 0a74 6573  arget SMILES.tes
-00000d50: 742e 616e 616c 7973 6528 636f 6d70 6f75  t.analyse(compou
-00000d60: 6e64 736d 696c 6573 3d74 6172 6765 745f  ndsmiles=target_
-00000d70: 534d 494c 4553 2c0a 2020 2020 2020 2020  SMILES,.        
-00000d80: 2020 2020 2069 6f6e 7374 6f61 6464 3d5b       ionstoadd=[
-00000d90: 225b 485d 222c 2022 5b4e 615d 222c 2022  "[H]", "[Na]", "
-00000da0: 5b4b 5d22 2c20 225b 4e48 342b 5d22 5d2c  [K]", "[NH4+]"],
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 746f  .             to
-00000dc0: 6c65 7261 6e63 653d 3129 0a0a 2320 4372  lerance=1)..# Cr
-00000dd0: 6561 7465 2061 202e 7376 6720 7265 706f  eate a .svg repo
-00000de0: 7274 202d 2069 6620 796f 7520 646f 206e  rt - if you do n
-00000df0: 6f74 2067 6976 6520 6120 636f 6d70 6f75  ot give a compou
-00000e00: 6e64 5f6e 616d 650a 2320 7468 6520 656e  nd_name.# the en
-00000e10: 6469 6e67 206c 6561 6620 6f66 2074 6865  ding leaf of the
-00000e20: 2066 696c 6520 6e61 6d65 2077 696c 6c20   file name will 
-00000e30: 6265 2075 7365 640a 7465 7374 2e63 7265  be used.test.cre
-00000e40: 6174 655f 7265 706f 7274 2863 6f6d 706f  ate_report(compo
-00000e50: 756e 645f 6e61 6d65 3d22 5465 7374 2229  und_name="Test")
-00000e60: 0a60 6060 0a0a 203c 6272 3e0a 0a54 6865  .```.. <br>..The
-00000e70: 202e 7376 6720 7265 706f 7274 2077 696c   .svg report wil
-00000e80: 6c20 6265 2069 6e20 6120 666f 6c64 6572  l be in a folder
-00000e90: 2063 616c 6c65 6420 5265 706f 7274 730a   called Reports.
-00000ea0: 0a45 7861 6d70 6c65 206f 6620 7265 706f  .Example of repo
-00000eb0: 7274 206f 7574 7075 743a 3c62 723e 0a0a  rt output:<br>..
-00000ec0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000ed0: 223e 0a3c 696d 6720 7372 633d 2269 6d61  ">.<img src="ima
-00000ee0: 6765 732f 7265 706f 7274 2e73 7667 2220  ges/report.svg" 
-00000ef0: 7769 6474 683d 2236 3030 7078 223e 0a3c  width="600px">.<
-00000f00: 2f70 3e0a 0a0a                           /p>...
+00000970: 5069 7020 696e 7374 616c 6c20 7079 4f70  Pip install pyOp
+00000980: 656e 4d53 0a0a 2020 203e 2060 7069 7020  enMS..   > `pip 
+00000990: 696e 7374 616c 6c20 2d2d 696e 6465 782d  install --index-
+000009a0: 7572 6c20 6874 7470 733a 2f2f 7079 7069  url https://pypi
+000009b0: 2e63 732e 756e 692d 7475 6562 696e 6765  .cs.uni-tuebinge
+000009c0: 6e2e 6465 2f73 696d 706c 652f 2070 796f  n.de/simple/ pyo
+000009d0: 7065 6e6d 7360 0a0a 342e 2050 6970 2069  penms`..4. Pip i
+000009e0: 6e73 7461 6c6c 204d 5363 6865 636b 0a0a  nstall MScheck..
+000009f0: 2020 203e 2060 7069 7020 696e 7374 616c     > `pip instal
+00000a00: 6c20 6d73 6368 6563 6b60 0a0a 2320 3c61  l mscheck`..# <a
+00000a10: 206e 616d 653d 2250 7265 7061 7269 6e67   name="Preparing
+00000a20: 2076 656e 646f 7220 6669 6c65 7322 3e3c   vendor files"><
+00000a30: 2f61 3e2a 2a50 7265 7061 7269 6e67 2076  /a>**Preparing v
+00000a40: 656e 646f 7220 6669 6c65 732a 2a0a 0a4d  endor files**..M
+00000a50: 5363 6865 636b 2068 6173 2062 6565 6e20  Scheck has been 
+00000a60: 7465 7374 6564 206f 6e20 7573 696e 6720  tested on using 
+00000a70: 4167 696c 656e 7420 4c43 4d53 2066 696c  Agilent LCMS fil
+00000a80: 6573 2028 2e44 2920 6173 2074 6865 2073  es (.D) as the s
+00000a90: 7461 7274 696e 6720 6669 6c65 2066 6f72  tarting file for
+00000aa0: 6d61 742e 204f 6e65 2063 6861 6c6c 656e  mat. One challen
+00000ab0: 6765 2069 7320 746f 2063 6f6e 7665 7274  ge is to convert
+00000ac0: 2076 656e 646f 7220 6669 6c65 2066 6f72   vendor file for
+00000ad0: 6d61 7473 2069 6e74 6f0a 6120 666f 726d  mats into.a form
+00000ae0: 6174 2077 6974 6820 7468 6520 6269 6e61  at with the bina
+00000af0: 7279 2064 6563 6f64 6564 2e0a 0a31 2e20  ry decoded...1. 
+00000b00: 436f 6e76 6572 7420 2e44 2041 6769 6c65  Convert .D Agile
+00000b10: 6e74 2066 6f6c 6465 7220 746f 2061 202e  nt folder to a .
+00000b20: 6420 4d61 7373 4875 6e74 6572 2066 6f72  d MassHunter for
+00000b30: 6d61 7420 7573 696e 6720 4167 696c 656e  mat using Agilen
+00000b40: 7427 7320 4368 656d 5374 6174 696f 6e20  t's ChemStation 
+00000b50: 746f 204d 6173 7348 756e 7465 7220 5472  to MassHunter Tr
+00000b60: 616e 736c 6174 6f72 2028 422e 3034 2e30  anslator (B.04.0
+00000b70: 3029 0a32 2e20 436f 6e76 6572 7420 2e64  0).2. Convert .d
+00000b80: 2066 6f72 6d61 7420 696e 746f 202e 6d7a   format into .mz
+00000b90: 4d4c 2066 6f72 6d61 7420 7573 696e 6720  ML format using 
+00000ba0: 5b50 726f 7465 6f57 697a 6172 6427 735d  [ProteoWizard's]
+00000bb0: 2868 7474 703a 2f2f 7072 6f74 656f 7769  (http://proteowi
+00000bc0: 7a61 7264 2e73 6f75 7263 6566 6f72 6765  zard.sourceforge
+00000bd0: 2e6e 6574 2f29 204d 5343 6f6e 7665 7274  .net/) MSConvert
+00000be0: 2074 6f6f 6c0a 332e 2046 696e 616c 6c79   tool.3. Finally
+00000bf0: 202d 2077 6520 6861 7665 2061 6e20 6669   - we have an fi
+00000c00: 6c65 2066 6f72 6d61 7420 7468 6174 2077  le format that w
+00000c10: 6520 6361 6e20 7573 6521 0a34 2e20 496e  e can use!.4. In
+00000c20: 2079 6f75 7220 6661 766f 7572 6974 6520   your favourite 
+00000c30: 4944 4520 6f72 204a 7570 7974 6572 206e  IDE or Jupyter n
+00000c40: 6f74 6562 6f6f 6b20 2d20 6120 6261 7369  otebook - a basi
+00000c50: 6320 6578 616d 706c 6520 6f66 2075 7369  c example of usi
+00000c60: 6e67 204d 5343 6865 636b 2069 7320 7072  ng MSCheck is pr
+00000c70: 6f76 6964 6564 2062 656c 6f77 3a3c 6272  ovided below:<br
+00000c80: 3e0a 0a60 6060 0a66 726f 6d20 6d73 6368  >..```.from msch
+00000c90: 6563 6b2e 616e 616c 7973 6520 696d 706f  eck.analyse impo
+00000ca0: 7274 2041 6e61 6c79 7365 5370 6563 7472  rt AnalyseSpectr
+00000cb0: 756d 0a0a 2320 4372 6561 7465 204d 5320  um..# Create MS 
+00000cc0: 7363 7074 7275 6d20 6f62 6a65 6374 2061  scptrum object a
+00000cd0: 6e64 2066 696e 6420 7065 616b 730a 7465  nd find peaks.te
+00000ce0: 7374 203d 2041 6e61 6c79 7365 5370 6563  st = AnalyseSpec
+00000cf0: 7472 756d 2822 3c70 6174 6820 746f 202e  trum("<path to .
+00000d00: 6d7a 4d4c 2066 696c 653e 222c 206d 6f64  mzML file>", mod
+00000d10: 653d 2250 6f73 6974 6976 6522 290a 0a23  e="Positive")..#
+00000d20: 2053 6574 2053 4d49 4c45 5320 6f66 2074   Set SMILES of t
+00000d30: 6172 6765 7420 746f 2073 6561 7263 6820  arget to search 
+00000d40: 666f 720a 7461 7267 6574 5f53 4d49 4c45  for.target_SMILE
+00000d50: 5320 3d20 2243 434f 4328 3d4f 294e 3143  S = "CCOC(=O)N1C
+00000d60: 434e 2843 283d 4f29 4e32 4343 4e28 4328  CN(C(=O)N2CCN(C(
+00000d70: 3d4f 2963 3363 6363 6f33 2943 4332 2943  =O)c3ccco3)CC2)C
+00000d80: 4331 220a 0a23 2041 6e61 6c79 7365 2074  C1"..# Analyse t
+00000d90: 6573 7420 7370 6563 7472 756d 2073 6561  est spectrum sea
+00000da0: 7263 6869 6e67 2066 6f72 2074 6172 6765  rching for targe
+00000db0: 7420 534d 494c 4553 0a74 6573 742e 616e  t SMILES.test.an
+00000dc0: 616c 7973 6528 636f 6d70 6f75 6e64 736d  alyse(compoundsm
+00000dd0: 696c 6573 3d74 6172 6765 745f 534d 494c  iles=target_SMIL
+00000de0: 4553 2c0a 2020 2020 2020 2020 2020 2020  ES,.            
+00000df0: 2069 6f6e 7374 6f61 6464 3d5b 225b 485d   ionstoadd=["[H]
+00000e00: 222c 2022 5b4e 615d 222c 2022 5b4b 5d22  ", "[Na]", "[K]"
+00000e10: 2c20 225b 4e48 342b 5d22 5d2c 0a20 2020  , "[NH4+]"],.   
+00000e20: 2020 2020 2020 2020 2020 746f 6c65 7261            tolera
+00000e30: 6e63 653d 3129 0a0a 2320 4372 6561 7465  nce=1)..# Create
+00000e40: 2061 202e 7376 6720 7265 706f 7274 202d   a .svg report -
+00000e50: 2069 6620 796f 7520 646f 206e 6f74 2067   if you do not g
+00000e60: 6976 6520 6120 636f 6d70 6f75 6e64 5f6e  ive a compound_n
+00000e70: 616d 650a 2320 7468 6520 656e 6469 6e67  ame.# the ending
+00000e80: 206c 6561 6620 6f66 2074 6865 2066 696c   leaf of the fil
+00000e90: 6520 6e61 6d65 2077 696c 6c20 6265 2075  e name will be u
+00000ea0: 7365 640a 7465 7374 2e63 7265 6174 655f  sed.test.create_
+00000eb0: 7265 706f 7274 2863 6f6d 706f 756e 645f  report(compound_
+00000ec0: 6e61 6d65 3d22 5465 7374 2229 0a60 6060  name="Test").```
+00000ed0: 0a0a 203c 6272 3e0a 0a54 6865 202e 7376  .. <br>..The .sv
+00000ee0: 6720 7265 706f 7274 2077 696c 6c20 6265  g report will be
+00000ef0: 2069 6e20 6120 666f 6c64 6572 2063 616c   in a folder cal
+00000f00: 6c65 6420 5265 706f 7274 730a 0a45 7861  led Reports..Exa
+00000f10: 6d70 6c65 206f 6620 7265 706f 7274 206f  mple of report o
+00000f20: 7574 7075 743a 3c62 723e 0a0a 3c70 2061  utput:<br>..<p a
+00000f30: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+00000f40: 696d 6720 7372 633d 2269 6d61 6765 732f  img src="images/
+00000f50: 7265 706f 7274 2e73 7667 2220 7769 6474  report.svg" widt
+00000f60: 683d 2236 3030 7078 223e 0a3c 2f70 3e0a  h="600px">.</p>.
+00000f70: 0a0a                                     ..
```

### Comparing `mscheck-0.2.8b0/setup.py` & `mscheck-0.2.9b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     author_email="waztom@gmail.com",
     py_modules=["mscheck"],
     description="Auto MS mass checker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     install_requires=[
-        "pyopenms",
         "rdkit",
         "matplotlib",
         "scipy",
         "svgutils",
     ],
     packages=find_packages(),
     url="https://github.com/Waztom/mscheck",
```

### Comparing `mscheck-0.2.8b0/tests/test_analyse.py` & `mscheck-0.2.9b0/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.8b0/tests/test_spectrum.py` & `mscheck-0.2.9b0/tests/test_spectrum.py`

 * *Files identical despite different names*


# Comparing `tmp/serl-0.1.0b0.tar.gz` & `tmp/serl-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serl-0.1.0b0.tar", last modified: Mon Apr 24 09:34:26 2023, max compression
+gzip compressed data, was "serl-0.2.0b0.tar", last modified: Thu Apr 27 11:19:50 2023, max compression
```

## Comparing `serl-0.1.0b0.tar` & `serl-0.2.0b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.668791 serl-0.1.0b0/
--rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.1.0b0/LICENSE
--rw-rw-rw-   0        0        0     2116 2023-04-24 09:34:26.668791 serl-0.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-03-30 20:15:20.000000 serl-0.1.0b0/README.md
--rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.1.0b0/pyproject.toml
--rw-rw-rw-   0        0        0      830 2023-04-24 09:34:26.675340 serl-0.1.0b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.581134 serl-0.1.0b0/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.635625 serl-0.1.0b0/src/serl/
--rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.1.0b0/src/serl/__init__.py
--rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.1.0b0/src/serl/__main__.py
--rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.1.0b0/src/serl/config.py
--rw-rw-rw-   0        0        0     3691 2023-04-24 09:28:08.000000 serl-0.1.0b0/src/serl/constants.py
--rw-rw-rw-   0        0        0     3814 2023-04-21 14:35:48.000000 serl-0.1.0b0/src/serl/highlight.py
--rw-rw-rw-   0        0        0     2670 2023-04-21 14:39:06.000000 serl-0.1.0b0/src/serl/lexer.py
--rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.1.0b0/src/serl/logger.py
--rw-rw-rw-   0        0        0    18130 2023-04-24 09:20:33.000000 serl-0.1.0b0/src/serl/main.py
--rw-rw-rw-   0        0        0     4893 2023-04-21 13:33:46.000000 serl-0.1.0b0/src/serl/parser.py
--rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.1.0b0/src/serl/schema.py
--rw-rw-rw-   0        0        0     4588 2023-04-17 08:06:23.000000 serl-0.1.0b0/src/serl/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.656553 serl-0.1.0b0/src/serl.egg-info/
--rw-rw-rw-   0        0        0     2116 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.667784 serl-0.1.0b0/tests/
--rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.1.0b0/tests/test_config.py
--rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.1.0b0/tests/test_highlight.py
--rw-rw-rw-   0        0        0     1603 2023-04-17 18:39:39.000000 serl-0.1.0b0/tests/test_lexer.py
--rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.1.0b0/tests/test_main.py
--rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.1.0b0/tests/test_parser.py
--rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.1.0b0/tests/test_schema.py
--rw-rw-rw-   0        0        0     5478 2023-04-17 17:32:39.000000 serl-0.1.0b0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:19:50.672275 serl-0.2.0b0/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.2.0b0/LICENSE
+-rw-rw-rw-   0        0        0     2294 2023-04-27 11:19:50.672275 serl-0.2.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-04-25 12:49:32.000000 serl-0.2.0b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.2.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0      897 2023-04-27 11:19:50.673550 serl-0.2.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 11:19:50.615109 serl-0.2.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 11:19:50.639000 serl-0.2.0b0/src/serl/
+-rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.2.0b0/src/serl/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.2.0b0/src/serl/__main__.py
+-rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.2.0b0/src/serl/config.py
+-rw-rw-rw-   0        0        0     3691 2023-04-27 11:12:08.000000 serl-0.2.0b0/src/serl/constants.py
+-rw-rw-rw-   0        0        0     3820 2023-04-26 14:50:50.000000 serl-0.2.0b0/src/serl/highlight.py
+-rw-rw-rw-   0        0        0     3731 2023-04-26 14:18:07.000000 serl-0.2.0b0/src/serl/lexer.py
+-rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.2.0b0/src/serl/logger.py
+-rw-rw-rw-   0        0        0    18751 2023-04-26 14:42:42.000000 serl-0.2.0b0/src/serl/main.py
+-rw-rw-rw-   0        0        0     4893 2023-04-25 10:39:37.000000 serl-0.2.0b0/src/serl/parser.py
+-rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.2.0b0/src/serl/schema.py
+-rw-rw-rw-   0        0        0     4772 2023-04-25 10:43:38.000000 serl-0.2.0b0/src/serl/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:19:50.662079 serl-0.2.0b0/src/serl.egg-info/
+-rw-rw-rw-   0        0        0     2294 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 11:19:50.000000 serl-0.2.0b0/src/serl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 11:19:50.671787 serl-0.2.0b0/tests/
+-rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.2.0b0/tests/test_config.py
+-rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.2.0b0/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     2156 2023-04-26 14:06:44.000000 serl-0.2.0b0/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.2.0b0/tests/test_main.py
+-rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.2.0b0/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.2.0b0/tests/test_schema.py
+-rw-rw-rw-   0        0        0     5486 2023-04-25 06:59:43.000000 serl-0.2.0b0/tests/test_utils.py
```

### Comparing `serl-0.1.0b0/LICENSE` & `serl-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/PKG-INFO` & `serl-0.2.0b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
 License: MIT
-Project-URL: repository, https://github.com/harrydowning/serl
+Project-URL: Repository, https://github.com/harrydowning/serl
+Project-URL: Documentation, https://serl.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Serialized Language (serl)
 Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
+Documentation can be found on [Read The Docs](https://serl.readthedocs.io/en/latest/index.html).
+
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
 | `py -m build` | Build distribution |
```

### Comparing `serl-0.1.0b0/README.md` & `serl-0.2.0b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Serialized Language (serl)
 Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
+Documentation can be found on [Read The Docs](https://serl.readthedocs.io/en/latest/index.html).
+
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
 | `py -m build` | Build distribution |
```

### Comparing `serl-0.1.0b0/setup.cfg` & `serl-0.2.0b0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,41 +12,46 @@
 000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
 000000c0: 6669 6c65 3a20 5245 4144 4d45 2e6d 642c  file: README.md,
 000000d0: 204c 4943 454e 5345 0d0a 6c6f 6e67 5f64   LICENSE..long_d
 000000e0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 000000f0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
 00000100: 6172 6b64 6f77 6e0d 0a6c 6963 656e 7365  arkdown..license
 00000110: 203d 204d 4954 0d0a 7072 6f6a 6563 745f   = MIT..project_
-00000120: 7572 6c73 203d 200d 0a09 7265 706f 7369  urls = ...reposi
+00000120: 7572 6c73 203d 200d 0a09 5265 706f 7369  urls = ...Reposi
 00000130: 746f 7279 203d 2068 7474 7073 3a2f 2f67  tory = https://g
 00000140: 6974 6875 622e 636f 6d2f 6861 7272 7964  ithub.com/harryd
-00000150: 6f77 6e69 6e67 2f73 6572 6c0d 0a63 6c61  owning/serl..cla
-00000160: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000170: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000180: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000190: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-000001a0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001b0: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-000001c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000001d0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-000001e0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-000001f0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000200: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000210: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000220: 6571 7569 7265 7320 3d20 3e3d 332e 3131  equires = >=3.11
-00000230: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000240: 6573 203d 200d 0a09 5079 5941 4d4c 0d0a  es = ...PyYAML..
-00000250: 0964 6f63 6f70 740d 0a09 706c 793d 3d33  .docopt...ply==3
-00000260: 2e31 310d 0a09 7265 6765 780d 0a09 6e65  .11...regex...ne
-00000270: 7477 6f72 6b78 0d0a 096a 736f 6e73 6368  tworkx...jsonsch
-00000280: 656d 610d 0a09 5079 676d 656e 7473 0d0a  ema...Pygments..
-00000290: 0950 696c 6c6f 770d 0a09 7265 7175 6573  .Pillow...reques
-000002a0: 7473 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ts....[options.p
-000002b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000002c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
-000002d0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000002e0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-000002f0: 7269 7074 7320 3d20 0d0a 0973 6572 6c20  ripts = ...serl 
-00000300: 3d20 7365 726c 2e6d 6169 6e3a 6d61 696e  = serl.main:main
-00000310: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000320: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000330: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000150: 6f77 6e69 6e67 2f73 6572 6c0d 0a09 446f  owning/serl...Do
+00000160: 6375 6d65 6e74 6174 696f 6e20 3d20 6874  cumentation = ht
+00000170: 7470 733a 2f2f 7365 726c 2e72 6561 6474  tps://serl.readt
+00000180: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000190: 6573 742f 696e 6465 782e 6874 6d6c 0d0a  est/index.html..
+000001a0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+000001b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000001d0: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
+000001e0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001f0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
+00000200: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000210: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000220: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
+00000230: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000240: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+00000250: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000260: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000270: 2e31 310d 0a69 6e73 7461 6c6c 5f72 6571  .11..install_req
+00000280: 7569 7265 7320 3d20 0d0a 0950 7959 414d  uires = ...PyYAM
+00000290: 4c0d 0a09 646f 636f 7074 0d0a 0970 6c79  L...docopt...ply
+000002a0: 3d3d 332e 3131 0d0a 0972 6567 6578 0d0a  ==3.11...regex..
+000002b0: 096e 6574 776f 726b 780d 0a09 6a73 6f6e  .networkx...json
+000002c0: 7363 6865 6d61 0d0a 0950 7967 6d65 6e74  schema...Pygment
+000002d0: 730d 0a09 5069 6c6c 6f77 0d0a 0972 6571  s...Pillow...req
+000002e0: 7565 7374 730d 0a0d 0a5b 6f70 7469 6f6e  uests....[option
+000002f0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000300: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000310: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+00000320: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
+00000330: 5f73 6372 6970 7473 203d 200d 0a09 7365  _scripts = ...se
+00000340: 726c 203d 2073 6572 6c2e 6d61 696e 3a6d  rl = serl.main:m
+00000350: 6169 6e0d 0a0d 0a5b 6567 675f 696e 666f  ain....[egg_info
+00000360: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000370: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000380: 0a                                       .
```

### Comparing `serl-0.1.0b0/src/serl/config.py` & `serl-0.2.0b0/src/serl/config.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/src/serl/constants.py` & `serl-0.2.0b0/src/serl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 NAME = __package__
-VERSION = '0.1.0-beta'
+VERSION = '0.2.0-beta'
 
 SYSTEM_CONFIG_DIR = f'.{NAME}'
 SYSTEM_CONFIG_ENV_DIR = 'environments'
 SHELL_CHAR = '$'
 VENV_CONFIG = 'pyvenv.cfg'
 EXCEPTION_ATTR = 'serl_loc'
```

### Comparing `serl-0.1.0b0/src/serl/highlight.py` & `serl-0.2.0b0/src/serl/highlight.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from pygments.style import Style, StyleMeta
 from pygments.util import ClassNotFound
 from pygments.lexer import RegexLexer
 from pygments.token import string_to_tokentype, Token, Comment, Whitespace
 from pygments.formatters import get_formatter_by_name
 from pygments.styles import get_style_by_name
 
-SerlToken = string_to_tokentype('Token.Serl')
+# SerlToken = string_to_tokentype('Token.Serl')
 def get_pygments_lexer(_tokens: dict, ignore: str, tokentypes: dict):
     tokentypes = {t: ttype.title() for t, ttype in tokentypes.items()}
     class PygmentsLexer(RegexLexer):
         flags = re.VERBOSE
 
         tokens = {
             'root': [
                 (_tokens.get(name_or_pattern, name_or_pattern), 
                  string_to_tokentype(ttype)) 
                 for name_or_pattern, ttype in tokentypes.items()
             ] + [(r'\s', Whitespace)]
         }
         if ignore:
             tokens['root'].append((ignore, Comment))
-        tokens['root'].append(('.', SerlToken))
+        # tokens['root'].append(('.', SerlToken))
     try:
         return PygmentsLexer()
     except ValueError as err:
         logger.error(f'Syntax highlighter lexer error: {err}', code=1)
 
 def get_pygments_style(style: StyleMeta, user_styles: dict[str, str]):
     attrs = {
@@ -38,15 +38,15 @@
         if not attr.startswith('_')
     }
 
     attrs['styles'] = attrs.get('styles', {}) | {
         string_to_tokentype(tokentype.title()): user_style
         for tokentype, user_style in user_styles.items()
     }
-    attrs['styles'][SerlToken] = attrs['styles'][Token]
+    # attrs['styles'][SerlToken] = attrs['styles'][Token]
     # Create class with type(...) to allow dynamic creation of attrs
     PygmentsStyle = type('PygmentsStyle', (Style,), attrs)
     return PygmentsStyle
 
 def parse_key_value(input: str) -> dict:
     result = {}
     str_re = r'(?s)([\'\"])(.*?)\1'
```

### Comparing `serl-0.1.0b0/src/serl/lexer.py` & `serl-0.2.0b0/src/serl/lexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,35 +5,54 @@
 
 import ply.lex as lex
 import regex
 
 implementation = platform.python_implementation()
 using_cpython = implementation == 'CPython'
 
-def get_pattern_func(token, pattern, using_regex):
+class SerlToken(tuple):
+    def __new__(cls, lineno, col, captures):
+        return super(SerlToken, cls).__new__(cls, (*captures,))
+    
+    def __init__(self, lineno, col, *captures):
+        super().__init__()
+        self.lineno = lineno
+        self.col = col
+
+def get_pattern_func(token, pattern, using_regex, g_span):
     def f(t):
-        s, e = t.lexer.lexmatch.span()
-        string = t.lexer.lexmatch.string[s:e]
-        # Obtain capture groups
+        lexmatch = t.lexer.lexmatch
+        span = lexmatch.span()
+        lineno = t.lexer.lineno
+        col = (span[0] + 1) - getattr(t.lexer, 'lastlinepos', 0)
+        
+        g_start, g_end = g_span
         if using_regex and using_cpython:
-            m = regex.match(pattern, string, regex.VERBOSE)
-            t.value = m.allcaptures()
+            groups = lexmatch.allcaptures()
+            # Add 1 as allcaptures has 1 whole capture first
+            t.value = SerlToken(lineno, col, groups[g_start + 1: g_end + 1])
         else:
-            m = re.match(pattern, string, re.VERBOSE)
-            t.value = (m.group(), *m.groups())
-        t.lexer.lineno += string.count('\n')
+            groups = lexmatch.groups()
+            t.value = SerlToken(lineno, col, groups[g_start:g_end])
+
+        string = t.lexer.lexdata[span[0]:span[1]]
+        newlines = string.count('\n')
+        if newlines:
+            t.lexer.lineno += newlines
+            t.lexer.lastlinepos = t.lexer.lexpos
         return t
     
     f.__doc__ = pattern
     f.__name__ = token
     return f
 
 def newline(t):
     r'\n+'
     t.lexer.lineno += len(t.value)
+    t.lexer.lastlinepos = t.lexer.lexpos
 
 def t_error(t):
     logger.error(f'Illegal character \'{t.value[0]}\' on line '
                  f'{t.lexer.lineno}.')
 
 def get_ignore_func(pattern):
     def f(t): pass
@@ -43,33 +62,15 @@
 
 def get_whole_match(token):
     if isinstance(token.value[0], list):
         return token.value[0][0]
     else:
         return token.value[0]
 
-def build_lexer(_tokens: dict[str, str], token_map: dict[str,str], ignore: str,
-                using_regex: bool, flags: str, default: bool):
-    g = globals()
-    g['tokens'] = ('default',) if default else ()
-
-    for token, pattern in _tokens.items():
-        token_name = token_map[token]
-
-        g['tokens'] = (*g['tokens'], token_name)
-        g[f't_{token_name}'] = get_pattern_func(token, pattern, using_regex)
-
-    # Lower precedence than user rules
-    g['t_newline'] = newline
-    if ignore != None:
-        g['t_ignore_func'] = get_ignore_func(ignore)
-    
-    if default:
-        g['t_default'] = '.'
-
+def get_flag_value(using_regex, flags):
     if using_regex:
         if using_cpython:
             lex.re = regex
         else:
             logger.error(f'Use of \'regex\' package requires \'CPython\' '
                          f'implementation. Current implementation: '
                          f'\'{implementation}\'.', code=1)
@@ -80,10 +81,38 @@
             flag = getattr(lex.re, flag_str)
             if isinstance(flag, lex.re.RegexFlag):
                 flag_value |= flag
                 continue
         except AttributeError:
             pass
         logger.warning(f'Can\'t find regex flag \'{flag_str}\'.')
+    return flag_value
+
+def build_lexer(_tokens: dict[str, str], token_map: dict[str,str], ignore: str,
+                using_regex: bool, flags: str, default: bool): 
+    flag_value = get_flag_value(using_regex, flags)
+    
+    g = globals()
+    g['tokens'] = ('default',) if default else ()
+
+    g_start = 0
+    for token, pattern in _tokens.items():
+        token_name = token_map[token]
+        # Add 1 as PLY surrounds each token pattern i.e., an extra group
+        groups = lex.re.compile(pattern).groups + 1
+        g_end = g_start + groups
+
+        g['tokens'] = (*g['tokens'], token_name)
+        g[f't_{token_name}'] = get_pattern_func(token, pattern, using_regex,
+                                                (g_start, g_end))
+        g_start += groups
+
+    # Lower precedence than user rules
+    g['t_newline'] = newline
+    if ignore != None:
+        g['t_ignore_func'] = get_ignore_func(ignore)
+    
+    if default:
+        g['t_default'] = '.'
     
     errorlog = logger.LoggingWrapper(ply_repl=True)
     return lex.lex(errorlog=errorlog, reflags=flag_value)
```

### Comparing `serl-0.1.0b0/src/serl/logger.py` & `serl-0.2.0b0/src/serl/logger.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/src/serl/main.py` & `serl-0.2.0b0/src/serl/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,16 +162,16 @@
     flags = meta_tokens.get('flags', 'VERBOSE')
     default = meta_tokens.get('default', True)
     
     tokens_copy = tokens.copy()
     if ref != None:
         # if 'token' not used assume given string is prefix of token repl.
         ref += '' if 'token' in ref else 'token'
-        logger.info(f'Performing token expansion with \'ref\' pattern '
-                    f'\'{ref}\' (default: \'{DEFAULT_REF}\')')
+        logger.info(f'Performing token expansion with $.meta.tokens.ref '
+                    f'pattern \'{ref}\'')
         tokens = token_expansion(tokens, ref.split('token'))
     
     for token in tokens_copy:
         tb, ta = tokens_copy[token].strip(), tokens[token].strip()
         if tb != ta: # TODO case where expansion is actually equal?
             logger.info(f'Token \'{token}\' expanded: \'{tb}\' -> \'{ta}\'')
 
@@ -187,14 +187,22 @@
     s = '\', \''
     if common_keys:
         logger.error(f'Grammar identifiers \'{s.join(common_keys)}\' already '
                      f'used in tokens', code=1)
     
     symbol_map = token_map | grammar_map
     grammar = utils.normalise_grammar(symbol_map, grammar)
+    
+    flipped_grammar_map = utils.flip_dict(grammar_map)
+    for nt, rules in grammar.items():
+        for i, rule in enumerate(rules):
+            if rule.strip() == '':
+                name = flipped_grammar_map[nt]
+                msg = f'Empty production in $.grammar.{name}[{i}] not allowed'
+                logger.error(msg, code=1)
 
     tokens_used, implicit_map = utils.get_tokens_in_grammar(token_map, 
                                                             error_sym, grammar)
     tokens = utils.keep_keys_in_list(tokens, tokens_used)
     token_map = utils.keep_keys_in_list(token_map, tokens_used) | implicit_map
     tokens |= {k: re.escape(k) for k, v in implicit_map.items()}
     symbol_map = token_map | grammar_map
@@ -243,21 +251,24 @@
     serl_ast = parser.parse(src, lexer=lexer, tracking=True)
     if (not permissive and logger.error_seen) or not serl_ast:
         logger.error('Parse Failed', code=1)
     
     code = utils.normalise_dict(config['code'])
     main_code = utils.get_main_code(code, grammar_map)
     
-    for code_name, code_list in code.items():
-        internal_name = grammar_map.get(code_name, None)
-        if not internal_name: continue
-        for i in range(len(grammar[internal_name])):
-            value = code_list[i] if len(code_list) > i else None
-            if value == None:
-                logger.warning(f'Code missing for $.code.{code_name}[{i}]')
+    flipped_grammar_map = utils.flip_dict(grammar_map)
+    for nt, rules in grammar.items():
+        name = flipped_grammar_map.get(nt, None)
+        code_list = code.get(name, None)
+        if code_list != None:
+            for i in range(len(rules)):
+                if len(code_list) <= i or not code_list[i]:
+                    logger.warning(f'Code missing for $.code.{name}[{i}]')
+            continue
+        logger.warning(f'Code missing for $.code.{name}')
     
     # #################################################################
 
     venv_name = config.get('environment', None)
     venv_created = False
     if venv_name:
         for sitepackage in site.getsitepackages():
@@ -289,28 +300,34 @@
         '__name__': lang_name,
         'args': language_args,
     }
     execute_func = get_execute_func(serl_ast, code, global_env)
     sys.setrecursionlimit(10000)
     try:
         if main_code:
+            name = main_code[0]
             global_env[serl_ast[0]] = execute_func
-            result = exec_or_error(main_code[0], 0, main_code[1], global_env)
+            for i, m_code in enumerate(main_code[1]):
+                result = exec_or_error(name, i, m_code, global_env)
+                if result:
+                    print(result)
         else:
             result = execute_func()
+            if result:
+                print(result)
     except SyntaxError as err:
         err.__traceback__ = None
         err.__context__ = None
         err.__notes__ = None
         err.filename = getattr(err, EXCEPTION_ATTR, '')
         logger.error(f'In {err.filename}:\n\n', exc_info=True, code=1)
     except subprocess.CalledProcessError as err:
         err.__notes__ = None
         filename = getattr(err, EXCEPTION_ATTR, '')
-        logger.error(f'In {filename}:\n\n{err.stderr}',code=err.returncode)
+        logger.error(f'In {filename}:\n\n{err.cmd}\n\n{err.stderr}',code=err.returncode)
     except Exception as err:
         filename_re = r'^\$\.code\.(.*?)\[(\d+)\]$'
         frames = traceback.extract_tb(err.__traceback__)
         frame = next((frame for frame in frames[::-1] 
                         if re.match(filename_re, frame.filename)), frames[-1])
         name, i = re.match(filename_re, frame.filename).groups()
         i = int(i)
@@ -318,17 +335,15 @@
         err.__traceback__ = None
         err.__context__ = None
         code_lines = code[name][i].split('\n')
         code_line = code_lines[lineno - 1]
         err.__notes__ = None
         err_msg = f'In {frame.filename}, line {lineno}:\n\n{code_line}\n\n'
         logger.error(err_msg, exc_info=True, code=1)
-
-    if result:
-        print(result)
+    # End of run
 
 def exec_and_eval(name, i, code, global_env, local_env=None):
     filename = f'$.code.{name}[{i}]'
     code_ast = ast.parse(code)
 
     try:
         last_stmt = code_ast.body.pop()
```

### Comparing `serl-0.1.0b0/src/serl/parser.py` & `serl-0.2.0b0/src/serl/parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/src/serl/schema.py` & `serl-0.2.0b0/src/serl/schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/src/serl/utils.py` & `serl-0.2.0b0/src/serl/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import os
 from typing import Callable, Iterable
+import serl.logger as logger
 
 def expand(rule: str, symbol_map: list[tuple[str, str]], 
            symbol_f: Callable[[str], str] = lambda x: x, 
            repl_f: Callable[[str], str] = lambda x: x):
     if symbol_map == []:
         return rule
     symbol, repl = symbol_map[0]
@@ -75,14 +76,17 @@
             new_rule = ''
             for symbol in rule.split(' '):
                 if symbol in tokens:
                     tokens_used.add(flipped_token_map[symbol])
                 elif symbol in nonterms:
                     pass
                 elif symbol == error:
+                    if i == len(rules) - 1:
+                        logger.error(f'Error token \'{symbol}\' appears at the'
+                                     f' end of a production.', code=1)
                     symbol = 'error'
                 else:
                     if not implicit_map.get(symbol, None):
                         implicit_map[symbol] = f'ITERMINAL{len(implicit_map)}'
                     symbol = implicit_map[symbol]
                 new_rule += f'{symbol} '
             norm_grammar[nt][i] = new_rule.strip()
@@ -102,13 +106,13 @@
 def get_valid_identifier(s: str):
    s = re.sub('[^0-9a-zA-Z_]', '', s)
    s = re.sub('^[^a-zA-Z_]+', '', s)
    return s
 
 def get_main_code(
         code: dict[str, list[str]], grammar_map: dict[str, str]
-    ) -> tuple[str, str] | None:
+    ) -> tuple[str, list[str]] | None:
     item = next(iter(code.items()), None)
-    if item:
-        return None if item[0] in grammar_map else (item[0], next(iter(item[1]), None))
-    else:
+    if item[0] in grammar_map:
         return None
+    else:
+        return item
```

### Comparing `serl-0.1.0b0/src/serl.egg-info/PKG-INFO` & `serl-0.2.0b0/src/serl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
 License: MIT
-Project-URL: repository, https://github.com/harrydowning/serl
+Project-URL: Repository, https://github.com/harrydowning/serl
+Project-URL: Documentation, https://serl.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Serialized Language (serl)
 Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
+Documentation can be found on [Read The Docs](https://serl.readthedocs.io/en/latest/index.html).
+
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
 | `py -m build` | Build distribution |
```

### Comparing `serl-0.1.0b0/src/serl.egg-info/SOURCES.txt` & `serl-0.2.0b0/src/serl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_config.py` & `serl-0.2.0b0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_highlight.py` & `serl-0.2.0b0/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_lexer.py` & `serl-0.2.0b0/tests/test_lexer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from types import SimpleNamespace
 import pytest
 import serl.lexer as lexer
+import re, regex
 
 class MockLexToken(object):
-    def __init__(self, span=None, string=None, lineno=None, value=None):
+    def __init__(self, span=(0,0), string=None, lineno=None, value=None, allcaptures=None, groups=None):
         self.lexer = SimpleNamespace(
-            lexmatch = SimpleNamespace(span=lambda: span, string=string),
-            lineno = lineno
+            lexmatch = SimpleNamespace(
+                span= lambda: span,
+                allcaptures=lambda: allcaptures,
+                groups= lambda: groups
+            ),
+            lineno = lineno,
+            lexpos = span[0],
+            lexdata = string
         )
         self.value = value
 
     def __eq__(self, __value: object) -> bool:
         return __value.value == self.value and __value.lexer.lineno == self.lexer.lineno
 
 
 @pytest.mark.parametrize('token, pattern, using_regex, using_cpython, t, expected', [
-    ('TOK1', r':(\d+):', False, True, MockLexToken((3,8), 'aaa:123:a', 1), MockLexToken(lineno=1, value=(':123:', '123'))),
-    ('TOK2', r':(\d+):', True, True, MockLexToken((3,8), 'aaa:123:a', 2), MockLexToken(lineno=2, value=([':123:'], ['123']))),
-    ('TOK3', r'(\|(\d+))+\n', True, True, MockLexToken((5,20), 'start|1|22|333|4444\nend', 2), MockLexToken(lineno=3, value=(['|1|22|333|4444\n'], ['|1', '|22', '|333', '|4444'], ['1', '22', '333', '4444']))),
+    ('TOK1', r':(\d+):', False, True, MockLexToken((3,8), 'aaa:123:a', 1, ':123:', groups=(':123:', '123')), MockLexToken(lineno=1, value=(':123:', '123'))),
+    ('TOK2', r':(\d+):', True, True, MockLexToken((3,8), 'aaa:123:a', 2, ':123:', allcaptures=([':123:'], [':123:'], ['123'])), MockLexToken(lineno=2, value=([':123:'], ['123']))),
+    ('TOK3', r'(\|(\d+))+\n', True, True, MockLexToken((5,20), 'start|1|22|333|4444\nend', 2, '|1|22|333|4444\n', allcaptures=(['|1|22|333|4444\n'],['|1|22|333|4444\n'], ['|1', '|22', '|333', '|4444'], ['1', '22', '333', '4444'])), MockLexToken(lineno=3, value=(['|1|22|333|4444\n'], ['|1', '|22', '|333', '|4444'], ['1', '22', '333', '4444']))),
 ])
 def test_get_pattern_func(token, pattern, using_regex, using_cpython, t, expected):
     lexer.using_cpython = using_cpython
-    pattern_func = lexer.get_pattern_func(token, pattern, using_regex)
+    lexer.lex.re = regex if using_regex and using_cpython else re
+    g_span = (0, len(t.value))
+    pattern_func = lexer.get_pattern_func(token, pattern, using_regex, g_span)
     assert pattern_func.__doc__ == pattern
     assert pattern_func.__name__ == token
     t = pattern_func(t)
     assert t == expected
 
 
 def test_get_ignore_func():
```

### Comparing `serl-0.1.0b0/tests/test_main.py` & `serl-0.2.0b0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_parser.py` & `serl-0.2.0b0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_schema.py` & `serl-0.2.0b0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.1.0b0/tests/test_utils.py` & `serl-0.2.0b0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,14 @@
     ('not-valid', 'notvalid'), ('90notvalid.txt', 'notvalidtxt')
 ])
 def test_get_valid_identifier(string, expected):
     actual = utils.get_valid_identifier(string)
     assert actual == expected
 
 @pytest.mark.parametrize('code, expected', [
-    ({'init': ['c1', 'c2'], 'MAIN': ['c3'], 'OTHER': ['c4']}, ('init', 'c1')),
+    ({'init': ['c1', 'c2'], 'MAIN': ['c3'], 'OTHER': ['c4']}, ('init', ['c1', 'c2'])),
     ({'MAIN': ['c2'], 'OTHER': ['c3']}, None),
     ({'MAIN': ['c1'], 'init': ['c2'], 'OTHER': ['c3']}, None)
 ])
 def test_get_main_code(code, expected):
     actual = utils.get_main_code(code,  grammar_map)
     assert actual == expected
```


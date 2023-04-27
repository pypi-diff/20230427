# Comparing `tmp/docx2python-2.6.0.tar.gz` & `tmp/docx2python-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx2python-2.6.0.tar", max compression
+gzip compressed data, was "docx2python-2.6.3.tar", max compression
```

## Comparing `docx2python-2.6.0.tar` & `docx2python-2.6.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      240 2023-01-19 19:29:25.943561 docx2python-2.6.0/docx2python/__init__.py
--rw-r--r--   0        0        0     4945 2023-01-19 19:29:25.944712 docx2python-2.6.0/docx2python/attribute_register.py
--rw-r--r--   0        0        0     5272 2023-01-19 19:29:25.944712 docx2python-2.6.0/docx2python/bullets_and_numbering.py
--rw-r--r--   0        0        0     9246 2023-01-23 22:13:46.338596 docx2python-2.6.0/docx2python/depth_collector.py
--rw-r--r--   0        0        0     6923 2023-01-19 19:29:25.945760 docx2python-2.6.0/docx2python/docx_context.py
--rw-r--r--   0        0        0     8410 2023-01-27 18:14:24.180137 docx2python-2.6.0/docx2python/docx_output.py
--rw-r--r--   0        0        0    16656 2023-01-23 22:13:46.338596 docx2python-2.6.0/docx2python/docx_reader.py
--rw-r--r--   0        0        0    10196 2023-01-23 22:13:46.339594 docx2python-2.6.0/docx2python/docx_text.py
--rw-r--r--   0        0        0     3244 2023-01-19 19:29:25.947556 docx2python-2.6.0/docx2python/forms.py
--rw-r--r--   0        0        0     9725 2023-01-19 19:29:25.947999 docx2python-2.6.0/docx2python/iterators.py
--rw-r--r--   0        0        0     1939 2023-01-23 22:13:46.340597 docx2python-2.6.0/docx2python/main.py
--rw-r--r--   0        0        0     5291 2023-01-19 19:29:25.949121 docx2python-2.6.0/docx2python/merge_runs.py
--rw-r--r--   0        0        0     2857 2023-01-19 19:29:25.949556 docx2python-2.6.0/docx2python/namespace.py
--rw-r--r--   0        0        0     3587 2023-01-19 19:29:25.949556 docx2python-2.6.0/docx2python/numbering_formats.py
--rw-r--r--   0        0        0        0 2023-02-03 22:08:10.380704 docx2python-2.6.0/docx2python/py.typed
--rw-r--r--   0        0        0    10053 2023-01-23 22:13:46.340597 docx2python-2.6.0/docx2python/text_runs.py
--rw-r--r--   0        0        0     3060 2023-01-23 17:50:37.267372 docx2python-2.6.0/docx2python/utilities.py
--rw-r--r--   0        0        0     1097 2023-01-19 19:29:25.942725 docx2python-2.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1486 2023-02-03 22:08:10.380704 docx2python-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    13515 2023-01-23 22:13:46.337643 docx2python-2.6.0/README.md
--rw-r--r--   0        0        0    14214 1970-01-01 00:00:00.000000 docx2python-2.6.0/setup.py
--rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/__init__.py
+-rw-r--r--   0        0        0     4945 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/attribute_register.py
+-rw-r--r--   0        0        0     5272 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/bullets_and_numbering.py
+-rw-r--r--   0        0        0     9246 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/depth_collector.py
+-rw-r--r--   0        0        0     6857 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_context.py
+-rw-r--r--   0        0        0     8410 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_output.py
+-rw-r--r--   0        0        0    16656 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_reader.py
+-rw-r--r--   0        0        0    10196 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_text.py
+-rw-r--r--   0        0        0     3244 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/forms.py
+-rw-r--r--   0        0        0     9725 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/iterators.py
+-rw-r--r--   0        0        0     1939 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/main.py
+-rw-r--r--   0        0        0     5291 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/merge_runs.py
+-rw-r--r--   0        0        0     2857 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/namespace.py
+-rw-r--r--   0        0        0     3587 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/numbering_formats.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/py.typed
+-rw-r--r--   0        0        0    10053 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/text_runs.py
+-rw-r--r--   0        0        0     4525 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/utilities.py
+-rw-r--r--   0        0        0     1097 2023-04-27 18:33:43.953747 docx2python-2.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     1486 2023-04-27 18:33:43.969370 docx2python-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0    13515 2023-04-27 18:33:43.953747 docx2python-2.6.3/README.md
+-rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.6.3/PKG-INFO
```

### Comparing `docx2python-2.6.0/docx2python/attribute_register.py` & `docx2python-2.6.3/docx2python/attribute_register.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/bullets_and_numbering.py` & `docx2python-2.6.3/docx2python/bullets_and_numbering.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/depth_collector.py` & `docx2python-2.6.3/docx2python/depth_collector.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/docx_context.py` & `docx2python-2.6.3/docx2python/docx_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,16 @@
         for lvl in abstractNum.findall(qn("w:lvl")):
             numFmt = lvl.find(qn("w:numFmt"))
             if numFmt is not None:
                 abstractNumId2numFmts[id_].append(str(numFmt.attrib[qn("w:val")]))
 
     numId2numFmts: dict[str, list[str]] = {}
     num: EtreeElement
-    for num in (x for x in numFmts_root.findall(qn("w:num")) if x is not None):
+    for num in (x for x in numFmts_root.findall(qn("w:num"))):
         numId = num.attrib[qn("w:numId")]
-        if numId is None:
-            continue
         abstractNumId = num.find(qn("w:abstractNumId"))
         if abstractNumId is None:
             continue
         abstractNumIdval = abstractNumId.attrib.get(qn("w:val"))
         numId2numFmts[str(numId)] = abstractNumId2numFmts[str(abstractNumIdval)]
 
     return numId2numFmts
```

### Comparing `docx2python-2.6.0/docx2python/docx_output.py` & `docx2python-2.6.3/docx2python/docx_output.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/docx_reader.py` & `docx2python-2.6.3/docx2python/docx_reader.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/docx_text.py` & `docx2python-2.6.3/docx2python/docx_text.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/forms.py` & `docx2python-2.6.3/docx2python/forms.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/iterators.py` & `docx2python-2.6.3/docx2python/iterators.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/main.py` & `docx2python-2.6.3/docx2python/main.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/merge_runs.py` & `docx2python-2.6.3/docx2python/merge_runs.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/namespace.py` & `docx2python-2.6.3/docx2python/namespace.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/numbering_formats.py` & `docx2python-2.6.3/docx2python/numbering_formats.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/docx2python/text_runs.py` & `docx2python-2.6.3/docx2python/text_runs.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/LICENSE.txt` & `docx2python-2.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/pyproject.toml` & `docx2python-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docx2python"
-version = "2.6.0"
+version = "2.6.3"
 description = "Extract content from docx files"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,15 +14,15 @@
 pytest = "^7.2.0"
 types-lxml = "^2022.11.8"
 commitizen = "^2.39.1"
 pre-commit = "^3.0.4"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.6.0"
+version = "2.7.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `docx2python-2.6.0/README.md` & `docx2python-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.0/setup.py` & `docx2python-2.6.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,889 +1,859 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2764 6f63 7832 7079 7468 6f6e   \.['docx2python
-00000050: 275d 0a0a 7061 636b 6167 655f 6461 7461  ']..package_data
-00000060: 203d 205c 0a7b 2727 3a20 5b27 2a27 5d7d   = \.{'': ['*']}
-00000070: 0a0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000080: 6573 203d 205c 0a5b 276c 786d 6c3e 3d34  es = \.['lxml>=4
-00000090: 2e39 2e32 2c3c 352e 302e 3027 5d0a 0a73  .9.2,<5.0.0']..s
-000000a0: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-000000b0: 2020 2020 276e 616d 6527 3a20 2764 6f63      'name': 'doc
-000000c0: 7832 7079 7468 6f6e 272c 0a20 2020 2027  x2python',.    '
-000000d0: 7665 7273 696f 6e27 3a20 2732 2e36 2e30  version': '2.6.0
-000000e0: 272c 0a20 2020 2027 6465 7363 7269 7074  ',.    'descript
-000000f0: 696f 6e27 3a20 2745 7874 7261 6374 2063  ion': 'Extract c
-00000100: 6f6e 7465 6e74 2066 726f 6d20 646f 6378  ontent from docx
-00000110: 2066 696c 6573 272c 0a20 2020 2027 6c6f   files',.    'lo
-00000120: 6e67 5f64 6573 6372 6970 7469 6f6e 273a  ng_description':
-00000130: 2027 2320 646f 6378 3270 7974 686f 6e5c   '# docx2python\
-00000140: 6e5c 6e45 7874 7261 6374 2064 6f63 7820  n\nExtract docx 
-00000150: 6865 6164 6572 732c 2066 6f6f 7465 7273  headers, footers
-00000160: 2c20 7465 7874 2c20 666f 6f74 6e6f 7465  , text, footnote
-00000170: 732c 2065 6e64 6e6f 7465 732c 2070 726f  s, endnotes, pro
-00000180: 7065 7274 6965 732c 2061 6e64 2069 6d61  perties, and ima
-00000190: 6765 7320 746f 2061 2050 7974 686f 6e20  ges to a Python 
-000001a0: 6f62 6a65 6374 2e5c 6e5c 6e60 5245 4144  object.\n\n`READ
-000001b0: 4d45 5f44 4f43 585f 4649 4c45 5f53 5452  ME_DOCX_FILE_STR
-000001c0: 5543 5455 5245 2e6d 6460 206d 6179 2068  UCTURE.md` may h
-000001d0: 656c 7020 6966 2079 6f75 5c27 6420 6c69  elp if you\'d li
-000001e0: 6b65 2074 6f20 6578 7465 6e64 2064 6f63  ke to extend doc
-000001f0: 7832 7079 7468 6f6e 2e5c 6e5c 6e46 6f72  x2python.\n\nFor
-00000200: 2061 2073 756d 6d61 7279 206f 6620 7768   a summary of wh
-00000210: 6174 5c27 7320 6e65 7720 696e 2064 6f63  at\'s new in doc
-00000220: 7832 7079 7468 6f6e 2032 2c20 7363 726f  x2python 2, scro
-00000230: 6c6c 2064 6f77 6e20 746f 202a 2a4e 6577  ll down to **New
-00000240: 2069 6e20 646f 6378 3270 7974 686f 6e20   in docx2python 
-00000250: 5665 7273 696f 6e20 322a 2a5c 6e5c 6e54  Version 2**\n\nT
-00000260: 6865 2063 6f64 6520 6973 2061 6e20 6578  he code is an ex
-00000270: 7061 6e73 696f 6e2f 636f 6e74 7261 6374  pansion/contract
-00000280: 696f 6e20 6f66 205b 7079 7468 6f6e 2d64  ion of [python-d
-00000290: 6f63 7832 7478 745d 2868 7474 7073 3a2f  ocx2txt](https:/
-000002a0: 2f67 6974 6875 622e 636f 6d2f 616e 6b75  /github.com/anku
-000002b0: 7368 7368 6168 3839 2f70 7974 686f 6e2d  shshah89/python-
-000002c0: 646f 6378 3274 7874 2920 2843 6f70 7972  docx2txt) (Copyr
-000002d0: 6967 6874 2028 6329 2032 3031 3520 416e  ight (c) 2015 An
-000002e0: 6b75 7368 2053 6861 6829 2e20 5468 6520  kush Shah). The 
-000002f0: 6f72 6967 696e 616c 2063 6f64 6520 6973  original code is
-00000300: 206d 6f73 746c 7920 676f 6e65 2c20 6275   mostly gone, bu
-00000310: 7420 736f 6d65 206f 6620 7468 6520 626f  t some of the bo
-00000320: 6e65 7320 6d61 7920 7374 696c 6c20 6265  nes may still be
-00000330: 2068 6572 652e 5c6e 5c6e 5f5f 7368 6172   here.\n\n__shar
-00000340: 6564 2066 6561 7475 7265 735f 5f3a 5c6e  ed features__:\n
-00000350: 2a20 6578 7472 6163 7473 2074 6578 7420  * extracts text 
-00000360: 6672 6f6d 2064 6f63 7820 6669 6c65 735c  from docx files\
-00000370: 6e2a 2065 7874 7261 6374 7320 696d 6167  n* extracts imag
-00000380: 6573 2066 726f 6d20 646f 6378 2066 696c  es from docx fil
-00000390: 6573 5c6e 5c6e 5f5f 6164 6469 7469 6f6e  es\n\n__addition
-000003a0: 733a 5f5f 5c6e 2a20 6578 7472 6163 7473  s:__\n* extracts
-000003b0: 2066 6f6f 746e 6f74 6573 2061 6e64 2065   footnotes and e
-000003c0: 6e64 6e6f 7465 735c 6e2a 2063 6f6e 7665  ndnotes\n* conve
-000003d0: 7274 7320 6275 6c6c 6574 7320 616e 6420  rts bullets and 
-000003e0: 6e75 6d62 6572 6564 206c 6973 7473 2074  numbered lists t
-000003f0: 6f20 6173 6369 6920 7769 7468 2069 6e64  o ascii with ind
-00000400: 656e 7461 7469 6f6e 5c6e 2a20 636f 6e76  entation\n* conv
-00000410: 6572 7473 2068 7970 6572 6c69 6e6b 7320  erts hyperlinks 
-00000420: 746f 2060 603c 6120 6872 6566 3d22 6874  to ``<a href="ht
-00000430: 7470 3a2f 2e2e 2e22 3e6c 696e 6b20 7465  tp:/...">link te
-00000440: 7874 3c2f 613e 6060 5c6e 2a20 7265 7461  xt</a>``\n* reta
-00000450: 696e 7320 736f 6d65 2073 7472 7563 7475  ins some structu
-00000460: 7265 206f 6620 7468 6520 6f72 6967 696e  re of the origin
-00000470: 616c 2066 696c 6520 286d 6f72 6520 6265  al file (more be
-00000480: 6c6f 7729 5c6e 2a20 6578 7472 6163 7473  low)\n* extracts
-00000490: 2064 6f63 756d 656e 7420 7072 6f70 6572   document proper
-000004a0: 7469 6573 2028 6372 6561 746f 722c 206c  ties (creator, l
-000004b0: 6173 744d 6f64 6966 6965 6442 792c 2065  astModifiedBy, e
-000004c0: 7463 2e29 5c6e 2a20 696e 7365 7274 7320  tc.)\n* inserts 
-000004d0: 696d 6167 6520 706c 6163 6568 6f6c 6465  image placeholde
-000004e0: 7273 2069 6e20 7465 7874 2028 6060 5c27  rs in text (``\'
-000004f0: 2d2d 2d2d 696d 6167 6531 2e6a 7067 2d2d  ----image1.jpg--
-00000500: 2d2d 5c27 6060 295c 6e2a 2069 6e73 6572  --\'``)\n* inser
-00000510: 7473 2070 6c61 696e 2074 6578 7420 666f  ts plain text fo
-00000520: 6f74 6e6f 7465 2061 6e64 2065 6e64 6e6f  otnote and endno
-00000530: 7465 2072 6566 6572 656e 6365 7320 696e  te references in
-00000540: 2074 6578 7420 2860 605c 272d 2d2d 2d66   text (``\'----f
-00000550: 6f6f 746e 6f74 6531 2d2d 2d2d 5c27 6060  ootnote1----\'``
-00000560: 295c 6e2a 2028 6f70 7469 6f6e 616c 6c79  )\n* (optionally
-00000570: 2920 7265 7461 696e 7320 666f 6e74 2073  ) retains font s
-00000580: 697a 652c 2066 6f6e 7420 636f 6c6f 722c  ize, font color,
-00000590: 2062 6f6c 642c 2069 7461 6c69 6373 2c20   bold, italics, 
-000005a0: 616e 6420 756e 6465 7273 636f 7265 2061  and underscore a
-000005b0: 7320 6874 6d6c 5c6e 2a20 6578 7472 6163  s html\n* extrac
-000005c0: 7420 6d61 7468 2065 7175 6174 696f 6e73  t math equations
-000005d0: 5c6e 2a20 6578 7472 6163 7420 7573 6572  \n* extract user
-000005e0: 2073 656c 6563 7469 6f6e 7320 6672 6f6d   selections from
-000005f0: 2063 6865 636b 626f 7865 7320 616e 6420   checkboxes and 
-00000600: 6472 6f70 646f 776e 206d 656e 7573 5c6e  dropdown menus\n
-00000610: 5c6e 5f5f 7375 6274 7261 6374 696f 6e73  \n__subtractions
-00000620: 3a5f 5f5c 6e2a 206e 6f20 636f 6d6d 616e  :__\n* no comman
-00000630: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
-00000640: 5c6e 2a20 7769 6c6c 206f 6e6c 7920 776f  \n* will only wo
-00000650: 726b 2077 6974 6820 5079 7468 6f6e 2033  rk with Python 3
-00000660: 2e38 2b5c 6e5c 6e5c 6e23 2320 496e 7374  .8+\n\n\n## Inst
-00000670: 616c 6c61 7469 6f6e 5c6e 6060 6062 6173  allation\n```bas
-00000680: 685c 6e70 6970 2069 6e73 7461 6c6c 2064  h\npip install d
-00000690: 6f63 7832 7079 7468 6f6e 5c6e 6060 605c  ocx2python\n```\
-000006a0: 6e5c 6e23 2320 5573 655c 6e5c 6e60 6060  n\n## Use\n\n```
-000006b0: 2070 7974 686f 6e5c 6e66 726f 6d20 646f   python\nfrom do
-000006c0: 6378 3270 7974 686f 6e20 696d 706f 7274  cx2python import
-000006d0: 2064 6f63 7832 7079 7468 6f6e 5c6e 5c6e   docx2python\n\n
-000006e0: 2320 6578 7472 6163 7420 646f 6378 2063  # extract docx c
-000006f0: 6f6e 7465 6e74 5c6e 7769 7468 2064 6f63  ontent\nwith doc
-00000700: 7832 7079 7468 6f6e 285c 2770 6174 682f  x2python(\'path/
-00000710: 746f 2f66 696c 652e 646f 6378 5c27 2920  to/file.docx\') 
-00000720: 6173 2064 6f63 785f 636f 6e74 656e 743a  as docx_content:
-00000730: 5c6e 2020 2020 7072 696e 7428 646f 6378  \n    print(docx
-00000740: 5f63 6f6e 7465 6e74 2e74 6578 7429 5c6e  _content.text)\n
-00000750: 5c6e 646f 6378 5f63 6f6e 7465 6e74 203d  \ndocx_content =
-00000760: 2064 6f63 7832 7079 7468 6f6e 285c 2770   docx2python(\'p
-00000770: 6174 682f 746f 2f66 696c 652e 646f 6378  ath/to/file.docx
-00000780: 5c27 295c 6e70 7269 6e74 2864 6f63 785f  \')\nprint(docx_
-00000790: 636f 6e74 656e 742e 7465 7874 295c 6e64  content.text)\nd
-000007a0: 6f63 785f 636f 6e74 656e 742e 636c 6f73  ocx_content.clos
-000007b0: 6528 295c 6e5c 6e23 2065 7874 7261 6374  e()\n\n# extract
-000007c0: 2064 6f63 7820 636f 6e74 656e 742c 2077   docx content, w
-000007d0: 7269 7465 2069 6d61 6765 7320 746f 2069  rite images to i
-000007e0: 6d61 6765 5f64 6972 6563 746f 7279 5c6e  mage_directory\n
-000007f0: 7769 7468 2064 6f63 7832 7079 7468 6f6e  with docx2python
-00000800: 285c 2770 6174 682f 746f 2f66 696c 652e  (\'path/to/file.
-00000810: 646f 6378 5c27 2c20 5c27 7061 7468 2f74  docx\', \'path/t
-00000820: 6f2f 696d 6167 655f 6469 7265 6374 6f72  o/image_director
-00000830: 795c 2729 2061 7320 646f 6378 5f63 6f6e  y\') as docx_con
-00000840: 7465 6e74 3a5c 6e20 2020 2070 7269 6e74  tent:\n    print
-00000850: 2864 6f63 785f 636f 6e74 656e 742e 7465  (docx_content.te
-00000860: 7874 295c 6e5c 6e23 2065 7874 7261 6374  xt)\n\n# extract
-00000870: 2064 6f63 7820 636f 6e74 656e 7420 7769   docx content wi
-00000880: 7468 2062 6173 6963 2066 6f6e 7420 7374  th basic font st
-00000890: 796c 6573 2063 6f6e 7665 7274 6564 2074  yles converted t
-000008a0: 6f20 6874 6d6c 5c6e 7769 7468 2064 6f63  o html\nwith doc
-000008b0: 7832 7079 7468 6f6e 285c 2770 6174 682f  x2python(\'path/
-000008c0: 746f 2f66 696c 652e 646f 6378 5c27 2c20  to/file.docx\', 
-000008d0: 6874 6d6c 3d54 7275 6529 2061 7320 646f  html=True) as do
-000008e0: 6378 5f63 6f6e 7465 6e74 3a5c 6e20 2020  cx_content:\n   
-000008f0: 2070 7269 6e74 2864 6f63 785f 636f 6e74   print(docx_cont
-00000900: 656e 742e 7465 7874 295c 6e60 6060 5c6e  ent.text)\n```\n
-00000910: 5c6e 6064 6f63 7832 7079 7468 6f6e 6020  \n`docx2python` 
-00000920: 6f70 656e 7320 6120 7a69 7066 696c 6520  opens a zipfile 
-00000930: 6f62 6a65 6374 2061 6e64 2028 6c61 7a69  object and (lazi
-00000940: 6c79 2920 7265 6164 7320 6974 2e20 5573  ly) reads it. Us
-00000950: 6520 636f 6e74 6578 7420 6d61 6e61 6765  e context manage
-00000960: 6d65 6e74 2028 6077 6974 6820 2e2e 2e20  ment (`with ... 
-00000970: 6173 6029 2074 6f20 636c 6f73 6520 7468  as`) to close th
-00000980: 6973 207a 6970 6669 6c65 206f 626a 6563  is zipfile objec
-00000990: 7420 6f72 2065 7870 6c69 6369 746c 7920  t or explicitly 
-000009a0: 636c 6f73 6520 7769 7468 2060 646f 6378  close with `docx
-000009b0: 5f63 6f6e 7465 6e74 2e63 6c6f 7365 2829  _content.close()
-000009c0: 602e 5c6e 5c6e 4e6f 7465 206f 6e20 6874  `.\n\nNote on ht
-000009d0: 6d6c 2066 6561 7475 7265 3a5c 6e2a 2073  ml feature:\n* s
-000009e0: 7570 706f 7274 7320 6060 3c69 3e60 6069  upports ``<i>``i
-000009f0: 7461 6c69 632c 2060 603c 623e 6060 626f  talic, ``<b>``bo
-00000a00: 6c64 2c20 6060 3c75 3e60 6075 6e64 6572  ld, ``<u>``under
-00000a10: 6c69 6e65 2c20 6060 3c73 3e60 6073 7472  line, ``<s>``str
-00000a20: 696b 652c 2060 603c 7375 703e 6060 7375  ike, ``<sup>``su
-00000a30: 7065 7273 6372 6970 742c 2060 603c 7375  perscript, ``<su
-00000a40: 623e 6060 7375 6273 6372 6970 742c 2060  b>``subscript, `
-00000a50: 603c 7370 616e 2073 7479 6c65 3d22 666f  `<span style="fo
-00000a60: 6e74 2d76 6172 6961 6e74 3a20 736d 616c  nt-variant: smal
-00000a70: 6c2d 6361 7073 223e 6060 736d 616c 6c20  l-caps">``small 
-00000a80: 6361 7073 2c20 6060 3c73 7061 6e20 7374  caps, ``<span st
-00000a90: 796c 653d 2274 6578 742d 7472 616e 7366  yle="text-transf
-00000aa0: 6f72 6d3a 7570 7065 7263 6173 6522 3e60  orm:uppercase">`
-00000ab0: 6061 6c6c 2063 6170 732c 2060 603c 7370  `all caps, ``<sp
-00000ac0: 616e 2073 7479 6c65 3d22 6261 636b 6772  an style="backgr
-00000ad0: 6f75 6e64 2d63 6f6c 6f72 3a20 7965 6c6c  ound-color: yell
-00000ae0: 6f77 223e 6060 6869 6768 6c69 6768 7465  ow">``highlighte
-00000af0: 642c 2060 603c 7370 616e 2073 7479 6c65  d, ``<span style
-00000b00: 3d22 666f 6e74 2d73 697a 653a 3332 223e  ="font-size:32">
-00000b10: 6060 666f 6e74 2073 697a 652c 2060 603c  ``font size, ``<
-00000b20: 7370 616e 2073 7479 6c65 3d22 636f 6c6f  span style="colo
-00000b30: 723a 2366 6630 3030 3022 3e60 6063 6f6c  r:#ff0000">``col
-00000b40: 6f72 6564 2074 6578 742e 5c6e 2a20 6879  ored text.\n* hy
-00000b50: 7065 726c 696e 6b73 2077 696c 6c20 616c  perlinks will al
-00000b60: 7761 7973 2062 6520 6578 706f 7274 6564  ways be exported
-00000b70: 2061 7320 6874 6d6c 2028 6060 3c61 2068   as html (``<a h
-00000b80: 7265 663d 2268 7474 703a 2f2e 2e2e 223e  ref="http:/...">
-00000b90: 6c69 6e6b 2074 6578 743c 2f61 3e60 6029  link text</a>``)
-00000ba0: 2c20 6576 656e 2069 6620 6060 6874 6d6c  , even if ``html
-00000bb0: 3d46 616c 7365 6060 2c20 6265 6361 7573  =False``, becaus
-00000bc0: 6520 4920 636f 756c 646e 5c27 7420 7468  e I couldn\'t th
-00000bd0: 696e 6b20 6f66 2061 206d 6f72 6520 6361  ink of a more ca
-00000be0: 6e6f 6e69 6361 6c20 7265 7072 6573 656e  nonical represen
-00000bf0: 7461 7469 6f6e 2e5c 6e2a 2065 7665 7279  tation.\n* every
-00000c00: 2074 6167 206f 7065 6e20 696e 2061 2070   tag open in a p
-00000c10: 6172 6167 7261 7068 2077 696c 6c20 6265  aragraph will be
-00000c20: 2063 6c6f 7365 6420 696e 2074 6861 7420   closed in that 
-00000c30: 7061 7261 6772 6170 6820 2861 6e64 2c20  paragraph (and, 
-00000c40: 7768 6572 6520 6170 7072 6f70 7269 6174  where appropriat
-00000c50: 652c 2072 656f 7065 6e65 6420 696e 2074  e, reopened in t
-00000c60: 6865 206e 6578 7420 7061 7261 6772 6170  he next paragrap
-00000c70: 6829 2e20 4966 2074 776f 2073 7562 7365  h). If two subse
-00000c80: 7175 656e 6374 2070 6172 6167 7261 7068  quenct paragraph
-00000c90: 7320 6172 6520 626f 6c64 2c20 7468 6579  s are bold, they
-00000ca0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-00000cb0: 6420 6173 2060 3c62 3e70 6172 6167 7261  d as `<b>paragra
-00000cc0: 7068 2061 3c2f 623e 602c 2060 3c62 3e70  ph a</b>`, `<b>p
-00000cd0: 6172 6167 7261 7068 2062 3c2f 623e 602e  aragraph b</b>`.
-00000ce0: 2054 6869 7320 6973 2069 6e74 656e 7469   This is intenti
-00000cf0: 6f6e 616c 2074 6f20 6d61 6b65 2020 6561  onal to make  ea
-00000d00: 6368 2070 6172 6167 7261 7068 2069 7473  ch paragraph its
-00000d10: 206f 776e 2065 6e74 6974 792e 5c6e 2a20   own entity.\n* 
-00000d20: 6966 2079 6f75 2073 7065 6369 6679 2060  if you specify `
-00000d30: 6874 6d6c 3d54 7275 6560 2c20 6026 602c  html=True`, `&`,
-00000d40: 2060 3e60 2061 6e64 2060 3c60 2069 6e20   `>` and `<` in 
-00000d50: 796f 7572 2064 6f63 7820 7465 7874 2077  your docx text w
-00000d60: 696c 6c20 6265 2065 6e63 6f64 6564 2061  ill be encoded a
-00000d70: 7320 6026 616d 7060 2c20 6026 6774 3b60  s `&amp`, `&gt;`
-00000d80: 2061 6e64 2060 266c 743b 605c 6e5c 6e23   and `&lt;`\n\n#
-00000d90: 2320 5265 7475 726e 2056 616c 7565 5c6e  # Return Value\n
-00000da0: 5c6e 4675 6e63 7469 6f6e 2060 646f 6378  \nFunction `docx
-00000db0: 3270 7974 686f 6e60 2072 6574 7572 6e73  2python` returns
-00000dc0: 2061 2044 6f63 7843 6f6e 7465 6e74 2069   a DocxContent i
-00000dd0: 6e73 7461 6e63 6520 7769 7468 2073 6576  nstance with sev
-00000de0: 6572 616c 2061 7474 7269 6275 7465 732e  eral attributes.
-00000df0: 5c6e 5c6e 5f5f 6865 6164 6572 5f5f 202d  \n\n__header__ -
-00000e00: 2063 6f6e 7465 6e74 7320 6f66 2074 6865   contents of the
-00000e10: 2064 6f63 7820 6865 6164 6572 7320 696e   docx headers in
-00000e20: 2074 6865 2072 6574 7572 6e20 666f 726d   the return form
-00000e30: 6174 2064 6573 6372 6962 6564 2068 6572  at described her
-00000e40: 6569 6e5c 6e5c 6e5f 5f66 6f6f 7465 725f  ein\n\n__footer_
-00000e50: 5f20 2d20 636f 6e74 656e 7473 206f 6620  _ - contents of 
-00000e60: 7468 6520 646f 6378 2066 6f6f 7465 7273  the docx footers
-00000e70: 2069 6e20 7468 6520 7265 7475 726e 2066   in the return f
-00000e80: 6f72 6d61 7420 6465 7363 7269 6265 6420  ormat described 
-00000e90: 6865 7265 696e 5c6e 5c6e 5f5f 626f 6479  herein\n\n__body
-00000ea0: 5f5f 202d 2063 6f6e 7465 6e74 7320 6f66  __ - contents of
-00000eb0: 2074 6865 2064 6f63 7820 696e 2074 6865   the docx in the
-00000ec0: 2072 6574 7572 6e20 666f 726d 6174 2064   return format d
-00000ed0: 6573 6372 6962 6564 2068 6572 6569 6e5c  escribed herein\
-00000ee0: 6e5c 6e5f 5f66 6f6f 746e 6f74 6573 5f5f  n\n__footnotes__
-00000ef0: 202d 2063 6f6e 7465 6e74 7320 6f66 2074   - contents of t
-00000f00: 6865 2064 6f63 7820 696e 2074 6865 2072  he docx in the r
-00000f10: 6574 7572 6e20 666f 726d 6174 2064 6573  eturn format des
-00000f20: 6372 6962 6564 2068 6572 6569 6e5c 6e5c  cribed herein\n\
-00000f30: 6e5f 5f65 6e64 6e6f 7465 735f 5f20 2d20  n__endnotes__ - 
-00000f40: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
-00000f50: 646f 6378 2069 6e20 7468 6520 7265 7475  docx in the retu
-00000f60: 726e 2066 6f72 6d61 7420 6465 7363 7269  rn format descri
-00000f70: 6265 6420 6865 7265 696e 5c6e 5c6e 5f5f  bed herein\n\n__
-00000f80: 646f 6375 6d65 6e74 5f5f 202d 2068 6561  document__ - hea
-00000f90: 6465 7220 202b 2062 6f64 7920 2b20 666f  der  + body + fo
-00000fa0: 6f74 6572 2028 7265 6164 206f 6e6c 7929  oter (read only)
-00000fb0: 5c6e 5c6e 5f5f 7465 7874 5f5f 202d 2061  \n\n__text__ - a
-00000fc0: 6c6c 2064 6f63 7820 7465 7874 2061 7320  ll docx text as 
-00000fd0: 6f6e 6520 7374 7269 6e67 2c20 7369 6d69  one string, simi
-00000fe0: 6c61 7220 746f 2077 6861 7420 796f 755c  lar to what you\
-00000ff0: 2764 2067 6574 2066 726f 6d20 6070 7974  'd get from `pyt
-00001000: 686f 6e2d 646f 6378 3274 7874 605c 6e5c  hon-docx2txt`\n\
-00001010: 6e5f 5f70 726f 7065 7274 6965 735f 5f20  n__properties__ 
-00001020: 2d20 646f 6378 2070 726f 7065 7274 7920  - docx property 
-00001030: 6e61 6d65 7320 6d61 7070 6564 2074 6f20  names mapped to 
-00001040: 7661 6c75 6573 2028 652e 672e 2c20 607b  values (e.g., `{
-00001050: 226c 6173 744d 6f64 6966 6965 6442 7922  "lastModifiedBy"
-00001060: 3a20 2253 6861 7920 4869 6c6c 227d 6029  : "Shay Hill"}`)
-00001070: 5c6e 5c6e 5f5f 696d 6167 6573 5f5f 202d  \n\n__images__ -
-00001080: 2069 6d61 6765 206e 616d 6573 206d 6170   image names map
-00001090: 7065 6420 746f 2069 6d61 6765 7320 696e  ped to images in
-000010a0: 2062 696e 6172 7920 666f 726d 6174 2e20   binary format. 
-000010b0: 5772 6974 6520 746f 2066 696c 6573 7973  Write to filesys
-000010c0: 7465 6d20 7769 7468 5c6e 5c6e 6060 605c  tem with\n\n```\
-000010d0: 6e66 6f72 206e 616d 652c 2069 6d61 6765  nfor name, image
-000010e0: 2069 6e20 7265 7375 6c74 2e69 6d61 6765   in result.image
-000010f0: 732e 6974 656d 7328 293a 5c6e 2020 2020  s.items():\n    
-00001100: 7769 7468 206f 7065 6e28 6e61 6d65 2c20  with open(name, 
-00001110: 5c27 7762 5c27 2920 6173 2069 6d61 6765  \'wb\') as image
-00001120: 5f64 6573 7469 6e61 7469 6f6e 3a5c 6e20  _destination:\n 
-00001130: 2020 2020 2020 2077 7269 7465 2869 6d61         write(ima
-00001140: 6765 5f64 6573 7469 6e61 7469 6f6e 2c20  ge_destination, 
-00001150: 696d 6167 6529 5c6e 5c6e 2320 6f72 5c6e  image)\n\n# or\n
-00001160: 5c6e 7769 7468 2064 6f63 7832 7079 7468  \nwith docx2pyth
-00001170: 6f6e 285c 2770 6174 682f 746f 2f66 696c  on(\'path/to/fil
-00001180: 652e 646f 6378 5c27 2c20 5c27 7061 7468  e.docx\', \'path
-00001190: 2f74 6f2f 696d 6167 652f 6469 7265 6374  /to/image/direct
-000011a0: 6f72 795c 2729 2061 7320 646f 6378 5f63  ory\') as docx_c
-000011b0: 6f6e 7465 6e74 3a5c 6e20 2020 202e 2e2e  ontent:\n    ...
-000011c0: 5c6e 5c6e 2320 6f72 5c6e 5c6e 7769 7468  \n\n# or\n\nwith
-000011d0: 2064 6f63 7832 7079 7468 6f6e 285c 2770   docx2python(\'p
-000011e0: 6174 682f 746f 2f66 696c 652e 646f 6378  ath/to/file.docx
-000011f0: 5c27 2920 6173 2064 6f63 785f 636f 6e74  \') as docx_cont
-00001200: 656e 743a 5c6e 2020 2020 646f 6378 5f63  ent:\n    docx_c
-00001210: 6f6e 7465 6e74 2e73 6176 655f 696d 6167  ontent.save_imag
-00001220: 6573 285c 2770 6174 682f 746f 2f69 6d61  es(\'path/to/ima
-00001230: 6765 2f64 6972 6563 746f 7279 5c27 295c  ge/directory\')\
-00001240: 6e5c 6e60 6060 5c6e 5c6e 5f5f 646f 6378  n\n```\n\n__docx
-00001250: 5f72 6561 6465 725f 5f20 2d20 6120 446f  _reader__ - a Do
-00001260: 6378 5265 6164 6572 2028 7365 6520 6064  cxReader (see `d
-00001270: 6f63 785f 7265 6164 6572 2e70 7960 2920  ocx_reader.py`) 
-00001280: 696e 7374 616e 6365 2077 6974 6820 7365  instance with se
-00001290: 7665 7261 6c20 6d65 7468 6f64 7320 666f  veral methods fo
-000012a0: 7220 6578 7472 6163 7469 6e67 2078 6d6c  r extracting xml
-000012b0: 2070 6f72 7469 6f6e 732e 5c6e 5c6e 5c6e   portions.\n\n\n
-000012c0: 2323 2041 7267 756d 656e 7473 5c6e 5c6e  ## Arguments\n\n
-000012d0: 2020 2020 6465 6620 646f 6378 3270 7974      def docx2pyt
-000012e0: 686f 6e28 5c6e 2020 2020 2020 2020 646f  hon(\n        do
-000012f0: 6378 5f66 696c 656e 616d 653a 2073 7472  cx_filename: str
-00001300: 207c 2050 6174 6820 7c20 4279 7465 7349   | Path | BytesI
-00001310: 4f2c 5c6e 2020 2020 2020 2020 696d 6167  O,\n        imag
-00001320: 655f 666f 6c64 6572 3a20 7374 7220 7c20  e_folder: str | 
-00001330: 4e6f 6e65 203d 204e 6f6e 652c 5c6e 2020  None = None,\n  
-00001340: 2020 2020 2020 6874 6d6c 3a20 626f 6f6c        html: bool
-00001350: 203d 2046 616c 7365 2c5c 6e20 2020 2020   = False,\n     
-00001360: 2020 2070 6172 6167 7261 7068 5f73 7479     paragraph_sty
-00001370: 6c65 733a 2062 6f6f 6c20 3d20 4661 6c73  les: bool = Fals
-00001380: 652c 5c6e 2020 2020 2020 2020 6578 7472  e,\n        extr
-00001390: 6163 745f 696d 6167 653a 2062 6f6f 6c20  act_image: bool 
-000013a0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 5c6e  | None = None,\n
-000013b0: 2020 2020 2020 2020 6475 706c 6963 6174          duplicat
-000013c0: 655f 6d65 7267 6564 5f63 656c 6c73 3a20  e_merged_cells: 
-000013d0: 626f 6f6c 203d 2046 616c 7365 5c6e 2020  bool = False\n  
-000013e0: 2020 2920 2d3e 2044 6f63 7843 6f6e 7465    ) -> DocxConte
-000013f0: 6e74 3a5c 6e20 2020 2020 2020 2022 2222  nt:\n        """
-00001400: 5c6e 2020 2020 2020 2020 556e 7a69 7020  \n        Unzip 
-00001410: 6120 646f 6378 2066 696c 6520 616e 6420  a docx file and 
-00001420: 6578 7472 6163 7420 636f 6e74 656e 7473  extract contents
-00001430: 2e5c 6e5c 6e20 2020 2020 2020 203a 7061  .\n\n        :pa
-00001440: 7261 6d20 646f 6378 5f66 696c 656e 616d  ram docx_filenam
-00001450: 653a 2070 6174 6820 746f 2061 2064 6f63  e: path to a doc
-00001460: 7820 6669 6c65 5c6e 2020 2020 2020 2020  x file\n        
-00001470: 3a70 6172 616d 2069 6d61 6765 5f66 6f6c  :param image_fol
-00001480: 6465 723a 206f 7074 696f 6e61 6c6c 7920  der: optionally 
-00001490: 7370 6563 6966 7920 616e 2069 6d61 6765  specify an image
-000014a0: 2066 6f6c 6465 725c 6e20 2020 2020 2020   folder\n       
-000014b0: 2020 2020 2028 696d 6167 6573 2069 6e20       (images in 
-000014c0: 646f 6378 2077 696c 6c20 6265 2063 6f70  docx will be cop
-000014d0: 6965 6420 746f 2074 6869 7320 666f 6c64  ied to this fold
-000014e0: 6572 295c 6e20 2020 2020 2020 203a 7061  er)\n        :pa
-000014f0: 7261 6d20 6874 6d6c 3a20 626f 6f6c 2c20  ram html: bool, 
-00001500: 6578 7472 6163 7420 736f 6d65 2066 6f72  extract some for
-00001510: 6d61 7474 696e 6720 6173 2068 746d 6c5c  matting as html\
-00001520: 6e20 2020 2020 2020 203a 7061 7261 6d20  n        :param 
-00001530: 7061 7261 6772 6170 685f 7374 796c 6573  paragraph_styles
-00001540: 3a20 7072 6570 656e 6420 7468 6520 7061  : prepend the pa
-00001550: 7261 6772 6170 6873 2073 7479 6c65 2028  ragraphs style (
-00001560: 6966 2061 6e79 2c20 656c 7365 2022 2229  if any, else "")
-00001570: 2074 6f20 6561 6368 5c6e 2020 2020 2020   to each\n      
-00001580: 2020 2020 2020 7061 7261 6772 6170 682e        paragraph.
-00001590: 2054 6869 7320 7769 6c6c 206f 6e6c 7920   This will only 
-000015a0: 6265 2075 7365 6675 6c20 7769 7468 2060  be useful with `
-000015b0: 602a 5f72 756e 7360 6020 6174 7472 6962  `*_runs`` attrib
-000015c0: 7574 6573 2e5c 6e20 2020 2020 2020 203a  utes.\n        :
-000015d0: 7061 7261 6d20 6475 706c 6963 6174 655f  param duplicate_
-000015e0: 6d65 7267 6564 5f63 656c 6c73 3a20 626f  merged_cells: bo
-000015f0: 6f6c 2c20 6475 706c 6963 6174 6520 6d65  ol, duplicate me
-00001600: 7267 6564 2063 656c 6c73 2074 6f20 7265  rged cells to re
-00001610: 7475 726e 2061 206d 786e 5c6e 2020 2020  turn a mxn\n    
-00001620: 2020 2020 2020 2020 6e65 7374 6564 206c          nested l
-00001630: 6973 7420 666f 7220 6561 6368 2074 6162  ist for each tab
-00001640: 6c65 2028 6465 6661 756c 7420 4661 6c73  le (default Fals
-00001650: 6529 5c6e 2020 2020 2020 2020 3a72 6574  e)\n        :ret
-00001660: 7572 6e3a 2044 6f63 7843 6f6e 7465 6e74  urn: DocxContent
-00001670: 206f 626a 6563 745c 6e20 2020 2020 2020   object\n       
-00001680: 2022 2222 5c6e 5c6e 5c6e 2323 2052 6574   """\n\n\n## Ret
-00001690: 7572 6e20 466f 726d 6174 5c6e 5c6e 536f  urn Format\n\nSo
-000016a0: 6d65 2073 7472 7563 7475 7265 2077 696c  me structure wil
-000016b0: 6c20 6265 206d 6169 6e74 6169 6e65 642e  l be maintained.
-000016c0: 2054 6578 7420 7769 6c6c 2062 6520 7265   Text will be re
-000016d0: 7475 726e 6564 2069 6e20 6120 6e65 7374  turned in a nest
-000016e0: 6564 206c 6973 742c 2077 6974 6820 7061  ed list, with pa
-000016f0: 7261 6772 6170 6873 2061 6c77 6179 7320  ragraphs always 
-00001700: 6174 2064 6570 7468 2034 2028 692e 652e  at depth 4 (i.e.
-00001710: 2c20 606f 7574 7075 742e 626f 6479 5b69  , `output.body[i
-00001720: 5d5b 6a5d 5b6b 5d5b 6c5d 6020 7769 6c6c  ][j][k][l]` will
-00001730: 2062 6520 6120 7061 7261 6772 6170 6829   be a paragraph)
-00001740: 2e5c 6e5c 6e49 6620 796f 7572 2064 6f63  .\n\nIf your doc
-00001750: 7820 6861 7320 6e6f 2074 6162 6c65 732c  x has no tables,
-00001760: 206f 7574 7075 742e 626f 6479 2077 696c   output.body wil
-00001770: 6c20 6170 7065 6172 2061 7320 6f6e 6520  l appear as one 
-00001780: 6120 7461 626c 6520 7769 7468 2061 6c6c  a table with all
-00001790: 2063 6f6e 7465 6e74 2069 6e20 6f6e 6520   content in one 
-000017a0: 6365 6c6c 3a5c 6e5c 6e60 6060 7079 7468  cell:\n\n```pyth
-000017b0: 6f6e 5c6e 5b20 2023 2064 6f63 756d 656e  on\n[  # documen
-000017c0: 745c 6e20 2020 205b 2020 2320 7461 626c  t\n    [  # tabl
-000017d0: 655c 6e20 2020 2020 2020 205b 2020 2320  e\n        [  # 
-000017e0: 726f 775c 6e20 2020 2020 2020 2020 2020  row\n           
-000017f0: 205b 2020 2320 6365 6c6c 5c6e 2020 2020   [  # cell\n    
-00001800: 2020 2020 2020 2020 2020 2020 2250 6172              "Par
-00001810: 6167 7261 7068 2031 222c 5c6e 2020 2020  agraph 1",\n    
-00001820: 2020 2020 2020 2020 2020 2020 2250 6172              "Par
-00001830: 6167 7261 7068 2032 222c 5c6e 2020 2020  agraph 2",\n    
-00001840: 2020 2020 2020 2020 2020 2020 222d 2d20              "-- 
-00001850: 6275 6c6c 6574 6564 206c 6973 7422 2c5c  bulleted list",\
-00001860: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00001870: 2022 2d2d 2063 6f6e 7469 6e75 696e 6720   "-- continuing 
-00001880: 6275 6c6c 6574 6564 206c 6973 7422 2c5c  bulleted list",\
-00001890: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000018a0: 2022 3129 2020 6e75 6d62 6572 6564 206c   "1)  numbered l
-000018b0: 6973 7422 2c5c 6e20 2020 2020 2020 2020  ist",\n         
-000018c0: 2020 2020 2020 2022 3229 2020 636f 6e74         "2)  cont
-000018d0: 696e 7569 6e67 206e 756d 6265 7265 6420  inuing numbered 
-000018e0: 6c69 7374 225c 6e20 2020 2020 2020 2020  list"\n         
-000018f0: 2020 2020 2020 2022 2020 2020 6129 2020         "    a)  
-00001900: 7375 626c 6973 7422 2c5c 6e20 2020 2020  sublist",\n     
-00001910: 2020 2020 2020 2020 2020 2022 2020 2020             "    
-00001920: 2020 2020 6929 2020 7375 626c 6973 7420      i)  sublist 
-00001930: 6f66 2073 7562 6c69 7374 222c 5c6e 2020  of sublist",\n  
-00001940: 2020 2020 2020 2020 2020 2020 2020 2233                "3
-00001950: 2920 206b 6565 7073 2074 7261 636b 206f  )  keeps track o
-00001960: 6620 696e 6465 6e74 696f 6e20 6c65 7665  f indention leve
-00001970: 6c73 222c 5c6e 2020 2020 2020 2020 2020  ls",\n          
-00001980: 2020 2020 2020 2220 2020 2061 2920 2072        "    a)  r
-00001990: 6573 6574 7320 7375 626c 6973 7420 636f  esets sublist co
-000019a0: 756e 7465 7273 225c 6e20 2020 2020 2020  unters"\n       
-000019b0: 2020 2020 205d 5c6e 2020 2020 2020 2020       ]\n        
-000019c0: 5d5c 6e20 2020 2020 5d5c 6e20 5d5c 6e60  ]\n     ]\n ]\n`
-000019d0: 6060 5c6e 5c6e 5461 626c 6520 6365 6c6c  ``\n\nTable cell
-000019e0: 7320 7769 6c6c 2061 7070 6561 7220 6173  s will appear as
-000019f0: 2074 6162 6c65 2063 656c 6c73 2e20 5465   table cells. Te
-00001a00: 7874 206f 7574 7369 6465 2074 6162 6c65  xt outside table
-00001a10: 7320 7769 6c6c 2061 7070 6561 7220 6173  s will appear as
-00001a20: 2074 6162 6c65 2063 656c 6c73 2e5c 6e5c   table cells.\n\
-00001a30: 6e5c 6e41 2064 6f63 7820 646f 6375 6d65  n\nA docx docume
-00001a40: 6e74 2063 616e 2062 6520 7461 626c 6573  nt can be tables
-00001a50: 2077 6974 6869 6e20 7461 626c 6573 2077   within tables w
-00001a60: 6974 6869 6e20 7461 626c 6573 2e20 446f  ithin tables. Do
-00001a70: 6378 3250 7974 686f 6e20 666c 6174 7465  cx2Python flatte
-00001a80: 6e73 206d 6f73 7420 6f66 2074 6869 7320  ns most of this 
-00001a90: 746f 206d 6f72 6520 6561 7369 6c79 206e  to more easily n
-00001aa0: 6176 6967 6174 655c 6e77 6974 6869 6e20  avigate\nwithin 
-00001ab0: 7468 6520 636f 6e74 656e 742e 5c6e 5c6e  the content.\n\n
-00001ac0: 2323 2057 6f72 6b69 6e67 2077 6974 6820  ## Working with 
-00001ad0: 6f75 7470 7574 5c6e 5c6e 5468 6973 2070  output\n\nThis p
-00001ae0: 6163 6b61 6765 2070 726f 7669 6465 7320  ackage provides 
-00001af0: 7365 7665 7261 6c20 646f 6375 6d65 6e74  several document
-00001b00: 6564 2068 656c 7065 7220 6675 6e63 7469  ed helper functi
-00001b10: 6f6e 7320 696e 205b 7468 6520 6060 646f  ons in [the ``do
-00001b20: 6378 3270 7974 686f 6e2e 6974 6572 6174  cx2python.iterat
-00001b30: 6f72 7360 6020 6d6f 6475 6c65 5d28 6874  ors`` module](ht
-00001b40: 7470 733a 2f2f 646f 6378 3270 7974 686f  tps://docx2pytho
-00001b50: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-00001b60: 2f65 6e2f 6c61 7465 7374 2f64 6f63 7832  /en/latest/docx2
-00001b70: 7079 7468 6f6e 2e68 746d 6c23 6d6f 6475  python.html#modu
-00001b80: 6c65 2d69 7465 7261 746f 7273 292e 2048  le-iterators). H
-00001b90: 6572 6520 6172 6520 6120 6665 7720 7265  ere are a few re
-00001ba0: 6369 7065 7320 706f 7373 6962 6c65 2077  cipes possible w
-00001bb0: 6974 6820 7468 6573 6520 6675 6e63 7469  ith these functi
-00001bc0: 6f6e 733a 5c6e 5c6e 6060 6070 7974 686f  ons:\n\n```pytho
-00001bd0: 6e5c 6e66 726f 6d20 646f 6378 3270 7974  n\nfrom docx2pyt
-00001be0: 686f 6e2e 6974 6572 6174 6f72 7320 696d  hon.iterators im
-00001bf0: 706f 7274 2065 6e75 6d5f 6365 6c6c 735c  port enum_cells\
-00001c00: 6e5c 6e64 6566 2072 656d 6f76 655f 656d  n\ndef remove_em
-00001c10: 7074 795f 7061 7261 6772 6170 6873 2874  pty_paragraphs(t
-00001c20: 6162 6c65 7329 3a5c 6e20 2020 2066 6f72  ables):\n    for
-00001c30: 2028 692c 206a 2c20 6b29 2c20 6365 6c6c   (i, j, k), cell
-00001c40: 2069 6e20 656e 756d 5f63 656c 6c73 2874   in enum_cells(t
-00001c50: 6162 6c65 7329 3a5c 6e20 2020 2020 2020  ables):\n       
-00001c60: 2074 6162 6c65 735b 695d 5b6a 5d5b 6b5d   tables[i][j][k]
-00001c70: 203d 205b 7820 666f 7220 7820 696e 2063   = [x for x in c
-00001c80: 656c 6c20 6966 2078 5d5c 6e60 6060 5c6e  ell if x]\n```\n
-00001c90: 5c6e 6060 605c 6e3e 3e3e 2074 6162 6c65  \n```\n>>> table
-00001ca0: 7320 3d20 5b5b 5b5b 5c27 615c 272c 205c  s = [[[[\'a\', \
-00001cb0: 2762 5c27 5d2c 205b 5c27 615c 272c 205c  'b\'], [\'a\', \
-00001cc0: 275c 272c 205c 2764 5c27 2c20 5c27 5c27  '\', \'d\', \'\'
-00001cd0: 5d5d 5d5d 5c6e 3e3e 3e20 7265 6d6f 7665  ]]]]\n>>> remove
-00001ce0: 5f65 6d70 7479 5f70 6172 6167 7261 7068  _empty_paragraph
-00001cf0: 7328 7461 626c 6573 295c 6e20 2020 205b  s(tables)\n    [
-00001d00: 5b5b 5b5c 2761 5c27 2c20 5c27 625c 275d  [[[\'a\', \'b\']
-00001d10: 2c20 5b5c 2761 5c27 2c20 5c27 645c 275d  , [\'a\', \'d\']
-00001d20: 5d5d 5d5c 6e60 6060 5c6e 5c6e 6060 6070  ]]]\n```\n\n```p
-00001d30: 7974 686f 6e5c 6e66 726f 6d20 646f 6378  ython\nfrom docx
-00001d40: 3270 7974 686f 6e2e 6974 6572 6174 6f72  2python.iterator
-00001d50: 7320 696d 706f 7274 2065 6e75 6d5f 6174  s import enum_at
-00001d60: 5f64 6570 7468 5c6e 5c6e 6465 6620 6874  _depth\n\ndef ht
-00001d70: 6d6c 5f6d 6170 2874 6162 6c65 7329 202d  ml_map(tables) -
-00001d80: 3e20 7374 723a 5c6e 2020 2020 2222 2243  > str:\n    """C
-00001d90: 7265 6174 6520 616e 2048 544d 4c20 6d61  reate an HTML ma
-00001da0: 7020 6f66 2064 6f63 756d 656e 7420 636f  p of document co
-00001db0: 6e74 656e 7473 2e5c 6e5c 6e20 2020 2052  ntents.\n\n    R
-00001dc0: 656e 6465 7220 7468 6973 2069 6e20 6120  ender this in a 
-00001dd0: 6272 6f77 7365 7220 746f 2076 6973 7561  browser to visua
-00001de0: 6c6c 7920 7365 6172 6368 2066 6f72 2064  lly search for d
-00001df0: 6174 612e 5c6e 5c6e 2020 2020 3a74 6162  ata.\n\n    :tab
-00001e00: 6c65 733a 2076 616c 7565 2063 6f75 6c64  les: value could
-00001e10: 2063 6f6d 6520 6672 6f6d 2c20 652e 672e   come from, e.g.
-00001e20: 2c5c 6e20 2020 2020 2020 202a 2064 6f63  ,\n        * doc
-00001e30: 785f 746f 5f74 6578 745f 6f75 7470 7574  x_to_text_output
-00001e40: 2e64 6f63 756d 656e 745c 6e20 2020 2020  .document\n     
-00001e50: 2020 202a 2064 6f63 785f 746f 5f74 6578     * docx_to_tex
-00001e60: 745f 6f75 7470 7574 2e62 6f64 795c 6e20  t_output.body\n 
-00001e70: 2020 2022 2222 5c6e 5c6e 2020 2020 2320     """\n\n    # 
-00001e80: 7072 6570 656e 6420 696e 6465 7820 7475  prepend index tu
-00001e90: 706c 6520 746f 2065 6163 6820 7061 7261  ple to each para
-00001ea0: 6772 6170 685c 6e20 2020 2066 6f72 2028  graph\n    for (
-00001eb0: 692c 206a 2c20 6b2c 206c 292c 2070 6172  i, j, k, l), par
-00001ec0: 6167 7261 7068 2069 6e20 656e 756d 5f61  agraph in enum_a
-00001ed0: 745f 6465 7074 6828 7461 626c 6573 2c20  t_depth(tables, 
-00001ee0: 3429 3a5c 6e20 2020 2020 2020 2074 6162  4):\n        tab
-00001ef0: 6c65 735b 695d 5b6a 5d5b 6b5d 5b6c 5d20  les[i][j][k][l] 
-00001f00: 3d20 2220 222e 6a6f 696e 285b 7374 7228  = " ".join([str(
-00001f10: 2869 2c20 6a2c 206b 2c20 6c29 292c 2070  (i, j, k, l)), p
-00001f20: 6172 6167 7261 7068 5d29 5c6e 5c6e 2020  aragraph])\n\n  
-00001f30: 2020 2320 7772 6170 2065 6163 6820 7061    # wrap each pa
-00001f40: 7261 6772 6170 6820 696e 203c 7072 653e  ragraph in <pre>
-00001f50: 2074 6167 735c 6e20 2020 2066 6f72 2028   tags\n    for (
-00001f60: 692c 206a 2c20 6b29 2c20 6365 6c6c 2069  i, j, k), cell i
-00001f70: 6e20 656e 756d 5f61 745f 6465 7074 6828  n enum_at_depth(
-00001f80: 7461 626c 6573 2c20 3329 3a5c 6e20 2020  tables, 3):\n   
-00001f90: 2020 2020 2074 6162 6c65 735b 695d 5b6a       tables[i][j
-00001fa0: 5d5b 6b5d 203d 2022 222e 6a6f 696e 285b  ][k] = "".join([
-00001fb0: 223c 7072 653e 7b78 7d3c 2f70 7265 3e22  "<pre>{x}</pre>"
-00001fc0: 2e66 6f72 6d61 7428 7829 2066 6f72 2078  .format(x) for x
-00001fd0: 2069 6e20 6365 6c6c 5d29 5c6e 5c6e 2020   in cell])\n\n  
-00001fe0: 2020 2320 7772 6170 2065 6163 6820 6365    # wrap each ce
-00001ff0: 6c6c 2069 6e20 3c74 643e 2074 6167 735c  ll in <td> tags\
-00002000: 6e20 2020 2066 6f72 2028 692c 206a 292c  n    for (i, j),
-00002010: 2072 6f77 2069 6e20 656e 756d 5f61 745f   row in enum_at_
-00002020: 6465 7074 6828 7461 626c 6573 2c20 3229  depth(tables, 2)
-00002030: 3a5c 6e20 2020 2020 2020 2074 6162 6c65  :\n        table
-00002040: 735b 695d 5b6a 5d20 3d20 2222 2e6a 6f69  s[i][j] = "".joi
-00002050: 6e28 5b22 3c74 643e 7b78 7d3c 2f74 643e  n(["<td>{x}</td>
-00002060: 222e 666f 726d 6174 2878 2920 666f 7220  ".format(x) for 
-00002070: 7820 696e 2072 6f77 5d29 5c6e 5c6e 2020  x in row])\n\n  
-00002080: 2020 2320 7772 6170 2065 6163 6820 726f    # wrap each ro
-00002090: 7720 696e 203c 7472 3e20 7461 6773 5c6e  w in <tr> tags\n
-000020a0: 2020 2020 666f 7220 2869 2c29 2c20 7461      for (i,), ta
-000020b0: 626c 6520 696e 2065 6e75 6d5f 6174 5f64  ble in enum_at_d
-000020c0: 6570 7468 2874 6162 6c65 732c 2031 293a  epth(tables, 1):
-000020d0: 5c6e 2020 2020 2020 2020 7461 626c 6573  \n        tables
-000020e0: 5b69 5d20 3d20 2222 2e6a 6f69 6e28 223c  [i] = "".join("<
-000020f0: 7472 3e7b 787d 3c2f 7472 3e22 2e66 6f72  tr>{x}</tr>".for
-00002100: 6d61 7428 7829 2066 6f72 2078 2069 6e20  mat(x) for x in 
-00002110: 7461 626c 6529 5c6e 5c6e 2020 2020 2320  table)\n\n    # 
-00002120: 7772 6170 2065 6163 6820 7461 626c 6520  wrap each table 
-00002130: 696e 203c 7461 626c 653e 2074 6167 735c  in <table> tags\
-00002140: 6e20 2020 2074 6162 6c65 7320 3d20 2222  n    tables = ""
-00002150: 2e6a 6f69 6e28 5b5c 273c 7461 626c 6520  .join([\'<table 
-00002160: 626f 7264 6572 3d22 3122 3e7b 787d 3c2f  border="1">{x}</
-00002170: 7461 626c 653e 5c27 2e66 6f72 6d61 7428  table>\'.format(
-00002180: 7829 2066 6f72 2078 2069 6e20 7461 626c  x) for x in tabl
-00002190: 6573 5d29 5c6e 5c6e 2020 2020 7265 7475  es])\n\n    retu
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646f 6378  : 2.1.Name: docx
+00000020: 3270 7974 686f 6e0a 5665 7273 696f 6e3a  2python.Version:
+00000030: 2032 2e36 2e33 0a53 756d 6d61 7279 3a20   2.6.3.Summary: 
+00000040: 4578 7472 6163 7420 636f 6e74 656e 7420  Extract content 
+00000050: 6672 6f6d 2064 6f63 7820 6669 6c65 730a  from docx files.
+00000060: 4c69 6365 6e73 653a 204d 4954 0a41 7574  License: MIT.Aut
+00000070: 686f 723a 2053 6861 7920 4869 6c6c 0a41  hor: Shay Hill.A
+00000080: 7574 686f 722d 656d 6169 6c3a 2073 6861  uthor-email: sha
+00000090: 795f 7075 626c 6963 4068 6f74 6d61 696c  y_public@hotmail
+000000a0: 2e63 6f6d 0a52 6571 7569 7265 732d 5079  .com.Requires-Py
+000000b0: 7468 6f6e 3a20 3e3d 332e 382c 3c34 2e30  thon: >=3.8,<4.0
+000000c0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+000000d0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000000e0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000000f0: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000100: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000110: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000120: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000150: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000160: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000170: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000180: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000190: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000001a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001b0: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+000001c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 2e31 310a 5265  ython :: 3.11.Re
+000001f0: 7175 6972 6573 2d44 6973 743a 206c 786d  quires-Dist: lxm
+00000200: 6c20 283e 3d34 2e39 2e32 2c3c 352e 302e  l (>=4.9.2,<5.0.
+00000210: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
+00000220: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000230: 742f 6d61 726b 646f 776e 0a0a 2320 646f  t/markdown..# do
+00000240: 6378 3270 7974 686f 6e0a 0a45 7874 7261  cx2python..Extra
+00000250: 6374 2064 6f63 7820 6865 6164 6572 732c  ct docx headers,
+00000260: 2066 6f6f 7465 7273 2c20 7465 7874 2c20   footers, text, 
+00000270: 666f 6f74 6e6f 7465 732c 2065 6e64 6e6f  footnotes, endno
+00000280: 7465 732c 2070 726f 7065 7274 6965 732c  tes, properties,
+00000290: 2061 6e64 2069 6d61 6765 7320 746f 2061   and images to a
+000002a0: 2050 7974 686f 6e20 6f62 6a65 6374 2e0a   Python object..
+000002b0: 0a60 5245 4144 4d45 5f44 4f43 585f 4649  .`README_DOCX_FI
+000002c0: 4c45 5f53 5452 5543 5455 5245 2e6d 6460  LE_STRUCTURE.md`
+000002d0: 206d 6179 2068 656c 7020 6966 2079 6f75   may help if you
+000002e0: 2764 206c 696b 6520 746f 2065 7874 656e  'd like to exten
+000002f0: 6420 646f 6378 3270 7974 686f 6e2e 0a0a  d docx2python...
+00000300: 466f 7220 6120 7375 6d6d 6172 7920 6f66  For a summary of
+00000310: 2077 6861 7427 7320 6e65 7720 696e 2064   what's new in d
+00000320: 6f63 7832 7079 7468 6f6e 2032 2c20 7363  ocx2python 2, sc
+00000330: 726f 6c6c 2064 6f77 6e20 746f 202a 2a4e  roll down to **N
+00000340: 6577 2069 6e20 646f 6378 3270 7974 686f  ew in docx2pytho
+00000350: 6e20 5665 7273 696f 6e20 322a 2a0a 0a54  n Version 2**..T
+00000360: 6865 2063 6f64 6520 6973 2061 6e20 6578  he code is an ex
+00000370: 7061 6e73 696f 6e2f 636f 6e74 7261 6374  pansion/contract
+00000380: 696f 6e20 6f66 205b 7079 7468 6f6e 2d64  ion of [python-d
+00000390: 6f63 7832 7478 745d 2868 7474 7073 3a2f  ocx2txt](https:/
+000003a0: 2f67 6974 6875 622e 636f 6d2f 616e 6b75  /github.com/anku
+000003b0: 7368 7368 6168 3839 2f70 7974 686f 6e2d  shshah89/python-
+000003c0: 646f 6378 3274 7874 2920 2843 6f70 7972  docx2txt) (Copyr
+000003d0: 6967 6874 2028 6329 2032 3031 3520 416e  ight (c) 2015 An
+000003e0: 6b75 7368 2053 6861 6829 2e20 5468 6520  kush Shah). The 
+000003f0: 6f72 6967 696e 616c 2063 6f64 6520 6973  original code is
+00000400: 206d 6f73 746c 7920 676f 6e65 2c20 6275   mostly gone, bu
+00000410: 7420 736f 6d65 206f 6620 7468 6520 626f  t some of the bo
+00000420: 6e65 7320 6d61 7920 7374 696c 6c20 6265  nes may still be
+00000430: 2068 6572 652e 0a0a 5f5f 7368 6172 6564   here...__shared
+00000440: 2066 6561 7475 7265 735f 5f3a 0a2a 2065   features__:.* e
+00000450: 7874 7261 6374 7320 7465 7874 2066 726f  xtracts text fro
+00000460: 6d20 646f 6378 2066 696c 6573 0a2a 2065  m docx files.* e
+00000470: 7874 7261 6374 7320 696d 6167 6573 2066  xtracts images f
+00000480: 726f 6d20 646f 6378 2066 696c 6573 0a0a  rom docx files..
+00000490: 5f5f 6164 6469 7469 6f6e 733a 5f5f 0a2a  __additions:__.*
+000004a0: 2065 7874 7261 6374 7320 666f 6f74 6e6f   extracts footno
+000004b0: 7465 7320 616e 6420 656e 646e 6f74 6573  tes and endnotes
+000004c0: 0a2a 2063 6f6e 7665 7274 7320 6275 6c6c  .* converts bull
+000004d0: 6574 7320 616e 6420 6e75 6d62 6572 6564  ets and numbered
+000004e0: 206c 6973 7473 2074 6f20 6173 6369 6920   lists to ascii 
+000004f0: 7769 7468 2069 6e64 656e 7461 7469 6f6e  with indentation
+00000500: 0a2a 2063 6f6e 7665 7274 7320 6879 7065  .* converts hype
+00000510: 726c 696e 6b73 2074 6f20 6060 3c61 2068  rlinks to ``<a h
+00000520: 7265 663d 2268 7474 703a 2f2e 2e2e 223e  ref="http:/...">
+00000530: 6c69 6e6b 2074 6578 743c 2f61 3e60 600a  link text</a>``.
+00000540: 2a20 7265 7461 696e 7320 736f 6d65 2073  * retains some s
+00000550: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+00000560: 6f72 6967 696e 616c 2066 696c 6520 286d  original file (m
+00000570: 6f72 6520 6265 6c6f 7729 0a2a 2065 7874  ore below).* ext
+00000580: 7261 6374 7320 646f 6375 6d65 6e74 2070  racts document p
+00000590: 726f 7065 7274 6965 7320 2863 7265 6174  roperties (creat
+000005a0: 6f72 2c20 6c61 7374 4d6f 6469 6669 6564  or, lastModified
+000005b0: 4279 2c20 6574 632e 290a 2a20 696e 7365  By, etc.).* inse
+000005c0: 7274 7320 696d 6167 6520 706c 6163 6568  rts image placeh
+000005d0: 6f6c 6465 7273 2069 6e20 7465 7874 2028  olders in text (
+000005e0: 6060 272d 2d2d 2d69 6d61 6765 312e 6a70  ``'----image1.jp
+000005f0: 672d 2d2d 2d27 6060 290a 2a20 696e 7365  g----'``).* inse
+00000600: 7274 7320 706c 6169 6e20 7465 7874 2066  rts plain text f
+00000610: 6f6f 746e 6f74 6520 616e 6420 656e 646e  ootnote and endn
+00000620: 6f74 6520 7265 6665 7265 6e63 6573 2069  ote references i
+00000630: 6e20 7465 7874 2028 6060 272d 2d2d 2d66  n text (``'----f
+00000640: 6f6f 746e 6f74 6531 2d2d 2d2d 2760 6029  ootnote1----'``)
+00000650: 0a2a 2028 6f70 7469 6f6e 616c 6c79 2920  .* (optionally) 
+00000660: 7265 7461 696e 7320 666f 6e74 2073 697a  retains font siz
+00000670: 652c 2066 6f6e 7420 636f 6c6f 722c 2062  e, font color, b
+00000680: 6f6c 642c 2069 7461 6c69 6373 2c20 616e  old, italics, an
+00000690: 6420 756e 6465 7273 636f 7265 2061 7320  d underscore as 
+000006a0: 6874 6d6c 0a2a 2065 7874 7261 6374 206d  html.* extract m
+000006b0: 6174 6820 6571 7561 7469 6f6e 730a 2a20  ath equations.* 
+000006c0: 6578 7472 6163 7420 7573 6572 2073 656c  extract user sel
+000006d0: 6563 7469 6f6e 7320 6672 6f6d 2063 6865  ections from che
+000006e0: 636b 626f 7865 7320 616e 6420 6472 6f70  ckboxes and drop
+000006f0: 646f 776e 206d 656e 7573 0a0a 5f5f 7375  down menus..__su
+00000700: 6274 7261 6374 696f 6e73 3a5f 5f0a 2a20  btractions:__.* 
+00000710: 6e6f 2063 6f6d 6d61 6e64 2d6c 696e 6520  no command-line 
+00000720: 696e 7465 7266 6163 650a 2a20 7769 6c6c  interface.* will
+00000730: 206f 6e6c 7920 776f 726b 2077 6974 6820   only work with 
+00000740: 5079 7468 6f6e 2033 2e38 2b0a 0a0a 2323  Python 3.8+...##
+00000750: 2049 6e73 7461 6c6c 6174 696f 6e0a 6060   Installation.``
+00000760: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00000770: 6c20 646f 6378 3270 7974 686f 6e0a 6060  l docx2python.``
+00000780: 600a 0a23 2320 5573 650a 0a60 6060 2070  `..## Use..``` p
+00000790: 7974 686f 6e0a 6672 6f6d 2064 6f63 7832  ython.from docx2
+000007a0: 7079 7468 6f6e 2069 6d70 6f72 7420 646f  python import do
+000007b0: 6378 3270 7974 686f 6e0a 0a23 2065 7874  cx2python..# ext
+000007c0: 7261 6374 2064 6f63 7820 636f 6e74 656e  ract docx conten
+000007d0: 740a 7769 7468 2064 6f63 7832 7079 7468  t.with docx2pyth
+000007e0: 6f6e 2827 7061 7468 2f74 6f2f 6669 6c65  on('path/to/file
+000007f0: 2e64 6f63 7827 2920 6173 2064 6f63 785f  .docx') as docx_
+00000800: 636f 6e74 656e 743a 0a20 2020 2070 7269  content:.    pri
+00000810: 6e74 2864 6f63 785f 636f 6e74 656e 742e  nt(docx_content.
+00000820: 7465 7874 290a 0a64 6f63 785f 636f 6e74  text)..docx_cont
+00000830: 656e 7420 3d20 646f 6378 3270 7974 686f  ent = docx2pytho
+00000840: 6e28 2770 6174 682f 746f 2f66 696c 652e  n('path/to/file.
+00000850: 646f 6378 2729 0a70 7269 6e74 2864 6f63  docx').print(doc
+00000860: 785f 636f 6e74 656e 742e 7465 7874 290a  x_content.text).
+00000870: 646f 6378 5f63 6f6e 7465 6e74 2e63 6c6f  docx_content.clo
+00000880: 7365 2829 0a0a 2320 6578 7472 6163 7420  se()..# extract 
+00000890: 646f 6378 2063 6f6e 7465 6e74 2c20 7772  docx content, wr
+000008a0: 6974 6520 696d 6167 6573 2074 6f20 696d  ite images to im
+000008b0: 6167 655f 6469 7265 6374 6f72 790a 7769  age_directory.wi
+000008c0: 7468 2064 6f63 7832 7079 7468 6f6e 2827  th docx2python('
+000008d0: 7061 7468 2f74 6f2f 6669 6c65 2e64 6f63  path/to/file.doc
+000008e0: 7827 2c20 2770 6174 682f 746f 2f69 6d61  x', 'path/to/ima
+000008f0: 6765 5f64 6972 6563 746f 7279 2729 2061  ge_directory') a
+00000900: 7320 646f 6378 5f63 6f6e 7465 6e74 3a0a  s docx_content:.
+00000910: 2020 2020 7072 696e 7428 646f 6378 5f63      print(docx_c
+00000920: 6f6e 7465 6e74 2e74 6578 7429 0a0a 2320  ontent.text)..# 
+00000930: 6578 7472 6163 7420 646f 6378 2063 6f6e  extract docx con
+00000940: 7465 6e74 2077 6974 6820 6261 7369 6320  tent with basic 
+00000950: 666f 6e74 2073 7479 6c65 7320 636f 6e76  font styles conv
+00000960: 6572 7465 6420 746f 2068 746d 6c0a 7769  erted to html.wi
+00000970: 7468 2064 6f63 7832 7079 7468 6f6e 2827  th docx2python('
+00000980: 7061 7468 2f74 6f2f 6669 6c65 2e64 6f63  path/to/file.doc
+00000990: 7827 2c20 6874 6d6c 3d54 7275 6529 2061  x', html=True) a
+000009a0: 7320 646f 6378 5f63 6f6e 7465 6e74 3a0a  s docx_content:.
+000009b0: 2020 2020 7072 696e 7428 646f 6378 5f63      print(docx_c
+000009c0: 6f6e 7465 6e74 2e74 6578 7429 0a60 6060  ontent.text).```
+000009d0: 0a0a 6064 6f63 7832 7079 7468 6f6e 6020  ..`docx2python` 
+000009e0: 6f70 656e 7320 6120 7a69 7066 696c 6520  opens a zipfile 
+000009f0: 6f62 6a65 6374 2061 6e64 2028 6c61 7a69  object and (lazi
+00000a00: 6c79 2920 7265 6164 7320 6974 2e20 5573  ly) reads it. Us
+00000a10: 6520 636f 6e74 6578 7420 6d61 6e61 6765  e context manage
+00000a20: 6d65 6e74 2028 6077 6974 6820 2e2e 2e20  ment (`with ... 
+00000a30: 6173 6029 2074 6f20 636c 6f73 6520 7468  as`) to close th
+00000a40: 6973 207a 6970 6669 6c65 206f 626a 6563  is zipfile objec
+00000a50: 7420 6f72 2065 7870 6c69 6369 746c 7920  t or explicitly 
+00000a60: 636c 6f73 6520 7769 7468 2060 646f 6378  close with `docx
+00000a70: 5f63 6f6e 7465 6e74 2e63 6c6f 7365 2829  _content.close()
+00000a80: 602e 0a0a 4e6f 7465 206f 6e20 6874 6d6c  `...Note on html
+00000a90: 2066 6561 7475 7265 3a0a 2a20 7375 7070   feature:.* supp
+00000aa0: 6f72 7473 2060 603c 693e 6060 6974 616c  orts ``<i>``ital
+00000ab0: 6963 2c20 6060 3c62 3e60 6062 6f6c 642c  ic, ``<b>``bold,
+00000ac0: 2060 603c 753e 6060 756e 6465 726c 696e   ``<u>``underlin
+00000ad0: 652c 2060 603c 733e 6060 7374 7269 6b65  e, ``<s>``strike
+00000ae0: 2c20 6060 3c73 7570 3e60 6073 7570 6572  , ``<sup>``super
+00000af0: 7363 7269 7074 2c20 6060 3c73 7562 3e60  script, ``<sub>`
+00000b00: 6073 7562 7363 7269 7074 2c20 6060 3c73  `subscript, ``<s
+00000b10: 7061 6e20 7374 796c 653d 2266 6f6e 742d  pan style="font-
+00000b20: 7661 7269 616e 743a 2073 6d61 6c6c 2d63  variant: small-c
+00000b30: 6170 7322 3e60 6073 6d61 6c6c 2063 6170  aps">``small cap
+00000b40: 732c 2060 603c 7370 616e 2073 7479 6c65  s, ``<span style
+00000b50: 3d22 7465 7874 2d74 7261 6e73 666f 726d  ="text-transform
+00000b60: 3a75 7070 6572 6361 7365 223e 6060 616c  :uppercase">``al
+00000b70: 6c20 6361 7073 2c20 6060 3c73 7061 6e20  l caps, ``<span 
+00000b80: 7374 796c 653d 2262 6163 6b67 726f 756e  style="backgroun
+00000b90: 642d 636f 6c6f 723a 2079 656c 6c6f 7722  d-color: yellow"
+00000ba0: 3e60 6068 6967 686c 6967 6874 6564 2c20  >``highlighted, 
+00000bb0: 6060 3c73 7061 6e20 7374 796c 653d 2266  ``<span style="f
+00000bc0: 6f6e 742d 7369 7a65 3a33 3222 3e60 6066  ont-size:32">``f
+00000bd0: 6f6e 7420 7369 7a65 2c20 6060 3c73 7061  ont size, ``<spa
+00000be0: 6e20 7374 796c 653d 2263 6f6c 6f72 3a23  n style="color:#
+00000bf0: 6666 3030 3030 223e 6060 636f 6c6f 7265  ff0000">``colore
+00000c00: 6420 7465 7874 2e0a 2a20 6879 7065 726c  d text..* hyperl
+00000c10: 696e 6b73 2077 696c 6c20 616c 7761 7973  inks will always
+00000c20: 2062 6520 6578 706f 7274 6564 2061 7320   be exported as 
+00000c30: 6874 6d6c 2028 6060 3c61 2068 7265 663d  html (``<a href=
+00000c40: 2268 7474 703a 2f2e 2e2e 223e 6c69 6e6b  "http:/...">link
+00000c50: 2074 6578 743c 2f61 3e60 6029 2c20 6576   text</a>``), ev
+00000c60: 656e 2069 6620 6060 6874 6d6c 3d46 616c  en if ``html=Fal
+00000c70: 7365 6060 2c20 6265 6361 7573 6520 4920  se``, because I 
+00000c80: 636f 756c 646e 2774 2074 6869 6e6b 206f  couldn't think o
+00000c90: 6620 6120 6d6f 7265 2063 616e 6f6e 6963  f a more canonic
+00000ca0: 616c 2072 6570 7265 7365 6e74 6174 696f  al representatio
+00000cb0: 6e2e 0a2a 2065 7665 7279 2074 6167 206f  n..* every tag o
+00000cc0: 7065 6e20 696e 2061 2070 6172 6167 7261  pen in a paragra
+00000cd0: 7068 2077 696c 6c20 6265 2063 6c6f 7365  ph will be close
+00000ce0: 6420 696e 2074 6861 7420 7061 7261 6772  d in that paragr
+00000cf0: 6170 6820 2861 6e64 2c20 7768 6572 6520  aph (and, where 
+00000d00: 6170 7072 6f70 7269 6174 652c 2072 656f  appropriate, reo
+00000d10: 7065 6e65 6420 696e 2074 6865 206e 6578  pened in the nex
+00000d20: 7420 7061 7261 6772 6170 6829 2e20 4966  t paragraph). If
+00000d30: 2074 776f 2073 7562 7365 7175 656e 6374   two subsequenct
+00000d40: 2070 6172 6167 7261 7068 7320 6172 6520   paragraphs are 
+00000d50: 626f 6c64 2c20 7468 6579 2077 696c 6c20  bold, they will 
+00000d60: 6265 2072 6574 7572 6e65 6420 6173 2060  be returned as `
+00000d70: 3c62 3e70 6172 6167 7261 7068 2061 3c2f  <b>paragraph a</
+00000d80: 623e 602c 2060 3c62 3e70 6172 6167 7261  b>`, `<b>paragra
+00000d90: 7068 2062 3c2f 623e 602e 2054 6869 7320  ph b</b>`. This 
+00000da0: 6973 2069 6e74 656e 7469 6f6e 616c 2074  is intentional t
+00000db0: 6f20 6d61 6b65 2020 6561 6368 2070 6172  o make  each par
+00000dc0: 6167 7261 7068 2069 7473 206f 776e 2065  agraph its own e
+00000dd0: 6e74 6974 792e 0a2a 2069 6620 796f 7520  ntity..* if you 
+00000de0: 7370 6563 6966 7920 6068 746d 6c3d 5472  specify `html=Tr
+00000df0: 7565 602c 2060 2660 2c20 603e 6020 616e  ue`, `&`, `>` an
+00000e00: 6420 603c 6020 696e 2079 6f75 7220 646f  d `<` in your do
+00000e10: 6378 2074 6578 7420 7769 6c6c 2062 6520  cx text will be 
+00000e20: 656e 636f 6465 6420 6173 2060 2661 6d70  encoded as `&amp
+00000e30: 602c 2060 2667 743b 6020 616e 6420 6026  `, `&gt;` and `&
+00000e40: 6c74 3b60 0a0a 2323 2052 6574 7572 6e20  lt;`..## Return 
+00000e50: 5661 6c75 650a 0a46 756e 6374 696f 6e20  Value..Function 
+00000e60: 6064 6f63 7832 7079 7468 6f6e 6020 7265  `docx2python` re
+00000e70: 7475 726e 7320 6120 446f 6378 436f 6e74  turns a DocxCont
+00000e80: 656e 7420 696e 7374 616e 6365 2077 6974  ent instance wit
+00000e90: 6820 7365 7665 7261 6c20 6174 7472 6962  h several attrib
+00000ea0: 7574 6573 2e0a 0a5f 5f68 6561 6465 725f  utes...__header_
+00000eb0: 5f20 2d20 636f 6e74 656e 7473 206f 6620  _ - contents of 
+00000ec0: 7468 6520 646f 6378 2068 6561 6465 7273  the docx headers
+00000ed0: 2069 6e20 7468 6520 7265 7475 726e 2066   in the return f
+00000ee0: 6f72 6d61 7420 6465 7363 7269 6265 6420  ormat described 
+00000ef0: 6865 7265 696e 0a0a 5f5f 666f 6f74 6572  herein..__footer
+00000f00: 5f5f 202d 2063 6f6e 7465 6e74 7320 6f66  __ - contents of
+00000f10: 2074 6865 2064 6f63 7820 666f 6f74 6572   the docx footer
+00000f20: 7320 696e 2074 6865 2072 6574 7572 6e20  s in the return 
+00000f30: 666f 726d 6174 2064 6573 6372 6962 6564  format described
+00000f40: 2068 6572 6569 6e0a 0a5f 5f62 6f64 795f   herein..__body_
+00000f50: 5f20 2d20 636f 6e74 656e 7473 206f 6620  _ - contents of 
+00000f60: 7468 6520 646f 6378 2069 6e20 7468 6520  the docx in the 
+00000f70: 7265 7475 726e 2066 6f72 6d61 7420 6465  return format de
+00000f80: 7363 7269 6265 6420 6865 7265 696e 0a0a  scribed herein..
+00000f90: 5f5f 666f 6f74 6e6f 7465 735f 5f20 2d20  __footnotes__ - 
+00000fa0: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00000fb0: 646f 6378 2069 6e20 7468 6520 7265 7475  docx in the retu
+00000fc0: 726e 2066 6f72 6d61 7420 6465 7363 7269  rn format descri
+00000fd0: 6265 6420 6865 7265 696e 0a0a 5f5f 656e  bed herein..__en
+00000fe0: 646e 6f74 6573 5f5f 202d 2063 6f6e 7465  dnotes__ - conte
+00000ff0: 6e74 7320 6f66 2074 6865 2064 6f63 7820  nts of the docx 
+00001000: 696e 2074 6865 2072 6574 7572 6e20 666f  in the return fo
+00001010: 726d 6174 2064 6573 6372 6962 6564 2068  rmat described h
+00001020: 6572 6569 6e0a 0a5f 5f64 6f63 756d 656e  erein..__documen
+00001030: 745f 5f20 2d20 6865 6164 6572 2020 2b20  t__ - header  + 
+00001040: 626f 6479 202b 2066 6f6f 7465 7220 2872  body + footer (r
+00001050: 6561 6420 6f6e 6c79 290a 0a5f 5f74 6578  ead only)..__tex
+00001060: 745f 5f20 2d20 616c 6c20 646f 6378 2074  t__ - all docx t
+00001070: 6578 7420 6173 206f 6e65 2073 7472 696e  ext as one strin
+00001080: 672c 2073 696d 696c 6172 2074 6f20 7768  g, similar to wh
+00001090: 6174 2079 6f75 2764 2067 6574 2066 726f  at you'd get fro
+000010a0: 6d20 6070 7974 686f 6e2d 646f 6378 3274  m `python-docx2t
+000010b0: 7874 600a 0a5f 5f70 726f 7065 7274 6965  xt`..__propertie
+000010c0: 735f 5f20 2d20 646f 6378 2070 726f 7065  s__ - docx prope
+000010d0: 7274 7920 6e61 6d65 7320 6d61 7070 6564  rty names mapped
+000010e0: 2074 6f20 7661 6c75 6573 2028 652e 672e   to values (e.g.
+000010f0: 2c20 607b 226c 6173 744d 6f64 6966 6965  , `{"lastModifie
+00001100: 6442 7922 3a20 2253 6861 7920 4869 6c6c  dBy": "Shay Hill
+00001110: 227d 6029 0a0a 5f5f 696d 6167 6573 5f5f  "}`)..__images__
+00001120: 202d 2069 6d61 6765 206e 616d 6573 206d   - image names m
+00001130: 6170 7065 6420 746f 2069 6d61 6765 7320  apped to images 
+00001140: 696e 2062 696e 6172 7920 666f 726d 6174  in binary format
+00001150: 2e20 5772 6974 6520 746f 2066 696c 6573  . Write to files
+00001160: 7973 7465 6d20 7769 7468 0a0a 6060 600a  ystem with..```.
+00001170: 666f 7220 6e61 6d65 2c20 696d 6167 6520  for name, image 
+00001180: 696e 2072 6573 756c 742e 696d 6167 6573  in result.images
+00001190: 2e69 7465 6d73 2829 3a0a 2020 2020 7769  .items():.    wi
+000011a0: 7468 206f 7065 6e28 6e61 6d65 2c20 2777  th open(name, 'w
+000011b0: 6227 2920 6173 2069 6d61 6765 5f64 6573  b') as image_des
+000011c0: 7469 6e61 7469 6f6e 3a0a 2020 2020 2020  tination:.      
+000011d0: 2020 7772 6974 6528 696d 6167 655f 6465    write(image_de
+000011e0: 7374 696e 6174 696f 6e2c 2069 6d61 6765  stination, image
+000011f0: 290a 0a23 206f 720a 0a77 6974 6820 646f  )..# or..with do
+00001200: 6378 3270 7974 686f 6e28 2770 6174 682f  cx2python('path/
+00001210: 746f 2f66 696c 652e 646f 6378 272c 2027  to/file.docx', '
+00001220: 7061 7468 2f74 6f2f 696d 6167 652f 6469  path/to/image/di
+00001230: 7265 6374 6f72 7927 2920 6173 2064 6f63  rectory') as doc
+00001240: 785f 636f 6e74 656e 743a 0a20 2020 202e  x_content:.    .
+00001250: 2e2e 0a0a 2320 6f72 0a0a 7769 7468 2064  ....# or..with d
+00001260: 6f63 7832 7079 7468 6f6e 2827 7061 7468  ocx2python('path
+00001270: 2f74 6f2f 6669 6c65 2e64 6f63 7827 2920  /to/file.docx') 
+00001280: 6173 2064 6f63 785f 636f 6e74 656e 743a  as docx_content:
+00001290: 0a20 2020 2064 6f63 785f 636f 6e74 656e  .    docx_conten
+000012a0: 742e 7361 7665 5f69 6d61 6765 7328 2770  t.save_images('p
+000012b0: 6174 682f 746f 2f69 6d61 6765 2f64 6972  ath/to/image/dir
+000012c0: 6563 746f 7279 2729 0a0a 6060 600a 0a5f  ectory')..```.._
+000012d0: 5f64 6f63 785f 7265 6164 6572 5f5f 202d  _docx_reader__ -
+000012e0: 2061 2044 6f63 7852 6561 6465 7220 2873   a DocxReader (s
+000012f0: 6565 2060 646f 6378 5f72 6561 6465 722e  ee `docx_reader.
+00001300: 7079 6029 2069 6e73 7461 6e63 6520 7769  py`) instance wi
+00001310: 7468 2073 6576 6572 616c 206d 6574 686f  th several metho
+00001320: 6473 2066 6f72 2065 7874 7261 6374 696e  ds for extractin
+00001330: 6720 786d 6c20 706f 7274 696f 6e73 2e0a  g xml portions..
+00001340: 0a0a 2323 2041 7267 756d 656e 7473 0a0a  ..## Arguments..
+00001350: 2020 2020 6465 6620 646f 6378 3270 7974      def docx2pyt
+00001360: 686f 6e28 0a20 2020 2020 2020 2064 6f63  hon(.        doc
+00001370: 785f 6669 6c65 6e61 6d65 3a20 7374 7220  x_filename: str 
+00001380: 7c20 5061 7468 207c 2042 7974 6573 494f  | Path | BytesIO
+00001390: 2c0a 2020 2020 2020 2020 696d 6167 655f  ,.        image_
+000013a0: 666f 6c64 6572 3a20 7374 7220 7c20 4e6f  folder: str | No
+000013b0: 6e65 203d 204e 6f6e 652c 0a20 2020 2020  ne = None,.     
+000013c0: 2020 2068 746d 6c3a 2062 6f6f 6c20 3d20     html: bool = 
+000013d0: 4661 6c73 652c 0a20 2020 2020 2020 2070  False,.        p
+000013e0: 6172 6167 7261 7068 5f73 7479 6c65 733a  aragraph_styles:
+000013f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00001400: 2020 2020 2020 2065 7874 7261 6374 5f69         extract_i
+00001410: 6d61 6765 3a20 626f 6f6c 207c 204e 6f6e  mage: bool | Non
+00001420: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00001430: 2020 6475 706c 6963 6174 655f 6d65 7267    duplicate_merg
+00001440: 6564 5f63 656c 6c73 3a20 626f 6f6c 203d  ed_cells: bool =
+00001450: 2046 616c 7365 0a20 2020 2029 202d 3e20   False.    ) -> 
+00001460: 446f 6378 436f 6e74 656e 743a 0a20 2020  DocxContent:.   
+00001470: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001480: 2055 6e7a 6970 2061 2064 6f63 7820 6669   Unzip a docx fi
+00001490: 6c65 2061 6e64 2065 7874 7261 6374 2063  le and extract c
+000014a0: 6f6e 7465 6e74 732e 0a0a 2020 2020 2020  ontents...      
+000014b0: 2020 3a70 6172 616d 2064 6f63 785f 6669    :param docx_fi
+000014c0: 6c65 6e61 6d65 3a20 7061 7468 2074 6f20  lename: path to 
+000014d0: 6120 646f 6378 2066 696c 650a 2020 2020  a docx file.    
+000014e0: 2020 2020 3a70 6172 616d 2069 6d61 6765      :param image
+000014f0: 5f66 6f6c 6465 723a 206f 7074 696f 6e61  _folder: optiona
+00001500: 6c6c 7920 7370 6563 6966 7920 616e 2069  lly specify an i
+00001510: 6d61 6765 2066 6f6c 6465 720a 2020 2020  mage folder.    
+00001520: 2020 2020 2020 2020 2869 6d61 6765 7320          (images 
+00001530: 696e 2064 6f63 7820 7769 6c6c 2062 6520  in docx will be 
+00001540: 636f 7069 6564 2074 6f20 7468 6973 2066  copied to this f
+00001550: 6f6c 6465 7229 0a20 2020 2020 2020 203a  older).        :
+00001560: 7061 7261 6d20 6874 6d6c 3a20 626f 6f6c  param html: bool
+00001570: 2c20 6578 7472 6163 7420 736f 6d65 2066  , extract some f
+00001580: 6f72 6d61 7474 696e 6720 6173 2068 746d  ormatting as htm
+00001590: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
+000015a0: 2070 6172 6167 7261 7068 5f73 7479 6c65   paragraph_style
+000015b0: 733a 2070 7265 7065 6e64 2074 6865 2070  s: prepend the p
+000015c0: 6172 6167 7261 7068 7320 7374 796c 6520  aragraphs style 
+000015d0: 2869 6620 616e 792c 2065 6c73 6520 2222  (if any, else ""
+000015e0: 2920 746f 2065 6163 680a 2020 2020 2020  ) to each.      
+000015f0: 2020 2020 2020 7061 7261 6772 6170 682e        paragraph.
+00001600: 2054 6869 7320 7769 6c6c 206f 6e6c 7920   This will only 
+00001610: 6265 2075 7365 6675 6c20 7769 7468 2060  be useful with `
+00001620: 602a 5f72 756e 7360 6020 6174 7472 6962  `*_runs`` attrib
+00001630: 7574 6573 2e0a 2020 2020 2020 2020 3a70  utes..        :p
+00001640: 6172 616d 2064 7570 6c69 6361 7465 5f6d  aram duplicate_m
+00001650: 6572 6765 645f 6365 6c6c 733a 2062 6f6f  erged_cells: boo
+00001660: 6c2c 2064 7570 6c69 6361 7465 206d 6572  l, duplicate mer
+00001670: 6765 6420 6365 6c6c 7320 746f 2072 6574  ged cells to ret
+00001680: 7572 6e20 6120 6d78 6e0a 2020 2020 2020  urn a mxn.      
+00001690: 2020 2020 2020 6e65 7374 6564 206c 6973        nested lis
+000016a0: 7420 666f 7220 6561 6368 2074 6162 6c65  t for each table
+000016b0: 2028 6465 6661 756c 7420 4661 6c73 6529   (default False)
+000016c0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000016d0: 3a20 446f 6378 436f 6e74 656e 7420 6f62  : DocxContent ob
+000016e0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+000016f0: 0a0a 0a23 2320 5265 7475 726e 2046 6f72  ...## Return For
+00001700: 6d61 740a 0a53 6f6d 6520 7374 7275 6374  mat..Some struct
+00001710: 7572 6520 7769 6c6c 2062 6520 6d61 696e  ure will be main
+00001720: 7461 696e 6564 2e20 5465 7874 2077 696c  tained. Text wil
+00001730: 6c20 6265 2072 6574 7572 6e65 6420 696e  l be returned in
+00001740: 2061 206e 6573 7465 6420 6c69 7374 2c20   a nested list, 
+00001750: 7769 7468 2070 6172 6167 7261 7068 7320  with paragraphs 
+00001760: 616c 7761 7973 2061 7420 6465 7074 6820  always at depth 
+00001770: 3420 2869 2e65 2e2c 2060 6f75 7470 7574  4 (i.e., `output
+00001780: 2e62 6f64 795b 695d 5b6a 5d5b 6b5d 5b6c  .body[i][j][k][l
+00001790: 5d60 2077 696c 6c20 6265 2061 2070 6172  ]` will be a par
+000017a0: 6167 7261 7068 292e 0a0a 4966 2079 6f75  agraph)...If you
+000017b0: 7220 646f 6378 2068 6173 206e 6f20 7461  r docx has no ta
+000017c0: 626c 6573 2c20 6f75 7470 7574 2e62 6f64  bles, output.bod
+000017d0: 7920 7769 6c6c 2061 7070 6561 7220 6173  y will appear as
+000017e0: 206f 6e65 2061 2074 6162 6c65 2077 6974   one a table wit
+000017f0: 6820 616c 6c20 636f 6e74 656e 7420 696e  h all content in
+00001800: 206f 6e65 2063 656c 6c3a 0a0a 6060 6070   one cell:..```p
+00001810: 7974 686f 6e0a 5b20 2023 2064 6f63 756d  ython.[  # docum
+00001820: 656e 740a 2020 2020 5b20 2023 2074 6162  ent.    [  # tab
+00001830: 6c65 0a20 2020 2020 2020 205b 2020 2320  le.        [  # 
+00001840: 726f 770a 2020 2020 2020 2020 2020 2020  row.            
+00001850: 5b20 2023 2063 656c 6c0a 2020 2020 2020  [  # cell.      
+00001860: 2020 2020 2020 2020 2020 2250 6172 6167            "Parag
+00001870: 7261 7068 2031 222c 0a20 2020 2020 2020  raph 1",.       
+00001880: 2020 2020 2020 2020 2022 5061 7261 6772           "Paragr
+00001890: 6170 6820 3222 2c0a 2020 2020 2020 2020  aph 2",.        
+000018a0: 2020 2020 2020 2020 222d 2d20 6275 6c6c          "-- bull
+000018b0: 6574 6564 206c 6973 7422 2c0a 2020 2020  eted list",.    
+000018c0: 2020 2020 2020 2020 2020 2020 222d 2d20              "-- 
+000018d0: 636f 6e74 696e 7569 6e67 2062 756c 6c65  continuing bulle
+000018e0: 7465 6420 6c69 7374 222c 0a20 2020 2020  ted list",.     
+000018f0: 2020 2020 2020 2020 2020 2022 3129 2020             "1)  
+00001900: 6e75 6d62 6572 6564 206c 6973 7422 2c0a  numbered list",.
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2232 2920 2063 6f6e 7469 6e75 696e 6720  "2)  continuing 
+00001930: 6e75 6d62 6572 6564 206c 6973 7422 0a20  numbered list". 
+00001940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001950: 2020 2020 6129 2020 7375 626c 6973 7422      a)  sublist"
+00001960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001970: 2020 2220 2020 2020 2020 2069 2920 2073    "        i)  s
+00001980: 7562 6c69 7374 206f 6620 7375 626c 6973  ublist of sublis
+00001990: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+000019a0: 2020 2020 2233 2920 206b 6565 7073 2074      "3)  keeps t
+000019b0: 7261 636b 206f 6620 696e 6465 6e74 696f  rack of indentio
+000019c0: 6e20 6c65 7665 6c73 222c 0a20 2020 2020  n levels",.     
+000019d0: 2020 2020 2020 2020 2020 2022 2020 2020             "    
+000019e0: 6129 2020 7265 7365 7473 2073 7562 6c69  a)  resets subli
+000019f0: 7374 2063 6f75 6e74 6572 7322 0a20 2020  st counters".   
+00001a00: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00001a10: 2020 205d 0a20 2020 2020 5d0a 205d 0a60     ].     ]. ].`
+00001a20: 6060 0a0a 5461 626c 6520 6365 6c6c 7320  ``..Table cells 
+00001a30: 7769 6c6c 2061 7070 6561 7220 6173 2074  will appear as t
+00001a40: 6162 6c65 2063 656c 6c73 2e20 5465 7874  able cells. Text
+00001a50: 206f 7574 7369 6465 2074 6162 6c65 7320   outside tables 
+00001a60: 7769 6c6c 2061 7070 6561 7220 6173 2074  will appear as t
+00001a70: 6162 6c65 2063 656c 6c73 2e0a 0a0a 4120  able cells....A 
+00001a80: 646f 6378 2064 6f63 756d 656e 7420 6361  docx document ca
+00001a90: 6e20 6265 2074 6162 6c65 7320 7769 7468  n be tables with
+00001aa0: 696e 2074 6162 6c65 7320 7769 7468 696e  in tables within
+00001ab0: 2074 6162 6c65 732e 2044 6f63 7832 5079   tables. Docx2Py
+00001ac0: 7468 6f6e 2066 6c61 7474 656e 7320 6d6f  thon flattens mo
+00001ad0: 7374 206f 6620 7468 6973 2074 6f20 6d6f  st of this to mo
+00001ae0: 7265 2065 6173 696c 7920 6e61 7669 6761  re easily naviga
+00001af0: 7465 0a77 6974 6869 6e20 7468 6520 636f  te.within the co
+00001b00: 6e74 656e 742e 0a0a 2323 2057 6f72 6b69  ntent...## Worki
+00001b10: 6e67 2077 6974 6820 6f75 7470 7574 0a0a  ng with output..
+00001b20: 5468 6973 2070 6163 6b61 6765 2070 726f  This package pro
+00001b30: 7669 6465 7320 7365 7665 7261 6c20 646f  vides several do
+00001b40: 6375 6d65 6e74 6564 2068 656c 7065 7220  cumented helper 
+00001b50: 6675 6e63 7469 6f6e 7320 696e 205b 7468  functions in [th
+00001b60: 6520 6060 646f 6378 3270 7974 686f 6e2e  e ``docx2python.
+00001b70: 6974 6572 6174 6f72 7360 6020 6d6f 6475  iterators`` modu
+00001b80: 6c65 5d28 6874 7470 733a 2f2f 646f 6378  le](https://docx
+00001b90: 3270 7974 686f 6e2e 7265 6164 7468 6564  2python.readthed
+00001ba0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001bb0: 2f64 6f63 7832 7079 7468 6f6e 2e68 746d  /docx2python.htm
+00001bc0: 6c23 6d6f 6475 6c65 2d69 7465 7261 746f  l#module-iterato
+00001bd0: 7273 292e 2048 6572 6520 6172 6520 6120  rs). Here are a 
+00001be0: 6665 7720 7265 6369 7065 7320 706f 7373  few recipes poss
+00001bf0: 6962 6c65 2077 6974 6820 7468 6573 6520  ible with these 
+00001c00: 6675 6e63 7469 6f6e 733a 0a0a 6060 6070  functions:..```p
+00001c10: 7974 686f 6e0a 6672 6f6d 2064 6f63 7832  ython.from docx2
+00001c20: 7079 7468 6f6e 2e69 7465 7261 746f 7273  python.iterators
+00001c30: 2069 6d70 6f72 7420 656e 756d 5f63 656c   import enum_cel
+00001c40: 6c73 0a0a 6465 6620 7265 6d6f 7665 5f65  ls..def remove_e
+00001c50: 6d70 7479 5f70 6172 6167 7261 7068 7328  mpty_paragraphs(
+00001c60: 7461 626c 6573 293a 0a20 2020 2066 6f72  tables):.    for
+00001c70: 2028 692c 206a 2c20 6b29 2c20 6365 6c6c   (i, j, k), cell
+00001c80: 2069 6e20 656e 756d 5f63 656c 6c73 2874   in enum_cells(t
+00001c90: 6162 6c65 7329 3a0a 2020 2020 2020 2020  ables):.        
+00001ca0: 7461 626c 6573 5b69 5d5b 6a5d 5b6b 5d20  tables[i][j][k] 
+00001cb0: 3d20 5b78 2066 6f72 2078 2069 6e20 6365  = [x for x in ce
+00001cc0: 6c6c 2069 6620 785d 0a60 6060 0a0a 6060  ll if x].```..``
+00001cd0: 600a 3e3e 3e20 7461 626c 6573 203d 205b  `.>>> tables = [
+00001ce0: 5b5b 5b27 6127 2c20 2762 275d 2c20 5b27  [[['a', 'b'], ['
+00001cf0: 6127 2c20 2727 2c20 2764 272c 2027 275d  a', '', 'd', '']
+00001d00: 5d5d 5d0a 3e3e 3e20 7265 6d6f 7665 5f65  ]]].>>> remove_e
+00001d10: 6d70 7479 5f70 6172 6167 7261 7068 7328  mpty_paragraphs(
+00001d20: 7461 626c 6573 290a 2020 2020 5b5b 5b5b  tables).    [[[[
+00001d30: 2761 272c 2027 6227 5d2c 205b 2761 272c  'a', 'b'], ['a',
+00001d40: 2027 6427 5d5d 5d5d 0a60 6060 0a0a 6060   'd']]]].```..``
+00001d50: 6070 7974 686f 6e0a 6672 6f6d 2064 6f63  `python.from doc
+00001d60: 7832 7079 7468 6f6e 2e69 7465 7261 746f  x2python.iterato
+00001d70: 7273 2069 6d70 6f72 7420 656e 756d 5f61  rs import enum_a
+00001d80: 745f 6465 7074 680a 0a64 6566 2068 746d  t_depth..def htm
+00001d90: 6c5f 6d61 7028 7461 626c 6573 2920 2d3e  l_map(tables) ->
+00001da0: 2073 7472 3a0a 2020 2020 2222 2243 7265   str:.    """Cre
+00001db0: 6174 6520 616e 2048 544d 4c20 6d61 7020  ate an HTML map 
+00001dc0: 6f66 2064 6f63 756d 656e 7420 636f 6e74  of document cont
+00001dd0: 656e 7473 2e0a 0a20 2020 2052 656e 6465  ents...    Rende
+00001de0: 7220 7468 6973 2069 6e20 6120 6272 6f77  r this in a brow
+00001df0: 7365 7220 746f 2076 6973 7561 6c6c 7920  ser to visually 
+00001e00: 7365 6172 6368 2066 6f72 2064 6174 612e  search for data.
+00001e10: 0a0a 2020 2020 3a74 6162 6c65 733a 2076  ..    :tables: v
+00001e20: 616c 7565 2063 6f75 6c64 2063 6f6d 6520  alue could come 
+00001e30: 6672 6f6d 2c20 652e 672e 2c0a 2020 2020  from, e.g.,.    
+00001e40: 2020 2020 2a20 646f 6378 5f74 6f5f 7465      * docx_to_te
+00001e50: 7874 5f6f 7574 7075 742e 646f 6375 6d65  xt_output.docume
+00001e60: 6e74 0a20 2020 2020 2020 202a 2064 6f63  nt.        * doc
+00001e70: 785f 746f 5f74 6578 745f 6f75 7470 7574  x_to_text_output
+00001e80: 2e62 6f64 790a 2020 2020 2222 220a 0a20  .body.    """.. 
+00001e90: 2020 2023 2070 7265 7065 6e64 2069 6e64     # prepend ind
+00001ea0: 6578 2074 7570 6c65 2074 6f20 6561 6368  ex tuple to each
+00001eb0: 2070 6172 6167 7261 7068 0a20 2020 2066   paragraph.    f
+00001ec0: 6f72 2028 692c 206a 2c20 6b2c 206c 292c  or (i, j, k, l),
+00001ed0: 2070 6172 6167 7261 7068 2069 6e20 656e   paragraph in en
+00001ee0: 756d 5f61 745f 6465 7074 6828 7461 626c  um_at_depth(tabl
+00001ef0: 6573 2c20 3429 3a0a 2020 2020 2020 2020  es, 4):.        
+00001f00: 7461 626c 6573 5b69 5d5b 6a5d 5b6b 5d5b  tables[i][j][k][
+00001f10: 6c5d 203d 2022 2022 2e6a 6f69 6e28 5b73  l] = " ".join([s
+00001f20: 7472 2828 692c 206a 2c20 6b2c 206c 2929  tr((i, j, k, l))
+00001f30: 2c20 7061 7261 6772 6170 685d 290a 0a20  , paragraph]).. 
+00001f40: 2020 2023 2077 7261 7020 6561 6368 2070     # wrap each p
+00001f50: 6172 6167 7261 7068 2069 6e20 3c70 7265  aragraph in <pre
+00001f60: 3e20 7461 6773 0a20 2020 2066 6f72 2028  > tags.    for (
+00001f70: 692c 206a 2c20 6b29 2c20 6365 6c6c 2069  i, j, k), cell i
+00001f80: 6e20 656e 756d 5f61 745f 6465 7074 6828  n enum_at_depth(
+00001f90: 7461 626c 6573 2c20 3329 3a0a 2020 2020  tables, 3):.    
+00001fa0: 2020 2020 7461 626c 6573 5b69 5d5b 6a5d      tables[i][j]
+00001fb0: 5b6b 5d20 3d20 2222 2e6a 6f69 6e28 5b22  [k] = "".join(["
+00001fc0: 3c70 7265 3e7b 787d 3c2f 7072 653e 222e  <pre>{x}</pre>".
+00001fd0: 666f 726d 6174 2878 2920 666f 7220 7820  format(x) for x 
+00001fe0: 696e 2063 656c 6c5d 290a 0a20 2020 2023  in cell])..    #
+00001ff0: 2077 7261 7020 6561 6368 2063 656c 6c20   wrap each cell 
+00002000: 696e 203c 7464 3e20 7461 6773 0a20 2020  in <td> tags.   
+00002010: 2066 6f72 2028 692c 206a 292c 2072 6f77   for (i, j), row
+00002020: 2069 6e20 656e 756d 5f61 745f 6465 7074   in enum_at_dept
+00002030: 6828 7461 626c 6573 2c20 3229 3a0a 2020  h(tables, 2):.  
+00002040: 2020 2020 2020 7461 626c 6573 5b69 5d5b        tables[i][
+00002050: 6a5d 203d 2022 222e 6a6f 696e 285b 223c  j] = "".join(["<
+00002060: 7464 3e7b 787d 3c2f 7464 3e22 2e66 6f72  td>{x}</td>".for
+00002070: 6d61 7428 7829 2066 6f72 2078 2069 6e20  mat(x) for x in 
+00002080: 726f 775d 290a 0a20 2020 2023 2077 7261  row])..    # wra
+00002090: 7020 6561 6368 2072 6f77 2069 6e20 3c74  p each row in <t
+000020a0: 723e 2074 6167 730a 2020 2020 666f 7220  r> tags.    for 
+000020b0: 2869 2c29 2c20 7461 626c 6520 696e 2065  (i,), table in e
+000020c0: 6e75 6d5f 6174 5f64 6570 7468 2874 6162  num_at_depth(tab
+000020d0: 6c65 732c 2031 293a 0a20 2020 2020 2020  les, 1):.       
+000020e0: 2074 6162 6c65 735b 695d 203d 2022 222e   tables[i] = "".
+000020f0: 6a6f 696e 2822 3c74 723e 7b78 7d3c 2f74  join("<tr>{x}</t
+00002100: 723e 222e 666f 726d 6174 2878 2920 666f  r>".format(x) fo
+00002110: 7220 7820 696e 2074 6162 6c65 290a 0a20  r x in table).. 
+00002120: 2020 2023 2077 7261 7020 6561 6368 2074     # wrap each t
+00002130: 6162 6c65 2069 6e20 3c74 6162 6c65 3e20  able in <table> 
+00002140: 7461 6773 0a20 2020 2074 6162 6c65 7320  tags.    tables 
+00002150: 3d20 2222 2e6a 6f69 6e28 5b27 3c74 6162  = "".join(['<tab
+00002160: 6c65 2062 6f72 6465 723d 2231 223e 7b78  le border="1">{x
+00002170: 7d3c 2f74 6162 6c65 3e27 2e66 6f72 6d61  }</table>'.forma
+00002180: 7428 7829 2066 6f72 2078 2069 6e20 7461  t(x) for x in ta
+00002190: 626c 6573 5d29 0a0a 2020 2020 7265 7475  bles])..    retu
 000021a0: 726e 205b 223c 6874 6d6c 3e3c 626f 6479  rn ["<html><body
 000021b0: 3e22 5d20 2b20 7461 626c 6573 202b 205b  >"] + tables + [
 000021c0: 223c 2f62 6f64 793e 3c2f 6874 6d6c 3e22  "</body></html>"
-000021d0: 5d5c 6e60 6060 5c6e 5c6e 6060 605c 6e3e  ]\n```\n\n```\n>
-000021e0: 3e3e 2074 6162 6c65 7320 3d20 5b5b 5b5b  >> tables = [[[[
-000021f0: 5c27 615c 272c 205c 2762 5c27 5d2c 205b  \'a\', \'b\'], [
-00002200: 5c27 615c 272c 205c 2764 5c27 5d5d 5d5d  \'a\', \'d\']]]]
-00002210: 5c6e 3e3e 3e20 6874 6d6c 5f6d 6170 2874  \n>>> html_map(t
-00002220: 6162 6c65 7329 5c6e 3c68 746d 6c3e 5c6e  ables)\n<html>\n
-00002230: 2020 2020 3c62 6f64 793e 5c6e 2020 2020      <body>\n    
-00002240: 2020 2020 3c74 6162 6c65 2062 6f72 6465      <table borde
-00002250: 723d 2231 223e 5c6e 2020 2020 2020 2020  r="1">\n        
-00002260: 2020 2020 3c74 723e 5c6e 2020 2020 2020      <tr>\n      
-00002270: 2020 2020 2020 2020 2020 3c74 643e 5c6e            <td>\n
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 5c27 2830 2c20 302c 2030 2c20      \'(0, 0, 0, 
-000022a0: 3029 2061 5c27 5c6e 2020 2020 2020 2020  0) a\'\n        
-000022b0: 2020 2020 2020 2020 2020 2020 5c27 2830              \'(0
-000022c0: 2c20 302c 2030 2c20 3129 2062 5c27 5c6e  , 0, 0, 1) b\'\n
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 3c2f 7464 3e5c 6e20 2020 2020 2020 2020  </td>\n         
-000022f0: 2020 2020 2020 203c 7464 3e5c 6e20 2020         <td>\n   
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 205c 2728 302c 2030 2c20 312c 2030 2920   \'(0, 0, 1, 0) 
-00002320: 615c 275c 6e20 2020 2020 2020 2020 2020  a\'\n           
-00002330: 2020 2020 2020 2020 205c 2728 302c 2030           \'(0, 0
-00002340: 2c20 312c 2031 2920 645c 275c 6e20 2020  , 1, 1) d\'\n   
-00002350: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
-00002360: 643e 5c6e 2020 2020 2020 2020 2020 2020  d>\n            
-00002370: 3c2f 7472 3e5c 6e20 2020 2020 2020 203c  </tr>\n        <
-00002380: 2f74 6162 6c65 3e5c 6e20 2020 203c 2f62  /table>\n    </b
-00002390: 6f64 793e 5c6e 3c2f 6874 6d6c 3e5c 6e60  ody>\n</html>\n`
-000023a0: 6060 5c6e 5c6e 5b53 6565 2068 656c 7065  ``\n\n[See helpe
-000023b0: 7220 6675 6e63 7469 6f6e 732e 5d28 6874  r functions.](ht
-000023c0: 7470 733a 2f2f 646f 6378 3270 7974 686f  tps://docx2pytho
-000023d0: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-000023e0: 2f65 6e2f 6c61 7465 7374 2f69 6e64 6578  /en/latest/index
-000023f0: 2e68 746d 6c29 5c6e 5c6e 536f 6d65 2066  .html)\n\nSome f
-00002400: 696e 6520 7072 696e 7420 6162 6f75 7420  ine print about 
-00002410: 6368 6563 6b62 6f78 6573 3a5c 6e5c 6e4d  checkboxes:\n\nM
-00002420: 5320 576f 7264 2068 6173 2063 6865 636b  S Word has check
-00002430: 626f 7865 7320 7468 6174 2063 616e 2062  boxes that can b
-00002440: 6520 6368 6563 6b65 6420 616e 7920 7469  e checked any ti
-00002450: 6d65 2c20 616e 6420 6f74 6865 7273 2074  me, and others t
-00002460: 6861 7420 6361 6e20 6f6e 6c79 2062 6520  hat can only be 
-00002470: 6368 6563 6b65 6420 7768 656e 2074 6865  checked when the
-00002480: 2066 6f72 6d20 6973 206c 6f63 6b65 642e   form is locked.
-00002490: 5c6e 5468 6520 7072 6576 696f 7573 2070  \nThe previous p
-000024a0: 7269 6e74 2061 732e 2060 605c 5c75 3236  rint as. ``\\u26
-000024b0: 3130 6060 2028 6f70 656e 2063 6865 636b  10`` (open check
-000024c0: 626f 7829 206f 7220 6060 5c5c 7532 3631  box) or ``\\u261
-000024d0: 3260 6020 2863 726f 7373 6564 2063 6865  2`` (crossed che
-000024e0: 636b 626f 7829 2e20 5768 6963 6820 7468  ckbox). Which th
-000024f0: 6973 206d 6f64 756c 652c 2074 6865 206c  is module, the l
-00002500: 6174 7465 7220 7769 6c6c 5c6e 746f 6f2e  atter will\ntoo.
-00002510: 2049 2067 6176 6520 6368 6563 6b62 6f78   I gave checkbox
-00002520: 6573 2061 2062 6169 6c6f 7574 2076 616c  es a bailout val
-00002530: 7565 206f 6620 6060 2d2d 2d2d 6368 6563  ue of ``----chec
-00002540: 6b62 6f78 2066 6169 6c65 642d 2d2d 2d60  kbox failed----`
-00002550: 6020 6966 2074 6865 2078 6d6c 2064 6f65  ` if the xml doe
-00002560: 736e 5c27 7420 6c6f 6f6b 206c 696b 6520  sn\'t look like 
-00002570: 4920 6578 7065 6374 2069 7420 746f 2c5c  I expect it to,\
-00002580: 6e62 6563 6175 7365 2049 2064 6f6e 5c27  nbecause I don\'
-00002590: 7420 6861 7665 2073 6576 6572 616c 2d74  t have several-t
-000025a0: 686f 7573 616e 6420 7465 7374 2066 696c  housand test fil
-000025b0: 6573 2077 6974 6820 6368 6563 6b62 6f78  es with checkbox
-000025c0: 6573 2028 6173 2049 2064 6964 2077 6974  es (as I did wit
-000025d0: 6820 6d6f 7374 206f 6620 7468 6520 6f74  h most of the ot
-000025e0: 6865 7220 666f 726d 2065 6c65 6d65 6e74  her form element
-000025f0: 7329 2e5c 6e43 6865 636b 626f 7865 7320  s).\nCheckboxes 
-00002600: 2a73 686f 756c 642a 2077 6f72 6b2c 2062  *should* work, b
-00002610: 7574 2070 6c65 6173 6520 6c65 7420 6d65  ut please let me
-00002620: 206b 6e6f 7720 6966 2079 6f75 2065 6e63   know if you enc
-00002630: 6f75 6e74 6572 2061 6e79 2074 6861 7420  ounter any that 
-00002640: 646f 206e 6f74 2e5c 6e5c 6e23 204e 6577  do not.\n\n# New
-00002650: 2069 6e20 646f 6378 3270 7974 686f 6e20   in docx2python 
-00002660: 5665 7273 696f 6e20 325c 6e5c 6e23 2320  Version 2\n\n## 
-00002670: 6d65 7267 6520 636f 6e73 6563 7574 6976  merge consecutiv
-00002680: 6520 7275 6e73 2077 6974 6820 6964 656e  e runs with iden
-00002690: 7469 6361 6c20 666f 726d 6174 7469 6e67  tical formatting
-000026a0: 5c6e 5c6e 4d53 2057 6f72 6420 7769 6c6c  \n\nMS Word will
-000026b0: 2062 7265 616b 2075 7020 7465 7874 2072   break up text r
-000026c0: 756e 7320 6172 6269 7472 6172 696c 792c  uns arbitrarily,
-000026d0: 206f 6674 656e 2069 6e20 7468 6520 6d69   often in the mi
-000026e0: 6464 6c65 206f 6620 6120 776f 7264 2e5c  ddle of a word.\
-000026f0: 6e5c 6e5c 6e20 2020 203c 773a 723e 5c6e  n\n\n    <w:r>\n
-00002700: 2020 2020 2020 2020 3c77 3a74 3e77 6f72          <w:t>wor
-00002710: 6b20 746f 2069 6d3c 2f77 3a74 3e5c 6e20  k to im</w:t>\n 
-00002720: 2020 203c 2f77 3a72 3e5c 6e20 2020 203c     </w:r>\n    <
-00002730: 773a 723e 5c6e 2020 2020 2020 2020 3c77  w:r>\n        <w
-00002740: 3a74 3e70 726f 7665 2064 6f63 7832 7079  :t>prove docx2py
-00002750: 7468 6f6e 3c2f 773a 743e 5c6e 2020 2020  thon</w:t>\n    
-00002760: 3c2f 773a 723e 5c6e 5c6e 5468 6973 206d  </w:r>\n\nThis m
-00002770: 616b 6573 2074 6869 6e67 7320 6c69 6b65  akes things like
-00002780: 2061 6c67 6f72 6974 686d 6963 2073 6561   algorithmic sea
-00002790: 7263 682d 616e 642d 7265 706c 6163 6520  rch-and-replace 
-000027a0: 7072 6f62 6c65 6d61 7469 632e 2044 6f63  problematic. Doc
-000027b0: 7832 7079 7468 6f6e 2064 6f65 7320 6e6f  x2python does no
-000027c0: 7420 6375 7272 656e 746c 7920 7772 6974  t currently writ
-000027d0: 6520 646f 6378 2066 696c 6573 2c5c 6e62  e docx files,\nb
-000027e0: 7574 2049 206f 6674 656e 2075 7365 2064  ut I often use d
-000027f0: 6f63 7820 7465 6d70 6c61 7465 7320 7769  ocx templates wi
-00002800: 7468 2070 6c61 6365 686f 6c64 6572 7320  th placeholders 
-00002810: 2865 2e67 2e2c 2060 2343 4154 4547 4f52  (e.g., `#CATEGOR
-00002820: 595f 4e41 4d45 2360 2920 7468 656e 2072  Y_NAME#`) then r
-00002830: 6570 6c61 6365 2074 686f 7365 2070 6c61  eplace those pla
-00002840: 6365 686f 6c64 6572 7320 7769 7468 2064  ceholders with d
-00002850: 6174 612e 5c6e 5468 6973 2077 6f6e 5c27  ata.\nThis won\'
-00002860: 7420 776f 726b 2069 6620 796f 7572 2070  t work if your p
-00002870: 6c61 6365 686f 6c64 6572 7320 6172 6520  laceholders are 
-00002880: 6272 6f6b 656e 2075 7020 2865 2e67 2c20  broken up (e.g, 
-00002890: 6023 4341 5460 2c20 6045 602c 2060 474f  `#CAT`, `E`, `GO
-000028a0: 5259 5f4e 414d 4523 6029 2e5c 6e5c 6e44  RY_NAME#`).\n\nD
-000028b0: 6f63 7832 7079 7468 6f6e 2076 3120 6d65  ocx2python v1 me
-000028c0: 7267 6573 2073 7563 6820 7275 6e73 2074  rges such runs t
-000028d0: 6f67 6574 6865 7220 7768 656e 2065 7870  ogether when exp
-000028e0: 6f72 7469 6e67 2074 6578 742e 2044 6f63  orting text. Doc
-000028f0: 7832 7079 7468 6f6e 2076 3220 7769 6c6c  x2python v2 will
-00002900: 206d 6572 6765 2073 7563 6820 7275 6e73   merge such runs
-00002910: 2069 6e20 7468 6520 584d 4c20 6173 2061   in the XML as a
-00002920: 5c6e 7072 652d 7072 6f63 6573 7369 6e67  \npre-processing
-00002930: 2073 7465 702e 2054 6869 7320 7769 6c6c   step. This will
-00002940: 2061 6c6c 6f77 2073 6176 696e 6720 7375   allow saving su
-00002950: 6368 2022 7265 7061 6972 6564 2220 584d  ch "repaired" XM
-00002960: 4c20 6c61 7465 7220 6f6e 2e5c 6e5c 6e23  L later on.\n\n#
-00002970: 2320 6d65 7267 6520 636f 6e73 6563 7574  # merge consecut
-00002980: 6976 6520 6c69 6e6b 7320 7769 7468 2069  ive links with i
-00002990: 6465 6e74 6963 616c 2068 7265 6673 5c6e  dentical hrefs\n
-000029a0: 5c6e 4d53 2057 6f72 6420 7769 6c6c 2062  \nMS Word will b
-000029b0: 7265 616b 2075 7020 6c69 6e6b 732c 2067  reak up links, g
-000029c0: 6976 696e 6720 6561 6368 206c 696e 6b20  iving each link 
-000029d0: 6120 6469 6666 6572 656e 7420 6072 4964  a different `rId
-000029e0: 602c 2065 7665 6e20 7768 656e 2074 6865  `, even when the
-000029f0: 7365 2060 7249 6473 6020 706f 696e 7420  se `rIds` point 
-00002a00: 746f 2074 6865 2073 616d 6520 6164 6472  to the same addr
-00002a10: 6573 732e 5c6e 5c6e 2020 2020 3c77 3a68  ess.\n\n    <w:h
-00002a20: 7970 6572 6c69 6e6b 2072 3a69 643d 2272  yperlink r:id="r
-00002a30: 4964 3133 223e 2020 2320 7249 4431 3320  Id13">  # rID13 
-00002a40: 706f 696e 7473 2074 6f20 6874 7470 733a  points to https:
-00002a50: 2f2f 6769 7468 7562 2e63 6f6d 2f53 6861  //github.com/Sha
-00002a60: 7948 696c 6c2f 646f 6378 3270 7974 686f  yHill/docx2pytho
-00002a70: 6e5c 6e20 2020 2020 2020 203c 773a 723e  n\n        <w:r>
-00002a80: 5c6e 2020 2020 2020 2020 2020 2020 3c77  \n            <w
-00002a90: 3a74 3e64 6f63 7832 7079 3c2f 773a 743e  :t>docx2py</w:t>
-00002aa0: 5c6e 2020 2020 2020 2020 3c2f 773a 723e  \n        </w:r>
-00002ab0: 5c6e 2020 2020 3c2f 773a 6879 7065 726c  \n    </w:hyperl
-00002ac0: 696e 6b3e 5c6e 2020 2020 3c77 3a68 7970  ink>\n    <w:hyp
-00002ad0: 6572 6c69 6e6b 2072 3a69 643d 2272 4964  erlink r:id="rId
-00002ae0: 3134 223e 2020 2320 7249 4431 3420 414c  14">  # rID14 AL
-00002af0: 534f 2070 6f69 6e74 7320 746f 2068 7474  SO points to htt
-00002b00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002b10: 5368 6179 4869 6c6c 2f64 6f63 7832 7079  ShayHill/docx2py
-00002b20: 7468 6f6e 5c6e 2020 2020 2020 2020 3c77  thon\n        <w
-00002b30: 3a72 3e5c 6e20 2020 2020 2020 2020 2020  :r>\n           
-00002b40: 203c 773a 743e 7468 6f6e 3c2f 773a 743e   <w:t>thon</w:t>
-00002b50: 5c6e 2020 2020 2020 2020 3c2f 773a 723e  \n        </w:r>
-00002b60: 5c6e 2020 2020 3c2f 773a 6879 7065 726c  \n    </w:hyperl
-00002b70: 696e 6b3e 5c6e 5c6e 5468 6973 2069 7320  ink>\n\nThis is 
-00002b80: 7369 6d69 6c61 7220 746f 2074 6865 2062  similar to the b
-00002b90: 726f 6b65 6e2d 7570 2072 756e 732c 2062  roken-up runs, b
-00002ba0: 7574 2074 6865 2063 6175 7365 2069 7320  ut the cause is 
-00002bb0: 6120 6c69 7474 6c65 2064 6565 7065 7220  a little deeper 
-00002bc0: 696e 2e20 446f 6378 3270 7974 686f 6e20  in. Docx2python 
-00002bd0: 7631 206d 616b 6573 2061 206d 6573 7320  v1 makes a mess 
-00002be0: 6f66 2074 6865 7365 2e5c 6e5c 6e20 2020  of these.\n\n   
-00002bf0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00002c00: 2f2f 6769 7468 7562 2e63 6f6d 2f53 6861  //github.com/Sha
-00002c10: 7948 696c 6c2f 646f 6378 3270 7974 686f  yHill/docx2pytho
-00002c20: 6e22 3e64 6f63 7832 7079 3c2f 613e 5c6e  n">docx2py</a>\n
-00002c30: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00002c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002c50: 5368 6179 4869 6c6c 2f64 6f63 7832 7079  ShayHill/docx2py
-00002c60: 7468 6f6e 223e 7468 6f6e 3c2f 613e 5c6e  thon">thon</a>\n
-00002c70: 5c6e 446f 6378 3270 7974 686f 6e20 7632  \nDocx2python v2
-00002c80: 2077 696c 6c20 6d65 7267 6520 7375 6368   will merge such
-00002c90: 206c 696e 6b73 2074 6f67 6574 6865 7220   links together 
-00002ca0: 696e 2074 6865 2058 4d4c 2061 7320 6120  in the XML as a 
-00002cb0: 7072 652d 7072 6f63 6573 7369 6e67 2073  pre-processing s
-00002cc0: 7465 702e 2041 7320 6162 6f76 652c 2074  tep. As above, t
-00002cd0: 6869 7320 7769 6c6c 2061 6c6c 6f77 2073  his will allow s
-00002ce0: 6176 696e 675c 6e73 7563 6820 2272 6570  aving\nsuch "rep
-00002cf0: 6169 7265 6422 2058 4d4c 206c 6174 6572  aired" XML later
-00002d00: 206f 6e2e 5c6e 5c6e 2323 2063 6f72 7265   on.\n\n## corre
-00002d10: 6374 6c79 2068 616e 646c 6520 6e65 7374  ctly handle nest
-00002d20: 6564 2070 6172 6167 7261 7068 735c 6e5c  ed paragraphs\n\
-00002d30: 6e4d 5320 576f 7264 2077 696c 6c20 6e65  nMS Word will ne
-00002d40: 7374 2070 6172 6167 7261 7068 735c 6e5c  st paragraphs\n\
-00002d50: 6e20 2020 203c 773a 703e 5c6e 2020 2020  n    <w:p>\n    
-00002d60: 2020 2020 3c77 3a72 3e5c 6e20 2020 2020      <w:r>\n     
-00002d70: 2020 2020 2020 203c 773a 743e 7465 7874         <w:t>text
-00002d80: 3c2f 773a 743e 5c6e 2020 2020 2020 2020  </w:t>\n        
-00002d90: 3c2f 773a 723e 5c6e 2020 2020 2020 2020  </w:r>\n        
-00002da0: 3c77 3a70 3e20 2023 2070 6172 6167 7261  <w:p>  # paragra
-00002db0: 7068 2069 6e73 6964 6520 6120 7061 7261  ph inside a para
-00002dc0: 6772 6170 685c 6e20 2020 2020 2020 2020  graph\n         
-00002dd0: 2020 203c 773a 723e 5c6e 2020 2020 2020     <w:r>\n      
-00002de0: 2020 2020 2020 2020 2020 3c77 3a74 3e74            <w:t>t
-00002df0: 6578 743c 2f77 3a74 3e5c 6e20 2020 2020  ext</w:t>\n     
-00002e00: 2020 2020 2020 203c 2f77 3a72 3e5c 6e20         </w:r>\n 
-00002e10: 2020 2020 2020 203c 2f77 3a70 3e5c 6e20         </w:p>\n 
-00002e20: 2020 2020 2020 203c 773a 723e 5c6e 2020         <w:r>\n  
-00002e30: 2020 2020 2020 2020 2020 3c77 3a74 3e74            <w:t>t
-00002e40: 6578 743c 2f77 3a74 3e5c 6e20 2020 2020  ext</w:t>\n     
-00002e50: 2020 203c 2f77 3a72 3e5c 6e20 2020 203c     </w:r>\n    <
-00002e60: 2f77 3a70 3e5c 6e5c 6e49 2068 6176 656e  /w:p>\n\nI haven
-00002e70: 5c27 7420 6265 656e 2061 626c 6520 746f  \'t been able to
-00002e80: 2063 7265 6174 6520 7375 6368 2061 2070   create such a p
-00002e90: 6172 6167 7261 7068 2c20 6275 7420 495c  aragraph, but I\
-00002ea0: 2776 6520 666f 756e 6420 6120 6665 7720  've found a few 
-00002eb0: 6669 6c65 7320 7468 6174 2068 6176 6520  files that have 
-00002ec0: 7468 656d 2e20 446f 6378 3270 7968 6f6e  them. Docx2pyhon
-00002ed0: 2076 3120 7769 6c6c 206f 6d69 745c 6e63   v1 will omit\nc
-00002ee0: 6c6f 7369 6e67 2068 746d 6c20 7461 6773  losing html tags
-00002ef0: 2077 6865 6e20 6120 6e65 7720 7061 7261   when a new para
-00002f00: 6772 6170 6820 6973 206f 7065 6e65 6420  graph is opened 
-00002f10: 6265 666f 7265 2074 6865 206f 6c64 2070  before the old p
-00002f20: 6172 6167 7261 7068 2069 7320 636c 6f73  aragraph is clos
-00002f30: 6564 2e5c 6e5c 6e20 2020 203c 623e 6f75  ed.\n\n    <b>ou
-00002f40: 7465 7220 7061 7220 626f 6c64 2074 6578  ter par bold tex
-00002f50: 745c 6e5c 6e20 2020 203c 693e 5468 6973  t\n\n    <i>This
-00002f60: 2074 6578 7420 6973 2069 6e20 6e65 7374   text is in nest
-00002f70: 6564 2070 6172 2028 6e6f 7420 626f 6c64  ed par (not bold
-00002f80: 293c 2f69 3e5c 6e5c 6e20 2020 206f 7574  )</i>\n\n    out
-00002f90: 6572 2070 6172 2062 6f6c 6420 7465 7874  er par bold text
-00002fa0: 3c2f 623e 5c6e 5c6e 446f 6378 3270 7974  </b>\n\nDocx2pyt
-00002fb0: 686f 6e20 7632 2077 696c 6c20 636f 7272  hon v2 will corr
-00002fc0: 6563 746c 7920 6861 6e64 6c65 2073 7563  ectly handle suc
-00002fd0: 6820 6361 7365 732c 2062 7574 2074 6869  h cases, but thi
-00002fe0: 7320 7769 6c6c 2072 6571 7569 7265 2073  s will require s
-00002ff0: 7562 7374 616e 7469 616c 2069 6e74 6572  ubstantial inter
-00003000: 6e61 6c20 6368 616e 6765 7320 746f 2074  nal changes to t
-00003010: 6865 2077 6179 5c6e 646f 6378 3270 7974  he way\ndocx2pyt
-00003020: 686f 6e20 6f70 656e 7320 616e 6420 636c  hon opens and cl
-00003030: 6f73 6573 2070 6172 6167 7261 7068 732e  oses paragraphs.
-00003040: 5c6e 5c6e 2020 2020 3c62 3e6f 7574 6572  \n\n    <b>outer
-00003050: 2070 6172 2062 6f6c 6420 7465 7874 3c2f   par bold text</
-00003060: 623e 5c6e 5c6e 2020 2020 3c69 3e54 6869  b>\n\n    <i>Thi
-00003070: 7320 7465 7874 2069 7320 696e 206e 6573  s text is in nes
-00003080: 7465 6420 7061 7220 286e 6f74 2062 6f6c  ted par (not bol
-00003090: 6429 3c2f 693e 5c6e 5c6e 2020 2020 3c2f  d)</i>\n\n    </
-000030a0: 623e 6f75 7465 7220 7061 7220 626f 6c64  b>outer par bold
-000030b0: 2074 6578 743c 2f62 3e5c 6e5c 6e23 2320   text</b>\n\n## 
-000030c0: 7061 7261 6772 6170 6820 7374 796c 6573  paragraph styles
-000030d0: 5c6e 5c6e 5468 6520 696e 7465 726e 616c  \n\nThe internal
-000030e0: 2063 6861 6e67 6573 2061 6c6c 6f77 2066   changes allow f
-000030f0: 6f72 2065 6173 7920 6163 6365 7373 2074  or easy access t
-00003100: 6f20 7061 7261 6772 6170 6820 7374 796c  o paragraph styl
-00003110: 6573 2028 652e 672e 2c20 6048 6561 6469  es (e.g., `Headi
-00003120: 6e67 2031 6029 2e20 446f 6378 3270 7974  ng 1`). Docx2pyt
-00003130: 686f 6e20 7631 2069 676e 6f72 6573 2074  hon v1 ignores t
-00003140: 6865 7365 2c20 6576 656e 5c6e 7769 7468  hese, even\nwith
-00003150: 2060 6874 6d6c 3d54 7275 6560 2e20 446f   `html=True`. Do
-00003160: 6378 3270 7974 686f 6e20 7632 2077 696c  cx2python v2 wil
-00003170: 6c20 6361 7074 7572 6520 7061 7261 6772  l capture paragr
-00003180: 6170 6820 7374 796c 6573 2e5c 6e5c 6e20  aph styles.\n\n 
-00003190: 2020 203c 6831 3e68 3120 6973 2061 2070     <h1>h1 is a p
-000031a0: 6172 6167 7261 7068 2073 7479 6c65 3c62  aragraph style<b
-000031b0: 3e62 6f6c 6420 6973 2061 2072 756e 2073  >bold is a run s
-000031c0: 7479 6c65 3c2f 623e 3c2f 6831 3e5c 6e5c  tyle</b></h1>\n\
-000031d0: 6e23 2320 6578 706f 7274 2078 6d6c 5c6e  n## export xml\n
-000031e0: 5c6e 546f 2061 6c6c 6f77 2061 626f 7665  \nTo allow above
-000031f0: 2d64 6573 6372 6962 6564 206c 6967 6874  -described light
-00003200: 2065 6469 7469 6e67 2028 652e 672e 2c20   editing (e.g., 
-00003210: 7365 6172 6368 2061 6e64 2072 6570 6c61  search and repla
-00003220: 6365 292c 2064 6f63 7832 7079 7468 6f6e  ce), docx2python
-00003230: 2076 3220 7769 6c6c 2067 6976 6520 7468   v2 will give th
-00003240: 6520 7573 6572 2061 6363 6573 7320 746f  e user access to
-00003250: 5c6e 5c6e 2020 2020 312e 2065 7874 7261  \n\n    1. extra
-00003260: 6374 6564 2078 6d6c 2066 696c 6573 5c6e  cted xml files\n
-00003270: 2020 2020 322e 2074 6865 2066 756e 6374      2. the funct
-00003280: 696f 6e73 2075 7365 6420 746f 2077 7269  ions used to wri
-00003290: 7465 2074 6865 7365 2066 696c 6573 2074  te these files t
-000032a0: 6f20 6120 646f 6378 5c6e 5c6e 5468 6520  o a docx\n\nThe 
-000032b0: 7573 6572 2063 616e 206f 6e6c 7920 676f  user can only go
-000032c0: 2073 6f20 6661 7220 7769 7468 2074 6869   so far with thi
-000032d0: 732e 2041 2064 6f63 7820 6669 6c65 2069  s. A docx file i
-000032e0: 7320 6275 696c 7420 6672 6f6d 2066 6f6c  s built from fol
-000032f0: 6465 7273 2066 756c 6c20 6f66 2078 6d6c  ders full of xml
-00003300: 2066 696c 6573 2e20 4e6f 6e65 206f 6620   files. None of 
-00003310: 7468 6573 6520 786d 6c5c 6e66 696c 6573  these xml\nfiles
-00003320: 2061 7265 2073 656c 6620 636f 6e74 6169   are self contai
-00003330: 6e65 642e 2042 7574 2073 6561 7263 6820  ned. But search 
-00003340: 616e 6420 7265 706c 6163 6520 6973 2065  and replace is e
-00003350: 6e6f 7567 6820 746f 206d 616b 6520 646f  nough to make do
-00003360: 6375 6d65 6e74 2074 656d 706c 6174 6573  cument templates
-00003370: 2028 646f 6375 6d65 6e74 7320 7769 7468   (documents with
-00003380: 2070 6c61 6365 686f 6c64 6572 7320 666f   placeholders fo
-00003390: 725c 6e64 6174 6129 2c20 616e 6420 7468  r\ndata), and th
-000033a0: 6174 5c27 7320 7072 6574 7479 2075 7365  at\'s pretty use
-000033b0: 6675 6c20 696e 2069 7473 656c 662e 5c6e  ful in itself.\n
-000033c0: 5c6e 2323 2065 7870 6f73 6520 736f 6d65  \n## expose some
-000033d0: 2069 6e74 6572 6d65 6469 6174 6520 6675   intermediate fu
-000033e0: 6e63 7469 6f6e 616c 6974 795c 6e5c 6e4e  nctionality\n\nN
-000033f0: 6176 6967 6174 696e 6720 7468 726f 7567  avigating throug
-00003400: 6820 584d 4c20 6973 2073 7472 6169 6768  h XML is straigh
-00003410: 7466 6f72 7761 7264 2077 6974 6820 606c  tforward with `l
-00003420: 786d 6c60 2e20 4974 2069 7320 6120 7365  xml`. It is a se
-00003430: 7061 7261 7465 2073 7465 7020 746f 2074  parate step to t
-00003440: 616b 6520 7768 6174 6576 6572 2079 6f75  ake whatever you
-00003450: 2066 696e 6420 616e 6420 6272 696e 6720   find and bring 
-00003460: 6974 5c6e 2a6f 7574 2a20 6f66 2074 6865  it\n*out* of the
-00003470: 2058 4d4c 2e20 466f 7220 696e 7374 616e   XML. For instan
-00003480: 6365 2c20 796f 7520 6d61 7920 7761 6e74  ce, you may want
-00003490: 2074 6f20 6974 6572 6174 6520 6f76 6572   to iterate over
-000034a0: 2061 2064 6f63 756d 656e 742c 206c 6f6f   a document, loo
-000034b0: 6b69 6e67 2066 6f72 2070 6172 6167 7261  king for paragra
-000034c0: 7068 7320 7769 7468 2061 2070 6172 7469  phs with a parti
-000034d0: 6375 6c61 725c 6e66 6f72 6d61 742c 2074  cular\nformat, t
-000034e0: 6865 6e20 7075 6c6c 2074 6865 2074 6578  hen pull the tex
-000034f0: 7420 6f75 7420 6f66 2074 686f 7365 2070  t out of those p
-00003500: 6172 6167 7261 7068 732e 2044 6f63 7832  aragraphs. Docx2
-00003510: 7079 7468 6f6e 2076 3120 6469 6420 6e6f  python v1 did no
-00003520: 7420 7365 7061 7261 7465 206f 7220 6578  t separate or ex
-00003530: 706f 7365 2022 6974 6572 2074 6865 2064  pose "iter the d
-00003540: 6f63 756d 656e 7422 2061 6e64 5c6e 2270  ocument" and\n"p
-00003550: 756c 6c20 7468 6520 636f 6e74 656e 7422  ull the content"
-00003560: 2e20 446f 6378 3270 7974 686f 6e20 7632  . Docx2python v2
-00003570: 2073 6570 6172 6174 6573 2061 6e64 2065   separates and e
-00003580: 7870 6f73 6573 2074 6865 7365 2073 7465  xposes these ste
-00003590: 7073 2e20 5468 6973 2077 696c 6c20 616c  ps. This will al
-000035a0: 6c6f 7720 6561 7369 6572 2065 7874 656e  low easier exten
-000035b0: 7369 6f6e 2e5c 6e5c 6e53 6565 2074 6865  sion.\n\nSee the
-000035c0: 2060 646f 6378 5f72 6561 6465 722e 7079   `docx_reader.py
-000035d0: 6020 6d6f 6475 6c65 2061 6e64 2073 696d  ` module and sim
-000035e0: 706c 6520 6578 616d 706c 6573 2069 6e20  ple examples in 
-000035f0: 7468 6520 6075 7469 6c69 7469 6573 2e70  the `utilities.p
-00003600: 7960 206d 6f64 756c 652e 5c6e 5c6e 2323  y` module.\n\n##
-00003610: 2073 6565 2075 7469 6c69 7469 6573 2e70   see utilities.p
-00003620: 7920 666f 7220 6578 616d 706c 6573 206f  y for examples o
-00003630: 6620 6d61 6a6f 7220 6e65 7720 6665 6174  f major new feat
-00003640: 7572 6573 2e5c 6e27 2c0a 2020 2020 2761  ures.\n',.    'a
-00003650: 7574 686f 7227 3a20 2753 6861 7920 4869  uthor': 'Shay Hi
-00003660: 6c6c 272c 0a20 2020 2027 6175 7468 6f72  ll',.    'author
-00003670: 5f65 6d61 696c 273a 2027 7368 6179 5f70  _email': 'shay_p
-00003680: 7562 6c69 6340 686f 746d 6169 6c2e 636f  ublic@hotmail.co
-00003690: 6d27 2c0a 2020 2020 276d 6169 6e74 6169  m',.    'maintai
-000036a0: 6e65 7227 3a20 274e 6f6e 6527 2c0a 2020  ner': 'None',.  
-000036b0: 2020 276d 6169 6e74 6169 6e65 725f 656d    'maintainer_em
-000036c0: 6169 6c27 3a20 274e 6f6e 6527 2c0a 2020  ail': 'None',.  
-000036d0: 2020 2775 726c 273a 2027 4e6f 6e65 272c    'url': 'None',
-000036e0: 0a20 2020 2027 7061 636b 6167 6573 273a  .    'packages':
-000036f0: 2070 6163 6b61 6765 732c 0a20 2020 2027   packages,.    '
-00003700: 7061 636b 6167 655f 6461 7461 273a 2070  package_data': p
-00003710: 6163 6b61 6765 5f64 6174 612c 0a20 2020  ackage_data,.   
-00003720: 2027 696e 7374 616c 6c5f 7265 7175 6972   'install_requir
-00003730: 6573 273a 2069 6e73 7461 6c6c 5f72 6571  es': install_req
-00003740: 7569 7265 732c 0a20 2020 2027 7079 7468  uires,.    'pyth
-00003750: 6f6e 5f72 6571 7569 7265 7327 3a20 273e  on_requires': '>
-00003760: 3d33 2e38 2c3c 342e 3027 2c0a 7d0a 0a0a  =3.8,<4.0',.}...
-00003770: 7365 7475 7028 2a2a 7365 7475 705f 6b77  setup(**setup_kw
-00003780: 6172 6773 290a                           args).
+000021d0: 5d0a 6060 600a 0a60 6060 0a3e 3e3e 2074  ].```..```.>>> t
+000021e0: 6162 6c65 7320 3d20 5b5b 5b5b 2761 272c  ables = [[[['a',
+000021f0: 2027 6227 5d2c 205b 2761 272c 2027 6427   'b'], ['a', 'd'
+00002200: 5d5d 5d5d 0a3e 3e3e 2068 746d 6c5f 6d61  ]]]].>>> html_ma
+00002210: 7028 7461 626c 6573 290a 3c68 746d 6c3e  p(tables).<html>
+00002220: 0a20 2020 203c 626f 6479 3e0a 2020 2020  .    <body>.    
+00002230: 2020 2020 3c74 6162 6c65 2062 6f72 6465      <table borde
+00002240: 723d 2231 223e 0a20 2020 2020 2020 2020  r="1">.         
+00002250: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+00002260: 2020 2020 2020 2020 3c74 643e 0a20 2020          <td>.   
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2027 2830 2c20 302c 2030 2c20 3029 2061   '(0, 0, 0, 0) a
+00002290: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+000022a0: 2020 2020 2020 2728 302c 2030 2c20 302c        '(0, 0, 0,
+000022b0: 2031 2920 6227 0a20 2020 2020 2020 2020   1) b'.         
+000022c0: 2020 2020 2020 203c 2f74 643e 0a20 2020         </td>.   
+000022d0: 2020 2020 2020 2020 2020 2020 203c 7464               <td
+000022e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000022f0: 2020 2020 2020 2728 302c 2030 2c20 312c        '(0, 0, 1,
+00002300: 2030 2920 6127 0a20 2020 2020 2020 2020   0) a'.         
+00002310: 2020 2020 2020 2020 2020 2027 2830 2c20             '(0, 
+00002320: 302c 2031 2c20 3129 2064 270a 2020 2020  0, 1, 1) d'.    
+00002330: 2020 2020 2020 2020 2020 2020 3c2f 7464              </td
+00002340: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00002350: 7472 3e0a 2020 2020 2020 2020 3c2f 7461  tr>.        </ta
+00002360: 626c 653e 0a20 2020 203c 2f62 6f64 793e  ble>.    </body>
+00002370: 0a3c 2f68 746d 6c3e 0a60 6060 0a0a 5b53  .</html>.```..[S
+00002380: 6565 2068 656c 7065 7220 6675 6e63 7469  ee helper functi
+00002390: 6f6e 732e 5d28 6874 7470 733a 2f2f 646f  ons.](https://do
+000023a0: 6378 3270 7974 686f 6e2e 7265 6164 7468  cx2python.readth
+000023b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000023c0: 7374 2f69 6e64 6578 2e68 746d 6c29 0a0a  st/index.html)..
+000023d0: 536f 6d65 2066 696e 6520 7072 696e 7420  Some fine print 
+000023e0: 6162 6f75 7420 6368 6563 6b62 6f78 6573  about checkboxes
+000023f0: 3a0a 0a4d 5320 576f 7264 2068 6173 2063  :..MS Word has c
+00002400: 6865 636b 626f 7865 7320 7468 6174 2063  heckboxes that c
+00002410: 616e 2062 6520 6368 6563 6b65 6420 616e  an be checked an
+00002420: 7920 7469 6d65 2c20 616e 6420 6f74 6865  y time, and othe
+00002430: 7273 2074 6861 7420 6361 6e20 6f6e 6c79  rs that can only
+00002440: 2062 6520 6368 6563 6b65 6420 7768 656e   be checked when
+00002450: 2074 6865 2066 6f72 6d20 6973 206c 6f63   the form is loc
+00002460: 6b65 642e 0a54 6865 2070 7265 7669 6f75  ked..The previou
+00002470: 7320 7072 696e 7420 6173 2e20 6060 5c75  s print as. ``\u
+00002480: 3236 3130 6060 2028 6f70 656e 2063 6865  2610`` (open che
+00002490: 636b 626f 7829 206f 7220 6060 5c75 3236  ckbox) or ``\u26
+000024a0: 3132 6060 2028 6372 6f73 7365 6420 6368  12`` (crossed ch
+000024b0: 6563 6b62 6f78 292e 2057 6869 6368 2074  eckbox). Which t
+000024c0: 6869 7320 6d6f 6475 6c65 2c20 7468 6520  his module, the 
+000024d0: 6c61 7474 6572 2077 696c 6c0a 746f 6f2e  latter will.too.
+000024e0: 2049 2067 6176 6520 6368 6563 6b62 6f78   I gave checkbox
+000024f0: 6573 2061 2062 6169 6c6f 7574 2076 616c  es a bailout val
+00002500: 7565 206f 6620 6060 2d2d 2d2d 6368 6563  ue of ``----chec
+00002510: 6b62 6f78 2066 6169 6c65 642d 2d2d 2d60  kbox failed----`
+00002520: 6020 6966 2074 6865 2078 6d6c 2064 6f65  ` if the xml doe
+00002530: 736e 2774 206c 6f6f 6b20 6c69 6b65 2049  sn't look like I
+00002540: 2065 7870 6563 7420 6974 2074 6f2c 0a62   expect it to,.b
+00002550: 6563 6175 7365 2049 2064 6f6e 2774 2068  ecause I don't h
+00002560: 6176 6520 7365 7665 7261 6c2d 7468 6f75  ave several-thou
+00002570: 7361 6e64 2074 6573 7420 6669 6c65 7320  sand test files 
+00002580: 7769 7468 2063 6865 636b 626f 7865 7320  with checkboxes 
+00002590: 2861 7320 4920 6469 6420 7769 7468 206d  (as I did with m
+000025a0: 6f73 7420 6f66 2074 6865 206f 7468 6572  ost of the other
+000025b0: 2066 6f72 6d20 656c 656d 656e 7473 292e   form elements).
+000025c0: 0a43 6865 636b 626f 7865 7320 2a73 686f  .Checkboxes *sho
+000025d0: 756c 642a 2077 6f72 6b2c 2062 7574 2070  uld* work, but p
+000025e0: 6c65 6173 6520 6c65 7420 6d65 206b 6e6f  lease let me kno
+000025f0: 7720 6966 2079 6f75 2065 6e63 6f75 6e74  w if you encount
+00002600: 6572 2061 6e79 2074 6861 7420 646f 206e  er any that do n
+00002610: 6f74 2e0a 0a23 204e 6577 2069 6e20 646f  ot...# New in do
+00002620: 6378 3270 7974 686f 6e20 5665 7273 696f  cx2python Versio
+00002630: 6e20 320a 0a23 2320 6d65 7267 6520 636f  n 2..## merge co
+00002640: 6e73 6563 7574 6976 6520 7275 6e73 2077  nsecutive runs w
+00002650: 6974 6820 6964 656e 7469 6361 6c20 666f  ith identical fo
+00002660: 726d 6174 7469 6e67 0a0a 4d53 2057 6f72  rmatting..MS Wor
+00002670: 6420 7769 6c6c 2062 7265 616b 2075 7020  d will break up 
+00002680: 7465 7874 2072 756e 7320 6172 6269 7472  text runs arbitr
+00002690: 6172 696c 792c 206f 6674 656e 2069 6e20  arily, often in 
+000026a0: 7468 6520 6d69 6464 6c65 206f 6620 6120  the middle of a 
+000026b0: 776f 7264 2e0a 0a0a 2020 2020 3c77 3a72  word....    <w:r
+000026c0: 3e0a 2020 2020 2020 2020 3c77 3a74 3e77  >.        <w:t>w
+000026d0: 6f72 6b20 746f 2069 6d3c 2f77 3a74 3e0a  ork to im</w:t>.
+000026e0: 2020 2020 3c2f 773a 723e 0a20 2020 203c      </w:r>.    <
+000026f0: 773a 723e 0a20 2020 2020 2020 203c 773a  w:r>.        <w:
+00002700: 743e 7072 6f76 6520 646f 6378 3270 7974  t>prove docx2pyt
+00002710: 686f 6e3c 2f77 3a74 3e0a 2020 2020 3c2f  hon</w:t>.    </
+00002720: 773a 723e 0a0a 5468 6973 206d 616b 6573  w:r>..This makes
+00002730: 2074 6869 6e67 7320 6c69 6b65 2061 6c67   things like alg
+00002740: 6f72 6974 686d 6963 2073 6561 7263 682d  orithmic search-
+00002750: 616e 642d 7265 706c 6163 6520 7072 6f62  and-replace prob
+00002760: 6c65 6d61 7469 632e 2044 6f63 7832 7079  lematic. Docx2py
+00002770: 7468 6f6e 2064 6f65 7320 6e6f 7420 6375  thon does not cu
+00002780: 7272 656e 746c 7920 7772 6974 6520 646f  rrently write do
+00002790: 6378 2066 696c 6573 2c0a 6275 7420 4920  cx files,.but I 
+000027a0: 6f66 7465 6e20 7573 6520 646f 6378 2074  often use docx t
+000027b0: 656d 706c 6174 6573 2077 6974 6820 706c  emplates with pl
+000027c0: 6163 6568 6f6c 6465 7273 2028 652e 672e  aceholders (e.g.
+000027d0: 2c20 6023 4341 5445 474f 5259 5f4e 414d  , `#CATEGORY_NAM
+000027e0: 4523 6029 2074 6865 6e20 7265 706c 6163  E#`) then replac
+000027f0: 6520 7468 6f73 6520 706c 6163 6568 6f6c  e those placehol
+00002800: 6465 7273 2077 6974 6820 6461 7461 2e0a  ders with data..
+00002810: 5468 6973 2077 6f6e 2774 2077 6f72 6b20  This won't work 
+00002820: 6966 2079 6f75 7220 706c 6163 6568 6f6c  if your placehol
+00002830: 6465 7273 2061 7265 2062 726f 6b65 6e20  ders are broken 
+00002840: 7570 2028 652e 672c 2060 2343 4154 602c  up (e.g, `#CAT`,
+00002850: 2060 4560 2c20 6047 4f52 595f 4e41 4d45   `E`, `GORY_NAME
+00002860: 2360 292e 0a0a 446f 6378 3270 7974 686f  #`)...Docx2pytho
+00002870: 6e20 7631 206d 6572 6765 7320 7375 6368  n v1 merges such
+00002880: 2072 756e 7320 746f 6765 7468 6572 2077   runs together w
+00002890: 6865 6e20 6578 706f 7274 696e 6720 7465  hen exporting te
+000028a0: 7874 2e20 446f 6378 3270 7974 686f 6e20  xt. Docx2python 
+000028b0: 7632 2077 696c 6c20 6d65 7267 6520 7375  v2 will merge su
+000028c0: 6368 2072 756e 7320 696e 2074 6865 2058  ch runs in the X
+000028d0: 4d4c 2061 7320 610a 7072 652d 7072 6f63  ML as a.pre-proc
+000028e0: 6573 7369 6e67 2073 7465 702e 2054 6869  essing step. Thi
+000028f0: 7320 7769 6c6c 2061 6c6c 6f77 2073 6176  s will allow sav
+00002900: 696e 6720 7375 6368 2022 7265 7061 6972  ing such "repair
+00002910: 6564 2220 584d 4c20 6c61 7465 7220 6f6e  ed" XML later on
+00002920: 2e0a 0a23 2320 6d65 7267 6520 636f 6e73  ...## merge cons
+00002930: 6563 7574 6976 6520 6c69 6e6b 7320 7769  ecutive links wi
+00002940: 7468 2069 6465 6e74 6963 616c 2068 7265  th identical hre
+00002950: 6673 0a0a 4d53 2057 6f72 6420 7769 6c6c  fs..MS Word will
+00002960: 2062 7265 616b 2075 7020 6c69 6e6b 732c   break up links,
+00002970: 2067 6976 696e 6720 6561 6368 206c 696e   giving each lin
+00002980: 6b20 6120 6469 6666 6572 656e 7420 6072  k a different `r
+00002990: 4964 602c 2065 7665 6e20 7768 656e 2074  Id`, even when t
+000029a0: 6865 7365 2060 7249 6473 6020 706f 696e  hese `rIds` poin
+000029b0: 7420 746f 2074 6865 2073 616d 6520 6164  t to the same ad
+000029c0: 6472 6573 732e 0a0a 2020 2020 3c77 3a68  dress...    <w:h
+000029d0: 7970 6572 6c69 6e6b 2072 3a69 643d 2272  yperlink r:id="r
+000029e0: 4964 3133 223e 2020 2320 7249 4431 3320  Id13">  # rID13 
+000029f0: 706f 696e 7473 2074 6f20 6874 7470 733a  points to https:
+00002a00: 2f2f 6769 7468 7562 2e63 6f6d 2f53 6861  //github.com/Sha
+00002a10: 7948 696c 6c2f 646f 6378 3270 7974 686f  yHill/docx2pytho
+00002a20: 6e0a 2020 2020 2020 2020 3c77 3a72 3e0a  n.        <w:r>.
+00002a30: 2020 2020 2020 2020 2020 2020 3c77 3a74              <w:t
+00002a40: 3e64 6f63 7832 7079 3c2f 773a 743e 0a20  >docx2py</w:t>. 
+00002a50: 2020 2020 2020 203c 2f77 3a72 3e0a 2020         </w:r>.  
+00002a60: 2020 3c2f 773a 6879 7065 726c 696e 6b3e    </w:hyperlink>
+00002a70: 0a20 2020 203c 773a 6879 7065 726c 696e  .    <w:hyperlin
+00002a80: 6b20 723a 6964 3d22 7249 6431 3422 3e20  k r:id="rId14"> 
+00002a90: 2023 2072 4944 3134 2041 4c53 4f20 706f   # rID14 ALSO po
+00002aa0: 696e 7473 2074 6f20 6874 7470 733a 2f2f  ints to https://
+00002ab0: 6769 7468 7562 2e63 6f6d 2f53 6861 7948  github.com/ShayH
+00002ac0: 696c 6c2f 646f 6378 3270 7974 686f 6e0a  ill/docx2python.
+00002ad0: 2020 2020 2020 2020 3c77 3a72 3e0a 2020          <w:r>.  
+00002ae0: 2020 2020 2020 2020 2020 3c77 3a74 3e74            <w:t>t
+00002af0: 686f 6e3c 2f77 3a74 3e0a 2020 2020 2020  hon</w:t>.      
+00002b00: 2020 3c2f 773a 723e 0a20 2020 203c 2f77    </w:r>.    </w
+00002b10: 3a68 7970 6572 6c69 6e6b 3e0a 0a54 6869  :hyperlink>..Thi
+00002b20: 7320 6973 2073 696d 696c 6172 2074 6f20  s is similar to 
+00002b30: 7468 6520 6272 6f6b 656e 2d75 7020 7275  the broken-up ru
+00002b40: 6e73 2c20 6275 7420 7468 6520 6361 7573  ns, but the caus
+00002b50: 6520 6973 2061 206c 6974 746c 6520 6465  e is a little de
+00002b60: 6570 6572 2069 6e2e 2044 6f63 7832 7079  eper in. Docx2py
+00002b70: 7468 6f6e 2076 3120 6d61 6b65 7320 6120  thon v1 makes a 
+00002b80: 6d65 7373 206f 6620 7468 6573 652e 0a0a  mess of these...
+00002b90: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00002ba0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002bb0: 5368 6179 4869 6c6c 2f64 6f63 7832 7079  ShayHill/docx2py
+00002bc0: 7468 6f6e 223e 646f 6378 3270 793c 2f61  thon">docx2py</a
+00002bd0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00002be0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002bf0: 6d2f 5368 6179 4869 6c6c 2f64 6f63 7832  m/ShayHill/docx2
+00002c00: 7079 7468 6f6e 223e 7468 6f6e 3c2f 613e  python">thon</a>
+00002c10: 0a0a 446f 6378 3270 7974 686f 6e20 7632  ..Docx2python v2
+00002c20: 2077 696c 6c20 6d65 7267 6520 7375 6368   will merge such
+00002c30: 206c 696e 6b73 2074 6f67 6574 6865 7220   links together 
+00002c40: 696e 2074 6865 2058 4d4c 2061 7320 6120  in the XML as a 
+00002c50: 7072 652d 7072 6f63 6573 7369 6e67 2073  pre-processing s
+00002c60: 7465 702e 2041 7320 6162 6f76 652c 2074  tep. As above, t
+00002c70: 6869 7320 7769 6c6c 2061 6c6c 6f77 2073  his will allow s
+00002c80: 6176 696e 670a 7375 6368 2022 7265 7061  aving.such "repa
+00002c90: 6972 6564 2220 584d 4c20 6c61 7465 7220  ired" XML later 
+00002ca0: 6f6e 2e0a 0a23 2320 636f 7272 6563 746c  on...## correctl
+00002cb0: 7920 6861 6e64 6c65 206e 6573 7465 6420  y handle nested 
+00002cc0: 7061 7261 6772 6170 6873 0a0a 4d53 2057  paragraphs..MS W
+00002cd0: 6f72 6420 7769 6c6c 206e 6573 7420 7061  ord will nest pa
+00002ce0: 7261 6772 6170 6873 0a0a 2020 2020 3c77  ragraphs..    <w
+00002cf0: 3a70 3e0a 2020 2020 2020 2020 3c77 3a72  :p>.        <w:r
+00002d00: 3e0a 2020 2020 2020 2020 2020 2020 3c77  >.            <w
+00002d10: 3a74 3e74 6578 743c 2f77 3a74 3e0a 2020  :t>text</w:t>.  
+00002d20: 2020 2020 2020 3c2f 773a 723e 0a20 2020        </w:r>.   
+00002d30: 2020 2020 203c 773a 703e 2020 2320 7061       <w:p>  # pa
+00002d40: 7261 6772 6170 6820 696e 7369 6465 2061  ragraph inside a
+00002d50: 2070 6172 6167 7261 7068 0a20 2020 2020   paragraph.     
+00002d60: 2020 2020 2020 203c 773a 723e 0a20 2020         <w:r>.   
+00002d70: 2020 2020 2020 2020 2020 2020 203c 773a               <w:
+00002d80: 743e 7465 7874 3c2f 773a 743e 0a20 2020  t>text</w:t>.   
+00002d90: 2020 2020 2020 2020 203c 2f77 3a72 3e0a           </w:r>.
+00002da0: 2020 2020 2020 2020 3c2f 773a 703e 0a20          </w:p>. 
+00002db0: 2020 2020 2020 203c 773a 723e 0a20 2020         <w:r>.   
+00002dc0: 2020 2020 2020 2020 203c 773a 743e 7465           <w:t>te
+00002dd0: 7874 3c2f 773a 743e 0a20 2020 2020 2020  xt</w:t>.       
+00002de0: 203c 2f77 3a72 3e0a 2020 2020 3c2f 773a   </w:r>.    </w:
+00002df0: 703e 0a0a 4920 6861 7665 6e27 7420 6265  p>..I haven't be
+00002e00: 656e 2061 626c 6520 746f 2063 7265 6174  en able to creat
+00002e10: 6520 7375 6368 2061 2070 6172 6167 7261  e such a paragra
+00002e20: 7068 2c20 6275 7420 4927 7665 2066 6f75  ph, but I've fou
+00002e30: 6e64 2061 2066 6577 2066 696c 6573 2074  nd a few files t
+00002e40: 6861 7420 6861 7665 2074 6865 6d2e 2044  hat have them. D
+00002e50: 6f63 7832 7079 686f 6e20 7631 2077 696c  ocx2pyhon v1 wil
+00002e60: 6c20 6f6d 6974 0a63 6c6f 7369 6e67 2068  l omit.closing h
+00002e70: 746d 6c20 7461 6773 2077 6865 6e20 6120  tml tags when a 
+00002e80: 6e65 7720 7061 7261 6772 6170 6820 6973  new paragraph is
+00002e90: 206f 7065 6e65 6420 6265 666f 7265 2074   opened before t
+00002ea0: 6865 206f 6c64 2070 6172 6167 7261 7068  he old paragraph
+00002eb0: 2069 7320 636c 6f73 6564 2e0a 0a20 2020   is closed...   
+00002ec0: 203c 623e 6f75 7465 7220 7061 7220 626f   <b>outer par bo
+00002ed0: 6c64 2074 6578 740a 0a20 2020 203c 693e  ld text..    <i>
+00002ee0: 5468 6973 2074 6578 7420 6973 2069 6e20  This text is in 
+00002ef0: 6e65 7374 6564 2070 6172 2028 6e6f 7420  nested par (not 
+00002f00: 626f 6c64 293c 2f69 3e0a 0a20 2020 206f  bold)</i>..    o
+00002f10: 7574 6572 2070 6172 2062 6f6c 6420 7465  uter par bold te
+00002f20: 7874 3c2f 623e 0a0a 446f 6378 3270 7974  xt</b>..Docx2pyt
+00002f30: 686f 6e20 7632 2077 696c 6c20 636f 7272  hon v2 will corr
+00002f40: 6563 746c 7920 6861 6e64 6c65 2073 7563  ectly handle suc
+00002f50: 6820 6361 7365 732c 2062 7574 2074 6869  h cases, but thi
+00002f60: 7320 7769 6c6c 2072 6571 7569 7265 2073  s will require s
+00002f70: 7562 7374 616e 7469 616c 2069 6e74 6572  ubstantial inter
+00002f80: 6e61 6c20 6368 616e 6765 7320 746f 2074  nal changes to t
+00002f90: 6865 2077 6179 0a64 6f63 7832 7079 7468  he way.docx2pyth
+00002fa0: 6f6e 206f 7065 6e73 2061 6e64 2063 6c6f  on opens and clo
+00002fb0: 7365 7320 7061 7261 6772 6170 6873 2e0a  ses paragraphs..
+00002fc0: 0a20 2020 203c 623e 6f75 7465 7220 7061  .    <b>outer pa
+00002fd0: 7220 626f 6c64 2074 6578 743c 2f62 3e0a  r bold text</b>.
+00002fe0: 0a20 2020 203c 693e 5468 6973 2074 6578  .    <i>This tex
+00002ff0: 7420 6973 2069 6e20 6e65 7374 6564 2070  t is in nested p
+00003000: 6172 2028 6e6f 7420 626f 6c64 293c 2f69  ar (not bold)</i
+00003010: 3e0a 0a20 2020 203c 2f62 3e6f 7574 6572  >..    </b>outer
+00003020: 2070 6172 2062 6f6c 6420 7465 7874 3c2f   par bold text</
+00003030: 623e 0a0a 2323 2070 6172 6167 7261 7068  b>..## paragraph
+00003040: 2073 7479 6c65 730a 0a54 6865 2069 6e74   styles..The int
+00003050: 6572 6e61 6c20 6368 616e 6765 7320 616c  ernal changes al
+00003060: 6c6f 7720 666f 7220 6561 7379 2061 6363  low for easy acc
+00003070: 6573 7320 746f 2070 6172 6167 7261 7068  ess to paragraph
+00003080: 2073 7479 6c65 7320 2865 2e67 2e2c 2060   styles (e.g., `
+00003090: 4865 6164 696e 6720 3160 292e 2044 6f63  Heading 1`). Doc
+000030a0: 7832 7079 7468 6f6e 2076 3120 6967 6e6f  x2python v1 igno
+000030b0: 7265 7320 7468 6573 652c 2065 7665 6e0a  res these, even.
+000030c0: 7769 7468 2060 6874 6d6c 3d54 7275 6560  with `html=True`
+000030d0: 2e20 446f 6378 3270 7974 686f 6e20 7632  . Docx2python v2
+000030e0: 2077 696c 6c20 6361 7074 7572 6520 7061   will capture pa
+000030f0: 7261 6772 6170 6820 7374 796c 6573 2e0a  ragraph styles..
+00003100: 0a20 2020 203c 6831 3e68 3120 6973 2061  .    <h1>h1 is a
+00003110: 2070 6172 6167 7261 7068 2073 7479 6c65   paragraph style
+00003120: 3c62 3e62 6f6c 6420 6973 2061 2072 756e  <b>bold is a run
+00003130: 2073 7479 6c65 3c2f 623e 3c2f 6831 3e0a   style</b></h1>.
+00003140: 0a23 2320 6578 706f 7274 2078 6d6c 0a0a  .## export xml..
+00003150: 546f 2061 6c6c 6f77 2061 626f 7665 2d64  To allow above-d
+00003160: 6573 6372 6962 6564 206c 6967 6874 2065  escribed light e
+00003170: 6469 7469 6e67 2028 652e 672e 2c20 7365  diting (e.g., se
+00003180: 6172 6368 2061 6e64 2072 6570 6c61 6365  arch and replace
+00003190: 292c 2064 6f63 7832 7079 7468 6f6e 2076  ), docx2python v
+000031a0: 3220 7769 6c6c 2067 6976 6520 7468 6520  2 will give the 
+000031b0: 7573 6572 2061 6363 6573 7320 746f 0a0a  user access to..
+000031c0: 2020 2020 312e 2065 7874 7261 6374 6564      1. extracted
+000031d0: 2078 6d6c 2066 696c 6573 0a20 2020 2032   xml files.    2
+000031e0: 2e20 7468 6520 6675 6e63 7469 6f6e 7320  . the functions 
+000031f0: 7573 6564 2074 6f20 7772 6974 6520 7468  used to write th
+00003200: 6573 6520 6669 6c65 7320 746f 2061 2064  ese files to a d
+00003210: 6f63 780a 0a54 6865 2075 7365 7220 6361  ocx..The user ca
+00003220: 6e20 6f6e 6c79 2067 6f20 736f 2066 6172  n only go so far
+00003230: 2077 6974 6820 7468 6973 2e20 4120 646f   with this. A do
+00003240: 6378 2066 696c 6520 6973 2062 7569 6c74  cx file is built
+00003250: 2066 726f 6d20 666f 6c64 6572 7320 6675   from folders fu
+00003260: 6c6c 206f 6620 786d 6c20 6669 6c65 732e  ll of xml files.
+00003270: 204e 6f6e 6520 6f66 2074 6865 7365 2078   None of these x
+00003280: 6d6c 0a66 696c 6573 2061 7265 2073 656c  ml.files are sel
+00003290: 6620 636f 6e74 6169 6e65 642e 2042 7574  f contained. But
+000032a0: 2073 6561 7263 6820 616e 6420 7265 706c   search and repl
+000032b0: 6163 6520 6973 2065 6e6f 7567 6820 746f  ace is enough to
+000032c0: 206d 616b 6520 646f 6375 6d65 6e74 2074   make document t
+000032d0: 656d 706c 6174 6573 2028 646f 6375 6d65  emplates (docume
+000032e0: 6e74 7320 7769 7468 2070 6c61 6365 686f  nts with placeho
+000032f0: 6c64 6572 7320 666f 720a 6461 7461 292c  lders for.data),
+00003300: 2061 6e64 2074 6861 7427 7320 7072 6574   and that's pret
+00003310: 7479 2075 7365 6675 6c20 696e 2069 7473  ty useful in its
+00003320: 656c 662e 0a0a 2323 2065 7870 6f73 6520  elf...## expose 
+00003330: 736f 6d65 2069 6e74 6572 6d65 6469 6174  some intermediat
+00003340: 6520 6675 6e63 7469 6f6e 616c 6974 790a  e functionality.
+00003350: 0a4e 6176 6967 6174 696e 6720 7468 726f  .Navigating thro
+00003360: 7567 6820 584d 4c20 6973 2073 7472 6169  ugh XML is strai
+00003370: 6768 7466 6f72 7761 7264 2077 6974 6820  ghtforward with 
+00003380: 606c 786d 6c60 2e20 4974 2069 7320 6120  `lxml`. It is a 
+00003390: 7365 7061 7261 7465 2073 7465 7020 746f  separate step to
+000033a0: 2074 616b 6520 7768 6174 6576 6572 2079   take whatever y
+000033b0: 6f75 2066 696e 6420 616e 6420 6272 696e  ou find and brin
+000033c0: 6720 6974 0a2a 6f75 742a 206f 6620 7468  g it.*out* of th
+000033d0: 6520 584d 4c2e 2046 6f72 2069 6e73 7461  e XML. For insta
+000033e0: 6e63 652c 2079 6f75 206d 6179 2077 616e  nce, you may wan
+000033f0: 7420 746f 2069 7465 7261 7465 206f 7665  t to iterate ove
+00003400: 7220 6120 646f 6375 6d65 6e74 2c20 6c6f  r a document, lo
+00003410: 6f6b 696e 6720 666f 7220 7061 7261 6772  oking for paragr
+00003420: 6170 6873 2077 6974 6820 6120 7061 7274  aphs with a part
+00003430: 6963 756c 6172 0a66 6f72 6d61 742c 2074  icular.format, t
+00003440: 6865 6e20 7075 6c6c 2074 6865 2074 6578  hen pull the tex
+00003450: 7420 6f75 7420 6f66 2074 686f 7365 2070  t out of those p
+00003460: 6172 6167 7261 7068 732e 2044 6f63 7832  aragraphs. Docx2
+00003470: 7079 7468 6f6e 2076 3120 6469 6420 6e6f  python v1 did no
+00003480: 7420 7365 7061 7261 7465 206f 7220 6578  t separate or ex
+00003490: 706f 7365 2022 6974 6572 2074 6865 2064  pose "iter the d
+000034a0: 6f63 756d 656e 7422 2061 6e64 0a22 7075  ocument" and."pu
+000034b0: 6c6c 2074 6865 2063 6f6e 7465 6e74 222e  ll the content".
+000034c0: 2044 6f63 7832 7079 7468 6f6e 2076 3220   Docx2python v2 
+000034d0: 7365 7061 7261 7465 7320 616e 6420 6578  separates and ex
+000034e0: 706f 7365 7320 7468 6573 6520 7374 6570  poses these step
+000034f0: 732e 2054 6869 7320 7769 6c6c 2061 6c6c  s. This will all
+00003500: 6f77 2065 6173 6965 7220 6578 7465 6e73  ow easier extens
+00003510: 696f 6e2e 0a0a 5365 6520 7468 6520 6064  ion...See the `d
+00003520: 6f63 785f 7265 6164 6572 2e70 7960 206d  ocx_reader.py` m
+00003530: 6f64 756c 6520 616e 6420 7369 6d70 6c65  odule and simple
+00003540: 2065 7861 6d70 6c65 7320 696e 2074 6865   examples in the
+00003550: 2060 7574 696c 6974 6965 732e 7079 6020   `utilities.py` 
+00003560: 6d6f 6475 6c65 2e0a 0a23 2320 7365 6520  module...## see 
+00003570: 7574 696c 6974 6965 732e 7079 2066 6f72  utilities.py for
+00003580: 2065 7861 6d70 6c65 7320 6f66 206d 616a   examples of maj
+00003590: 6f72 206e 6577 2066 6561 7475 7265 732e  or new features.
+000035a0: 0a0a                                     ..
```


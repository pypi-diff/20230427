# Comparing `tmp/reportlab-3.6.8.tar.gz` & `tmp/reportlab-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-3.6.8.tar", last modified: Mon Feb 28 12:29:49 2022, max compression
+gzip compressed data, was "reportlab-3.6.9.tar", last modified: Fri Mar 25 10:55:02 2022, max compression
```

## Comparing `reportlab-3.6.8.tar` & `reportlab-3.6.9.tar`

### file list

```diff
@@ -1,900 +1,900 @@
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.569640 reportlab-3.6.8/
--rw-r--r--   0 robin     (1000) robin     (1000)    46198 2022-02-28 11:03:17.000000 reportlab-3.6.8/CHANGES.md
--rw-r--r--   0 robin     (1000) robin     (1000)       53 2019-10-12 07:24:05.000000 reportlab-3.6.8/INSTALL.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.8/LICENSE.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      595 2022-02-14 09:12:02.000000 reportlab-3.6.8/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1102 2022-02-28 12:29:49.569640 reportlab-3.6.8/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     7506 2022-02-28 09:25:02.000000 reportlab-3.6.8/README.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       72 2019-10-12 07:24:05.000000 reportlab-3.6.8/VERSION.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.432971 reportlab-3.6.8/demos/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.439638 reportlab-3.6.8/demos/colors/
--rw-r--r--   0 robin     (1000) robin     (1000)     2728 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/colors/colortest.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.439638 reportlab-3.6.8/demos/gadflypaper/
--rw-r--r--   0 robin     (1000) robin     (1000)      105 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/gadflypaper/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    32486 2022-01-24 09:42:51.000000 reportlab-3.6.8/demos/gadflypaper/gfe.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.439638 reportlab-3.6.8/demos/odyssey/
--rw-r--r--   0 robin     (1000) robin     (1000)     2098 2022-02-14 09:12:02.000000 reportlab-3.6.8/demos/odyssey/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     7649 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/odyssey/dodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4580 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/odyssey/fodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4235 2022-02-14 09:12:02.000000 reportlab-3.6.8/demos/odyssey/odyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10950 2020-10-29 09:10:51.000000 reportlab-3.6.8/demos/odyssey/odyssey.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.439638 reportlab-3.6.8/demos/rlzope/
--rw-r--r--   0 robin     (1000) robin     (1000)     2538 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/rlzope/readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     6791 2022-02-16 09:20:12.000000 reportlab-3.6.8/demos/rlzope/rlzope.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.439638 reportlab-3.6.8/demos/stdfonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/stdfonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     2381 2021-06-01 15:46:32.000000 reportlab-3.6.8/demos/stdfonts/stdfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.442971 reportlab-3.6.8/demos/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      525 2019-10-12 07:24:05.000000 reportlab-3.6.8/demos/tests/testdemos.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.442971 reportlab-3.6.8/docs/
--rw-r--r--   0 robin     (1000) robin     (1000)      313 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     3136 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/Makefile
--rwxr-xr-x   0 robin     (1000) robin     (1000)     1497 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/genAll.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)      143 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/gen_epydoc
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.446304 reportlab-3.6.8/docs/images/
--rw-r--r--   0 robin     (1000) robin     (1000)     9685 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/Edit_Prefs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    28106 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/Python_21.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    29117 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/Python_21_HINT.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    37812 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/fileExchange.gif
--rw-r--r--   0 robin     (1000) robin     (1000)   533144 2021-05-05 14:45:00.000000 reportlab-3.6.8/docs/images/jpegrgb_dissected.png
--rw-r--r--   0 robin     (1000) robin     (1000)    10513 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/jpn.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33898 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/jpnchars.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)      393 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/redsquare.png
--rw-r--r--   0 robin     (1000) robin     (1000)    26548 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/replogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)    16583 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/replogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      924 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/images/testimg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3081 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/make.bat
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.446304 reportlab-3.6.8/docs/reference/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      110 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/reference/build.bat
--rw-r--r--   0 robin     (1000) robin     (1000)     1206 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/reference/genreference.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9927 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/reference/reference.yml
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.446304 reportlab-3.6.8/docs/source/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.446304 reportlab-3.6.8/docs/source/_static/
--rw-r--r--   0 robin     (1000) robin     (1000)      252 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/_static/basic.css
--rw-r--r--   0 robin     (1000) robin     (1000)    16419 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/_static/default.css
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.446304 reportlab-3.6.8/docs/source/_templates/
--rw-r--r--   0 robin     (1000) robin     (1000)      167 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/_templates/layout.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/_templates/page.html
--rw-r--r--   0 robin     (1000) robin     (1000)     6427 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/conf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1345 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/graphics.rst
--rw-r--r--   0 robin     (1000) robin     (1000)     1049 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/index.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      885 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/lib.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      238 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/pdfgen.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      984 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/source/platypus.rst
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.449638 reportlab-3.6.8/docs/userguide/
--rw-r--r--   0 robin     (1000) robin     (1000)     4494 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/app_demos.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17692 2022-02-28 09:22:40.000000 reportlab-3.6.8/docs/userguide/ch1_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45531 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/ch2_graphics.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19934 2022-01-24 09:42:51.000000 reportlab-3.6.8/docs/userguide/ch2a_fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30547 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/ch3_pdffeatures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19315 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/ch4_platypus_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    23044 2022-01-24 09:42:51.000000 reportlab-3.6.8/docs/userguide/ch5_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34555 2022-01-24 09:42:51.000000 reportlab-3.6.8/docs/userguide/ch6_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2643 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/ch7_custom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-02-18 09:22:22.000000 reportlab-3.6.8/docs/userguide/genuserguide.py
--rw-r--r--   0 robin     (1000) robin     (1000)    52769 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/graph_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/graph_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      490 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/graph_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12403 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/graph_shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13522 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/graph_widgets.py
--rw-r--r--   0 robin     (1000) robin     (1000)      112 2019-10-12 07:24:05.000000 reportlab-3.6.8/docs/userguide/testfile.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      254 2022-02-28 12:29:49.569640 reportlab-3.6.8/setup.cfg
--rw-r--r--   0 robin     (1000) robin     (1000)    29139 2022-02-28 09:22:40.000000 reportlab-3.6.8/setup.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.436304 reportlab-3.6.8/src/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.449638 reportlab-3.6.8/src/reportlab/
--rw-r--r--   0 robin     (1000) robin     (1000)      185 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/reportlab/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1320 2022-02-28 11:03:51.000000 reportlab-3.6.8/src/reportlab/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.456304 reportlab-3.6.8/src/reportlab/fonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      318 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      504 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGarden-changelog.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    17976 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGarden-copying-gpl.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1318 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGarden-copying.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     4122 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGarden-readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)   519634 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGarden.sfd
--rw-r--r--   0 robin     (1000) robin     (1000)    10351 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGardenMK.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    79824 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/DarkGardenMK.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    65932 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/Vera.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63208 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/VeraBI.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    58716 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/VeraBd.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63684 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/VeraIt.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    32084 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_a______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    31966 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_ab_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32019 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_abi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32115 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_ai_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35377 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_eb_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    38543 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_ebi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    37518 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_ei_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35380 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/_er_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)     5954 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/fonts/bitstream-vera-license.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     8318 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/callig15.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    59663 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/callig15.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35500 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/cob_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    50532 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/cobo____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34585 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/com_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    48468 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/coo_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34705 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/sy______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    49593 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/zd______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    75573 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/zx______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    96418 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab/fonts/zy______.pfb
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.459638 reportlab-3.6.8/src/reportlab/graphics/
--rw-r--r--   0 robin     (1000) robin     (1000)      274 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.462971 reportlab-3.6.8/src/reportlab/graphics/barcode/
--rw-r--r--   0 robin     (1000) robin     (1000)     1741 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/README
--rw-r--r--   0 robin     (1000) robin     (1000)      915 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/TODO
--rw-r--r--   0 robin     (1000) robin     (1000)     5886 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18451 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/code128.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9799 2022-02-16 08:38:59.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/code39.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9077 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/code93.py
--rw-r--r--   0 robin     (1000) robin     (1000)    23636 2022-02-16 08:38:59.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/common.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7872 2022-02-07 10:01:51.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/dmtx.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18922 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/eanbc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17884 2020-09-29 08:33:07.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/ecc200datamatrix.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3746 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/fourstate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7377 2022-02-16 08:38:59.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/lto.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6266 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/qr.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34117 2022-02-07 10:01:51.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/qrencoder.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11516 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/test.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8076 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/usps.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15554 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/usps4s.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17139 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/barcode/widgets.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.466305 reportlab-3.6.8/src/reportlab/graphics/charts/
--rw-r--r--   0 robin     (1000) robin     (1000)      234 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/charts/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4405 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/areas.py
--rw-r--r--   0 robin     (1000) robin     (1000)    91512 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/axes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    72283 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/barcharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6628 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/dotbox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18834 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/doughnut.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25533 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/legends.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27178 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/linecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    49394 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/lineplots.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1739 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    66610 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/piecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8548 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15692 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/spider.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22693 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11556 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7194 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/charts/utils3d.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15155 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/renderPDF.py
--rw-r--r--   0 robin     (1000) robin     (1000)    28772 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/graphics/renderPM.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37937 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37686 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12828 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/graphics/renderbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.469638 reportlab-3.6.8/src/reportlab/graphics/samples/
--rw-r--r--   0 robin     (1000) robin     (1000)       69 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/samples/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3584 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/bubble.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4241 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/clustered_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4188 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/clustered_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1947 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/excelcolors.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3126 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/exploded_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2691 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/filled_radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4267 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/line_chart.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5007 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/linechart_with_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3244 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1957 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/runall.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3566 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/scatter.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4164 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/scatter_lines.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/scatter_lines_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2933 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/simple_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4284 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/stacked_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4230 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/samples/stacked_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)    59326 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/graphics/shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9433 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/testdrawings.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17242 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/testshapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1943 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/graphics/transform.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4606 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/graphics/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25552 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgetbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.469638 reportlab-3.6.8/src/reportlab/graphics/widgets/
--rw-r--r--   0 robin     (1000) robin     (1000)      242 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3920 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/adjustableArrow.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13073 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/eventcal.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30233 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/flags.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17504 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8424 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    31655 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/signsandsymbols.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6932 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/graphics/widgets/table.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.472972 reportlab-3.6.8/src/reportlab/lib/
--rw-r--r--   0 robin     (1000) robin     (1000)     4972 2022-01-21 12:16:59.000000 reportlab-3.6.8/src/reportlab/lib/PyFontify.py
--rw-r--r--   0 robin     (1000) robin     (1000)      256 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1122 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/abag.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7272 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/lib/arciv.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5770 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/lib/attrmap.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2927 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/boxstuff.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13051 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/codecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    36654 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27141 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/corp.py
--rw-r--r--   0 robin     (1000) robin     (1000)      296 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/enums.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2226 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/extformat.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13369 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/lib/fontfinder.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3503 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3804 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/formatters.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1163 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1747 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/logger.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22017 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/normalDate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2001 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/pagesizes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30680 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/lib/pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2509 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/pygments2xpre.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22859 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/lib/randomtext.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12606 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37051 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/lib/rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1121 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/rltempfile.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17803 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/rparsexml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9647 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/lib/sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16783 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/lib/styles.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12251 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/lib/testutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9723 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/textsplit.py
--rw-r--r--   0 robin     (1000) robin     (1000)      917 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/units.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45329 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/lib/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11310 2022-02-28 12:17:45.000000 reportlab-3.6.8/src/reportlab/lib/validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5717 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/lib/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/reportlab/license.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.476305 reportlab-3.6.8/src/reportlab/pdfbase/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      275 2020-07-24 11:15:51.000000 reportlab-3.6.8/src/reportlab/pdfbase/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1794 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/_can_cmap_data.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32044 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_cidfontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10141 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2934 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_macroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2308 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1829 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_standard.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3187 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_winansi.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2222 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courier.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3367 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3672 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3668 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3665 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3667 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2732 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)   108467 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/pdfbase/_glyphlist.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45680 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/acroform.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18821 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/cidfonts.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    90151 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/pdfbase/pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15704 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/pdfform.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    29935 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3763 2022-02-07 10:01:51.000000 reportlab-3.6.8/src/reportlab/pdfbase/pdfpattern.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    10135 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfbase/pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    56426 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/pdfbase/rl_codecs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    53122 2022-02-16 09:20:12.000000 reportlab-3.6.8/src/reportlab/pdfbase/ttfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.479638 reportlab-3.6.8/src/reportlab/pdfgen/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      270 2020-07-24 11:15:51.000000 reportlab-3.6.8/src/reportlab/pdfgen/__init__.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    81667 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/pdfgen/canvas.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5737 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/pdfgen/pathobject.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     2980 2020-07-24 11:15:51.000000 reportlab-3.6.8/src/reportlab/pdfgen/pdfgeom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8269 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/pdfgen/pdfimages.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    19531 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/pdfgen/textobject.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.479638 reportlab-3.6.8/src/reportlab/platypus/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      502 2020-07-24 11:15:51.000000 reportlab-3.6.8/src/reportlab/platypus/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    54601 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/platypus/doctemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18313 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/platypus/figures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    95657 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/platypus/flowables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11246 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/platypus/frames.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2753 2020-07-24 11:13:36.000000 reportlab-3.6.8/src/reportlab/platypus/multicol.py
--rw-r--r--   0 robin     (1000) robin     (1000)    93001 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/platypus/para.py
--rw-r--r--   0 robin     (1000) robin     (1000)   117624 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/platypus/paragraph.py
--rw-r--r--   0 robin     (1000) robin     (1000)   213795 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/platypus/paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)    21268 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/platypus/tableofcontents.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    80184 2022-02-28 09:13:23.000000 reportlab-3.6.8/src/reportlab/platypus/tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12947 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/reportlab/platypus/xpreformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4411 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/reportlab/rl_config.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14759 2022-02-28 09:22:40.000000 reportlab-3.6.8/src/reportlab/rl_settings.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.449638 reportlab-3.6.8/src/reportlab.egg-info/
--rw-r--r--   0 robin     (1000) robin     (1000)     1102 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab.egg-info/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)    35671 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab.egg-info/SOURCES.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab.egg-info/dependency_links.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       44 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab.egg-info/requires.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       10 2022-02-28 12:29:49.000000 reportlab-3.6.8/src/reportlab.egg-info/top_level.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.482972 reportlab-3.6.8/src/rl_addons/
--rw-r--r--   0 robin     (1000) robin     (1000)      326 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/README
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.482972 reportlab-3.6.8/src/rl_addons/renderPM/
--rw-r--r--   0 robin     (1000) robin     (1000)    59470 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/_renderPM.c
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.482972 reportlab-3.6.8/src/rl_addons/renderPM/gt1/
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-dict.c
--rw-r--r--   0 robin     (1000) robin     (1000)      847 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-dict.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1125 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-misc.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6380 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-namecontext.c
--rw-r--r--   0 robin     (1000) robin     (1000)      796 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-namecontext.h
--rw-r--r--   0 robin     (1000) robin     (1000)    68782 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-parset1.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1115 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-parset1.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2249 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-region.c
--rw-r--r--   0 robin     (1000) robin     (1000)      271 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-region.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1185 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-value.h
--rw-r--r--   0 robin     (1000) robin     (1000)    45589 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/parseAFM.c
--rw-r--r--   0 robin     (1000) robin     (1000)    11656 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/gt1/parseAFM.h
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.499639 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/
--rw-r--r--   0 robin     (1000) robin     (1000)       27 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/AUTHORS
--rw-r--r--   0 robin     (1000) robin     (1000)    25292 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/COPYING
--rw-r--r--   0 robin     (1000) robin     (1000)    41340 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/ChangeLog
--rw-r--r--   0 robin     (1000) robin     (1000)     3608 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/Makefile.am
--rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/NEWS
--rw-r--r--   0 robin     (1000) robin     (1000)      682 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/README
--rw-r--r--   0 robin     (1000) robin     (1000)      455 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/README.CVS
--rw-r--r--   0 robin     (1000) robin     (1000)       30 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/acconfig.h
--rw-r--r--   0 robin     (1000) robin     (1000)    12103 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2656 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2547 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1424 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2470 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_bpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1560 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_bpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)      294 2022-02-28 12:29:48.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_config.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2394 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_filterlevel.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3357 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1338 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2134 2021-01-17 17:34:27.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_misc.c
--rw-r--r--   0 robin     (1000) robin     (1000)     3078 2020-09-16 15:20:01.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_misc.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1131 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pathcode.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9103 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2937 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1110 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_point.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6364 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2303 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2243 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1387 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3927 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1277 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.h
--rw-r--r--   0 robin     (1000) robin     (1000)    35686 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render.c
--rw-r--r--   0 robin     (1000) robin     (1000)     4702 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render.h
--rw-r--r--   0 robin     (1000) robin     (1000)    19265 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2327 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4190 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_mask.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1368 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_mask.h
--rw-r--r--   0 robin     (1000) robin     (1000)    10028 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1357 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4420 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1220 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4548 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1531 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3647 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1487 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3363 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1209 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6151 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1578 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3471 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1570 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4451 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1535 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)    11735 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1581 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6720 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgba.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1391 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgba.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4417 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1736 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)    45995 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1925 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.h
--rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1434 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3404 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_point.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1305 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_point.h
--rw-r--r--   0 robin     (1000) robin     (1000)    13258 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1935 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5575 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1282 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)    21659 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1959 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.h
--rw-r--r--   0 robin     (1000) robin     (1000)    40901 2021-02-08 17:02:15.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1517 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2354 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1926 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3433 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1217 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3464 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1225 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1636 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1289 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9925 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1454 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6178 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1906 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9617 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1447 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5262 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1372 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5064 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1301 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1530 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/autogen.sh
--rw-r--r--   0 robin     (1000) robin     (1000)      696 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/config.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2694 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/configure.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1238 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/gen_art_config.c
--rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-2.0.pc.in
--rw-r--r--   0 robin     (1000) robin     (1000)      976 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-config.in
--rw-r--r--   0 robin     (1000) robin     (1000)      366 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-features.c
--rw-r--r--   0 robin     (1000) robin     (1000)      696 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-features.h.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1351 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6262 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart.m4
--rw-r--r--   0 robin     (1000) robin     (1000)      176 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libartConf.sh.in
--rw-r--r--   0 robin     (1000) robin     (1000)     8530 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/test_gradient.c
--rw-r--r--   0 robin     (1000) robin     (1000)    14315 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/testart.c
--rw-r--r--   0 robin     (1000) robin     (1000)     5652 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/testuta.c
--rw-r--r--   0 robin     (1000) robin     (1000)    24390 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/pfm.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17530 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/test_renderPM.py
--rw-r--r--   0 robin     (1000) robin     (1000)      587 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/renderPM/tr.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.502972 reportlab-3.6.8/src/rl_addons/rl_accel/
--rw-r--r--   0 robin     (1000) robin     (1000)      469 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/README.extensions
--rw-r--r--   0 robin     (1000) robin     (1000)    35650 2022-01-24 09:42:51.000000 reportlab-3.6.8/src/rl_addons/rl_accel/_rl_accel.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/hnjalloc.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1543 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/hnjalloc.h
--rw-r--r--   0 robin     (1000) robin     (1000)    13502 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2130 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.h
--rw-r--r--   0 robin     (1000) robin     (1000)    36457 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.mashed
--rw-r--r--   0 robin     (1000) robin     (1000)     9150 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/pyHnjmodule.c
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.502972 reportlab-3.6.8/src/rl_addons/rl_accel/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      669 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/getrc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1378 2022-02-18 09:22:22.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t0.py
--rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t1.py
--rw-r--r--   0 robin     (1000) robin     (1000)      747 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1875 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1687 2019-10-12 07:24:05.000000 reportlab-3.6.8/src/rl_addons/rl_accel/tests/t5.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.516306 reportlab-3.6.8/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      913 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      540 2021-05-05 14:58:39.000000 reportlab-3.6.8/tests/7x11.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)       99 2021-05-05 14:57:42.000000 reportlab-3.6.8/tests/7x11.png
--rw-r--r--   0 robin     (1000) robin     (1000)       80 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2022-02-28 12:24:36.000000 reportlab-3.6.8/tests/_i_am_actually_a_gif.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2022-02-28 12:24:36.000000 reportlab-3.6.8/tests/_i_am_actually_a_jpeg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3813 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/alpha_test.png
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.519639 reportlab-3.6.8/tests/barcode-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     1098 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/Codabar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1429 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/Code11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1333 2022-02-28 12:24:37.000000 reportlab-3.6.8/tests/barcode-out/Code128.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1454 2022-02-28 12:24:37.000000 reportlab-3.6.8/tests/barcode-out/Code128Auto.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2980 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/EAN13.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1751 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/EAN5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2383 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/EAN8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3091 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/ECC200DataMatrix.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1566 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/Extended39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1919 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/Extended93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1082 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/FIM.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1104 2022-02-28 12:24:37.000000 reportlab-3.6.8/tests/barcode-out/I2of5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3596 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/ISBN.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1128 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/MSI.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1524 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/POSTNET.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2762 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/QR.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3211 2022-02-28 12:24:39.000000 reportlab-3.6.8/tests/barcode-out/QR_with_comma.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1545 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/Standard39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1241 2022-02-28 12:24:37.000000 reportlab-3.6.8/tests/barcode-out/Standard93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2987 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/UPCA.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1590 2022-02-28 12:24:38.000000 reportlab-3.6.8/tests/barcode-out/USPS_4State.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2388 2022-02-28 12:24:39.000000 reportlab-3.6.8/tests/barcode-out/test_cbcim.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2210 2022-02-28 12:24:39.000000 reportlab-3.6.8/tests/barcode-out/test_cbcim.png
--rw-r--r--   0 robin     (1000) robin     (1000)    12180 2022-02-28 12:24:39.000000 reportlab-3.6.8/tests/barcode-out/test_cbcim.tiff
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.552973 reportlab-3.6.8/tests/charts-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     1641 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1506 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1479 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1168 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4006 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3240 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2799 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3742 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2272 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2345 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3630 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2270 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1887 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1846 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2266 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2288 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2328 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3616 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2288 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2270 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2681 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3743 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2679 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3727 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2692 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3734 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2701 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3807 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2758 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2747 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3728 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2734 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3776 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2766 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1729 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1859 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3510 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13857 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6770 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15564 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7108 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15568 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8113 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2619 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample_hatching.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3383 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5299 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3071 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4033 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3120 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2287 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2868 2022-02-28 12:24:43.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5477 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9274 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4218 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7323 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4289 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7447 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4952 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9053 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4741 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6406 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3050 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3287 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4149 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2884 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3669 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2807 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3020 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3887 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5378 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3956 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5381 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3464 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5290 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3459 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5291 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5286 2022-02-28 12:24:44.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3389 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5293 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6675 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    48255 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7857 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46272 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3139 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4036 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3029 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3116 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2291 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5932 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9403 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4468 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7338 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4473 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7450 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5370 2022-02-28 12:24:45.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9105 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6379 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3140 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4004 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3206 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4118 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2891 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3654 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2924 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5412 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4853 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5422 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4426 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5332 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4437 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4602 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4455 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5859 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1492 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6451 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2174 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7297 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7278 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-02-28 12:24:46.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2469 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2843 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2512 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2847 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2078 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2483 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2097 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2508 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3649 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3344 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6052 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13106 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6759 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    14174 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6782 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    62954 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7754 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41220 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2447 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8150 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5435 2022-02-28 12:24:47.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33385 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4772 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10135 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4632 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9133 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6048 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10000 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3585 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7027 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2352 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2420 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4239 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2775 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5724 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3940 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3533 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1272 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4024 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2052 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6870 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5057 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample5.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6126 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample6.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5182 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample6.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16767 2022-02-28 12:24:48.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample7.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    23088 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample7.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9369 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12584 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample8.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10699 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample9.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12623 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample9.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4504 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_bcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7899 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_bcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4376 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_hlcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8690 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_hlcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4678 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_lpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10059 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_lpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3914 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_pcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3805 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_pcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4889 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_plpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6410 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_plpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6996 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8945 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9425 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1barline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8676 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1barline.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4865 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6067 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8486 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12166 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5283 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6357 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1765 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1182 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4283 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample4pie.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7687 2022-02-28 12:24:50.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample4pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6776 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_scleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5397 2022-02-28 12:24:51.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_scleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8883 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4414 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11410 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10045 2022-02-28 12:24:49.000000 reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2979 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/encryption.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1908 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/gray-alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/pythonpowered-gs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/pythonpowered.gif
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.562973 reportlab-3.6.8/tests/render-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     2589 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/410.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1362 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/410.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3229 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing01.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5062 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing01.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2850 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing01.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1020 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing01.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2560 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing02.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5773 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing02.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2739 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing02.png
--rw-r--r--   0 robin     (1000) robin     (1000)      846 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing02.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8923 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing03.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8747 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing03.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    14798 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing03.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1327 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing03.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2369 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing04.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2784 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing04.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2765 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing04.png
--rw-r--r--   0 robin     (1000) robin     (1000)      858 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing04.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3163 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing05.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3729 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing05.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4721 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing05.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1393 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing05.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6353 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing06.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10835 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing06.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12964 2022-02-28 12:24:40.000000 reportlab-3.6.8/tests/render-out/Drawing06.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing06.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3929 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing07.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5433 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing07.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     7028 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing07.png
--rw-r--r--   0 robin     (1000) robin     (1000)     8298 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing07.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3428 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing08.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6355 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing08.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4097 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing08.png
--rw-r--r--   0 robin     (1000) robin     (1000)    10846 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing08.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7990 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing09.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8280 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing09.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    15924 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing09.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1339 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing09.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3154 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing10.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5817 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing10.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing10.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2163 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing10.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2189 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2946 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing11.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     3105 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing11.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7969 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing11.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17038 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing12.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    16031 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing12.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    28701 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing12.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1219 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing12.py
--rw-r--r--   0 robin     (1000) robin     (1000)    40966 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing13.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    51803 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing13.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    72941 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing13.png
--rw-r--r--   0 robin     (1000) robin     (1000)     4246 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing13.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1374 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing14.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2181 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing14.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)      882 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing14.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1064 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/Drawing14.py
--rw-r--r--   0 robin     (1000) robin     (1000)      342 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-none.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1011 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-none.py
--rw-r--r--   0 robin     (1000) robin     (1000)      336 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-pdf.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)      352 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-svg.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/autoclose-svg.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11577 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/fillmode-even-odd.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/fillmode-even-odd.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11621 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/fillmode-non-zero.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/fillmode-non-zero.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14199 2022-02-28 12:24:41.000000 reportlab-3.6.8/tests/render-out/hatch.png
--rw-r--r--   0 robin     (1000) robin     (1000)     6477 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/render-out/hatch.py
--rw-r--r--   0 robin     (1000) robin     (1000)      879 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/render-out/svglib-issue104.png
--rw-r--r--   0 robin     (1000) robin     (1000)    24350 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/render-out/textmode.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2027 2022-02-28 12:24:42.000000 reportlab-3.6.8/tests/render-out/textmode.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6504 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/rltw-icon-tr.png
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5209 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/runAll.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2402 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/solid_red_alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/tall_red.png
--rw-r--r--   0 robin     (1000) robin     (1000)      288 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test-cross.tiff
--rw-r--r--   0 robin     (1000) robin     (1000)      168 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test-indexed.png
--rw-r--r--   0 robin     (1000) robin     (1000)      157 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test-rgba.png
--rw-r--r--   0 robin     (1000) robin     (1000)     9464 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_charts_textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6252 2019-11-23 12:29:07.000000 reportlab-3.6.8/tests/test_crypto_algorithms.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1462 2022-02-14 09:12:02.000000 reportlab-3.6.8/tests/test_docs_build.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6506 2022-02-14 09:12:02.000000 reportlab-3.6.8/tests/test_docstrings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2022-02-14 09:12:02.000000 reportlab-3.6.8/tests/test_extra.py
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14652 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_graphics_barcode.py
--rw-r--r--   0 robin     (1000) robin     (1000)    41317 2022-02-03 15:17:16.000000 reportlab-3.6.8/tests/test_graphics_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32774 2022-02-28 12:25:07.000000 reportlab-3.6.8/tests/test_graphics_images-cairo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46849 2022-02-28 12:25:07.000000 reportlab-3.6.8/tests/test_graphics_images-cairo.png
--rw-r--r--   0 robin     (1000) robin     (1000)    16209 2022-02-28 12:25:06.000000 reportlab-3.6.8/tests/test_graphics_images.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    21349 2022-02-28 12:25:06.000000 reportlab-3.6.8/tests/test_graphics_images.png
--rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_graphics_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2523 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_graphics_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15789 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_graphics_render.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2628 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_graphics_speed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1893 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_hello.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2662 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2511 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_invariant.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4214 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_issues.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8276 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_lib_colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11916 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_lib_normaldate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6062 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_lib_pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6780 2022-02-07 10:01:51.000000 reportlab-3.6.8/tests/test_lib_rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3748 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_lib_sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13278 2022-02-16 09:20:12.000000 reportlab-3.6.8/tests/test_lib_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5592 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_lib_validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2448 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_multibyte_chs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4973 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_multibyte_cht.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25468 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_multibyte_jpn.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6658 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_multibyte_kor.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34098 2022-02-28 09:22:40.000000 reportlab-3.6.8/tests/test_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10715 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfbase_encodings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3875 2020-01-26 19:46:34.000000 reportlab-3.6.8/tests/test_pdfbase_fontembed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2713 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfbase_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18606 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_pdfbase_pdfform.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4120 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_pdfbase_pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1609 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_pdfbase_pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfbase_postscript.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19727 2022-02-16 09:20:12.000000 reportlab-3.6.8/tests/test_pdfbase_ttfonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      989 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfgen_callback.py
--rw-r--r--   0 robin     (1000) robin     (1000)    48259 2022-02-16 09:20:12.000000 reportlab-3.6.8/tests/test_pdfgen_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6925 2021-07-06 13:47:00.000000 reportlab-3.6.8/tests/test_pdfgen_links.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3133 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfgen_overprint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1850 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_pdfgen_pagemodes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3168 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_platypus_accum.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27202 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_breaking.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5973 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_cjk_wrap.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34433 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4226 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8549 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_indents.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5383 2022-02-18 09:22:22.000000 reportlab-3.6.8/tests/test_platypus_index.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6293 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_leftright.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10786 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_lists.py
--rw-r--r--   0 robin     (1000) robin     (1000)   113010 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5094 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_platypus_paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9402 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_pleaseturnover.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8635 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_preformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7373 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_programming.py
--rw-r--r--   0 robin     (1000) robin     (1000)    53423 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12590 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_toc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3773 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_wrapping.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5183 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_platypus_xref.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4762 2022-02-14 09:12:02.000000 reportlab-3.6.8/tests/test_pyfiles.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7690 2022-02-28 09:22:40.000000 reportlab-3.6.8/tests/test_renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9773 2022-02-28 09:22:40.000000 reportlab-3.6.8/tests/test_renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9669 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3423 2022-01-24 09:42:51.000000 reportlab-3.6.8/tests/test_source_chars.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19261 2022-02-28 09:13:23.000000 reportlab-3.6.8/tests/test_table_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1244 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_tools_pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1353 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4890 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_widgetbase_tpc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15476 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/test_widgets_grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.8/tests/unimportable.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.562973 reportlab-3.6.8/tools/
--rw-r--r--   0 robin     (1000) robin     (1000)      193 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/README
--rw-r--r--   0 robin     (1000) robin     (1000)      160 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.566306 reportlab-3.6.8/tools/docco/
--rw-r--r--   0 robin     (1000) robin     (1000)      292 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/docco/README
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/docco/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7791 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/docco/codegrab.py
--rw-r--r--   0 robin     (1000) robin     (1000)    41170 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/docpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    29268 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/docco/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32661 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/graphdocpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13738 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/rl_doc_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5898 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/rltemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6939 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/stylesheet.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9899 2022-02-16 08:38:59.000000 reportlab-3.6.8/tools/docco/t_parse.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7023 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3284 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/docco/yaml2pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1056 2022-02-11 10:12:47.000000 reportlab-3.6.8/tools/pdfpath.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.566306 reportlab-3.6.8/tools/pythonpoint/
--rw-r--r--   0 robin     (1000) robin     (1000)     1099 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/README
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8840 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/customshapes.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.566306 reportlab-3.6.8/tools/pythonpoint/demos/
--rw-r--r--   0 robin     (1000) robin     (1000)    26656 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/figures.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     4859 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/htu.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     3008 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/leftlogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)     2198 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/leftlogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    11730 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/monterey.xml
--rw-r--r--   0 robin     (1000) robin     (1000)    12918 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/outline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3429 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/pplogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)   125666 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/python.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41307 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/pythonpoint.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     1704 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1855 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/spectrum.png
--rw-r--r--   0 robin     (1000) robin     (1000)    20910 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/demos/vertpython.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7920 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/pythonpoint.dtd
--rw-r--r--   0 robin     (1000) robin     (1000)    34726 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)    28933 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/stdparser.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.569640 reportlab-3.6.8/tools/pythonpoint/styles/
--rw-r--r--   0 robin     (1000) robin     (1000)      179 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/styles/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/pythonpoint/styles/horrible.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5079 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/styles/htu.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3692 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/styles/modern.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3215 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/styles/projection.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/pythonpoint/styles/standard.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-02-28 12:29:49.569640 reportlab-3.6.8/tools/utils/
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2022-02-18 09:22:22.000000 reportlab-3.6.8/tools/utils/add_bleed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1891 2019-10-12 07:24:05.000000 reportlab-3.6.8/tools/utils/dumpttf.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/
+-rw-r--r--   0 robin     (1000) robin     (1000)    46400 2022-03-22 08:37:04.000000 reportlab-3.6.9/CHANGES.md
+-rw-r--r--   0 robin     (1000) robin     (1000)       53 2019-10-12 07:24:05.000000 reportlab-3.6.9/INSTALL.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.9/LICENSE.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)      595 2022-03-02 12:17:05.000000 reportlab-3.6.9/MANIFEST.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     1052 2022-03-25 10:55:02.782211 reportlab-3.6.9/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)     7506 2022-03-02 12:17:05.000000 reportlab-3.6.9/README.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)       72 2019-10-12 07:24:05.000000 reportlab-3.6.9/VERSION.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.675542 reportlab-3.6.9/demos/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/colors/
+-rw-r--r--   0 robin     (1000) robin     (1000)     2728 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/colors/colortest.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/gadflypaper/
+-rw-r--r--   0 robin     (1000) robin     (1000)      105 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/gadflypaper/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)    32486 2022-01-24 09:42:51.000000 reportlab-3.6.9/demos/gadflypaper/gfe.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/odyssey/
+-rw-r--r--   0 robin     (1000) robin     (1000)     2098 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/odyssey/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     7649 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/odyssey/dodyssey.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4580 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/odyssey/fodyssey.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4235 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/odyssey/odyssey.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10950 2020-10-29 09:10:51.000000 reportlab-3.6.9/demos/odyssey/odyssey.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/rlzope/
+-rw-r--r--   0 robin     (1000) robin     (1000)     2538 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/rlzope/readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     6791 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/rlzope/rlzope.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/stdfonts/
+-rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/stdfonts/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     2381 2021-06-01 15:46:32.000000 reportlab-3.6.9/demos/stdfonts/stdfonts.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/tests/
+-rw-r--r--   0 robin     (1000) robin     (1000)      525 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/tests/testdemos.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/docs/
+-rw-r--r--   0 robin     (1000) robin     (1000)      313 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     3136 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/Makefile
+-rwxr-xr-x   0 robin     (1000) robin     (1000)     1497 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/genAll.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      143 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/gen_epydoc
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/docs/images/
+-rw-r--r--   0 robin     (1000) robin     (1000)     9685 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Edit_Prefs.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    28106 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Python_21.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    29117 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Python_21_HINT.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    37812 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/fileExchange.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)   533144 2021-05-05 14:45:00.000000 reportlab-3.6.9/docs/images/jpegrgb_dissected.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    10513 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/jpn.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    33898 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/jpnchars.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/lj8100.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)      393 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/redsquare.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    26548 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/replogo.a85
+-rw-r--r--   0 robin     (1000) robin     (1000)    16583 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/replogo.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)      924 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/testimg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3081 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/make.bat
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/reference/
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      110 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/build.bat
+-rw-r--r--   0 robin     (1000) robin     (1000)     1206 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/genreference.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9927 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/reference.yml
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/_static/
+-rw-r--r--   0 robin     (1000) robin     (1000)      252 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_static/basic.css
+-rw-r--r--   0 robin     (1000) robin     (1000)    16419 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_static/default.css
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/_templates/
+-rw-r--r--   0 robin     (1000) robin     (1000)      167 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_templates/layout.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_templates/page.html
+-rw-r--r--   0 robin     (1000) robin     (1000)     6427 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/conf.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1345 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/graphics.rst
+-rw-r--r--   0 robin     (1000) robin     (1000)     1049 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/index.rst
+-rw-r--r--   0 robin     (1000) robin     (1000)      885 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/lib.rst
+-rw-r--r--   0 robin     (1000) robin     (1000)      238 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/pdfgen.rst
+-rw-r--r--   0 robin     (1000) robin     (1000)      984 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/platypus.rst
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/docs/userguide/
+-rw-r--r--   0 robin     (1000) robin     (1000)     4494 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/app_demos.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17692 2022-03-02 12:17:05.000000 reportlab-3.6.9/docs/userguide/ch1_intro.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    45531 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch2_graphics.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    19934 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch2a_fonts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    30547 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch3_pdffeatures.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    19315 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch4_platypus_concepts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    23044 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch5_paragraphs.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    34555 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch6_tables.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2643 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch7_custom.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-03-02 12:17:05.000000 reportlab-3.6.9/docs/userguide/genuserguide.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    52769 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_charts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_concepts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      490 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_intro.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12403 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_shapes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13522 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_widgets.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      112 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/testfile.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)      254 2022-03-25 10:55:02.782211 reportlab-3.6.9/setup.cfg
+-rw-r--r--   0 robin     (1000) robin     (1000)    31084 2022-03-22 12:49:38.000000 reportlab-3.6.9/setup.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/src/
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/src/reportlab/
+-rw-r--r--   0 robin     (1000) robin     (1000)      185 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/MANIFEST.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     1320 2022-03-22 08:57:03.000000 reportlab-3.6.9/src/reportlab/__init__.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.692209 reportlab-3.6.9/src/reportlab/fonts/
+-rw-r--r--   0 robin     (1000) robin     (1000)      318 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)      504 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-changelog.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)    17976 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     1318 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     4122 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)   519634 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden.sfd
+-rw-r--r--   0 robin     (1000) robin     (1000)    10351 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.afm
+-rw-r--r--   0 robin     (1000) robin     (1000)    79824 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    65932 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/Vera.ttf
+-rw-r--r--   0 robin     (1000) robin     (1000)    63208 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraBI.ttf
+-rw-r--r--   0 robin     (1000) robin     (1000)    58716 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraBd.ttf
+-rw-r--r--   0 robin     (1000) robin     (1000)    63684 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraIt.ttf
+-rw-r--r--   0 robin     (1000) robin     (1000)    32084 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_a______.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    31966 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ab_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    32019 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_abi____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    32115 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ai_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    35377 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_eb_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    38543 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ebi____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    37518 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ei_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    35380 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_er_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)     5954 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/bitstream-vera-license.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)     8318 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/callig15.afm
+-rw-r--r--   0 robin     (1000) robin     (1000)    59663 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/callig15.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    35500 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/cob_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    50532 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/cobo____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    34585 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/com_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    48468 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/coo_____.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    34705 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/sy______.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    49593 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zd______.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    75573 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zx______.pfb
+-rw-r--r--   0 robin     (1000) robin     (1000)    96418 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zy______.pfb
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.695542 reportlab-3.6.9/src/reportlab/graphics/
+-rw-r--r--   0 robin     (1000) robin     (1000)      274 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/__init__.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.695542 reportlab-3.6.9/src/reportlab/graphics/barcode/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1741 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/README
+-rw-r--r--   0 robin     (1000) robin     (1000)      915 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/TODO
+-rw-r--r--   0 robin     (1000) robin     (1000)     5886 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18451 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code128.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9799 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code39.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9077 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code93.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    23636 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/common.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7872 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/dmtx.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18922 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/eanbc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17884 2020-09-29 08:33:07.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/ecc200datamatrix.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3746 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/fourstate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7377 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/lto.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6266 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/qr.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    34117 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/qrencoder.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11516 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/test.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8076 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/usps.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15554 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/usps4s.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17139 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/widgets.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.698876 reportlab-3.6.9/src/reportlab/graphics/charts/
+-rw-r--r--   0 robin     (1000) robin     (1000)      234 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/charts/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4405 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/areas.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    91512 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/axes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    72283 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/barcharts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6628 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/dotbox.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18834 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/doughnut.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    25533 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/legends.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    27178 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/linecharts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    49394 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/lineplots.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1739 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/markers.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    66610 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/piecharts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8548 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/slidebox.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15692 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/spider.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    22693 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/textlabels.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11556 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7194 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/utils3d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15155 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPDF.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    28772 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPM.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    37937 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPS.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    37686 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderSVG.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12828 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/renderbase.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.702209 reportlab-3.6.9/src/reportlab/graphics/samples/
+-rw-r--r--   0 robin     (1000) robin     (1000)       69 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/samples/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3584 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/bubble.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4241 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/clustered_bar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4188 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/clustered_column.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1947 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/excelcolors.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3126 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/exploded_pie.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2691 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/filled_radar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4267 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/line_chart.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5007 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/linechart_with_markers.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3244 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/radar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1957 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/runall.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3566 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4164 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines_markers.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2933 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/simple_pie.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4284 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/stacked_bar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4230 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/stacked_column.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    59326 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/shapes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9433 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/testdrawings.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17242 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/testshapes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1943 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/transform.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4606 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    25552 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgetbase.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.702209 reportlab-3.6.9/src/reportlab/graphics/widgets/
+-rw-r--r--   0 robin     (1000) robin     (1000)      242 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3920 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/adjustableArrow.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13073 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/eventcal.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    30233 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/flags.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17504 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/grids.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8424 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/markers.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    31655 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/signsandsymbols.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6932 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/table.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.705543 reportlab-3.6.9/src/reportlab/lib/
+-rw-r--r--   0 robin     (1000) robin     (1000)     4972 2022-01-21 12:16:59.000000 reportlab-3.6.9/src/reportlab/lib/PyFontify.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      256 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1122 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/abag.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7272 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/arciv.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5770 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/attrmap.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2927 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/boxstuff.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13051 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/codecharts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    36654 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/colors.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    27141 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/corp.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      296 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/enums.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2226 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/extformat.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13369 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/fontfinder.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3503 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/fonts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3804 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/formatters.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1163 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/geomutils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1747 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/logger.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    22017 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/normalDate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2001 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/pagesizes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    30680 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/pdfencrypt.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2509 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/pygments2xpre.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    22859 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/randomtext.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12606 2022-03-21 15:35:15.000000 reportlab-3.6.9/src/reportlab/lib/rl_accel.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    37051 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/rl_safe_eval.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1121 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/rltempfile.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17803 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/rparsexml.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9647 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/sequencer.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    16783 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/styles.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12251 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/testutils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9723 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/textsplit.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      917 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/units.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    45361 2022-03-02 12:17:06.000000 reportlab-3.6.9/src/reportlab/lib/utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11310 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/validators.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5717 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/yaml.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/license.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.708876 reportlab-3.6.9/src/reportlab/pdfbase/
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      275 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfbase/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1794 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/_can_cmap_data.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    32044 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_cidfontdata.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10141 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3058 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2934 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2308 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1829 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_standard.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3187 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3003 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2222 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courier.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3367 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3672 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3668 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3665 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3667 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2732 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
+-rw-r--r--   0 robin     (1000) robin     (1000)   108467 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_glyphlist.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    45680 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/acroform.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18821 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/cidfonts.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    90151 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfdoc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15704 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfform.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    29935 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfmetrics.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3763 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfpattern.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    10135 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfutils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    56426 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/pdfbase/rl_codecs.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    53122 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/ttfonts.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/reportlab/pdfgen/
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      270 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/__init__.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    81667 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/canvas.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)     5737 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/pathobject.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)     2980 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/pdfgeom.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8269 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/pdfimages.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    19531 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/textobject.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/reportlab/platypus/
+-rwxr-xr-x   0 robin     (1000) robin     (1000)      502 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/platypus/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    54601 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/platypus/doctemplate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18313 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/platypus/figures.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    95657 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/flowables.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11246 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/frames.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2753 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/platypus/multicol.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    93001 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/platypus/para.py
+-rw-r--r--   0 robin     (1000) robin     (1000)   117624 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/paragraph.py
+-rw-r--r--   0 robin     (1000) robin     (1000)   213795 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/paraparser.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    21268 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/tableofcontents.py
+-rwxr-xr-x   0 robin     (1000) robin     (1000)    80184 2022-03-22 08:49:11.000000 reportlab-3.6.9/src/reportlab/platypus/tables.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12947 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/xpreformatted.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4411 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/rl_config.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    14759 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/rl_settings.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/src/reportlab.egg-info/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1052 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)    35671 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/SOURCES.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        1 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/dependency_links.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)       44 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/requires.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)       10 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/top_level.txt
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/rl_addons/
+-rw-r--r--   0 robin     (1000) robin     (1000)      326 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/README
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.715543 reportlab-3.6.9/src/rl_addons/renderPM/
+-rw-r--r--   0 robin     (1000) robin     (1000)    59470 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/_renderPM.c
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.715543 reportlab-3.6.9/src/rl_addons/renderPM/gt1/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.c
+-rw-r--r--   0 robin     (1000) robin     (1000)      847 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1125 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-misc.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6380 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.c
+-rw-r--r--   0 robin     (1000) robin     (1000)      796 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    68782 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1115 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2249 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-region.c
+-rw-r--r--   0 robin     (1000) robin     (1000)      271 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-region.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1185 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-value.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    45589 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.c
+-rw-r--r--   0 robin     (1000) robin     (1000)    11656 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.h
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.725543 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/
+-rw-r--r--   0 robin     (1000) robin     (1000)       27 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/AUTHORS
+-rw-r--r--   0 robin     (1000) robin     (1000)    25292 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/COPYING
+-rw-r--r--   0 robin     (1000) robin     (1000)    41340 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/ChangeLog
+-rw-r--r--   0 robin     (1000) robin     (1000)     3608 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/Makefile.am
+-rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/NEWS
+-rw-r--r--   0 robin     (1000) robin     (1000)      682 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/README
+-rw-r--r--   0 robin     (1000) robin     (1000)      455 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/README.CVS
+-rw-r--r--   0 robin     (1000) robin     (1000)       30 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/acconfig.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    12103 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     2656 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2547 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1424 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2470 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1560 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.h
+-rw-r--r--   0 robin     (1000) robin     (1000)      294 2022-03-25 10:55:00.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_config.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2394 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_filterlevel.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3357 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1338 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2134 2021-01-17 17:34:27.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     3078 2020-09-16 15:20:01.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1131 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pathcode.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     9103 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     2937 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1110 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_point.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6364 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     2303 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2243 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1387 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3927 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1277 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    35686 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     4702 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    19265 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     2327 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     4190 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1368 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    10028 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1357 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     4420 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1220 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     4548 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1531 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3647 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1487 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3363 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1209 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6151 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1578 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3471 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1570 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     4451 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1535 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    11735 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1581 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6720 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1391 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     4417 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1736 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    45995 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1925 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1434 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3404 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1305 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    13258 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1935 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     5575 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1282 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    21659 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1959 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    40901 2021-02-08 17:02:15.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1517 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2354 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1926 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3433 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1217 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     3464 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1225 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1636 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1289 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     9925 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1454 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6178 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1906 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     9617 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1447 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     5262 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1372 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     5064 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1301 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     1530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/autogen.sh
+-rw-r--r--   0 robin     (1000) robin     (1000)      696 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/config.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     2694 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/configure.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     1238 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/gen_art_config.c
+-rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-2.0.pc.in
+-rw-r--r--   0 robin     (1000) robin     (1000)      976 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-config.in
+-rw-r--r--   0 robin     (1000) robin     (1000)      366 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-features.c
+-rw-r--r--   0 robin     (1000) robin     (1000)      696 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-features.h.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     1351 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.h
+-rw-r--r--   0 robin     (1000) robin     (1000)     6262 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.m4
+-rw-r--r--   0 robin     (1000) robin     (1000)      176 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libartConf.sh.in
+-rw-r--r--   0 robin     (1000) robin     (1000)     8530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/test_gradient.c
+-rw-r--r--   0 robin     (1000) robin     (1000)    14315 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testart.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     5652 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testuta.c
+-rw-r--r--   0 robin     (1000) robin     (1000)    24390 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/pfm.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/test_renderPM.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      587 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/tr.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.728876 reportlab-3.6.9/src/rl_addons/rl_accel/
+-rw-r--r--   0 robin     (1000) robin     (1000)      469 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/README.extensions
+-rw-r--r--   0 robin     (1000) robin     (1000)    39181 2022-03-25 08:39:56.000000 reportlab-3.6.9/src/rl_addons/rl_accel/_rl_accel.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     1543 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    13502 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.c
+-rw-r--r--   0 robin     (1000) robin     (1000)     2130 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.h
+-rw-r--r--   0 robin     (1000) robin     (1000)    36457 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.mashed
+-rw-r--r--   0 robin     (1000) robin     (1000)     9150 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/pyHnjmodule.c
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.728876 reportlab-3.6.9/src/rl_addons/rl_accel/tests/
+-rw-r--r--   0 robin     (1000) robin     (1000)      669 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/getrc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1378 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t0.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      747 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1875 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1687 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t5.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.738877 reportlab-3.6.9/tests/
+-rw-r--r--   0 robin     (1000) robin     (1000)      913 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/00readme.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)      540 2021-05-05 14:58:39.000000 reportlab-3.6.9/tests/7x11.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)       99 2021-05-05 14:57:42.000000 reportlab-3.6.9/tests/7x11.png
+-rw-r--r--   0 robin     (1000) robin     (1000)       80 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1077 2022-03-25 08:40:21.000000 reportlab-3.6.9/tests/_i_am_actually_a_gif.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    12463 2022-03-25 08:40:21.000000 reportlab-3.6.9/tests/_i_am_actually_a_jpeg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3813 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/alpha_test.png
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.742210 reportlab-3.6.9/tests/barcode-out/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1091 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Codabar.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1458 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code11.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1309 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code128.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1457 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code128Auto.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3014 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN13.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1769 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN5.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2385 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN8.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3091 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/ECC200DataMatrix.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1562 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Extended39.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1906 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Extended93.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1080 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/FIM.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1114 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/I2of5.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3631 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/ISBN.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1119 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/MSI.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1530 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/POSTNET.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2767 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/QR.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3229 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/QR_with_comma.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1565 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Standard39.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1234 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Standard93.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2933 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/UPCA.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1589 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/USPS_4State.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2388 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2210 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    12180 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.tiff
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.768877 reportlab-3.6.9/tests/charts-out/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1643 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1506 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1480 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1168 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4004 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3240 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2807 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3742 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2267 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2347 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3630 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2274 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1883 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1846 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2267 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2291 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2332 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3616 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2288 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2277 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2700 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3743 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2681 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3727 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2685 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3734 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2712 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3807 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2756 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2753 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3728 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2734 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3776 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2766 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1724 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1872 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3516 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    13857 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6784 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    15564 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7126 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    15568 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8113 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2619 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3383 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5299 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3071 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4033 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3120 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2287 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2868 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5477 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     9274 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4218 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7323 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4289 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7447 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4952 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     9053 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4741 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6406 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3050 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3287 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4149 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2884 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3669 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2807 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3020 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3887 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5378 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3956 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5381 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3464 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5290 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3459 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5291 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5286 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3389 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5293 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6675 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    48255 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7857 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    46272 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3139 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4036 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3029 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3116 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2291 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5932 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     9403 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4468 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7338 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4473 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7450 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5370 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     9105 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6379 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3140 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4004 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3206 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4118 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2891 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3654 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2924 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3003 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5412 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4853 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5422 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4426 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5332 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4437 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4602 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4455 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5859 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1492 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6451 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2174 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7297 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7278 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2471 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2843 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2512 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2847 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2080 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2483 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2100 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2508 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3628 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3344 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6052 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    13106 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6759 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    14174 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6782 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    62954 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7754 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    41220 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2447 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8150 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5435 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    33385 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4772 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    10135 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4632 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     9133 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6048 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    10000 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3585 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7027 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2352 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2420 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4239 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2775 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5724 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3940 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3533 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1272 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4024 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2052 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6870 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5057 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6126 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5182 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    16767 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    23088 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9369 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    12584 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10699 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    12623 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4504 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7899 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4376 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8690 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4678 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    10059 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3914 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3805 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4889 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6410 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6996 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8945 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9425 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8676 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4865 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6067 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8486 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    12166 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5283 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6357 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1765 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1182 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4283 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7687 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6776 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5397 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8883 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     4414 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11410 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    10045 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2979 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/encryption.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1908 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/gray-alpha.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/pythonpowered-gs.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     1077 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/pythonpowered.gif
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tests/render-out/
+-rw-r--r--   0 robin     (1000) robin     (1000)     2589 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/410.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1362 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/410.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3229 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5106 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     2850 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1020 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2560 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5750 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     2739 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.png
+-rw-r--r--   0 robin     (1000) robin     (1000)      846 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8923 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8747 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    14798 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1327 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2369 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2785 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     2765 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.png
+-rw-r--r--   0 robin     (1000) robin     (1000)      858 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3163 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3729 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     4721 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1393 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6353 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    10726 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    12964 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3929 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5433 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     7028 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     8298 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3428 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     6355 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     4097 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    10846 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7990 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing09.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     8280 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    15924 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1339 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3154 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     5783 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     2163 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2189 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2915 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)     3105 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     7969 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    17038 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    16031 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    28701 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1219 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    40966 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    51523 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    72941 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     4246 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1374 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     2183 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)      882 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1064 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      342 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-none.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1011 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-none.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      336 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-pdf.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-pdf.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      352 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-svg.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-svg.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11577 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-even-odd.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-even-odd.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11621 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-non-zero.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-non-zero.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    14199 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/hatch.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     6477 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/hatch.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      879 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/svglib-issue104.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    24350 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/textmode.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     2027 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/textmode.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6504 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/rltw-icon-tr.png
+-rwxr-xr-x   0 robin     (1000) robin     (1000)     5209 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/runAll.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2402 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/solid_red_alpha.png
+-rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/tall_red.png
+-rw-r--r--   0 robin     (1000) robin     (1000)      288 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-cross.tiff
+-rw-r--r--   0 robin     (1000) robin     (1000)      168 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-indexed.png
+-rw-r--r--   0 robin     (1000) robin     (1000)      157 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-rgba.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     9464 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_charts_textlabels.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6252 2019-11-23 12:29:07.000000 reportlab-3.6.9/tests/test_crypto_algorithms.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1462 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_docs_build.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6506 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_docstrings.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3058 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_extra.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      954 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_geomutils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    14652 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_barcode.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    41317 2022-02-03 15:17:16.000000 reportlab-3.6.9/tests/test_graphics_charts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    32774 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images-cairo.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    46849 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images-cairo.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    16209 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    21349 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images.png
+-rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_images.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2523 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_graphics_layout.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15789 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_render.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2628 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_graphics_speed.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1893 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_hello.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2662 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_images.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2511 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_invariant.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4214 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_issues.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8276 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_lib_colors.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    11916 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_normaldate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6062 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_pdfencrypt.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6780 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_lib_rl_safe_eval.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3748 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_sequencer.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13278 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_lib_utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5592 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_lib_validators.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2448 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_chs.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4973 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_cht.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    25468 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_multibyte_jpn.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6658 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_kor.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    34098 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_paragraphs.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10715 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_encodings.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3875 2020-01-26 19:46:34.000000 reportlab-3.6.9/tests/test_pdfbase_fontembed.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2713 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_pdfdoc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    18606 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfform.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4120 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfmetrics.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1609 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfutils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_postscript.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    19727 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pdfbase_ttfonts.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      989 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_callback.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    48259 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pdfgen_general.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6925 2021-07-06 13:47:00.000000 reportlab-3.6.9/tests/test_pdfgen_links.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3133 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_overprint.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1850 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_pagemodes.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3168 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_platypus_accum.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    27202 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_breaking.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5973 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_cjk_wrap.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    34433 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_general.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4226 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_images.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8549 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_indents.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5383 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_platypus_index.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6293 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_leftright.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10786 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_lists.py
+-rw-r--r--   0 robin     (1000) robin     (1000)   113010 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_paragraphs.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5094 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_platypus_paraparser.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9402 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_pleaseturnover.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8635 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_preformatted.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7373 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_programming.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    53423 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_tables.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12590 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_toc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3773 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_wrapping.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5183 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_xref.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4762 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pyfiles.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7690 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_renderPS.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9773 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_renderSVG.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    10617 2022-03-24 13:23:54.000000 reportlab-3.6.9/tests/test_rl_accel.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3423 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_source_chars.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    19261 2022-03-22 08:49:11.000000 reportlab-3.6.9/tests/test_table_layout.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1244 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_tools_pythonpoint.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1353 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4890 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_widgetbase_tpc.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    15476 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_widgets_grids.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/unimportable.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/
+-rw-r--r--   0 robin     (1000) robin     (1000)      193 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/README
+-rw-r--r--   0 robin     (1000) robin     (1000)      160 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/__init__.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/docco/
+-rw-r--r--   0 robin     (1000) robin     (1000)      292 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/README
+-rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7791 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/codegrab.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    41170 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/docpy.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    29268 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/examples.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    32661 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/graphdocpy.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    13738 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/rl_doc_utils.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5898 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/rltemplate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6939 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/stylesheet.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     9899 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/t_parse.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     7023 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/yaml.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3284 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/yaml2pdf.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1056 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pdfpath.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/pythonpoint/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1099 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/README
+-rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     8840 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/customshapes.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/pythonpoint/demos/
+-rw-r--r--   0 robin     (1000) robin     (1000)    26656 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/examples.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3670 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/figures.xml
+-rw-r--r--   0 robin     (1000) robin     (1000)     4859 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/htu.xml
+-rw-r--r--   0 robin     (1000) robin     (1000)     3008 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.a85
+-rw-r--r--   0 robin     (1000) robin     (1000)     2198 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/lj8100.jpg
+-rw-r--r--   0 robin     (1000) robin     (1000)    11730 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/monterey.xml
+-rw-r--r--   0 robin     (1000) robin     (1000)    12918 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/outline.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     3429 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/pplogo.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)   125666 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/python.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)    41307 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/pythonpoint.xml
+-rw-r--r--   0 robin     (1000) robin     (1000)     1704 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/slidebox.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1855 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/spectrum.png
+-rw-r--r--   0 robin     (1000) robin     (1000)    20910 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/vertpython.gif
+-rw-r--r--   0 robin     (1000) robin     (1000)     7920 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/pythonpoint.dtd
+-rw-r--r--   0 robin     (1000) robin     (1000)    34726 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/pythonpoint.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    28933 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/stdparser.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/pythonpoint/styles/
+-rw-r--r--   0 robin     (1000) robin     (1000)      179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/horrible.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5079 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/htu.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3692 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/modern.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3215 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/projection.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/standard.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/utils/
+-rw-r--r--   0 robin     (1000) robin     (1000)      954 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/utils/add_bleed.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1891 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/utils/dumpttf.py
```

### Comparing `reportlab-3.6.8/CHANGES.md` & `reportlab-3.6.9/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 E.g. to retrieve the changes made between release 3.4 and release 3.5, type::
 
   $ hg log -r 54ce2469ba5c
 
 The contributors lists are in no order and apologies to those accidentally not
 mentioned. If we missed you, please let us know!
 
+CHANGES  3.6.9   22/03/2022
+---------------------------
+	* fix up _rl_accel.c 0.81 to allow better error messages and support python 3.11.0a6
+	* change the cibuildwheel setup to support macos M1 build
+
 CHANGES  3.6.8   28/02/2022
 ---------------------------
 	* remove old Python2 constructs; patch from Claude Paroz < claude at 2xlibre dot net >
 
 CHANGES  3.6.7   18/02/2022
 ---------------------------
 	* Remove use of cPickle; patch from Claude Paroz < claude at 2xlibre dot net >
```

### Comparing `reportlab-3.6.8/LICENSE.txt` & `reportlab-3.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/MANIFEST.in` & `reportlab-3.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/PKG-INFO` & `reportlab-3.6.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 3.6.8
+Version: 3.6.9
 Summary: The Reportlab Toolkit
 Home-page: http://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
 License: BSD license (see license.txt for details), Copyright (c) 2000-2018, ReportLab Inc.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Printing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: RLPYCAIRO
 License-File: LICENSE.txt
 
 The ReportLab Toolkit. An Open Source Python library for generating PDFs and graphics.
```

### Comparing `reportlab-3.6.8/README.txt` & `reportlab-3.6.9/README.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/colors/colortest.py` & `reportlab-3.6.9/demos/colors/colortest.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/gadflypaper/gfe.py` & `reportlab-3.6.9/demos/gadflypaper/gfe.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/odyssey/00readme.txt` & `reportlab-3.6.9/demos/odyssey/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/odyssey/dodyssey.py` & `reportlab-3.6.9/demos/odyssey/dodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/odyssey/fodyssey.py` & `reportlab-3.6.9/demos/odyssey/fodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/odyssey/odyssey.py` & `reportlab-3.6.9/demos/odyssey/odyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/odyssey/odyssey.txt` & `reportlab-3.6.9/demos/odyssey/odyssey.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/rlzope/readme.txt` & `reportlab-3.6.9/demos/rlzope/readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/rlzope/rlzope.py` & `reportlab-3.6.9/demos/rlzope/rlzope.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/stdfonts/stdfonts.py` & `reportlab-3.6.9/demos/stdfonts/stdfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/demos/tests/testdemos.py` & `reportlab-3.6.9/demos/tests/testdemos.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/Makefile` & `reportlab-3.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/genAll.py` & `reportlab-3.6.9/docs/genAll.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/Edit_Prefs.gif` & `reportlab-3.6.9/docs/images/Edit_Prefs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/Python_21.gif` & `reportlab-3.6.9/docs/images/Python_21.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/Python_21_HINT.gif` & `reportlab-3.6.9/docs/images/Python_21_HINT.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/fileExchange.gif` & `reportlab-3.6.9/docs/images/fileExchange.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/jpegrgb_dissected.png` & `reportlab-3.6.9/docs/images/jpegrgb_dissected.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/jpn.gif` & `reportlab-3.6.9/docs/images/jpn.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/jpnchars.jpg` & `reportlab-3.6.9/docs/images/jpnchars.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/lj8100.jpg` & `reportlab-3.6.9/docs/images/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/replogo.a85` & `reportlab-3.6.9/docs/images/replogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/replogo.gif` & `reportlab-3.6.9/docs/images/replogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/images/testimg.gif` & `reportlab-3.6.9/docs/images/testimg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/make.bat` & `reportlab-3.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/reference/genreference.py` & `reportlab-3.6.9/docs/reference/genreference.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/reference/reference.yml` & `reportlab-3.6.9/docs/reference/reference.yml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/_static/default.css` & `reportlab-3.6.9/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/_templates/page.html` & `reportlab-3.6.9/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/conf.py` & `reportlab-3.6.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/graphics.rst` & `reportlab-3.6.9/docs/source/graphics.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/index.rst` & `reportlab-3.6.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/lib.rst` & `reportlab-3.6.9/docs/source/lib.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/source/platypus.rst` & `reportlab-3.6.9/docs/source/platypus.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/app_demos.py` & `reportlab-3.6.9/docs/userguide/app_demos.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch1_intro.py` & `reportlab-3.6.9/docs/userguide/ch1_intro.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch2_graphics.py` & `reportlab-3.6.9/docs/userguide/ch2_graphics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch2a_fonts.py` & `reportlab-3.6.9/docs/userguide/ch2a_fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch3_pdffeatures.py` & `reportlab-3.6.9/docs/userguide/ch3_pdffeatures.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch4_platypus_concepts.py` & `reportlab-3.6.9/docs/userguide/ch4_platypus_concepts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch5_paragraphs.py` & `reportlab-3.6.9/docs/userguide/ch5_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch6_tables.py` & `reportlab-3.6.9/docs/userguide/ch6_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/ch7_custom.py` & `reportlab-3.6.9/docs/userguide/ch7_custom.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/genuserguide.py` & `reportlab-3.6.9/docs/userguide/genuserguide.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/graph_charts.py` & `reportlab-3.6.9/docs/userguide/graph_charts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/graph_concepts.py` & `reportlab-3.6.9/docs/userguide/graph_concepts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/graph_shapes.py` & `reportlab-3.6.9/docs/userguide/graph_shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/docs/userguide/graph_widgets.py` & `reportlab-3.6.9/docs/userguide/graph_widgets.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/setup.py` & `reportlab-3.6.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 pjoin = os.path.join
 abspath = os.path.abspath
 isfile = os.path.isfile
 isdir = os.path.isdir
 dirname = os.path.dirname
 basename = os.path.basename
 splitext = os.path.splitext
-archName = 'amd64' if sys.maxsize > 2**32 else 'x86'    #correct for windows builds
+addrSize = 64 if sys.maxsize > 2**32 else 32
+sysconfig_platform = sysconfig.get_platform()
 
 INFOLINES=[]
 def infoline(t,
         pfx='#####',
         add=True,
         ):
     bn = splitext(basename(sys.argv[0]))[0]
     ver = '.'.join(map(str,sys.version_info[:3]))
-    platform = sysconfig.get_platform()
-    s = '%s %s-python-%s-%s: %s' % (pfx, bn, ver, platform, t)
+    s = '%s %s-python-%s-%s: %s' % (pfx, bn, ver, sysconfig_platform, t)
     print(s)
     if add: INFOLINES.append(s)
 
 def showTraceback(s):
     buf = io.StringIO()
     print(s,file=buf)
     if verbose>2:
@@ -185,50 +185,109 @@
 def aDir(P, d, x=None):
     if d and isdir(d) and d not in P:
         if x is None:
             P.append(d)
         else:
             P.insert(x, d)
 
+def findFile(root, wanted, followlinks=True):
+    for p, _, F in os.walk(root,followlinks=followlinks):
+        for fn in F:
+            if fn==wanted:  
+                return abspath(pjoin(p,fn))
+
+def listFiles(root,followlinks=True,strJoin=None):
+    R = [].append
+    for p, _, F in os.walk(root,followlinks=followlinks):
+        for fn in F:
+            R(abspath(pjoin(p,fn)))
+    R = R.__self__
+    return strJoin.join(R) if strJoin else R
+
+def freetypeVersion(fn,default='20'):
+    with open(fn,'r') as _:
+        text = _.read()
+    pat = re.compile(r'^#define\s+FREETYPE_(?P<level>MAJOR|MINOR|PATCH)\s*(?P<value>\d*)\s*$',re.M)
+    locmap=dict(MAJOR=0,MINOR=1,PATCH=2)
+    loc = ['','','']
+    for m in pat.finditer(text):
+        loc[locmap[m.group('level')]] = m.group('value')
+    loc = list(filter(None,loc))
+    return '.'.join(loc) if loc else default
+
 class inc_lib_dirs:
-    L = None
-    I = None
-    def __call__(self):
-        if self.L is None:
-            L = []
-            I = []
-            if platform == "cygwin":
-                aDir(L, os.path.join("/usr/lib", "python%s" % sys.version[:3], "config"))
-            elif platform == "darwin":
-                # attempt to make sure we pick freetype2 over other versions
-                aDir(I, "/sw/include/freetype2")
-                aDir(I, "/sw/lib/freetype2/include")
-                # fink installation directories
-                aDir(L, "/sw/lib")
-                aDir(I, "/sw/include")
-                # darwin ports installation directories
-                aDir(L, "/opt/local/lib")
-                aDir(I, "/opt/local/include")
-            aDir(I, "/usr/local/include")
-            aDir(L, "/usr/local/lib")
-            aDir(I, "/usr/include")
-            aDir(L, "/usr/lib")
-            aDir(I, "/usr/include/freetype2")
-            if archName=='amd64':
-                aDir(L, "/usr/lib/lib64")
-                aDir(L, "/usr/lib/x86_64-linux-gnu")
-            else:
-                aDir(L, "/usr/lib/lib32")
-            prefix = sysconfig.get_config_var("prefix")
-            if prefix:
-                aDir(L, pjoin(prefix, "lib"))
-                aDir(I, pjoin(prefix, "include"))
-            self.L=L
-            self.I=I
-        return self.I,self.L
+    def __call__(self,libname=None):
+        L = config('FREETYPE_PATHS','lib')
+        L = [L] if L else []
+        I = config('FREETYPE_PATHS','inc')
+        I = [I] if I else []
+        if platform == "cygwin":
+            aDir(L, os.path.join("/usr/lib", "python%s" % sys.version[:3], "config"))
+        elif platform == "darwin":
+            machine = sysconfig_platform.split('-')[-1]
+            if machine=='arm64' or os.environ.get('ARCHFLAGS','')=='-arch arm64':
+                #print('!!!!! detected darwin arm64 build')
+                #probably an M1
+                target = pjoin(
+                            ensureResourceStuff('m1stuff.tar.gz','m1stuff','tar',
+                                baseDir=os.environ.get('RL_CACHE_DIR','/tmp/reportlab')),
+                            'm1stuff','opt','homebrew'
+                            )
+                _lib = pjoin(target,'lib')
+                _inc = pjoin(target,'include','freetype2')
+                #print('!!!!! target=%s' % target)
+                #print('!!!!! _lib=%s -->\n %s'%(_lib,listFiles(_lib,strJoin='\n ')))
+                #print('!!!!! _inc=%s -->\n %s'%(_inc,listFiles(_inc,strJoin='\n ')))
+                aDir(L, _lib)
+                aDir(I, _inc)
+                #print('!!!!! L=%s I=%s' % (L,I))
+            elif machine=='x86_64':
+                aDir(L,'/usr/local/lib')
+                aDir(I, "/usr/local/include/freetype2")
+            # attempt to make sure we pick freetype2 over other versions
+            aDir(I, "/sw/include/freetype2")
+            aDir(I, "/sw/lib/freetype2/include")
+            # fink installation directories
+            aDir(L, "/sw/lib")
+            aDir(I, "/sw/include")
+            # darwin ports installation directories
+            aDir(L, "/opt/local/lib")
+            aDir(I, "/opt/local/include")
+        aDir(I, "/usr/local/include")
+        aDir(L, "/usr/local/lib")
+        aDir(I, "/usr/include")
+        aDir(L, "/usr/lib")
+        aDir(I, "/usr/include/freetype2")
+        if addrSize==64:
+            aDir(L, "/usr/lib/lib64")
+            aDir(L, "/usr/lib/x86_64-linux-gnu")
+        else:
+            aDir(L, "/usr/lib/lib32")
+        prefix = sysconfig.get_config_var("prefix")
+        if prefix:
+            aDir(L, pjoin(prefix, "lib"))
+            aDir(I, pjoin(prefix, "include"))
+        if libname:
+            gsn = ''.join((('lib' if not libname.startswith('lib') else ''),libname,'*'))
+            L = list(filter(lambda _: glob.glob(pjoin(_,gsn)),L))
+        for d in I:
+            mif = findFile(d,'ft2build.h')
+            if mif:
+                #print('!!!!! d=%s --> mif=%r' % (d,mif))
+                break
+        else:
+            mif = None
+        if mif:
+            d = dirname(mif)
+            I = [dirname(d), d]
+            ftv = freetypeVersion(findFile(d,'freetype.h'),'22')
+        else:
+            print('!!!!! cannot find ft2build.h')
+            sys.exit(1)
+        return ftv,I,L
 inc_lib_dirs=inc_lib_dirs()
 
 def getVersionFromCCode(fn):
     tag = re.search(r'^#define\s+VERSION\s+"([^"]*)"',open(fn,'r').read(),re.M)
     return tag and tag.group(1) or ''
 
 class _rl_dir_info:
@@ -323,24 +382,33 @@
     remotehandle = ureq.urlopen(url)
     try:
         raw = remotehandle.read()
         return raw if returnRaw else io.BytesIO(raw)
     finally:
         remotehandle.close()
 
-def ensureWinStuff(
-                    url='https://www.reportlab.com/ftp/winstuff.zip',
-                    target=pjoin(pkgDir,'build','winstuff'),
+def ensureResourceStuff(
+                ftpName='winstuff.zip',
+                buildName='winstuff',
+                extract='zip',
+                baseDir=pjoin(pkgDir,'build'),
                 ):
+    url='https://www.reportlab.com/ftp/%s' % ftpName
+    target=pjoin(baseDir,buildName)
     done = pjoin(target,'.done')
     if not isfile(done):
         if not isdir(target):
             os.makedirs(target)
-            import zipfile, time
-            zipfile.ZipFile(url2data(url), 'r').extractall(path=target)
+            if extract=='zip':
+                import zipfile
+                zipfile.ZipFile(url2data(url), 'r').extractall(path=target)
+            elif extract=='tar':
+                import tarfile
+                tarfile.open(fileobj=url2data(url), mode='r:gz').extractall(path=target)
+            import time
             with open(done,'w') as _:
                 _.write(time.strftime('%Y%m%dU%H%M%S\n',time.gmtime()))
     return target
 
 def get_fonts(PACKAGE_DIR, reportlab_files):
     import zipfile
     rl_dir = PACKAGE_DIR['reportlab']
@@ -473,14 +541,16 @@
         rl_ixu = vopt('rl-index-url')
         if len(rl_ixu)==1:
             pipInstallGroups(rl_pip_installs,qup(rl_ixu[0]))
         else:
             raise ValueError('rl-pip-install requires exactly 1 --rl-index-url not %d' % len(rl_ixu))
 
 def showEnv():
+    action = -1 if specialOption('--show-env-only') else 1 if specialOption('--show-env') else 0
+    if not action: return
     print('+++++ setup.py environment')
     print('+++++ sys.version = %s' % sys.version.replace('\n',''))
     import platform
     for k in sorted((_ for _ in dir(platform) if not _.startswith('_'))):
         try:
             v = getattr(platform,k)
             if isinstance(v,(str,list,tuple,bool)):
@@ -492,18 +562,19 @@
         except:
             v = '?????'
         print('+++++ platform.%s = %s' % (k,v))
     print('--------------------------')
     for k, v in sorted(os.environ.items()):
         print('+++++ environ[%s] = %r' % (k,v))
     print('--------------------------')
+    if action<0:
+        sys.exit(0)
 
 def main():
-    if specialOption('--show-env'):
-        showEnv()
+    showEnv()
     performPipInstalls()
     #test to see if we've a special command
     if 'test' in sys.argv \
         or 'tests' in sys.argv \
         or 'tests-postinstall' in sys.argv \
         or 'tests-preinstall' in sys.argv:
         verboseTests = specialOption('--verbose-tests')
@@ -640,16 +711,16 @@
                     pjoin(GT1_DIR,'gt1-parset1.c'),
                     pjoin(GT1_DIR,'gt1-dict.c'),
                     pjoin(GT1_DIR,'gt1-namecontext.c'),
                     pjoin(GT1_DIR,'gt1-region.c'),
                     ]+LIBART_SOURCES
 
         if platform=='win32':
-            target = ensureWinStuff()
-            FT_LIB = pjoin(target,'libs',archName,'freetype.lib')
+            target = ensureResourceStuff()
+            FT_LIB = pjoin(target,'libs','amd64' if addrSize==64 else 'x86','freetype.lib')
             if not isfile(FT_LIB):
                 infoline('freetype lib %r not found' % FT_LIB, pfx='!!!!')
                 FT_LIB=[]
             if FT_LIB:
                 FT_INC_DIR = pjoin(target,'include')
                 if not isfile(pjoin(FT_INC_DIR,'ft2build.h')):
                     FT_INC_DIR = pjoin(FT_INC_DIR,'freetype2')
@@ -662,45 +733,21 @@
                 FT_LIB_PATH = FT_LIB
                 FT_LIB = [splitext(basename(FT_LIB))[0]]
                 if isdir(FT_INC_DIR[0]):
                     infoline('installing with freetype %r' % FT_LIB_PATH)
             else:
                 FT_LIB=FT_LIB_DIR=FT_INC_DIR=FT_MACROS=[]
         else:
-            if os.path.isdir('/usr/include/freetype2'):
-                FT_LIB_DIR = []
-                FT_INC_DIR = ['/usr/include/freetype2']
-            else:
-                FT_LIB_DIR=config('FREETYPE_PATHS','lib')
-                FT_LIB_DIR=[FT_LIB_DIR] if FT_LIB_DIR else []
-                FT_INC_DIR=config('FREETYPE_PATHS','inc')
-                FT_INC_DIR=[FT_INC_DIR] if FT_INC_DIR else []
-            I,L=inc_lib_dirs()
-            ftv = None
-            for d in I:
-                if isfile(pjoin(d, "ft2build.h")):
-                    ftv = 21
-                    FT_INC_DIR=[d,pjoin(d, "freetype2")]
-                    break
-                d = pjoin(d, "freetype2")
-                if isfile(pjoin(d, "ft2build.h")):
-                    ftv = 21
-                    FT_INC_DIR=[d]
-                    break
-                if isdir(pjoin(d, "freetype")):
-                    ftv = 20
-                    FT_INC_DIR=[d]
-                    break
-            if ftv:
-                FT_LIB=['freetype']
-                FT_LIB_DIR=L
-                FT_MACROS = [('RENDERPM_FT',None)]
-                infoline('# installing with freetype version %d' % ftv)
-            else:
-                FT_LIB=FT_LIB_DIR=FT_INC_DIR=FT_MACROS=[]
+            ftv, I, L = inc_lib_dirs('freetype')
+            FT_LIB=['freetype']
+            FT_LIB_DIR=L
+            FT_INC_DIR=I
+            FT_MACROS = [('RENDERPM_FT',None)]
+            infoline('installing with freetype version %s' % ftv)
+            infoline('FT_LIB_DIR=%r FT_INC_DIR=%r' % (FT_LIB_DIR,FT_INC_DIR))
         if not FT_LIB:
             infoline('# installing without freetype no ttf, sorry!')
             infoline('# You need to install a static library version of the freetype2 software')
             infoline('# If you need truetype support in renderPM')
             infoline('# You may need to edit setup.cfg (win32)')
             infoline('# or edit this file to access the library if it is installed')
 
@@ -754,25 +801,24 @@
             classifiers = [
                 'Development Status :: 5 - Production/Stable',
                 'Intended Audience :: Developers',
                 'License :: OSI Approved :: BSD License',
                 'Topic :: Printing',
                 'Topic :: Text Processing :: Markup',
                 'Programming Language :: Python :: 3',
-                'Programming Language :: Python :: 3.6',
                 'Programming Language :: Python :: 3.7',
                 'Programming Language :: Python :: 3.8',
                 'Programming Language :: Python :: 3.9',
                 'Programming Language :: Python :: 3.10',
                 'Programming Language :: Python :: 3.11',
                 ],
             
             #this probably only works for setuptools, but distutils seems to ignore it
             install_requires=['pillow>=4.0.0'],
-            python_requires='>=3.6, <4',
+            python_requires='>=3.7, <4',
             extras_require={
                 'RLPYCAIRO': ['rlPyCairo>=0.0.5'],
                 },
             )
         print()
         print('########## SUMMARY INFO #########')
         print('\n'.join(INFOLINES))
```

### Comparing `reportlab-3.6.8/src/reportlab/__init__.py` & `reportlab-3.6.9/src/reportlab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #Copyright ReportLab Europe Ltd. 2000-2021
 #see license.txt for license details
 __doc__="""The Reportlab PDF generation library."""
-Version = "3.6.8"
+Version = "3.6.9"
 __version__=Version
-__date__='20220228'
+__date__='20220322'
 
 import sys, os
 
-__min_python_version__ = (3,6)
+__min_python_version__ = (3,7)
 if sys.version_info< __min_python_version__:
     raise ImportError("""reportlab requires %s.%s+; other versions are unsupported.
 If you want to try with other python versions edit line 10 of reportlab/__init__
 to remove this error.""" % (__min_python_version__))
 
 #define these early in reportlab's life
 def cmp(a,b):
```

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGarden-copying-gpl.txt` & `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGarden-copying.txt` & `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGarden-readme.txt` & `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGarden.sfd` & `reportlab-3.6.9/src/reportlab/fonts/DarkGarden.sfd`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGardenMK.afm` & `reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.afm`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/DarkGardenMK.pfb` & `reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/Vera.ttf` & `reportlab-3.6.9/src/reportlab/fonts/Vera.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/VeraBI.ttf` & `reportlab-3.6.9/src/reportlab/fonts/VeraBI.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/VeraBd.ttf` & `reportlab-3.6.9/src/reportlab/fonts/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/VeraIt.ttf` & `reportlab-3.6.9/src/reportlab/fonts/VeraIt.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_a______.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_a______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_ab_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_ab_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_abi____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_abi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_ai_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_ai_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_eb_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_eb_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_ebi____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_ebi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_ei_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_ei_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/_er_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/_er_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/bitstream-vera-license.txt` & `reportlab-3.6.9/src/reportlab/fonts/bitstream-vera-license.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/callig15.afm` & `reportlab-3.6.9/src/reportlab/fonts/callig15.afm`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/callig15.pfb` & `reportlab-3.6.9/src/reportlab/fonts/callig15.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/cob_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/cob_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/cobo____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/cobo____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/com_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/com_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/coo_____.pfb` & `reportlab-3.6.9/src/reportlab/fonts/coo_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/sy______.pfb` & `reportlab-3.6.9/src/reportlab/fonts/sy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/zd______.pfb` & `reportlab-3.6.9/src/reportlab/fonts/zd______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/zx______.pfb` & `reportlab-3.6.9/src/reportlab/fonts/zx______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/fonts/zy______.pfb` & `reportlab-3.6.9/src/reportlab/fonts/zy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/README` & `reportlab-3.6.9/src/reportlab/graphics/barcode/README`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/TODO` & `reportlab-3.6.9/src/reportlab/graphics/barcode/TODO`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/__init__.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/__init__.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/code128.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/code128.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/code39.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/code39.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/code93.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/code93.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/common.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/common.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/dmtx.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/dmtx.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/eanbc.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/eanbc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/ecc200datamatrix.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/ecc200datamatrix.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/fourstate.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/fourstate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/lto.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/lto.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/qr.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/qr.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/qrencoder.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/qrencoder.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/test.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/test.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/usps.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/usps.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/usps4s.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/usps4s.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/barcode/widgets.py` & `reportlab-3.6.9/src/reportlab/graphics/barcode/widgets.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/areas.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/areas.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/axes.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/axes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/barcharts.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/barcharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/dotbox.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/dotbox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/doughnut.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/doughnut.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/legends.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/legends.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/linecharts.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/linecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/lineplots.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/lineplots.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/markers.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/piecharts.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/piecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/slidebox.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/spider.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/spider.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/textlabels.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/utils.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/charts/utils3d.py` & `reportlab-3.6.9/src/reportlab/graphics/charts/utils3d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/renderPDF.py` & `reportlab-3.6.9/src/reportlab/graphics/renderPDF.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/renderPM.py` & `reportlab-3.6.9/src/reportlab/graphics/renderPM.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/renderPS.py` & `reportlab-3.6.9/src/reportlab/graphics/renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/renderSVG.py` & `reportlab-3.6.9/src/reportlab/graphics/renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/renderbase.py` & `reportlab-3.6.9/src/reportlab/graphics/renderbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/bubble.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/bubble.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/clustered_bar.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/clustered_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/clustered_column.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/clustered_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/excelcolors.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/excelcolors.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/exploded_pie.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/exploded_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/filled_radar.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/filled_radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/line_chart.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/line_chart.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/linechart_with_markers.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/linechart_with_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/radar.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/runall.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/runall.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/scatter.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/scatter.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/scatter_lines.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/scatter_lines_markers.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/simple_pie.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/simple_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/stacked_bar.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/samples/stacked_column.py` & `reportlab-3.6.9/src/reportlab/graphics/samples/stacked_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/shapes.py` & `reportlab-3.6.9/src/reportlab/graphics/shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/testdrawings.py` & `reportlab-3.6.9/src/reportlab/graphics/testdrawings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/testshapes.py` & `reportlab-3.6.9/src/reportlab/graphics/testshapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/transform.py` & `reportlab-3.6.9/src/reportlab/graphics/transform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/utils.py` & `reportlab-3.6.9/src/reportlab/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgetbase.py` & `reportlab-3.6.9/src/reportlab/graphics/widgetbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/adjustableArrow.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/adjustableArrow.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/eventcal.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/eventcal.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/flags.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/flags.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/grids.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/markers.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/signsandsymbols.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/signsandsymbols.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/graphics/widgets/table.py` & `reportlab-3.6.9/src/reportlab/graphics/widgets/table.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/PyFontify.py` & `reportlab-3.6.9/src/reportlab/lib/PyFontify.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/abag.py` & `reportlab-3.6.9/src/reportlab/lib/abag.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/arciv.py` & `reportlab-3.6.9/src/reportlab/lib/arciv.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/attrmap.py` & `reportlab-3.6.9/src/reportlab/lib/attrmap.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/boxstuff.py` & `reportlab-3.6.9/src/reportlab/lib/boxstuff.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/codecharts.py` & `reportlab-3.6.9/src/reportlab/lib/codecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/colors.py` & `reportlab-3.6.9/src/reportlab/lib/colors.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/corp.py` & `reportlab-3.6.9/src/reportlab/lib/corp.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/extformat.py` & `reportlab-3.6.9/src/reportlab/lib/extformat.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/fontfinder.py` & `reportlab-3.6.9/src/reportlab/lib/fontfinder.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/fonts.py` & `reportlab-3.6.9/src/reportlab/lib/fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/formatters.py` & `reportlab-3.6.9/src/reportlab/lib/formatters.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/geomutils.py` & `reportlab-3.6.9/src/reportlab/lib/geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/logger.py` & `reportlab-3.6.9/src/reportlab/lib/logger.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/normalDate.py` & `reportlab-3.6.9/src/reportlab/lib/normalDate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/pagesizes.py` & `reportlab-3.6.9/src/reportlab/lib/pagesizes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/pdfencrypt.py` & `reportlab-3.6.9/src/reportlab/lib/pdfencrypt.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/pygments2xpre.py` & `reportlab-3.6.9/src/reportlab/lib/pygments2xpre.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/randomtext.py` & `reportlab-3.6.9/src/reportlab/lib/randomtext.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/rl_accel.py` & `reportlab-3.6.9/src/reportlab/lib/rl_accel.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,25 +95,25 @@
         return R
     _py_funcs['unicode2T1'] = unicode2T1
 
 if 'instanceStringWidthT1' in _py_funcs:
     def instanceStringWidthT1(self, text, size, encoding='utf8'):
         """This is the "purist" approach to width"""
         if not isUnicode(text): text = text.decode(encoding)
-        return sum([sum(map(f.widths.__getitem__,t)) for f, t in unicode2T1(text,[self]+self.substitutionFonts)])*0.001*size
+        return sum((sum(map(f.widths.__getitem__,t)) for f, t in unicode2T1(text,[self]+self.substitutionFonts)))*0.001*size
     _py_funcs['instanceStringWidthT1'] = instanceStringWidthT1
 
 if 'instanceStringWidthTTF' in _py_funcs:
     def instanceStringWidthTTF(self, text, size, encoding='utf-8'):
         "Calculate text width"
         if not isUnicode(text):
             text = text.decode(encoding or 'utf-8')
         g = self.face.charWidths.get
         dw = self.face.defaultWidth
-        return 0.001*size*sum([g(ord(u),dw) for u in text])
+        return 0.001*size*sum((g(ord(u),dw) for u in text))
     _py_funcs['instanceStringWidthTTF'] = instanceStringWidthTTF
 
 if 'hex32' in _py_funcs:
     def hex32(i):
         return '0X%8.8X' % (int(i)&0xFFFFFFFF)
     _py_funcs['hex32'] = hex32
```

### Comparing `reportlab-3.6.8/src/reportlab/lib/rl_safe_eval.py` & `reportlab-3.6.9/src/reportlab/lib/rl_safe_eval.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/rltempfile.py` & `reportlab-3.6.9/src/reportlab/lib/rltempfile.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/rparsexml.py` & `reportlab-3.6.9/src/reportlab/lib/rparsexml.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/sequencer.py` & `reportlab-3.6.9/src/reportlab/lib/sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/styles.py` & `reportlab-3.6.9/src/reportlab/lib/styles.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/testutils.py` & `reportlab-3.6.9/src/reportlab/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/textsplit.py` & `reportlab-3.6.9/src/reportlab/lib/textsplit.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/units.py` & `reportlab-3.6.9/src/reportlab/lib/units.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/utils.py` & `reportlab-3.6.9/src/reportlab/lib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,18 +1327,18 @@
 
     @property
     def asctime(self):
         return time.asctime(self.lt)
 
 def recursiveGetAttr(obj, name, g=None):
     "Can call down into e.g. object1.object2[4].attr"
-    if not isStr(name): raise TypeError('invalid reursive acess using %r' % name)
+    if not isStr(name): raise TypeError('invalid recursive access of %s.%s' % (repr(obj),name))
     name = asNative(name)
     name = name.strip()
-    if not name: raise ValueError('empty recursive access')
+    if not name: raise ValueError('empty recursive access of %s' % repr(obj))
     dot = '.' if name and name[0] not in '[.(' else ''
     return rl_safe_eval('obj%s%s'%(dot,name), g={}, l=dict(obj=obj))
 
 def recursiveSetAttr(obj, name, value):
     "Can call down into e.g. object1.object2[4].attr = value"
     #get the thing above last.
     tokens = name.split('.')
```

### Comparing `reportlab-3.6.8/src/reportlab/lib/validators.py` & `reportlab-3.6.9/src/reportlab/lib/validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/lib/yaml.py` & `reportlab-3.6.9/src/reportlab/lib/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/license.txt` & `reportlab-3.6.9/src/reportlab/license.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_can_cmap_data.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_can_cmap_data.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_cidfontdata.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_cidfontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_macexpert.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_macroman.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_standard.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_symbol.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_winansi.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courier.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courier.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courierbold.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helvetica.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_symbol.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesbold.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_timesroman.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/_glyphlist.py` & `reportlab-3.6.9/src/reportlab/pdfbase/_glyphlist.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/acroform.py` & `reportlab-3.6.9/src/reportlab/pdfbase/acroform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/cidfonts.py` & `reportlab-3.6.9/src/reportlab/pdfbase/cidfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/pdfdoc.py` & `reportlab-3.6.9/src/reportlab/pdfbase/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/pdfform.py` & `reportlab-3.6.9/src/reportlab/pdfbase/pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/pdfmetrics.py` & `reportlab-3.6.9/src/reportlab/pdfbase/pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/pdfpattern.py` & `reportlab-3.6.9/src/reportlab/pdfbase/pdfpattern.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/pdfutils.py` & `reportlab-3.6.9/src/reportlab/pdfbase/pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/rl_codecs.py` & `reportlab-3.6.9/src/reportlab/pdfbase/rl_codecs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfbase/ttfonts.py` & `reportlab-3.6.9/src/reportlab/pdfbase/ttfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfgen/canvas.py` & `reportlab-3.6.9/src/reportlab/pdfgen/canvas.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfgen/pathobject.py` & `reportlab-3.6.9/src/reportlab/pdfgen/pathobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfgen/pdfgeom.py` & `reportlab-3.6.9/src/reportlab/pdfgen/pdfgeom.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfgen/pdfimages.py` & `reportlab-3.6.9/src/reportlab/pdfgen/pdfimages.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/pdfgen/textobject.py` & `reportlab-3.6.9/src/reportlab/pdfgen/textobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/doctemplate.py` & `reportlab-3.6.9/src/reportlab/platypus/doctemplate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/figures.py` & `reportlab-3.6.9/src/reportlab/platypus/figures.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/flowables.py` & `reportlab-3.6.9/src/reportlab/platypus/flowables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/frames.py` & `reportlab-3.6.9/src/reportlab/platypus/frames.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/multicol.py` & `reportlab-3.6.9/src/reportlab/platypus/multicol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/para.py` & `reportlab-3.6.9/src/reportlab/platypus/para.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/paragraph.py` & `reportlab-3.6.9/src/reportlab/platypus/paragraph.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/paraparser.py` & `reportlab-3.6.9/src/reportlab/platypus/paraparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/tableofcontents.py` & `reportlab-3.6.9/src/reportlab/platypus/tableofcontents.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/tables.py` & `reportlab-3.6.9/src/reportlab/platypus/tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/platypus/xpreformatted.py` & `reportlab-3.6.9/src/reportlab/platypus/xpreformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/rl_config.py` & `reportlab-3.6.9/src/reportlab/rl_config.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab/rl_settings.py` & `reportlab-3.6.9/src/reportlab/rl_settings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/reportlab.egg-info/PKG-INFO` & `reportlab-3.6.9/src/reportlab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 3.6.8
+Version: 3.6.9
 Summary: The Reportlab Toolkit
 Home-page: http://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
 License: BSD license (see license.txt for details), Copyright (c) 2000-2018, ReportLab Inc.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Printing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: RLPYCAIRO
 License-File: LICENSE.txt
 
 The ReportLab Toolkit. An Open Source Python library for generating PDFs and graphics.
```

### Comparing `reportlab-3.6.8/src/reportlab.egg-info/SOURCES.txt` & `reportlab-3.6.9/src/reportlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/_renderPM.c` & `reportlab-3.6.9/src/rl_addons/renderPM/_renderPM.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-dict.c` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-dict.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-misc.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-misc.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-namecontext.c` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-namecontext.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-parset1.c` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-parset1.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-region.c` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-region.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/gt1-value.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-value.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/parseAFM.c` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/gt1/parseAFM.h` & `reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/COPYING` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/COPYING`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/ChangeLog` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/ChangeLog`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/Makefile.am` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/Makefile.am`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/NEWS` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/NEWS`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/README` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/README`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_bpath.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_bpath.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_filterlevel.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_filterlevel.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_misc.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_misc.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pathcode.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pathcode.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_point.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_point.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_mask.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_mask.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_render_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgba.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_rgba.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_point.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_point.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/autogen.sh` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/autogen.sh`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/config.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/config.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/configure.in` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/configure.in`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/gen_art_config.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/gen_art_config.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-config.in` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-config.in`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart-features.h.in` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-features.h.in`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart.h` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/libart.m4` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.m4`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/test_gradient.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/test_gradient.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/testart.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testart.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/libart_lgpl/testuta.c` & `reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testuta.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/pfm.py` & `reportlab-3.6.9/src/rl_addons/renderPM/pfm.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/test_renderPM.py` & `reportlab-3.6.9/src/rl_addons/renderPM/test_renderPM.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/renderPM/tr.py` & `reportlab-3.6.9/src/rl_addons/renderPM/tr.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/_rl_accel.c` & `reportlab-3.6.9/src/rl_addons/rl_accel/_rl_accel.c`

 * *Files 10% similar despite different names*

```diff
@@ -23,58 +23,97 @@
 #endif
 #ifndef max
 #	define max(a,b) ((a)>(b)?(a):(b))
 #endif
 #ifndef min
 #	define min(a,b) ((a)<(b)?(a):(b))
 #endif
-#define VERSION "0.80"
+#define VERSION "0.81"
 #define MODULE "_rl_accel"
 
-struct module_state	{
-	int moduleLineno;
-	};
-#define GETSTATE(m) ((struct module_state*)PyModule_GetState(m))
 #define STRNAME "str"
 #define BYTESNAME "bytes"
+static void ModifyExcValue(PyObject *exc,const char *funcname,int lineno,const char* fmt,va_list ap)
+{
+	PyObject *type = NULL, *value = NULL, *tb = NULL, *aval=NULL, *uval=NULL;
+	const char* sval=NULL;
+	PyErr_Fetch(&type, &value, &tb);
+	PyErr_NormalizeException(&type, &value, &tb);
+	if(PyErr_Occurred()) goto L_BAD;
+	uval = PyUnicode_FromFormatV(fmt,ap);
+	if(uval){
+		PyErr_Format(exc,"%U in %s @ %s:%d\ncaused by %S",uval,funcname,__FILE__,lineno,value);
+		}
+	else {
+		PyErr_Format(exc,"in %s:%d\ncaused by %S",funcname,__FILE__,lineno,value);
+		}
+
+L_exit:
+	Py_XDECREF(uval);
+	Py_XDECREF(type);
+	Py_XDECREF(value);
+	Py_XDECREF(tb);
+	return;
+L_BAD:
+	if(type && value){
+		PyErr_Restore(type,value,tb);
+		type = value = tb = NULL;
+		}
+	goto L_exit;
+}
 
-#define ERROR_EXIT() {GETSTATE(module)->moduleLineno=__LINE__;goto L_ERR;}
-#define ADD_TB(module,name) _add_TB(module,name)
-#include "compile.h"
-#include "frameobject.h"
-#include "traceback.h"
-static void _add_TB(PyObject *module,char *funcname)
-{
-	int	moduleLineno = GETSTATE(module)->moduleLineno;
-	PyObject *py_globals = NULL;
-	PyCodeObject *py_code = NULL;
-	PyFrameObject *py_frame = NULL;
-
-	py_globals = PyModule_GetDict(module);
-	if(!py_globals) goto bad;
-	py_code = PyCode_NewEmpty(
-						__FILE__,		/*PyObject *filename,*/
-						funcname,	/*PyObject *name,*/
-						moduleLineno	/*int firstlineno,*/
-						);
-	if(!py_code) goto bad;
-	py_frame = PyFrame_New(
-		PyThreadState_Get(), /*PyThreadState *tstate,*/
-		py_code,			 /*PyCodeObject *code,*/
-		py_globals,			 /*PyObject *globals,*/
-		0					 /*PyObject *locals*/
-		);
-	if(!py_frame) goto bad;
-	py_frame->f_lineno = moduleLineno;
-	PyTraceBack_Here(py_frame);
-bad:
-	Py_XDECREF(py_code);
-	Py_XDECREF(py_frame);
+static void _excAddInfo(const char* funcname,int lineno, PyObject *exc, const char* fmt, va_list ap)
+{
+	PyObject *uval = NULL;
+	if(PyErr_Occurred()){
+		ModifyExcValue(exc,funcname,lineno,fmt,ap);
+		}
+	else{
+		uval = PyUnicode_FromFormatV(fmt,ap);
+		if(uval) {
+			PyErr_Format(exc,"in %s@%s:%d %U",funcname,__FILE__,lineno,uval);
+			Py_DECREF(uval);
+			}
+		else
+			PyErr_Format(exc,"in %s@%s:%d",funcname,__FILE__,lineno,uval);
+		}
 }
 
+static void excAddInfo(const char* funcname,int lineno, PyObject *exc, const char* fmt, ...)
+{
+	va_list ap;
+	va_start(ap,fmt);
+	_excAddInfo(funcname,lineno,exc,fmt,ap);
+	va_end(ap);
+}
+/*
+ * https://stackoverflow.com/questions/5588855/standard-alternative-to-gccs-va-args-trick
+ * expands to the first argument
+ */
+#define FIRST(...) FIRST_HELPER(__VA_ARGS__, throwaway)
+#define FIRST_HELPER(first, ...) first
+/*
+ * if there's only one argument, expands to nothing.  if there is more
+ * than one argument, expands to a comma followed by everything but
+ * the first argument.  only supports up to 9 arguments but can be
+ * trivially expanded.
+ */
+#define REST(...) REST_HELPER(NUM(__VA_ARGS__), __VA_ARGS__)
+#define REST_HELPER(qty, ...) REST_HELPER2(qty, __VA_ARGS__)
+#define REST_HELPER2(qty, ...) REST_HELPER_##qty(__VA_ARGS__)
+#define REST_HELPER_ONE(first)
+#define REST_HELPER_TWOORMORE(first, ...) , __VA_ARGS__
+#define NUM(...) \
+    SELECT_10TH(__VA_ARGS__, TWOORMORE, TWOORMORE, TWOORMORE, TWOORMORE,\
+                TWOORMORE, TWOORMORE, TWOORMORE, TWOORMORE, ONE, throwaway)
+#define SELECT_10TH(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, ...) a10
+#define EXC_SET(exc,...) do{excAddInfo(__func__,__LINE__,exc,FIRST(__VA_ARGS__) REST(__VA_ARGS__));}while(0)
+#define EXC_EXIT(exc,...)  do{EXC_SET(exc,FIRST(__VA_ARGS__) REST(__VA_ARGS__));goto L_exit;}while(0)
+#define MODULE_STATE_SIZE 0
+
 #define a85_0		   1L
 #define a85_1		   85L
 #define a85_2		 7225L
 #define a85_3	   614125L
 #define a85_4	 52200625L
 
 PyObject *_a85_encode(PyObject *module, PyObject *args)
@@ -85,27 +124,24 @@
 	unsigned long	block, res;
 	char			*buf;
 	PyObject		*retVal=NULL, *inObj, *_o1=NULL;
 	if(!PyArg_ParseTuple(args, "O", &inObj)) return NULL;
 	if(PyUnicode_Check(inObj)){
 		_o1 = PyUnicode_AsLatin1String(inObj);
 		if(!_o1){
-			PyErr_SetString(PyExc_ValueError,"argument not decodable as latin1");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not decodable as latin1");
 			}
 		inData = PyBytes_AsString(_o1);
 		inObj = _o1;
 		if(!inData){
-			PyErr_SetString(PyExc_ValueError,"argument not converted to internal char string");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not converted to internal char string");
 			}
 		}
 	else if(!PyBytes_Check(inObj)){
-		PyErr_SetString(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
 		}
 	inData = PyBytes_AsString(inObj);
 	length = PyBytes_GET_SIZE(inObj);
 
 	blocks = length / 4;
 	extra = length % 4;
 
@@ -164,48 +200,41 @@
 		}
 
 	buf[k++] = '~';
 	buf[k++] = '>';
 	retVal = PyUnicode_FromStringAndSize(buf, k);
 	free(buf);
 	if(!retVal){
-		PyErr_SetString(PyExc_ValueError,"failed to create return " STRNAME " value" );
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError,"failed to create return " STRNAME " value" );
 		}
 L_exit:
 	Py_XDECREF(_o1);
 	return retVal;
-L_ERR:
-	ADD_TB(module,"asciiBase85Encode");
-	goto L_exit;
 }
 
 PyObject *_a85_decode(PyObject *module, PyObject *args)
 {
 	unsigned char	*inData, *p, *q, *tmp, *buf;
 	unsigned int	length, blocks, extra, k, num, c1, c2, c3, c4, c5;
 	static unsigned pad[] = {0,0,0xffffff,0xffff,0xff};
 	PyObject		*retVal=NULL, *inObj, *_o1=NULL;
 	if(!PyArg_ParseTuple(args, "O", &inObj)) return NULL;
 	if(PyUnicode_Check(inObj)){
 		_o1 = PyUnicode_AsLatin1String(inObj);
 		if(!_o1){
-			PyErr_SetString(PyExc_ValueError,"argument not decodable as latin1");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not decodable as latin1");
 			}
 		inData = PyBytes_AsString(_o1);
 		inObj = _o1;
 		if(!inData){
-			PyErr_SetString(PyExc_ValueError,"argument not converted to internal char string");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not converted to internal char string");
 			}
 		}
 	else if(!PyBytes_Check(inObj)){
-		PyErr_SetString(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
 		}
 	inData = PyBytes_AsString(inObj);
 	length = (unsigned int)PyBytes_GET_SIZE(inObj);
 	for(k=0,q=inData, p=q+length;q<p && (q=(unsigned char*)strchr((const char*)q,'z'));k++, q++);	/*count 'z'*/
 	length += k*4;
 	tmp = q = (unsigned char*)malloc(length+1);
 	while(inData<p && (k = *inData++)){
@@ -218,17 +247,16 @@
 		else
 			*q++ = k;
 		}
 	inData = tmp;
 	length = (unsigned int)(q - inData);
 	buf = inData+length-2;
 	if(buf[0]!='~' || buf[1]!='>'){
-		PyErr_SetString(PyExc_ValueError, "Invalid terminator for Ascii Base 85 Stream");
 		free(inData);
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError, "Invalid terminator for Ascii Base 85 Stream");
 		}
 	length -= 2;
 	buf[0] = 0;
 
 	blocks = length / 5;
 	extra = length % 5;
 
@@ -263,48 +291,45 @@
 				}
 			}
 		}
 	retVal = PyBytes_FromStringAndSize((const char*)buf, k);
 	free(buf);
 	free(tmp);
 	if(!retVal){
-		PyErr_SetString(PyExc_ValueError,"failed to create return " BYTESNAME " value" );
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError,"failed to create return " BYTESNAME " value" );
 		}
 L_exit:
 	Py_XDECREF(_o1);
 	return retVal;
-L_ERR:
-	ADD_TB(module,"asciiBase85Decode");
-	goto L_exit;
 }
 
 static	char* _fp_fmts[]={"%.0f", "%.1f", "%.2f", "%.3f", "%.4f", "%.5f", "%.6f"};
 static	char *_fp_one(PyObject* module,PyObject *pD)
 {
 	double	d, ad;
 	static	char s[30];
 	int l;
 	char*	dot;
-	if((pD=PyNumber_Float(pD))){
-		d = PyFloat_AS_DOUBLE(pD);
-		Py_DECREF(pD);
+	PyObject *cD;
+	if((cD=PyNumber_Float(pD))){
+		d = PyFloat_AS_DOUBLE(cD);
+		Py_DECREF(cD);
 		}
 	else {
-		PyErr_SetString(PyExc_ValueError, "bad numeric value");
+		EXC_SET(PyExc_ValueError, "bad numeric value %S",pD);
 		return NULL;
 		}
 	ad = fabs(d);
 	if(ad<=1.0e-7){
 		s[0]='0';
 		s[1]=0;
 		}
 	else{
 		if(ad>1e20){
-			PyErr_SetString(PyExc_ValueError, "number too large");
+			EXC_SET(PyExc_ValueError, "number too large %S",pD);
 			return NULL;
 			}
 		if(ad>1) l = min(max(0,6-(int)log10(ad)),6);
 		else l = 6;
 		sprintf(s,_fp_fmts[l], d);
 		if(l){
 			l = (int)strlen(s)-1;
@@ -347,15 +372,15 @@
 			if(retVal){
 				pD = _fp_one(module,retVal);
 				Py_DECREF(retVal);
 				}
 			else pD = NULL;
 			if(!pD){
 				free(buf);
-				return NULL;
+				EXC_EXIT(PyExc_ValueError,"_fp_one failed");
 				}
 			if(pB!=buf){
 				*pB++ = ' ';
 				}
 			strcpy(pB,pD);
 			pB = pB + strlen(pB);
 			}
@@ -363,15 +388,15 @@
 		retVal = PyUnicode_FromString(buf);
 		free(buf);
 		return retVal;
 		}
 	else {
 		PyErr_Clear();
 		PyArg_ParseTuple(args, "O:_fp_str", &retVal);
-		return NULL;
+L_exit: return NULL;
 		}
 }
 
 static PyObject *_escapePDF(unsigned char* text, Py_ssize_t textlen)
 {
 	unsigned char*	out = PyMem_Malloc((textlen<<2)+1);
 	int				j=0, i=0;
@@ -403,37 +428,31 @@
 	Py_ssize_t		length;
 	PyObject		*retVal=NULL, *inObj, *_o1=NULL;
 
 	if (!PyArg_ParseTuple(args, "O:escapePDF", &inObj)) return NULL;
 	if(PyUnicode_Check(inObj)){
 		_o1 = PyUnicode_AsLatin1String(inObj);
 		if(!_o1){
-			PyErr_SetString(PyExc_ValueError,"argument not decodable as latin1");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not decodable as latin1");
 			}
 		inData = PyBytes_AsString(_o1);
 		inObj = _o1;
 		if(!inData){
-			PyErr_SetString(PyExc_ValueError,"argument not converted to internal char string");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError,"argument not converted to internal char string");
 			}
 		}
 	else if(!PyBytes_Check(inObj)){
-		PyErr_SetString(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
-		ERROR_EXIT();
+		EXC_EXIT(PyExc_ValueError,"argument should be " BYTESNAME " or latin1 decodable " STRNAME);
 		}
 	inData = PyBytes_AsString(inObj);
 	length = PyBytes_GET_SIZE(inObj);
 	retVal = _escapePDF(inData,length);
 L_exit:
 	Py_XDECREF(_o1);
 	return retVal;
-L_ERR:
-	ADD_TB(module,"excapePDF");
-	goto L_exit;
 }
 
 static PyObject *sameFrag(PyObject *module, PyObject* args)
 {
 	PyObject *f, *g;
 	static char *names[] = {"fontName", "fontSize", "textColor", "rise", "us_lines", "link", "backColor", "nobr", NULL};
 	int	r=0, t;
@@ -531,15 +550,15 @@
 	Py_XDECREF(value);
 	Py_XDECREF(tb);
 	return result;
 }
 static PyObject *_GetAttrString(PyObject *obj, char *name)
 {
 	PyObject *res = PyObject_GetAttrString(obj, name);
-	if(!res) PyErr_SetString(PyExc_AttributeError, name);
+	if(!res) EXC_SET(PyExc_AttributeError, "missing attribute %s",name);
 	return res;
 }
 
 /* Get a UTF8 encoded string buffer, the return value is the PyObject
    holding the memory for the buffer and should be decrefed to free
    memory */
 static PyObject *_GetStringBuf(PyObject *obj, const char **buf)
@@ -553,16 +572,15 @@
 		}
 	else if(PyBytes_Check(obj)){
 		res = obj;
 		Py_INCREF(res);
 		*buf = PyBytes_AsString(res);
 		}
 	else{
-		PyErr_SetString(PyExc_ValueError,
-				"require bytes or unicode object");
+		EXC_SET(PyExc_ValueError, "require bytes or unicode object");
 		return NULL;
 		}
 	return res;
 }
 
 
 static PyObject *unicode2T1(PyObject *module, PyObject *args, PyObject *kwds)
@@ -576,124 +594,123 @@
 	if (!PyArg_ParseTupleAndKeywords(args, kwds, "OO", argnames, &utext, &fonts)) return NULL;
 	Py_INCREF(utext);
 	Py_INCREF(fonts);
 	R = Py_None; Py_INCREF(Py_None);
 	font = Py_None; Py_INCREF(Py_None);
 
 
-	_o2 = PyList_New(0); if(!_o2) ERROR_EXIT();
+	_o2 = PyList_New(0); if(!_o2) EXC_EXIT(PyExc_MemoryError,"unable to create list");
 	Py_DECREF(R);
 	R = _o2;
 	_o2 = NULL;
 
-	_o2 = PySequence_GetItem(fonts,0); if(!_o2) ERROR_EXIT();
-	_o1 = PySequence_GetSlice(fonts, 1, 0x7fffffff); if(!_o1) ERROR_EXIT();
+	_o2 = PySequence_GetItem(fonts,0); if(!_o2) EXC_EXIT(PyExc_IndexError,"fonts[0] failed");
+	_o1 = PySequence_GetSlice(fonts, 1, 0x7fffffff); if(!_o1) EXC_EXIT(PyExc_IndexError,"fonts[1:] failed");
 	Py_DECREF(font);
 	font = _o2;
 	Py_DECREF(fonts);
 	fonts = _o1;
 	_o1 = _o2 = NULL;
 
-	_o2 = _GetAttrString(font, "encName"); if(!_o2) ERROR_EXIT();
+	_o2 = _GetAttrString(font, "encName"); if(!_o2) EXC_EXIT(PyExc_AttributeError,"no encName");
 	encObj = _GetStringBuf(_o2, &encStr);
 	Py_DECREF(_o2);
 	_o2 = NULL;
-	if (!encObj) ERROR_EXIT();
+	if (!encObj) EXC_EXIT(PyExc_TypeError,"could not convert str(font.encName) failed");
 	if(strstr(encStr,"UCS-2")) encStr = "UTF16";
 
 	while((_i1=PyObject_IsTrue(utext))>0){
 		if((_o1 = PyUnicode_AsEncodedString(utext, encStr, NULL))){
-			_o2 = PyTuple_New(2); if(!_o2) ERROR_EXIT();
+			_o2 = PyTuple_New(2); if(!_o2) EXC_EXIT(PyExc_MemoryError,"create tuple length 2 failed");
 			Py_INCREF(font);
 			PyTuple_SET_ITEM(_o2, 0, font);
 			PyTuple_SET_ITEM(_o2, 1, _o1);
 			_o1 = NULL;
-			if(PyList_Append(R, _o2)) ERROR_EXIT();
+			if(PyList_Append(R, _o2)) EXC_EXIT(PyExc_RuntimeError,"could not append to result list");
 			Py_DECREF(_o2); _o2 = NULL;
 			break;
 			}
 		else{
 			Py_XDECREF(_o1); _o1 = NULL;
-			if(!PyErr_ExceptionMatches(PyExc_UnicodeEncodeError)) ERROR_EXIT();
-			_o1 = _GetExcValue(); if(!_o1) ERROR_EXIT();
+			if(!PyErr_ExceptionMatches(PyExc_UnicodeEncodeError)) EXC_EXIT(PyExc_RuntimeError,"unexpected exception");
+			_o1 = _GetExcValue(); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"could not obtain exception value");
 			PyErr_Clear();
-			_o2 = _GetAttrString(_o1, "args"); if(!_o2) ERROR_EXIT();
+			_o2 = _GetAttrString(_o1, "args"); if(!_o2) EXC_EXIT(PyExc_AttributeError,"missing args attribute");
 			Py_DECREF(_o1);
-			_o1 = PySequence_GetSlice(_o2, 2, 4); if(!_o1) ERROR_EXIT();
+			_o1 = PySequence_GetSlice(_o2, 2, 4); if(!_o1) EXC_EXIT(PyExc_IndexError,"args[2:4] failed");
 			Py_DECREF(_o2);
-			_o2 = PySequence_GetItem(_o1, 0); if(!_o2) ERROR_EXIT();
-			i = PyLong_AsLong(_o2); if(PyErr_Occurred()) ERROR_EXIT();
+			_o2 = PySequence_GetItem(_o1, 0); if(!_o2) EXC_EXIT(PyExc_IndexError,"args[2:4][0] failed");
+			i = PyLong_AsLong(_o2); if(PyErr_Occurred()) EXC_EXIT(PyExc_ValueError,"int(args[2:4][0]) failed");
 			Py_DECREF(_o2);
 
-			_o2 = PySequence_GetItem(_o1, 1); if(!_o1) ERROR_EXIT();
-			j = PyLong_AsLong(_o2); if(PyErr_Occurred()) ERROR_EXIT();
+			_o2 = PySequence_GetItem(_o1, 1); if(!_o1) EXC_EXIT(PyExc_IndexError,"args[2:4][1] failed");
+			j = PyLong_AsLong(_o2); if(PyErr_Occurred()) EXC_EXIT(PyExc_ValueError,"int(args[2:4][1]) failed");
 			Py_DECREF(_o2);
 
 			Py_DECREF(_o1); _o2 = _o1 = 0;
 
 			if(i){
-				_o1 = PySequence_GetSlice(utext, 0, i); if(!_o1) ERROR_EXIT();
-				_o2 = PyUnicode_AsEncodedString(_o1, encStr, NULL); if(!_o2) ERROR_EXIT();
+				_o1 = PySequence_GetSlice(utext, 0, i); if(!_o1) EXC_EXIT(PyExc_IndexError,"utext[0:%d] failed",i);
+				_o2 = PyUnicode_AsEncodedString(_o1, encStr, NULL); if(!_o2) EXC_EXIT(PyExc_UnicodeEncodeError,"encode(utext[0:%d],'%s') failed",i,encStr);
 				Py_DECREF(_o1);
-				_o1 = PyTuple_New(2); if(!_o1) ERROR_EXIT();
+				_o1 = PyTuple_New(2); if(!_o1) EXC_EXIT(PyExc_MemoryError,"create tuple of length 2 failed");
 				Py_INCREF(font);
 				PyTuple_SET_ITEM(_o1, 0, font);
 				PyTuple_SET_ITEM(_o1, 1, _o2);
 				_o2 = NULL;
-				if(PyList_Append(R, _o1)) ERROR_EXIT();
+				if(PyList_Append(R, _o1)) EXC_EXIT(PyExc_RuntimeError,"could not append to result list");
 				Py_DECREF(_o1); _o1 = NULL;
 				}
 
-			_i2 = PyObject_IsTrue(fonts); if(_i2<0) ERROR_EXIT();
+			_i2 = PyObject_IsTrue(fonts); if(_i2<0) EXC_EXIT(PyExc_ValueError,"bool(fonts) is not True");
 			if(_i2){
-				_o1 = PySequence_GetSlice(utext, i, j); if(!_o1) ERROR_EXIT();
-				_o2 = PyTuple_New(2); if(!_o2) ERROR_EXIT();
+				_o1 = PySequence_GetSlice(utext, i, j); if(!_o1) EXC_EXIT(PyExc_IndexError,"utext[%d:%d] failed",i,j);
+				_o2 = PyTuple_New(2); if(!_o2) EXC_EXIT(PyExc_MemoryError,"create tuple of length 2 failed");
 				PyTuple_SET_ITEM(_o2, 0, _o1);
 				Py_INCREF(fonts);
 				PyTuple_SET_ITEM(_o2, 1, fonts);
-				_o1 = unicode2T1(module,_o2,NULL); if(!_o1) ERROR_EXIT();
+				_o1 = unicode2T1(module,_o2,NULL); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"PyTuple_SET_ITEM(_o2,1,fonts) failed");
 				Py_DECREF(_o2); _o2 = 0;
-				_o3 = PyTuple_New(1); if(!_o3) ERROR_EXIT();
+				_o3 = PyTuple_New(1); if(!_o3) EXC_EXIT(PyExc_MemoryError,"create tuple of length 1 failed");
 				PyTuple_SET_ITEM(_o3, 0, _o1);
-				_o1 = _GetAttrString(R, "extend"); if(!_o1) ERROR_EXIT();
-				_o2 = PyObject_CallObject(_o1, _o3); if(!_o2) ERROR_EXIT();
+				_o1 = _GetAttrString(R, "extend"); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"no attriute extend");
+				_o2 = PyObject_CallObject(_o1, _o3); if(!_o2) EXC_EXIT(PyExc_TypeError,"result.extend call failed");
 				Py_DECREF(_o1);
 				Py_DECREF(_o3);
 				Py_DECREF(_o2); _o1 = _o2 = _o3 = NULL;
 				}
 			else{
 				_o3 = _GetAttrString(font,"_notdefChar");
-				if(!_o3) ERROR_EXIT();
-				_o2 = PyLong_FromLong((j - i)); if(!_o2) ERROR_EXIT();
-				_o1 = PyNumber_Multiply(_o3, _o2); if(!_o1) ERROR_EXIT();
+				if(!_o3) EXC_EXIT(PyExc_RuntimeError,"missing _notdefChar");
+				_o2 = PyLong_FromLong((j - i)); if(!_o2) EXC_EXIT(PyExc_ValueError,"int((%d - %d)) failed",j,i);
+				_o1 = PyNumber_Multiply(_o3, _o2); if(!_o1) EXC_EXIT(PyExc_ArithmeticError,"_notdefChar multiply failed");
 				Py_DECREF(_o2); Py_DECREF(_o3); _o2=_o3=NULL;
-				_o2 = PyTuple_New(2); if(!_o2) ERROR_EXIT();
-				_o3 = _GetAttrString(font,"_notdefFont"); if(!_o3) ERROR_EXIT();
+				_o2 = PyTuple_New(2); if(!_o2) EXC_EXIT(PyExc_MemoryError,"create tuple of length 2 failed");
+				_o3 = _GetAttrString(font,"_notdefFont"); if(!_o3) EXC_EXIT(PyExc_AttributeError,"missing _notdefFont");
 				PyTuple_SET_ITEM(_o2, 0, _o3);
 				PyTuple_SET_ITEM(_o2, 1, _o1);
 				Py_INCREF(_o3); _o3=NULL;
 				_o1 = NULL;
-				if(PyList_Append(R, _o2)) ERROR_EXIT();
+				if(PyList_Append(R, _o2)) EXC_EXIT(PyExc_RuntimeError,"Could not append to result");
 				Py_DECREF(_o2); _o2 = NULL;
 				}
 
-			_o1 = PySequence_GetSlice(utext, j, 0x7fffffff); if(!_o1) ERROR_EXIT();
+			_o1 = PySequence_GetSlice(utext, j, 0x7fffffff); if(!_o1) EXC_EXIT(PyExc_IndexError,"utext[%d:] failed",j);
 			Py_DECREF(utext);
 			utext = _o1;
 			_o1 = NULL;
 			}
 		}
-	if(_i1<0) ERROR_EXIT();
+	if(_i1<0) EXC_EXIT(PyExc_ValueError,"_i1=%d became negative",_i1);
 
 	Py_INCREF(R);
 	res = R;
 	goto L_OK;
 
-L_ERR:
-	ADD_TB(module,"unicode2T1");
+L_exit:
 	Py_XDECREF(_o1);
 	Py_XDECREF(_o2);
 	Py_XDECREF(_o3);
 	res = NULL;
 L_OK:
 	Py_XDECREF(encObj);
 	Py_DECREF(R);
@@ -713,89 +730,87 @@
 	int	i, j, s, _i1;
 	static char *argnames[]={"self","text","size","encoding",0};
 	if(!PyArg_ParseTupleAndKeywords(args, kwds, "OOO|O", argnames, &self, &text, &size, &encoding)) return 0;
 	Py_INCREF(text);
 	if(!encoding) encStr="utf8";
 	else {
 		encObj = _GetStringBuf(encoding, &encStr);
-		if(!encObj) ERROR_EXIT();
+		if(!encObj) EXC_EXIT(PyExc_ValueError,"cannot obtain encoding");
 		}
 
 	if(!PyUnicode_Check(text)){
 		if(PyBytes_Check(text)){
 			_o1=PyUnicode_Decode(PyBytes_AS_STRING(text), PyBytes_GET_SIZE(text), encStr,"strict");
-			if(!_o1) ERROR_EXIT();
+			if(!_o1) EXC_EXIT(PyExc_ValueError,"cannot decode text argument");
 			Py_DECREF(text);
 			text = _o1;
 			_o1 = NULL;
 			}
 		else{
-			PyErr_SetString(PyExc_ValueError, "invalid type for argument text");
-			ERROR_EXIT();
+			EXC_EXIT(PyExc_ValueError, "invalid type for argument text");
 			}
 		}
 
-	_o3 = PyList_New(1); if(!_o3) ERROR_EXIT();
+	_o3 = PyList_New(1); if(!_o3) EXC_EXIT(PyExc_MemoryError,"PyList_New(1) failed");
 	Py_INCREF(self);
 	PyList_SET_ITEM(_o3, 0, self);
-	_o2 = _GetAttrString(self, "substitutionFonts"); if(!_o2) ERROR_EXIT();
-	_o1 = PyNumber_Add(_o3, _o2); if(!_o1) ERROR_EXIT();
+	_o2 = _GetAttrString(self, "substitutionFonts"); if(!_o2) EXC_EXIT(PyExc_RuntimeError,"missing substitutionFonts");
+	_o1 = PyNumber_Add(_o3, _o2); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"substitution addition failed");
 	Py_DECREF(_o3); _o3 = 0;
 	Py_DECREF(_o2); _o2 = NULL;
-	_o3 = PyTuple_New(2); if(!_o3) ERROR_EXIT();
+	_o3 = PyTuple_New(2); if(!_o3) EXC_EXIT(PyExc_MemoryError,"PyTuple_New(2) failed");
 	Py_INCREF(text);
 	PyTuple_SET_ITEM(_o3, 0, text);
 	PyTuple_SET_ITEM(_o3, 1, _o1);
 	_o1 = NULL;
-	_o2 = unicode2T1(module,_o3,NULL); if(!_o2) ERROR_EXIT();
+	_o2 = unicode2T1(module,_o3,NULL); if(!_o2) EXC_EXIT(PyExc_RuntimeError,"unicode2T1 call failed");
 	Py_DECREF(_o3); _o3 = NULL;
 	L = _o2;
 	_o2 = NULL;
 
 	n = PyList_GET_SIZE(L);
 
 	for(s=i=0;i<n;++i){
-		_o1 = PyList_GetItem(L,i); if(!_o1) ERROR_EXIT();
+		_o1 = PyList_GetItem(L,i); if(!_o1) EXC_EXIT(PyExc_IndexError,"L[%d] failed",i);
 		Py_INCREF(_o1);
 
-		_o2 = PySequence_GetItem(_o1, 0); if(!_o2) ERROR_EXIT();
+		_o2 = PySequence_GetItem(_o1, 0); if(!_o2) EXC_EXIT(PyExc_IndexError,"L[%d][0] failed",i);
 		Py_XDECREF(f);
 		f = _o2;
 		_o2 = NULL;
 
-		_o2 = _GetAttrString(f, "widths"); if(!_o2) ERROR_EXIT();
+		_o2 = _GetAttrString(f, "widths"); if(!_o2) EXC_EXIT(PyExc_AttributeError,"no widths");
 		Py_DECREF(f);
 		f = _o2;
 		_o2 = NULL;
 
-		_o2 = PySequence_GetItem(_o1, 1); if(!_o2) ERROR_EXIT();
+		_o2 = PySequence_GetItem(_o1, 1); if(!_o2) EXC_EXIT(PyExc_IndexError,"L[%d][1] failed",i);
 		Py_XDECREF(t);
 		t = _o2;
 		Py_DECREF(_o1);
 		_o1 = _o2 = NULL;
 
 		m = PyBytes_Size(t);
 		b = (unsigned char*)PyBytes_AS_STRING(t);
 
 		for(j=0;j<m;++j){
 			_i1 = (long)(b[j]);
-			_o2 = PyList_GetItem(f,_i1); if(!_o2) {PyErr_Format(PyExc_IndexError,"widths index %d out of range",_i1);ERROR_EXIT();}
+			_o2 = PyList_GetItem(f,_i1); if(!_o2) {EXC_EXIT(PyExc_IndexError,"widths index %d out of range",_i1);}
 			_i1 = PyLong_AsLong(_o2);
 			_o2 = NULL;	/*we borrowed this*/
-			if(PyErr_Occurred()) ERROR_EXIT();
+			if(PyErr_Occurred()) EXC_EXIT(PyExc_RuntimeError,"longint conversion failed");
 			s += _i1;
 			}
 		}
 
-	_o1 = PyFloat_FromDouble((s * 0.001)); if(!_o1) ERROR_EXIT();
-	res = PyNumber_Multiply(_o1, size); if(!res) ERROR_EXIT();
+	_o1 = PyFloat_FromDouble((s * 0.001)); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"float(s*0.001) failed");
+	res = PyNumber_Multiply(_o1, size); if(!res) EXC_EXIT(PyExc_RuntimeError,"multiply by size failed");
 	Py_DECREF(_o1);
 	goto L_OK;
-L_ERR:
-	ADD_TB(module,"instanceStringWidthT1");
+L_exit:
 	Py_XDECREF(_o1);
 	Py_XDECREF(_o2);
 	Py_XDECREF(_o3);
 	res = NULL;
 L_OK:
 	Py_XDECREF(encObj);
 	Py_XDECREF(L);
@@ -817,67 +832,67 @@
 	Py_INCREF(text);
 	if(_o1){
 		encoding = _o1;
 		_o1 = NULL;
 		Py_INCREF(encoding);
 		}
 	else{
-		_o1 = PyUnicode_FromString("utf8"); if(!_o1) ERROR_EXIT();
+		_o1 = PyUnicode_FromString("utf8"); if(!_o1) EXC_EXIT(PyExc_UnicodeDecodeError,"utf8 decode failed");
 		encoding = _o1;
 		_o1 = NULL;
 		}
 
 	if(!PyUnicode_Check(text)){
-		i = PyObject_IsTrue(encoding); if(i<0) ERROR_EXIT();
+		i = PyObject_IsTrue(encoding); if(i<0) EXC_EXIT(PyExc_RuntimeError,"truth(encoding)=%d",i);
 		if(!i){
 			Py_DECREF(encoding);
-			encoding = PyUnicode_FromString("utf8"); if(!encoding) ERROR_EXIT();
+			encoding = PyUnicode_FromString("utf8"); if(!encoding) EXC_EXIT(PyExc_UnicodeDecodeError,"utf8 decode failed");
 			}
-		_o1 = _GetAttrString(text, "decode"); if(!_o1) ERROR_EXIT();
-		_o3 = PyTuple_New(1); if(!_o3) ERROR_EXIT();
+		_o1 = _GetAttrString(text, "decode"); if(!_o1) EXC_EXIT(PyExc_AttributeError,"missing attribute decode");
+		_o3 = PyTuple_New(1); if(!_o3) EXC_EXIT(PyExc_MemoryError,"PyTuple_New(1) failed");
 		Py_INCREF(encoding);
 		PyTuple_SET_ITEM(_o3, 0, encoding);
-		_o2 = PyObject_CallObject(_o1, _o3); if(!_o2) ERROR_EXIT();
+		_o2 = PyObject_CallObject(_o1, _o3); if(!_o2) EXC_EXIT(PyExc_RuntimeError,"call of decode attribute failed");
 		Py_DECREF(_o1);
 		Py_DECREF(_o3); _o1 = _o3 = NULL;
 		Py_DECREF(text);
 		text = _o2; /*no _o2=NULL as we assign there straight away*/ 
 		}
 
 	/*self.face.charWidths --> _o1, self.face.defaultWidth --> _o3*/
-	_o2 = _GetAttrString(self, "face"); if(!_o2) ERROR_EXIT();
-	_o1 = _GetAttrString(_o2, "charWidths"); if(!_o1) ERROR_EXIT(); if(!PyDict_Check(_o1)){PyErr_SetString(PyExc_TypeError, "TTFontFace instance charWidths is not a dict");ERROR_EXIT();}
-	_o3 = _GetAttrString(_o2, "defaultWidth"); if(!_o3) ERROR_EXIT();
+	_o2 = _GetAttrString(self, "face"); if(!_o2) EXC_EXIT(PyExc_AttributeError,"missing attribute face");
+	_o1 = _GetAttrString(_o2, "charWidths"); if(!_o1) EXC_EXIT(PyExc_AttributeError,"no attribute charWidths");
+	if(!PyDict_Check(_o1)){EXC_EXIT(PyExc_TypeError, "TTFontFace instance charWidths is not a dict");}
+	_o3 = _GetAttrString(_o2, "defaultWidth"); if(!_o3) EXC_EXIT(PyExc_AttributeError,"missing attribute defaultWidth");
 	Py_DECREF(_o2); _o2 = NULL;
 	dw = PyFloat_AsDouble(_o3);
-	if(PyErr_Occurred()) ERROR_EXIT();
+	if(PyErr_Occurred()) EXC_EXIT(PyExc_RuntimeError,"float() failed");
 	Py_DECREF(_o3);	_o3=NULL;
 
 	n = PyUnicode_GET_SIZE(text);
 	b = PyUnicode_AS_UNICODE(text);
 
 	for(s=i=0;i<n;++i){
-		_o3 = PyLong_FromLong((long)b[i]); if(!_o3) ERROR_EXIT();
+		_o3 = PyLong_FromLong((long)b[i]); if(!_o3) EXC_EXIT(PyExc_RuntimeError,"FromLong failed");
 		_o2 = PyDict_GetItem(_o1,_o3);
 		Py_DECREF(_o3); _o3 = NULL;
 		if(!_o2) _d1 = dw;
 		else{
 			_d1 = PyFloat_AsDouble(_o2);
 			_o2=NULL;	/*no decref as we borrowed it*/
-			if(PyErr_Occurred()) ERROR_EXIT();
+			if(PyErr_Occurred()) EXC_EXIT(PyExc_RuntimeError,"float-->double failed");
 			}
 		s += _d1;
 		}
 	Py_DECREF(_o1);
-	_o1 = PyFloat_FromDouble((s * 0.001)); if(!_o1) ERROR_EXIT();
-	res = PyNumber_Multiply(_o1, size); if(!res) ERROR_EXIT();
+	_o1 = PyFloat_FromDouble((s * 0.001)); if(!_o1) EXC_EXIT(PyExc_RuntimeError,"float(s*0.001) failed");
+	res = PyNumber_Multiply(_o1, size); if(!res) EXC_EXIT(PyExc_RuntimeError,"multiply by size failed");
 	Py_DECREF(_o1);
 	goto L_OK;
-L_ERR:
-	ADD_TB(module,"instanceStringWidthTTF");
+L_exit:
 	Py_XDECREF(_o1);
 	Py_XDECREF(_o2);
 	Py_XDECREF(_o3);
 	res = NULL;
 L_OK:
 	Py_DECREF(text);
 	Py_DECREF(encoding);
@@ -926,15 +941,15 @@
 	if(value==Py_None){
 		self->is_none = 1;
 		}
 	else {
 		char *v = PyBytes_AsString(value);
 		if(!v) return -1;
 		if(PyBytes_GET_SIZE(value)!=1){
-			PyErr_Format(PyExc_AttributeError,"Bad size %d('%s') for attribute character",PyBytes_GET_SIZE(value),v);
+			EXC_SET(PyExc_AttributeError,"Bad size %d('%s') for attribute character",PyBytes_GET_SIZE(value),v);
 			return -1;
 			}
 		self->character = v[0];
 		self->is_none = 0;
 		}
 
 	return 0;
@@ -948,16 +963,16 @@
 	else if(!strcmp(name,"shrink")) return Box_set_double(name,&self->shrink,value);
 	else if(!strcmp(name,"penalty")) return Box_set_double(name,&self->penalty,value);
 	else if(!strcmp(name,"flagged")) return Box_set_int(name,&self->flagged,value);
 	else if(
 			!strcmp(name,"is_penalty") ||
 			!strcmp(name,"is_box") ||
 			!strcmp(name,"is_glue")
-			) PyErr_Format(PyExc_AttributeError, "readonly attribute %s", name);
-	else PyErr_Format(PyExc_AttributeError, "no attribute %s", name);
+			) EXC_SET(PyExc_AttributeError, "readonly attribute %s", name);
+	else EXC_SET(PyExc_AttributeError, "no attribute %s", name);
 	return -1;
 }
 
 static double _Glue_compute_width(BoxObject *self, double r)
 {
 	if(self->is_glue) return self->width+r*(r<0?self->shrink:self->stretch);
 	return self->width;
@@ -1207,14 +1222,16 @@
 
 #ifdef	HAVE_BOX
 #define _BOX__DOC__ \
 	"\tBox(width,character=None) creates a Knuth character Box with the specified width.\n" \
 	"\tGlue(width,stretch,shrink) creates a Knuth glue Box with the specified width, stretch and shrink.\n" \
 	"\tPenalty(width,penalty,flagged=0) creates a Knuth penalty Box with the specified width and penalty.\n" \
 	"\tBoxList() creates a knuth box list.\n"
+#else
+#define _BOX__DOC__
 #endif
 
 PyDoc_STRVAR(__DOC__,
 "_rl_accel contains various accelerated utilities\n\
 \n\
 \tescapePDF makes a unicode or latin1 bytes safe for PDF\n\
 \n\
@@ -1252,30 +1269,30 @@
 	};
 
 /*Initialization function for the module*/
 static struct PyModuleDef moduledef = {
 	PyModuleDef_HEAD_INIT,
 	"_rl_accel",
 	__DOC__,
-	sizeof(struct module_state),
+	MODULE_STATE_SIZE,
 	_methods,
 	NULL,
 	NULL,
 	NULL,
 	NULL
 	};
 
 PyMODINIT_FUNC PyInit__rl_accel(void)
 {
 	PyObject			*module=NULL, *moduleVersion=NULL;
 	/*Create the module and add the functions and module doc string*/
 	module = PyModule_Create(&moduledef);
 	if(!module) goto err;
 	/*Add some symbolic constants to the module */
-	moduleVersion = PyBytes_FromString(VERSION);
+	moduleVersion = PyUnicode_FromString(VERSION);
 	if(!moduleVersion)goto err;
 	PyModule_AddObject(module, "version", moduleVersion);
 
 #ifdef	HAVE_BOX
 	if(PyType_Ready(&BoxType)<0) goto err;
 	BoxList_type.tp_base = &PyList_Type;
 	if(PyType_Ready(&BoxList_type)<0) goto err;
```

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/hnjalloc.c` & `reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/hnjalloc.h` & `reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.c` & `reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.h` & `reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.h`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/hyphen.mashed` & `reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.mashed`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/pyHnjmodule.c` & `reportlab-3.6.9/src/rl_addons/rl_accel/pyHnjmodule.c`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/getrc.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/getrc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t0.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t0.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t1.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t2.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t3.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t4.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/src/rl_addons/rl_accel/tests/t5.py` & `reportlab-3.6.9/src/rl_addons/rl_accel/tests/t5.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/00readme.txt` & `reportlab-3.6.9/tests/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/7x11.jpg` & `reportlab-3.6.9/tests/7x11.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/_i_am_actually_a_gif.jpg` & `reportlab-3.6.9/tests/_i_am_actually_a_gif.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/_i_am_actually_a_jpeg.gif` & `reportlab-3.6.9/tests/_i_am_actually_a_jpeg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/alpha_test.png` & `reportlab-3.6.9/tests/alpha_test.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/barcode-out/ECC200DataMatrix.gif` & `reportlab-3.6.9/tests/barcode-out/ECC200DataMatrix.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/barcode-out/test_cbcim.gif` & `reportlab-3.6.9/tests/barcode-out/test_cbcim.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/barcode-out/test_cbcim.png` & `reportlab-3.6.9/tests/barcode-out/test_cbcim.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/barcode-out/test_cbcim.tiff` & `reportlab-3.6.9/tests/barcode-out/test_cbcim.tiff`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.gif`

 * *Files 25% similar despite different names*

#### gifbuild

```diff
@@ -15,50 +15,51 @@
 	rgb 250 250 250
 	rgb 248 248 248
 	rgb 246 246 246
 	rgb 240 240 240
 	rgb 238 238 238
 	rgb 237 237 237
 	rgb 236 236 236
-	rgb 234 234 234
+	rgb 235 235 235
+	rgb 233 233 233
 	rgb 232 232 232
 	rgb 231 231 231
 	rgb 230 230 230
 	rgb 229 229 229
 	rgb 225 225 225
 	rgb 223 223 223
-	rgb 219 219 219
+	rgb 220 220 220
 	rgb 215 215 215
 	rgb 211 211 211
 	rgb 209 209 209
 	rgb 208 208 208
 	rgb 207 207 207
+	rgb 206 206 206
 	rgb 200 200 200
 	rgb 197 197 197
 	rgb 196 196 196
 	rgb 195 195 195
 	rgb 193 193 193
 	rgb 191 191 191
-	rgb 190 190 190
+	rgb 189 189 189
 	rgb 186 186 186
 	rgb 181 181 181
 	rgb 179 179 179
 	rgb 178 178 178
-	rgb 176 176 176
+	rgb 175 175 175
 	rgb 172 172 172
 	rgb 170 170 170
 	rgb 163 163 163
-	rgb 162 162 162
+	rgb 161 161 161
 	rgb 160 160 160
-	rgb 159 159 159
 	rgb 158 158 158
-	rgb 152 152 152
+	rgb 151 151 151
 	rgb 146 146 146
 	rgb 143 143 143
-	rgb 141 141 141
+	rgb 142 142 142
 	rgb 140 140 140
 	rgb 139 139 139
 	rgb 136 136 136
 	rgb 128 128 128
 	rgb 127 127 127
 	rgb 126 126 126
 	rgb 124 124 124
@@ -258,15 +259,14 @@
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
-	rgb 000 000 000
 end
 
 image # 1
 image left 0
 image top 0
 image interlaced
 image bits 400 by 200 hex
@@ -390,33 +390,33 @@
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000034343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343400000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003447343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434343434344734000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003434000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000035353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353500000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003548353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535353535354835000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003535000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000213c240007322b05400900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000422d0000350400030000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000f4c1123150008370714272c3302002223281b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000029442e00000648081f45093e191c38004817000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004d0d0000004608183c0039201e3b00430b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004b0c0000004608183c003920043a201a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000164e2601000d4a1d2a4510413118493f3c1b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000025140e1230000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000363d2e2f16000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a130300000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000233d260007332c05410900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000432e0000360400030000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000104d1224160008380715292d34020024252a1d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002b452f00000649082146093f1b1e39004918000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004e0e00000047081a3d003a22203c00440b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004c0c0000004708193d003a22043b221c00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000174f2801000d4b1f2b46114232194a403d1d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000027150f1331000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000373e303017000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a140300000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
```

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample0c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4c1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample4d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.gif`

 * *Files 26% similar despite different names*

#### gifbuild

```diff
@@ -14,15 +14,14 @@
 	rgb 251 251 251
 	rgb 250 250 250
 	rgb 249 249 249
 	rgb 248 248 248
 	rgb 247 247 247
 	rgb 246 246 246
 	rgb 245 245 245
-	rgb 244 244 244
 	rgb 243 243 243
 	rgb 242 242 242
 	rgb 241 241 241
 	rgb 240 240 240
 	rgb 239 239 239
 	rgb 237 237 237
 	rgb 236 236 236
@@ -55,19 +54,21 @@
 	rgb 206 206 206
 	rgb 205 205 205
 	rgb 204 204 204
 	rgb 203 203 203
 	rgb 202 202 202
 	rgb 200 200 200
 	rgb 198 198 198
+	rgb 197 197 197
 	rgb 196 196 196
 	rgb 195 195 195
 	rgb 194 194 194
 	rgb 193 193 193
 	rgb 191 191 191
+	rgb 190 190 190
 	rgb 189 189 189
 	rgb 187 187 187
 	rgb 186 186 186
 	rgb 185 185 185
 	rgb 184 184 184
 	rgb 182 182 182
 	rgb 181 181 181
@@ -104,27 +105,29 @@
 	rgb 145 145 145
 	rgb 144 144 144
 	rgb 143 143 143
 	rgb 141 141 141
 	rgb 140 140 140
 	rgb 139 139 139
 	rgb 138 138 138
+	rgb 137 137 137
 	rgb 136 136 136
 	rgb 135 135 135
 	rgb 133 133 133
 	rgb 132 132 132
 	rgb 131 131 131
 	rgb 130 130 130
 	rgb 127 127 127
 	rgb 126 126 126
 	rgb 125 125 125
 	rgb 124 124 124
 	rgb 123 123 123
 	rgb 119 119 119
 	rgb 117 117 117
+	rgb 116 116 116
 	rgb 115 115 115
 	rgb 114 114 114
 	rgb 113 113 113
 	rgb 112 112 112
 	rgb 111 111 111
 	rgb 109 109 109
 	rgb 108 108 108
@@ -139,15 +142,14 @@
 	rgb 098 098 098
 	rgb 097 097 097
 	rgb 096 096 096
 	rgb 095 095 095
 	rgb 094 094 094
 	rgb 093 093 093
 	rgb 092 092 092
-	rgb 091 091 091
 	rgb 090 090 090
 	rgb 088 088 088
 	rgb 087 087 087
 	rgb 086 086 086
 	rgb 085 085 085
 	rgb 084 084 084
 	rgb 083 083 083
@@ -172,18 +174,16 @@
 	rgb 062 062 062
 	rgb 060 060 060
 	rgb 059 059 059
 	rgb 058 058 058
 	rgb 057 057 057
 	rgb 055 055 055
 	rgb 054 054 054
-	rgb 053 053 053
 	rgb 052 052 052
 	rgb 051 051 051
-	rgb 049 049 049
 	rgb 048 048 048
 	rgb 047 047 047
 	rgb 045 045 045
 	rgb 044 044 044
 	rgb 043 043 043
 	rgb 040 040 040
 	rgb 038 038 038
@@ -291,155 +291,155 @@
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001951f00345d6516000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004aa42002aa022186000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000243e8f202aa20001bd5e9191919bbe00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000055b008f2039950000c53042424257bb00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000599084b8902d9c0004c0000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000091111942e02a6012b86000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000721b00355a6a17000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004b938703002e5b6111000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000032200962901a704247f000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001680227a30001bc558383838ebd00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000045fb92439950000c43751515163bb00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000556e2c9b0003c1000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000375304a700278c000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b9f5d5904003d5a6d1d000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000010000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000509f810c0026595d0d000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000153e017b6601a4062978000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000020000436324a50002ba4b75757581bd00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006e1239950000c43d6060606dbc00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003c37002e9a0002c2000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002d3a001305a8002392000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001caf9d9e770044536e22000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000080300000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000007603700001e565708000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000b724500009f092d71000000001eb700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b9f8c6b77bb6b6cc28ba1a1a1a7c46b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006ba16b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6bb7846b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6bc76b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b9f8c6b84b46b6bc68ca1a1a1a17d6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b84b76b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c700000000000000000000000000000000000000000000000000000000000000000069450031990001c300000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c700000000000000000000000000000000000000000000000000000000000000000069450007a900209800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c7000000000000000000000000000000000000000000000000000000000000000010887007004e4a6c2a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006b6b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c70000000000000000000000000000000000000000000000000000000000000000000000000000120a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b80000000434641000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b8a912b0002584c2c00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000328b7a0600125a57120000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008602002c50540200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010b400002a7e00742a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004e0c3bb0005c4d00970700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000034018940008d1b138c00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004cb70307a101435c00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad00006f58004f6f000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000050000a700a32400823a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000651109ba0000b309000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000233fab033a8a001da400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad0000854600448500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002c5900b814007752000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004bb5281fb10000af1f0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000055c00ab0352790012b900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ac00007949004e790000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000007640000b11700814700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004a8313b20000b6140000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000636660ba57477c001db100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad00004867006d48000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000045e05000f7b34009f190000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000187300ab0507ae000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000253939b336199800397b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000024bf2f0002763378020000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000029ea59eaa121a713e64000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000098e4c6215003a5d603a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ab0200633d741a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b0100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000061600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001318000000000e0e000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000016060000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001971d00345e6715000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004ba61f02ab022089000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000233f911f29a40001bd5f9393939dbe00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000055c00911f3a970000c52f43434358bb00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005a9287b8922b9e0004c0000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000091010962e02a8012a89000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000751a00355b6c16000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004c958a03002d5c6210000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000032100982801a9042482000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000016a0226a50001bc5686868690bd00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000460b9233a970000c43752525264bb00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000056702b9d0003c1000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000375404a900268e000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001aa15e5a04003d5b6f1c000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000010000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000051a1840b00255a5e0c000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000143f017e6801a606287b000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000020000446423a70002ba4c78787884bd00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000701139970000c43e6161616fbc00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003c37002d9c0002c2000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002c3c001205aa002294000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001bafa0a07a0045547021000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000080300000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000007613700001d575808000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000b75460000a1092c74000000001db700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6da08e6d7abb6d6ec38da3a3a3a9c46d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006da36d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6db7876d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6dc76d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6da18e6d87b46d6dc68ea3a3a3a3806d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d87b76d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a2380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c70000000000000000000000000000000000000000000000000000000000000000006b4600309b0001c300000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a20000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a2380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c70000000000000000000000000000000000000000000000000000000000000000006b460007aa001f9a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a20000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a2380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c700000000000000000000000000000000000000000000000000000000000000000f8b7207004f4b6e2900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a20000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006d6d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a2380000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c70000000000000000000000000000000000000000000000000000000000000000000000000000110a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000038a20000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a83000000444742000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a8c932a0002594d2b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000318d7d0600115b58110000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008902002b51550200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000fb4000029810077290000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004f0b3cb0005d4e00990700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000034018b41008f1a128e00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004db80207a301445d00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad00007159005071000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000050000a900a52300853b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000671009ba0000b3090000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002240ac023b8c001ca500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad0000884700468800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002b5a00b913007a53000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004cb5271eb10000af1e0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000055c00ac02537c0011b900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad00007c4a004f7c0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000007660000b11500844800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004b8612b20000b6130000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000646861bb58487f001bb100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ad00004969006f49000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000045f05000e7e3300a1180000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000177600ac0507ae000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000243a3ab336189a003a7e00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000023bf2e000279327b02000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002a0a79fab1119733f6500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000009904d6314003b5e613b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ac0200643e771900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000011a0100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000061500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001217000000000d0d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000015060000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
```

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample5d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample6d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample7d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample8b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample9c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_axes_sample_hatching.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample4.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_doughnut_sample4.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample1c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample2c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample3a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_legends_sample4a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample1a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sample3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample1c.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sample2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0a.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample0b.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample4.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample4.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample5.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample5.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample6.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample6.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample7.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample7.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample8.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample8.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample9.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_piecharts_sample9.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_bcleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_bcleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_hlcleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_hlcleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_lpleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_lpleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_pcleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_pcleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_plpleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_plpleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1bar.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1bar.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1barline.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1barline.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1line.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample1line.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2bar.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2bar.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2line.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample2line.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample3.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample3.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample4pie.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_sample4pie.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_scleg.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_special_scleg.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample1.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample1.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample2.gif` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/charts-out/test_graphics_charts_spider_sample2.py` & `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/encryption.gif` & `reportlab-3.6.9/tests/encryption.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/gray-alpha.png` & `reportlab-3.6.9/tests/gray-alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/pythonpowered-gs.gif` & `reportlab-3.6.9/tests/pythonpowered-gs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/pythonpowered.gif` & `reportlab-3.6.9/tests/pythonpowered.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/410.png` & `reportlab-3.6.9/tests/render-out/410.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/410.py` & `reportlab-3.6.9/tests/render-out/410.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing01.gif` & `reportlab-3.6.9/tests/render-out/Drawing01.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing01.png` & `reportlab-3.6.9/tests/render-out/Drawing01.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing01.py` & `reportlab-3.6.9/tests/render-out/Drawing01.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing02.gif` & `reportlab-3.6.9/tests/render-out/Drawing02.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing02.png` & `reportlab-3.6.9/tests/render-out/Drawing02.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing02.py` & `reportlab-3.6.9/tests/render-out/Drawing02.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing03.gif` & `reportlab-3.6.9/tests/render-out/Drawing03.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing03.jpg` & `reportlab-3.6.9/tests/render-out/Drawing03.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing03.png` & `reportlab-3.6.9/tests/render-out/Drawing03.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing03.py` & `reportlab-3.6.9/tests/render-out/Drawing03.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing04.gif` & `reportlab-3.6.9/tests/render-out/Drawing04.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing04.png` & `reportlab-3.6.9/tests/render-out/Drawing04.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing04.py` & `reportlab-3.6.9/tests/render-out/Drawing04.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing05.gif` & `reportlab-3.6.9/tests/render-out/Drawing05.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing05.jpg` & `reportlab-3.6.9/tests/render-out/Drawing05.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing05.png` & `reportlab-3.6.9/tests/render-out/Drawing05.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing05.py` & `reportlab-3.6.9/tests/render-out/Drawing05.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing06.gif` & `reportlab-3.6.9/tests/render-out/Drawing06.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing06.png` & `reportlab-3.6.9/tests/render-out/Drawing06.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing06.py` & `reportlab-3.6.9/tests/render-out/Drawing06.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing07.gif` & `reportlab-3.6.9/tests/render-out/Drawing07.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing07.jpg` & `reportlab-3.6.9/tests/render-out/Drawing07.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing07.png` & `reportlab-3.6.9/tests/render-out/Drawing07.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing07.py` & `reportlab-3.6.9/tests/render-out/Drawing07.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing08.gif` & `reportlab-3.6.9/tests/render-out/Drawing08.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing08.jpg` & `reportlab-3.6.9/tests/render-out/Drawing08.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing08.png` & `reportlab-3.6.9/tests/render-out/Drawing08.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing08.py` & `reportlab-3.6.9/tests/render-out/Drawing08.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing09.gif` & `reportlab-3.6.9/tests/render-out/Drawing09.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing09.jpg` & `reportlab-3.6.9/tests/render-out/Drawing09.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing09.png` & `reportlab-3.6.9/tests/render-out/Drawing09.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing09.py` & `reportlab-3.6.9/tests/render-out/Drawing09.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing10.gif` & `reportlab-3.6.9/tests/render-out/Drawing10.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing10.png` & `reportlab-3.6.9/tests/render-out/Drawing10.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing10.py` & `reportlab-3.6.9/tests/render-out/Drawing10.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing11.gif` & `reportlab-3.6.9/tests/render-out/Drawing11.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing11.png` & `reportlab-3.6.9/tests/render-out/Drawing11.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing11.py` & `reportlab-3.6.9/tests/render-out/Drawing11.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing12.gif` & `reportlab-3.6.9/tests/render-out/Drawing12.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing12.jpg` & `reportlab-3.6.9/tests/render-out/Drawing12.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing12.png` & `reportlab-3.6.9/tests/render-out/Drawing12.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing12.py` & `reportlab-3.6.9/tests/render-out/Drawing12.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing13.gif` & `reportlab-3.6.9/tests/render-out/Drawing13.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing13.png` & `reportlab-3.6.9/tests/render-out/Drawing13.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing13.py` & `reportlab-3.6.9/tests/render-out/Drawing13.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing14.gif` & `reportlab-3.6.9/tests/render-out/Drawing14.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing14.jpg` & `reportlab-3.6.9/tests/render-out/Drawing14.jpg`

 * *Files 26% similar despite different names*

#### Image content

```diff
@@ -1,18 +1,18 @@
                                                        ..X8.
-  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  .  .  .;S;
+  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  .  . . ;%;
    .       .       .       .       .       .       .        
-     .  .    .  .    .  .    .  .    .  .    .  .    .  .   
- .       .       .       .       .       .       .       .  
-   .  .    .  .    .  .    .  .    .  .    .  .    .  .   . 
-  .    .  .    .  .    .  .    .  .    .  .    .  .     .   
-    .       .       .       .       .       .       . .    .
-  .   . .    .  .    .  .    .  .    .  .    .  .        .  
-    .     .    .  .    .  .    .  .    .  .    .  . .  .    
-  .    .   .       .       .       .       .              . 
-     .   .   .  .    .  .    .  .    .  .    .  . .  .  .   
-  .    .      .   .   .   .   .   .   .   .   .       .    .
-    .     . .   .   .   .   .   .   .   .   .    . .     .  
-  .   .           .       .       .       .    .     . .    
-    .   . .  . .     . .     . .     . .     .    .       . 
-  .         .    .       .       .       .     .    .  .    
-:@    . .      .   . .     . .     . .     . .   .      .  .
+     .  .    .  .    .  .    .  .    .  .    .  .    .   .  
+ .       .       .       .       .       .       .          
+   .  .    .  .    .  .    .  .    .  .    .  .    .  .  .  
+  .    .  .    .  .    .  .    .  .    .  .    .  .    .    
+    .       .       .       .       .       .       .     . 
+  .   . .    .  .    .  .    .  .    .  .    .  .    .  .   
+    .     .    .  .    .  .    .  .    .  .    .  .         
+  .    .   .       .       .       .       .       .  .  .  
+     .   .   .  .    .  .    .  .    .  .    .  .    .    . 
+  .    .      .   .   .   .   .   .   .   .   .   .    .    
+    .     . .   .   .   .   .   .   .   .   .   .   .    .  
+  .   .           .       .       .       .       .   .    .
+    .   . .  . .     . .     . .     . .     . .        .   
+  .         .    .       .       .       .       .  . .   . 
+:@    . .      .   . .     . .     . .     . .     .
```

#### Image metadata

```diff
@@ -1,9 +1,9 @@
 Image format: JPEG
-File size: 2181B
+File size: 2183B
 Height: 200
 Width: 400
 Orientation: Undefined
 Compression type: JPEG
 Compression quality: 75
 Colorspace: sRGB
 Channels: srgb
@@ -11,10 +11,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 0
 Y resolution: 0
 Resolution units: Undefined
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 306
+Number of unique colors: 309
 Comment: 
 EXIF data:
```

### Comparing `reportlab-3.6.8/tests/render-out/Drawing14.png` & `reportlab-3.6.9/tests/render-out/Drawing14.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/Drawing14.py` & `reportlab-3.6.9/tests/render-out/Drawing14.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Image
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Image(0,0,None,None,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7FA727365E10>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Image(380,186,20,14,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7FA7273657F0>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Image(0,0,None,None,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7F55C982F750>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Image(380,186,20,14,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7F55C836F5D0>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.8/tests/render-out/autoclose-none.py` & `reportlab-3.6.9/tests/render-out/autoclose-none.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/autoclose-pdf.py` & `reportlab-3.6.9/tests/render-out/autoclose-pdf.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/autoclose-svg.py` & `reportlab-3.6.9/tests/render-out/autoclose-svg.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/fillmode-even-odd.png` & `reportlab-3.6.9/tests/render-out/fillmode-even-odd.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/fillmode-even-odd.py` & `reportlab-3.6.9/tests/render-out/fillmode-even-odd.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/fillmode-non-zero.png` & `reportlab-3.6.9/tests/render-out/fillmode-non-zero.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/fillmode-non-zero.py` & `reportlab-3.6.9/tests/render-out/fillmode-non-zero.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/hatch.png` & `reportlab-3.6.9/tests/render-out/hatch.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/hatch.py` & `reportlab-3.6.9/tests/render-out/hatch.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/svglib-issue104.png` & `reportlab-3.6.9/tests/render-out/svglib-issue104.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/textmode.png` & `reportlab-3.6.9/tests/render-out/textmode.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/render-out/textmode.py` & `reportlab-3.6.9/tests/render-out/textmode.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/rltw-icon-tr.png` & `reportlab-3.6.9/tests/rltw-icon-tr.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/runAll.py` & `reportlab-3.6.9/tests/runAll.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/solid_red_alpha.png` & `reportlab-3.6.9/tests/solid_red_alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_charts_textlabels.py` & `reportlab-3.6.9/tests/test_charts_textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_crypto_algorithms.py` & `reportlab-3.6.9/tests/test_crypto_algorithms.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_docs_build.py` & `reportlab-3.6.9/tests/test_docs_build.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_docstrings.py` & `reportlab-3.6.9/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_extra.py` & `reportlab-3.6.9/tests/test_extra.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_geomutils.py` & `reportlab-3.6.9/tests/test_geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_barcode.py` & `reportlab-3.6.9/tests/test_graphics_barcode.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_charts.py` & `reportlab-3.6.9/tests/test_graphics_charts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_images-cairo.gif` & `reportlab-3.6.9/tests/test_graphics_images-cairo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_images-cairo.png` & `reportlab-3.6.9/tests/test_graphics_images-cairo.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_images.gif` & `reportlab-3.6.9/tests/test_graphics_images.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_images.png` & `reportlab-3.6.9/tests/test_graphics_images.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_images.py` & `reportlab-3.6.9/tests/test_graphics_images.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_layout.py` & `reportlab-3.6.9/tests/test_graphics_layout.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_render.py` & `reportlab-3.6.9/tests/test_graphics_render.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_graphics_speed.py` & `reportlab-3.6.9/tests/test_graphics_speed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_hello.py` & `reportlab-3.6.9/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_images.py` & `reportlab-3.6.9/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_invariant.py` & `reportlab-3.6.9/tests/test_invariant.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_issues.py` & `reportlab-3.6.9/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_colors.py` & `reportlab-3.6.9/tests/test_lib_colors.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_normaldate.py` & `reportlab-3.6.9/tests/test_lib_normaldate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_pdfencrypt.py` & `reportlab-3.6.9/tests/test_lib_pdfencrypt.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_rl_safe_eval.py` & `reportlab-3.6.9/tests/test_lib_rl_safe_eval.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_sequencer.py` & `reportlab-3.6.9/tests/test_lib_sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_utils.py` & `reportlab-3.6.9/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_lib_validators.py` & `reportlab-3.6.9/tests/test_lib_validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_multibyte_chs.py` & `reportlab-3.6.9/tests/test_multibyte_chs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_multibyte_cht.py` & `reportlab-3.6.9/tests/test_multibyte_cht.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_multibyte_jpn.py` & `reportlab-3.6.9/tests/test_multibyte_jpn.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_multibyte_kor.py` & `reportlab-3.6.9/tests/test_multibyte_kor.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_paragraphs.py` & `reportlab-3.6.9/tests/test_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_encodings.py` & `reportlab-3.6.9/tests/test_pdfbase_encodings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_fontembed.py` & `reportlab-3.6.9/tests/test_pdfbase_fontembed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_pdfdoc.py` & `reportlab-3.6.9/tests/test_pdfbase_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_pdfform.py` & `reportlab-3.6.9/tests/test_pdfbase_pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_pdfmetrics.py` & `reportlab-3.6.9/tests/test_pdfbase_pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_pdfutils.py` & `reportlab-3.6.9/tests/test_pdfbase_pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_postscript.py` & `reportlab-3.6.9/tests/test_pdfbase_postscript.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfbase_ttfonts.py` & `reportlab-3.6.9/tests/test_pdfbase_ttfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfgen_callback.py` & `reportlab-3.6.9/tests/test_pdfgen_callback.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfgen_general.py` & `reportlab-3.6.9/tests/test_pdfgen_general.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfgen_links.py` & `reportlab-3.6.9/tests/test_pdfgen_links.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfgen_overprint.py` & `reportlab-3.6.9/tests/test_pdfgen_overprint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pdfgen_pagemodes.py` & `reportlab-3.6.9/tests/test_pdfgen_pagemodes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_accum.py` & `reportlab-3.6.9/tests/test_platypus_accum.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_breaking.py` & `reportlab-3.6.9/tests/test_platypus_breaking.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_cjk_wrap.py` & `reportlab-3.6.9/tests/test_platypus_cjk_wrap.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_general.py` & `reportlab-3.6.9/tests/test_platypus_general.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_images.py` & `reportlab-3.6.9/tests/test_platypus_images.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_indents.py` & `reportlab-3.6.9/tests/test_platypus_indents.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_index.py` & `reportlab-3.6.9/tests/test_platypus_index.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_leftright.py` & `reportlab-3.6.9/tests/test_platypus_leftright.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_lists.py` & `reportlab-3.6.9/tests/test_platypus_lists.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_paragraphs.py` & `reportlab-3.6.9/tests/test_platypus_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_paraparser.py` & `reportlab-3.6.9/tests/test_platypus_paraparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_pleaseturnover.py` & `reportlab-3.6.9/tests/test_platypus_pleaseturnover.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_preformatted.py` & `reportlab-3.6.9/tests/test_platypus_preformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_programming.py` & `reportlab-3.6.9/tests/test_platypus_programming.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_tables.py` & `reportlab-3.6.9/tests/test_platypus_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_toc.py` & `reportlab-3.6.9/tests/test_platypus_toc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_wrapping.py` & `reportlab-3.6.9/tests/test_platypus_wrapping.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_platypus_xref.py` & `reportlab-3.6.9/tests/test_platypus_xref.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_pyfiles.py` & `reportlab-3.6.9/tests/test_pyfiles.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_renderPS.py` & `reportlab-3.6.9/tests/test_renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_renderSVG.py` & `reportlab-3.6.9/tests/test_renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_rl_accel.py` & `reportlab-3.6.9/tests/test_rl_accel.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,20 @@
         L = {}
         LL.reverse()
         for l in LL:
             L.update(l)
     else:
         L = L.copy()
     G0 = G0.copy()
-    return ' '.join([str(getrefcount(eval(x,L,G0))-1) for x in defns.split()])
+    return [getrefcount(eval(x,L,G0))-1 for x in defns.split()]
 
 def checkrc(defns,rcv0):
     if isPyPy: return ''
     rcv1 = getrc(defns,2)
-    return ' '.join(["%s %s-->%s" % (x,v,w) for x,v,w in zip(defns.split(),rcv0.split(),rcv1.split()) if v!=w])
+    return ' '.join(["%s %s-->%s" % (x,v,w) for x,v,w in zip(defns.split(),rcv0,rcv1) if abs(v-w)>1])
 
 class RlAccelTestCase(unittest.TestCase):
 
     def testFpStr(self):
         # should give siz decimal places if less than 1.
         # if more, give up to seven sig figs
         for func, kind in getFuncs('fp_str'):
@@ -115,23 +115,34 @@
         def tfunc(f,ts,fontSize,enc,funcs,i):
             w1 = funcs[i][0](f,ts,fontSize,enc)
             w2 = funcs[1][0](f,ts,fontSize,enc) #python version
             if abs(w1-w2)>=1e-10: F.append("stringWidth%s(%r,%r,%s,%r)-->%r != f._py_stringWidth(...)-->%r" % (fontType,f,ts,fontSize,enc,w1,w2))
         for font,fontType in ((t1f,'T1'),(ttf,'TTF')):
             funcs = getFuncs('instanceStringWidth'+fontType)
             for i,kind in enumerate(('c','py')):
-                for j in (3,2,1,0): #we run several times to allow the refcounts to stabilize
-                    if j: rcv = getrc(defns)
+                for j in (9,8,7,6,5,4,3,2,1,0): #we run several times to allow the refcounts to stabilize
+                    if j==7: rcv = getrc(defns)
                     tfunc(font,testCp1252,fontSize,enc,funcs,i)
                     tfunc(font,ts,fontSize,senc,funcs,i)
                     tfunc(font,utext,fontSize,senc,funcs,i)
-                    if not j:
+                    if j==0:
                         rcc = checkrc(defns,rcv)
                         if rcc: F.append("%s %s refcount diffs (%s)" % (fontType,kind,rcc))
         assert not F,"instanceStringWidth failures\n\t%s" % '\n\t'.join(F)
+        isw = _c_funcs.get('instanceStringWidthTTF',None)
+        if isw:
+            saved = ttf.face.charWidths
+            del ttf.face.charWidths
+            try:
+                w = isw(ttf,'hello world',10)
+            except AttributeError as e:
+                se = str(e)
+                assert 'charWidths' in se,f"expected 'charWidths' not in\n{se!r}"
+            finally:
+                ttf.face.charWidths = saved
 
     def test_unicode2T1(self):
         from reportlab.pdfbase.pdfmetrics import getFont, _fonts
         t1fn = 'Times-Roman'
         t1f = getFont(t1fn)
         enc = 'cp1252'
         senc = 'utf8'
@@ -141,20 +152,32 @@
         def tfunc(f,ts,func,kind):
             w1 = func(ts,[f]+f.substitutionFonts)
             w2 = FUNCS[1][0](ts,[f]+f.substitutionFonts)
             assert w1==w2,"%s unicode2T1 %r != %r" % (kind,w1,w2)
         defns="t1fn t1f testCp1252 enc senc utext t1f.widths t1f.encName t1f.substitutionFonts _fonts"
         F = []
         for func,kind in FUNCS:
-            rcv = getrc(defns)
-            tfunc(t1f,testCp1252,func,kind)
-            tfunc(t1f,utext,func,kind)
-            rcc = checkrc(defns,rcv)
-            if rcc: F.append("%s refcount diffs (%s)" % (kind,rcc))
+            for j in (9,8,7,6,5,4,3,2,1,0): #we run several times to allow the refcounts to stabilize
+                if j==7: rcv = getrc(defns)
+                tfunc(t1f,testCp1252,func,kind)
+                tfunc(t1f,utext,func,kind)
+                if j==0:
+                    rcc = checkrc(defns,rcv)
+                    if rcc: F.append("%s refcount diffs (%s)" % (kind,rcc))
         assert not F,"test_unicode2T1 failures\n\t%s" % '\n\t'.join(F)
+        if FUNCS[0]:
+            t1fencName = t1f.encName
+            del t1f.encName
+            try:
+                FUNCS[0][0](utext,[t1f]+t1f.substitutionFonts)
+            except Exception as e:
+                se = str(e)
+                assert 'encName' in se,f"expected 'encName' not in\n{se!r}"
+            finally:
+                t1f.encName = t1fencName
 
     def test_sameFrag(self):
         class ABag:
             def __init__(self,**kwd):
                 self.__dict__.update(kwd)
             def __str__(self):
                 V=['%s=%r' % v for v in self.__dict__.items()]
```

### Comparing `reportlab-3.6.8/tests/test_source_chars.py` & `reportlab-3.6.9/tests/test_source_chars.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_table_layout.py` & `reportlab-3.6.9/tests/test_table_layout.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_tools_pythonpoint.py` & `reportlab-3.6.9/tests/test_tools_pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_utils.py` & `reportlab-3.6.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_widgetbase_tpc.py` & `reportlab-3.6.9/tests/test_widgetbase_tpc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tests/test_widgets_grids.py` & `reportlab-3.6.9/tests/test_widgets_grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/codegrab.py` & `reportlab-3.6.9/tools/docco/codegrab.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/docpy.py` & `reportlab-3.6.9/tools/docco/docpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/examples.py` & `reportlab-3.6.9/tools/docco/examples.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/graphdocpy.py` & `reportlab-3.6.9/tools/docco/graphdocpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/rl_doc_utils.py` & `reportlab-3.6.9/tools/docco/rl_doc_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/rltemplate.py` & `reportlab-3.6.9/tools/docco/rltemplate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/stylesheet.py` & `reportlab-3.6.9/tools/docco/stylesheet.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/t_parse.py` & `reportlab-3.6.9/tools/docco/t_parse.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/yaml.py` & `reportlab-3.6.9/tools/docco/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/docco/yaml2pdf.py` & `reportlab-3.6.9/tools/docco/yaml2pdf.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pdfpath.py` & `reportlab-3.6.9/tools/pdfpath.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/README` & `reportlab-3.6.9/tools/pythonpoint/README`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/customshapes.py` & `reportlab-3.6.9/tools/pythonpoint/customshapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/examples.py` & `reportlab-3.6.9/tools/pythonpoint/demos/examples.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/figures.xml` & `reportlab-3.6.9/tools/pythonpoint/demos/figures.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/htu.xml` & `reportlab-3.6.9/tools/pythonpoint/demos/htu.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/leftlogo.a85` & `reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/leftlogo.gif` & `reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/lj8100.jpg` & `reportlab-3.6.9/tools/pythonpoint/demos/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/monterey.xml` & `reportlab-3.6.9/tools/pythonpoint/demos/monterey.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/outline.gif` & `reportlab-3.6.9/tools/pythonpoint/demos/outline.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/pplogo.gif` & `reportlab-3.6.9/tools/pythonpoint/demos/pplogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/python.gif` & `reportlab-3.6.9/tools/pythonpoint/demos/python.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/pythonpoint.xml` & `reportlab-3.6.9/tools/pythonpoint/demos/pythonpoint.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/slidebox.py` & `reportlab-3.6.9/tools/pythonpoint/demos/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/spectrum.png` & `reportlab-3.6.9/tools/pythonpoint/demos/spectrum.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/demos/vertpython.gif` & `reportlab-3.6.9/tools/pythonpoint/demos/vertpython.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/pythonpoint.dtd` & `reportlab-3.6.9/tools/pythonpoint/pythonpoint.dtd`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/pythonpoint.py` & `reportlab-3.6.9/tools/pythonpoint/pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/stdparser.py` & `reportlab-3.6.9/tools/pythonpoint/stdparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/styles/horrible.py` & `reportlab-3.6.9/tools/pythonpoint/styles/horrible.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/styles/htu.py` & `reportlab-3.6.9/tools/pythonpoint/styles/htu.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/styles/modern.py` & `reportlab-3.6.9/tools/pythonpoint/styles/modern.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/styles/projection.py` & `reportlab-3.6.9/tools/pythonpoint/styles/projection.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/pythonpoint/styles/standard.py` & `reportlab-3.6.9/tools/pythonpoint/styles/standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/utils/add_bleed.py` & `reportlab-3.6.9/tools/utils/add_bleed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.8/tools/utils/dumpttf.py` & `reportlab-3.6.9/tools/utils/dumpttf.py`

 * *Files identical despite different names*


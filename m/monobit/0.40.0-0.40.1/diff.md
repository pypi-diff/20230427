# Comparing `tmp/monobit-0.40.0.tar.gz` & `tmp/monobit-0.40.1.tar.gz`

## Comparing `monobit-0.40.0.tar` & `monobit-0.40.1.tar`

### file list

```diff
@@ -1,510 +1,510 @@
--rw-r--r--   0        0        0    26847 2020-02-02 00:00:00.000000 monobit-0.40.0/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.40.0/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.40.0/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.40.0/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/basetypes.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/binary.py
--rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/cachedprops.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/canvas.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/constants.py
--rw-r--r--   0        0        0    57985 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/encoding.py
--rw-r--r--   0        0        0    48755 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/font.py
--rw-r--r--   0        0        0    31744 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/glyph.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/labels.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/magic.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/pack.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/properties.py
--rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/raster.py
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/renderer.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripting.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/storage.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/streams.py
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/struct.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/taggers.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/vector.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/__init__.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/mac.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/bbc.py
--rw-r--r--   0        0        0    41746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/borland.py
--rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dec.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26402 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/geos.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/hurt.py
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pkfont.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/psf.py
--rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/raw.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/signum.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/svg.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/vfont.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/__init__.py
--rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/sfnt.py
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/sfnt_writer.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_d_a_t.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_h_e_d.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_l_o_c.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/__init__.py
--rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/draw.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/hex.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/yaff.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/__init__.py
--rw-r--r--   0        0        0    41619 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/bdf.py
--rw-r--r--   0        0        0    18491 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/hbf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.40.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.40.0/LICENSE
--rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 monobit-0.40.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.40.0/pyproject.toml
--rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 monobit-0.40.0/PKG-INFO
+-rw-r--r--   0        0        0    26847 2020-02-02 00:00:00.000000 monobit-0.40.1/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.40.1/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.40.1/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.40.1/explore.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/basetypes.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/binary.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/cachedprops.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/canvas.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/chart.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/constants.py
+-rw-r--r--   0        0        0    58249 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/encoding.py
+-rw-r--r--   0        0        0    47201 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/font.py
+-rw-r--r--   0        0        0    30606 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/glyph.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/labels.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/magic.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/pack.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/properties.py
+-rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/raster.py
+-rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/renderer.py
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/scripting.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/storage.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/streams.py
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/struct.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/taggers.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/vector.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/__init__.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/KOREAN.TXT
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/freedos/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/ms-linedraw.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/manual/windows-3.1.txt
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/charmaps/xfonts/viscii1.1-1.enc
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/compressors.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/container.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/directory.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/mac.py
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/source.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/tar.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/containers/zip.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/__init__.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/amiga.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/bbc.py
+-rw-r--r--   0        0        0    41778 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/bmfont.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/borland.py
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/cpi.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/daisydot.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/dashen.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/dec.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/dosstart.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/figlet.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/fontx.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/fzx.py
+-rw-r--r--   0        0        0    26408 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/gdos.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/geos.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/hurt.py
+-rw-r--r--   0        0        0    10414 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/image.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mousegraphics.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mzfon.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/nearlyraw.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/palm.py
+-rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/pcl.py
+-rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/pcpaint.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/pdf.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/pkfont.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/printshop.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/psf.py
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/raw.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/signum.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/svg.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/vfont.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/dfont.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/fond.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/iigs.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/lisa.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/mac/nfnt.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/os2/__init__.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/os2/gpifont.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/os2/lx.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/os2/ne.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/text/__init__.py
+-rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/text/draw.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/text/hex.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/text/yaff.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/LICENSE.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/__init__.py
+-rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/fnt.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/mz.py
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/ne.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/windows/pe.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    41478 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.40.1/monobit/scripts/convert.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.40.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.40.1/LICENSE
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 monobit-0.40.1/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.40.1/pyproject.toml
+-rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 monobit-0.40.1/PKG-INFO
```

### Comparing `monobit-0.40.0/YAFF.md` & `monobit-0.40.1/YAFF.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/explore.py` & `monobit-0.40.1/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/__init__.py` & `monobit-0.40.1/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/basetypes.py` & `monobit-0.40.1/monobit/basetypes.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/binary.py` & `monobit-0.40.1/monobit/binary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/cachedprops.py` & `monobit-0.40.1/monobit/streams.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,242 @@
 """
-monobit.cachedprops - defaultable, cached property sets with type conversion
+monobit.streams - file stream tools
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
-
+import io
+import os
+import sys
 import logging
-from types import SimpleNamespace
-from functools import partial, wraps, cache
-from itertools import chain
-from textwrap import indent, wrap
-
-from .basetypes import CONVERTERS
-from .properties import Props, normalise_property
-
+from pathlib import Path
 
 
-class DefaultProps:
-    """
-    Namespace with recognised fields and defaults.
-    Define field types (converters) and defaults in class definition.
-    >>> class MyProps(DefaultProps)
-    >>>    field_1: int
-    >>>    field_2: int = 2
-    >>> p = MyProps()
-    >>> p.field_2
-    >>> 2
-    >>> p.field_1
-    >>> 0
-    where field_1 has an implied default, int() == 0
-    """
-
-    def __init__(self, _comments=None, **kwargs):
-        # disable cacheing while building the object
-        self._set_defaults()
-        self._props = {}
-        [
-            setattr(self, _field, _value)
-            for _field, _value in kwargs.items()
-            #if not _field.startswith('_')
-        ]
-        _comments = _comments or {}
-        self._comments = {
-            normalise_property(_k): _v
-            for _k, _v in _comments.items()
-        }
-        # enable cacheing
-        self._cache = {}
+def get_bytesio(bytestring):
+    """Workaround as our streams objects require a buffer."""
+    return io.BufferedReader(io.BytesIO(bytestring))
+
+def get_stringio(string):
+    """Workaround as our streams objects require a buffer."""
+    return io.TextIOWrapper(get_bytesio(string.encode()))
+
+
+class StreamBase:
+    """Base class for streams."""
+
+    def __init__(self, stream, mode='', name='', where=None):
+        self._stream = stream
+        self.name = name
+        self.mode = mode[:1]
+        if self._stream:
+            if not self.name:
+                self.name = get_name(stream)
+            if not self.mode:
+                try:
+                    self.mode = self._stream.mode[:1]
+                except AttributeError:
+                    if self._stream.readable():
+                        self.mode = 'r'
+                    else:
+                        self.mode = 'w'
+        self._refcount = 0
+        # embedding container
+        self.where = where
+        self.closed = False
+
+    def __enter__(self):
+        self._refcount += 1
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Ensure stream is closed."""
+        if exc_type == BrokenPipeError:
+            return True
+        self._refcount -= 1
+        logging.debug(
+            'Exiting %r with reference count %d. '
+            '[Underlying stream %r]', self, self._refcount, self._stream)
+        if not self._refcount:
+            self.close()
 
     def __repr__(self):
+        """String representation."""
         return (
-            type(self).__name__
-            + '(\n    ' +
-            '\n    '.join(
-                f'{_k}={_v!r},' for _k, _v in self._props.items()
-                if not _k.startswith('_')
-            )
-            + '\n)'
+            f"<{type(self).__name__} name='{self.name}' mode='{self.mode}'"
+            f"{' [closed]' if self.closed else ''}>"
         )
 
-    @classmethod
-    def _set_defaults(cls):
-        """If a type constructor is given in the annotations, use that to set the default."""
-        # if a type constructor is given in the annotations, use that to set the default
-        # note that we're changing the *class* namespace on the *instance* initialiser
-        # which feels a bit hacky
-        # but this will be a no-op after the first instance has initialised
-        if not hasattr(cls, '_init'):
-            # type's attributes - these are the calculated properties
-            cls._attribs = list(vars(cls))
-            try:
-                start = cls._attribs.index('__properties_start__')
-                end = cls._attribs.index('__properties_end__')
-            except ValueError:
-                pass
-            else:
-                # cut back the list, speeds up setattr
-                cls._attribs = cls._attribs[start+1:end]
-            cls._attribs = set(cls._attribs)
-            # types, converters and default values for overriding/custom properties
-            cls._types = {**cls.__annotations__}
-            cls._converters = {
-                _field: CONVERTERS.get(_type, _type)
-                for _field, _type in cls._types.items()
-            }
-            cls._defaults = {
-                # can't use .get() as _type() would fail for some defaulted fields
-                _field: vars(cls)[_field] if _field in vars(cls) else _type()
-                #CONVERTERS(_type, _type)()
-                for _field, _type in cls.__annotations__.items()
-                if _field not in cls._attribs
-            }
-            cls._init = True
+    def close(self):
+        if self._stream and not self._refcount:
+            logging.debug('Closing %r', self)
+            self._stream.close()
+        self.closed = True
+
+
+class StreamWrapper(StreamBase):
+    """Wrapper object to emulate a single text stream."""
+
+    def __getattr__(self, attr):
+        """Delegate undefined attributes to wrapped stream."""
+        return getattr(self._stream, attr)
+
+    def __iter__(self):
+        # dunder methods not delegated
+        return self._stream.__iter__()
+
+
+class KeepOpen(StreamWrapper):
+    """Wrapper to avoid closing wrapped stream."""
+
+    def close(self):
+        """Don't close underlying stream."""
+        self._stream.flush()
+
+
+class Stream(StreamWrapper):
+    """Manage file resource."""
+
+    def __init__(self, file, mode, *, name='', where=None):
+        """
+        Ensure file is a stream of the right type, open or wrap if necessary.
+
+        file: stream or file-like object
+        mode: 'r' or 'w'
+        where: embedding container
+        """
+        if not file:
+            raise ValueError('No stream provided.')
+        mode = mode[:1]
+        if isinstance(file, (str, Path)):
+            raise ValueError('Argument `file` must be a Python file or stream-like object.')
+        # initialise wrapper
+        super().__init__(file, mode=mode, name=name, where=where)
+        # check r/w mode is consistent
+        self._ensure_rw()
+        # Ensure we have a binary stream
+        self._ensure_binary()
+        if mode == 'r' and not self._stream.seekable():
+            # we need streams to be seekable - drain to buffer
+            # note you can only do this once on the input stream!
+            self._stream = get_bytesio(self._stream.read())
+            self._ensure_binary()
+        if mode == 'r':
+            self._anchor = self._stream.tell()
+        else:
+            self._anchor = 0
 
     @classmethod
-    def _get_default(cls, field):
-        """Default value for a property."""
-        return cls._defaults.get(normalise_property(field), None)
-
-    def _defined(self, field):
-        """Writable property has been explicitly set."""
-        return self._props.get(normalise_property(field), None)
+    def from_data(cls, data, **kwargs):
+        """BytesIO stream on bytes data."""
+        # Stream requires a buffer so we wrap
+        return cls(get_bytesio(data), **kwargs)
 
     @classmethod
-    def _known(cls, field):
-        """Field is a writable property."""
-        # note that checked_properties are not included, writable_properties and regular fields are
-        field = normalise_property(field)
-        return field in cls._defaults or field in cls._attribs
-
-    def __getattr__(self, field):
-        if field.startswith('_'):
-            raise AttributeError(field)
-        try:
-            return self._get_property(field)
-        except KeyError as e:
-            raise AttributeError(e)
-
-    def _get_property(self, field):
-        field = normalise_property(field)
-        try:
-            return self._props[field]
-        except KeyError:
-            pass
-        return self._defaults[field]
-
-    def __setattr__(self, field, value):
-        if field.startswith('_'):
-            return super().__setattr__(field, value)
-        field = normalise_property(field)
-        if field in self._attribs:
-            self._cache = {}
-            return super().__setattr__(field, value)
-        return self._set_property(field, value)
-
-    def _set_property(self, field, value):
-        field = normalise_property(field)
-        if value is None:
-            self._props.pop(field, None)
+    def from_string(cls, text, **kwargs):
+        """StringIO stream on string data."""
+        return cls.from_data(text.encode(), **kwargs)
+
+    def _ensure_rw(self):
+        """Ensure r/w mode is consistent."""
+        if self.mode == 'r' and not self._stream.readable():
+            raise ValueError('Expected readable stream, got writable.')
+        if self.mode == 'w' and not self._stream.writable():
+            raise ValueError('Expected writable stream, got readable.')
+
+    def _ensure_binary(self):
+        """Ensure we have a binary stream."""
+        # a text format can be read from/written to a binary stream with a wrapper
+        if not is_binary(self._stream):
+            self._textstream = self._stream
+            try:
+                self._stream = self._stream.buffer
+            except AttributeError as e:
+                raise ValueError('Unable to access binary stream.') from e
+            logging.debug('Getting buffer %r from text stream %r.', self._stream, self._textstream)
         else:
-            # this fails because not all our annotations are actual types
-            #field_type = self._types.get(field, None)
-            #if field_type and not isinstance(field, field_type):
-            converter = self._converters.get(field, None)
-            if converter:
-                value = converter(value)
-            self._props[field] = value
-        self._cache = {}
-
-
-def writable_property(arg=None, *, field=None):
-    """Decorator to take property from property table, if defined; calculate otherwise."""
-    if not callable(arg):
-        return partial(writable_property, field=arg)
-    fn = arg
-    field = field or fn.__name__
-    field = normalise_property(field)
-    cached_fn = delayed_cache(fn)
+            # placeholder for text wrapper
+            self._textstream = None
 
-    @wraps(fn)
-    def _getter(self):
+    @property
+    def text(self):
+        """Return underlying text stream or wrap underlying binary stream with utf-8 wrapper."""
+        if not self._textstream:
+            encoding = 'utf-8-sig' if self.mode == 'r' else 'utf-8'
+            self._textstream = io.TextIOWrapper(
+                self._stream, encoding=encoding,
+                # on the one hand, this avoids breaks on slightly damaged files
+                # on the other hand, we are less likely to break
+                # on files that are clearly not text
+                errors='ignore'
+            )
+        return self._textstream
+
+    def seek(self, loc, whence=0, /):
+        """Seek relative to anchor."""
+        if whence == 0:
+            loc += self._anchor
+        self._stream.seek(loc, whence)
+
+    def tell(self):
+        """Location relative to anchor."""
+        return self._stream.tell() - self._anchor
+
+    def __getattr__(self, attr):
+        """Delegate undefined attributes to wrapped stream."""
+        return getattr(self._stream, attr)
+
+    def close(self):
+        """Close stream, absorb errors."""
+        # always close at wrapper level
+        self.closed = True
+        if self._textstream:
+            try:
+                self._textstream.close()
+            except EnvironmentError:
+                pass
         try:
-            # only use if explicitly set on the instance
-            return self._props[field]
-        except KeyError:
+            super().close()
+        except EnvironmentError:
             pass
-        return cached_fn(self)
-
-    @wraps(fn)
-    def _setter(self, value):
-        #logging.debug(f'Setting overridable property {field}={value}.')
-        self._set_property(field, value)
 
-    return property(_getter, _setter)
 
+class DirectoryStream(Stream):
+    """Fake stream to represent directory."""
 
-def checked_property(fn):
-    """Non-overridable property, attempted writes will be logged and dropped."""
-    field = normalise_property(fn.__name__)
-
-    _getter = delayed_cache(fn)
-
-    @wraps(fn)
-    def _setter(self, value):
-        logging.info(f'Non-overridable property {field} cannot be set to {value}; ignored.')
-
-    return property(_getter, _setter)
-
-
-def as_tuple(arg=None, *, fields=None, tuple_type=None):
-    """
-    Decorator to take summarise multiple fields as a (settable) tuple.
-
-    The decorated function is discarded except for the name, so use as:
-    @as_tuple(('x', 'y'))
-        def coord(): pass
-    """
-    if not callable(arg):
-        return partial(as_tuple, fields=arg, tuple_type=tuple_type)
-    fn = arg
-
-    tuple_type = tuple_type or tuple
-
-    @wraps(fn)
-    def _getter(self):
-        # in this case, always use the fields, whether defaulted or set
-        return tuple_type(tuple(
-            getattr(self, _field)
-            for _field in fields
-        ))
-
-    @wraps(fn)
-    def _setter(self, value):
-        for field, element in zip(fields, tuple_type(value)):
-            self._set_property(field, element)
-
-    return property(_getter, _setter)
-
-
-def delayed_cache(fn):
-    """Cache only once _frozen attribute is set."""
-    field = normalise_property(fn.__name__)
-
-    @wraps(fn)
-    def _getter(self):
-        try:
-            return self._cache[field]
-        except KeyError:
-            pass
-        value = fn(self)
-        self._cache[field] = value
-        return value
-
-    return _getter
+    def __init__(self, file, mode, *, name='', where=None):
+        name = name or str(file)
+        mode = mode[:1]
+        if isinstance(file, DirectoryStream):
+            file = file.name
+        if not isinstance(file, (str, Path)):
+            raise TypeError(
+                'DirectoryStream initialiser must be DirectoryStream, Path or str.'
+            )
+        # path is what should be used to open the actual directory
+        self.path = Path(file)
+        dummystream = open(os.devnull, mode + 'b')
+        # initialise wrapper
+        super().__init__(dummystream, mode=mode, name=name, where=where)
+
+
+###############################################################################
+
+def is_binary(stream):
+    """Check if stream is binary."""
+    if stream.readable():
+        # read 0 bytes - the return type will tell us if this is a text or binary stream
+        return isinstance(stream.read(0), bytes)
+    # write empty bytes - error if text stream
+    try:
+        stream.write(b'')
+    except TypeError:
+        return False
+    return True
+
+def get_name(stream):
+    """Get stream name, if available."""
+    try:
+        return stream.name
+    except AttributeError:
+        # not all streams have one (e.g. BytesIO)
+        return ''
```

### Comparing `monobit-0.40.0/monobit/canvas.py` & `monobit-0.40.1/monobit/canvas.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/chart.py` & `monobit-0.40.1/monobit/chart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/encoding.py` & `monobit-0.40.1/monobit/encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -834,17 +834,25 @@
             )
         ))
 
     def __repr__(self):
         """Representation."""
         return f"{type(self).__name__}(name='{self.name}')"
 
-    def __str__(self):
-        """Yaff representation."""
-        return CharmapRegistry.normalise(self.name)
+
+class EncodingName(str):
+
+    def __new__(cls, value=''):
+        """Convert char or char sequence to char label."""
+        if not isinstance(value, str):
+            raise ValueError(
+                f'Can only convert `str` to encoding name, not `{type(value)}`.'
+            )
+        value = CharmapRegistry.normalise(value)
+        return super().__new__(cls, value)
 
 
 class Charmap(Encoder):
     """Convert between unicode and ordinals using stored mapping."""
 
     # charmap file format parameters
     _formats = {}
```

### Comparing `monobit-0.40.0/monobit/font.py` & `monobit-0.40.1/monobit/font.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,139 +11,137 @@
 from unicodedata import normalize
 
 from .scripting import scriptable, get_scriptables, Any
 from .glyph import Glyph
 from .raster import turn_method
 from .basetypes import Coord, Bounds
 from .basetypes import to_int
-from .encoding import charmaps, encoder
+from .encoding import charmaps, encoder, EncodingName
 from .taggers import tagger
 from .labels import Tag, Char, Codepoint, Label, to_label
 from .binary import ceildiv
-from .properties import normalise_property, extend_string
-from .cachedprops import DefaultProps, writable_property, as_tuple, checked_property
+from .properties import extend_string
+from .cachedprops import HasProps, writable_property, checked_property
 from .taggers import tagmaps
 
 
 # sentinel object
 NOT_SET = object()
 
 
 ###############################################################################
 # font class
 
 # pylint: disable=redundant-keyword-arg, no-member
-class Font(DefaultProps):
+class FontProperties:
     """Representation of font, including glyphs and metadata."""
 
-    # recognised properties and converters from str
+    # recognised properties and types
     # this also defines the default order in yaff files
 
     # naming - can be determined from source file if needed
+
     # full human name
     name: str
     # typeface/font family
     family: str
     # further specifiers
     subfamily: str
     # unique id
-    font_id: str
+    font_id: str = ''
 
     # font metadata
-    # can't be calculated
+
     # author or issuer
-    author: str
+    author: str = ''
     foundry: str
     # copyright string
-    copyright: str
+    copyright: str = ''
     # license string or similar
-    notice: str
+    notice: str = ''
     # font version
     revision: str = '0'
 
     # font description
-    # can't be calculated
+
     # serif, sans, etc.
-    style: str
+    style: str = ''
     # nominal point size
     point_size: float
     # normal, bold, light, ...
     weight: str = 'regular'
     # roman, italic, oblique, ...
     slant: str = 'roman'
     # normal, condensed, expanded, ...
     setwidth: str = 'normal'
     # underline, strikethrough, etc.
-    decoration: str
+    decoration: str = ''
+
+    # rendering target
 
-    # target info
-    # can't be calculated
     # target device name
-    device: str
+    device: str = ''
     # calculated or given
     # pixel aspect ratio - square pixel
     pixel_aspect: Coord = Coord(1, 1)
     # target resolution in dots per inch
     dpi: Coord
 
-    # summarising quantities
-    # determined from the bitmaps only
+    # summarising quantities, determined from bitmaps (not writable)
 
     # proportional, monospace, character-cell, multi-cell
     spacing: str
     # maximum raster (not necessarily ink) width/height
     raster_size: Coord
+    raster: Bounds
     # width, height of the character cell
     cell_size: Coord
     # overall ink bounds - overlay all glyphs with fixed origin and determine maximum ink extent
     bounding_box: Coord
+    ink_bounds: Bounds
     # average advance width, rounded to tenths
     average_width: float
     # maximum glyph advance width
     max_width: int
     # advance width of LATIN CAPITAL LETTER X
     cap_width: int
     # advance width of digits, if fixed.
     digit_width: int
 
     # descriptive typographic quantities
-    # can be calculated or given, may affect rendering
 
     # height of lowercase x relative to baseline
     x_height: int
     # height of capital relative to baseline
     cap_height: int
-    # can't be calculated, affect rendering (vertical positioning)
-    # might affect e.g. composition of characters
+
+    # metrics
+
     # recommended typographic ascent relative to baseline (not necessarily equal to top)
     ascent: int
     # recommended typographic descent relative to baseline (not necessarily equal to bottom)
     descent: int
-    # 'descent' for vertical rendering
-    left_extent: int
-    # 'ascent' for vertical rendering
-    right_extent: int
+    # vertical distance between consecutive baselines, in pixels
+    line_height: int
     # nominal pixel size, always equals ascent + descent
     pixel_size: int
     # vertical interline spacing, defined as line_height - pixel_size
     leading: int
 
-    # metrics
-    # can't be calculated, affect rendering
-
-    # vertical distance between consecutive baselines, in pixels
-    line_height: int
+    # 'descent' for vertical rendering
+    left_extent: int
+    # 'ascent' for vertical rendering
+    right_extent: int
     # horizontal distance between consecutive baselines, in pixels
     line_width: int
 
     # encoding parameters
-    # can't be calculated, affect rendering
 
     # character map, stored as normalised name
-    encoding: charmaps.normalise
+    encoding: EncodingName
     # replacement for missing glyph
     default_char: Label
     # word-break character (usually space)
     word_boundary: Label = Char(' ')
 
     # rendering hints
     # may affect rendering if effects are applied
@@ -179,54 +177,55 @@
     min_word_space: int
     # recommended maximum space between words, in pixels
     max_word_space: int
     # recommended space between sentences, in pixels
     sentence_space: int
 
     # conversion metadata
-    # can't be calculated, informational
-    converter: str
-    source_name: str
-    source_format: str
-    history: str
-
-    # type converters for compatibility synonyms
-    average_advance: float
-    max_advance: int
-    cap_advance: int
+    converter: str = ''
+    source_name: str = ''
+    source_format: str = ''
+    history: str = ''
 
-    # non-overridable, for pylint's benefit
-    raster: Bounds
 
-    __properties_start__ = True
+class Font(HasProps):
+    """Representation of font, including glyphs and metadata."""
+
+    _defaults = vars(FontProperties)
+    _converters = HasProps.get_converters(FontProperties)
+
 
     @writable_property
     def name(self):
         """Full human-friendly name."""
         if self.spacing in ('character-cell', 'multi-cell'):
-            size = 'x'.join(str(_x) for _x in self.cell_size)
+            size = str(self.cell_size)
         else:
             size = str(self.point_size)
-        return ' '.join(
-            _x for _x in (self.family, self.subfamily, size) if _x
-        )
+        try:
+            name = ' '.join(
+                _x for _x in (self.family, self.subfamily, size) if _x
+            )
+        except AttributeError as e:
+            raise
+        return name
 
     @writable_property
     def subfamily(self):
         """Font additional names."""
-        if self.slant == self._get_default('slant'):
+        if self.slant == self.get_default('slant'):
             slant = ''
         else:
             # title-case
             slant = self.slant.title()
-        if self.setwidth == self._get_default('setwidth'):
+        if self.setwidth == self.get_default('setwidth'):
             setwidth = ''
         else:
             setwidth = self.setwidth.title()
-        if (slant or setwidth) and self.weight == self._get_default('weight'):
+        if (slant or setwidth) and self.weight == self.get_default('weight'):
             weight = ''
         else:
             weight = self.weight.title()
         return ' '.join(
             _x for _x in (setwidth, weight, slant) if _x
         )
 
@@ -256,15 +255,15 @@
         # if dpi not given assumes 72 dpi, so point-size == pixel-size
         return int(self.pixel_size * self.dpi.y / 72.)
 
     @writable_property
     def dpi(self):
         """Target screen resolution in dots per inch."""
         # if point-size has been overridden and dpi not set, determine from pixel-size & point-size
-        if self._defined('point-size') is not None:
+        if 'point_size' in self._props:
             dpi = (72 * self.pixel_size) // self.point_size
         else:
             # default: 72 dpi; 1 point == 1 pixel
             dpi = 72
         # stretch/shrink dpi.x if aspect ratio is not square
         return Coord((dpi*self.pixel_aspect.x)//self.pixel_aspect.y, dpi)
 
@@ -278,15 +277,15 @@
 
     ##########################################################################
     # metrics
 
     @writable_property
     def line_height(self):
         """Vertical distance between consecutive baselines, in pixels."""
-        if self._defined('leading') is not None:
+        if 'leading' in self._props:
             return self.pixel_size + self.leading
         return max(self.raster_size.y, self.pixel_size)
 
     @writable_property
     def line_width(self):
         """Horizontal distance between consecutive baselines, in pixels."""
         return self.max_width
@@ -628,56 +627,38 @@
         """Label for default character."""
         repl = '\ufffd'
         if repl not in self.get_chars():
             repl = ''
         return Char(repl)
 
 
-    ##########################################################################
-    # deprecated compatibility synonyms
-
-    @writable_property('average_width')
-    def average_advance(self):
-        """Average advance width, rounded to tenths."""
-        return self.average_width
-
-    @writable_property('max_width')
-    def max_advance(self):
-        """Maximum glyph advance width."""
-        return self.max_width
-
-    @writable_property('cap_width')
-    def cap_advance(self):
-        """Advance width of LATIN CAPITAL LETTER X."""
-        return self.cap_width
-
-
-    __properties_end__ = True
-
     ###########################################################################
 
 
     def __init__(self, glyphs=(), *, comment=None, **properties):
         """Create new font."""
+        super().__init__()
         self._glyphs = tuple(glyphs)
         # construct lookup tables
         self._labels = {
             _label: _index
             for _index, _glyph in enumerate(self._glyphs)
             for _label in _glyph.get_labels()
         }
         # comment can be str (just global comment) or mapping of property comments
         if isinstance(comment, str):
             comment = {'': comment}
+        else:
+            comment = comment or {}
         self._glyphs, properties = self._apply_metrics(self._glyphs, properties)
+        self._comment = {**comment}
         # update properties
-        # set encoding first so we can set labels
         # NOTE - we must be careful NOT TO ACCESS CACHED PROPERTIES
         #        until the constructor is complete
-        super().__init__(**properties, _comments=comment)
+        self._set_properties(properties)
 
     @staticmethod
     def _apply_metrics(glyphs, props):
         """Apply globally specified glyph metrics."""
         glyph_metrics = {
             _k: props[_k]
             for _k in (
@@ -694,32 +675,32 @@
         }
         if glyph_metrics:
             # create a dummy glyph to ensure values get converted to right type
             glob = Glyph(**glyph_metrics)
             # localise glyph metrics
             glyphs = tuple(
                 _g.modify(**{
-                    _k: _g.get_property(_k) + _v
-                    for _k, _v in glob.properties.items()
+                    _k: _g._get_property(_k) + _v
+                    for _k, _v in glob.get_properties().items()
                 })
                 for _g in glyphs
             )
         return glyphs, props
 
 
     ##########################################################################
     # representation
 
     def __repr__(self):
         """Representation."""
         elements = (
             f'glyphs=(...{len(self._glyphs)} glyphs...)' if self._glyphs else '',
             ',\n    '.join(
-                f'{normalise_property(_k)}={repr(_v)}'
-                for _k, _v in self.properties.items()
+                f'{_k}={repr(_v)}'
+                for _k, _v in self.get_properties().items()
             ),
         )
         return '{}({})'.format(
             type(self).__name__,
             ', '.join(_e for _e in elements if _e)
         )
 
@@ -737,18 +718,15 @@
         old_comment = self._get_comment_dict()
         if isinstance(comment, str):
             old_comment[''] = comment
         elif comment is not NOT_SET:
             old_comment.update(comment)
         # comment and properties are replaced keyword by keyword
         properties = {**self._props}
-        properties.update({
-            normalise_property(_k): _v
-            for _k, _v in kwargs.items()
-        })
+        properties.update(kwargs)
         return Font(
             tuple(glyphs),
             comment=old_comment,
             **properties
         )
 
     def append(
@@ -759,15 +737,15 @@
         if not comment:
             comment = {}
         for key, comment in comment.items():
             old_comment = self.get_comment(key)
             if old_comment:
                 comment[key] = extend_string(old_comment, comment)
         for key, value in properties.items():
-            if self._defined(key):
+            if key in self._props:
                 properties[key] = extend_string(self._props[key], value)
         if glyphs:
             glyphs = (*self.glyphs, *glyphs)
         else:
             glyphs = NOT_SET
         return self.modify(glyphs, comment={**comment}, **properties)
 
@@ -781,54 +759,35 @@
             # not in list
             glyphs = NOT_SET
         try:
             args.remove('comment')
             comment = {'': None}
         except ValueError:
             comment = {}
-        none_args = {normalise_property(_k): None for _k in args}
+        none_args = {_k: None for _k in args}
         # remove property comments for dropped properties
         comment.update(none_args)
         return self.modify(
             glyphs,
             comment=comment,
             **none_args,
         )
 
     ##########################################################################
     # property access
 
+    # __getattr__ = HasProps._getattr
+
     def get_comment(self, key=''):
         """Get global or property comment."""
-        key = normalise_property(key)
-        return self._comments.get(key, '')
+        return self._comment.get(key, '')
 
     def _get_comment_dict(self):
         """Get all global and property comments as a dict."""
-        return self._comments
-
-    @property
-    def properties(self):
-        """Non-defaulted properties in order of default definition list."""
-        return {_k.replace('_', '-'): _v for _k, _v in self._props.items()}
-
-    def is_known_property(self, key):
-        """Field is a recognised property."""
-        return self._known(key)
-
-    def get_property(self, key):
-        """Get value for property."""
-        try:
-            return self._get_property(key)
-        except KeyError:
-            return None
-
-    def get_default(self, property):
-        """Default value for a property."""
-        return self._get_default(property)
+        return {**self._comment}
 
     def format_properties(self, template, **kwargs):
         """Format a string template using font properties."""
         from string import Formatter
 
         # pylint: disable=no-self-argument
         class FontFormatter(Formatter):
@@ -839,16 +798,16 @@
 
         return FontFormatter().format(template, **kwargs)
 
     def get_features(self):
         """Get set of special features for this font."""
         feats = set.union(*(_g.features for _g in self.glyphs))
         if any(
-                self._defined(_p)
-                for _p in ('line_width', 'left-extent', 'right-extent')
+                self.get_defined(_p)
+                for _p in ('line_width', 'left_extent', 'right_extent')
             ):
             feats.add('vertical')
         return feats
 
 
     ##########################################################################
     # glyph access
@@ -934,18 +893,18 @@
         """Get default glyph; empty if not defined."""
         try:
             return self.get_glyph(self.default_char, missing='raise')
         except KeyError:
             # use fully inked space-sized block if default glyph undefined
             return self.get_space_glyph().invert()
 
-
     @cache
     def get_space_glyph(self):
         """Get blank glyph with advance width defined by word-space property."""
+        # pylint: disable=invalid-unary-operand-type
         return Glyph.blank(
             width=self.word_space, height=self.pixel_size,
             shift_up=-self.descent
         )
 
     @cache
     def get_empty_glyph(self):
@@ -1090,16 +1049,16 @@
         glyphs = [
             _glyph
             for _glyph in self.glyphs
             if not (set(_glyph.get_labels()) & set(labels))
         ]
         return self.modify(glyphs)
 
-
-    def _set(self, **kwargs):
+    @scriptable(script_args=FontProperties.__annotations__.items())
+    def set(self, **kwargs):
         """Return a copy of the font with one or more recognised properties changed."""
         kwargs = {
             _k: (_v if _v != '' else None)
             for _k, _v in kwargs.items()
         }
         return self.modify(**kwargs)
 
@@ -1463,12 +1422,10 @@
             @wraps(_func)
             def _modify_glyphs(self, _func=_func, **kwargs):
                 return self._apply_to_all_glyphs(_func, **kwargs)
 
             locals()[_name] = _modify_glyphs
 
 
-# set properties from script
-Font.set = scriptable(script_args=Font.__annotations__.items())(Font._set)
 
 # scriptable font/glyph operations
 operations = get_scriptables(Font)
```

### Comparing `monobit-0.40.0/monobit/glyph.py` & `monobit-0.40.1/monobit/glyph.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import logging
 from functools import cache
 
 from .encoding import is_graphical, is_blank
 from .labels import Codepoint, Char, Tag, to_label
 from .raster import Raster, NOT_SET, turn_method
-from .properties import Props, normalise_property, extend_string
-from .cachedprops import DefaultProps, writable_property, as_tuple, checked_property
+from .properties import Props, extend_string
+from .cachedprops import HasProps, checked_property
 from .basetypes import Coord, Bounds, to_number
 from .scripting import scriptable
 from .vector import StrokePath
 
 
 ##############################################################################
 # kerning table
@@ -60,50 +60,57 @@
         # no kerning is zero kerning
         return 0
 
 
 ##############################################################################
 # glyph properties
 
-class Glyph(DefaultProps):
-    """Single glyph including raster and properties."""
+class GlyphProperties:
+    """Default, calculated and settable properties for glyph."""
 
     # horizontal offset from leftward origin to matrix left edge
-    left_bearing: int
+    left_bearing: int = 0
     # horizontal offset from matrix right edge to rightward origin
-    right_bearing: int
+    right_bearing: int = 0
     # upward offset from origin to matrix bottom
-    shift_up: int
+    shift_up: int = 0
     # kerning - pairwaise additional right-bearing
-    right_kerning: KernTable
+    right_kerning: KernTable = KernTable()
     # kerning - pairwaise additional left-bearing
-    left_kerning: KernTable
+    left_kerning: KernTable = KernTable()
 
     # vertical metrics
     # vertical offset from upward origin to matrix top edge
-    top_bearing: int
+    top_bearing: int = 0
     # vertical offset from matrix bottom edge to downward origin
-    bottom_bearing: int
+    bottom_bearing: int = 0
     # leftward offset from origin to matrix left edge
-    shift_left: int
-
-    # compatibility synonyms
-    kern_to: KernTable
-    tracking: int
-    offset: Coord
+    shift_left: int = 0
 
     # path segments for stroke fonts
-    path: StrokePath
+    path: StrokePath = StrokePath()
 
-    # non-overridable, hinted for pylint
-    padding: Bounds
+    # non overridable known properties
+    advance_width: int
+    advance_height: int
+    width: int
     height: int
+    ink_bounds: Bounds
+    bounding_box: Coord
+    padding: Bounds
+    raster: Bounds
+    raster_size: Coord
+
+
+class Glyph(HasProps):
+    """Single glyph including raster and properties."""
+
+    _defaults = vars(GlyphProperties)
+    _converters = HasProps.get_converters(GlyphProperties)
 
-    # sentinel to help build the list of calculated properties
-    __properties_start__ = True
 
     @checked_property
     def advance_width(self):
         """Internal advance width of glyph, including internal bearings."""
         return self.left_bearing + self.width + self.right_bearing
 
     @checked_property
@@ -162,91 +169,67 @@
 
     @checked_property
     def raster_size(self):
         """Raster dimensions."""
         return Coord(self.width, self.height)
 
 
-    ##########################################################################
-    # deprecated compatibility synonymms
-
-    @writable_property('kern_to')
-    def kern_to(self):
-        """Deprecated synonym of right-kerning."""
-        return self.right_kerning
 
-    @writable_property('right_bearing')
-    def tracking(self):
-        """
-        Horizontal offset from matrix right edge to rightward origin
-        Deprecated synonym for right-bearing.
-        """
-        return self.right_bearing
-
-    @as_tuple(('left_bearing', 'shift_up'), tuple_type=Coord.create)
-    def offset(self):
-        """
-        (horiz, vert) offset from origin to matrix start
-        Deprecated synonym for left-bearing, shift-up.
-        """
-
-
-    __properties_end__ = True
 
     ##########################################################################
     # dunder methods
 
     def __init__(
             self, pixels=(), *,
             labels=(), codepoint=b'', char='', tag='', comment='',
             _0=NOT_SET, _1=NOT_SET, _trustme=False,
             **properties
         ):
         """Create glyph from tuple of tuples."""
+        super().__init__()
         if _trustme:
             self._pixels = Raster(pixels, _0=_0, _1=_1)
             self._labels = labels
             self._comment = comment
-            super().__init__(**properties)
+            self._set_properties(properties)
             return
         # raster data
         self._pixels = Raster(pixels, _0=_0, _1=_1)
         # labels
         labels = (
             Char(char), Codepoint(codepoint), Tag(tag),
             *(to_label(_l) for _l in labels)
         )
         self._labels = tuple(_l for _l in labels if _l)
         # comment
         if not isinstance(comment, str):
             raise TypeError('Glyph comment must be a single string.')
         self._comment = comment
         # recognised properties
-        super().__init__(**properties)
+        self._set_properties(properties)
 
     def __eq__(self, other):
         """Equality."""
         if not isinstance(other, type(self)):
             return False
         if (self.width, self.height) != (other.width, other.height):
             return False
-        for p in (*self.properties.keys(), *other.properties.keys()):
-            p = normalise_property(p)
+        for p in (*self._props.keys(), *other._props.keys()):
             if not getattr(self, p) == getattr(other, p):
                 return False
         return self.as_matrix() == other.as_matrix()
 
     def __repr__(self):
         """Text representation."""
         elements = (
             f"labels={repr(self._labels)}" if self._labels else '',
             "comment=({})".format(
                 "\n  '" + "\n',\n  '".join(self.comment.splitlines()) + "'"
             ) if self._comment else '',
-            ', '.join(f'{_k}={_v}' for _k, _v in self.properties.items()),
+            ', '.join(f'{_k}={_v}' for _k, _v in self.get_properties().items()),
             "pixels=({})".format(
                 self.as_text(start="\n  '", end="',")
             ) if self._pixels else ''
         )
         return '{}({})'.format(
             type(self).__name__,
             ', '.join(_e for _e in elements if _e)
@@ -281,18 +264,15 @@
         if char is not NOT_SET:
             labels = [_l for _l in labels if not isinstance(_l, Char)]
             if char:
                 labels.append(Char(char))
         if comment is NOT_SET:
             comment = self._comment
         properties = {**self._props}
-        properties.update({
-            normalise_property(_k): _v
-            for _k, _v in kwargs.items()
-        })
+        properties.update(kwargs)
         return type(self)(
             pixels,
             labels=labels,
             comment=comment or '',
             **properties,
             _trustme=True,
         )
@@ -346,15 +326,15 @@
             comment=None, **properties
         ):
         """Return a copy of the glyph with changes."""
         if not comment:
             comment = ''
         comment = extend_string(self._comment, comment)
         for key, value in properties.items():
-            if self._defined(key):
+            if self.get_defined(key):
                 properties[key] = extend_string(self._props[key], value)
         # do not record glyph history
         try:
             history = properties.pop('history')
             #logging.debug("Ignoring glyph history '%s'", history)
         except KeyError:
             pass
@@ -377,69 +357,51 @@
         except ValueError:
             labels = NOT_SET
         try:
             args.remove('comment')
             comment = ''
         except ValueError:
             comment = NOT_SET
-        none_args = {normalise_property(_k): None for _k in args}
+        none_args = {_k: None for _k in args}
         return self.modify(
             pixels,
             labels=labels,
             comment=comment,
             **none_args
         )
 
 
     ##########################################################################
     # property access
 
+    # __getattr__ = HasProps._getattr
+
     @property
     def comment(self):
         return self._comment
 
-    def get_default(self, property):
-        """Default value for a property."""
-        return self._get_default(property)
-
-    @property
-    def properties(self):
-        """Non-defaulted properties in order of default definition list."""
-        return {_k.replace('_', '-'): _v for _k, _v in self._props.items()}
-
-    def get_property(self, key):
-        """Get value for property."""
-        try:
-            return self._get_property(key)
-        except KeyError:
-            return None
-
-    def get_defined(self, key):
-        """Get value for property, if explicitly defined."""
-        return self._defined(key)
-
     @property
     def features(self):
         """Get set of special features for this glyph."""
         feats = set()
         if any(
-                self._defined(_p)
-                for _p in ('top-bearing', 'bottom-bearing', 'shift-left')
+                self.get_defined(_p)
+                for _p in ('top_bearing', 'bottom_bearing', 'shift_left')
             ):
             feats.add('vertical')
         if any(
-                self._defined(_p)
-                for _p in ('left-kerning', 'right-kerning')
+                self.get_defined(_p)
+                for _p in ('left_kerning', 'right_kerning')
             ):
             feats.add('kerning')
         if any(
                 self._get_property(_p) < 0
                 for _p in (
-                    'left-bearing', 'right-bearing',
-                    'top-bearing', 'bottom-bearing'
+                    'left_bearing', 'right_bearing',
+                    'top_bearing', 'bottom_bearing'
                 )
             ):
             feats.add('overlap')
         return feats
 
     ##########################################################################
     # label access
@@ -592,14 +554,15 @@
         """
         Reverse pixels vertically.
 
         adjust_metrics: also reverse metrics (default: True)
         """
         pixels = self._pixels.flip()
         if adjust_metrics:
+            # pylint: disable=invalid-unary-operand-type
             return self.modify(
                 pixels,
                 top_bearing=self.bottom_bearing,
                 bottom_bearing=self.top_bearing,
                 # flip about baseline
                 shift_up=-self.height - self.shift_up
             )
@@ -717,14 +680,15 @@
     def reduce(self, *, adjust_metrics:bool=True, create_vertical_metrics:bool=False):
         """
         Return a glyph reduced to the bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
+        # pylint: disable=not-an-iterable
         return self.crop(
             *self.padding, adjust_metrics=adjust_metrics,
             create_vertical_metrics=create_vertical_metrics,
         )
 
 
     # scaling
@@ -838,14 +802,15 @@
 
         left: number of times to repeat inked pixel leftwards
         right: number of times to repeat inked pixel rightwards
         up: number of times to repeat inked pixel upwards
         down: number of times to repeat inked pixel downwards
         adjust_metrics: ensure advances stay the same (default: True)
         """
+        # pylint: disable=unpacking-non-sequence
         pleft, pdown, pright, pup = self.padding
         work = self.expand(
             max(0, left-pleft), max(0, down-pdown),
             max(0, right-pright), max(0, up-pup),
             adjust_metrics=adjust_metrics
         )
         return work.modify(work._pixels.smear(
```

### Comparing `monobit-0.40.0/monobit/labels.py` & `monobit-0.40.1/monobit/labels.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/magic.py` & `monobit-0.40.1/monobit/magic.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/pack.py` & `monobit-0.40.1/monobit/pack.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from .font import Font
+from .font import Font, FontProperties
 from .scripting import scriptable, get_scriptables
 
 
 class Pack:
     """Holds one or more potentially unrelated fonts."""
 
     def __init__(self, fonts=()):
@@ -43,15 +43,15 @@
 
         index: which font to pick; 0 is first, -1 is last (default: zero)
         """
         return self[index]
 
     @scriptable(
         pack_operation=True,
-        script_args=Font.__annotations__.items()
+        script_args=FontProperties.__annotations__.items()
     )
     def select(self, **properties):
         """Get a subset of fonts from the pack by property. E.g. select(name='Times')."""
         return Pack(
             _font
             for _font in self
             if all(
```

### Comparing `monobit-0.40.0/monobit/properties.py` & `monobit-0.40.1/monobit/properties.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,68 +24,34 @@
     """Add a line to a multiline string."""
     return '\n'.join(
         _line
         for _line in string.split('\n') + [line]
         if _line
     )
 
-def normalise_property(field):
-    # preserve distinction between starting underscore (internal) and starting dash (user property)
-    return field[:1] + field[1:].replace('-', '_')
-
 
 ##############################################################################
 # property sets
 
 class Props(SimpleNamespace):
-    """
-    SimpleNamespace with the dunder methods of a dict
-    Not a mapping but allows both key-style and attribute-style access
-    """
+    """SimpleNamespace with additional methods"""
 
     # don't pollute the object namespace
     # we only have __dunder__ methods
 
     def __init__(self, *args, **kwargs):
         # convert from string representation
         if len(args) == 1 and isinstance(args[0], str):
             kwargs = dict(
                 _line.strip().split(':', 1)
                 for _line in args[0].splitlines()
             )
             args = ()
         super().__init__(*args, **kwargs)
 
-    def __getitem__(self, field):
-        try:
-            return getattr(self, normalise_property(field))
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __setitem__(self, field, value):
-        try:
-            setattr(self, normalise_property(field), value)
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __delitem__(self, field):
-        try:
-            delattr(self, normalise_property(field))
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __len__(self):
-        return len(vars(self))
-
-    def __iter__(self):
-        return iter(vars(self))
-
-    def __contains__(self, key):
-        return key in vars(self)
-
     def __str__(self):
         strs = tuple(
             (str(_k), str(_v))
             for _k, _v in vars(self).items()
         )
         return '\n'.join(
             f'{_k}: ' + (indent('\n' + _v, '    ') if '\n' in _v else _v)
```

### Comparing `monobit-0.40.0/monobit/raster.py` & `monobit-0.40.1/monobit/raster.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/renderer.py` & `monobit-0.40.1/monobit/renderer.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/scripting.py` & `monobit-0.40.1/monobit/scripting.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/storage.py` & `monobit-0.40.1/monobit/storage.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/struct.py` & `monobit-0.40.1/monobit/struct.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/taggers.py` & `monobit-0.40.1/monobit/taggers.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/vector.py` & `monobit-0.40.1/monobit/vector.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.40.1/monobit/charmaps/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.40.1/monobit/charmaps/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/adobe/symbol.txt` & `monobit-0.40.1/monobit/charmaps/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.40.1/monobit/charmaps/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/agl/LICENSE.md` & `monobit-0.40.1/monobit/charmaps/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/agl/README.md` & `monobit-0.40.1/monobit/charmaps/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/agl/aglfn.txt` & `monobit-0.40.1/monobit/charmaps/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.40.1/monobit/charmaps/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.40.1/monobit/charmaps/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.40.1/monobit/charmaps/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.40.1/monobit/charmaps/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.40.1/monobit/charmaps/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.40.1/monobit/charmaps/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.40.1/monobit/charmaps/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.40.1/monobit/charmaps/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.40.1/monobit/charmaps/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.40.1/monobit/charmaps/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.40.1/monobit/charmaps/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.40.1/monobit/charmaps/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.40.1/monobit/charmaps/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.40.1/monobit/charmaps/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.40.1/monobit/charmaps/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.40.1/monobit/charmaps/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.40.1/monobit/charmaps/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.40.1/monobit/charmaps/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.40.1/monobit/charmaps/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.40.1/monobit/charmaps/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/THAI.TXT` & `monobit-0.40.1/monobit/charmaps/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.40.1/monobit/charmaps/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.40.1/monobit/charmaps/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/README.md` & `monobit-0.40.1/monobit/charmaps/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.40.1/monobit/charmaps/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-de` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-es` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-it` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-us` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.40.1/monobit/charmaps/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.40.1/monobit/charmaps/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/dkuug/x0201-7` & `monobit-0.40.1/monobit/charmaps/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.40.1/monobit/charmaps/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/emacs/README.md` & `monobit-0.40.1/monobit/charmaps/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.40.1/monobit/charmaps/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.40.1/monobit/charmaps/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/evertype/README.md` & `monobit-0.40.1/monobit/charmaps/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1116.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1117.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1118.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1119.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1125.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/113.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/1131.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30000.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30001.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30002.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30003.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30004.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30005.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30006.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30007.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30008.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30009.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30010.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30011.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30012.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30013.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30014.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30015.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30016.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30017.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30018.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30019.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30020.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30021.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30022.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30023.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30024.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30025.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30026.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30027.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30028.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30029.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30030.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30031.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30032.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30033.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30034.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30039.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/30040.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/3012.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/3021.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/3845.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/3846.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/3848.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/437.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/57781.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/58152.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/58210.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/58335.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/59234.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/59829.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/60258.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/60853.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/61282.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/62306.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/667.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/668.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/737.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/770.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/771.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/772.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/773.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/774.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/775.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/777.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/778.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/790.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/808.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/848.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/849.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/850.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/851.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/852.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/853.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/855.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/856.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/857.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/858.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/859.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/860.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/861.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/862.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/863.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/864.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/865.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/866.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/867.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/869.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/872.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/895.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/899.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/991.ucp` & `monobit-0.40.1/monobit/charmaps/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/freedos/README.md` & `monobit-0.40.1/monobit/charmaps/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iana/Amiga-1251` & `monobit-0.40.1/monobit/charmaps/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iana/PTCP154` & `monobit-0.40.1/monobit/charmaps/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.40.1/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.40.1/monobit/charmaps/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.40.1/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.40.1/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.40.1/monobit/charmaps/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/README.md` & `monobit-0.40.1/monobit/charmaps/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.40.1/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.40.1/monobit/charmaps/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.40.1/monobit/charmaps/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.40.1/monobit/charmaps/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.40.1/monobit/charmaps/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.40.1/monobit/charmaps/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.40.1/monobit/charmaps/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.40.1/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.40.1/monobit/charmaps/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/hp48.txt` & `monobit-0.40.1/monobit/charmaps/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.40.1/monobit/charmaps/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.40.1/monobit/charmaps/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/ms-linedraw.txt` & `monobit-0.40.1/monobit/charmaps/manual/ms-linedraw.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/russup3.ucp` & `monobit-0.40.1/monobit/charmaps/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.40.1/monobit/charmaps/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.40.1/monobit/charmaps/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.40.1/monobit/charmaps/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.40.1/monobit/charmaps/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.40.1/monobit/charmaps/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.40.1/monobit/charmaps/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.40.1/monobit/charmaps/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.40.1/monobit/charmaps/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.40.1/monobit/charmaps/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/CP424.TXT` & `monobit-0.40.1/monobit/charmaps/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/CP856.TXT` & `monobit-0.40.1/monobit/charmaps/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.40.1/monobit/charmaps/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.40.1/monobit/charmaps/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.40.1/monobit/charmaps/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.40.1/monobit/charmaps/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.40.1/monobit/charmaps/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.40.1/monobit/charmaps/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.40.1/monobit/charmaps/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.40.1/monobit/charmaps/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/SGML.TXT` & `monobit-0.40.1/monobit/charmaps/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.40.1/monobit/charmaps/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.40.1/monobit/charmaps/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.40.1/monobit/charmaps/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/README.md` & `monobit-0.40.1/monobit/charmaps/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.40.1/monobit/charmaps/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.40.1/monobit/charmaps/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/moztw/eten.txt` & `monobit-0.40.1/monobit/charmaps/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.40.1/monobit/charmaps/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.40.1/monobit/charmaps/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.40.1/monobit/charmaps/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/vietstd/unicode.html` & `monobit-0.40.1/monobit/charmaps/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.40.1/monobit/charmaps/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/gem.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/lics.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.40.1/monobit/charmaps/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.40.1/monobit/charmaps/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.40.1/monobit/charmaps/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.40.1/monobit/charmaps/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.40.1/monobit/charmaps/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/charmaps/xfonts/viscii1.1-1.enc` & `monobit-0.40.1/monobit/charmaps/xfonts/viscii1.1-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/compressors.py` & `monobit-0.40.1/monobit/containers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/container.py` & `monobit-0.40.1/monobit/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/directory.py` & `monobit-0.40.1/monobit/containers/directory.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/mac.py` & `monobit-0.40.1/monobit/containers/mac.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/source.py` & `monobit-0.40.1/monobit/containers/source.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/tar.py` & `monobit-0.40.1/monobit/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/containers/zip.py` & `monobit-0.40.1/monobit/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/amiga.py` & `monobit-0.40.1/monobit/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/bbc.py` & `monobit-0.40.1/monobit/formats/bbc.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/bmfont.py` & `monobit-0.40.1/monobit/formats/bmfont.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,14 +584,15 @@
     # convert to yaff properties
     properties = _parse_bmfont_props(
         name, bmformat, imgformats, info, common,
     )
     # > The `yoffset` gives the distance from the top of the cell height to the top
     # > of the character. A negative value here would mean that the character extends
     # > above the cell height.
+    # pylint: disable=no-member
     raster_top = Font(glyphs, **properties).raster.top
     glyphs = [
         _glyph.modify(
             shift_up=raster_top-_glyph.height-_char.yoffset,
         )
         for _glyph, _char in zip(glyphs, chars)
     ]
@@ -608,19 +609,19 @@
         encoding = 'unicode'
         bmfont_props.pop('charset')
     else:
         # if props are from binary, this has already been converted through CHARSETMAP
         charset = bmfont_props.pop('charset')
         encoding = _CHARSET_STR_MAP.get(charset.upper(), charset)
     properties = {
-        'source-format':
+        'source_format':
             'BMFont ({} descriptor; {} spritesheet)'.format(bmformat, ','.join(imgformats)),
-        'source-name': Path(name).name,
+        'source_name': Path(name).name,
         'family': bmfont_props.pop('face'),
-        'line-height': common.lineHeight,
+        'line_height': common.lineHeight,
         # shift-up is set per-glyph
         'encoding': encoding,
     }
     if _to_int(bmfont_props.pop('bold')):
         properties['weight'] = 'bold'
     if _to_int(bmfont_props.pop('italic')):
         properties['slant'] = 'italic'
```

### Comparing `monobit-0.40.0/monobit/formats/borland.py` & `monobit-0.40.1/monobit/formats/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/cpi.py` & `monobit-0.40.1/monobit/formats/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,15 +436,15 @@
     return font
 
 def _get_consistent(fonts, property):
     """Get value for a property across fonts, or None if inconsistent."""
     values = tuple(set(
         _font.get_property(property)
         for _font in fonts
-        if property in _font.properties
+        if property in _font.get_properties()
     ))
     if len(values) == 1:
         return values[0]
     return None
 
 
 def _convert_to_cp(fonts):
@@ -477,15 +477,15 @@
             num_fonts=len(cp_fonts),
             #size_to_end='short',
         )
         cp_output.fhs = []
         cp_output.bitmaps = []
         for font in cp_fonts:
             # apparently never used
-            if 'cpi' in font.properties:
+            if 'cpi' in font.get_properties():
                 propsplit = (item.partition('=') for item in font.cpi.split())
                 cpiprops = {_k: _v for _k, _, _v in propsplit}
             else:
                 cpiprops = {}
             cp_output.fhs.append(_SCREEN_FONT_HEADER(
                 height=font.cell_size.y,
                 width=font.cell_size.x,
```

### Comparing `monobit-0.40.0/monobit/formats/daisydot.py` & `monobit-0.40.1/monobit/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/dashen.py` & `monobit-0.40.1/monobit/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/dec.py` & `monobit-0.40.1/monobit/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/dosstart.py` & `monobit-0.40.1/monobit/formats/dosstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             if not move:
                 path.append((StrokePath.MOVE, -dx, -dy))
         # turtle moves to next origin, therefore raster includes this column
         glyph = Glyph.from_path(
             StrokePath(path), advance_width=advance, codepoint=0x20+i,
         )
         # remove extra column generated by path going to next origin
-        glyph = glyph.crop(right=1).drop('shift-left')
+        glyph = glyph.crop(right=1)
         glyphs.append(glyph)
     return glyphs
 
 def _read_command(code, offset):
     """Read mode and command characer."""
     try:
         cmd = code[offset]
```

### Comparing `monobit-0.40.0/monobit/formats/figlet.py` & `monobit-0.40.1/monobit/formats/figlet.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         shift_up=-int(props.height)+int(props.baseline),
         direction=_DIRECTIONS[int(props.print_direction)],
         encoding='unicode',
     )
     # > If a FIGcharacter with code 0 is present, it is treated
     # > specially.  It is a FIGfont's "missing character".
     if any(_g.char == '\0' for _g in glyphs):
-        properties['default_char'] = '\0'
+        properties.default_char = '\0'
     # keep uninterpreted parameters in namespace
     properties.figlet = ' '.join(
         f'{_k}={_v}' for _k, _v in vars(props).items() if _k not in (
             'baseline', 'print_direction',
             'hardblank', 'signature_hardblank', 'height', 'max_length',
             'comment_lines', 'codetag_count'
         )
@@ -233,15 +233,15 @@
         # > The Print_Direction parameter tells which direction the font is to be
         # > printed by default.  A value of 0 means left-to-right, and 1 means
         # > right-to-left.  If this parameter is absent, 0 (left-to-right) is assumed.
         print_direction=reverse_dict(_DIRECTIONS).get(font.direction, 0),
         codetag_count = len(coded_chars)
     )
     # keep namespace properties
-    if 'figlet' in font.properties:
+    if 'figlet' in font.get_properties():
         propsplit = (item.partition('=') for item in font.figlet.split())
         figprops = {_k: _v for _k, _, _v in propsplit}
     else:
         figprops = {}
     props.old_layout = figprops.get('old_layout', 0)
     props.full_layout = figprops.get('full_layout', 0)
     # first get glyphs in default repertoire
```

### Comparing `monobit-0.40.0/monobit/formats/fontx.py` & `monobit-0.40.1/monobit/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/fzx.py` & `monobit-0.40.1/monobit/formats/fzx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/gdos.py` & `monobit-0.40.1/monobit/formats/gdos.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,15 +567,15 @@
     font, add_shift_up = _normalise_metrics(font)
     # check glyph dimensions / bitfield ranges
     if any(_g.left_bearing < -127 or _g.right_bearing < -127 for _g in font.glyphs):
         raise FileFormatError(
             'GDOS format: negative bearings must not exceed 127.'
         )
     # keep namespace properties
-    if 'gdos' in font.properties:
+    if 'gdos' in font.get_properties():
         propsplit = (item.partition('=') for item in font.gdos.split())
         add_props = {_k: int(_v) for _k, _, _v in propsplit}
     else:
         add_props = {}
     endian = endianness[0].lower()
     flags = _FH_FLAGS[endian](
         default=add_props.get('font-id', 255) == 1,
```

### Comparing `monobit-0.40.0/monobit/formats/geos.py` & `monobit-0.40.1/monobit/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/hurt.py` & `monobit-0.40.1/monobit/formats/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/image.py` & `monobit-0.40.1/monobit/formats/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from ..storage import loaders, savers
 from ..magic import FileFormatError
 from ..font import Font
 from ..glyph import Glyph
 from ..chart import chart, grid_traverser
 from ..canvas import Canvas
 
+from .bmfont import glyph_map_to_images
+
 
 DEFAULT_IMAGE_FORMAT = 'png'
 
 
 # available background policies
 # -----------------------------
 #
@@ -246,12 +248,12 @@
         """
         if len(fonts) > 1:
             raise FileFormatError('Can only save one font to image file.')
         font = fonts[0]
         font = font.equalise_horizontal()
         font = font.stretch(*scale)
         glyph_map = chart(font, columns, margin, padding, order, direction, codepoint_range)
-        img = Canvas.from_glyph_map(glyph_map).as_image(border=border, paper=paper, ink=ink)
+        img, = glyph_map_to_images(glyph_map, border=border, paper=paper, ink=ink)
         try:
             img.save(outfile, format=image_format or Path(outfile).suffix[1:])
         except (KeyError, ValueError, TypeError):
             img.save(outfile, format=DEFAULT_IMAGE_FORMAT)
```

### Comparing `monobit-0.40.0/monobit/formats/mousegraphics.py` & `monobit-0.40.1/monobit/formats/mousegraphics.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/mzfon.py` & `monobit-0.40.1/monobit/formats/mzfon.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/nearlyraw.py` & `monobit-0.40.1/monobit/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/palm.py` & `monobit-0.40.1/monobit/formats/palm.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/pcl.py` & `monobit-0.40.1/monobit/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/pcpaint.py` & `monobit-0.40.1/monobit/formats/pcpaint.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             right_bearing=(_wid or header.defaultwidth)-header.hsize,
             codepoint=_i+0x20+header.firstchar,
             shift_up=shift_up,
         )
         for _i, _wid in enumerate(widths)
     )
     glyphs = [
-        _g.crop(right=max(0, -_g.right_bearing)).drop('shift-left')
+        _g.crop(right=max(0, -_g.right_bearing))
         for _g in glyphs
     ]
     if header.line_gap:
         # assuming distance from baseline to next raster top
         line_height = header.line_gap + header.baseline
     else:
         line_height = None
```

### Comparing `monobit-0.40.0/monobit/formats/pdf.py` & `monobit-0.40.1/monobit/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/pkfont.py` & `monobit-0.40.1/monobit/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/printshop.py` & `monobit-0.40.1/monobit/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/psf.py` & `monobit-0.40.1/monobit/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/raw.py` & `monobit-0.40.1/monobit/formats/raw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/signum.py` & `monobit-0.40.1/monobit/formats/signum.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,13 +150,14 @@
                 signum=notes if notes else None,
             )
             # as the width in printer fonts is given in bytes, not pixels,
             # these seem to have no information about advance width.
             # from actual files it looks reasonable to preserve only left bearing
             # it is unclear how the advance width of whitespace is determined
             # perhaps this is encoded in the unknown parts of the file header
+            # pylint: disable=no-member
             glyph = glyph.crop(
                 right=glyph.padding.right,
                 adjust_metrics=bool(fixed_byte_width)
-            ).drop('shift-left')
+            )
         glyphs.append(glyph)
     return Font(glyphs, line_height=line_height, dpi=dpi)
```

### Comparing `monobit-0.40.0/monobit/formats/svg.py` & `monobit-0.40.1/monobit/formats/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 def save_svg(fonts, outfile):
     """Export vector font to Scalable Vector Graphics font."""
     if len(fonts) > 1:
         raise FileFormatError('Can only export one font to SVG file.')
     font = fonts[0]
     # matching whitespace doesn't work as label thinks path-only glyphs are empty
     font = font.label(match_whitespace=False)
-    if not any('path' in _g.properties for _g in font.glyphs):
+    if not any('path' in _g.get_properties() for _g in font.glyphs):
         logging.warning(
             "SVG file will have empty glyphs: no stroke path found"
         )
     outfile = outfile.text
     outfile.write('<svg>\n')
     font_attr = {
         'id': font.font_id or font.family or '0',
```

### Comparing `monobit-0.40.0/monobit/formats/vfont.py` & `monobit-0.40.1/monobit/formats/vfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/mac/__init__.py` & `monobit-0.40.1/monobit/formats/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/mac/dfont.py` & `monobit-0.40.1/monobit/formats/mac/dfont.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,29 +255,29 @@
         elif rsrc_type in (b'FONT', b'NFNT'):
             format = ''.join((
                 rsrc_type.decode('mac-roman'),
                 f' in {formatstr}' if formatstr else ''
             ))
             props = {
                 'family': kwargs.get('name', '') or f'{rsrc_id}',
-                'source-format': f'[Mac] {format}',
+                'source_format': f'[Mac] {format}',
             }
             if rsrc_type == b'FONT':
                 # get name and size info from resource ID
                 # https://developer.apple.com/library/archive/documentation/mac/Text/Text-191.html#HEADING191-0
                 # > The resource ID of the font must equal the number produced by
                 # > concatenating the font ID times 128 with the font size.
                 # > Remember that fonts stored in 'FONT' resources are restricted
                 # > to a point size of less than 128 and to a font ID in the range
                 # > 0 to 255. The resource ID is computed by the following formula:
                 # >     resourceID := (font ID * 128) + font size;
                 font_number, font_size = divmod(rsrc_id, 128)
                 # we've already filtered out the case font_size == 0
                 props.update({
-                    'point-size': font_size,
+                    'point_size': font_size,
                     'family': _FONT_NAMES.get(font_number, str(font_number))
                 })
                 # prefer directory info to info inferred from resource ID
                 # (in so far provided by FOND or directory FONT)
                 props.update(info.get(rsrc_id, info.get(font_number, {})))
             else:
                 # update properties with directory info
```

### Comparing `monobit-0.40.0/monobit/formats/mac/fond.py` & `monobit-0.40.1/monobit/formats/mac/fond.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     # > 16384 each non-Roman script system has a range of 512 ($200) font IDs available
     encoding = MAC_ENCODING.get(max(0, 1 + (fond_header.ffFamID - 16384) // 512))
     info = {
         # rsrc_id
         fa_entry.fontID: {
             'family': name,
             'style': mac_style_name(fa_entry.fontStyle),
-            'point-size': fa_entry.fontSize,
+            'point_size': fa_entry.fontSize,
             #'spacing': 'monospace' if fond_header.ffFlags.fixed_width else 'proportional',
             'encoding': encoding,
             'kerning-table': kerning_table.get(fa_entry.fontStyle, ()),
             'encoding-table': encoding_table,
         }
         for fa_entry in fa_list
     }
```

### Comparing `monobit-0.40.0/monobit/formats/mac/iigs.py` & `monobit-0.40.1/monobit/formats/mac/iigs.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,17 @@
 
 def _convert_iigs(glyphs, fontrec, header, name):
     """Convert IIgs font data to monobit font."""
     font = _convert_nfnt({}, glyphs, fontrec)
     # properties from IIgs header
     properties = {
         'family': name,
-        'point-size': header.pointSize,
-        'source-format': 'IIgs v{}.{}'.format(*divmod(header.version, 256)),
-        'iigs.family-id': header.family,
+        'point_size': header.pointSize,
+        'source_format': 'IIgs v{}.{}'.format(*divmod(header.version, 256)),
+        'iigs.family_id': header.family,
     }
     if name not in _NON_ROMAN_NAMES:
         properties['encoding'] = 'mac-roman'
     # decode style field
     if header.style.bold:
         properties['weight'] = 'bold'
     if header.style.italic:
```

### Comparing `monobit-0.40.0/monobit/formats/mac/lisa.py` & `monobit-0.40.1/monobit/formats/mac/lisa.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/mac/nfnt.py` & `monobit-0.40.1/monobit/formats/mac/nfnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     # keep scalable_width
     glyphs = tuple(_glyph.drop('wo_offset', 'wo_width') for _glyph in glyphs)
     # store kerning table
     if properties.get('kerning-table', None):
         kern_table = sorted(
             (
                 _entry.kernFirst, _entry.kernSecond,
-                _entry.kernWidth * properties['point-size'] / 2**12
+                _entry.kernWidth * properties['point_size'] / 2**12
             )
             for _entry in properties['kerning-table']
         )
         glyphs = tuple(
             _glyph.modify(right_kerning=KernTable({
                 _right: f'{_width:.2f}'
                 for _left, _right, _width in kern_table
@@ -372,23 +372,23 @@
             _glyph.modify(tag=tag_table.get(_glyph.codepoint, ''))
             for _glyph in glyphs
         )
     # store properties
     properties.update({
         # not overridable; also seems incorrect for system fonts
         #'spacing': 'monospace' if fontrec.fontType.fixed_width else 'proportional',
-        'default-char': 'missing',
+        'default_char': 'missing',
         'ascent': fontrec.ascent,
         'descent': fontrec.descent,
-        'line-height': fontrec.ascent + fontrec.descent + fontrec.leading,
-        'shift-up': -fontrec.descent,
+        'line_height': fontrec.ascent + fontrec.descent + fontrec.leading,
+        'shift_up': -fontrec.descent,
         # remove the kerning table and encoding table now stored in glyphs
-        'kerning-table': None,
-        'encoding-table': None,
-        'source-format': 'NFNT',
+        'kerning_table': None,
+        'encoding_table': None,
+        'source_format': 'NFNT',
     })
     return Font(glyphs, **properties)
 
 
 
 ###############################################################################
 # NFNT writer
```

### Comparing `monobit-0.40.0/monobit/formats/os2/__init__.py` & `monobit-0.40.1/monobit/formats/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/os2/gpifont.py` & `monobit-0.40.1/monobit/formats/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/os2/lx.py` & `monobit-0.40.1/monobit/formats/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/os2/ne.py` & `monobit-0.40.1/monobit/formats/os2/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/sfnt/sfnt.py` & `monobit-0.40.1/monobit/formats/sfnt/sfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/sfnt/sfnt_writer.py` & `monobit-0.40.1/monobit/formats/sfnt/sfnt_writer.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py` & `monobit-0.40.1/monobit/formats/sfnt/fonttools/E_B_S_C_.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/sfnt/fonttools/__init__.py` & `monobit-0.40.1/monobit/formats/sfnt/fonttools/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/text/draw.py` & `monobit-0.40.1/monobit/formats/text/draw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/text/hex.py` & `monobit-0.40.1/monobit/formats/text/hex.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/text/yaff.py` & `monobit-0.40.1/monobit/formats/text/yaff.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ...storage import loaders, savers
 from ...encoding import charmaps
 from ...magic import FileFormatError
 from ...font import Font
 from ...glyph import Glyph
 from ...raster import Raster
 from ...labels import Label, strip_matching
-from ...properties import Props, normalise_property
-from ...basetypes import passthrough
+from ...properties import Props
+from ...basetypes import Coord, passthrough
 from .draw import NonEmptyBlock, DrawComment, Empty, Unparsed, iter_blocks
 from .draw import format_comment
 
 
 ##############################################################################
 # interface
 
@@ -74,14 +74,36 @@
     empty = '-'
 
     # string to be quoted if one of these chars at start and/or end
     quotable = (':', ' ')
     glyphchars = (ink, paper, empty)
 
 
+# deprecated compatibility synonymms
+_DEPRECATED_SYNONYMS = {
+    'kern_to': 'right_kerning',
+    'tracking': 'right_bearing',
+    'offset': ('left_bearing', 'shift_up'),
+
+    'average_advance': 'average_width',
+    'max_advance': 'max_width',
+    'cap_advance': 'cap_width',
+}
+def _set_property(propsdict, key, value):
+    try:
+        key = _DEPRECATED_SYNONYMS[key]
+    except KeyError:
+        pass
+    if isinstance(key, tuple):
+        for key, value in zip(key, Coord.create(value)):
+            propsdict[key] = value
+    else:
+        propsdict[key] = value
+
+
 ##############################################################################
 # read file
 
 
 def _load_yaffs(text_stream, allow_empty):
     """Parse a yaff or yaffs file."""
     fonts = []
@@ -131,15 +153,16 @@
         if isinstance(block, (YaffGlyph, YaffPropertyOrGlyph)) and block.is_glyph():
             glyphs.append(block.get_glyph_value() | Props(
                 comment='\n\n'.join(current_comment),
             ))
             current_comment = []
         elif isinstance(block, (YaffProperty, YaffPropertyOrGlyph)):
             key = block.get_key()
-            font_props[key] = block.get_value()
+            value = block.get_value()
+            _set_property(font_props, key, value)
             font_prop_comms[key] = '\n\n'.join(current_comment)
             current_comment = []
         if not glyphs and not font_props:
             font_comments.extend(current_comment)
             current_comment = []
         if isinstance(block, YaffComment):
             current_comment.append(block.get_value())
@@ -198,24 +221,27 @@
         else:
             i += 1
         raster = lines[:i]
         properties = {}
         key = None
         for line in lines[i:]:
             if line[:1] in self.whitespace:
-                # multiline glyph properties
+                # follow-up lines in multiline glyph properties
+                # note - won't work with deprecated synonyms
                 if not properties[key]:
                     properties[key] = line.strip()
                 else:
                     properties[key] = '\n'.join((properties[key], line.strip()))
             else:
+                # first line of property
                 # one-line glyph properties
                 key, _, value = line.partition(self.separator)
+                key = normalise_property(key)
                 value = value.strip()
-                properties[key] = value.strip()
+                _set_property(properties, key, value)
         # deal with sized empties (why?)
         if all(set(_line) == set([self.empty]) for _line in raster):
             raster = Raster.blank(width=len(raster[0])-1, height=len(raster)-1)
         return Props(
             pixels=Raster(raster, _0=self.paper, _1=self.ink),
             labels=labels, **properties
         )
@@ -229,14 +255,21 @@
 
     def is_glyph(self):
         return True
 
     get_glyph_value = get_value
 
 
+
+def normalise_property(field):
+    # preserve distinction between starting underscore (internal) and starting dash (user property)
+    return field[:1] + field[1:].replace('-', '_')
+
+
+
 class YaffProperty(NonEmptyBlock, YaffParams):
 
     def starts(self, line):
         return (
             line[:1] not in self.whitespace
             and line[-1:] != self.separator
             and self.separator in line
@@ -244,15 +277,15 @@
 
     def get_value(self):
         _, _, value = self.lines[0].partition(self.separator)
         return _strip_quotes(value)
 
     def get_key(self):
         key, _, _ = self.lines[0].partition(self.separator)
-        return key
+        return normalise_property(key)
 
 
 def _strip_quotes(line):
     line = line.strip()
     if len(line) > 1 and line[0] == line[-1] == '"':
         return line[1:-1]
     return line
@@ -263,15 +296,15 @@
     def starts(self, line):
         return line[:1] not in self.whitespace and line[-1:] == self.separator
 
     def get_value(self):
         return '\n'.join(_strip_quotes(_l) for _l in self.lines[1:])
 
     def get_key(self):
-        return self.lines[0][:-1]
+        return normalise_property(self.lines[0][:-1])
 
     # glyph block with plain label
 
     get_glyph_value = YaffGlyph.get_value
     n_keys = cached_property(YaffGlyph._count_keys)
 
     def is_glyph(self):
@@ -321,15 +354,15 @@
             'name': font.name,
             'spacing': font.spacing,
         }
         if font.spacing in ('character-cell', 'multi-cell'):
             props['cell_size'] = font.cell_size
         else:
             props['bounding_box'] = font.bounding_box
-        props.update(font.properties)
+        props.update(font.get_properties())
         global_metrics = _globalise_glyph_metrics(font.glyphs)
         props.update(global_metrics)
         if props:
             # write recognised yaff properties first, in defined order
             for key, value in props.items():
                 if value != font.get_default(key):
                     _write_property(outstream, key, value, font.get_comment(key))
@@ -354,17 +387,17 @@
     else:
         glyphtxt = glyph.pixels.as_text(
             start=YaffParams.tab,
             ink=YaffParams.ink, paper=YaffParams.paper,
             end='\n'
         )
     outstream.write(glyphtxt)
-    properties = glyph.properties
+    properties = glyph.get_properties()
     for key in global_metrics:
-        properties.pop(key.replace('_', '-'), None)
+        properties.pop(key, None)
     if properties:
         outstream.write(f'\n')
     for key, value in properties.items():
         if value != glyph.get_default(key):
             _write_property(outstream, key, value, None, indent=YaffParams.tab)
     if properties:
         outstream.write('\n')
```

### Comparing `monobit-0.40.0/monobit/formats/windows/LICENSE.md` & `monobit-0.40.1/monobit/formats/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/windows/__init__.py` & `monobit-0.40.1/monobit/formats/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/windows/fnt.py` & `monobit-0.40.1/monobit/formats/windows/fnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,47 +512,47 @@
     vector = win_props.dfType & 1
     if vector:
         logging.info('This is a vector font')
     logging.info('Windows FNT properties:')
     for key, value in win_props.__dict__.items():
         logging.info('    {}: {}'.format(key, value))
     properties = {
-        'source-format': 'Windows FNT v{}.{}'.format(*divmod(version, 256)),
+        'source_format': 'Windows FNT v{}.{}'.format(*divmod(version, 256)),
         'family': bytes_to_str(data[win_props.dfFace:]),
         'copyright': bytes_to_str(win_props.dfCopyright),
-        'point-size': win_props.dfPoints,
+        'point_size': win_props.dfPoints,
         'slant': 'italic' if win_props.dfItalic else 'roman',
         # Windows dfAscent means distance between matrix top and baseline
         # and it calls the space where accents go the dfInternalLeading
         # which is specified to be 'inside the bounds set by dfPixHeight'
         'ascent': win_props.dfAscent - win_props.dfInternalLeading,
         # the dfPixHeight is the 'height of the character bitmap', i.e. our raster-size.y
         # and dfAscent is the distance between the raster top and the baseline,
         'descent': win_props.dfPixHeight - win_props.dfAscent,
         # dfExternalLeading is the 'amount of extra leading ... the application add between rows'
-        'line-height': win_props.dfPixHeight + win_props.dfExternalLeading,
-        'default-char': win_props.dfDefaultChar + win_props.dfFirstChar,
+        'line_height': win_props.dfPixHeight + win_props.dfExternalLeading,
+        'default_char': win_props.dfDefaultChar + win_props.dfFirstChar,
     }
     if not vector:
         # vector font determines shift-up (which only applies to raster) from path
-        properties['shift-up'] = -properties['descent']
+        properties['shift_up'] = -properties['descent']
     if win_props.dfPixWidth:
         properties['spacing'] = 'character-cell'
     else:
         properties['spacing'] = 'proportional'
         # this can be extracted from the font - will be dropped if consistent
         # Windows documentation defines this as 'width of the character "X."'
         # for 1.0 system fonts, it is consistent with the advance width of LATIN CAPITAL LETTER X.
         # for 2.0+ system fonts, this appears to be set to the average advance width.
         # fontforge follows the "new" definition while mkwinfont follows the "old".
         # we'll make it depend on the version
         if version == 0x100:
-            properties['cap-width'] = win_props.dfAvgWidth
+            properties['cap_width'] = win_props.dfAvgWidth
         else:
-            properties['average-width'] = win_props.dfAvgWidth
+            properties['average_width'] = win_props.dfAvgWidth
     # check prop/fixed flag
     if bool(win_props.dfPitchAndFamily & 1) == bool(win_props.dfPixWidth):
         logging.warning(
             'Inconsistent spacing properties: dfPixWidth=={} dfPitchAndFamily=={:04x}'.format(
                 win_props.dfPixWidth, win_props.dfPitchAndFamily
             )
         )
@@ -571,15 +571,15 @@
     charset = win_props.dfCharSet
     if charset in CHARSET_MAP:
         properties['encoding'] = CHARSET_MAP[charset]
     else:
         properties['windows.dfCharSet'] = str(charset)
     properties['style'] = _STYLE_MAP.get(win_props.dfPitchAndFamily & 0xff00, None)
     if win_props.dfBreakChar:
-        properties['word-boundary'] = win_props.dfFirstChar + win_props.dfBreakChar
+        properties['word_boundary'] = win_props.dfFirstChar + win_props.dfBreakChar
     properties['device'] = bytes_to_str(data[win_props.dfDevice:])
     # unparsed properties: dfMaxWidth - but this can be calculated from the matrices
     if version == 0x300:
         # https://github.com/letolabs/fontforge/blob/master/fontforge/winfonts.c
         # /* These fields are not present in 2.0 and are not meaningful in 3.0 */
         # /*  they are there for future expansion */
         # yet another prop/fixed flag
@@ -647,15 +647,15 @@
             # bring all glyphs to same height
             top=max(0, font.raster_size.y-_g.height - add_shift_up),
             # expand into horizontal bearings
             left=max(0, _g.left_bearing),
             right=max(0, _g.right_bearing),
             # expand by positive shift to make all upshifts equal
             bottom=_g.shift_up + add_shift_up
-        ).drop('shift-up')
+        ).drop('shift_up')
         for _g in font.glyphs
     )
     font = font.modify(ord_glyphs)
     return font, add_shift_up
 
 
 def create_fnt(font, version=0x200, vector=False):
@@ -745,15 +745,15 @@
         dfPoints=int(font.point_size),
         dfVertRes=font.dpi.y,
         dfHorizRes=font.dpi.x,
         # Windows dfAscent means distance between matrix top and baseline
         dfAscent=font.raster_size.y - add_shift_up,
         #'ascent': win_props.dfAscent - win_props.dfInternalLeading,
         dfInternalLeading=font.raster_size.y - add_shift_up - font.ascent,
-        #'line-height': win_props.dfPixHeight + win_props.dfExternalLeading,
+        #'line_height': win_props.dfPixHeight + win_props.dfExternalLeading,
         dfExternalLeading=font.line_height-font.raster_size.y,
         dfItalic=(font.slant in ('italic', 'oblique')),
         dfUnderline=('underline' in font.decoration),
         dfStrikeOut=('strikethrough' in font.decoration),
         dfWeight=_WEIGHT_REVERSE_MAP.get(
             font.weight, _WEIGHT_REVERSE_MAP['regular']
         ),
```

### Comparing `monobit-0.40.0/monobit/formats/windows/mz.py` & `monobit-0.40.1/monobit/formats/windows/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/windows/ne.py` & `monobit-0.40.1/monobit/formats/windows/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/windows/pe.py` & `monobit-0.40.1/monobit/formats/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/formats/xlfd/bdf.py` & `monobit-0.40.1/monobit/formats/xlfd/bdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
 from ...binary import int_to_bytes, bytes_to_int, ceildiv
-from ...properties import normalise_property
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from ...font import Font, Coord
 from ...glyph import Glyph
 from ...encoding import charmaps, NotFoundError
 from ...taggers import tagmaps
 from ...labels import Char
@@ -614,16 +613,16 @@
     size_prop = bdf_props.pop('SIZE').split()
     if len(size_prop) > 3:
         if size_prop[3] != 1:
             raise ValueError('Anti-aliasing and colour not supported.')
         size_prop = size_prop[:3]
     size, xdpi, ydpi = size_prop
     properties = {
-        'source-format': 'BDF v{}'.format(bdf_props.pop('STARTFONT')),
-        'point-size': int(size),
+        'source_format': 'BDF v{}'.format(bdf_props.pop('STARTFONT')),
+        'point_size': int(size),
         'dpi': _all_ints(xdpi, ydpi),
         'revision': bdf_props.pop('CONTENTVERSION', None),
     }
     writing_direction = bdf_props.pop('METRICSSET', '0')
     if writing_direction not in ('0', '1', '2'):
         logging.warning(f'Unsupported value METRICSSET={writing_direction} ignored')
         writing_direction = 0
@@ -643,54 +642,54 @@
     mod_glyphs = []
     for glyph, props in zip(glyphs, glyph_props):
         new_props = {}
         # bounding box & offset
         bbx = props.get('BBX', global_bbx)
         if writing_direction in (0, 2):
             _bbx_width, _bbx_height, bboffx, shift_up = (int(_p) for _p in bbx.split(' '))
-            new_props['shift-up'] = shift_up
+            new_props['shift_up'] = shift_up
             # advance width
             dwidth = props.get('DWIDTH', global_dwidth)
             dwidth_x, dwidth_y = (int(_p) for _p in dwidth.split(' '))
             if dwidth_y:
                 raise FileFormatError('Vertical advance in horizontal writing not supported.')
             if dwidth_x > 0:
                 advance_width = dwidth_x
                 left_bearing = bboffx
             else:
                 advance_width = -dwidth_x
                 # bboffx would likely be negative
                 left_bearing = advance_width + bboffx
-            new_props['left-bearing'] = left_bearing
-            new_props['right-bearing'] = advance_width - glyph.width - left_bearing
+            new_props['left_bearing'] = left_bearing
+            new_props['right_bearing'] = advance_width - glyph.width - left_bearing
         if writing_direction in (1, 2):
             vvector = props.get('VVECTOR', global_vvector)
             bbx_width, _bbx_height, bboffx, bboffy = (int(_p) for _p in bbx.split(' '))
             voffx, voffy = (int(_p) for _p in vvector.split(' '))
             to_bottom = bboffy - voffy
             # vector from baseline to raster left; negative: baseline to right of left raster edge
             to_left = bboffx - voffx
             # leftward shift from baseline to raster central axis
-            new_props['shift-left'] = ceildiv(bbx_width, 2) + to_left
+            new_props['shift_left'] = ceildiv(bbx_width, 2) + to_left
             # advance height
             dwidth1 = props.get('DWIDTH1', global_dwidth1)
             dwidth1_x, dwidth1_y = (int(_p) for _p in dwidth1.split(' '))
             if dwidth1_x:
                 raise FileFormatError('Horizontal advance in vertical writing not supported.')
             # dwidth1 vector: negative is down
             if dwidth1_y < 0:
                 advance_height = -dwidth1_y
                 top_bearing = -to_bottom - glyph.height
                 bottom_bearing = advance_height - glyph.height - top_bearing
             else:
                 advance_height = dwidth1_y
                 bottom_bearing = to_bottom
                 top_bearing = advance_height - glyph.height - bottom_bearing
-            new_props['top-bearing'] = top_bearing
-            new_props['bottom-bearing'] = bottom_bearing
+            new_props['top_bearing'] = top_bearing
+            new_props['bottom_bearing'] = bottom_bearing
         mod_glyphs.append(glyph.modify(**new_props))
     # check char counters
     nchars = int(bdf_props.pop('CHARS'))
     # check number of characters, but don't break if no match
     if nchars != len(glyphs):
         logging.warning('Number of characters found does not match CHARS declaration.')
     xlfd_name = bdf_props.pop('FONT')
@@ -744,42 +743,42 @@
         'foundry': _from_quoted_string(x_props.pop('FOUNDRY', '')),
         'copyright': _from_quoted_string(x_props.pop('COPYRIGHT', '')),
         'notice': _from_quoted_string(x_props.pop('NOTICE', '')),
         'family': _from_quoted_string(x_props.pop('FAMILY_NAME', '')),
         'style': _from_quoted_string(x_props.pop('ADD_STYLE_NAME', '')).lower(),
         'ascent': x_props.pop('FONT_ASCENT', None),
         'descent': x_props.pop('FONT_DESCENT', None),
-        'x-height': x_props.pop('X_HEIGHT', None),
-        'cap-height': x_props.pop('CAP_HEIGHT', None),
-        'pixel-size': x_props.pop('PIXEL_SIZE', None),
+        'x_height': x_props.pop('X_HEIGHT', None),
+        'cap_height': x_props.pop('CAP_HEIGHT', None),
+        'pixel_size': x_props.pop('PIXEL_SIZE', None),
         'slant': _SLANT_MAP.get(
             _from_quoted_string(x_props.pop('SLANT', '')), None
         ),
         'spacing': _SPACING_MAP.get(
             _from_quoted_string(x_props.pop('SPACING', '')), None
         ),
-        'underline-descent': x_props.pop('UNDERLINE_POSITION', None),
-        'underline-thickness': x_props.pop('UNDERLINE_THICKNESS', None),
-        'superscript-size': x_props.pop('SUPERSCRIPT_SIZE', None),
-        'subscript-size': x_props.pop('SUBSCRIPT_SIZE', None),
-        'small-cap-size': x_props.pop('SMALL_CAP_SIZE', None),
-        'digit-width': x_props.pop('FIGURE_WIDTH', None),
-        'min-word-space': x_props.pop('MIN_SPACE', None),
-        'word-space': x_props.pop('NORM_SPACE', None),
-        'max-word-space': x_props.pop('MAX_SPACE', None),
-        'sentence-space': x_props.pop('END_SPACE', None),
+        'underline_descent': x_props.pop('UNDERLINE_POSITION', None),
+        'underline_thickness': x_props.pop('UNDERLINE_THICKNESS', None),
+        'superscript_size': x_props.pop('SUPERSCRIPT_SIZE', None),
+        'subscript_size': x_props.pop('SUBSCRIPT_SIZE', None),
+        'small_cap_size': x_props.pop('SMALL_CAP_SIZE', None),
+        'digit_width': x_props.pop('FIGURE_WIDTH', None),
+        'min_word_space': x_props.pop('MIN_SPACE', None),
+        'word_space': x_props.pop('NORM_SPACE', None),
+        'max_word_space': x_props.pop('MAX_SPACE', None),
+        'sentence_space': x_props.pop('END_SPACE', None),
     }
     if 'DESTINATION' in x_props and to_int(x_props['DESTINATION']) < 2:
         dest = to_int(x_props.pop('DESTINATION'))
         properties['device'] = 'screen' if dest else 'printer'
     if 'POINT_SIZE' in x_props:
-        properties['point-size'] = round(to_int(x_props.pop('POINT_SIZE')) / 10)
+        properties['point_size'] = round(to_int(x_props.pop('POINT_SIZE')) / 10)
     if 'AVERAGE_WIDTH' in x_props:
         # average width can have a tilde for negative - because it occurs in the xlfd font name
-        properties['average-width'] = to_int(
+        properties['average_width'] = to_int(
             x_props.pop('AVERAGE_WIDTH').replace('~', '-')
         ) / 10
     # prefer the more precise relative weight and setwidth measures
     if 'RELATIVE_SETWIDTH' in x_props:
         properties['setwidth'] = _SETWIDTH_MAP.get(
             x_props.pop('RELATIVE_SETWIDTH'), None
         )
@@ -801,20 +800,20 @@
         x_props.pop('RESOLUTION', None)
     elif 'RESOLUTION' in x_props:
         # deprecated
         properties['dpi'] = _all_ints(
             x_props.get('RESOLUTION'), x_props.pop('RESOLUTION'), to_int=to_int
         )
     if 'SUPERSCRIPT_X' in x_props and 'SUPERSCRIPT_Y' in x_props:
-        properties['superscript-offset'] = _all_ints(
+        properties['superscript_offset'] = _all_ints(
             x_props.pop('SUPERSCRIPT_X'), x_props.pop('SUPERSCRIPT_Y'),
             to_int=to_int
         )
     if 'SUBSCRIPT_X' in x_props and 'SUBSCRIPT_Y' in x_props:
-        properties['subscript-offset'] = _all_ints(
+        properties['subscript_offset'] = _all_ints(
             x_props.pop('SUBSCRIPT_X'), x_props.pop('SUBSCRIPT_Y'),
             to_int=to_int
         )
     # encoding
     registry = _from_quoted_string(x_props.pop('CHARSET_REGISTRY', '')).lower()
     encoding = _from_quoted_string(x_props.pop('CHARSET_ENCODING', '')).lower()
     if registry and encoding and encoding != '0':
@@ -824,38 +823,38 @@
     elif encoding != '0':
         properties['encoding'] = encoding
     if properties['encoding'] in _UNDEFINED_ENCODINGS:
         properties['encoding'] = ''
     if 'DEFAULT_CHAR' in x_props:
         default_ord = to_int(x_props.pop('DEFAULT_CHAR', None))
         if charmaps.is_unicode(properties['encoding']):
-            properties['default-char'] = Char(chr(default_ord))
+            properties['default_char'] = Char(chr(default_ord))
         else:
-            properties['default-char'] = default_ord
+            properties['default_char'] = default_ord
     # keep original FontName if invalid or conflicting
     if not xlfd_name_props or conflicting:
-        properties['xlfd.font-name'] = xlfd_name
+        properties['xlfd.font_name'] = xlfd_name
     # keep unparsed but known properties
     for key in _XLFD_UNPARSED:
         try:
             value = x_props.pop(key)
         except KeyError:
             continue
-        key = key.lower().replace('_', '-')
+        key = key.lower()
         value = _from_quoted_string(value)
         if value:
             properties[f'xlfd.{key}'] = value
     # drop empty known properties
     properties = {
         _k: _v for _k, _v in properties.items()
         if _v is not None and _v != ''
     }
     # keep unrecognised properties
     properties.update({
-        _k.lower().replace('_', '-'): _from_quoted_string(_v)
+        _k.lower(): _from_quoted_string(_v)
         for _k, _v in x_props.items()
     })
     return properties
 
 
 
 ##############################################################################
@@ -876,26 +875,26 @@
     """Return quoted version of string, if any."""
     return '"{}"'.format(unquoted.replace('"', '""'))
 
 def _create_xlfd_properties(font):
     """Construct XLFD properties."""
     # construct the fields needed for FontName if not defined, leave others optional
     xlfd_props = {
-        'FONT_ASCENT': font.properties.get('ascent'),
-        'FONT_DESCENT': font.properties.get('descent'),
+        'FONT_ASCENT': font.get_defined('ascent'),
+        'FONT_DESCENT': font.get_defined('descent'),
         'PIXEL_SIZE': font.pixel_size,
-        'X_HEIGHT': font.properties.get('x-height', None),
-        'CAP_HEIGHT': font.properties.get('cap-height', None),
+        'X_HEIGHT': font.get_defined('x_height'),
+        'CAP_HEIGHT': font.get_defined('cap_height'),
         'RESOLUTION_X': font.dpi.x,
         'RESOLUTION_Y': font.dpi.y,
         'POINT_SIZE': int(font.point_size) * 10,
-        'FACE_NAME': _quoted_string(font.name) if 'name' in font.properties else None,
-        'FONT_VERSION': _quoted_string(font.revision) if 'revision' in font.properties else None,
-        'COPYRIGHT': _quoted_string(font.copyright) if 'copyright' in font.properties else None,
-        'NOTICE': _quoted_string(font.notice) if 'notice' in font.properties else None,
+        'FACE_NAME': _quoted_string(font.name) if 'name' in font.get_properties() else None,
+        'FONT_VERSION': _quoted_string(font.revision) if 'revision' in font.get_properties() else None,
+        'COPYRIGHT': _quoted_string(font.copyright) if 'copyright' in font.get_properties() else None,
+        'NOTICE': _quoted_string(font.notice) if 'notice' in font.get_properties() else None,
         'FOUNDRY': _quoted_string(font.foundry),
         'FAMILY_NAME': _quoted_string(font.family),
         'WEIGHT_NAME': _quoted_string(font.weight.title()),
         'RELATIVE_WEIGHT': (
             {_v: _k for _k, _v in _WEIGHT_MAP.items()}.get(font.weight, 50)
         ),
         'SLANT': _quoted_string(
@@ -908,29 +907,29 @@
         'RELATIVE_SETWIDTH': (
             # 50 is medium
             {_v: _k for _k, _v in _SETWIDTH_MAP.items()}.get(font.setwidth, 50)
         ),
         'ADD_STYLE_NAME': _quoted_string(font.style.title()),
         'AVERAGE_WIDTH': str(round(float(font.average_width) * 10)).replace('-', '~'),
         # only set if explicitly defined
-        'UNDERLINE_POSITION': font.properties.get('underline-descent', None),
-        'UNDERLINE_THICKNESS': font.properties.get('underline-thickness', None),
-        'DESTINATION': {'printer': 0, 'screen': 1, None: None}.get(font.device.lower(), None),
-        'SUPERSCRIPT_SIZE': font.properties.get('superscript-size', None),
-        'SUBSCRIPT_SIZE': font.properties.get('subscript-size', None),
-        'SMALL_CAP_SIZE': font.properties.get('small-cap-size', None),
-        'SUPERSCRIPT_X': font.superscript_offset.x if 'superscript-offset' in font.properties else None,
-        'SUPERSCRIPT_Y': font.superscript_offset.y if 'superscript-offset' in font.properties else None,
-        'SUBSCRIPT_X': font.subscript_offset.x if 'subscript-offset' in font.properties else None,
-        'SUBSCRIPT_Y': font.subscript_offset.y if 'subscript-offset' in font.properties else None,
-        'FIGURE_WIDTH': font.properties.get('digit-width', None),
-        'MIN_SPACE': font.properties.get('min-word-space', None),
-        'NORM_SPACE': font.properties.get('word-space', None),
-        'MAX_SPACE': font.properties.get('max-word-space', None),
-        'END_SPACE': font.properties.get('sentence-space', None),
+        'UNDERLINE_POSITION': font.get_defined('underline_descent'),
+        'UNDERLINE_THICKNESS': font.get_defined('underline_thickness'),
+        'DESTINATION': {'printer': 0, 'screen': 1}.get(font.device.lower(), None),
+        'SUPERSCRIPT_SIZE': font.get_defined('superscript_size'),
+        'SUBSCRIPT_SIZE': font.get_defined('subscript_size'),
+        'SMALL_CAP_SIZE': font.get_defined('small_cap_size'),
+        'SUPERSCRIPT_X': font.superscript_offset.x if 'superscript_offset' in font.get_properties() else None,
+        'SUPERSCRIPT_Y': font.superscript_offset.y if 'superscript_offset' in font.get_properties() else None,
+        'SUBSCRIPT_X': font.subscript_offset.x if 'subscript_offset' in font.get_properties() else None,
+        'SUBSCRIPT_Y': font.subscript_offset.y if 'subscript_offset' in font.get_properties() else None,
+        'FIGURE_WIDTH': font.get_defined('digit_width'),
+        'MIN_SPACE': font.get_defined('min_word_space'),
+        'NORM_SPACE': font.get_defined('word_space'),
+        'MAX_SPACE': font.get_defined('max_word_space'),
+        'END_SPACE': font.get_defined('sentence_space'),
     }
     # encoding dependent values
     default_glyph = font.get_default_glyph()
     if charmaps.is_unicode(font.encoding):
         if default_glyph.char:
             default_codepoint = tuple(ord(_c) for _c in default_glyph.char)
         else:
@@ -960,21 +959,21 @@
         else:
             xlfd_props['CHARSET_ENCODING'] = '"0"'
     # remove unset properties
     xlfd_props = {_k: _v for _k, _v in xlfd_props.items() if _v is not None}
     # keep unparsed properties
     xlfd_props.update({
         _k.split('.')[1].replace('-', '_').upper(): _quoted_string(' '.join(_v.splitlines()))
-        for _k, _v in font.properties.items()
+        for _k, _v in font.get_properties().items()
         if _k.startswith('xlfd.')
     })
     # keep unknown properties
     xlfd_props.update({
         _k.replace('-', '_').upper(): _quoted_string(' '.join(_v.splitlines()))
-        for _k, _v in font.properties.items()
+        for _k, _v in font.get_properties().items()
         if not _k.startswith('xlfd.') and not font.is_known_property(_k)
     })
     return xlfd_props
 
 def _swidth(dwidth, point_size, dpi):
     """SWIDTH = DWIDTH / ( points/1000 * dpi / 72 )"""
     return int(
@@ -998,17 +997,17 @@
             # are the font's ink-bounds
             'FONTBOUNDINGBOX', (
                 f'{font.bounding_box.x} {font.bounding_box.y} '
                 f'{font.ink_bounds.left} {font.ink_bounds.bottom}'
             )
         )
     ]
-    vertical_metrics = ('shift-left', 'top-bearing', 'bottom-bearing')
+    vertical_metrics = ('shift_left', 'top_bearing', 'bottom_bearing')
     has_vertical_metrics = any(
-        _k in _g.properties
+        _k in _g.get_properties()
         for _g in font.glyphs
         for _k in vertical_metrics
     )
     if has_vertical_metrics:
         bdf_props.append(('METRICSSET', '2'))
     # minimize glyphs to ink-bounds (BBX) before storing, except "cell" fonts
     if font.spacing not in ('character-cell', 'multi-cell'):
```

### Comparing `monobit-0.40.0/monobit/formats/xlfd/hbf.py` & `monobit-0.40.1/monobit/formats/xlfd/hbf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 
-from ...properties import normalise_property
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from ...font import Font, Coord
 from ...glyph import Glyph
 from ...binary import ceildiv
 
 from .bdf import read_props, _parse_xlfd_properties, _create_xlfd_properties
@@ -276,46 +275,46 @@
                 'Inconsistency between HBF and XLFD properties: '
                 '%s=%s (from XLFD) but %s=%s (from HBF). Taking HBF property.',
                 key, value, key, properties[key]
             )
         else:
             properties[key] = value
     # ensure default codepoint gets a plane value
-    if plane is not None and 'default-char' in properties:
-        properties['default-char'] += (0x80+plane) * 0x10000
+    if plane is not None and 'default_char' in properties:
+        properties['default_char'] += (0x80+plane) * 0x10000
     # prefer hbf code scheme to charset values from xlfd
     logging.info('yaff properties:')
     for name, value in properties.items():
         logging.info('    %s: %s', name, value)
     return properties
 
 def _parse_hbf_properties(hbf_props):
     """Parse HBF properties."""
     size, xdpi, ydpi = _split_hbf_ints(hbf_props.pop('SIZE'))
     properties = {
-        'source-format': 'HBF v{}'.format(hbf_props.pop('HBF_START_FONT')),
-        'point-size': size,
+        'source_format': 'HBF v{}'.format(hbf_props.pop('HBF_START_FONT')),
+        'point_size': size,
         'dpi': (xdpi, ydpi),
     }
     width, height, offset_x, offset_y = _split_hbf_ints(
         hbf_props.pop('HBF_BITMAP_BOUNDING_BOX')
     )
     # https://www.ibiblio.org/pub/packages/ccic/software/info/HBF-1.1/BoundingBoxes.html
     # fontboundingbox is equal or larger than bitmap bounding box
     # may be used to specify inter-glyph and inter-line spacing
     # the documented examples show the effect of different bounding box heights
     # but the impact of the fondboundingbox offset is unclear to me
     full_width, full_height, full_offset_x, full_offset_y = _split_hbf_ints(
         hbf_props.pop('FONTBOUNDINGBOX')
     )
     properties.update({
-        'line-height': full_height,
+        'line_height': full_height,
         # full_width :==: advance-width == left-bearing + width + right-bearing
-        'left-bearing': offset_x,
-        'right-bearing': full_width - width - offset_x,
+        'left_bearing': offset_x,
+        'right_bearing': full_width - width - offset_x,
         # I think the fontboundingbox offsets actually go unused
         'shift_up': offset_y,
     })
     # known but we don't use it
     properties['font-id'] = hbf_props.pop('FONT', None)
     # match encoding name
     code_scheme = hbf_props.pop('HBF_CODE_SCHEME')
@@ -361,15 +360,15 @@
     # bring font to normal form
     font, shift_up = _normalise_metrics(font)
     #TODO
     left_bearing = 0
     #glyphs, properties = _globalise_glyph_metrics(font)
     # convert properties
     xlfd_props = _create_xlfd_properties(font)
-    if 'hbf.font' in font.properties:
+    if 'hbf.font' in font.get_properties():
         fontname = font.get_property('hbf.font')
         xlfd_props.pop('HBF.FONT')
     else:
         fontname = _create_xlfd_name(xlfd_props)
     bbx = (
         f'{font.cell_size.x} {font.cell_size.y} '
         f'{left_bearing} {shift_up}'
```

### Comparing `monobit-0.40.0/monobit/scripts/banner.py` & `monobit-0.40.1/monobit/scripts/banner.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/monobit/scripts/convert.py` & `monobit-0.40.1/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/LICENSE` & `monobit-0.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/README.md` & `monobit-0.40.1/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.0/pyproject.toml` & `monobit-0.40.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.40.0"
+version = "0.40.1"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.40.0/PKG-INFO` & `monobit-0.40.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monobit
-Version: 0.40.0
+Version: 0.40.1
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
```


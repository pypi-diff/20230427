# Comparing `tmp/boringavatars-0.3.2.tar.gz` & `tmp/boringavatars-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boringavatars-0.3.2.tar", last modified: Fri Mar 10 05:23:45 2023, max compression
+gzip compressed data, was "boringavatars-1.0.0.tar", last modified: Thu Apr 27 14:52:12 2023, max compression
```

## Comparing `boringavatars-0.3.2.tar` & `boringavatars-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-0.3.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-0.3.2/.flake8
--rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-0.3.2/.gitignore
--rw-r--r--   0        0        0     1481 2022-12-28 02:54:09.917879 boringavatars-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-0.3.2/.pypirc
--rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-0.3.2/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2022-12-19 18:05:58.284537 boringavatars-0.3.2/.vscode/settings.json
--rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-0.3.2/LICENSE
--rw-r--r--   0        0        0      595 2022-12-28 04:17:59.054029 boringavatars-0.3.2/README.md
--rw-r--r--   0        0        0     1496 2022-12-28 03:07:09.774453 boringavatars-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       46 2022-12-28 00:17:00.765116 boringavatars-0.3.2/requirements.txt
--rw-r--r--   0        0        0      901 2023-03-10 05:21:25.768332 boringavatars-0.3.2/src/boringavatars/__init__.py
--rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-0.3.2/src/boringavatars/bauhaus.py
--rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-0.3.2/src/boringavatars/beam.py
--rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-0.3.2/src/boringavatars/marble.py
--rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-0.3.2/src/boringavatars/pixel.py
--rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-0.3.2/src/boringavatars/py.typed
--rw-r--r--   0        0        0      879 2022-12-28 04:11:44.524937 boringavatars-0.3.2/src/boringavatars/ring.py
--rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-0.3.2/src/boringavatars/sunset.py
--rw-r--r--   0        0        0     1509 2022-12-28 04:04:14.154433 boringavatars-0.3.2/src/boringavatars/templates/bauhaus.svg
--rw-r--r--   0        0        0     1781 2022-12-28 04:04:17.147883 boringavatars-0.3.2/src/boringavatars/templates/beam.svg
--rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-0.3.2/src/boringavatars/templates/marble.svg
--rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-0.3.2/src/boringavatars/templates/pixel.svg
--rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-0.3.2/src/boringavatars/templates/ring.svg
--rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-0.3.2/src/boringavatars/templates/sunset.svg
--rw-r--r--   0        0        0     1381 2022-12-28 04:29:33.256766 boringavatars-0.3.2/src/boringavatars/utils.py
--rw-r--r--   0        0        0      214 2022-12-28 04:17:17.661063 boringavatars-0.3.2/tests/test_avatars.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 boringavatars-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-1.0.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-1.0.0/.flake8
+-rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1481 2022-12-28 02:54:09.917879 boringavatars-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-1.0.0/.pypirc
+-rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-1.0.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2022-12-19 18:05:58.284537 boringavatars-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-1.0.0/LICENSE
+-rw-r--r--   0        0        0      595 2022-12-28 04:17:59.054029 boringavatars-1.0.0/README.md
+-rw-r--r--   0        0        0     1508 2023-04-27 14:48:30.715137 boringavatars-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2022-12-28 00:17:00.765116 boringavatars-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      901 2023-04-27 14:49:22.705903 boringavatars-1.0.0/src/boringavatars/__init__.py
+-rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-1.0.0/src/boringavatars/bauhaus.py
+-rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-1.0.0/src/boringavatars/beam.py
+-rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-1.0.0/src/boringavatars/marble.py
+-rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-1.0.0/src/boringavatars/pixel.py
+-rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-1.0.0/src/boringavatars/py.typed
+-rw-r--r--   0        0        0      879 2022-12-28 04:11:44.524937 boringavatars-1.0.0/src/boringavatars/ring.py
+-rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-1.0.0/src/boringavatars/sunset.py
+-rw-r--r--   0        0        0     1510 2023-03-28 18:26:32.049497 boringavatars-1.0.0/src/boringavatars/templates/bauhaus.svg
+-rw-r--r--   0        0        0     1782 2023-03-28 18:23:50.460090 boringavatars-1.0.0/src/boringavatars/templates/beam.svg
+-rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-1.0.0/src/boringavatars/templates/marble.svg
+-rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-1.0.0/src/boringavatars/templates/pixel.svg
+-rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-1.0.0/src/boringavatars/templates/ring.svg
+-rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-1.0.0/src/boringavatars/templates/sunset.svg
+-rw-r--r--   0        0        0     1381 2022-12-28 04:29:33.256766 boringavatars-1.0.0/src/boringavatars/utils.py
+-rw-r--r--   0        0        0      214 2022-12-28 04:17:17.661063 boringavatars-1.0.0/tests/test_avatars.py
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 boringavatars-1.0.0/PKG-INFO
```

### Comparing `boringavatars-0.3.2/.devcontainer/devcontainer.json` & `boringavatars-1.0.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/.gitignore` & `boringavatars-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/.pre-commit-config.yaml` & `boringavatars-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/LICENSE` & `boringavatars-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/README.md` & `boringavatars-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/pyproject.toml` & `boringavatars-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name =  "boringavatars"
 authors = [
     {name = "Federico Bond", email = "federicobond@gmail.com"},
 ]
 description = ""
 readme = "README.md"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `boringavatars-0.3.2/src/boringavatars/__init__.py` & `boringavatars-1.0.0/src/boringavatars/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .bauhaus import bauhaus
 from .beam import beam
 from .marble import marble
 from .pixel import pixel
 from .ring import ring
 from .sunset import sunset
 
-__version__ = "0.3.2"
+__version__ = "1.0.0"
 
 __all__ = ["avatar"]
 
 DEFAULT_COLORS = ["FFAD08", "EDD75A", "73B06F", "0C8F8F", "405059"]
 
 VARIANTS = {
     "beam": beam,
```

### Comparing `boringavatars-0.3.2/src/boringavatars/bauhaus.py` & `boringavatars-1.0.0/src/boringavatars/bauhaus.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/beam.py` & `boringavatars-1.0.0/src/boringavatars/beam.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/marble.py` & `boringavatars-1.0.0/src/boringavatars/marble.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/pixel.py` & `boringavatars-1.0.0/src/boringavatars/pixel.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/ring.py` & `boringavatars-1.0.0/src/boringavatars/ring.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/sunset.py` & `boringavatars-1.0.0/src/boringavatars/sunset.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/bauhaus.svg` & `boringavatars-1.0.0/src/boringavatars/templates/bauhaus.svg`

 * *Files 0% similar despite different names*

```diff
@@ -73,23 +73,23 @@
 00000480: 7465 5f79 207d 7d29 220a 2020 2020 2f3e  te_y }})".    />
 00000490: 0a20 2020 203c 6c69 6e65 0a20 2020 2020  .    <line.     
 000004a0: 2078 313d 2230 220a 2020 2020 2020 7931   x1="0".      y1
 000004b0: 3d22 7b7b 2053 495a 4520 2f20 3220 7d7d  ="{{ SIZE / 2 }}
 000004c0: 220a 2020 2020 2020 7832 3d22 7b7b 2053  ".      x2="{{ S
 000004d0: 495a 4520 7d7d 220a 2020 2020 2020 7932  IZE }}".      y2
 000004e0: 3d22 7b7b 2053 495a 4520 2f20 3220 7d7d  ="{{ SIZE / 2 }}
-000004f0: 220a 2020 2020 2020 7374 726f 6b65 5769  ".      strokeWi
-00000500: 6474 683d 2232 220a 2020 2020 2020 7374  dth="2".      st
-00000510: 726f 6b65 3d22 237b 7b20 7072 6f70 6572  roke="#{{ proper
-00000520: 7469 6573 5b33 5d2e 636f 6c6f 7220 7d7d  ties[3].color }}
-00000530: 220a 2020 2020 2020 7472 616e 7366 6f72  ".      transfor
-00000540: 6d3d 2274 7261 6e73 6c61 7465 287b 7b20  m="translate({{ 
-00000550: 7072 6f70 6572 7469 6573 5b33 5d2e 7472  properties[3].tr
-00000560: 616e 736c 6174 655f 7820 7d7d 207b 7b20  anslate_x }} {{ 
-00000570: 7072 6f70 6572 7469 6573 5b33 5d2e 7472  properties[3].tr
-00000580: 616e 736c 6174 655f 7920 7d7d 2920 726f  anslate_y }}) ro
-00000590: 7461 7465 287b 7b20 7072 6f70 6572 7469  tate({{ properti
-000005a0: 6573 5b33 5d2e 726f 7461 7465 207d 7d20  es[3].rotate }} 
-000005b0: 7b7b 2053 495a 4520 2f20 3220 7d7d 207b  {{ SIZE / 2 }} {
-000005c0: 7b20 5349 5a45 202f 2032 207d 7d29 220a  { SIZE / 2 }})".
-000005d0: 2020 2020 2f3e 0a20 203c 2f67 3e0a 3c2f      />.  </g>.</
-000005e0: 7376 673e 0a                             svg>.
+000004f0: 220a 2020 2020 2020 7374 726f 6b65 2d77  ".      stroke-w
+00000500: 6964 7468 3d22 3222 0a20 2020 2020 2073  idth="2".      s
+00000510: 7472 6f6b 653d 2223 7b7b 2070 726f 7065  troke="#{{ prope
+00000520: 7274 6965 735b 335d 2e63 6f6c 6f72 207d  rties[3].color }
+00000530: 7d22 0a20 2020 2020 2074 7261 6e73 666f  }".      transfo
+00000540: 726d 3d22 7472 616e 736c 6174 6528 7b7b  rm="translate({{
+00000550: 2070 726f 7065 7274 6965 735b 335d 2e74   properties[3].t
+00000560: 7261 6e73 6c61 7465 5f78 207d 7d20 7b7b  ranslate_x }} {{
+00000570: 2070 726f 7065 7274 6965 735b 335d 2e74   properties[3].t
+00000580: 7261 6e73 6c61 7465 5f79 207d 7d29 2072  ranslate_y }}) r
+00000590: 6f74 6174 6528 7b7b 2070 726f 7065 7274  otate({{ propert
+000005a0: 6965 735b 335d 2e72 6f74 6174 6520 7d7d  ies[3].rotate }}
+000005b0: 207b 7b20 5349 5a45 202f 2032 207d 7d20   {{ SIZE / 2 }} 
+000005c0: 7b7b 2053 495a 4520 2f20 3220 7d7d 2922  {{ SIZE / 2 }})"
+000005d0: 0a20 2020 202f 3e0a 2020 3c2f 673e 0a3c  .    />.  </g>.<
+000005e0: 2f73 7667 3e0a                           /svg>.
```

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/beam.svg` & `boringavatars-1.0.0/src/boringavatars/templates/beam.svg`

 * *Files 0% similar despite different names*

```diff
@@ -70,43 +70,43 @@
 00000450: 224d 3135 207b 7b20 3139 202b 206d 6f75  "M15 {{ 19 + mou
 00000460: 7468 5f73 7072 6561 6420 7d7d 6332 2031  th_spread }}c2 1
 00000470: 2034 2031 2036 2030 220a 2020 2020 2020   4 1 6 0".      
 00000480: 2020 2020 7374 726f 6b65 3d22 7b7b 2066      stroke="{{ f
 00000490: 6163 655f 636f 6c6f 7220 7d7d 220a 2020  ace_color }}".  
 000004a0: 2020 2020 2020 2020 6669 6c6c 3d22 6e6f          fill="no
 000004b0: 6e65 220a 2020 2020 2020 2020 2020 7374  ne".          st
-000004c0: 726f 6b65 4c69 6e65 6361 703d 2272 6f75  rokeLinecap="rou
-000004d0: 6e64 220a 2020 2020 2020 2020 2f3e 0a20  nd".        />. 
-000004e0: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
-000004f0: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
-00000500: 2020 2020 2020 2020 643d 224d 3133 2c7b          d="M13,{
-00000510: 7b20 3139 202b 206d 6f75 7468 5f73 7072  { 19 + mouth_spr
-00000520: 6561 6420 7d7d 2061 312c 302e 3735 2030  ead }} a1,0.75 0
-00000530: 2030 2c30 2031 302c 3022 0a20 2020 2020   0,0 10,0".     
-00000540: 2020 2020 2066 696c 6c3d 227b 7b20 6661       fill="{{ fa
-00000550: 6365 5f63 6f6c 6f72 207d 7d22 0a20 2020  ce_color }}".   
-00000560: 2020 2020 202f 3e0a 2020 2020 2020 7b25       />.      {%
-00000570: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000580: 3c72 6563 740a 2020 2020 2020 2020 783d  <rect.        x=
-00000590: 227b 7b20 3134 202d 2065 7965 5f73 7072  "{{ 14 - eye_spr
-000005a0: 6561 6420 7d7d 220a 2020 2020 2020 2020  ead }}".        
-000005b0: 793d 2231 3422 0a20 2020 2020 2020 2077  y="14".        w
-000005c0: 6964 7468 3d22 312e 3522 0a20 2020 2020  idth="1.5".     
-000005d0: 2020 2068 6569 6768 743d 2232 220a 2020     height="2".  
-000005e0: 2020 2020 2020 7278 3d22 3122 0a20 2020        rx="1".   
-000005f0: 2020 2020 2073 7472 6f6b 653d 226e 6f6e       stroke="non
-00000600: 6522 0a20 2020 2020 2020 2066 696c 6c3d  e".        fill=
-00000610: 227b 7b20 6661 6365 5f63 6f6c 6f72 207d  "{{ face_color }
-00000620: 7d22 0a20 2020 2020 202f 3e0a 2020 2020  }".      />.    
-00000630: 2020 3c72 6563 740a 2020 2020 2020 2020    <rect.        
-00000640: 783d 227b 7b20 3230 202b 2065 7965 5f73  x="{{ 20 + eye_s
-00000650: 7072 6561 6420 7d7d 220a 2020 2020 2020  pread }}".      
-00000660: 2020 793d 2231 3422 0a20 2020 2020 2020    y="14".       
-00000670: 2077 6964 7468 3d22 312e 3522 0a20 2020   width="1.5".   
-00000680: 2020 2020 2068 6569 6768 743d 2232 220a       height="2".
-00000690: 2020 2020 2020 2020 7278 3d22 3122 0a20          rx="1". 
-000006a0: 2020 2020 2020 2073 7472 6f6b 653d 226e         stroke="n
-000006b0: 6f6e 6522 0a20 2020 2020 2020 2066 696c  one".        fil
-000006c0: 6c3d 227b 7b20 6661 6365 5f63 6f6c 6f72  l="{{ face_color
-000006d0: 207d 7d22 0a20 2020 2020 202f 3e0a 2020   }}".      />.  
-000006e0: 2020 3c2f 673e 0a20 203c 2f67 3e0a 3c2f    </g>.  </g>.</
-000006f0: 7376 673e 0a                             svg>.
+000004c0: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
+000004d0: 756e 6422 0a20 2020 2020 2020 202f 3e0a  und".        />.
+000004e0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
+000004f0: 0a20 2020 2020 2020 203c 7061 7468 0a20  .        <path. 
+00000500: 2020 2020 2020 2020 2064 3d22 4d31 332c           d="M13,
+00000510: 7b7b 2031 3920 2b20 6d6f 7574 685f 7370  {{ 19 + mouth_sp
+00000520: 7265 6164 207d 7d20 6131 2c30 2e37 3520  read }} a1,0.75 
+00000530: 3020 302c 3020 3130 2c30 220a 2020 2020  0 0,0 10,0".    
+00000540: 2020 2020 2020 6669 6c6c 3d22 7b7b 2066        fill="{{ f
+00000550: 6163 655f 636f 6c6f 7220 7d7d 220a 2020  ace_color }}".  
+00000560: 2020 2020 2020 2f3e 0a20 2020 2020 207b        />.      {
+00000570: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000580: 203c 7265 6374 0a20 2020 2020 2020 2078   <rect.        x
+00000590: 3d22 7b7b 2031 3420 2d20 6579 655f 7370  ="{{ 14 - eye_sp
+000005a0: 7265 6164 207d 7d22 0a20 2020 2020 2020  read }}".       
+000005b0: 2079 3d22 3134 220a 2020 2020 2020 2020   y="14".        
+000005c0: 7769 6474 683d 2231 2e35 220a 2020 2020  width="1.5".    
+000005d0: 2020 2020 6865 6967 6874 3d22 3222 0a20      height="2". 
+000005e0: 2020 2020 2020 2072 783d 2231 220a 2020         rx="1".  
+000005f0: 2020 2020 2020 7374 726f 6b65 3d22 6e6f        stroke="no
+00000600: 6e65 220a 2020 2020 2020 2020 6669 6c6c  ne".        fill
+00000610: 3d22 7b7b 2066 6163 655f 636f 6c6f 7220  ="{{ face_color 
+00000620: 7d7d 220a 2020 2020 2020 2f3e 0a20 2020  }}".      />.   
+00000630: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
+00000640: 2078 3d22 7b7b 2032 3020 2b20 6579 655f   x="{{ 20 + eye_
+00000650: 7370 7265 6164 207d 7d22 0a20 2020 2020  spread }}".     
+00000660: 2020 2079 3d22 3134 220a 2020 2020 2020     y="14".      
+00000670: 2020 7769 6474 683d 2231 2e35 220a 2020    width="1.5".  
+00000680: 2020 2020 2020 6865 6967 6874 3d22 3222        height="2"
+00000690: 0a20 2020 2020 2020 2072 783d 2231 220a  .        rx="1".
+000006a0: 2020 2020 2020 2020 7374 726f 6b65 3d22          stroke="
+000006b0: 6e6f 6e65 220a 2020 2020 2020 2020 6669  none".        fi
+000006c0: 6c6c 3d22 7b7b 2066 6163 655f 636f 6c6f  ll="{{ face_colo
+000006d0: 7220 7d7d 220a 2020 2020 2020 2f3e 0a20  r }}".      />. 
+000006e0: 2020 203c 2f67 3e0a 2020 3c2f 673e 0a3c     </g>.  </g>.<
+000006f0: 2f73 7667 3e0a                           /svg>.
```

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/marble.svg` & `boringavatars-1.0.0/src/boringavatars/templates/marble.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/pixel.svg` & `boringavatars-1.0.0/src/boringavatars/templates/pixel.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/ring.svg` & `boringavatars-1.0.0/src/boringavatars/templates/ring.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/templates/sunset.svg` & `boringavatars-1.0.0/src/boringavatars/templates/sunset.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/src/boringavatars/utils.py` & `boringavatars-1.0.0/src/boringavatars/utils.py`

 * *Files identical despite different names*

### Comparing `boringavatars-0.3.2/PKG-INFO` & `boringavatars-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boringavatars
-Version: 0.3.2
+Version: 1.0.0
 Summary: 
 Author-email: Federico Bond <federicobond@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: boringavatars Version: 0.3.2 Summary: Author-email:
+Metadata-Version: 2.1 Name: boringavatars Version: 1.0.0 Summary: Author-email:
 Federico Bond
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: Jinja2==3.1.2 Requires-Dist: bandit[toml]==1.7.4 ; extra == "test"
-Requires-Dist: black==22.1.0 ; extra == "test" Requires-Dist: check-
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2==3.1.2 Requires-Dist: bandit[toml]==1.7.4 ; extra ==
+"test" Requires-Dist: black==22.1.0 ; extra == "test" Requires-Dist: check-
 manifest==0.48 ; extra == "test" Requires-Dist: flake8-bugbear==22.1.11 ; extra
 == "test" Requires-Dist: flake8-docstrings ; extra == "test" Requires-Dist:
 flake8-formatter_junit_xml ; extra == "test" Requires-Dist: flake8==4.0.1 ;
 extra == "test" Requires-Dist: pre-commit==2.17.0 ; extra == "test" Requires-
 Dist: pylint==2.12.2 ; extra == "test" Requires-Dist: pylint_junit ; extra ==
 "test" Requires-Dist: pytest-cov==3.0.0 ; extra == "test" Requires-Dist:
 pytest-runner ; extra == "test" Requires-Dist: pytest==7.1.0 ; extra == "test"
```


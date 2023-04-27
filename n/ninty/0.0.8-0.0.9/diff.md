# Comparing `tmp/ninty-0.0.8.tar.gz` & `tmp/ninty-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ninty-0.0.8.tar", last modified: Fri Jul  9 16:47:35 2021, max compression
+gzip compressed data, was "dist/ninty-0.0.9.tar", last modified: Fri Jul  9 18:15:20 2021, max compression
```

## Comparing `ninty-0.0.8.tar` & `ninty-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       38 2021-07-09 16:47:35.000000 ninty-0.0.8/setup.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      320 2021-07-09 16:47:35.000000 ninty-0.0.8/PKG-INFO
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1187 2021-07-05 07:56:04.000000 ninty-0.0.8/README.md
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/dsptool/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    12449 2021-07-04 10:48:59.000000 ninty-0.0.8/src/dsptool/encoder.cpp
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/gx2/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1930 2021-07-09 16:27:19.000000 ninty-0.0.8/src/gx2/helpers.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2161 2021-07-09 16:35:38.000000 ninty-0.0.8/src/gx2/codecs.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3106 2021-07-09 16:43:37.000000 ninty-0.0.8/src/gx2/compression.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1788 2021-07-09 16:27:46.000000 ninty-0.0.8/src/gx2/facade.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    10564 2021-07-09 16:28:06.000000 ninty-0.0.8/src/gx2/surface.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3253 2021-07-09 16:29:24.000000 ninty-0.0.8/src/module_gx2.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3264 2021-07-03 13:24:19.000000 ninty-0.0.8/src/module_endian.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     9267 2021-07-05 08:06:17.000000 ninty-0.0.8/src/module_audio.cpp
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/addrlib/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/addrlib/core/
--rwxr-xr-x   0 yannik    (1000) yannik    (1000)    32240 2019-12-29 15:19:09.000000 ninty-0.0.8/src/addrlib/core/addrlib.cpp
--rwxr-xr-x   0 yannik    (1000) yannik    (1000)    11574 2021-07-09 08:57:31.000000 ninty-0.0.8/src/addrlib/core/addrelemlib.cpp
--rwxr-xr-x   0 yannik    (1000) yannik    (1000)     4620 2019-12-29 15:19:09.000000 ninty-0.0.8/src/addrlib/core/addrobject.cpp
--rwxr-xr-x   0 yannik    (1000) yannik    (1000)     6030 2019-12-29 15:19:09.000000 ninty-0.0.8/src/addrlib/addrinterface.cpp
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/src/addrlib/r600/
--rwxr-xr-x   0 yannik    (1000) yannik    (1000)    62551 2021-07-09 08:59:25.000000 ninty-0.0.8/src/addrlib/r600/r600addrlib.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3148 2021-06-27 08:22:49.000000 ninty-0.0.8/src/module_lzss.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     5128 2021-07-03 13:48:44.000000 ninty-0.0.8/src/module_yaz0.cpp
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1097 2021-07-09 16:47:16.000000 ninty-0.0.8/setup.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 16:47:35.000000 ninty-0.0.8/ninty.egg-info/
--rw-r--r--   0 yannik    (1000) yannik    (1000)        6 2021-07-09 16:47:35.000000 ninty-0.0.8/ninty.egg-info/top_level.txt
--rw-r--r--   0 yannik    (1000) yannik    (1000)      320 2021-07-09 16:47:35.000000 ninty-0.0.8/ninty.egg-info/PKG-INFO
--rw-r--r--   0 yannik    (1000) yannik    (1000)      519 2021-07-09 16:47:35.000000 ninty-0.0.8/ninty.egg-info/SOURCES.txt
--rw-r--r--   0 yannik    (1000) yannik    (1000)        1 2021-07-09 16:47:35.000000 ninty-0.0.8/ninty.egg-info/dependency_links.txt
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)       38 2021-07-09 18:15:20.000000 ninty-0.0.9/setup.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      320 2021-07-09 18:15:20.000000 ninty-0.0.9/PKG-INFO
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1187 2021-07-05 07:56:04.000000 ninty-0.0.9/README.md
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/dsptool/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    12449 2021-07-04 10:48:59.000000 ninty-0.0.9/src/dsptool/encoder.cpp
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/gx2/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1930 2021-07-09 16:27:19.000000 ninty-0.0.9/src/gx2/helpers.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     2472 2021-07-09 18:10:16.000000 ninty-0.0.9/src/gx2/codecs.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3545 2021-07-09 18:05:15.000000 ninty-0.0.9/src/gx2/compression.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1788 2021-07-09 16:27:46.000000 ninty-0.0.9/src/gx2/facade.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    10564 2021-07-09 16:28:06.000000 ninty-0.0.9/src/gx2/surface.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3320 2021-07-09 18:08:53.000000 ninty-0.0.9/src/module_gx2.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3264 2021-07-03 13:24:19.000000 ninty-0.0.9/src/module_endian.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     9267 2021-07-05 08:06:17.000000 ninty-0.0.9/src/module_audio.cpp
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/addrlib/
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/addrlib/core/
+-rwxr-xr-x   0 yannik    (1000) yannik    (1000)    32240 2019-12-29 15:19:09.000000 ninty-0.0.9/src/addrlib/core/addrlib.cpp
+-rwxr-xr-x   0 yannik    (1000) yannik    (1000)    11574 2021-07-09 08:57:31.000000 ninty-0.0.9/src/addrlib/core/addrelemlib.cpp
+-rwxr-xr-x   0 yannik    (1000) yannik    (1000)     4620 2019-12-29 15:19:09.000000 ninty-0.0.9/src/addrlib/core/addrobject.cpp
+-rwxr-xr-x   0 yannik    (1000) yannik    (1000)     6030 2019-12-29 15:19:09.000000 ninty-0.0.9/src/addrlib/addrinterface.cpp
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/src/addrlib/r600/
+-rwxr-xr-x   0 yannik    (1000) yannik    (1000)    62551 2021-07-09 08:59:25.000000 ninty-0.0.9/src/addrlib/r600/r600addrlib.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3148 2021-06-27 08:22:49.000000 ninty-0.0.9/src/module_lzss.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     5128 2021-07-03 13:48:44.000000 ninty-0.0.9/src/module_yaz0.cpp
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1097 2021-07-09 16:48:15.000000 ninty-0.0.9/setup.py
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2021-07-09 18:15:20.000000 ninty-0.0.9/ninty.egg-info/
+-rw-r--r--   0 yannik    (1000) yannik    (1000)        6 2021-07-09 18:15:19.000000 ninty-0.0.9/ninty.egg-info/top_level.txt
+-rw-r--r--   0 yannik    (1000) yannik    (1000)      320 2021-07-09 18:15:19.000000 ninty-0.0.9/ninty.egg-info/PKG-INFO
+-rw-r--r--   0 yannik    (1000) yannik    (1000)      519 2021-07-09 18:15:19.000000 ninty-0.0.9/ninty.egg-info/SOURCES.txt
+-rw-r--r--   0 yannik    (1000) yannik    (1000)        1 2021-07-09 18:15:19.000000 ninty-0.0.9/ninty.egg-info/dependency_links.txt
```

### Comparing `ninty-0.0.8/README.md` & `ninty-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/dsptool/encoder.cpp` & `ninty-0.0.9/src/dsptool/encoder.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/gx2/helpers.cpp` & `ninty-0.0.9/src/gx2/helpers.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/gx2/codecs.cpp` & `ninty-0.0.9/src/gx2/codecs.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,32 @@
 }
 
 uint32_t decode_pixel(const void *pix, GX2SurfaceFormat format) {
 	if (format == GX2_SURFACE_FORMAT_UNORM_R8_G8) {
 		uint8_t *ptr = (uint8_t *)pix;
 		return pixel(ptr[0], ptr[1], 0, 0xFF);
 	}
+	else if (format == GX2_SURFACE_FORMAT_UNORM_R5_G6_B5) {
+		uint16_t value = *(uint16_t *)pix;
+		uint8_t r = value >> 11;
+		uint8_t g = (value >> 5) & 0x3F;
+		uint8_t b = value & 0x1F;
+		return pixel(r << 3, g << 2, b << 3, 0xFF);
+	}
 	else if (format == GX2_SURFACE_FORMAT_UNORM_R8_G8_B8_A8) {
 		uint8_t *ptr = (uint8_t *)pix;
 		return pixel(ptr[0], ptr[1], ptr[2], ptr[3]);
 	}
 	return 0;
 }
 
 void decompress_block(uint8_t *block, const uint8_t *pix, GX2SurfaceFormat format) {
 	if (format == GX2_SURFACE_FORMAT_UNORM_BC1) decompress_bc1(block, pix);
 	else if (format == GX2_SURFACE_FORMAT_UNORM_BC3) decompress_bc3(block, pix);
+	else if (format == GX2_SURFACE_FORMAT_UNORM_BC4) decompress_bc4(block, pix);
 	else if (format == GX2_SURFACE_FORMAT_UNORM_BC5) decompress_bc5(block, pix);
 }
 
 void decompress_pixels(uint8_t *dst, const uint8_t *src, uint32_t width, uint32_t height, GX2SurfaceFormat format) {
 	int bpp = surface_format_bpp[format & 0x3F];
 	for (uint32_t by = 0; by < height; by += 4) {
 		for (uint32_t bx = 0; bx < width; bx += 4) {
```

### Comparing `ninty-0.0.8/src/gx2/compression.cpp` & `ninty-0.0.9/src/gx2/compression.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 	}
 	else {
 		bc_interpolate(colors, 5);
 		colors[6] = 0;
 		colors[7] = 0xFF;
 	}
 }
-	
+
 void bc_decode_565(uint16_t color, uint8_t *red, uint8_t *green, uint8_t *blue) {
 	red[0] = (color >> 11) << 3;
 	green[0] = (color >> 3) & 0xFC;
 	blue[0] = (color & 0x1F) << 3;
 }
 
 void decompress_bc1(uint8_t *out, const uint8_t *in) {
@@ -101,14 +101,37 @@
 			*out++ = alpha[alphabits & 7];
 			alphabits >>= 3;
 			colorbits >>= 2;
 		}
 	}
 }
 
+void decompress_bc4(uint8_t *out, const uint8_t *in) {
+	uint8_t red[8];
+	red[0] = in[0];
+	red[1] = in[1];
+	
+	bc3_interpolate(red);
+	
+	uint32_t bits = in[2] | (in[3] << 8) | (in[4] << 16);
+	uint32_t bits2 = in[5] | (in[6] << 8) | (in[7] << 16);
+	
+	for (int y = 0; y < 4; y++) {
+		if (y == 2) bits = bits2;
+		
+		for (int x = 0; x < 4; x++) {
+			*out++ = red[bits & 7];
+			*out++ = 0;
+			*out++ = 0;
+			*out++ = 0xFF;
+			bits >>= 3;
+		}
+	}
+}
+
 void decompress_bc5(uint8_t *out, const uint8_t *in) {
 	uint8_t red[8], green[8];
 	red[0] = in[0];
 	red[1] = in[1];
 	green[0] = in[8];
 	green[1] = in[9];
```

### Comparing `ninty-0.0.8/src/gx2/facade.cpp` & `ninty-0.0.9/src/gx2/facade.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/gx2/surface.cpp` & `ninty-0.0.9/src/gx2/surface.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/module_gx2.cpp` & `ninty-0.0.9/src/module_gx2.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 #include <Python.h>
 #include <cstdint>
 #include <cstring>
 
 
 GX2SurfaceFormat supported_formats[] = {
 	GX2_SURFACE_FORMAT_UNORM_R8_G8,
+	GX2_SURFACE_FORMAT_UNORM_R5_G6_B5,
 	GX2_SURFACE_FORMAT_UNORM_R8_G8_B8_A8,
 	GX2_SURFACE_FORMAT_UNORM_BC1,
 	GX2_SURFACE_FORMAT_UNORM_BC3,
+	GX2_SURFACE_FORMAT_UNORM_BC4,
 	GX2_SURFACE_FORMAT_UNORM_BC5
 };
 
 
 PyObject *GX2_deswizzle(PyObject *self, PyObject *args) {
 	uint8_t *in;
 	size_t inlen;
```

### Comparing `ninty-0.0.8/src/module_endian.cpp` & `ninty-0.0.9/src/module_endian.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/module_audio.cpp` & `ninty-0.0.9/src/module_audio.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/addrlib/core/addrlib.cpp` & `ninty-0.0.9/src/addrlib/core/addrlib.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/addrlib/core/addrelemlib.cpp` & `ninty-0.0.9/src/addrlib/core/addrelemlib.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/addrlib/core/addrobject.cpp` & `ninty-0.0.9/src/addrlib/core/addrobject.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/addrlib/addrinterface.cpp` & `ninty-0.0.9/src/addrlib/addrinterface.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/addrlib/r600/r600addrlib.cpp` & `ninty-0.0.9/src/addrlib/r600/r600addrlib.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/module_lzss.cpp` & `ninty-0.0.9/src/module_lzss.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/src/module_yaz0.cpp` & `ninty-0.0.9/src/module_yaz0.cpp`

 * *Files identical despite different names*

### Comparing `ninty-0.0.8/setup.py` & `ninty-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 		sources = files,
 		include_dirs = ["src", "src/addrlib"]
 	)
 	extensions.append(extension)
 
 setuptools.setup(
 	name = "ninty",
-	version = "0.0.8",
+	version = "0.0.9",
 	description = description,
 	long_description = long_description,
 	author = "Yannik Marchand",
 	author_email = "ymarchand@me.com",
 	url = "https://github.com/kinnay/ninty",
 	license = "GPLv3",
 	ext_modules = extensions
```

### Comparing `ninty-0.0.8/ninty.egg-info/SOURCES.txt` & `ninty-0.0.9/ninty.egg-info/SOURCES.txt`

 * *Files identical despite different names*


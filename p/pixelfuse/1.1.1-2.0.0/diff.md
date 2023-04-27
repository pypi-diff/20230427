# Comparing `tmp/pixelfuse-1.1.1.tar.gz` & `tmp/pixelfuse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelfuse-1.1.1.tar", max compression
+gzip compressed data, was "pixelfuse-2.0.0.tar", max compression
```

## Comparing `pixelfuse-1.1.1.tar` & `pixelfuse-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/LICENSE
--rw-r--r--   0        0        0     3202 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/README.md
--rw-r--r--   0        0        0      116 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/__init__.py
--rw-r--r--   0        0        0      112 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/__main__.py
--rw-r--r--   0        0        0     1346 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/cli.py
--rw-r--r--   0        0        0     3541 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/f2v.py
--rw-r--r--   0        0        0     2098 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/old_files/d_v1.py
--rw-r--r--   0        0        0     2995 2023-04-26 08:40:56.424840 pixelfuse-1.1.1/pixelfuse/src/v2f.py
--rw-r--r--   0        0        0      667 2023-04-26 08:40:56.428840 pixelfuse-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 pixelfuse-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4845 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/README.md
+-rw-r--r--   0        0        0       89 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/__main__.py
+-rw-r--r--   0        0        0     4219 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/cli.py
+-rw-r--r--   0        0        0     3599 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/src/f2v.py
+-rw-r--r--   0        0        0     4118 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/src/v2f.py
+-rw-r--r--   0        0        0      667 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 pixelfuse-2.0.0/PKG-INFO
```

### Comparing `pixelfuse-1.1.1/LICENSE` & `pixelfuse-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelfuse-1.1.1/README.md` & `pixelfuse-2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PixelFuse
+# 📄🔄🎞️ PixelFuse
 
 Convert any file to video and video to file.
 
 **WARNING: videos created from files are extremely fragile**
 
 ## 💿 Installation
 
@@ -11,57 +11,82 @@
 pip install pixelfuse
 ```
 * Install from `Git`:
 ```bash
 pip install git+https://github.com/TheTS-labs/PixelFuse.git
 ```
 
-## Usage
+## 🎬 Usage
 
-### Convert file to video(`convertToVideo`)
+### Convert file to video(`fileToVideo`)
 
 To convert a file into a video just write the following command:
 ```bash
 python -m pixelfuse fileToVideo "test/example.text.txt"
 ```
 
 Where ["test/example.text.txt"](./test/example.text.txt) the file you want to convert to video
 
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
-* `path: str` - mandatory, the path to the file you want to convert
+* `path: Path` - mandatory, the path to the file you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
 * `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
-* `output: str` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
+* `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
 
-### Convert video to file(`convertToFile`)
+### 🆕 Convert files to video(`filesToVideo`)
 
-To get your file back now you need to use this command:
+To convert a file into a video just write the following command:
+```bash
+python -m pixelfuse filesToVideo "test/example.text.txt" "test/example.image.jpg"
+```
+
+Where ["test/example.text.txt"](./test/example.text.txt) and ["test/example.image.jpg"](./test/example.image.jpg) the files you want to convert to video
+
+This command will create a tar.gz archive which will later convert to a video, and delete the archive
+
+This command will also create a hash map in which it will write the hash of **each** file. Then `convertToFile` unpacks all files and checks them according to this map
+
+As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
+
+As for the parameters:
+* `paths: list[Path]` - mandatory, the paths to the files you want to convert
+* `fps: float` - frame rate, default is `1.0`
+* `width: int` - Video length, default is `480px`
+* `height: int` - Video height, `640px` by default
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
+* `verbose: int` - Output level, from 0 to 3, default is 2
+
+### Convert video to file(`videoToFile`)
+
+To get your file(s) back now you need to use this command:
 ```bash
 python -m pixelfuse videoToFile "test/example.video.avi"
 ```
 
-Where ["test/example.video.avi"](./test/example.video.avi) is the file you want to convert into
+Where ["test/example.video.avi"](./test/example.video.avi) is the video you want to convert into file(s)
 
 As output, you will get the file with the name it was converted into a video. For example, if you converted the file "example.image.jpg", when you convert the video back to a file you get a file named example.image.jpg
 
+Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `exctractDir` parameter
+
 Regarding the parameters:
-* `path: str` - Mandatory, the path to the video you want to convert back to a file
+* `path: Path` - Mandatory, the path to the video you want to convert back to a file
 * `verbose: int` - Output level, from 0 to 2, default is 2
-* `decoder: str` - Which decoder to use, default is an empty string. Available decoders: 
-* * `v1` - Less memory efficient decoder, may be useful if standard decoder detects meta frame by mistake. Keep in mind that all video will be loaded into RAM
-* * Blank line - Standard decoder
+* `exctractDir: str` - Path to extract archive files
 
-## Warning
+## ⚠️ Warning
 
 Because of the way this converter works, the video output is **very, very** fragile
 
 In order for you to be able to convert the file back, every pixel **MUST remain unchanged**, that is what you should avoid:
 * Use ONLY lossless codecs, as all other codecs corrupt the pixels. E.g. FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS`, etc.
 * Do not convert videos to other formats, as this will most likely cause pixel damage
 * Keep in mind that if you upload videos to YouTube, it will re-encode the video(and, guess what, damage the pixels), so if you want to download videos from YouTube, you'll need to use [Google Takeout](https://takeout.google.com/)
 * Do not trim the video, it will trim some of the information, and therefore the file you converted
 * Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it
+* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot handle these archives properly, if you want to convert multiple files you better use the `filesToVideo` command
```

### Comparing `pixelfuse-1.1.1/pixelfuse/src/f2v.py` & `pixelfuse-2.0.0/pixelfuse/src/f2v.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+import hashlib
+import os
+from pathlib import Path
+import pickle
 import struct
+
 import cv2
 import numpy as np
-import pickle
-import hashlib
-import os
-from rich.progress import Progress, SpinnerColumn, MofNCompleteColumn, BarColumn, TimeElapsedColumn, TimeRemainingColumn
 from rich import print
+from rich.progress import (BarColumn, MofNCompleteColumn, Progress,
+                           SpinnerColumn, TimeElapsedColumn,
+                           TimeRemainingColumn)
+
 from pixelfuse import encoder
 
+
 class ToVideo(object):
-    def __init__(self, filename, fps=1., width=640, height=480, fourcc="HFYU", output="output.avi", verbose=2):
-        self.filename = filename
+    def __init__(self, file: Path, fps=1., width=640, height=480, fourcc="HFYU", output: Path=Path("output.avi"), verbose=2, hashmap=None):
+        self.file = file
         self.fps = fps
         self.width = width
         self.height = height
         self.fourcc = cv2.VideoWriter_fourcc(*fourcc)
         self.output = output
-        self.checksum = hashlib.sha512(open(self.filename, 'rb').read()).hexdigest()
+        self.checksum = hashlib.sha512(self.file.read_bytes()).hexdigest()
         self.verbose = verbose
+        self.hashmap = hashmap
 
-        self.bytesInFile = os.stat(self.filename).st_size
+        self.bytesInFile = self.file.stat().st_size
         self.pixelsInFile = (self.bytesInFile//3)+1
 
         self.barColumns = [
             SpinnerColumn(),
             "{task.description}",
             BarColumn(),
             "Elapsed time:",
@@ -34,63 +41,64 @@
             MofNCompleteColumn()
         ]
         self.barKwargs = {
             "transient": True
         }
 
     def convert(self):
-        out = cv2.VideoWriter(self.output, self.fourcc, self.fps, (self.width, self.height))
+        out = cv2.VideoWriter(self.output.name, self.fourcc, self.fps, (self.width, self.height))
 
         frame = np.zeros((self.height, self.width, 3), dtype=np.uint8)
-        self.print_verbose("Opening the file...", 1)
-        with open(self.filename, 'rb') as f:
+        self.print("Opening the file...", 1)
+        with self.file.open("rb") as f:
             y = 0
             x = 0
-            self.print_verbose("Creating meta data...", 2)
+            self.print("Creating meta data...", 2)
             meta = {
                 "checksum": self.checksum,
-                "filename": self.filename.split("/")[-1],
+                "filename": self.file.name,
                 "encoder": encoder,
-                "lastZeros": 0
+                "lastZeros": 0,
+                "hashmap": self.hashmap
             }
 
-            self.print_verbose("Starting video writing...", 1)
+            self.print("Starting video writing...", 1)
             with Progress(*self.barColumns, **self.barKwargs) as progress:
                 for i in progress.track(range(self.pixelsInFile)):
                     b = f.read(3)
                     if not b:
-                        self.print_verbose("File end", 3)
+                        self.print("File end", 3)
                         break
                     if len(b) < 3:
                         meta["lastZeros"] = 3-len(b)
-                        self.print_verbose(f"File end with {meta['lastZeros']} left zeros", 3)
+                        self.print(f"File end with {meta['lastZeros']} left zeros", 3)
                         b = b.ljust(3, b'\x00')
 
                     frame[y, x] = struct.unpack('<BBB', b)
                     x += 1
                     if x >= self.width:
                         x = 0
                         y += 1
                     if y >= self.height:
-                        self.print_verbose(f"Done {frame[0, 0]} frame", 2)
+                        self.print(f"Done {frame[0, 0]} frame", 2)
                         out.write(frame)
                         y = 0
                         frame = np.zeros((self.height, self.width, 3), dtype=np.uint8)
 
                 if np.any(frame):
-                    self.print_verbose(f"Writing not full {frame[0, 0]} frame", 2)
+                    self.print(f"Writing not full {frame[0, 0]} frame", 2)
                     out.write(frame)
 
-                self.print_verbose(f"Creating meta data frame...", 3)
+                self.print(f"Creating meta data frame...", 3)
                 pickle_bytes = pickle.dumps(meta)
                 frame = np.frombuffer(pickle_bytes, dtype=np.uint8).copy()
                 frame.resize((self.height, self.width, 3))
 
-                self.print_verbose(f"Writing meta data {frame[0, 0]} frame", 2)
+                self.print(f"Writing meta data {frame[0, 0]} frame", 2)
                 out.write(frame)
 
-        self.print_verbose(f"Writing video...", 1)
+        self.print(f"Writing video...", 1)
         out.release()
 
-    def print_verbose(self, text, verbose):
+    def print(self, text, verbose):
         if self.verbose >= verbose:
             print(text)
```

### Comparing `pixelfuse-1.1.1/pixelfuse/src/v2f.py` & `pixelfuse-2.0.0/pixelfuse/src/v2f.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-import cv2 
+import hashlib
+import os
+from pathlib import Path
 import pickle
-import numpy as np
+import tarfile
 import tempfile
-import os
-import hashlib
+
+import cv2
+import numpy as np
 from rich.console import Console
-from pixelfuse import decoder, compatible_encoders
+
+from pixelfuse import compatible_encoders, decoder
+
 
 class ToFile:
-    def __init__(self, filename, verbose):
-        self.cap = cv2.VideoCapture(filename)
+    def __init__(self, filename: Path, verbose, exctractDir):
+        self.cap = cv2.VideoCapture(filename.name)
         self.console = Console()
         self.verbose = verbose
+        self.exctractDir = exctractDir
 
         if not self.cap.isOpened(): 
             raise FileNotFoundError("Error opening video file")
 
     def writeTempFile(self):
         self.print("Start reading video", 1)
         ret, frame = self.cap.read()
@@ -52,31 +58,59 @@
             toWriteFrame = frame
             ret, frame = self.cap.read()
 
         self.temp.close()
         self.print("[green bold]Done writing temp file", 1)
 
     def renameAccordingToMeta(self):
+        if self.meta["hashmap"] is not None:
+            return
+
         try:
             self.print(f"Rename temp file: {self.temp.name} -> ./{self.meta['filename']}", 1)
             os.link(self.temp.name, self.meta["filename"])
         except FileExistsError:
             os.remove(self.temp.name)
             raise FileExistsError(f"Cannot write file, file already exists: {self.meta['filename']}")
 
         self.print(f"Remove temp file {self.temp.name}", 2)
         os.remove(self.temp.name)
 
+    def extract(self):
+        if self.meta["hashmap"] is not None:
+            self.print(f"Extracting files...", 2)
+            archive = tarfile.open(self.temp.name, "r:gz")
+            if self.exctractDir is None:
+                self.exctractDir = self.meta["filename"].split(".")[0]
+            archive.extractall(self.exctractDir)
+            archive.close()
+
+            self.print(f"Remove temp file {self.temp.name}", 2)
+
+            os.remove(self.temp.name)
+
     def verify(self):
-        self.print(f"Verify file", 2)
-        if self.meta["checksum"] != hashlib.sha512(open(self.meta["filename"], 'rb').read()).hexdigest():
-            print("Doesn't match")
+        if self.meta["hashmap"] is None:
+            self.print(f"Verify file", 2)
+
+            if self.meta["checksum"] != hashlib.sha512(Path(self.meta["filename"]).read_bytes()).hexdigest():
+                self.print("[bold yellow]Checksums doesn't match!", 1)
+
+            return
+
+        for filename in self.meta["hashmap"]:
+            self.print(f"Verifing {filename}...", 2)
+            hashsum = hashlib.sha512(Path(self.exctractDir, filename).read_bytes()).hexdigest()
+            
+            if hashsum != self.meta["hashmap"][filename]:
+                self.print(f"[bold yellow]{filename} checksum doesn't match!", 1)
 
     def convert(self):
         with self.console.status("[green]Decoding video..."):
             self.writeTempFile()
             self.renameAccordingToMeta()
+            self.extract()
             self.verify()
 
     def print(self, text, verbose):
         if self.verbose >= verbose:
             self.console.print(text)
```

### Comparing `pixelfuse-1.1.1/pyproject.toml` & `pixelfuse-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelfuse"
-version = "1.1.1"
+version = "2.0.0"
 description = "Convert any file to video and video to file"
 authors = ["Roman <romantovt31@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/TheTS-labs/PixelFuse"
 repository = "https://github.com/TheTS-labs/PixelFuse"
 keywords = ["video", "file", "converter"]
```

### Comparing `pixelfuse-1.1.1/PKG-INFO` & `pixelfuse-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelfuse
-Version: 1.1.1
+Version: 2.0.0
 Summary: Convert any file to video and video to file
 Home-page: https://github.com/TheTS-labs/PixelFuse
 License: GPL-3.0
 Keywords: video,file,converter
 Author: Roman
 Author-email: romantovt31@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -16,15 +16,15 @@
 Requires-Dist: ffmpegio (>=0.8.3,<0.9.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/TheTS-labs/PixelFuse
 Description-Content-Type: text/markdown
 
-# PixelFuse
+# 📄🔄🎞️ PixelFuse
 
 Convert any file to video and video to file.
 
 **WARNING: videos created from files are extremely fragile**
 
 ## 💿 Installation
 
@@ -33,58 +33,83 @@
 pip install pixelfuse
 ```
 * Install from `Git`:
 ```bash
 pip install git+https://github.com/TheTS-labs/PixelFuse.git
 ```
 
-## Usage
+## 🎬 Usage
 
-### Convert file to video(`convertToVideo`)
+### Convert file to video(`fileToVideo`)
 
 To convert a file into a video just write the following command:
 ```bash
 python -m pixelfuse fileToVideo "test/example.text.txt"
 ```
 
 Where ["test/example.text.txt"](./test/example.text.txt) the file you want to convert to video
 
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
-* `path: str` - mandatory, the path to the file you want to convert
+* `path: Path` - mandatory, the path to the file you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
 * `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
-* `output: str` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
+* `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
 
-### Convert video to file(`convertToFile`)
+### 🆕 Convert files to video(`filesToVideo`)
 
-To get your file back now you need to use this command:
+To convert a file into a video just write the following command:
+```bash
+python -m pixelfuse filesToVideo "test/example.text.txt" "test/example.image.jpg"
+```
+
+Where ["test/example.text.txt"](./test/example.text.txt) and ["test/example.image.jpg"](./test/example.image.jpg) the files you want to convert to video
+
+This command will create a tar.gz archive which will later convert to a video, and delete the archive
+
+This command will also create a hash map in which it will write the hash of **each** file. Then `convertToFile` unpacks all files and checks them according to this map
+
+As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
+
+As for the parameters:
+* `paths: list[Path]` - mandatory, the paths to the files you want to convert
+* `fps: float` - frame rate, default is `1.0`
+* `width: int` - Video length, default is `480px`
+* `height: int` - Video height, `640px` by default
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
+* `verbose: int` - Output level, from 0 to 3, default is 2
+
+### Convert video to file(`videoToFile`)
+
+To get your file(s) back now you need to use this command:
 ```bash
 python -m pixelfuse videoToFile "test/example.video.avi"
 ```
 
-Where ["test/example.video.avi"](./test/example.video.avi) is the file you want to convert into
+Where ["test/example.video.avi"](./test/example.video.avi) is the video you want to convert into file(s)
 
 As output, you will get the file with the name it was converted into a video. For example, if you converted the file "example.image.jpg", when you convert the video back to a file you get a file named example.image.jpg
 
+Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `exctractDir` parameter
+
 Regarding the parameters:
-* `path: str` - Mandatory, the path to the video you want to convert back to a file
+* `path: Path` - Mandatory, the path to the video you want to convert back to a file
 * `verbose: int` - Output level, from 0 to 2, default is 2
-* `decoder: str` - Which decoder to use, default is an empty string. Available decoders: 
-* * `v1` - Less memory efficient decoder, may be useful if standard decoder detects meta frame by mistake. Keep in mind that all video will be loaded into RAM
-* * Blank line - Standard decoder
+* `exctractDir: str` - Path to extract archive files
 
-## Warning
+## ⚠️ Warning
 
 Because of the way this converter works, the video output is **very, very** fragile
 
 In order for you to be able to convert the file back, every pixel **MUST remain unchanged**, that is what you should avoid:
 * Use ONLY lossless codecs, as all other codecs corrupt the pixels. E.g. FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS`, etc.
 * Do not convert videos to other formats, as this will most likely cause pixel damage
 * Keep in mind that if you upload videos to YouTube, it will re-encode the video(and, guess what, damage the pixels), so if you want to download videos from YouTube, you'll need to use [Google Takeout](https://takeout.google.com/)
 * Do not trim the video, it will trim some of the information, and therefore the file you converted
 * Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it
+* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot handle these archives properly, if you want to convert multiple files you better use the `filesToVideo` command
```


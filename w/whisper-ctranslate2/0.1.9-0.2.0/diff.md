# Comparing `tmp/whisper-ctranslate2-0.1.9.tar.gz` & `tmp/whisper-ctranslate2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.9.tar", last modified: Sun Apr 16 15:31:45 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.0.tar", last modified: Wed Apr 26 16:31:18 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.9.tar` & `whisper-ctranslate2-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.9/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5510 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4859 2023-04-16 12:50:08.000000 whisper-ctranslate2-0.1.9/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-14 14:47:47.000000 whisper-ctranslate2-0.1.9/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.125990 whisper-ctranslate2-0.1.9/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.125990 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-16 13:14:32.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6124 2023-04-16 13:29:56.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-14 15:20:03.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13377 2023-04-16 13:34:29.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-16 13:22:55.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5510 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.0/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5641 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.0/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-26 15:07:48.000000 whisper-ctranslate2-0.2.0/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-26 16:27:40.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-19 16:58:21.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14312 2023-04-26 16:27:40.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-26 15:18:01.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5641 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.9/LICENSE` & `whisper-ctranslate2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.9/PKG-INFO` & `whisper-ctranslate2-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.9
+Version: 0.2.0
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -62,14 +62,16 @@
 
 To translate:
 
     whisper-ctranslate2 inaguracio2011.mp3 --model medium --task translate
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/226923535-b6583536-2486-4127-b17b-c58d85cdb90f.png">
 
+Whisper translate task translates the transcription from the source language to English (the only target language supported).
+
 Additionally using:
 
     whisper-ctranslate2 --help
 
 All the supported options with their help are shown.
 
 # CTranslate2 specific options
@@ -113,17 +115,17 @@
 
     whisper-ctranslate2 myfile.mp3 --print_colors True
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
 ## Live transcribe from your microphone
 
-`----live_transcribe True` option activates the live transcription mode from your microphone:
+`--live_transcribe True` option activates the live transcription mode from your microphone:
 
-    whisper-ctranslate2 myfile.mp3 --print_colors True
+    whisper-ctranslate2 --live_transcribe True --language en
 
 https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
 
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
```

### Comparing `whisper-ctranslate2-0.1.9/README.md` & `whisper-ctranslate2-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 To translate:
 
     whisper-ctranslate2 inaguracio2011.mp3 --model medium --task translate
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/226923535-b6583536-2486-4127-b17b-c58d85cdb90f.png">
 
+Whisper translate task translates the transcription from the source language to English (the only target language supported).
+
 Additionally using:
 
     whisper-ctranslate2 --help
 
 All the supported options with their help are shown.
 
 # CTranslate2 specific options
@@ -94,17 +96,17 @@
 
     whisper-ctranslate2 myfile.mp3 --print_colors True
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
 ## Live transcribe from your microphone
 
-`----live_transcribe True` option activates the live transcription mode from your microphone:
+`--live_transcribe True` option activates the live transcription mode from your microphone:
 
-    whisper-ctranslate2 myfile.mp3 --print_colors True
+    whisper-ctranslate2 --live_transcribe True --language en
 
 https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
 
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
```

### Comparing `whisper-ctranslate2-0.1.9/setup.py` & `whisper-ctranslate2-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/transcribe.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import tqdm
 import sys
 from faster_whisper import WhisperModel
 from .languages import LANGUAGES
 from typing import BinaryIO
 import numpy as np
 
-
 system_encoding = sys.getdefaultencoding()
 
 if system_encoding != "utf-8":
 
     def make_safe(string):
         return string.encode(system_encoding, errors="replace").decode(system_encoding)
 
@@ -95,14 +94,16 @@
 
         return vad_parameters
 
     def inference(
         self,
         audio: Union[str, BinaryIO, np.ndarray],
         model_path: str,
+        cache_directory: str,
+        local_files_only: bool,
         task: str,
         language: str,
         threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
         verbose: bool,
@@ -111,14 +112,16 @@
     ):
         model = WhisperModel(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
             cpu_threads=threads,
+            download_root=cache_directory,
+            local_files_only=local_files_only,
         )
 
         vad_parameters = self._get_vad_parameters_dictionary(options)
 
         segments, info = model.transcribe(
             audio=audio,
             language=language,
```

### Comparing `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import argparse
 import os
 from .transcribe import Transcribe, TranscriptionOptions
-from .models import Models
 from .languages import LANGUAGES, TO_LANGUAGE_CODE, from_language_to_iso_code
 import numpy as np
 import warnings
 from typing import Union, List
 from .writers import get_writer
 from .version import __version__
 from .live import Live
 import sys
 
+MODEL_NAMES = [
+    "tiny",
+    "tiny.en",
+    "base",
+    "base.en",
+    "small",
+    "small.en",
+    "medium",
+    "medium.en",
+    "large-v1",
+    "large-v2",
+]
+
 
 def optional_int(string):
     return None if string == "None" else int(string)
 
 
 def str2bool(string):
     str2val = {"True": True, "False": False}
@@ -34,22 +46,22 @@
     )
     parser.add_argument(
         "audio", nargs="*", type=str, help="audio file(s) to transcribe"
     )
     parser.add_argument(
         "--model",
         default="small",
-        choices=Models().get_list(),
+        choices=MODEL_NAMES,
         help="name of the Whisper model to use",
     )
     parser.add_argument(
         "--model_dir",
         type=str,
         default=None,
-        help="the path to save model files; uses ~/.cache/whisper-ctranslate2 by default",
+        help="the path to save model files; uses ~/.cache/huggingface/ by default",
     )
     parser.add_argument(
         "--output_dir",
         "-o",
         type=str,
         default=".",
         help="directory to save the outputs",
@@ -228,14 +240,21 @@
         type=int,
         default=None,
         help="When `vad_filter` is enabled, in the end of each speech chunk time to wait before separating it.",
     )
 
     # CTranslate2 specific parameters
     parser.add_argument(
+        "--local_files_only",
+        type=str2bool,
+        default=False,
+        help="Use models in cache without connecting to Internet to check if there are newer versions",
+    )
+
+    parser.add_argument(
         "--device_index",
         nargs="*",
         type=int,
         default=0,
         help="Device IDs where to place this model on",
     )
 
@@ -278,14 +297,22 @@
     parser.add_argument(
         "--live_transcribe", type=str2bool, default=False, help="Live transcribe mode"
     )
 
     return parser.parse_args().__dict__
 
 
+def _does_old_cache_dir_has_files():
+    default = os.path.join(os.path.expanduser("~"), ".cache")
+    cache_dir = os.path.join(
+        os.getenv("XDG_CACHE_HOME", default), "whisper-ctranslate2"
+    )
+    return cache_dir, os.path.exists(cache_dir)
+
+
 def main():
     args = read_command_line()
     output_dir: str = args.pop("output_dir")
     output_format: str = args.pop("output_format")
     os.makedirs(output_dir, exist_ok=True)
     model: str = args.pop("model")
     threads: int = args.pop("threads")
@@ -296,14 +323,15 @@
     verbose: bool = args.pop("verbose")
     model_directory: str = args.pop("model_directory")
     cache_directory: str = args.pop("model_dir")
     device_index: Union[int, List[int]] = args.pop("device_index")
     suppress_tokens: str = args.pop("suppress_tokens")
     live_transcribe: bool = args.pop("live_transcribe")
     audio: str = args.pop("audio")
+    local_files_only: bool = args.pop("local_files_only")
 
     temperature = args.pop("temperature")
     if (increment := args.pop("temperature_increment_on_fallback")) is not None:
         temperature = tuple(np.arange(temperature, 1.0 + 1e-6, increment))
     else:
         temperature = [temperature]
 
@@ -340,14 +368,21 @@
         vad_filter=args.pop("vad_filter"),
         vad_threshold=args.pop("vad_threshold"),
         vad_min_speech_duration_ms=args.pop("vad_min_speech_duration_ms"),
         vad_max_speech_duration_s=args.pop("vad_max_speech_duration_s"),
         vad_min_silence_duration_ms=args.pop("vad_min_silence_duration_ms"),
     )
 
+    if verbose:
+        cache_dir, exists = _does_old_cache_dir_has_files()
+        if exists:
+            print(
+                f"There are old cache files at `{cache_dir}` which are no longer used. Consider deleting them"
+            )
+
     if not verbose and options.print_colors:
         raise RuntimeError("You cannot disable verbose and enable print colors")
 
     if live_transcribe and not Live.is_available():
         Live.force_not_available_exception()
 
     if verbose and not language:
@@ -363,19 +398,20 @@
     output_dir = os.path.abspath(output_dir)
     if model_directory:
         model_filename = os.path.join(model_directory, "model.bin")
         if not os.path.exists(model_filename):
             raise RuntimeError(f"Model file '{model_filename}' does not exists")
         model_dir = model_directory
     else:
-        model_dir = Models(cache_directory).get_model_dir(model)
+        model_dir = model
 
     if live_transcribe:
         Live(
             model_dir,
+            cache_directory,
             task,
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
@@ -388,14 +424,16 @@
         sys.stderr.write("You need to specify one or more audio files\n")
         return
 
     for audio_path in audio:
         result = Transcribe().inference(
             audio_path,
             model_dir,
+            cache_directory,
+            local_files_only,
             task,
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
```

### Comparing `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.9
+Version: 0.2.0
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -62,14 +62,16 @@
 
 To translate:
 
     whisper-ctranslate2 inaguracio2011.mp3 --model medium --task translate
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/226923535-b6583536-2486-4127-b17b-c58d85cdb90f.png">
 
+Whisper translate task translates the transcription from the source language to English (the only target language supported).
+
 Additionally using:
 
     whisper-ctranslate2 --help
 
 All the supported options with their help are shown.
 
 # CTranslate2 specific options
@@ -113,17 +115,17 @@
 
     whisper-ctranslate2 myfile.mp3 --print_colors True
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
 ## Live transcribe from your microphone
 
-`----live_transcribe True` option activates the live transcription mode from your microphone:
+`--live_transcribe True` option activates the live transcription mode from your microphone:
 
-    whisper-ctranslate2 myfile.mp3 --print_colors True
+    whisper-ctranslate2 --live_transcribe True --language en
 
 https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
 
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
```

### Comparing `whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/whisper_ctranslate2/languages.py
 src/whisper_ctranslate2/live.py
-src/whisper_ctranslate2/models.py
 src/whisper_ctranslate2/transcribe.py
 src/whisper_ctranslate2/version.py
 src/whisper_ctranslate2/whisper_ctranslate2.py
 src/whisper_ctranslate2/writers.py
 whisper_ctranslate2.egg-info/PKG-INFO
 whisper_ctranslate2.egg-info/SOURCES.txt
 whisper_ctranslate2.egg-info/dependency_links.txt
```


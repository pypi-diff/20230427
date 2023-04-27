# Comparing `tmp/whisper-ctranslate2-0.2.0.tar.gz` & `tmp/whisper-ctranslate2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.0.tar", last modified: Wed Apr 26 16:31:18 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.1.tar", last modified: Thu Apr 27 12:20:43 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.0.tar` & `whisper-ctranslate2-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.0/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5641 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.0/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-26 15:07:48.000000 whisper-ctranslate2-0.2.0/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-26 16:27:40.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-19 16:58:21.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14312 2023-04-26 16:27:40.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-26 15:18:01.000000 whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 16:31:18.517226 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5641 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-26 16:31:18.000000 whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 12:20:43.445870 whisper-ctranslate2-0.2.1/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.1/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-27 12:20:43.445870 whisper-ctranslate2-0.2.1/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.1/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-27 12:20:43.445870 whisper-ctranslate2-0.2.1/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 11:58:54.000000 whisper-ctranslate2-0.2.1/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 12:20:43.441870 whisper-ctranslate2-0.2.1/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 12:20:43.441870 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-26 16:27:40.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-27 08:56:27.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15553 2023-04-27 11:52:25.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5803 2023-04-27 11:52:25.000000 whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 12:20:43.445870 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-27 12:20:43.000000 whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.0/LICENSE` & `whisper-ctranslate2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.0/PKG-INFO` & `whisper-ctranslate2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Whisper command line client that uses CTranslate2
-Home-page: https://github.com/jordimas/whisper-ctranslate2
+Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `whisper-ctranslate2-0.2.0/README.md` & `whisper-ctranslate2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.0/setup.py` & `whisper-ctranslate2-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 setup(
     name="whisper-ctranslate2",
     version=read_version(),
     description="Whisper command line client that uses CTranslate2",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/jordimas/whisper-ctranslate2",
+    url="https://github.com/Softcatala/whisper-ctranslate2",
     author="Jordi Mas",
     author_email="jmas@softcatala.org",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,259 +43,283 @@
 def read_command_line():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
     parser.add_argument(
         "audio", nargs="*", type=str, help="audio file(s) to transcribe"
     )
-    parser.add_argument(
+
+    model_args = parser.add_argument_group("Model selection options")
+
+    model_args.add_argument(
         "--model",
         default="small",
         choices=MODEL_NAMES,
         help="name of the Whisper model to use",
     )
-    parser.add_argument(
+
+    model_args.add_argument(
+        "--model_directory",
+        type=str,
+        default=None,
+        help="directory where to find a CTranslate Whisper model (e.g. fine-tuned model)",
+    )
+
+    caching_args = parser.add_argument_group("Model caching control options")
+
+    caching_args.add_argument(
         "--model_dir",
         type=str,
         default=None,
         help="the path to save model files; uses ~/.cache/huggingface/ by default",
     )
-    parser.add_argument(
+
+    caching_args.add_argument(
+        "--local_files_only",
+        type=str2bool,
+        default=False,
+        help="use models in cache without connecting to Internet to check if there are newer versions",
+    )
+
+    outputs_args = parser.add_argument_group(
+        "Configuration options to control generated outputs"
+    )
+
+    outputs_args.add_argument(
         "--output_dir",
         "-o",
         type=str,
         default=".",
         help="directory to save the outputs",
     )
-    parser.add_argument(
+    outputs_args.add_argument(
         "--output_format",
         "-f",
         type=str,
         default="all",
         choices=["txt", "vtt", "srt", "tsv", "json", "all"],
         help="format of the output file; if not specified, all available formats will be produced",
     )
 
-    parser.add_argument(
+    outputs_args.add_argument(
+        "--print_colors",
+        type=str2bool,
+        default=False,
+        help="print the transcribed text using an experimental color coding strategy to highlight words with high or low confidence",
+    )
+
+    outputs_args.add_argument(
         "--verbose",
         type=str2bool,
         default=True,
         help="whether to print out the progress and debug messages",
     )
 
-    parser.add_argument(
+    outputs_args.add_argument(
+        "--highlight_words",
+        type=str2bool,
+        default=False,
+        help="underline each word as it is spoken in srt and vtt (requires --word_timestamps True)",
+    )
+
+    computing_args = parser.add_argument_group("Computing configuration options")
+
+    computing_args.add_argument(
+        "--device",
+        choices=[
+            "auto",
+            "cpu",
+            "cuda",
+        ],
+        default="auto",
+        help="device to use for CTranslate2 inference",
+    )
+
+    computing_args.add_argument(
+        "--threads",
+        type=optional_int,
+        default=0,
+        help="number of threads used for CPU inference",
+    )
+
+    computing_args.add_argument(
+        "--device_index",
+        nargs="*",
+        type=int,
+        default=0,
+        help="device IDs where to place this model on",
+    )
+
+    computing_args.add_argument(
+        "--compute_type",
+        choices=[
+            "default",
+            "auto",
+            "int8",
+            "int8_float16",
+            "int16",
+            "float16",
+            "float32",
+        ],
+        default="auto",
+        help="Type of quantization to use (see https://opennmt.net/CTranslate2/quantization.html)",
+    )
+
+    algorithm_args = parser.add_argument_group("Algorithm execution options")
+
+    algorithm_args.add_argument(
         "--task",
         type=str,
         default="transcribe",
         choices=["transcribe", "translate"],
         help="whether to perform X->X speech recognition ('transcribe') or X->English translation ('translate')",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--language",
         type=str,
         default=None,
         choices=sorted(LANGUAGES.keys())
         + sorted([k.title() for k in TO_LANGUAGE_CODE.keys()]),
         help="language spoken in the audio, specify None to perform language detection",
     )
-    parser.add_argument(
-        "--threads",
-        type=optional_int,
-        default=0,
-        help="number of threads used for CPU inference",
-    )
 
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--temperature", type=float, default=0, help="temperature to use for sampling"
     )
 
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--temperature_increment_on_fallback",
         type=optional_float,
         default=0.2,
         help="temperature to increase when falling back when the decoding fails to meet either of the thresholds below",
     )
 
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--best_of",
         type=optional_int,
         default=5,
         help="number of candidates when sampling with non-zero temperature",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--beam_size",
         type=optional_int,
         default=5,
         help="number of beams in beam search, only applicable when temperature is zero",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--patience",
         type=float,
         default=1.0,
         help="optional patience value to use in beam decoding, as in https://arxiv.org/abs/2204.05424, the default (1.0) is equivalent to conventional beam search",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--length_penalty",
         type=float,
         default=1.0,
         help="optional token length penalty coefficient (alpha) as in https://arxiv.org/abs/1609.08144, uses simple length normalization by default",
     )
 
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--suppress_tokens",
         type=str,
         default="-1",
         help="comma-separated list of token ids to suppress during sampling; '-1' will suppress most special characters except common punctuations",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--initial_prompt",
         type=str,
         default=None,
         help="optional text to provide as a prompt for the first window.",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--condition_on_previous_text",
         type=str2bool,
         default=True,
         help="if True, provide the previous output of the model as a prompt for the next window; disabling may make the text inconsistent across windows, but the model becomes less prone to getting stuck in a failure loop",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--compression_ratio_threshold",
         type=optional_float,
         default=2.4,
         help="if the gzip compression ratio is higher than this value, treat the decoding as failed",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--logprob_threshold",
         type=optional_float,
         default=-1.0,
         help="if the average log probability is lower than this value, treat the decoding as failed",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--no_speech_threshold",
         type=optional_float,
         default=0.6,
         help="if the probability of the <|nospeech|> token is higher than this value AND the decoding has failed due to `logprob_threshold`, consider the segment as silence",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--word_timestamps",
         type=str2bool,
         default=False,
         help="(experimental) extract word-level timestamps and refine the results based on them",
     )
 
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--prepend_punctuations",
         type=str,
         default="\"'“¿([{-",
         help="if word_timestamps is True, merge these punctuation symbols with the next word",
     )
-    parser.add_argument(
+    algorithm_args.add_argument(
         "--append_punctuations",
         type=str,
         default="\"'.。,，!！?？:：”)]}、",
         help="if word_timestamps is True, merge these punctuation symbols with the previous word",
     )
 
-    parser.add_argument(
-        "--device",
-        choices=[
-            "auto",
-            "cpu",
-            "cuda",
-        ],
-        default="auto",
-        help="device to use for CTranslate2 inference",
-    )
+    vad_args = parser.add_argument_group("VAD filter arguments")
 
-    parser.add_argument(
+    vad_args.add_argument(
         "--vad_filter",
         type=bool,
         default=False,
-        help="Enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.",
+        help="enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.",
     )
 
-    parser.add_argument(
+    vad_args.add_argument(
         "--vad_threshold",
         type=float,
         default=None,
-        help="When `vad_filter` is enabled, probabilities above this value are considered as speech.",
+        help="when `vad_filter` is enabled, probabilities above this value are considered as speech.",
     )
 
-    parser.add_argument(
+    vad_args.add_argument(
         "--vad_min_speech_duration_ms",
         type=int,
         default=None,
-        help="When `vad_filter` is enabled, final speech chunks shorter min_speech_duration_ms are thrown out.",
+        help="when `vad_filter` is enabled, final speech chunks shorter min_speech_duration_ms are thrown out.",
     )
 
-    parser.add_argument(
+    vad_args.add_argument(
         "--vad_max_speech_duration_s",
         type=int,
         default=None,
-        help="When `vad_filter` is enabled, Maximum duration of speech chunks in seconds. Longer will be split at the timestamp of the last silence.",
+        help="when `vad_filter` is enabled, Maximum duration of speech chunks in seconds. Longer will be split at the timestamp of the last silence.",
     )
 
-    parser.add_argument(
+    vad_args.add_argument(
         "--vad_min_silence_duration_ms",
         type=int,
         default=None,
-        help="When `vad_filter` is enabled, in the end of each speech chunk time to wait before separating it.",
-    )
-
-    # CTranslate2 specific parameters
-    parser.add_argument(
-        "--local_files_only",
-        type=str2bool,
-        default=False,
-        help="Use models in cache without connecting to Internet to check if there are newer versions",
-    )
-
-    parser.add_argument(
-        "--device_index",
-        nargs="*",
-        type=int,
-        default=0,
-        help="Device IDs where to place this model on",
-    )
-
-    parser.add_argument(
-        "--compute_type",
-        choices=[
-            "default",
-            "auto",
-            "int8",
-            "int8_float16",
-            "int16",
-            "float16",
-            "float32",
-        ],
-        default="auto",
-        help="Type of quantization to use (see https://opennmt.net/CTranslate2/quantization.html)",
-    )
-    parser.add_argument(
-        "--model_directory",
-        type=str,
-        default=None,
-        help="Directory where to find a CTranslate Whisper model (e.g. fine-tuned model)",
-    )
-
-    # Whisper-ctranslate2 specific parameters
-    parser.add_argument(
-        "--print_colors",
-        type=str2bool,
-        default=False,
-        help="Print the transcribed text using an experimental color coding strategy to highlight words with high or low confidence",
+        help="when `vad_filter` is enabled, in the end of each speech chunk time to wait before separating it.",
     )
 
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
-        help="Show program's version number and exit",
+        help="show program's version number and exit",
     )
 
     parser.add_argument(
         "--live_transcribe", type=str2bool, default=False, help="Live transcribe mode"
     )
 
     return parser.parse_args().__dict__
@@ -324,14 +348,15 @@
     model_directory: str = args.pop("model_directory")
     cache_directory: str = args.pop("model_dir")
     device_index: Union[int, List[int]] = args.pop("device_index")
     suppress_tokens: str = args.pop("suppress_tokens")
     live_transcribe: bool = args.pop("live_transcribe")
     audio: str = args.pop("audio")
     local_files_only: bool = args.pop("local_files_only")
+    highlight_words: bool = args.pop("highlight_words")
 
     temperature = args.pop("temperature")
     if (increment := args.pop("temperature_increment_on_fallback")) is not None:
         temperature = tuple(np.arange(temperature, 1.0 + 1e-6, increment))
     else:
         temperature = [temperature]
 
@@ -368,14 +393,25 @@
         vad_filter=args.pop("vad_filter"),
         vad_threshold=args.pop("vad_threshold"),
         vad_min_speech_duration_ms=args.pop("vad_min_speech_duration_ms"),
         vad_max_speech_duration_s=args.pop("vad_max_speech_duration_s"),
         vad_min_silence_duration_ms=args.pop("vad_min_silence_duration_ms"),
     )
 
+    if len(audio) == 0:
+        sys.stderr.write("You need to specify one or more audio files\n")
+        sys.stderr.write(
+            "Use `whisper-ctranslate2 --help` to see the available options.\n"
+        )
+        return
+
+    if not options.word_timestamps and highlight_words:
+        sys.stderr.write("--highlight_words requires --word_timestamps True\n")
+        return
+
     if verbose:
         cache_dir, exists = _does_old_cache_dir_has_files()
         if exists:
             print(
                 f"There are old cache files at `{cache_dir}` which are no longer used. Consider deleting them"
             )
 
@@ -416,17 +452,15 @@
             compute_type,
             verbose,
             options,
         ).inference()
 
         return
 
-    if len(audio) == 0:
-        sys.stderr.write("You need to specify one or more audio files\n")
-        return
+    writer_args = {"highlight_words": highlight_words}
 
     for audio_path in audio:
         result = Transcribe().inference(
             audio_path,
             model_dir,
             cache_directory,
             local_files_only,
@@ -437,15 +471,15 @@
             device_index,
             compute_type,
             verbose,
             False,
             options,
         )
         writer = get_writer(output_format, output_dir)
-        writer(result, audio_path)
+        writer(result, audio_path, writer_args)
 
     if verbose:
         print(f"Transcription results written to '{output_dir}' directory")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `whisper-ctranslate2-0.2.0/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.1/src/whisper_ctranslate2/writers.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,51 +30,52 @@
 
 class ResultWriter:
     extension: str
 
     def __init__(self, output_dir: str):
         self.output_dir = output_dir
 
-    def __call__(self, result: dict, audio_path: str):
+    def __call__(self, result: dict, audio_path: str, options: dict):
         audio_basename = os.path.basename(audio_path)
         audio_basename = os.path.splitext(audio_basename)[0]
         output_path = os.path.join(
             self.output_dir, audio_basename + "." + self.extension
         )
 
         with open(output_path, "w", encoding="utf-8") as f:
-            self.write_result(result, file=f)
+            self.write_result(result, f, options)
 
-    def write_result(self, result: dict, file: TextIO):
+    def write_result(self, result: dict, file: TextIO, options: dict):
         raise NotImplementedError
 
 
 class SubtitlesWriter(ResultWriter):
     always_include_hours: bool
     decimal_marker: str
 
-    def iterate_result(self, result: dict):
+    def iterate_result(self, result: dict, options: dict):
         for segment in result["segments"]:
             segment_start = self.format_timestamp(segment["start"])
             segment_end = self.format_timestamp(segment["end"])
             segment_text = segment["text"].strip().replace("-->", "->")
+            highlight = options.get("highlight_words", False)
 
             if word_timings := segment["words"]:
                 all_words = [timing["word"] for timing in word_timings]
                 all_words[0] = all_words[0].strip()  # remove the leading space, if any
                 last = segment_start
                 for i, this_word in enumerate(word_timings):
                     start = self.format_timestamp(this_word["start"])
                     end = self.format_timestamp(this_word["end"])
                     if last != start:
                         yield last, start, segment_text
 
                     yield start, end, "".join(
                         [
-                            f"<u>{word}</u>" if j == i else word
+                            f"<u>{word}</u>" if j == i and highlight else word
                             for j, word in enumerate(all_words)
                         ]
                     )
                     last = end
 
                 if last != segment_end:
                     yield last, segment_end, segment_text
@@ -88,37 +89,39 @@
             decimal_marker=self.decimal_marker,
         )
 
 
 class WriteTXT(ResultWriter):
     extension: str = "txt"
 
-    def write_result(self, result: dict, file: TextIO):
+    def write_result(self, result: dict, file: TextIO, options: dict):
         for segment in result["segments"]:
             print(segment["text"].strip(), file=file, flush=True)
 
 
 class WriteSRT(SubtitlesWriter):
     extension: str = "srt"
     always_include_hours: bool = True
     decimal_marker: str = ","
 
-    def write_result(self, result: dict, file: TextIO):
-        for i, (start, end, text) in enumerate(self.iterate_result(result), start=1):
+    def write_result(self, result: dict, file: TextIO, options: dict):
+        for i, (start, end, text) in enumerate(
+            self.iterate_result(result, options), start=1
+        ):
             print(f"{i}\n{start} --> {end}\n{text}\n", file=file, flush=True)
 
 
 class WriteVTT(SubtitlesWriter):
     extension: str = "vtt"
     always_include_hours: bool = False
     decimal_marker: str = "."
 
-    def write_result(self, result: dict, file: TextIO):
+    def write_result(self, result: dict, file: TextIO, options: dict):
         print("WEBVTT\n", file=file)
-        for start, end, text in self.iterate_result(result):
+        for start, end, text in self.iterate_result(result, options):
             print(f"{start} --> {end}\n{text}\n", file=file, flush=True)
 
 
 class WriteTSV(ResultWriter):
     """
     Write a transcript to a file in TSV (tab-separated values) format containing lines like:
     <start time in integer milliseconds>\t<end time in integer milliseconds>\t<transcript text>
@@ -126,41 +129,43 @@
     Using integer milliseconds as start and end times means there's no chance of interference from
     an environment setting a language encoding that causes the decimal in a floating point number
     to appear as a comma; also is faster and more efficient to parse & store, e.g., in C++.
     """
 
     extension: str = "tsv"
 
-    def write_result(self, result: dict, file: TextIO):
+    def write_result(self, result: dict, file: TextIO, options: dict):
         print("start", "end", "text", sep="\t", file=file)
         for segment in result["segments"]:
             print(round(1000 * segment["start"]), file=file, end="\t")
             print(round(1000 * segment["end"]), file=file, end="\t")
             print(segment["text"].strip().replace("\t", " "), file=file, flush=True)
 
 
 class WriteJSON(ResultWriter):
     extension: str = "json"
 
-    def write_result(self, result: dict, file: TextIO):
+    def write_result(self, result: dict, file: TextIO, options: dict):
         json.dump(result, file)
 
 
-def get_writer(output_format: str, output_dir: str) -> Callable[[dict, TextIO], None]:
+def get_writer(
+    output_format: str, output_dir: str
+) -> Callable[[dict, TextIO, dict], None]:
     writers = {
         "txt": WriteTXT,
         "vtt": WriteVTT,
         "srt": WriteSRT,
         "tsv": WriteTSV,
         "json": WriteJSON,
     }
 
     if output_format == "all":
         all_writers = [writer(output_dir) for writer in writers.values()]
 
-        def write_all(result: dict, file: TextIO):
+        def write_all(result: dict, file: TextIO, options: dict):
             for writer in all_writers:
-                writer(result, file)
+                writer(result, file, options)
 
         return write_all
 
     return writers[output_format](output_dir)
```

### Comparing `whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Whisper command line client that uses CTranslate2
-Home-page: https://github.com/jordimas/whisper-ctranslate2
+Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `whisper-ctranslate2-0.2.0/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.1/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


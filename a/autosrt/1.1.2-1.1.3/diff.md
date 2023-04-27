# Comparing `tmp/autosrt-1.1.2.tar.gz` & `tmp/autosrt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.1.2.tar", last modified: Wed Apr  5 20:01:02 2023, max compression
+gzip compressed data, was "autosrt-1.1.3.tar", last modified: Thu Apr 27 11:43:27 2023, max compression
```

## Comparing `autosrt-1.1.2.tar` & `autosrt-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 20:01:02.433206 autosrt-1.1.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2454 2023-04-05 20:01:02.433955 autosrt-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3799 2023-02-13 02:23:24.000000 autosrt-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 20:01:02.414475 autosrt-1.1.2/autosrt/
--rw-rw-rw-   0        0        0    28631 2023-04-05 19:59:20.000000 autosrt-1.1.2/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:01:02.430957 autosrt-1.1.2/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2454 2023-04-05 20:01:01.000000 autosrt-1.1.2/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-05 20:01:02.000000 autosrt-1.1.2/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 20:01:01.000000 autosrt-1.1.2/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-05 20:01:01.000000 autosrt-1.1.2/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-04-05 20:01:01.000000 autosrt-1.1.2/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-05 20:01:01.000000 autosrt-1.1.2/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-05 20:01:02.435453 autosrt-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1884 2023-04-05 19:59:49.000000 autosrt-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.306422 autosrt-1.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2454 2023-04-27 11:43:27.307174 autosrt-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3799 2023-02-13 02:23:24.000000 autosrt-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.277954 autosrt-1.1.3/autosrt/
+-rw-rw-rw-   0        0        0    29249 2023-04-27 11:33:00.000000 autosrt-1.1.3/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.304924 autosrt-1.1.3/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2454 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-27 11:43:27.000000 autosrt-1.1.3/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-27 11:43:27.309420 autosrt-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1858 2023-04-27 11:28:48.000000 autosrt-1.1.3/setup.py
```

### Comparing `autosrt-1.1.2/LICENSE` & `autosrt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.1.2/PKG-INFO` & `autosrt-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.1.2
+Version: 1.1.3
 Summary: autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.1.2/README.md` & `autosrt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.1.2/autosrt/__init__.py` & `autosrt-1.1.3/autosrt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 from progressbar import ProgressBar, Percentage, Bar, ETA
 import pysrt
 import six
 # ADDITIONAL IMPORT FOR GoogleTranslate()
-import httpx
 from glob import glob
 # ADDITIONAL IMPORT FOR FfmpegProgress
 from ffmpeg_progress_yield import FfmpegProgress
 
 GOOGLE_SPEECH_API_KEY = "AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw"
 GOOGLE_SPEECH_API_URL = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}" # pylint: disable=line-too-long
 
@@ -418,15 +417,15 @@
                     except:
                         # no result
                         continue
 
         except KeyboardInterrupt:
             return
 
-
+'''
 def GoogleTranslate(text, src, dst):
     url = 'https://translate.googleapis.com/translate_a/'
     params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
     with httpx.Client(http2=True) as client:
         client.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',})
         response = client.get(url+params)
         #print('response.status_code = {}'.format(response.status_code))
@@ -437,14 +436,29 @@
             #print('length = {}'.format(length))
             translation = ""
             for i in range(length):
                 #print("{} {}".format(i, response_json[i][0]))
                 translation = translation + response_json[i][0]
             return translation
         return
+'''
+
+def GoogleTranslate(text, src, dst):
+    url = 'https://translate.googleapis.com/translate_a/'
+    params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
+    response = requests.get(url+params, headers=headers)
+    if response.status_code == 200:
+        response_json = response.json()[0]
+        length = len(response_json)
+        translation = ""
+        for i in range(length):
+            translation = translation + response_json[i][0]
+        return translation
+    return
 
 
 class SentenceTranslator(object):
     def __init__(self, src, dest, patience=-1):
         self.src = src
         self.dest = dest
         self.patience = patience
@@ -593,15 +607,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('source_path', help="Path to the video or audio files to generate subtitle (use wildcard for multiple files)", nargs='*')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
     parser.add_argument('-o', '--output', help="Output path for subtitles (by default, subtitles are saved in the same directory and name as the source path)")
     parser.add_argument('-F', '--format', help="Destination subtitle format", default="srt")
     parser.add_argument('-S', '--src-language', help="Language spoken in source file", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired language for the subtitles")
-    parser.add_argument('-v', '--version', action='version', version='1.1.2')
+    parser.add_argument('-v', '--version', action='version', version='1.1.3')
     parser.add_argument('-lf', '--list-formats', help="List all available subtitle formats", action='store_true')
     parser.add_argument('-ll', '--list-languages', help="List all available source/destination languages", action='store_true')
 
     args = parser.parse_args()
 
     if args.list_formats:
         print("List of formats:")
```

### Comparing `autosrt-1.1.2/autosrt.egg-info/PKG-INFO` & `autosrt-1.1.3/autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.1.2
+Version: 1.1.3
 Summary: autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.1.2/setup.py` & `autosrt-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'different language, and finally saves the resulting subtitles to disk. '
     'It supports a variety of input and output languages  and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 setup(
     name="autosrt",
-    version="1.1.2",
+    version="1.1.3",
     description="autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/autosrt",
     packages=[str("autosrt")],
     entry_points={
@@ -31,12 +31,11 @@
         ],
     },
     install_requires=[
         "requests>=2.3.0",
         "pysrt>=1.0.1",
         "progressbar2>=3.34.3",
         "six>=1.11.0",
-        "httpx>=0.13.3",
         "ffmpeg_progress_yield>=0.7.2",
     ],
     license=open("LICENSE").read()
 )
```


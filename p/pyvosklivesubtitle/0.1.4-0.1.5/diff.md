# Comparing `tmp/pyvosklivesubtitle-0.1.4.tar.gz` & `tmp/pyvosklivesubtitle-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.1.4.tar", last modified: Mon Apr 24 12:34:30 2023, max compression
+gzip compressed data, was "pyvosklivesubtitle-0.1.5.tar", last modified: Thu Apr 27 13:24:16 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.4.tar` & `pyvosklivesubtitle-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:34:30.003602 pyvosklivesubtitle-0.1.4/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1617 2023-04-24 12:34:30.004352 pyvosklivesubtitle-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:34:29.979113 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0   142738 2023-04-24 11:46:18.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:34:30.000605 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1617 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-24 12:34:29.000000 pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-24 12:34:30.007347 pyvosklivesubtitle-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1610 2023-04-24 12:32:33.000000 pyvosklivesubtitle-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.932245 pyvosklivesubtitle-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1617 2023-04-27 13:24:16.932995 pyvosklivesubtitle-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.906771 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0   143370 2023-04-27 12:27:06.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.929998 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1617 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-27 13:24:16.936740 pyvosklivesubtitle-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1610 2023-04-27 12:28:32.000000 pyvosklivesubtitle-0.1.5/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.4/LICENSE` & `pyvosklivesubtitle-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.4/PKG-INFO` & `pyvosklivesubtitle-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.4/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1201,15 +1201,15 @@
                 if patience == -1:
                     continue
                 patience -= 1
             else:
                 fail_to_translate = False
         return translated_sentence
 
-
+'''
 def GoogleTranslate(text, src, dst):
     url = 'https://translate.googleapis.com/translate_a/'
     params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
     with httpx.Client(http2=True) as client:
         client.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',})
         response = client.get(url+params)
         #print("response.status_code = {}".format(response.status_code))
@@ -1221,14 +1221,29 @@
                 #print("length = {}".format(length))
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
 
 
 def worker_timed_translate(src, dst):
     global main_window, recognizing
 
     while (recognizing==True):
         if not recognizing:
@@ -2566,15 +2581,15 @@
     parser.add_argument("-af", "--audio-filename", type=str, metavar="AUDIO_FILENAME", help="audio file to store recording to", default=None)
     parser.add_argument("-d", "--device", type=int_or_str, help="input device (numeric ID or substring)")
     parser.add_argument("-r", "--samplerate", type=int, help="sampling rate in Hertz for example 8000, 16000, 44100, or 48000", default=16000)
 
     parser.add_argument("-u", "--url", type=str, metavar="URL", help="URL of live streaming if you want to record the streaming")
     parser.add_argument("-vf", "--video-filename", type=str, metavar="VIDEO_FILENAME", help="video file to store recording to", default=None)
 
-    parser.add_argument('-v', '--version', action='version', version='0.1.4')
+    parser.add_argument('-v', '--version', action='version', version='0.1.5')
 
     args = parser.parse_args(remaining)
     args = parser.parse_args()
 
     if args.src_language:
         src = args.src_language
         last_selected_src = src
```

### Comparing `pyvosklivesubtitle-0.1.4/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.4/setup.py` & `pyvosklivesubtitle-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'pyvosklivesubtitle is a python based desktop aplication which can recognize any live streaming'
     'in 21 languages that supported by VOSK then translate and display it as LIVE SUBTITLES'
     )
 
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
-    version="0.1.4",
+    version="0.1.5",
     include_package_data=True,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
```


# Comparing `tmp/topcast-0.1.6.tar.gz` & `tmp/topcast-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topcast-0.1.6.tar", last modified: Wed Apr 26 19:10:19 2023, max compression
+gzip compressed data, was "topcast-0.1.7.tar", last modified: Thu Apr 27 21:25:21 2023, max compression
```

## Comparing `topcast-0.1.6.tar` & `topcast-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 19:10:03.000000 topcast-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-26 19:10:19.362921 topcast-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-26 19:10:03.000000 topcast-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:10:19.362921 topcast-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 19:10:03.000000 topcast-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.358921 topcast-0.1.6/topcast/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast/chatgpt_themes/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/conclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/interview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/none_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/chatgpt_themes/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/cutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/topcaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast/tts_providers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-26 19:10:03.000000 topcast-0.1.6/topcast/tts_providers/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:10:19.362921 topcast-0.1.6/topcast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 19:10:19.000000 topcast-0.1.6/topcast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:21.767693 topcast-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 21:25:05.000000 topcast-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-27 21:25:21.767693 topcast-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-27 21:25:05.000000 topcast-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:25:21.767693 topcast-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 21:25:05.000000 topcast-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:21.763693 topcast-0.1.7/topcast/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:21.767693 topcast-0.1.7/topcast/chatgpt_themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/conclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/interview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/none_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/chatgpt_themes/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/cutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/topcaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:21.767693 topcast-0.1.7/topcast/tts_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/tts_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/tts_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/tts_providers/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/tts_providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 21:25:05.000000 topcast-0.1.7/topcast/tts_providers/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:21.763693 topcast-0.1.7/topcast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-27 21:25:21.000000 topcast-0.1.7/topcast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 21:25:21.000000 topcast-0.1.7/topcast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:25:21.000000 topcast-0.1.7/topcast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 21:25:21.000000 topcast-0.1.7/topcast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 21:25:21.000000 topcast-0.1.7/topcast.egg-info/top_level.txt
```

### Comparing `topcast-0.1.6/LICENSE.txt` & `topcast-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/PKG-INFO` & `topcast-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topcast
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for Topcast
 Home-page: https://github.com/gormlabenz/topcast
 Author: Gorm Labenz
 Author-email: gorm@labenz.io
 License: MIT
 Keywords: topcast tts text-to-speech gcp google openai elevenlabs
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Topcast: Turn Text into Podcasts with TTS and ChatGPT
 
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
+## Example
+Generated using ChatGPT themes: Introduction with the ElevenLabs TTS Provider, Interview with the GCP TTS Provider and Summary also with the ElevenLabs TTS Provider.
+
+
+
+https://user-images.githubusercontent.com/53308156/234994155-2921b28a-9caa-46fc-9608-5ef01881713e.mp4
+
 
 ## Example Implementation
 
 ```python
 from topcast import Topcaster, set_openai_api_key
 from topcast.chatgpt_themes import Introduction
```

### Comparing `topcast-0.1.6/README.md` & `topcast-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Topcast: Turn Text into Podcasts with TTS and ChatGPT
 
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
+## Example
+Generated using ChatGPT themes: Introduction with the ElevenLabs TTS Provider, Interview with the GCP TTS Provider and Summary also with the ElevenLabs TTS Provider.
+
+
+
+https://user-images.githubusercontent.com/53308156/234994155-2921b28a-9caa-46fc-9608-5ef01881713e.mp4
+
 
 ## Example Implementation
 
 ```python
 from topcast import Topcaster, set_openai_api_key
 from topcast.chatgpt_themes import Introduction
```

### Comparing `topcast-0.1.6/setup.py` & `topcast-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="topcast",
-    version="0.1.6",
+    version="0.1.7",
     author="Gorm Labenz",
     author_email="gorm@labenz.io",
     description="A Python package for Topcast",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gormlabenz/topcast",
     packages=find_packages(),
```

### Comparing `topcast-0.1.6/topcast/chatgpt_themes/base.py` & `topcast-0.1.7/topcast/chatgpt_themes/base.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/chatgpt_themes/conclusion.py` & `topcast-0.1.7/topcast/chatgpt_themes/conclusion.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/chatgpt_themes/interview.py` & `topcast-0.1.7/topcast/chatgpt_themes/interview.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/chatgpt_themes/introduction.py` & `topcast-0.1.7/topcast/chatgpt_themes/introduction.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/chatgpt_themes/summary.py` & `topcast-0.1.7/topcast/chatgpt_themes/summary.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/cutter.py` & `topcast-0.1.7/topcast/cutter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 from pydub import AudioSegment
-from typing import List, Dict
+from typing import List, Dict, Union
 from .models import Timeline, ChapterData, AudioItem
 
 class Cutter:
     def __init__(self, timeline: Timeline):
         self.timeline = timeline
 
     def cut(self):
         topcast = AudioSegment.empty()
         
         self.set_raw_audio()
 
         for i, chapter in enumerate(self.timeline.timeline):
             main_audio = None
             overlays = []
-
+            
             for audio_item in chapter.audio_layers:
-                audio = audio_item.data.raw_audio
-
                 if audio_item.sets_length:
+                    audio = self.add_effects(audio_item.data.raw_audio, audio_item)
                     main_audio = audio
-                    padding_start = AudioSegment.silent(duration=audio_item.padding_start)
-                    main_audio = padding_start + main_audio
-                else:
+                
+            for audio_item in chapter.audio_layers:
+                if not audio_item.sets_length:
+                    audio = self.add_effects(audio_item.data.raw_audio[:len(main_audio)], audio_item)
                     overlays.append(audio)
-                    
+                
             if main_audio is not None:
                 chapter_audio = main_audio
-                
-                padding_end = AudioSegment.silent(duration=chapter.padding_end)
-                chapter_audio = chapter_audio + padding_end
-                
+                                
                 for overlay in overlays:
-                    if len(chapter_audio) == 0:
-                        chapter_audio = AudioSegment.silent(duration=len(overlay))
                     chapter_audio = chapter_audio.overlay(overlay)
-                    
-                chapter_audio = chapter_audio.fade_in(chapter.fade_in)
-                chapter_audio = chapter_audio.fade_out(chapter.fade_out)
                 
+                chapter_audio = self.add_effects(chapter_audio, chapter)
                 
                 topcast = topcast.append(chapter_audio, crossfade=chapter.crossfade if i > 0 else 0)
 
         return topcast
     
     def set_raw_audio(self):
         for chapter in self.timeline.timeline:
@@ -50,7 +43,19 @@
                 if not isinstance(audio_layer.data.raw_audio, AudioSegment):
                     raw_audio = AudioSegment.empty()
                     
                     for audio in audio_layer.data.audio_list:
                         raw_audio = raw_audio + audio
                         
                     audio_layer.data.raw_audio = raw_audio
+
+    def add_effects(self, audio: AudioSegment, audio_item: Union[AudioItem, ChapterData]):
+        padding_start = AudioSegment.silent(duration=audio_item.padding_start)
+        padding_end = AudioSegment.silent(duration=audio_item.padding_end)
+        
+        audio = padding_start + audio + padding_end
+
+        audio = audio.fade_in(audio_item.fade_in)
+        audio = audio.fade_out(audio_item.fade_out)
+
+        # audio = audio.apply_gain(audio_item.volume)
+        return audio
```

### Comparing `topcast-0.1.6/topcast/models.py` & `topcast-0.1.7/topcast/models.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/topcaster.py` & `topcast-0.1.7/topcast/topcaster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import asyncio
 from pydub import AudioSegment
 
-from .models import Timeline, AudioItem, ChapterData, Chapter
+from .models import Timeline, AudioItem, ChapterData, Chapter,AudioLayer
 from .cutter import Cutter
 
 class Topcaster:
     def __init__(self, timeline: Timeline = []):
         self.timeline = Timeline(timeline=timeline)
         self.topcast = AudioSegment.empty()
         self.already_generated = False
         
     def add_chapter(self, audio_layers = [], fade_in: int = 1, fade_out: int = 1 , padding_start: int = 0 , padding_end: int = 0 , crossfade: int = 0, volume: float = 1):
         self.already_generated = False
-        
+
         chapter = Chapter(audio_layers=audio_layers, fade_in=fade_in, fade_out=fade_out, padding_start=padding_start, padding_end=padding_end, crossfade=crossfade, volume=volume)
+        
+        
         self.timeline.timeline.append(chapter)
         
     def generate(self):        
         self.set_length_setter()
         self.add_chapter_data_dict()
         self.open_audio_files()
         asyncio.run(self.generate_text())
@@ -27,26 +29,24 @@
         self.already_generated = True
         return self.topcast
 
     def set_length_setter(self):
         for chapter in self.timeline.timeline:
             have_set_length = False
             
-            if(len(chapter.audio_layers) == 1):
-                chapter.audio_layers[0].sets_length = True
-                print("Only one audio layer in chapter, setting length setter")
-                continue
-            
             for audio_layer in chapter.audio_layers:
                 if audio_layer.sets_length:
                     if have_set_length:
                         raise Exception("Only one audio layer can set the length of a chapter")
                     else:
-                        print("Setting length setter")
                         have_set_length = True
+                        
+            if not have_set_length:
+                chapter.audio_layers[0].sets_length = True
+            
                 
     def add_chapter_data_dict(self):
         for chapter in self.timeline.timeline:
             for audio_layer in chapter.audio_layers:
                 audio_layer.data = ChapterData(raw_audio= None, text_list=[], audio_list= [])
                 
     def open_audio_files(self):
```

### Comparing `topcast-0.1.6/topcast/tts_providers/elevenlabs.py` & `topcast-0.1.7/topcast/tts_providers/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/tts_providers/gcp.py` & `topcast-0.1.7/topcast/tts_providers/gcp.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast/tts_providers/gt.py` & `topcast-0.1.7/topcast/tts_providers/gt.py`

 * *Files identical despite different names*

### Comparing `topcast-0.1.6/topcast.egg-info/PKG-INFO` & `topcast-0.1.7/topcast.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topcast
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for Topcast
 Home-page: https://github.com/gormlabenz/topcast
 Author: Gorm Labenz
 Author-email: gorm@labenz.io
 License: MIT
 Keywords: topcast tts text-to-speech gcp google openai elevenlabs
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Topcast: Turn Text into Podcasts with TTS and ChatGPT
 
 Topcast is a Python package that allows you to transform text into a podcast using Text-to-Speech (TTS) and language models. With Topcast, you can provide a text, and the package will create a podcast with an introduction, interview, conclusion, sound effects, and more. Topcast supports various TTS providers and language models.
+## Example
+Generated using ChatGPT themes: Introduction with the ElevenLabs TTS Provider, Interview with the GCP TTS Provider and Summary also with the ElevenLabs TTS Provider.
+
+
+
+https://user-images.githubusercontent.com/53308156/234994155-2921b28a-9caa-46fc-9608-5ef01881713e.mp4
+
 
 ## Example Implementation
 
 ```python
 from topcast import Topcaster, set_openai_api_key
 from topcast.chatgpt_themes import Introduction
```

### Comparing `topcast-0.1.6/topcast.egg-info/SOURCES.txt` & `topcast-0.1.7/topcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*


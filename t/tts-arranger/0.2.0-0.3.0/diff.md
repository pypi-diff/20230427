# Comparing `tmp/tts_arranger-0.2.0.tar.gz` & `tmp/tts_arranger-0.3.0.tar.gz`

## Comparing `tts_arranger-0.2.0.tar` & `tts_arranger-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,36 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    24332 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    16624 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_abstract_writer.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_html_converter.py
+-rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_writer_example.py
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/checkers_default.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/exclude_ids.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/examples/tts_processor_example.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/examples/tts_writer_example.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/__init__.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/checker.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_abstract_reader.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_epub_reader.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_based_reader.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_html_reader.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_srt_reader.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/tts_reader/tts_text_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/tests/reader_test.py
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 tts_arranger-0.3.0/PKG-INFO
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/tts_processor.py` & `tts_arranger-0.3.0/src/tts_arranger/tts_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 import contextlib
 import copy
-import csv
 import json
 import os
 import re
 import string
 from pathlib import Path
 from typing import Optional
 
 import numpy as np  # type: ignore
 import TTS  # type: ignore
 from num2words import num2words  # type: ignore
-from pydub import AudioSegment  # type: ignore
-from pydub.silence import detect_silence  # type: ignore
 from TTS.utils.manage import ModelManager  # type: ignore
 from TTS.utils.synthesizer import Synthesizer  # type: ignore
 
 from .items.tts_item import TTS_Item
-from .utils.audio import numpy_to_segment
 from .utils.log import LOG_TYPE, bcolors, log
 
 
 class TTS_Processor:
     def __init__(self, model='', vocoder: str = '', preferred_speakers: Optional[list[str]] = None) -> None:
         """
         Initializes a new instance of the TTS class.
 
         :param model: Name of the text-to-speech model to use.
         :type model: str
 
         :param vocoder: Name of the vocoder to use.
         :type vocoder: str
 
-        :param preferred_speakers: A list of preferred speaker names for multi-speaker models to be used instead of the available speakers of the selected model (not yet implemented).
+        :param preferred_speakers: A list of preferred speaker names for multi-speaker models to be used instead of the available speakers of the selected model.
                                 If set to None, the default speaker(s) will be used.
-        :type preferred_speakers: list[str] or None
+        :type preferred_speakers: Optional[list[str]]
 
         :return: None
         """
         self.model = model or 'tts_models/en/vctk/vits'
         self.vocoder = vocoder
         self.silence_length = 100
         self.silence_threshold = -60
@@ -387,15 +383,14 @@
         """
         final_items = []
 
         if tts_items:
             length = len(start_end[0])
 
             opened = False
-            current_speaker = ''
             current_speaker_idx = 0
 
             for tts_item in tts_items:
                 pos = 0
 
                 found = False
 
@@ -501,25 +496,47 @@
         final_items: list[TTS_Item] = []
 
         for tts_item in tts_items:
             final_items += self._prepare_item(tts_item)
 
         return final_items
 
-    def synthesize_tts_item(self, tts_item: TTS_Item) -> AudioSegment:
+    def pad_length(self, numpy_wav: np.ndarray, duration: float) -> np.ndarray:
         """
-        Synthesize a single item and return a PyDub AudioSegment object
+        Pad a numpy array of audio samples with zeros to achieve a desired duration.
+
+        :param numpy_wav: A 1D numpy array of audio samples.
+        :type numpy_wav: np.ndarray
+
+        :param duration: The desired duration of the audio in seconds.
+        :type duration: float
+
+        :return: A 1D numpy array of padded audio samples with the desired duration.
+        :rtype: np.ndarray
+        """
+        sample_rate = int(self.synthesizer.output_sample_rate)
+        current_duration = len(numpy_wav) / sample_rate
+        if current_duration < duration:
+            padding_duration = duration - current_duration
+            padding_samples = int(padding_duration * sample_rate)
+            numpy_wav = np.pad(numpy_wav, (0, padding_samples), 'constant')
+        return numpy_wav
+
+    def synthesize_tts_item(self, tts_item: TTS_Item) -> np.ndarray:
+        """
+        Synthesize a single item and return a numpy array
 
         :param tts_item: TTS item to be synthesized
         :type tts_item: TTS_Item
 
-        :return: AudioSegment object of synthesized audio
-        :rtype: AudioSegment
+        :return: numpy array of synthesized audio
+        :rtype: np.ndarray
         """
-        segment = AudioSegment.empty()
+
+        numpy_wav = np.array([0], dtype=np.float32)
 
         if tts_item.text:
             try:
                 speaker = ''
 
                 if self.synthesizer.tts_model and self.synthesizer.tts_model.num_speakers > 1:
                     speaker = self.speakers[tts_item.speaker_idx % len(self.speakers)]
@@ -532,26 +549,26 @@
                     wav = self.synthesizer.tts(
                         text=tts_item.text,
                         speaker_name=speaker,
                     )
             except Exception as e:
                 raise Exception(f'Error synthesizing "{tts_item.text}: {e}".')
             else:
-                speech_segment = numpy_to_segment(np.array(wav), int(self.synthesizer.output_sample_rate))
+                numpy_wav = np.asarray(wav, dtype=np.float32)
 
-                # If length is predefined, add padding if necessary
-                if int(speech_segment.duration_seconds * 1000) < tts_item.length:
-                    speech_segment += AudioSegment.silent(int(tts_item.length - speech_segment.duration_seconds * 1000), int(self.synthesizer.output_sample_rate))
-                else:
-                    # Strip some silence away to make pauses easier to control
-                    silence = detect_silence(speech_segment, min_silence_len=self.silence_length, silence_thresh=self.silence_threshold)
-                    speech_segment = speech_segment[:silence[-1][0]]
+                # TODO: Reintroduce silence stripping?
+                #     # Strip some silence away to make pauses easier to control
+                #     silence = detect_silence(speech_segment, min_silence_len=self.silence_length, silence_thresh=self.silence_threshold)
+                #     speech_segment = speech_segment[:silence[-1][0]]
 
-                if isinstance(speech_segment, AudioSegment):
-                    speech_segment = speech_segment.apply_gain(-20 - speech_segment.dBFS)
+        numpy_wav = self.pad_length(numpy_wav, tts_item.length / 1000.0)
 
-                segment += speech_segment
-        else:
-            if tts_item.length > 0:
-                segment += AudioSegment.silent(tts_item.length, int(self.synthesizer.output_sample_rate))
+        return numpy_wav
 
-        return segment
+    def get_sample_rate(self) -> int:
+        """
+        Returns the sample rate
+
+        :return: sample rate
+        :rtype: int
+        """
+        return int(self.synthesizer.output_sample_rate)
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.3.0/src/tts_arranger/examples/tts_processor_example.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
 preferred_speakers = ['p273', 'p330']
 
 tts_items.append(TTS_Item('This is a test', 1))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
 
 simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
 simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/tts_writer.py` & `tts_arranger-0.3.0/src/tts_arranger/tts_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import os
 import subprocess
 import sys
 import tempfile
 from typing import Callable, Optional
 
 import ffmpeg  # type: ignore
+import numpy as np  # type: ignore
+import scipy.io.wavfile  # type: ignore
 from pathvalidate._filename import sanitize_filename
 from PIL import Image
-from pydub import AudioSegment  # type: ignore
 
 from .items.tts_chapter import TTS_Chapter  # type: ignore
 from .items.tts_item import TTS_Item  # type: ignore
 from .items.tts_project import TTS_Project  # type: ignore
+from .tts_abstract_writer import TTS_Abstract_Writer
 from .tts_processor import TTS_Processor
 from .utils.log import LOG_TYPE, bcolors, log  # type: ignore
 
 
-class TTS_Writer():
+class TTS_Writer(TTS_Abstract_Writer):
     """
     Class to process TTS projects (containing of chapters each containing a number of items) and to finally write an audio file including chapter metadata and chapter info
     """
 
     def __init__(self, project: TTS_Project = TTS_Project(),  base_path: str = '', output_format='m4b', model: str = '', vocoder: str = '', preferred_speakers: Optional[list[str]] = None) -> None:
         """
         Constructor for the TTS_Writer class.
@@ -38,102 +40,117 @@
         :type output_format: str
 
         :param model: The name of the model to be used. Default is an empty string.
         :type model: str
 
         :param vocoder: The name of the vocoder to be used. Default is an empty string.
         :type vocoder: str
+
+        :param preferred_speakers: A list of preferred speaker names for multi-speaker models to be used instead of the available speakers of the selected model.
+                                If set to None, the default speaker(s) will be used.
+        :type preferred_speakers: Optional[list[str]]
+
         :return: None
         """
+        super().__init__(preferred_speakers)
+
         self.NANOSECONDS_IN_ONE_SECOND = 1e9
 
         self.project = project
         self.project_path = base_path
         self.output_format = output_format
         self.model = model
         self.vocoder = vocoder
 
         self.temp_files: list[tuple[str, str]] = []
-        self.preferred_speakers = preferred_speakers or []
 
-    def _get_nanoseconds_for_file(self, file_name):
+    def _get_nanoseconds_for_file(self, filename: str):
         """
         Get the duration of an audio file in nanoseconds.
 
-        :param file_name: The file name (including the path) of the audio file to get the duration of.
-        :type file_name: str
+        :param filename: The file name (including path) of the audio file to get the duration of.
+        :type filename: str
 
         :return: The duration of the audio file in nanoseconds.
         :rtype: int
         """
-        result = ffmpeg.probe(file_name, cmd='ffprobe', show_entries='format=duration')
+        result = ffmpeg.probe(filename, cmd='ffprobe', show_entries='format=duration')
         return int(float(result['format']['duration']) * self.NANOSECONDS_IN_ONE_SECOND)
 
-    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Callable[[float, TTS_Item], None] | None = None, max_pause_duration=0) -> None:
+    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Optional[Callable[[float, TTS_Item], None]] = None, optimize=True, max_pause_duration=0, preprocess=True) -> None:
         """
         Private method for synthesizing chapters into audio.
 
         :param chapters: A list of TTS chapters containing text to be synthesized into audio.
         :type chapters: list[TTS_Chapter]
 
         :param temp_dir: Path to the temporary directory.
         :type temp_dir: str
 
         :param tts_arranger: ATTS_Arranger object to be used for synthesizing.
         :type tts_arranger: TTS_Arranger
 
         :param callback: An optional function that can be used to monitor the progress of the synthesis process.
-        :type callback: Callable[[float, TTS_Item], None] | None
+        :type callback: Optional[Callable[[float, TTS_Item], None]]
+
+        :param optimize: Defines if the chapter should be optimized before synthesizing.
+        :type optimize: boolean
+
+        :param max_pause_duration: An optional maximum duration (in milliseconds) of silence to be inserted between adjacent TTS items in the output audio file. 
+        :type max_pause_duration: int
+
+        :param preprocess: Defines if the chapter should be preprocessed before synthesizing.
+        :type preprocess: boolean
 
         :return: None
         :rtype: None
         """
 
         log(LOG_TYPE.INFO, f'Preprocessing items.')
 
         for chapter in chapters:
-            chapter.optimize(max_pause_duration)
-            chapter.tts_items = tts_processor.preprocess_items(chapter.tts_items)
+            if optimize:
+                chapter.optimize(max_pause_duration)
+            if preprocess:
+                chapter.tts_items = tts_processor.preprocess_items(chapter.tts_items)
 
         tts_processor.initialize()
+        self.sample_rate = tts_processor.get_sample_rate()
 
         total_items = 0
 
         for chapter in chapters:
             total_items += len(chapter.tts_items)
 
         current_total_items = 0
 
         cumulative_time = 0
 
         for i, chapter in enumerate(chapters):
-            audio = AudioSegment.empty()
+            numpy_segments = np.array([0], dtype=np.float32)
 
             temp_format = 'wav'
 
             filename = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
             if len(chapters) > 1:
                 log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}.')
 
             if len(chapter.tts_items) > 0:
                 for j, tts_item in enumerate(chapter.tts_items):
-                    if tts_item.text:
-                        log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)}:{bcolors.ENDC}')
-                    else:
-                        log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC}')
-
-                    # Synthesize audio from TTS item text
-                    audio += tts_processor.synthesize_tts_item(tts_item)
+                    self.print_progress(j, len(chapter.tts_items), tts_item)
 
                     if callback is not None:
                         callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
 
+                    # Synthesize audio from TTS item text
+                    numpy_segments = np.concatenate((numpy_segments, tts_processor.synthesize_tts_item(tts_item)))
+
                 # Write synthesized audio as temp file
-                self._write_temp_audio(audio, filename)
+                scipy.io.wavfile.write(filename, self.sample_rate, numpy_segments)
 
                 current_total_items += len(chapter.tts_items)
 
                 num_zeros = len(str(len(self.temp_files)))
                 chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
 
                 filename_out = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
@@ -219,52 +236,32 @@
 
             (
                 ffmpeg
                 .output(audio, cover, output_file, vcodec='copy', acodec='copy', map_metadata=0, **{'disposition:v:0': 'attached_pic'}, loglevel='error')
                 .run(overwrite_output=True)
             )
 
-    def _write_temp_audio(self, segment: AudioSegment, output_filename: str) -> None:
-        """
-        Convert and write chapter AudioSegment as temporary audio file for later concatenation
-
-        :param segment: AudioSegment to be written
-        :type segment: AudioSegment
-
-        :param output_filename: Absolute path and filename of output audio file including file type extension (for example mp3, ogg)
-        :type output_filename: str
-
-        :return: None
-        :rtype: None
-        """
-
-        comp_expansion = 12.5
-        comp_raise = 0.0001
-
-        # Apply dynamic compression
-        params = ['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1']
-        bitrate = '320k'
-        format = 'wav'
-        segment.export(output_filename, format, parameters=params, bitrate=bitrate)
-
-    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Callable[[float, TTS_Item], None] | None = None, max_pause_duration=0) -> None:
+    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Optional[Callable[[float, TTS_Item], None]] = None, max_pause_duration=0) -> None:
         """
         Synthesize and write the output audio files for the given project.
 
-        :param project_filename: The project name.
+        :param project_filename: The name or path of the project file to be synthesized.
         :type project_filename: str
 
         :param temp_dir_prefix: An optional prefix for the temporary directory name used during synthesis.
         :type temp_dir_prefix: str
 
         :param concat: A boolean value indicating whether to concatenate the audio files into a single file or not. Defaults to True.
         :type concat: bool
 
         :param callback: An optional callback function that will be called periodically during synthesis with progress information.
-        :type callback: Callable[[float, TTS_Item], None] | None
+        :type callback: Optional[Callable[[float, TTS_Item], None]]
+
+        :param max_pause_duration: An optional maximum duration (in milliseconds) of silence to be inserted between adjacent TTS items in the output audio file. 
+        :type max_pause_duration: int
 
         :return: None
 
         :raises: ValueError if `project_filename` is not a valid file path.
         """
 
         if not self.project.tts_chapters:
@@ -286,15 +283,15 @@
                             self.model = 'tts_models/de/thorsten/tacotron2-DDC'
                             self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
                         case _:
                             raise ValueError(f'Language code "{self.project.lang_code}" not supported')
 
                     t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
 
-                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback, max_pause_duration)
+                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback, not self.project.raw, max_pause_duration, not self.project.raw)
 
             except Exception as e:
                 log(LOG_TYPE.ERROR, f'Synthesizing project "{self.project.title}" failed: {e}.')
                 sys.exit(1)
 
             else:
                 if len(self.temp_files) > 0:
@@ -319,26 +316,30 @@
                     output_path = output_filename + output_extension
 
                     output_files: list[str] = []
 
                     # Create directory if needed
                     os.makedirs(self.project_path, exist_ok=True)
 
+                    comp_expansion = 12.5
+                    comp_raise = 0.0001
+
                     # Concatenate all files, adding metadata and cover image (if set)
                     if concat:
                         infiles = [ffmpeg.input(file) for _, file in self.temp_files]
 
                         metadata_input = ffmpeg.input(metadata_filename)
 
                         if self.output_format not in ['m4b', 'm4a']:
                             log(LOG_TYPE.WARNING, f'Chapters are only possible for m4b/m4a at the moment.')
 
                         cmd = (
                             ffmpeg
                             .concat(*infiles, v=0, a=1)
+                            .filter('speechnorm', e=f'{comp_expansion}', r=f'{comp_raise}', l=1)
                             .output(metadata_input, output_path, map_metadata=1, **{'metadata': f'title={self.project.title}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
                             .compile(overwrite_output=True)
                         )
 
                         # Remove last map parameter (workaround for ffmpeg-python bug)
                         cmd = self._remove_last_arg(cmd, '-map')
 
@@ -358,14 +359,15 @@
                             if self.output_format == 'mp3':
                                 output_args['audio_bitrate'] = '320k'
 
                             # Convert to target format, adding metadata
                             (
                                 ffmpeg
                                 .input(file)
+                                .filter('speechnorm', e=f'{comp_expansion}', r=f'{comp_raise}', l=1)
                                 .output(output_chapter_filename, **output_args, loglevel='error')
                                 .run(overwrite_output=True)
                             )
 
                             output_files.append(output_chapter_filename)
                         log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under "{output_filename}/".')
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.3.0/src/tts_arranger/items/tts_chapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
-from pydub import AudioSegment  # type: ignore
+import numpy as np
 
 from .tts_item import TTS_Item  # type: ignore
 
 
 @dataclass
 class TTS_Chapter():
     """
@@ -19,23 +19,23 @@
 
     :param start_time: A float representing the start time of the chapter in nanoseconds. Default value is 0.
     :type start_time: float
 
     :param end_time: A float representing the end time of the chapter in nanoseconds. Default value is 0.
     :type end_time: float
 
-    :param audio: An AudioSegment object representing the synthesized audio for the chapter. Default value is an empty AudioSegment object.
-    :type audio: AudioSegment
+    :param audio: An numpy array representing the synthesized audio for the chapter. Default value is an empty numpy array.
+    :type audio: np.ndarray
     """
     tts_items: list[TTS_Item] = field(default_factory=list)
 
     title: str = ''
     start_time = 0
     end_time = 0
-    audio = AudioSegment.empty()
+    audio = np.array([0], dtype=np.float32)
 
     def _merge_items(self, tts_items: list[TTS_Item]) -> list[TTS_Item]:
         final_items: list[TTS_Item] = []
         merged_item: Optional[TTS_Item] = None
 
         for tts_item in tts_items:
             if not merged_item:
@@ -84,7 +84,23 @@
         # Limit pause duration for pause items, ignore if max_pause_duration == 0
         for non_empty_item in non_empty_items:
             if non_empty_item.speaker_idx == -1 and max_pause_duration > 0:
                 if non_empty_item.length > max_pause_duration:
                     non_empty_item.length = max_pause_duration
 
         self.tts_items = non_empty_items
+
+    def get_title(self, only_empty=True, max_length=100) -> None:
+        """
+        Set title to the text of the first item
+
+        :param only_empty: Only set empty titles
+        :type only_empty: bool
+
+        :param max_length: Maximus title length, a '…' will be added after this
+        :type max_length: int
+
+        :return: None
+        """
+
+        if len(self.tts_items) > 0:
+            self.title = self.tts_items[0].text[:max_length] + '…' if len(self.tts_items[0].text) > max_length else self.tts_items[0].text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.3.0/src/tts_arranger/items/tts_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 class TTS_Item():
     """
     Represents a TTS item containing various information.
 
     :param text: The text to be synthesized. Can be left empty in combination with length > 0 to create a pause.
     :type text: str
 
-    :param speaker: The name of the speaker to be used.
-    :type speaker: str
-
     :param speaker_idx: The index of the speaker to be used if no speaker name is given. Wraps around based on the actual available speaker indexes per model.
     :type speaker_idx: int
 
     :param length: The minimum length in milliseconds. Will be padded if the actual synthesized text fragment is shorter, and ignored if it is longer.
     :type length: int
     """
     text: str = ''
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.3.0/src/tts_arranger/items/tts_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import base64
 import datetime
-from io import BytesIO
 import pickle
 from dataclasses import dataclass, field
-from typing import Optional
-from PIL import Image
 
 
 import requests  # type: ignore
 
 from ..utils.log import LOG_TYPE, log
 from .tts_chapter import TTS_Chapter  # type: ignore
 from .tts_item import TTS_Item  # type: ignore
@@ -35,25 +32,30 @@
     :type author: str
 
     :param lang_code: A string representing the language code of the project. Default value is 'en'.
     :type lang_code: str
 
     :param image_bytes: A bytes object representing the image of the project encoded as b64. Default value is an empty bytes object.
     :type image_bytes: bytes
+
+    :param raw: Defines if this should be synthesized without optimization and preprocessing.
+    :type raw: boolean
     """
 
     tts_chapters: list[TTS_Chapter] = field(default_factory=list)
 
     title: str = ''
     subtitle: str = ''
     date: datetime.datetime = datetime.datetime.min
     author: str = ''
     lang_code: str = 'en'
     image_bytes: bytes = bytes(0)
 
+    raw: bool = False
+
     @classmethod
     def from_json_file(cls, filename: str = ''):
         """
         Class method to load a TTS project from a JSON file.
 
         :param filename: A string representing the name of the JSON file to be loaded. Default value is an empty string.
         :type filename: str
@@ -80,28 +82,28 @@
         :return: A TTS project object loaded from the JSON file.
         :rtype: TTS_Project
         """
         return TTS_Project([TTS_Chapter(tts_items)])
 
     def merge_from_project(self, project) -> None:
         """
-        Method to merge the contents of another TTS project into this one.
+        Merges the contents of another TTS project into this one.
 
         :param project: The TTS project to be merged.
         :type project: TTS_Project
 
         :return: None
         :rtype: None
         """
         if isinstance(project, TTS_Project):
             self.tts_chapters += project.tts_chapters
 
     def append(self, items: list[TTS_Item]) -> None:
         """
-        Method to add a list of TTS items to the last TTS chapter of this TTS project.
+        Adds a list of TTS items to the last TTS chapter of this TTS project.
 
         :param items: A list of TTS items to be added to the last chapter.
         :type items: list[TTS_Item]
 
         :return: None
         :rtype: None
         """
@@ -109,15 +111,15 @@
         if not self.tts_chapters:
             self.tts_chapters.append(TTS_Chapter())
 
         self.tts_chapters[-1].tts_items += items
 
     def to_json_file(self, filename: str) -> None:
         """
-        Method to save the TTS project to a JSON file.
+        Saves the TTS project to a JSON file.
 
         :param filename: A string representing the name of the JSON file to be saved.
         :type filename: str
 
         :return: None
         :rtype: None
         """
@@ -125,25 +127,28 @@
             with open(filename, 'wb') as file:
                 pickle.dump(self, file)
         except IOError:
             log(LOG_TYPE.WARNING, f'TTS Project export file "{filename}" could not be opened for writing.')
 
     def add_image_from_url(self, image_url: str) -> None:
         """
-        Opens the image from the given URL and adds it via the private function.
+        Loads the image from the given URL and sets it as the project image.
 
         :param image_url: The URL of the image to be added.
         :type image_url: str
 
         :return: None
         """
         if image_url:
             self.image_bytes = base64.b64encode(requests.get(image_url).content)
 
-    def clean_empty_chapters(self):
+    def clean_empty_chapters(self):       
+        """
+        Remove empty chapters.
+        """         
         final_chapters: list[TTS_Chapter] = []
 
         for chapter in self.tts_chapters:
             if len(chapter.tts_items) > 0:
                 final_chapters.append(chapter)
 
         self.tts_chapters = final_chapters
@@ -156,7 +161,22 @@
         :type max_pause_duration: int
 
         :return: None
         """
 
         for chapter in self.tts_chapters:
             chapter.optimize(max_pause_duration)
+
+    def get_titles(self, only_empty=True, max_length=100) -> None:
+        """
+        Set chapter titles to the text of the first chapter's item
+
+        :param only_empty: Only set empty titles
+        :type only_empty: bool
+
+        :param max_length: Maximus title length, a '…' will be added after this
+        :type max_length: int
+
+        :return: None
+        """
+        for chapter in self.tts_chapters:
+            chapter.get_title(only_empty, max_length)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tts_arranger-0.2.0/src/tts_arranger/utils/log.py` & `tts_arranger-0.3.0/src/tts_arranger/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 class LOG_TYPE(Enum):
-    """Log types."""
+    """Log color types."""
     INFO = auto()
     WARNING = auto()
     ERROR = auto()
     SUCCESS = auto()
 
 
 def log(log_type: LOG_TYPE, message: str):
```

### Comparing `tts_arranger-0.2.0/tests/tts_arranger_test.py` & `tts_arranger-0.3.0/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.2.0/LICENSE` & `tts_arranger-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.2.0/README.md` & `tts_arranger-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,36 +8,57 @@
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
-tts_items.append(TTS_Item('This is a test', 'p330'))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'p273', length=10000))
+preferred_speakers = ['p273', 'p330']
+
+tts_items.append(TTS_Item('This is a test', 1))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
 
-simple_writer = TTS_Simple_Writer(tts_items)
+simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
 simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
-items1.append(TTS_Item('This is a test:', speaker_idx=0))
-items1.append(TTS_Item('This is another test:',  speaker_idx=1))
+items1.append(TTS_Item('This is a test:', 0))
+items1.append(TTS_Item('This is another test:', 1))
 
 items2 = []
-items2.append(TTS_Item('Another test',  speaker_idx=0))
-items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
+items2.append(TTS_Item('Another test',  0))
+items2.append(TTS_Item('This is getting boring!', 1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
+
+# German example using Thorsten voice (no multispeaker support)
+
+items1 = []
+items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
+items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
+
+items2 = []
+items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
+items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
+
+chapter = []
+chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
+chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
+
+project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

### Comparing `tts_arranger-0.2.0/pyproject.toml` & `tts_arranger-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.2.0"
+version = "0.3.0"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.2.0/PKG-INFO` & `tts_arranger-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,36 +22,57 @@
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
-tts_items.append(TTS_Item('This is a test', 'p330'))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'p273', length=10000))
+preferred_speakers = ['p273', 'p330']
+
+tts_items.append(TTS_Item('This is a test', 1))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
 
-simple_writer = TTS_Simple_Writer(tts_items)
+simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
 simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
-items1.append(TTS_Item('This is a test:', speaker_idx=0))
-items1.append(TTS_Item('This is another test:',  speaker_idx=1))
+items1.append(TTS_Item('This is a test:', 0))
+items1.append(TTS_Item('This is another test:', 1))
 
 items2 = []
-items2.append(TTS_Item('Another test',  speaker_idx=0))
-items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
+items2.append(TTS_Item('Another test',  0))
+items2.append(TTS_Item('This is getting boring!', 1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
+
+# German example using Thorsten voice (no multispeaker support)
+
+items1 = []
+items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
+items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
+
+items2 = []
+items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
+items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
+
+chapter = []
+chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
+chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
+
+project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```


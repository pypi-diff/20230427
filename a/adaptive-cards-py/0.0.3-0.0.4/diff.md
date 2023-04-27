# Comparing `tmp/adaptive-cards-py-0.0.3.tar.gz` & `tmp/adaptive-cards-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-cards-py-0.0.3.tar", last modified: Wed Apr 26 19:07:57 2023, max compression
+gzip compressed data, was "adaptive-cards-py-0.0.4.tar", last modified: Wed Apr 26 19:27:31 2023, max compression
```

## Comparing `adaptive-cards-py-0.0.3.tar` & `adaptive-cards-py-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.3/LICENSE
--rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-26 19:07:24.000000 adaptive-cards-py-0.0.3/MANIFEST.in
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6713 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/README.md
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/adaptive_cards/
--rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-26 18:21:59.000000 adaptive-cards-py-0.0.3/adaptive_cards/__init__.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/actions.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5180 2023-04-26 18:03:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/card.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     4402 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/card_types.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/containers.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/elements.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/inputs.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      246 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/interface.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.3/adaptive_cards/utils.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/adaptive_cards/validation.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8379 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)      591 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/SOURCES.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/dependency_links.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       17 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/requires.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-04-26 19:07:57.000000 adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/top_level.txt
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.562086 adaptive-cards-py-0.0.3/examples/
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/examples/simple_card/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/examples/simple_card/simple_card.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.3/examples/simple_card/simple_card_2.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)      621 2023-04-26 19:07:41.000000 adaptive-cards-py-0.0.3/pyproject.toml
--rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-04-26 19:07:57.572086 adaptive-cards-py-0.0.3/setup.cfg
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.4/LICENSE
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-26 19:07:24.000000 adaptive-cards-py-0.0.4/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8448 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6713 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.4/README.md
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/adaptive_cards/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-26 18:21:59.000000 adaptive-cards-py-0.0.4/adaptive_cards/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.4/adaptive_cards/actions.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5540 2023-04-26 19:26:05.000000 adaptive-cards-py-0.0.4/adaptive_cards/card.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     4592 2023-04-26 19:21:33.000000 adaptive-cards-py-0.0.4/adaptive_cards/card_types.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.4/adaptive_cards/containers.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.4/adaptive_cards/elements.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.4/adaptive_cards/inputs.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.4/adaptive_cards/utils.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.4/adaptive_cards/validation.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8448 2023-04-26 19:27:31.000000 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      563 2023-04-26 19:27:31.000000 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-04-26 19:27:31.000000 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       25 2023-04-26 19:27:31.000000 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-04-26 19:27:31.000000 adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/top_level.txt
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:27:31.852090 adaptive-cards-py-0.0.4/examples/
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/examples/simple_card/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.4/examples/simple_card/simple_card.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.4/examples/simple_card/simple_card_2.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      711 2023-04-26 19:27:15.000000 adaptive-cards-py-0.0.4/pyproject.toml
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-04-26 19:27:31.862090 adaptive-cards-py-0.0.4/setup.cfg
```

### Comparing `adaptive-cards-py-0.0.3/LICENSE` & `adaptive-cards-py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/PKG-INFO` & `adaptive-cards-py-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,14 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Homepage, https://github.com/dennis6p/adaptive-cards-py
 Keywords: bot,ui,adaptivecards,cards,adaptivecardsio,python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `adaptive-cards-py-0.0.3/README.md` & `adaptive-cards-py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/actions.py` & `adaptive-cards-py-0.0.4/adaptive_cards/actions.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/card.py` & `adaptive-cards-py-0.0.4/adaptive_cards/card.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 
 from adaptive_cards.actions import SelectAction, ActionT
 from adaptive_cards.containers import ContainerT
 from adaptive_cards.elements import ElementT
 from adaptive_cards.inputs import InputT
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, LetterCase, config
-from typing import Self, TypeVar, Optional
+from typing import TypeVar, Optional
 import adaptive_cards.card_types as ct
 import adaptive_cards.utils as utils
 from abc import ABC
 
+AdaptiveCardBuilder = TypeVar("AdaptiveCardBuilder", bound="AdaptiveCardBuilder")
+
 SCHEMA: str = "http://adaptivecards.io/schemas/adaptive-card.json"
 TYPE: str = "AdaptiveCard"
 VERSION: str = "1.0"
 
 AdaptiveCard = TypeVar("AdaptiveCard", bound="AdaptiveCard")
 
 class Builder(ABC):
@@ -22,91 +24,92 @@
 class AdaptiveCardBuilder(Builder):
     def __init__(self) -> None:
         self.__reset()
         
     def __reset(self) -> None:
         self.__card = AdaptiveCard()
     
-    def type(self, type: str) -> Self:
+    def type(self, type: str) -> AdaptiveCardBuilder:
         self.__card.type = type
         return self
         
-    def version(self, version: str) -> Self:
+    def version(self, version: str) -> AdaptiveCardBuilder:
         self.__card.version = version
         return self
     
-    def refresh(self, refresh: ct.Refresh) -> Self:
+    def refresh(self, refresh: ct.Refresh) -> AdaptiveCardBuilder:
         self.__card.refresh = refresh
         return self
     
-    def authentication(self, authentication: ct.Authentication) -> Self:
+    def authentication(self, authentication: ct.Authentication) -> AdaptiveCardBuilder:
         self.__card.authentication = authentication
         return self
     
-    def select_action(self, select_action: SelectAction) -> Self:
+    def select_action(self, select_action: SelectAction) -> AdaptiveCardBuilder:
         self.__card.select_action = select_action
         return self
     
-    def fallback_text(self, fallback_text: str) -> Self:
+    def fallback_text(self, fallback_text: str) -> AdaptiveCardBuilder:
         self.__card.fallback_text = fallback_text
         return self
     
-    def background_image(self, background_image: ct.BackgroundImage) -> Self:
+    def background_image(self, background_image: ct.BackgroundImage) -> AdaptiveCardBuilder:
         self.__card.background_image = background_image
         return self
     
-    def metadata(self, metadata: ct.Metadata) -> Self:
+    def metadata(self, metadata: ct.Metadata) -> AdaptiveCardBuilder:
         self.__card.metadata = metadata
         return self
     
-    def min_height(self, min_height: str) -> Self:
+    def min_height(self, min_height: str) -> AdaptiveCardBuilder:
         self.__card.min_height = min_height
         return self
     
-    def rtl(self, rtl: bool) -> Self:
+    def rtl(self, rtl: bool) -> AdaptiveCardBuilder:
         self.__card.rtl = rtl
         return self
     
-    def speak(self, speak: str) -> Self:
+    def speak(self, speak: str) -> AdaptiveCardBuilder:
         self.__card.speak = speak
         return self
     
-    def lang(self, lang: str) -> Self:
+    def lang(self, lang: str) -> AdaptiveCardBuilder:
         self.__card.lang = lang
         return self
     
-    def vertical_content_alignment(self, vertical_content_align: ct.VerticalAlignment) -> Self:
+    def vertical_content_alignment(self, 
+            vertical_content_align: ct.VerticalAlignment) -> AdaptiveCardBuilder:
         self.__card.vertical_content_align = vertical_content_align
         return self
 
-    def schema(self, version: str) -> Self:
+    def schema(self, version: str) -> AdaptiveCardBuilder:
         self.__card.version = version
         return self
     
-    def add_item(self, item: ElementT | ContainerT | InputT) -> Self:
+    def add_item(self, item: ElementT | ContainerT | InputT) -> AdaptiveCardBuilder:
         if self.__card.body is None:
             self.__card.body = list()
         self.__card.body.append(item)
         return self
     
-    def add_items(self, items: list[ElementT | ContainerT | InputT]) -> Self:
+    def add_items(self, items: list[ElementT | ContainerT | InputT]) -> AdaptiveCardBuilder:
         if self.__card.body is None:
             self.__card.body = list()
         for item in items:
             self.add_item(item)
         
         return self    
     
-    def add_action(self, action: ActionT) -> Self:
+    def add_action(self, action: ActionT) -> AdaptiveCardBuilder:
         if self.__card.actions is None:
             self.__card.actions = list()
         self.__card.actions.append(action)
         return self
     
-    def add_actions(self, actions: list[ActionT]) -> Self:
+    def add_actions(self, actions: list[ActionT]) -> AdaptiveCardBuilder:
         if self.__card.actions is None:
             self.__card.actions = list()
         for action in actions:
             self.add_action(action)
         
         return self
```

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/card_types.py` & `adaptive-cards-py-0.0.4/adaptive_cards/card_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 from dataclasses import dataclass, field
 from typing import Optional
 from dataclasses_json import config, dataclass_json, LetterCase
-from enum import StrEnum, auto
+from enum import auto
+from strenum import LowercaseStrEnum
 import adaptive_cards.utils as utils
 
-class ImageFillMode(StrEnum):
+class ImageFillMode(LowercaseStrEnum):
     COVER = auto()
     REPEAT_HORIZONTALLY = "repeatHorizontally"
     REPEAT_VERTICALLY = "repeatVertically" 
     REPEAT = auto()
       
-class HorizontalAlignment(StrEnum):
+class HorizontalAlignment(LowercaseStrEnum):
     LEFT = auto()
     CENTER = auto()
     RIGHT = auto()   
 
-class VerticalAlignment(StrEnum):
+class VerticalAlignment(LowercaseStrEnum):
     TOP = auto()
     CENTER = auto()
     BOTTOM = auto()  
 
-class Colors(StrEnum):
+class Colors(LowercaseStrEnum):
     DEFAULT = auto()
     DARK = auto()
     LIGHT = auto()
     ACCENT = auto()
     GOOD = auto()
     WARNING = auto()
     ATTENTION = auto()
     
-class FontType(StrEnum):
+class FontType(LowercaseStrEnum):
     DEFAULT = auto()
     MONOSPACE = auto()
     
-class FontSize(StrEnum):
+class FontSize(LowercaseStrEnum):
     DEFAULT = auto()
     SMALL = auto()
     MEDIUM = auto()
     LARGE = auto()
     EXTRA_LARGE = "extraLarge"
 
-class FontWeight(StrEnum):
+class FontWeight(LowercaseStrEnum):
     DEFAULT = auto()
     LIGHTER = auto()
     BOLDER = auto()
     
-class TextBlockStyle(StrEnum):
+class TextBlockStyle(LowercaseStrEnum):
     DEFAULT = auto()
     HEADING = auto()
     
-class BlockElementHeight(StrEnum):
+class BlockElementHeight(LowercaseStrEnum):
     AUTO = auto()
     STRETCH = auto()
 
-class ImageSize(StrEnum):
+class ImageSize(LowercaseStrEnum):
     AUTO = auto()
     STRETCH = auto()
     SMALL = auto()
     MEDIUM = auto()
     LARGE = auto()
     
-class ImageStyle(StrEnum):
+class ImageStyle(LowercaseStrEnum):
     DEFAULT = auto()
     PERSON = auto()
 
-class ContainerStyle(StrEnum):
+class ContainerStyle(LowercaseStrEnum):
     DEFAULT = auto()
     EMPHASIS = auto()
     GOOD = auto()
     ATTENTION = auto()
     WARNING = auto()
     ACCENT = auto()
 
-class Spacing(StrEnum):
+class Spacing(LowercaseStrEnum):
     DEFAULT = auto()
     NONE = auto()
     SMALL = auto()
     MEDIUM = auto()
     LARGE = auto()
     EXTRA_LARGE = "extraLarge"
     PADDING = auto()
     
-class AssociatedInputs(StrEnum):
+class AssociatedInputs(LowercaseStrEnum):
     AUTO = auto()
     NONE = auto()
     
-class ActionStyle(StrEnum):
+class ActionStyle(LowercaseStrEnum):
     DEFAULT = auto()
     POSITIVE = auto()
     DESTRUCTIVE = auto()
     
-class ActionMode(StrEnum):
+class ActionMode(LowercaseStrEnum):
     PRIMARY = auto()
     SECONDARY = auto()
     
-class TextInputStyle(StrEnum):
+class TextInputStyle(LowercaseStrEnum):
     TEXT = auto()
     TEL = auto()
     URL = auto()
     EMAIL = auto()
     PASSWORD = auto()
     
-class ChoiceInputStyle(StrEnum):
+class ChoiceInputStyle(LowercaseStrEnum):
     COMPACT = auto()
     EXPANDED = auto()
     FILTERED = auto()
     
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(kw_only=True)
 class BackgroundImage:
```

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/containers.py` & `adaptive-cards-py-0.0.4/adaptive_cards/containers.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/elements.py` & `adaptive-cards-py-0.0.4/adaptive_cards/elements.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/inputs.py` & `adaptive-cards-py-0.0.4/adaptive_cards/inputs.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards/validation.py` & `adaptive-cards-py-0.0.4/adaptive_cards/validation.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/PKG-INFO` & `adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,14 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Homepage, https://github.com/dennis6p/adaptive-cards-py
 Keywords: bot,ui,adaptivecards,cards,adaptivecardsio,python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `adaptive-cards-py-0.0.3/adaptive_cards_py.egg-info/SOURCES.txt` & `adaptive-cards-py-0.0.4/adaptive_cards_py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 adaptive_cards/__init__.py
 adaptive_cards/actions.py
 adaptive_cards/card.py
 adaptive_cards/card_types.py
 adaptive_cards/containers.py
 adaptive_cards/elements.py
 adaptive_cards/inputs.py
-adaptive_cards/interface.py
 adaptive_cards/utils.py
 adaptive_cards/validation.py
 adaptive_cards_py.egg-info/PKG-INFO
 adaptive_cards_py.egg-info/SOURCES.txt
 adaptive_cards_py.egg-info/dependency_links.txt
 adaptive_cards_py.egg-info/requires.txt
 adaptive_cards_py.egg-info/top_level.txt
```

### Comparing `adaptive-cards-py-0.0.3/examples/simple_card/simple_card.jpg` & `adaptive-cards-py-0.0.4/examples/simple_card/simple_card.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/examples/simple_card/simple_card_2.jpg` & `adaptive-cards-py-0.0.4/examples/simple_card/simple_card_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.3/pyproject.toml` & `adaptive-cards-py-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive-cards-py"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python wrapper library for building beautiful adaptive cards"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["bot", "ui", "adaptivecards", "cards", "adaptivecardsio", "python"]
 dependencies = [
-    "dataclasses-json"
+    "dataclasses-json",
+    "StrEnum"
 ]
 requires-python = ">=3.10"
 
 [options]
-package_dir = ["adaptive_cards"]
+package_dir = ["adaptive_cards"]
+
+[project.urls]
+Homepage = "https://github.com/dennis6p/adaptive-cards-py"
```


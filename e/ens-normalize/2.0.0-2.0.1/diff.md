# Comparing `tmp/ens_normalize-2.0.0.tar.gz` & `tmp/ens_normalize-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ens_normalize-2.0.0.tar", max compression
+gzip compressed data, was "ens_normalize-2.0.1.tar", max compression
```

## Comparing `ens_normalize-2.0.0.tar` & `ens_normalize-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1110 2023-03-27 13:57:30.873201 ens_normalize-2.0.0/LICENSE
--rw-r--r--   0        0        0    13134 2023-03-27 13:57:30.873201 ens_normalize-2.0.0/README.md
--rw-r--r--   0        0        0      582 2023-03-27 13:57:30.873201 ens_normalize-2.0.0/ens_normalize/__init__.py
--rw-r--r--   0        0        0    34451 2023-03-27 13:57:30.873201 ens_normalize-2.0.0/ens_normalize/normalization.py
--rw-r--r--   0        0        0  4631174 2023-03-27 13:57:30.889201 ens_normalize-2.0.0/ens_normalize/spec.json
--rw-r--r--   0        0        0      676 2023-03-27 13:57:30.889201 ens_normalize-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    13924 1970-01-01 00:00:00.000000 ens_normalize-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/LICENSE
+-rw-r--r--   0        0        0    12777 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/README.md
+-rw-r--r--   0        0        0      582 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/ens_normalize/__init__.py
+-rw-r--r--   0        0        0    35437 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/ens_normalize/normalization.py
+-rw-r--r--   0        0        0  5153418 2023-04-27 15:53:15.777292 ens_normalize-2.0.1/ens_normalize/spec.pickle
+-rw-r--r--   0        0        0      678 2023-04-27 15:53:15.777292 ens_normalize-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13521 1970-01-01 00:00:00.000000 ens_normalize-2.0.1/PKG-INFO
```

### Comparing `ens_normalize-2.0.0/LICENSE` & `ens_normalize-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_normalize-2.0.0/README.md` & `ens_normalize-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: ens-normalize
+Version: 2.0.1
+Summary: Ethereum Name Service (ENS) Name Normalizer
+Home-page: https://github.com/namehash/ens-normalize-python
+License: MIT
+Author: Jakub Karbowski
+Author-email: jakub@namehash.io
+Maintainer: NameHash Team
+Maintainer-email: devops@namehash.io
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyunormalize (>=15.0.0,<16.0.0)
+Project-URL: Repository, https://github.com/namehash/ens-normalize-python
+Description-Content-Type: text/markdown
+
 # ENS Normalize Python
 
 ![Tests](https://github.com/namehash/ens-normalize-python/actions/workflows/python-app.yml/badge.svg?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/ens-normalize)
 ![Coverage](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/coverage_badge.svg)
 
 * Python implementation of the [ENS Name Normalization Standard](https://github.com/adraffy/ensip-norm/blob/main/draft.md).
@@ -212,15 +232,15 @@
 For fatal errors (not curable), it is challenging to communicate the normalization error as a problem with a specific substring.
 
 | `DisallowedNameErrorType` | General info |
 | ------------------------- | ------------ |
 | `EMPTY_NAME`   | The name is empty |
 | `NSM_REPEATED` | Contains a repeated non-spacing mark |
 | `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
-| `CONF_WHOLE` | Contains visually confusing characters that are disallowed |
+| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
 
 ## List of all `CurableError` types
 
 Curable errors contain additional information about the disallowed substring.
 
 | `CurableErrorType` | General info | Disallowed sequence info |
 | ------------------ | ------------ | ------------------------ |
@@ -230,15 +250,15 @@
 | `CM_START`    | Contains a combining mark in a disallowed position at the start of the label | A combining mark is disallowed at the start of a label |
 | `CM_EMOJI`    | Contains a combining mark in a disallowed position after an emoji | A combining mark is disallowed after an emoji |
 | `DISALLOWED`  | Contains a disallowed character | This character is disallowed |
 | `INVISIBLE`   | Contains a disallowed invisible character | This invisible character is disallowed |
 | `FENCED_LEADING`  | Contains a disallowed character at the start of a label | This character is disallowed at the start of a label |
 | `FENCED_MULTI`    | Contains a disallowed consecutive sequence of characters | Characters in this sequence cannot be placed next to each other |
 | `FENCED_TRAILING` | Contains a disallowed character at the end of a label | This character is disallowed at the end of a label |
-| `CONF_MIXED` | Contains visually confusing characters from different scripts that are disallowed | This character is disallowed because it is visually confusing with another character from a different script |
+| `CONF_MIXED` | Contains visually confusing characters from multiple scripts ({script1}/{script2}) | This character from the {script1} script is disallowed because it is visually confusing with another character from the {script2} script |
 
 ## List of all normalization transformations
 
 | `NormalizationTransformationType` | General info | Disallowed sequence info |
 | --------------------------------- | ------------ | ------------------------ |
 | `IGNORED`    | Contains disallowed "ignored" characters that have been removed | This character is ignored during normalization and has been automatically removed |
 | `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
@@ -261,20 +281,14 @@
 3. Run the updater:
 
     ```bash
     cd tools/updater
     npm start
     ```
 
-4. Update `NormalizationData.VERSION`:\
-   This library keeps cache files in `$HOME/.cache/ens_normalize` to speed up loading.
-   To make sure existing users regenerate their cache after a version update,
-   please increment the `NormalizationData.VERSION` constant in [normalization.py](/ens_normalize/normalization.py).
-   The first import of the new version will automatically regenerate the cache.
-
 ### Build and test
 
 Installs dependencies, runs validation tests and builds the wheel.
 
 1. Install requirements:
    * [Python](https://www.python.org)
    * [Poetry](https://python-poetry.org)
@@ -292,7 +306,8 @@
     ```
 
 4. Build Python wheel:
 
     ```bash
     poetry build
     ```
+
```

### Comparing `ens_normalize-2.0.0/ens_normalize/__init__.py` & `ens_normalize-2.0.1/ens_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `ens_normalize-2.0.0/ens_normalize/normalization.py` & `ens_normalize-2.0.1/ens_normalize/normalization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Callable, Dict, List, NamedTuple, Set, Optional, Tuple, Union, Iterable
 from enum import Enum
-import regex
+import re
 import json
 import os
 import pickle
-import pickletools
-from pyunormalize import NFC, NFD
+from pyunormalize import NFC, NFD, UNICODE_VERSION
+import warnings
 
 
-SPEC_PATH = os.path.join(os.path.dirname(__file__), 'spec.json')
+SPEC_PICKLE_PATH = os.path.join(os.path.dirname(__file__), 'spec.pickle')
 
 
 class ErrorTypeBase(Enum):
     def __new__(cls, *args):
         value = len(cls.__members__) + 1
         obj = object.__new__(cls)
         obj._value_ = value
@@ -55,15 +55,15 @@
 
     NSM_REPEATED = "Contains a repeated non-spacing mark"
 
     NSM_TOO_MANY = "Contains too many consecutive non-spacing marks"
 
     # CONFUSABLES ----------
 
-    CONF_WHOLE = "Contains visually confusing characters that are disallowed"
+    CONF_WHOLE = "Contains visually confusing characters from {script1} and {script2} scripts"
 
 
 class CurableErrorType(CurableErrorTypeBase):
     """
     The name is disallowed but a cure is available.
     """
 
@@ -103,16 +103,16 @@
                      "Characters in this sequence cannot be placed next to each other"
 
     FENCED_TRAILING = "Contains a disallowed character at the end of a label", \
                       "This character is disallowed at the end of a label"
 
     # CONFUSABLES ----------
 
-    CONF_MIXED = "Contains visually confusing characters from different scripts that are disallowed", \
-                 "This character is disallowed because it is visually confusing with another character from a different script"
+    CONF_MIXED = "Contains visually confusing characters from multiple scripts ({scripts})", \
+                 "This character{script1} is disallowed because it is visually confusing with another character{script2}"
 
 
 class NormalizationTransformationType(CurableErrorTypeBase):
     """
     The label is allowed but contains a sequence which has been automatically transformed into a normalized form.
     """
 
@@ -126,17 +126,18 @@
                 "This emoji has been automatically fixed to remove an invisible character"
 
     NFC       = "Contains a disallowed sequence that is not \"NFC normalized\" which has been replaced by an equivalent normalized sequence", \
                 "This sequence has been automatically normalized into NFC canonical form"
 
 
 class DisallowedNameError(Exception):
-    def __init__(self, type: DisallowedNameErrorType):
+    def __init__(self, type: DisallowedNameErrorType, meta: Dict[str, str] = {}):
         super().__init__(type.general_info)
         self.type = type
+        self.meta = meta
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(code="{self.type.code}")'
 
     def __str__(self) -> str:
         return self.general_info
 
@@ -148,24 +149,25 @@
         return self.type.code
 
     @property
     def general_info(self) -> str:
         """
         Information about the entire name.
         """
-        return self.type.general_info
+        return self.type.general_info.format(**self.meta)
 
 
 class CurableError(DisallowedNameError):
     def __init__(self,
                  type: CurableErrorType,
                  index: int,
                  disallowed: str,
-                 suggested: str):
-        super().__init__(type)
+                 suggested: str,
+                 meta: Dict[str, str] = {}):
+        super().__init__(type, meta)
         self.type = type
         self.index = index
         self.disallowed = disallowed
         self.suggested = suggested
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(code="{self.type.code}", index={self.index}, disallowed="{self.disallowed}", suggested="{self.suggested}")'
@@ -174,24 +176,26 @@
     def disallowed_sequence_info(self) -> str:
         """
         Information about the disallowed sequence.
         """
         return self.type.disallowed_sequence_info.format(
             disallowed=self.disallowed,
             suggested=self.suggested,
+            **self.meta,
         )
 
 
 class NormalizationTransformation(CurableError):
     def __init__(self,
                  type: NormalizationTransformationType,
                  index: int,
                  disallowed: str,
-                 suggested: str):
-        super().__init__(type, index, disallowed, suggested)
+                 suggested: str,
+                 meta: Dict[str, str] = {}):
+        super().__init__(type, index, disallowed, suggested, meta)
         self.type = type
 
 
 TY_VALID = 'valid'
 TY_MAPPED = 'mapped'
 TY_IGNORED = 'ignored'
 TY_DISALLOWED = 'disallowed'
@@ -318,18 +322,18 @@
 
     return emojis_out
 
 
 def create_emoji_regex_pattern(emojis: List[str]) -> str:
     # add all optional fe0f so that we can match emojis with or without it
     emojis = add_all_fe0f(emojis)
-    fe0f = regex.escape('\uFE0F')
+    fe0f = re.escape('\uFE0F')
     def make_emoji(emoji: str) -> str:
         # make FE0F optional
-        return regex.escape(emoji).replace(fe0f, f'{fe0f}?')
+        return re.escape(emoji).replace(fe0f, f'{fe0f}?')
     # sort to match the longest first
     return '|'.join(make_emoji(emoji) for emoji in sorted(emojis, key=len, reverse=True))
 
 
 def create_emoji_fe0f_lookup(emojis: List[str]) -> Dict[str, str]:
     """
     Create a lookup table for recreating FE0F emojis from non-FE0F emojis.
@@ -384,23 +388,19 @@
                 for i in range(len(v['M'][k])):
                     id = find_group_id(groups, v['M'][k][i])
                     assert id is not None
                     v['M'][k][i] = id
 
 
 class NormalizationData:
-    # Increment VERSION when the spec changes
-    # or if the code in this class changes.
-    # It will force the cache to be regenerated.
-    VERSION = 1
-
-    def __init__(self):
-        with open(SPEC_PATH) as f:
+    def __init__(self, spec_json_path: str):
+        with open(spec_json_path, encoding='utf-8') as f:
             spec = json.load(f)
 
+        self.unicode_version: str = spec['unicode']
         self.ignored: Set[int] = set(spec['ignored'])
         self.mapped: Dict[int, List[int]] = {cp_src: mapping for cp_src, mapping in spec['mapped']}
         self.cm: Set[int] = set(spec['cm'])
         self.emoji: List[List[int]] = spec['emoji']
         self.nfc_check: Set[int] = set(spec['nfc_check'])
         self.fenced: Dict[int, str] = {x[0]: x[1] for x in spec['fenced']}
         self.groups: List[Dict] = read_groups(spec['groups'])
@@ -409,40 +409,39 @@
         group_names_to_ids(self.groups, self.whole_map)
         self.nsm_max: int = spec['nsm_max']
         self.nsm: Set[int] = set(spec['nsm'])
 
         self.cm.remove(CP_FE0F)
 
         self.emoji_fe0f_lookup = create_emoji_fe0f_lookup([''.join(chr(cp) for cp in cps) for cps in self.emoji])
-        self.emoji_regex = regex.compile(create_emoji_regex_pattern([''.join(chr(cp) for cp in cps) for cps in self.emoji]))
+        self.emoji_regex = re.compile(create_emoji_regex_pattern([''.join(chr(cp) for cp in cps) for cps in self.emoji]))
+
 
-def load_normalization_data() -> NormalizationData:
+def load_normalization_data_pickle(spec_pickle_path: str) -> NormalizationData:
     """
-    Loads `NormalizationData` from cached pickle file if it exists, otherwise creates it.
-    Pickle is stored in `$HOME/.cache/ens_normalize/normalization_data.pkl`.
-    It contains a version number, so if the version changes, the pickle is recreated.
-    """
-    cache_dir = os.path.join(os.path.expanduser('~'), '.cache', 'ens_normalize')
-    os.makedirs(cache_dir, exist_ok=True)
-    cache_path = os.path.join(cache_dir, 'normalization_data.pkl')
-    if os.path.exists(cache_path):
-        with open(cache_path, 'rb') as f:
-            data: NormalizationData = pickle.load(f)
-            if data.VERSION == NormalizationData.VERSION:
-                return data
-    data = NormalizationData()
-    # Python >= 3.8 is required for protocol 5
-    buf = pickle.dumps(data, protocol=5)
-    buf = pickletools.optimize(buf)
-    with open(cache_path, 'wb') as f:
-        f.write(buf)
-    return data
+    Loads `NormalizationData` from a pickle file.
+    """
+    with open(spec_pickle_path, 'rb') as f:
+        return pickle.load(f)
+
+
+NORMALIZATION = load_normalization_data_pickle(SPEC_PICKLE_PATH)
+
+
+def check_spec_unicode_version():
+    if not NORMALIZATION.unicode_version.startswith(UNICODE_VERSION):
+        warnings.warn(
+            f'Unicode version mismatch: '
+            f'pyunormalize is using {UNICODE_VERSION}, '
+            f'but the ENS Normalization spec is for {NORMALIZATION.unicode_version}',
+            UnicodeWarning,
+        )
 
 
-NORMALIZATION = load_normalization_data()
+check_spec_unicode_version()
 
 
 def collapse_valid_tokens(tokens: List[Token]) -> List[Token]:
     """
     Combine cps from continuous valid tokens into single tokens.
     """
     out = []
@@ -629,18 +628,36 @@
     if e is not None:
         return e
     g = g[0]
     # pass is_greek up to the caller
     is_greek[0] = g['name'] == 'Greek'
     return (
         post_check_group(g, cps_no_fe0f, cps)
-        or post_check_whole(unique)
+        or post_check_whole(g, unique)
     )
 
 
+def meta_for_conf_mixed(g, cp):
+    s1 = [g['name'] for g in NORMALIZATION.groups if cp in g['V']]
+    s1 = s1[0] if s1 else None
+    s2 = g['name']
+    if s1 is not None:
+        return {
+            'scripts': f'{s1}/{s2}',
+            'script1': f' from the {s1} script',
+            'script2': f' from the {s2} script',
+        }
+    else:
+        return {
+            'scripts': f'{s2} plus other scripts',
+            'script1': '',
+            'script2': f' from the {s2} script',
+        }
+
+
 def determine_group(unique: Iterable[int], cps: List[int]) -> Tuple[Optional[List[Dict]], Optional[CurableError]]:
     groups = NORMALIZATION.groups
     for cp in unique:
         gs = [g for g in groups if cp in g['V']]
         if len(gs) == 0:
             if groups == NORMALIZATION.groups:
                 return None, CurableError(
@@ -651,14 +668,15 @@
                 )
             else:
                 return None, CurableError(
                     CurableErrorType.CONF_MIXED,
                     index=cps.index(cp),
                     disallowed=chr(cp),
                     suggested='',
+                    meta=meta_for_conf_mixed(groups[0], cp),
                 )
         groups = gs
         if len(groups) == 1:
             break
     return groups, None
 
 
@@ -667,14 +685,15 @@
     for cp in cps:
         if cp not in v:
             return CurableError(
                 CurableErrorType.CONF_MIXED,
                 index=input.index(cp),
                 disallowed=chr(cp),
                 suggested='',
+                meta=meta_for_conf_mixed(g, cp),
             )
     if m:
         decomposed = str2cps(NFD(cps2str(cps)))
         i = 1
         e = len(decomposed)
         while i < e:
             if decomposed[i] in NORMALIZATION.nsm:
@@ -686,15 +705,15 @@
                         if decomposed[k] == decomposed[j]:
                             return DisallowedNameError(DisallowedNameErrorType.NSM_REPEATED)
                     j += 1
                 i = j
             i += 1
 
 
-def post_check_whole(cps: Iterable[int]) -> Optional[DisallowedNameError]:
+def post_check_whole(group, cps: Iterable[int]) -> Optional[DisallowedNameError]:
     # Cannot report error index, operating on unique codepoints.
     # Not reporting disallowed sequence, see below.
     maker = None
     shared = []
     for cp in cps:
         whole = NORMALIZATION.whole_map.get(cp)
         if whole == 1:
@@ -709,15 +728,21 @@
                 return None
         else:
             shared.append(cp)
     if maker is not None:
         for g_ind in maker:
             g = NORMALIZATION.groups[g_ind]
             if all(cp in g['V'] for cp in shared):
-                return DisallowedNameError(DisallowedNameErrorType.CONF_WHOLE)
+                return DisallowedNameError(
+                    DisallowedNameErrorType.CONF_WHOLE,
+                    meta={
+                        'script1': group['name'],
+                        'script2': g['name'],
+                    },
+                )
 
 
 def post_check(name: str, label_is_greek: List[bool]) -> Optional[Union[DisallowedNameError, CurableError]]:
     # name has emojis replaced with a single FE0F
     e = post_check_empty(name)
     if e is not None:
         return e
@@ -1019,23 +1044,27 @@
     if res.error is not None:
         raise res.error
     return res.normalized
 
 
 def _ens_cure(text: str) -> Tuple[str, List[CurableError]]:
     cures = []
-    while True:
+    # Protect against infinite loops.
+    # The assumption is that n iterations are enough to cure the input (2n just in case).
+    # +1 is for the last iteration that should raise DisallowedNameError.
+    # All cures currently implemented remove a character so this assumption seems reasonable.
+    for _ in range(2 * len(text) + 1):
         try:
             return ens_normalize(text), cures
         except CurableError as e:
-            new_text = text[:e.index] + e.suggested + text[e.index + len(e.disallowed):]
-            # protect against infinite loops
-            assert new_text != text, 'ens_cure() entered an infinite loop'
-            text = new_text
+            text = text[:e.index] + e.suggested + text[e.index + len(e.disallowed):]
             cures.append(e)
+        # DisallowedNameError is not caught here because it is not curable
+    # this should never happen
+    raise Exception('ens_cure() exceeded max iterations. Please report this as a bug.')
 
 
 def ens_cure(text: str) -> str:
     """
     Apply ENS normalization to a string. If the result is not normalized then this function
     will try to make the input normalized by removing all disallowed characters.
```

### Comparing `ens_normalize-2.0.0/pyproject.toml` & `ens_normalize-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ens-normalize"
-version = "2.0.0"
+version = "2.0.1"
 description = "Ethereum Name Service (ENS) Name Normalizer"
 license = "MIT"
 authors = ["Jakub Karbowski <jakub@namehash.io>"]
 maintainers = ["NameHash Team <devops@namehash.io>"]
 homepage = "https://github.com/namehash/ens-normalize-python"
 repository = "https://github.com/namehash/ens-normalize-python"
 readme = "README.md"
 packages = [{include = "ens_normalize"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-regex = "^2022.10.31"
 pyunormalize = "^15.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ens_normalize-2.0.0/PKG-INFO` & `ens_normalize-2.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: ens-normalize
-Version: 2.0.0
-Summary: Ethereum Name Service (ENS) Name Normalizer
-Home-page: https://github.com/namehash/ens-normalize-python
-License: MIT
-Author: Jakub Karbowski
-Author-email: jakub@namehash.io
-Maintainer: NameHash Team
-Maintainer-email: devops@namehash.io
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyunormalize (>=15.0.0,<16.0.0)
-Requires-Dist: regex (>=2022.10.31,<2023.0.0)
-Project-URL: Repository, https://github.com/namehash/ens-normalize-python
-Description-Content-Type: text/markdown
-
 # ENS Normalize Python
 
 ![Tests](https://github.com/namehash/ens-normalize-python/actions/workflows/python-app.yml/badge.svg?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/ens-normalize)
 ![Coverage](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/coverage_badge.svg)
 
 * Python implementation of the [ENS Name Normalization Standard](https://github.com/adraffy/ensip-norm/blob/main/draft.md).
@@ -233,15 +212,15 @@
 For fatal errors (not curable), it is challenging to communicate the normalization error as a problem with a specific substring.
 
 | `DisallowedNameErrorType` | General info |
 | ------------------------- | ------------ |
 | `EMPTY_NAME`   | The name is empty |
 | `NSM_REPEATED` | Contains a repeated non-spacing mark |
 | `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
-| `CONF_WHOLE` | Contains visually confusing characters that are disallowed |
+| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
 
 ## List of all `CurableError` types
 
 Curable errors contain additional information about the disallowed substring.
 
 | `CurableErrorType` | General info | Disallowed sequence info |
 | ------------------ | ------------ | ------------------------ |
@@ -251,15 +230,15 @@
 | `CM_START`    | Contains a combining mark in a disallowed position at the start of the label | A combining mark is disallowed at the start of a label |
 | `CM_EMOJI`    | Contains a combining mark in a disallowed position after an emoji | A combining mark is disallowed after an emoji |
 | `DISALLOWED`  | Contains a disallowed character | This character is disallowed |
 | `INVISIBLE`   | Contains a disallowed invisible character | This invisible character is disallowed |
 | `FENCED_LEADING`  | Contains a disallowed character at the start of a label | This character is disallowed at the start of a label |
 | `FENCED_MULTI`    | Contains a disallowed consecutive sequence of characters | Characters in this sequence cannot be placed next to each other |
 | `FENCED_TRAILING` | Contains a disallowed character at the end of a label | This character is disallowed at the end of a label |
-| `CONF_MIXED` | Contains visually confusing characters from different scripts that are disallowed | This character is disallowed because it is visually confusing with another character from a different script |
+| `CONF_MIXED` | Contains visually confusing characters from multiple scripts ({script1}/{script2}) | This character from the {script1} script is disallowed because it is visually confusing with another character from the {script2} script |
 
 ## List of all normalization transformations
 
 | `NormalizationTransformationType` | General info | Disallowed sequence info |
 | --------------------------------- | ------------ | ------------------------ |
 | `IGNORED`    | Contains disallowed "ignored" characters that have been removed | This character is ignored during normalization and has been automatically removed |
 | `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
@@ -282,20 +261,14 @@
 3. Run the updater:
 
     ```bash
     cd tools/updater
     npm start
     ```
 
-4. Update `NormalizationData.VERSION`:\
-   This library keeps cache files in `$HOME/.cache/ens_normalize` to speed up loading.
-   To make sure existing users regenerate their cache after a version update,
-   please increment the `NormalizationData.VERSION` constant in [normalization.py](/ens_normalize/normalization.py).
-   The first import of the new version will automatically regenerate the cache.
-
 ### Build and test
 
 Installs dependencies, runs validation tests and builds the wheel.
 
 1. Install requirements:
    * [Python](https://www.python.org)
    * [Poetry](https://python-poetry.org)
@@ -313,8 +286,7 @@
     ```
 
 4. Build Python wheel:
 
     ```bash
     poetry build
     ```
-
```


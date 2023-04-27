# Comparing `tmp/fgo_api_types-2023.4.26.17.12.34.tar.gz` & `tmp/fgo_api_types-2023.4.26.6.49.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.26.17.12.34.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.26.6.49.58.tar", max compression
```

## Comparing `fgo_api_types-2023.4.26.17.12.34.tar` & `fgo_api_types-2023.4.26.6.49.58.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-26 17:11:53.981841 fgo_api_types-2023.4.26.17.12.34/LICENSE
--rw-r--r--   0        0        0      449 2023-04-26 17:11:53.981841 fgo_api_types-2023.4.26.17.12.34/README.md
--rw-r--r--   0        0        0        0 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/common.py
--rw-r--r--   0        0        0    37696 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/enums.py
--rw-r--r--   0        0        0   155885 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74299 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/nice.py
--rw-r--r--   0        0        0    49669 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18464 2023-04-26 17:12:34.782248 fgo_api_types-2023.4.26.17.12.34/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-26 17:12:35.106253 fgo_api_types-2023.4.26.17.12.34/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.26.17.12.34/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-26 06:49:31.888901 fgo_api_types-2023.4.26.6.49.58/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-26 06:49:31.888901 fgo_api_types-2023.4.26.6.49.58/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37431 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   155885 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74299 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    49669 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18464 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-26 06:49:59.281469 fgo_api_types-2023.4.26.6.49.58/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.26.6.49.58/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.26.17.12.34/LICENSE` & `fgo_api_types-2023.4.26.6.49.58/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/basic.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/common.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/enums.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,14 @@
     beastUnknown = "beastUnknown"
     unknown = "unknown"
     agarthaPenth = "agarthaPenth"
     cccFinaleEmiyaAlter = "cccFinaleEmiyaAlter"
     salemAbby = "salemAbby"
     uOlgaMarie = "uOlgaMarie"
     uOlgaMarieAlienGod = "uOlgaMarieAlienGod"
-    beast = "beast"
     atlasUnmappedClass = "atlasUnmappedClass"
     # OTHER = "OTHER"
     ALL = "ALL"
     # EXTRA = "EXTRA"
     # MIX = "MIX"
 
 
@@ -387,15 +386,14 @@
     26: SvtClass.beastIIIL,
     27: SvtClass.beastUnknown,  # LB 5.2 beast
     28: SvtClass.pretender,
     29: SvtClass.beastIV,
     30: SvtClass.beastILost,
     31: SvtClass.uOlgaMarieAlienGod,
     32: SvtClass.uOlgaMarie,
-    33: SvtClass.beast,
     97: SvtClass.unknown,
     # 98
     # 99
     # 100
     107: SvtClass.agarthaPenth,
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
@@ -947,17 +945,14 @@
     cardStrong = "cardStrong"
     servant = "servant"
     shadow = "shadow"
     chenGongNp = "chenGongNp"
     cantBeSacrificed = "cantBeSacrificed"
     gutsBlock = "gutsBlock"
     classBeastILost = "classBeastILost"
-    holdingHolyGrail = "holdingHolyGrail"
-    standardClassServant = "standardClassServant"
-    classBeast = "classBeast"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -980,15 +975,14 @@
     117: Trait.classForeigner,
     118: Trait.classBeastIIIL,
     119: Trait.classBeastUnknown,
     120: Trait.classPretender,
     121: Trait.classBeastIV,
     122: Trait.classBeastILost,
     123: Trait.classUOlgaMarie,
-    124: Trait.classBeast,
     200: Trait.attributeSky,
     201: Trait.attributeEarth,
     202: Trait.attributeHuman,
     203: Trait.attributeStar,
     204: Trait.attributeBeast,
     300: Trait.alignmentLawful,
     301: Trait.alignmentChaotic,
@@ -1121,16 +1115,14 @@
     2839: Trait.shinsengumiServant,
     2840: Trait.ryozanpaku,
     2847: Trait.levitating,
     2848: Trait.obstacleMaker,
     2849: Trait.defender,
     2850: Trait.hasGoddessMetamorphosis,
     2851: Trait.servantsWithSkyAttribute,
-    2857: Trait.holdingHolyGrail,
-    2858: Trait.standardClassServant,
     # 2xxx: CQ or Story quests buff
     3000: Trait.attackPhysical,  # Normal attack, including NP
     3001: Trait.attackProjectile,
     3002: Trait.attackMagical,
     3004: Trait.buffPositiveEffect,
     3005: Trait.buffNegativeEffect,  # mutually exclusive with 3004
     3006: Trait.buffIncreaseDamage,  # catch all damage: atk, np, powermod, ...
```

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/nice.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/nice.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/raw.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/fgo_api_types/search.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.26.17.12.34/pyproject.toml` & `fgo_api_types-2023.4.26.6.49.58/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.26.17.12.34"
+version = "2023.04.26.06.49.58"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.26.17.12.34/PKG-INFO` & `fgo_api_types-2023.4.26.6.49.58/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.26.17.12.34
+Version: 2023.4.26.6.49.58
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


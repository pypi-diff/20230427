# Comparing `tmp/driftpy-0.6.7.tar.gz` & `tmp/driftpy-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driftpy-0.6.7.tar", max compression
+gzip compressed data, was "driftpy-0.6.8.tar", max compression
```

## Comparing `driftpy-0.6.7.tar` & `driftpy-0.6.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1957 2022-11-04 13:38:23.916071 driftpy-0.6.7/README.md
--rw-r--r--   0        0        0      808 2022-11-04 13:38:23.920071 driftpy-0.6.7/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/__init__.py
--rw-r--r--   0        0        0    10951 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/_types.py
--rw-r--r--   0        0        0     2765 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/accounts.py
--rw-r--r--   0        0        0     2616 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/addresses.py
--rw-r--r--   0        0        0    17427 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/admin.py
--rw-r--r--   0        0        0    43903 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/clearing_house.py
--rw-r--r--   0        0        0    23577 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/clearing_house_user.py
--rw-r--r--   0        0        0       50 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/constants/__init__.py
--rw-r--r--   0        0        0      986 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/constants/banks.py
--rw-r--r--   0        0        0      768 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/constants/config.py
--rw-r--r--   0        0        0     7280 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/constants/markets.py
--rw-r--r--   0        0        0     3616 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/constants/numeric_constants.py
--rw-r--r--   0        0        0        0 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/__init__.py
--rw-r--r--   0        0        0   157112 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/clearing_house.json
--rw-r--r--   0        0        0   172558 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/drift.json
--rw-r--r--   0        0        0     2349 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/mock_usdc_faucet.json
--rw-r--r--   0        0        0     2277 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/pyth.json
--rw-r--r--   0        0        0     2776 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/idl/token_faucet.json
--rw-r--r--   0        0        0    12272 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/amm.py
--rw-r--r--   0        0        0     2158 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/funding.py
--rw-r--r--   0        0        0     6948 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/market.py
--rw-r--r--   0        0        0     3403 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/positions.py
--rw-r--r--   0        0        0    10423 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/repeg.py
--rw-r--r--   0        0        0    10072 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/trade.py
--rw-r--r--   0        0        0     4641 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/math/user.py
--rw-r--r--   0        0        0        0 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/py.typed
--rw-r--r--   0        0        0      328 2022-11-04 13:38:23.920071 driftpy-0.6.7/src/driftpy/sdk_types.py
--rw-r--r--   0        0        0     9408 2022-11-04 13:38:23.924071 driftpy-0.6.7/src/driftpy/setup/helpers.py
--rw-r--r--   0        0        0    17849 2022-11-04 13:38:23.924071 driftpy-0.6.7/src/driftpy/types.py
--rw-r--r--   0        0        0     2886 2022-11-04 13:38:45.350116 driftpy-0.6.7/setup.py
--rw-r--r--   0        0        0     2626 2022-11-04 13:38:45.350674 driftpy-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1957 2022-11-04 14:12:00.265651 driftpy-0.6.8/README.md
+-rw-r--r--   0        0        0      808 2022-11-04 14:12:00.265651 driftpy-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/__init__.py
+-rw-r--r--   0        0        0    10951 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/_types.py
+-rw-r--r--   0        0        0     2765 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/accounts.py
+-rw-r--r--   0        0        0     2616 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/addresses.py
+-rw-r--r--   0        0        0    17427 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/admin.py
+-rw-r--r--   0        0        0    43903 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/clearing_house.py
+-rw-r--r--   0        0        0    23577 2022-11-04 14:12:00.265651 driftpy-0.6.8/src/driftpy/clearing_house_user.py
+-rw-r--r--   0        0        0       50 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/constants/__init__.py
+-rw-r--r--   0        0        0      986 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/constants/banks.py
+-rw-r--r--   0        0        0      768 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/constants/config.py
+-rw-r--r--   0        0        0     7280 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/constants/markets.py
+-rw-r--r--   0        0        0     3616 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/constants/numeric_constants.py
+-rw-r--r--   0        0        0        0 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/__init__.py
+-rw-r--r--   0        0        0   157112 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/clearing_house.json
+-rw-r--r--   0        0        0   172536 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/drift.json
+-rw-r--r--   0        0        0     2349 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/mock_usdc_faucet.json
+-rw-r--r--   0        0        0     2277 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/pyth.json
+-rw-r--r--   0        0        0     2776 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/idl/token_faucet.json
+-rw-r--r--   0        0        0    12272 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/amm.py
+-rw-r--r--   0        0        0     2158 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/funding.py
+-rw-r--r--   0        0        0     6948 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/market.py
+-rw-r--r--   0        0        0     3403 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/positions.py
+-rw-r--r--   0        0        0    10423 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/repeg.py
+-rw-r--r--   0        0        0    10072 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/trade.py
+-rw-r--r--   0        0        0     4641 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/math/user.py
+-rw-r--r--   0        0        0        0 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/py.typed
+-rw-r--r--   0        0        0      328 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/sdk_types.py
+-rw-r--r--   0        0        0     9408 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/setup/helpers.py
+-rw-r--r--   0        0        0    17795 2022-11-04 14:12:00.269651 driftpy-0.6.8/src/driftpy/types.py
+-rw-r--r--   0        0        0     2886 2022-11-04 14:12:17.942118 driftpy-0.6.8/setup.py
+-rw-r--r--   0        0        0     2626 2022-11-04 14:12:17.942620 driftpy-0.6.8/PKG-INFO
```

### Comparing `driftpy-0.6.7/README.md` & `driftpy-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/pyproject.toml` & `driftpy-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "driftpy"
-version = "0.6.7"
+version = "0.6.8"
 description = "A Python client for the Drift DEX"
 authors = ["Kevin Heavey <kevinheavey123@gmail.com>", "Zane <zane@lunoho.company>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/drift-labs/driftpy"
 documentation = "https://drift-labs.github.io/driftpy/"
```

### Comparing `driftpy-0.6.7/src/driftpy/_types.py` & `driftpy-0.6.8/src/driftpy/_types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/accounts.py` & `driftpy-0.6.8/src/driftpy/accounts.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/addresses.py` & `driftpy-0.6.8/src/driftpy/addresses.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/admin.py` & `driftpy-0.6.8/src/driftpy/admin.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/clearing_house.py` & `driftpy-0.6.8/src/driftpy/clearing_house.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/clearing_house_user.py` & `driftpy-0.6.8/src/driftpy/clearing_house_user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/constants/banks.py` & `driftpy-0.6.8/src/driftpy/constants/banks.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/constants/config.py` & `driftpy-0.6.8/src/driftpy/constants/config.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/constants/markets.py` & `driftpy-0.6.8/src/driftpy/constants/markets.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/constants/numeric_constants.py` & `driftpy-0.6.8/src/driftpy/constants/numeric_constants.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/idl/clearing_house.json` & `driftpy-0.6.8/src/driftpy/idl/clearing_house.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/idl/drift.json` & `driftpy-0.6.8/src/driftpy/idl/drift.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992849024644261%*

 * *Differences: {"'errors'": "{insert: [(216, OrderedDict([('code', 6216), ('name', 'InvalidSpotPosition'), "*

 * *             "('msg', 'Invalid Spot Position')])), (217, OrderedDict([('code', 6217), ('name', "*

 * *             "'CantTransferBetweenSameUserAccount'), ('msg', 'Cant transfer between same user "*

 * *             "account')]))]}",*

 * * "'types'": "{13: {'type': {'fields': {delete: [3, 2]}}}, 14: {'type': {'fields': {0: {'type': "*

 * *            "'u64'}, 1: {'type': 'u64'}}}}}"}*

```diff
@@ -1876,14 +1876,24 @@
             "msg": "Invalid Sub Account Id",
             "name": "InvalidUserSubAccountId"
         },
         {
             "code": 6215,
             "msg": "Invalid Trigger Order Condition",
             "name": "InvalidTriggerOrderCondition"
+        },
+        {
+            "code": 6216,
+            "msg": "Invalid Spot Position",
+            "name": "InvalidSpotPosition"
+        },
+        {
+            "code": 6217,
+            "msg": "Cant transfer between same user account",
+            "name": "CantTransferBetweenSameUserAccount"
         }
     ],
     "events": [
         {
             "fields": [
                 {
                     "index": false,
@@ -7312,43 +7322,30 @@
                         }
                     },
                     {
                         "name": "validity",
                         "type": {
                             "defined": "ValidityGuardRails"
                         }
-                    },
-                    {
-                        "name": "useForLiquidations",
-                        "type": "bool"
-                    },
-                    {
-                        "name": "padding",
-                        "type": {
-                            "array": [
-                                "u8",
-                                7
-                            ]
-                        }
                     }
                 ],
                 "kind": "struct"
             }
         },
         {
             "name": "PriceDivergenceGuardRails",
             "type": {
                 "fields": [
                     {
                         "name": "markOracleDivergenceNumerator",
-                        "type": "u128"
+                        "type": "u64"
                     },
                     {
                         "name": "markOracleDivergenceDenominator",
-                        "type": "u128"
+                        "type": "u64"
                     }
                 ],
                 "kind": "struct"
             }
         },
         {
             "name": "ValidityGuardRails",
```

### Comparing `driftpy-0.6.7/src/driftpy/idl/mock_usdc_faucet.json` & `driftpy-0.6.8/src/driftpy/idl/mock_usdc_faucet.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/idl/pyth.json` & `driftpy-0.6.8/src/driftpy/idl/pyth.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/idl/token_faucet.json` & `driftpy-0.6.8/src/driftpy/idl/token_faucet.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/amm.py` & `driftpy-0.6.8/src/driftpy/math/amm.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/funding.py` & `driftpy-0.6.8/src/driftpy/math/funding.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/market.py` & `driftpy-0.6.8/src/driftpy/math/market.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/positions.py` & `driftpy-0.6.8/src/driftpy/math/positions.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/repeg.py` & `driftpy-0.6.8/src/driftpy/math/repeg.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/trade.py` & `driftpy-0.6.8/src/driftpy/math/trade.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/math/user.py` & `driftpy-0.6.8/src/driftpy/math/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/setup/helpers.py` & `driftpy-0.6.8/src/driftpy/setup/helpers.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.6.7/src/driftpy/types.py` & `driftpy-0.6.8/src/driftpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,14 @@
     confidence_interval_max_size: int
     too_volatile_ratio: int
  
 @dataclass
 class OracleGuardRails:
     price_divergence: PriceDivergenceGuardRails
     validity: ValidityGuardRails
-    use_for_liquidations: bool
-    padding: list[int]
  
 @dataclass
 class FeeTier:
     fee_numerator: int
     fee_denominator: int
     maker_rebate_numerator: int
     maker_rebate_denominator: int
```

### Comparing `driftpy-0.6.7/setup.py` & `driftpy-0.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['anchorpy==0.10.0',
  'requests>=2.28.1,<3.0.0',
  'solana>=0.25.0,<0.26.0',
  'types-requests>=2.28.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'driftpy',
-    'version': '0.6.7',
+    'version': '0.6.8',
     'description': 'A Python client for the Drift DEX',
     'long_description': '# DriftPy\n\n<div align="center">\n    <img src="https://camo.githubusercontent.com/d41b63c668d34e0ac5baba28a6fcff818da7b168752e511a605096dd9ba94039/68747470733a2f2f75706c6f6164732d73736c2e776562666c6f772e636f6d2f3631313538303033356164353962323034333765623032342f3631366639376134326635363337633435313764303139335f4c6f676f2532302831292532302831292e706e67" width="30%" height="30%">\n</div>\n\nDriftPy is the Python client for the [Drift](https://www.drift.trade/) protocol. It allows you to trade and fetch data from Drift using Python.\n\n[Read The Documentation](https://drift-labs.github.io/driftpy/)\n\n## Installation\n\n```\npip install driftpy\n```\n\nNote: requires Python >= 3.9.\n\n## Examples\n\n[Arbitrage Trading](https://github.com/0xbigz/driftpy-arb)\n\n[Querying and Visualization](https://gist.github.com/mcclurejt/b244d4ca8b0000ce5078ef8f60e937d9)\n\n## Development\n\n- `git submodule update --init --recursive`\n- cd protocol-v2 && yarn \n- cd sdk && yarn && yarn build && cd .. \n- anchor build \n- in deps/serum/dex run `cargo build-bpf`\n- update anchor IDL for v2 protocol on new re-builds (copy new idls to src/driftpy/idl/...json)\n- run python tests: `bash test.sh v2tests/test.py`\n\n### Development Setup\n\nIf you want to contribute to DriftPy, follow these steps to get set up:\n\n1. Install [poetry](https://python-poetry.org/docs/#installation)\n2. Install dev dependencies (in local env):\n```sh\npoetry install\n```\n\n### Testing\n\n1. `bash test.sh`\n\n### Building the docs\n\nRun `mkdocs serve` to build the docs and serve them locally.\n\n### Releasing a new version of the package\n\n1. Make sure CHANGELOG.md is updated.\n2. Run `bumpversion major|minor|patch` to update the version number locally and create a tagged commit.\n3. Run `git push origin <version_number>` to push the tag to GitHub.\n4. After merging your PR on GitHub, create a new release at https://github.com/drift-labs/driftpy/releases.\n   The CI process will upload a new version of the package to PyPI.\n',
     'author': 'Kevin Heavey',
     'author_email': 'kevinheavey123@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/drift-labs/driftpy',
```

### Comparing `driftpy-0.6.7/PKG-INFO` & `driftpy-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driftpy
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Python client for the Drift DEX
 Home-page: https://github.com/drift-labs/driftpy
 License: MIT
 Author: Kevin Heavey
 Author-email: kevinheavey123@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


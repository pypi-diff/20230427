# Comparing `tmp/algokit_utils-1.0.4b3-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.4b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31320 bytes, number of entries: 14
--rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+Zip file size: 31633 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     3667 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     3838 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+-rw-r--r--  2.0 unx     5019 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b3.dist-info/RECORD
-14 files, 120223 bytes uncompressed, 29366 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/RECORD
+14 files, 121578 bytes uncompressed, 29679 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.4b3.dist-info/LICENSE
+Filename: algokit_utils-1.0.4b4.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.4b3.dist-info/METADATA
+Filename: algokit_utils-1.0.4b4.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.4b3.dist-info/WHEEL
+Filename: algokit_utils-1.0.4b4.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.4b3.dist-info/RECORD
+Filename: algokit_utils-1.0.4b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -66,16 +66,19 @@
     OnCompleteCallParameters,
     OnCompleteCallParametersDict,
     TransactionResponse,
 )
 from algokit_utils.network_clients import (
     AlgoClientConfig,
     get_algod_client,
+    get_algonode_config,
+    get_default_localnet_config,
     get_indexer_client,
     get_kmd_client_from_algod_client,
+    get_purestake_config,
     is_localnet,
     is_sandbox,
 )
 
 __all__ = [
     "create_kmd_wallet_account",
     "get_account_from_mnemonic",
@@ -130,14 +133,17 @@
     "MethodHints",
     "LogicError",
     "ABITransactionResponse",
     "Account",
     "TransactionResponse",
     "AlgoClientConfig",
     "get_algod_client",
+    "get_algonode_config",
+    "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
+    "get_purestake_config",
     "is_localnet",
     "is_sandbox",
     "TransferParameters",
     "transfer",
 ]
```

## algokit_utils/network_clients.py

```diff
@@ -1,21 +1,25 @@
 import dataclasses
 import os
 import warnings
+from typing import Literal
 from urllib import parse
 
 from algosdk.kmd import KMDClient
 from algosdk.v2client.algod import AlgodClient
 from algosdk.v2client.indexer import IndexerClient
 
 __all__ = [
     "AlgoClientConfig",
     "get_algod_client",
+    "get_algonode_config",
+    "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
+    "get_purestake_config",
     "is_localnet",
     "is_sandbox",
 ]
 
 _PURE_STAKE_HOST = "purestake.io"
 
 
@@ -26,29 +30,55 @@
 
     server: str
     """URL for the service e.g. `http://localhost:4001` or `https://testnet-api.algonode.cloud`"""
     token: str
     """API Token to authenticate with the service"""
 
 
+def get_default_localnet_config(config: Literal["algod", "indexer", "kmd"]) -> AlgoClientConfig:
+    """Returns the client configuration to point to the default LocalNet"""
+    port = {"algod": 4001, "indexer": 8980, "kmd": 4002}[config]
+    return AlgoClientConfig(server=f"http://localhost:{port}", token="a" * 64)
+
+
+def get_algonode_config(
+    network: Literal["testnet", "mainnet"], config: Literal["algod", "indexer"], token: str
+) -> AlgoClientConfig:
+    client = "api" if config == "algod" else "idx"
+    return AlgoClientConfig(
+        server=f"https://{network}-{client}.algonode.cloud",
+        token=token,
+    )
+
+
+def get_purestake_config(
+    network: Literal["testnet", "mainnet"], config: Literal["algod", "indexer"], token: str
+) -> AlgoClientConfig:
+    client = "ps2" if config == "algod" else "idx2"
+    return AlgoClientConfig(
+        server=f"https://{network}-algorand.api.purestake.io/{client}",
+        token=token,
+    )
+
+
 def get_algod_client(config: AlgoClientConfig | None = None) -> AlgodClient:
     """Returns an {py:class}`algosdk.v2client.algod.AlgodClient` from `config` or environment
 
     If no configuration provided will use environment variables `ALGOD_SERVER`, `ALGOD_PORT` and `ALGOD_TOKEN`"""
     config = config or _get_config_from_environment("ALGOD")
-    headers = _get_headers(config)
+    headers = _get_headers(config, "X-Algo-API-Token")
     return AlgodClient(config.token, config.server, headers)
 
 
 def get_indexer_client(config: AlgoClientConfig | None = None) -> IndexerClient:
     """Returns an {py:class}`algosdk.v2client.indexer.IndexerClient` from `config` or environment.
 
     If no configuration provided will use environment variables `INDEXER_SERVER`, `INDEXER_PORT` and `INDEXER_TOKEN`"""
     config = config or _get_config_from_environment("INDEXER")
-    headers = _get_headers(config)
+    headers = _get_headers(config, "X-Indexer-API-Token")
     return IndexerClient(config.token, config.server, headers)  # type: ignore[no-untyped-call]
 
 
 def is_localnet(client: AlgodClient) -> bool:
     """Returns True if client genesis is `devnet-v1` or `sandnet-v1`"""
     params = client.suggested_params()
     return params.gen in ["devnet-v1", "sandnet-v1"]
@@ -91,9 +121,10 @@
 
 def _is_pure_stake_url(url: str) -> bool:
     parsed = parse.urlparse(url)
     host = parsed.netloc.split(":")[0].lower()
     return host.endswith(_PURE_STAKE_HOST)
 
 
-def _get_headers(config: AlgoClientConfig) -> dict[str, str] | None:
-    return {"X-API-TOKEN": config.token} if _is_pure_stake_url(config.server) else None
+def _get_headers(config: AlgoClientConfig, default_auth_header: str) -> dict[str, str] | None:
+    auth_header = "X-API-Key" if _is_pure_stake_url(config.server) else default_auth_header
+    return {auth_header: config.token}
```

## Comparing `algokit_utils-1.0.4b3.dist-info/LICENSE` & `algokit_utils-1.0.4b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.4b3.dist-info/METADATA` & `algokit_utils-1.0.4b4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.4b3
+Version: 1.0.4b4
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.0.4b3.dist-info/RECORD` & `algokit_utils-1.0.4b4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-algokit_utils/__init__.py,sha256=wZm8zcJh-bj3HlMpK-yoNJwzNX6NEKnWDPuD4JoRifA,3493
+algokit_utils/__init__.py,sha256=9dK3nmp6w9OgS_aEhGwpKp17v7G0IsD6N1Ru9Zfhzrg,3667
 algokit_utils/_transfer.py,sha256=MAu9lLMK_g9GB40X2pb5zzDDsrDkqge1Onx5_CDSwwg,3568
 algokit_utils/account.py,sha256=-OQn9mhKxZkgXhab_ugRlKt18LRvK6KxJkH5bhFb-6k,7709
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=Vg5K7xDSp7F8ImwT9FyboZDZFHeq_HeZgZyU26lvjE0,29956
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
 algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
-algokit_utils/network_clients.py,sha256=N4Xcp3xE2LUXtXIWuWUjQlPRhuGaDTW2gjjio_X45k8,3838
+algokit_utils/network_clients.py,sha256=OvPBtv79bMBPh_Pn0YgS1xkBVKuWl_nGLq42hskpokk,5019
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.4b3.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.4b3.dist-info/METADATA,sha256=t81g1kWZe6XgxOq10BCHf2uUntXwk7_2_B_ixhhKqZ8,2037
-algokit_utils-1.0.4b3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.4b3.dist-info/RECORD,,
+algokit_utils-1.0.4b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.0.4b4.dist-info/METADATA,sha256=NdxSdv2Q94ATnGCcsdsNyOkUo9S-1W-XUSR3EfkqNX8,2037
+algokit_utils-1.0.4b4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.0.4b4.dist-info/RECORD,,
```


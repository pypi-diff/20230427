# Comparing `tmp/ethconnect-1.0.3.tar.gz` & `tmp/ethconnect-1.0.4.tar.gz`

## Comparing `ethconnect-1.0.3.tar` & `ethconnect-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/Account.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/EllipticCurve.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/EthAccount.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/EthConnect.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/EthTransaction.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/Keyring.py
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/ZymbitEthKeyring.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/ZymbitKeyringManager.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ethconnect-1.0.3/src/ethconnect/__init__.py
--rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/ABI.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/bytecode.txt
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/test_eth_account.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/test_eth_connect.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/test_zymbit_eth_keyring.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 ethconnect-1.0.3/tests/test_zymbit_keyring_manager.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.0.3/.gitignore
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.0.3/LICENSE.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ethconnect-1.0.3/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ethconnect-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/Account.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/EllipticCurve.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/EthAccount.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/EthConnect.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/EthTransaction.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/Keyring.py
+-rw-r--r--   0        0        0    12149 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/ZymbitEthKeyring.py
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/ZymbitKeyringManager.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ethconnect-1.0.4/src/ethconnect/__init__.py
+-rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/ABI.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/bytecode.txt
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/test_eth_account.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/test_eth_connect.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/test_zymbit_eth_keyring.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 ethconnect-1.0.4/tests/test_zymbit_keyring_manager.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.0.4/.gitignore
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ethconnect-1.0.4/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ethconnect-1.0.4/PKG-INFO
```

### Comparing `ethconnect-1.0.3/src/ethconnect/EthAccount.py` & `ethconnect-1.0.4/src/ethconnect/EthAccount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['EthAccount']
 from Account import Account
 import zymkey
 import binascii
 from web3 import Web3
 import re
 
 class EthAccount(Account):
```

### Comparing `ethconnect-1.0.3/src/ethconnect/EthConnect.py` & `ethconnect-1.0.4/src/ethconnect/EthConnect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['EthConnect']
 from ZymbitEthKeyring import ZymbitEthKeyring
 from EthAccount import EthAccount
 from EthTransaction import EthTransaction, SignedEthTransaction
 import zymkey
 from web3 import Web3
 import binascii
 import rlp
```

### Comparing `ethconnect-1.0.3/src/ethconnect/EthTransaction.py` & `ethconnect-1.0.4/src/ethconnect/EthTransaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['EthTransaction', 'SignedEthTransaction']
 import rlp
 from rlp.sedes import binary, Binary, big_endian_int, BigEndianInt, List, CountableList, boolean
 
 access_list_sede_type = CountableList(List([Binary.fixed_length(20, allow_empty=False), CountableList(BigEndianInt(32)),]),)
 
 # Transaction EIP-1559 
 class EthTransaction(rlp.Serializable):
```

### Comparing `ethconnect-1.0.3/src/ethconnect/Keyring.py` & `ethconnect-1.0.4/src/ethconnect/Keyring.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['Keyring']
 from abc import ABC, abstractmethod
 from EllipticCurve import EllipticCurve
 from typing import Type
 from Account import Account
 import re
 
 class Keyring(ABC):
```

### Comparing `ethconnect-1.0.3/src/ethconnect/ZymbitEthKeyring.py` & `ethconnect-1.0.4/src/ethconnect/ZymbitEthKeyring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['ZymbitEthKeyring']
 from Keyring import Keyring
 from EthAccount import EthAccount
 from EllipticCurve import EllipticCurve
 from EthTransaction import EthTransaction, SignedEthTransaction
 import zymkey
 from web3 import Web3
 from Crypto.Hash import keccak, SHA256
```

### Comparing `ethconnect-1.0.3/src/ethconnect/ZymbitKeyringManager.py` & `ethconnect-1.0.4/src/ethconnect/ZymbitKeyringManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__all__ = ['ZymbitKeyringManager']
 from Keyring import Keyring
 from typing import Type
 from time import sleep
 import zymkey
 
 class ZymbitKeyringManager:
```

### Comparing `ethconnect-1.0.3/tests/ABI.json` & `ethconnect-1.0.4/tests/ABI.json`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/tests/bytecode.txt` & `ethconnect-1.0.4/tests/bytecode.txt`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/tests/test_eth_account.py` & `ethconnect-1.0.4/tests/test_eth_account.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/tests/test_eth_connect.py` & `ethconnect-1.0.4/tests/test_eth_connect.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/tests/test_zymbit_eth_keyring.py` & `ethconnect-1.0.4/tests/test_zymbit_eth_keyring.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/tests/test_zymbit_keyring_manager.py` & `ethconnect-1.0.4/tests/test_zymbit_keyring_manager.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/LICENSE.md` & `ethconnect-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/README.md` & `ethconnect-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.3/pyproject.toml` & `ethconnect-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ethconnect"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Shivaansh Kapoor", email="shiv@zymbit.com" },
 ]
 description = "ETH-Connect Python API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ethconnect-1.0.3/PKG-INFO` & `ethconnect-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethconnect
-Version: 1.0.3
+Version: 1.0.4
 Summary: ETH-Connect Python API
 Project-URL: Homepage, https://github.com/Zymbit-Wallet/ETH-Connect-PY
 Author-email: Shivaansh Kapoor <shiv@zymbit.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


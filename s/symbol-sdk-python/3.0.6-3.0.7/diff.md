# Comparing `tmp/symbol-sdk-python-3.0.6.tar.gz` & `tmp/symbol-sdk-python-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-sdk-python-3.0.6.tar", max compression
+gzip compressed data, was "symbol-sdk-python-3.0.7.tar", max compression
```

## Comparing `symbol-sdk-python-3.0.6.tar` & `symbol-sdk-python-3.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      353 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/README.md
--rw-r--r--   0        0        0      674 2023-04-14 14:31:04.281013 symbol-sdk-python-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     2508 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0        0        0     3728 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/ArrayHelpers.py
--rw-r--r--   0        0        0     1482 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/BaseValue.py
--rw-r--r--   0        0        0     1787 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/Bip32.py
--rw-r--r--   0        0        0      723 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/BlockchainSettings.py
--rw-r--r--   0        0        0      883 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/BufferReader.py
--rw-r--r--   0        0        0      639 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/BufferWriter.py
--rw-r--r--   0        0        0     1059 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/ByteArray.py
--rw-r--r--   0        0        0     2158 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/Cipher.py
--rw-r--r--   0        0        0     1233 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0        0        0     1844 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/CryptoTypes.py
--rw-r--r--   0        0        0     1848 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0        0        0     3368 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/Network.py
--rw-r--r--   0        0        0     1594 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/NetworkTimestamp.py
--rw-r--r--   0        0        0     1019 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0        0        0      397 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/Ordered.py
--rw-r--r--   0        0        0     1606 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0        0        0     1348 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/QrSignatureStorage.py
--rw-r--r--   0        0        0     1494 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/QrStorage.py
--rw-r--r--   0        0        0     4992 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0        0        0      593 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/SharedKey.py
--rw-r--r--   0        0        0     1809 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0        0        0      226 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/Transforms.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/external/__init__.py
--rw-r--r--   0        0        0     7833 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/external/ed25519.py
--rw-r--r--   0        0        0     2983 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/facade/BatchOperations.py
--rw-r--r--   0        0        0     2801 2023-04-14 13:59:56.977613 symbol-sdk-python-3.0.6/symbolchain/facade/NemFacade.py
--rw-r--r--   0        0        0     4940 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/facade/__init__.py
--rw-r--r--   0        0        0     2152 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/impl/CipherHelpers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/impl/__init__.py
--rw-r--r--   0        0        0   178806 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nc/__init__.py
--rw-r--r--   0        0        0     3712 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/KeyPair.py
--rw-r--r--   0        0        0     2374 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0        0        0     1746 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/Network.py
--rw-r--r--   0        0        0     1094 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/SharedKey.py
--rw-r--r--   0        0        0     3748 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/nem/__init__.py
--rw-r--r--   0        0        0      378 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/ripemd160.py
--rw-r--r--   0        0        0   477679 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/sc/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0        0        0     1506 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/KeyPair.py
--rw-r--r--   0        0        0     7243 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/Merkle.py
--rw-r--r--   0        0        0     2476 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0        0        0      567 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/Metadata.py
--rw-r--r--   0        0        0     2229 2023-04-14 13:59:56.981613 symbol-sdk-python-3.0.6/symbolchain/symbol/Network.py
--rw-r--r--   0        0        0      334 2023-04-14 13:59:56.985613 symbol-sdk-python-3.0.6/symbolchain/symbol/SharedKey.py
--rw-r--r--   0        0        0     3355 2023-04-14 13:59:56.985613 symbol-sdk-python-3.0.6/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0        0        0     1686 2023-04-14 13:59:56.985613 symbol-sdk-python-3.0.6/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0        0        0        0 2023-04-14 13:59:56.985613 symbol-sdk-python-3.0.6/symbolchain/symbol/__init__.py
--rw-r--r--   0        0        0     1361 2023-04-14 14:31:16.697944 symbol-sdk-python-3.0.6/setup.py
--rw-r--r--   0        0        0     1431 2023-04-14 14:31:16.698219 symbol-sdk-python-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4585 2023-04-27 18:15:06.272392 symbol-sdk-python-3.0.7/README.md
+-rw-r--r--   0        0        0      674 2023-04-27 18:44:29.145353 symbol-sdk-python-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2508 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0        0        0     3728 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ArrayHelpers.py
+-rw-r--r--   0        0        0     1482 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BaseValue.py
+-rw-r--r--   0        0        0     1787 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Bip32.py
+-rw-r--r--   0        0        0      723 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BlockchainSettings.py
+-rw-r--r--   0        0        0      883 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BufferReader.py
+-rw-r--r--   0        0        0      639 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BufferWriter.py
+-rw-r--r--   0        0        0     1059 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ByteArray.py
+-rw-r--r--   0        0        0     2158 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Cipher.py
+-rw-r--r--   0        0        0     1233 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0        0        0     1844 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/CryptoTypes.py
+-rw-r--r--   0        0        0     1848 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0        0        0     3368 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Network.py
+-rw-r--r--   0        0        0     1594 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0        0        0     1019 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0        0        0      397 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Ordered.py
+-rw-r--r--   0        0        0     1606 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0        0        0     1348 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0        0        0     1494 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/QrStorage.py
+-rw-r--r--   0        0        0     4992 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0        0        0      593 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/SharedKey.py
+-rw-r--r--   0        0        0     1809 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0        0        0      226 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Transforms.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/external/__init__.py
+-rw-r--r--   0        0        0     7833 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/external/ed25519.py
+-rw-r--r--   0        0        0     2983 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0        0        0     2801 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/NemFacade.py
+-rw-r--r--   0        0        0     4940 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/__init__.py
+-rw-r--r--   0        0        0     2152 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/impl/CipherHelpers.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/impl/__init__.py
+-rw-r--r--   0        0        0   178806 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nc/__init__.py
+-rw-r--r--   0        0        0     3712 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/KeyPair.py
+-rw-r--r--   0        0        0     2374 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0        0        0     1746 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/Network.py
+-rw-r--r--   0        0        0     1094 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/SharedKey.py
+-rw-r--r--   0        0        0     3748 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ripemd160.py
+-rw-r--r--   0        0        0   477679 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/sc/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0        0        0     1506 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0        0        0     7243 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Merkle.py
+-rw-r--r--   0        0        0     2476 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0        0        0      567 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Metadata.py
+-rw-r--r--   0        0        0     2229 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Network.py
+-rw-r--r--   0        0        0      334 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0        0        0     3355 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0        0        0     1686 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0        0        0        0 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/__init__.py
+-rw-r--r--   0        0        0     5609 2023-04-27 18:44:42.719073 symbol-sdk-python-3.0.7/setup.py
+-rw-r--r--   0        0        0     5567 2023-04-27 18:44:42.719560 symbol-sdk-python-3.0.7/PKG-INFO
```

### Comparing `symbol-sdk-python-3.0.6/pyproject.toml` & `symbol-sdk-python-3.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-sdk-python'
-version = '3.0.6'
+version = '3.0.7'
 description = 'Symbol SDK'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
 
@@ -14,15 +14,15 @@
 
 keywords = ['symbol', 'sdk', 'Symbol SDK']
 
 classifiers = ['Programming Language :: Python :: 3.7']
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cryptography = "40.0.1"
+cryptography = "40.0.2"
 mnemonic = "0.20"
 Pillow = "9.5.0"
 PyNaCl = "1.5.0"
 PyYAML = "6.0"
 pyzbar = "0.1.9"
 qrcode = "7.4.2"
 ripemd-hash = "1.0.0"
```

### Comparing `symbol-sdk-python-3.0.6/symbolchain/AccountDescriptorRepository.py` & `symbol-sdk-python-3.0.7/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/ArrayHelpers.py` & `symbol-sdk-python-3.0.7/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/BaseValue.py` & `symbol-sdk-python-3.0.7/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/Bip32.py` & `symbol-sdk-python-3.0.7/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/BlockchainSettings.py` & `symbol-sdk-python-3.0.7/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/BufferReader.py` & `symbol-sdk-python-3.0.7/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/BufferWriter.py` & `symbol-sdk-python-3.0.7/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/ByteArray.py` & `symbol-sdk-python-3.0.7/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/Cipher.py` & `symbol-sdk-python-3.0.7/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/CodeWordsEncoder.py` & `symbol-sdk-python-3.0.7/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/CryptoTypes.py` & `symbol-sdk-python-3.0.7/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/DiceMnemonicGenerator.py` & `symbol-sdk-python-3.0.7/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/Network.py` & `symbol-sdk-python-3.0.7/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/NetworkTimestamp.py` & `symbol-sdk-python-3.0.7/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/NodeDescriptorRepository.py` & `symbol-sdk-python-3.0.7/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/PrivateKeyStorage.py` & `symbol-sdk-python-3.0.7/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/QrSignatureStorage.py` & `symbol-sdk-python-3.0.7/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/QrStorage.py` & `symbol-sdk-python-3.0.7/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/RuleBasedTransactionFactory.py` & `symbol-sdk-python-3.0.7/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/SharedKey.py` & `symbol-sdk-python-3.0.7/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/TransactionDescriptorProcessor.py` & `symbol-sdk-python-3.0.7/symbolchain/TransactionDescriptorProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/external/ed25519.py` & `symbol-sdk-python-3.0.7/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/facade/BatchOperations.py` & `symbol-sdk-python-3.0.7/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/facade/NemFacade.py` & `symbol-sdk-python-3.0.7/symbolchain/facade/NemFacade.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/facade/SymbolFacade.py` & `symbol-sdk-python-3.0.7/symbolchain/facade/SymbolFacade.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/impl/CipherHelpers.py` & `symbol-sdk-python-3.0.7/symbolchain/impl/CipherHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nc/__init__.py` & `symbol-sdk-python-3.0.7/symbolchain/nc/__init__.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nem/KeyPair.py` & `symbol-sdk-python-3.0.7/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nem/MessageEncoder.py` & `symbol-sdk-python-3.0.7/symbolchain/nem/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nem/Network.py` & `symbol-sdk-python-3.0.7/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nem/SharedKey.py` & `symbol-sdk-python-3.0.7/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/nem/TransactionFactory.py` & `symbol-sdk-python-3.0.7/symbolchain/nem/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/sc/__init__.py` & `symbol-sdk-python-3.0.7/symbolchain/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/IdGenerator.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/IdGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/KeyPair.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/Merkle.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/Merkle.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/MessageEncoder.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/Metadata.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/Metadata.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/Network.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/TransactionFactory.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.6/symbolchain/symbol/VotingKeysGenerator.py` & `symbol-sdk-python-3.0.7/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*


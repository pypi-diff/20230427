# Comparing `tmp/trezor-0.9.0.tar.gz` & `tmp/trezor-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trezor-0.9.0.tar", last modified: Tue Feb  6 21:13:34 2018, max compression
+gzip compressed data, was "dist/trezor-0.9.1.tar", last modified: Mon Mar  5 18:15:07 2018, max compression
```

## Comparing `trezor-0.9.0.tar` & `trezor-0.9.1.tar`

### file list

```diff
@@ -1,252 +1,256 @@
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/bash_completion.d/
--rw-r--r--   0 stick     (1000) users      (100)      329 2016-11-05 20:45:28.000000 trezor-0.9.0/bash_completion.d/trezorctl.sh
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/
--rw-r--r--   0 stick     (1000) users      (100)      539 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/PKG-INFO
--rw-r--r--   0 stick     (1000) users      (100)    12082 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/SOURCES.txt
--rw-r--r--   0 stick     (1000) users      (100)        1 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/dependency_links.txt
--rw-r--r--   0 stick     (1000) users      (100)        1 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/not-zip-safe
--rw-r--r--   0 stick     (1000) users      (100)      123 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/requires.txt
--rw-r--r--   0 stick     (1000) users      (100)       10 2018-02-06 21:13:34.000000 trezor-0.9.0/trezor.egg-info/top_level.txt
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/messages/
--rw-r--r--   0 stick     (1000) users      (100)      237 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Address.py
--rw-r--r--   0 stick     (1000) users      (100)      226 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ApplyFlags.py
--rw-r--r--   0 stick     (1000) users      (100)      361 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ApplySettings.py
--rw-r--r--   0 stick     (1000) users      (100)      167 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/BackupDevice.py
--rw-r--r--   0 stick     (1000) users      (100)      164 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ButtonAck.py
--rw-r--r--   0 stick     (1000) users      (100)      267 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ButtonRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      204 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ButtonRequestType.py
--rw-r--r--   0 stick     (1000) users      (100)      161 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Cancel.py
--rw-r--r--   0 stick     (1000) users      (100)      222 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ChangePin.py
--rw-r--r--   0 stick     (1000) users      (100)      490 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CipherKeyValue.py
--rw-r--r--   0 stick     (1000) users      (100)      230 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CipheredKeyValue.py
--rw-r--r--   0 stick     (1000) users      (100)      167 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ClearSession.py
--rw-r--r--   0 stick     (1000) users      (100)      731 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CoinType.py
--rw-r--r--   0 stick     (1000) users      (100)      281 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CosiCommit.py
--rw-r--r--   0 stick     (1000) users      (100)      272 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CosiCommitment.py
--rw-r--r--   0 stick     (1000) users      (100)      375 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CosiSign.py
--rw-r--r--   0 stick     (1000) users      (100)      231 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/CosiSignature.py
--rw-r--r--   0 stick     (1000) users      (100)      244 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkDecision.py
--rw-r--r--   0 stick     (1000) users      (100)      237 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkFlashErase.py
--rw-r--r--   0 stick     (1000) users      (100)      173 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkGetState.py
--rw-r--r--   0 stick     (1000) users      (100)      309 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkLog.py
--rw-r--r--   0 stick     (1000) users      (100)      231 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkMemory.py
--rw-r--r--   0 stick     (1000) users      (100)      279 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkMemoryRead.py
--rw-r--r--   0 stick     (1000) users      (100)      315 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkMemoryWrite.py
--rw-r--r--   0 stick     (1000) users      (100)      673 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkState.py
--rw-r--r--   0 stick     (1000) users      (100)      169 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DebugLinkStop.py
--rw-r--r--   0 stick     (1000) users      (100)      363 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DecryptMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      274 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/DecryptedMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      234 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ECDHSessionKey.py
--rw-r--r--   0 stick     (1000) users      (100)      436 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EncryptMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      307 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EncryptedMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      235 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Entropy.py
--rw-r--r--   0 stick     (1000) users      (100)      226 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EntropyAck.py
--rw-r--r--   0 stick     (1000) users      (100)      169 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EntropyRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      374 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EstimateTxSize.py
--rw-r--r--   0 stick     (1000) users      (100)      243 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumAddress.py
--rw-r--r--   0 stick     (1000) users      (100)      296 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumGetAddress.py
--rw-r--r--   0 stick     (1000) users      (100)      282 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumMessageSignature.py
--rw-r--r--   0 stick     (1000) users      (100)      305 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumSignMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      583 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumSignTx.py
--rw-r--r--   0 stick     (1000) users      (100)      232 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumTxAck.py
--rw-r--r--   0 stick     (1000) users      (100)      373 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumTxRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      319 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/EthereumVerifyMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      263 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Failure.py
--rw-r--r--   0 stick     (1000) users      (100)      255 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/FailureType.py
--rw-r--r--   0 stick     (1000) users      (100)     1394 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Features.py
--rw-r--r--   0 stick     (1000) users      (100)      229 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/FirmwareErase.py
--rw-r--r--   0 stick     (1000) users      (100)      272 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/FirmwareRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      278 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/FirmwareUpload.py
--rw-r--r--   0 stick     (1000) users      (100)      529 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/GetAddress.py
--rw-r--r--   0 stick     (1000) users      (100)      373 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/GetECDHSessionKey.py
--rw-r--r--   0 stick     (1000) users      (100)      236 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/GetEntropy.py
--rw-r--r--   0 stick     (1000) users      (100)      166 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/GetFeatures.py
--rw-r--r--   0 stick     (1000) users      (100)      406 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/GetPublicKey.py
--rw-r--r--   0 stick     (1000) users      (100)      304 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/HDNodePathType.py
--rw-r--r--   0 stick     (1000) users      (100)      467 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/HDNodeType.py
--rw-r--r--   0 stick     (1000) users      (100)      410 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/IdentityType.py
--rw-r--r--   0 stick     (1000) users      (100)      164 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Initialize.py
--rw-r--r--   0 stick     (1000) users      (100)      121 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/InputScriptType.py
--rw-r--r--   0 stick     (1000) users      (100)      586 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/LoadDevice.py
--rw-r--r--   0 stick     (1000) users      (100)      276 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/MessageSignature.py
--rw-r--r--   0 stick     (1000) users      (100)     1576 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/MessageType.py
--rw-r--r--   0 stick     (1000) users      (100)      366 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/MultisigRedeemScriptType.py
--rw-r--r--   0 stick     (1000) users      (100)      240 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMAddress.py
--rw-r--r--   0 stick     (1000) users      (100)      364 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMAggregateModification.py
--rw-r--r--   0 stick     (1000) users      (100)      257 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMCosignatoryModification.py
--rw-r--r--   0 stick     (1000) users      (100)      376 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMDecryptMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      235 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMDecryptedMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      333 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMGetAddress.py
--rw-r--r--   0 stick     (1000) users      (100)      252 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMImportanceTransfer.py
--rw-r--r--   0 stick     (1000) users      (100)      101 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMImportanceTransferMode.py
--rw-r--r--   0 stick     (1000) users      (100)      102 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMModificationType.py
--rw-r--r--   0 stick     (1000) users      (100)      286 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMMosaic.py
--rw-r--r--   0 stick     (1000) users      (100)      347 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMMosaicCreation.py
--rw-r--r--   0 stick     (1000) users      (100)      839 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMMosaicDefinition.py
--rw-r--r--   0 stick     (1000) users      (100)       85 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMMosaicLevy.py
--rw-r--r--   0 stick     (1000) users      (100)      334 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMMosaicSupplyChange.py
--rw-r--r--   0 stick     (1000) users      (100)      332 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMProvisionNamespace.py
--rw-r--r--   0 stick     (1000) users      (100)     1047 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMSignTx.py
--rw-r--r--   0 stick     (1000) users      (100)      266 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMSignedTx.py
--rw-r--r--   0 stick     (1000) users      (100)       87 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMSupplyChangeType.py
--rw-r--r--   0 stick     (1000) users      (100)      433 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMTransactionCommon.py
--rw-r--r--   0 stick     (1000) users      (100)      413 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/NEMTransfer.py
--rw-r--r--   0 stick     (1000) users      (100)      146 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/OutputScriptType.py
--rw-r--r--   0 stick     (1000) users      (100)      246 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PassphraseAck.py
--rw-r--r--   0 stick     (1000) users      (100)      172 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PassphraseRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      238 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PinMatrixAck.py
--rw-r--r--   0 stick     (1000) users      (100)      231 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PinMatrixRequest.py
--rw-r--r--   0 stick     (1000) users      (100)       74 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PinMatrixRequestType.py
--rw-r--r--   0 stick     (1000) users      (100)      369 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Ping.py
--rw-r--r--   0 stick     (1000) users      (100)      307 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/PublicKey.py
--rw-r--r--   0 stick     (1000) users      (100)      611 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/RecoveryDevice.py
--rw-r--r--   0 stick     (1000) users      (100)       65 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/RecoveryDeviceType.py
--rw-r--r--   0 stick     (1000) users      (100)      102 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/RequestType.py
--rw-r--r--   0 stick     (1000) users      (100)      583 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/ResetDevice.py
--rw-r--r--   0 stick     (1000) users      (100)      224 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SelfTest.py
--rw-r--r--   0 stick     (1000) users      (100)      235 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SetU2FCounter.py
--rw-r--r--   0 stick     (1000) users      (100)      420 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SignIdentity.py
--rw-r--r--   0 stick     (1000) users      (100)      421 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SignMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      526 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SignTx.py
--rw-r--r--   0 stick     (1000) users      (100)      317 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SignedIdentity.py
--rw-r--r--   0 stick     (1000) users      (100)      657 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/SimpleSignTx.py
--rw-r--r--   0 stick     (1000) users      (100)      224 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/Success.py
--rw-r--r--   0 stick     (1000) users      (100)      773 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TransactionType.py
--rw-r--r--   0 stick     (1000) users      (100)      265 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxAck.py
--rw-r--r--   0 stick     (1000) users      (100)      757 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxInputType.py
--rw-r--r--   0 stick     (1000) users      (100)      331 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxOutputBinType.py
--rw-r--r--   0 stick     (1000) users      (100)      592 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxOutputType.py
--rw-r--r--   0 stick     (1000) users      (100)      452 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxRequest.py
--rw-r--r--   0 stick     (1000) users      (100)      358 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxRequestDetailsType.py
--rw-r--r--   0 stick     (1000) users      (100)      310 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxRequestSerializedType.py
--rw-r--r--   0 stick     (1000) users      (100)      224 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/TxSize.py
--rw-r--r--   0 stick     (1000) users      (100)      378 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/VerifyMessage.py
--rw-r--r--   0 stick     (1000) users      (100)      164 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/WipeDevice.py
--rw-r--r--   0 stick     (1000) users      (100)      234 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/WordAck.py
--rw-r--r--   0 stick     (1000) users      (100)      226 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/WordRequest.py
--rw-r--r--   0 stick     (1000) users      (100)       69 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/WordRequestType.py
--rw-r--r--   0 stick     (1000) users      (100)     3541 2018-02-06 15:25:24.000000 trezor-0.9.0/trezorlib/messages/__init__.py
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/qt/
--rw-r--r--   0 stick     (1000) users      (100)        0 2016-02-10 15:45:32.000000 trezor-0.9.0/trezorlib/qt/__init__.py
--rw-r--r--   0 stick     (1000) users      (100)     4569 2017-11-06 10:10:23.000000 trezor-0.9.0/trezorlib/qt/pinmatrix.py
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/tests/
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/tests/device_tests/
--rw-r--r--   0 stick     (1000) users      (100)        0 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/__init__.py
--rw-r--r--   0 stick     (1000) users      (100)     5858 2018-02-01 09:29:00.000000 trezor-0.9.0/trezorlib/tests/device_tests/common.py
--rw-r--r--   0 stick     (1000) users      (100)     1743 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_basic.py
--rw-r--r--   0 stick     (1000) users      (100)     2536 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_bip32_speed.py
--rw-r--r--   0 stick     (1000) users      (100)     3221 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_cosi.py
--rw-r--r--   0 stick     (1000) users      (100)     1778 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_debuglink.py
--rw-r--r--   0 stick     (1000) users      (100)     7351 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_applysettings.py
--rw-r--r--   0 stick     (1000) users      (100)     8554 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_changepin.py
--rw-r--r--   0 stick     (1000) users      (100)     4492 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_cipherkeyvalue.py
--rw-r--r--   0 stick     (1000) users      (100)     2578 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_clearsession.py
--rw-r--r--   0 stick     (1000) users      (100)     1552 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_getaddress.py
--rw-r--r--   0 stick     (1000) users      (100)     1681 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_signmessage.py
--rw-r--r--   0 stick     (1000) users      (100)    13706 2018-01-11 22:06:27.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_signtx.py
--rw-r--r--   0 stick     (1000) users      (100)     1711 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_verifymessage.py
--rw-r--r--   0 stick     (1000) users      (100)     4367 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress.py
--rw-r--r--   0 stick     (1000) users      (100)     2693 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_segwit.py
--rw-r--r--   0 stick     (1000) users      (100)     2958 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_segwit_native.py
--rw-r--r--   0 stick     (1000) users      (100)     2820 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_show.py
--rw-r--r--   0 stick     (1000) users      (100)     1679 2017-12-23 20:59:43.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getentropy.py
--rw-r--r--   0 stick     (1000) users      (100)     3382 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getpublickey.py
--rw-r--r--   0 stick     (1000) users      (100)     4663 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_loaddevice.py
--rw-r--r--   0 stick     (1000) users      (100)     1999 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_loaddevice_xprv.py
--rw-r--r--   0 stick     (1000) users      (100)     1216 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_nem_getaddress.py
--rw-r--r--   0 stick     (1000) users      (100)     3785 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_nem_signtx.py
--rw-r--r--   0 stick     (1000) users      (100)     2755 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ping.py
--rw-r--r--   0 stick     (1000) users      (100)     7040 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_recoverydevice.py
--rw-r--r--   0 stick     (1000) users      (100)     2625 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_recoverydevice_dryrun.py
--rw-r--r--   0 stick     (1000) users      (100)     7742 2017-12-23 21:00:37.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_resetdevice.py
--rw-r--r--   0 stick     (1000) users      (100)     4661 2017-12-28 15:20:22.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_resetdevice_skipbackup.py
--rw-r--r--   0 stick     (1000) users      (100)     4857 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signidentity.py
--rw-r--r--   0 stick     (1000) users      (100)     3339 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage.py
--rw-r--r--   0 stick     (1000) users      (100)     3667 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage_segwit.py
--rw-r--r--   0 stick     (1000) users      (100)     3692 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage_segwit_native.py
--rw-r--r--   0 stick     (1000) users      (100)    48113 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx.py
--rw-r--r--   0 stick     (1000) users      (100)    20863 2017-12-27 00:42:15.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_bcash.py
--rw-r--r--   0 stick     (1000) users      (100)    16705 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_decred.py
--rw-r--r--   0 stick     (1000) users      (100)    15287 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_segwit.py
--rw-r--r--   0 stick     (1000) users      (100)    33498 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_segwit_native.py
--rw-r--r--   0 stick     (1000) users      (100)     4368 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_zcash.py
--rw-r--r--   0 stick     (1000) users      (100)     7250 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage.py
--rw-r--r--   0 stick     (1000) users      (100)     4354 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage_segwit.py
--rw-r--r--   0 stick     (1000) users      (100)     4415 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage_segwit_native.py
--rw-r--r--   0 stick     (1000) users      (100)     1548 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_msg_wipedevice.py
--rw-r--r--   0 stick     (1000) users      (100)    16815 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_multisig.py
--rw-r--r--   0 stick     (1000) users      (100)    25476 2017-12-23 20:58:44.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_multisig_change.py
--rw-r--r--   0 stick     (1000) users      (100)     6310 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_op_return.py
--rw-r--r--   0 stick     (1000) users      (100)     5577 2017-12-23 20:49:39.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_protect_call.py
--rw-r--r--   0 stick     (1000) users      (100)     8523 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_protection_levels.py
--rw-r--r--   0 stick     (1000) users      (100)     3707 2017-12-23 20:41:23.000000 trezor-0.9.0/trezorlib/tests/device_tests/test_zerosig.py
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/tests/txcache/
--rw-r--r--   0 stick     (1000) users      (100)     1885 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c.json
--rw-r--r--   0 stick     (1000) users      (100)     2028 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_8b6db9b8ba24235d86b053ea2ccb484fc32b96f89c3c39f98d86f90db16076a0.json
--rw-r--r--   0 stick     (1000) users      (100)     1472 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_bc37c28dfb467d2ecb50261387bf752a3977d7e5337915071bb4151e6b711a78.json
--rw-r--r--   0 stick     (1000) users      (100)     2268 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_f68caf10df12d5b07a34601d88fa6856c6edcbf4d05ebef3486510ae1c293d5f.json
--rw-r--r--   0 stick     (1000) users      (100)     1743 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_1570416eb4302cf52979afd5e6909e37d8fdd874301f7cc87e547e509cb1caa6.json
--rw-r--r--   0 stick     (1000) users      (100)     2013 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_39a29e954977662ab3879c66fb251ef753e0912223a83d1dcb009111d28265e5.json
--rw-r--r--   0 stick     (1000) users      (100)     1878 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_50f6f1209ca92d7359564be803cb2c932cde7d370f7cee50fd1fad6790f6206d.json
--rw-r--r--   0 stick     (1000) users      (100)     2016 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_54aa5680dea781f45ebb536e53dffc526d68c0eb5c00547e323b2c32382dfba3.json
--rw-r--r--   0 stick     (1000) users      (100)     1998 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_58497a7757224d1ff1941488d23087071103e5bf855f4c1c44e5c8d9d82ca46e.json
--rw-r--r--   0 stick     (1000) users      (100)     1854 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_6189e3febb5a21cee8b725aa1ef04ffce7e609448446d3a8d6f483c634ef5315.json
--rw-r--r--   0 stick     (1000) users      (100)     1787 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_a6e2829d089cee47e481b1a753a53081b40738cc87e38f1d9b23ab57d9ad4396.json
--rw-r--r--   0 stick     (1000) users      (100)     1831 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c6091adf4c0c23982a35899a6e58ae11e703eacd7954f588ed4b9cdefc4dba52.json
--rw-r--r--   0 stick     (1000) users      (100)     2568 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb.json
--rw-r--r--   0 stick     (1000) users      (100)     2008 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c6be22d34946593bcad1d2b013e12f74159e69574ffea21581dad115572e031c.json
--rw-r--r--   0 stick     (1000) users      (100)     1789 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_d1d08ea63255af4ad16b098e9885a252632086fa6be53301521d05253ce8a73d.json
--rw-r--r--   0 stick     (1000) users      (100)     2411 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_d5f65ee80147b4bcc70b75e4bbf2d7382021b871bd8867ef8fa525ef50864882.json
--rw-r--r--   0 stick     (1000) users      (100)     1787 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_e4bc1ae5e5007a08f2b3926fe11c66612e8f73c6b00c69c7027213b84d259be3.json
--rw-r--r--   0 stick     (1000) users      (100)     1829 2017-12-23 12:48:21.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_16da185052740d85a630e79c140558215b64e26c500212b90e16b55d13ca06a8.json
--rw-r--r--   0 stick     (1000) users      (100)     1833 2017-12-23 12:48:21.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_3f7c395521d38387e7617565fe17628723ef6635a08537ad9c46cfb1619e4c3f.json
--rw-r--r--   0 stick     (1000) users      (100)     1509 2017-12-23 12:48:21.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_5e6e3500a333c53c02f523db5f1a9b17538a8850b4c2c24ecb9b7ba48059b970.json
--rw-r--r--   0 stick     (1000) users      (100)     1865 2017-12-23 12:48:21.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_ccf95b0fd220ef59ae2e5b17005a81e222758122682d522eff8ae1fcbc93bc74.json
--rw-r--r--   0 stick     (1000) users      (100)     1974 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_e16248f0b39a0a0c0e53d6f2f84c2a944f0d50e017a82701e8e02e46e979d5ed.json
--rw-r--r--   0 stick     (1000) users      (100)     1860 2017-12-23 12:48:21.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_f395ef3e72a831a766db15e7a38bc28025d4ee02234d68bdea2d8353b47a3113.json
--rw-r--r--   0 stick     (1000) users      (100)     1397 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_09144602765ce3dd8f4329445b20e3684e948709c5cdcaf12da3bb079c99448a.json
--rw-r--r--   0 stick     (1000) users      (100)     1792 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_16c6c8471b8db7a628f2b2bb86bfeefae1766463ce8692438c7fd3fce3f43ce5.json
--rw-r--r--   0 stick     (1000) users      (100)     1787 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_20912f98ea3ed849042efed0fdac8cb4fc301961c5988cba56902d8ffb61c337.json
--rw-r--r--   0 stick     (1000) users      (100)      980 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_31bc1c88ce6ae337a6b3057a16d5bad0b561ad1dfc047d0a7fbb8814668f91e5.json
--rw-r--r--   0 stick     (1000) users      (100)     1262 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_65b811d3eca0fe6915d9f2d77c86c5a7f19bf66b1b1253c2c51cb4ae5f0c017b.json
--rw-r--r--   0 stick     (1000) users      (100)     2515 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_6f90f3c7cbec2258b0971056ef3fe34128dbde30daa9c0639a898f9977299d54.json
--rw-r--r--   0 stick     (1000) users      (100)     1790 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_9c31922be756c06d02167656465c8dc83bb553bf386a3f478ae65b5c021002be.json
--rw-r--r--   0 stick     (1000) users      (100)     1726 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_b0946dc27ba308a749b11afecc2018980af18f79e89ad6b080b58220d856f739.json
--rw-r--r--   0 stick     (1000) users      (100)      933 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_c9348040bbc2024e12dcb4a0b4806b0398646b91acf314da028c3f03dd0179fc.json
--rw-r--r--   0 stick     (1000) users      (100)     1466 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d2dcdaf547ea7f57a713c607f15e883ddc4a98167ee2c43ed953c53cb5153e24.json
--rw-r--r--   0 stick     (1000) users      (100)      871 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d6da21677d7cca5f42fbc7631d062c9ae918a0254f7c6c22de8e8cb7fd5b8236.json
--rw-r--r--   0 stick     (1000) users      (100)     1792 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d80c34ee14143a8bf61125102b7ef594118a3796cad670fa8ee15080ae155318.json
--rw-r--r--   0 stick     (1000) users      (100)     1816 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd.json
--rw-r--r--   0 stick     (1000) users      (100)     1112 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_f41cbedd8becee05a830f418d13aa665125464547db5c7a6cd28f21639fe1228.json
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2018-02-06 21:13:34.000000 trezor-0.9.0/trezorlib/tests/unit_tests/
--rw-r--r--   0 stick     (1000) users      (100)        0 2017-12-19 13:18:15.000000 trezor-0.9.0/trezorlib/tests/unit_tests/__init__.py
--rw-r--r--   0 stick     (1000) users      (100)     1501 2017-12-19 14:54:04.000000 trezor-0.9.0/trezorlib/tests/unit_tests/test_ckd_public.py
--rw-r--r--   0 stick     (1000) users      (100)     2270 2017-12-19 14:53:54.000000 trezor-0.9.0/trezorlib/tests/unit_tests/test_tx_api.py
--rw-r--r--   0 stick     (1000) users      (100)       22 2018-02-06 21:12:12.000000 trezor-0.9.0/trezorlib/__init__.py
--rw-r--r--   0 stick     (1000) users      (100)     4770 2017-12-18 21:39:37.000000 trezor-0.9.0/trezorlib/ckd_public.py
--rw-r--r--   0 stick     (1000) users      (100)    44044 2018-02-06 20:37:38.000000 trezor-0.9.0/trezorlib/client.py
--rw-r--r--   0 stick     (1000) users      (100)      634 2017-12-27 00:39:17.000000 trezor-0.9.0/trezorlib/coins.py
--rw-r--r--   0 stick     (1000) users      (100)     4120 2017-12-17 01:25:39.000000 trezor-0.9.0/trezorlib/debuglink.py
--rw-r--r--   0 stick     (1000) users      (100)     2155 2018-02-04 10:53:05.000000 trezor-0.9.0/trezorlib/device.py
--rw-r--r--   0 stick     (1000) users      (100)     2658 2017-12-18 21:32:07.000000 trezor-0.9.0/trezorlib/ed25519cosi.py
--rw-r--r--   0 stick     (1000) users      (100)     3090 2017-12-18 21:32:00.000000 trezor-0.9.0/trezorlib/ed25519raw.py
--rw-r--r--   0 stick     (1000) users      (100)     2050 2017-12-17 02:21:38.000000 trezor-0.9.0/trezorlib/mapping.py
--rw-r--r--   0 stick     (1000) users      (100)     8340 2018-01-30 14:03:41.000000 trezor-0.9.0/trezorlib/protobuf.py
--rw-r--r--   0 stick     (1000) users      (100)     2687 2017-12-17 01:25:39.000000 trezor-0.9.0/trezorlib/protocol_v1.py
--rw-r--r--   0 stick     (1000) users      (100)     4571 2017-12-17 02:21:38.000000 trezor-0.9.0/trezorlib/protocol_v2.py
--rw-r--r--   0 stick     (1000) users      (100)     3454 2017-12-19 15:10:30.000000 trezor-0.9.0/trezorlib/tools.py
--rw-r--r--   0 stick     (1000) users      (100)     1459 2017-09-17 12:29:38.000000 trezor-0.9.0/trezorlib/transport.py
--rw-r--r--   0 stick     (1000) users      (100)     4020 2018-02-06 20:35:31.000000 trezor-0.9.0/trezorlib/transport_bridge.py
--rw-r--r--   0 stick     (1000) users      (100)     5833 2018-02-06 20:35:31.000000 trezor-0.9.0/trezorlib/transport_hid.py
--rw-r--r--   0 stick     (1000) users      (100)     3700 2018-02-06 20:35:31.000000 trezor-0.9.0/trezorlib/transport_udp.py
--rw-r--r--   0 stick     (1000) users      (100)     5999 2018-02-06 20:35:31.000000 trezor-0.9.0/trezorlib/transport_webusb.py
--rw-r--r--   0 stick     (1000) users      (100)     7221 2018-01-29 16:48:08.000000 trezor-0.9.0/trezorlib/tx_api.py
--rw-r--r--   0 stick     (1000) users      (100)     7651 2016-01-12 23:16:19.000000 trezor-0.9.0/COPYING
--rw-r--r--   0 stick     (1000) users      (100)       96 2017-12-19 13:18:15.000000 trezor-0.9.0/MANIFEST.in
--rw-r--r--   0 stick     (1000) users      (100)     1975 2018-02-02 19:00:39.000000 trezor-0.9.0/README.rst
--rwxr-xr-x   0 stick     (1000) users      (100)     1308 2018-02-02 19:00:39.000000 trezor-0.9.0/setup.py
--rwxr-xr-x   0 stick     (1000) users      (100)    28644 2018-02-02 19:00:39.000000 trezor-0.9.0/trezorctl
--rw-r--r--   0 stick     (1000) users      (100)      539 2018-02-06 21:13:34.000000 trezor-0.9.0/PKG-INFO
--rw-r--r--   0 stick     (1000) users      (100)       38 2018-02-06 21:13:34.000000 trezor-0.9.0/setup.cfg
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1975 2018-02-22 14:26:52.000000 trezor-0.9.1/README.rst
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       38 2018-03-05 18:15:07.000000 trezor-0.9.1/setup.cfg
+-rwxrwxr-x   0 matejcik  (1000) matejcik  (1000)    28959 2018-03-05 18:02:31.000000 trezor-0.9.1/trezorctl
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7651 2018-02-22 14:26:52.000000 trezor-0.9.1/COPYING
+-rwxrwxr-x   0 matejcik  (1000) matejcik  (1000)     1410 2018-03-05 18:07:23.000000 trezor-0.9.1/setup.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        1 2018-02-22 14:32:52.000000 trezor-0.9.1/trezor.egg-info/not-zip-safe
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       10 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/top_level.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        1 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/dependency_links.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    12341 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/SOURCES.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      134 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/requires.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      618 2018-03-05 18:15:07.000000 trezor-0.9.1/trezor.egg-info/PKG-INFO
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4770 2018-02-28 16:08:58.000000 trezor-0.9.1/trezorlib/ckd_public.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2658 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/ed25519cosi.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3454 2018-02-28 16:08:58.000000 trezor-0.9.1/trezorlib/tools.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7342 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tx_api.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/qt/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4569 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/qt/pinmatrix.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        0 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/qt/__init__.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2155 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/device.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    46202 2018-03-05 18:10:45.000000 trezor-0.9.1/trezorlib/client.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     5863 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/transport_hid.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4120 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/debuglink.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1459 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/transport.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4162 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/transport_bridge.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2050 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/mapping.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/messages/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      773 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TransactionType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      224 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Success.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      169 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EntropyRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       69 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/WordRequestType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       85 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMMosaicLevy.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      102 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMModificationType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      224 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxSize.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      224 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SelfTest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      173 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/PassphraseStateAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      611 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/RecoveryDevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      234 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ECDHSessionKey.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      237 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkFlashErase.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1394 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/Features.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      167 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/BackupDevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      378 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/VerifyMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      592 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxOutputType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      364 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMAggregateModification.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      267 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ButtonRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      673 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkState.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      230 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CipheredKeyValue.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      281 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CosiCommit.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      234 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/WordAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      420 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SignIdentity.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      222 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ChangePin.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      282 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumMessageSignature.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      272 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/FirmwareRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      272 2018-02-27 13:27:46.000000 trezor-0.9.1/trezorlib/messages/FailureType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      161 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Cancel.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      237 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Address.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      319 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumVerifyMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      421 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SignMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      257 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMCosignatoryModification.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      304 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/HDNodePathType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      226 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ApplyFlags.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      252 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMImportanceTransfer.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      406 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/GetPublicKey.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      101 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMImportanceTransferMode.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      452 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      310 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxRequestSerializedType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      529 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/GetAddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      266 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMSignedTx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      526 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SignTx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      332 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMProvisionNamespace.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      169 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkStop.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      307 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/PublicKey.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      583 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ResetDevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      333 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMGetAddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      231 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/PinMatrixRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      274 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DecryptedMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      436 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EncryptMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      164 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ButtonAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      231 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkMemory.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      839 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMMosaicDefinition.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      146 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/OutputScriptType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      265 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      263 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Failure.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      366 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/MultisigRedeemScriptType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      410 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/IdentityType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      373 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumTxRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      361 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ApplySettings.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      347 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMMosaicCreation.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      226 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/WordRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      413 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMTransfer.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      279 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkMemoryRead.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      307 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EncryptedMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      229 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/FirmwareErase.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      358 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxRequestDetailsType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      657 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SimpleSignTx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      731 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CoinType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      272 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CosiCommitment.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      467 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/HDNodeType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      305 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumSignMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      232 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumTxAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       87 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMSupplyChangeType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      375 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CosiSign.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      226 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EntropyAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      490 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CipherKeyValue.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3613 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/__init__.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      276 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/MessageSignature.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      373 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/GetECDHSessionKey.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      317 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SignedIdentity.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      173 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkGetState.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      164 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/WipeDevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      234 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/PassphraseAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      231 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/CosiSignature.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      286 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMMosaic.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      331 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxOutputBinType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      243 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumAddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      583 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumSignTx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      236 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/GetEntropy.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      363 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DecryptMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      240 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMAddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      166 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/GetFeatures.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      278 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/FirmwareUpload.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      334 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMMosaicSupplyChange.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      586 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/LoadDevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      296 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EthereumGetAddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      223 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Initialize.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      235 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/SetU2FCounter.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      167 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/ClearSession.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      369 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Ping.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      266 2018-02-27 13:27:46.000000 trezor-0.9.1/trezorlib/messages/ButtonRequestType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      376 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMDecryptMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      757 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/TxInputType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      374 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/EstimateTxSize.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       65 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/RecoveryDeviceType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      433 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMTransactionCommon.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      309 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkLog.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      121 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/InputScriptType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      238 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/PinMatrixAck.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       74 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/PinMatrixRequestType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      235 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/Entropy.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      244 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkDecision.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      234 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/PassphraseRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1047 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMSignTx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1628 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/MessageType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      236 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/messages/PassphraseStateRequest.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      102 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/RequestType.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      235 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/NEMDecryptedMessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      315 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/messages/DebugLinkMemoryWrite.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3470 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/transport_udp.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/tests/
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/tests/device_tests/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4857 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signidentity.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3785 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_nem_signtx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4394 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage_segwit_native.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4492 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_cipherkeyvalue.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3707 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_zerosig.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     8554 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_changepin.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2889 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getpublickey_curve.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2625 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_recoverydevice_dryrun.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1216 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_nem_getaddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     5526 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getpublickey.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7763 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_resetdevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    33498 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_segwit_native.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1702 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_signmessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4333 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage_segwit.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    55244 2018-02-27 13:27:46.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1679 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getentropy.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1747 2018-03-01 17:12:02.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_basic.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    16886 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_multisig.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    22543 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_bcash.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1999 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_loaddevice_xprv.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    25474 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_multisig_change.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1548 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_wipedevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1778 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_debuglink.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    15372 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_signtx.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    16705 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_decred.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3671 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage_segwit_native.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    15515 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_segwit.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2561 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_bip32_speed.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4342 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4684 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_loaddevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1732 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_verifymessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7250 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4368 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_zcash.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6080 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/tests/device_tests/common.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2578 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_clearsession.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3221 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_cosi.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2958 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_segwit_native.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7040 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_recoverydevice.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        0 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/__init__.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7650 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_applysettings.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     5577 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_protect_call.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6323 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_op_return.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2693 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_segwit.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3646 2018-03-05 17:56:59.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage_segwit.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1552 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_getaddress.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2799 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_show.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4661 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_resetdevice_skipbackup.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2755 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ping.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3339 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     8523 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/device_tests/test_protection_levels.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/tests/unit_tests/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1501 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/unit_tests/test_ckd_public.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2270 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/unit_tests/test_tx_api.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        0 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/unit_tests/__init__.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/trezorlib/tests/txcache/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1998 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_58497a7757224d1ff1941488d23087071103e5bf855f4c1c44e5c8d9d82ca46e.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1790 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_9c31922be756c06d02167656465c8dc83bb553bf386a3f478ae65b5c021002be.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1831 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c6091adf4c0c23982a35899a6e58ae11e703eacd7954f588ed4b9cdefc4dba52.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1787 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_20912f98ea3ed849042efed0fdac8cb4fc301961c5988cba56902d8ffb61c337.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2028 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_8b6db9b8ba24235d86b053ea2ccb484fc32b96f89c3c39f98d86f90db16076a0.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1865 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_ccf95b0fd220ef59ae2e5b17005a81e222758122682d522eff8ae1fcbc93bc74.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1829 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_16da185052740d85a630e79c140558215b64e26c500212b90e16b55d13ca06a8.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1789 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_d1d08ea63255af4ad16b098e9885a252632086fa6be53301521d05253ce8a73d.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      933 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_c9348040bbc2024e12dcb4a0b4806b0398646b91acf314da028c3f03dd0179fc.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1743 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_1570416eb4302cf52979afd5e6909e37d8fdd874301f7cc87e547e509cb1caa6.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1792 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_16c6c8471b8db7a628f2b2bb86bfeefae1766463ce8692438c7fd3fce3f43ce5.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1974 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_e16248f0b39a0a0c0e53d6f2f84c2a944f0d50e017a82701e8e02e46e979d5ed.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2016 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_54aa5680dea781f45ebb536e53dffc526d68c0eb5c00547e323b2c32382dfba3.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2568 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1833 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_3f7c395521d38387e7617565fe17628723ef6635a08537ad9c46cfb1619e4c3f.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1726 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_b0946dc27ba308a749b11afecc2018980af18f79e89ad6b080b58220d856f739.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    42348 2018-02-28 12:32:45.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_4a7b7e0403ae5607e473949cfa03f09f2cd8b0f404bf99ce10b7303d86280bf7.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2008 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c6be22d34946593bcad1d2b013e12f74159e69574ffea21581dad115572e031c.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2515 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_6f90f3c7cbec2258b0971056ef3fe34128dbde30daa9c0639a898f9977299d54.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2411 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_d5f65ee80147b4bcc70b75e4bbf2d7382021b871bd8867ef8fa525ef50864882.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      871 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d6da21677d7cca5f42fbc7631d062c9ae918a0254f7c6c22de8e8cb7fd5b8236.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2013 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_39a29e954977662ab3879c66fb251ef753e0912223a83d1dcb009111d28265e5.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1509 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_5e6e3500a333c53c02f523db5f1a9b17538a8850b4c2c24ecb9b7ba48059b970.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1397 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_09144602765ce3dd8f4329445b20e3684e948709c5cdcaf12da3bb079c99448a.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      980 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_31bc1c88ce6ae337a6b3057a16d5bad0b561ad1dfc047d0a7fbb8814668f91e5.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2268 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_f68caf10df12d5b07a34601d88fa6856c6edcbf4d05ebef3486510ae1c293d5f.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1787 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_a6e2829d089cee47e481b1a753a53081b40738cc87e38f1d9b23ab57d9ad4396.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1816 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1878 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_50f6f1209ca92d7359564be803cb2c932cde7d370f7cee50fd1fad6790f6206d.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1787 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_e4bc1ae5e5007a08f2b3926fe11c66612e8f73c6b00c69c7027213b84d259be3.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1112 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_f41cbedd8becee05a830f418d13aa665125464547db5c7a6cd28f21639fe1228.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1262 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_65b811d3eca0fe6915d9f2d77c86c5a7f19bf66b1b1253c2c51cb4ae5f0c017b.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1792 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d80c34ee14143a8bf61125102b7ef594118a3796cad670fa8ee15080ae155318.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1860 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_f395ef3e72a831a766db15e7a38bc28025d4ee02234d68bdea2d8353b47a3113.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1885 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1854 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_6189e3febb5a21cee8b725aa1ef04ffce7e609448446d3a8d6f483c634ef5315.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1472 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_bc37c28dfb467d2ecb50261387bf752a3977d7e5337915071bb4151e6b711a78.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1466 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d2dcdaf547ea7f57a713c607f15e883ddc4a98167ee2c43ed953c53cb5153e24.json
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     8340 2018-02-28 12:50:16.000000 trezor-0.9.1/trezorlib/protobuf.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     4571 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/protocol_v2.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       22 2018-03-05 18:14:01.000000 trezor-0.9.1/trezorlib/__init__.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     2687 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/protocol_v1.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3090 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/ed25519raw.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6029 2018-03-05 16:43:06.000000 trezor-0.9.1/trezorlib/transport_webusb.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      700 2018-02-22 14:26:52.000000 trezor-0.9.1/trezorlib/coins.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2018-03-05 18:15:07.000000 trezor-0.9.1/bash_completion.d/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      329 2018-02-22 14:26:52.000000 trezor-0.9.1/bash_completion.d/trezorctl.sh
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       96 2018-02-22 14:26:52.000000 trezor-0.9.1/MANIFEST.in
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      618 2018-03-05 18:15:07.000000 trezor-0.9.1/PKG-INFO
```

### Comparing `trezor-0.9.0/trezor.egg-info/PKG-INFO` & `trezor-0.9.1/trezor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: trezor
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python library for communicating with TREZOR Hardware Wallet
 Home-page: https://github.com/trezor/python-trezor
 Author: TREZOR
 Author-email: info@trezor.io
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.3
```

### Comparing `trezor-0.9.0/trezor.egg-info/SOURCES.txt` & `trezor-0.9.1/trezor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 trezorlib/messages/NEMSignedTx.py
 trezorlib/messages/NEMSupplyChangeType.py
 trezorlib/messages/NEMTransactionCommon.py
 trezorlib/messages/NEMTransfer.py
 trezorlib/messages/OutputScriptType.py
 trezorlib/messages/PassphraseAck.py
 trezorlib/messages/PassphraseRequest.py
+trezorlib/messages/PassphraseStateAck.py
+trezorlib/messages/PassphraseStateRequest.py
 trezorlib/messages/PinMatrixAck.py
 trezorlib/messages/PinMatrixRequest.py
 trezorlib/messages/PinMatrixRequestType.py
 trezorlib/messages/Ping.py
 trezorlib/messages/PublicKey.py
 trezorlib/messages/RecoveryDevice.py
 trezorlib/messages/RecoveryDeviceType.py
@@ -165,14 +167,15 @@
 trezorlib/tests/device_tests/test_msg_ethereum_verifymessage.py
 trezorlib/tests/device_tests/test_msg_getaddress.py
 trezorlib/tests/device_tests/test_msg_getaddress_segwit.py
 trezorlib/tests/device_tests/test_msg_getaddress_segwit_native.py
 trezorlib/tests/device_tests/test_msg_getaddress_show.py
 trezorlib/tests/device_tests/test_msg_getentropy.py
 trezorlib/tests/device_tests/test_msg_getpublickey.py
+trezorlib/tests/device_tests/test_msg_getpublickey_curve.py
 trezorlib/tests/device_tests/test_msg_loaddevice.py
 trezorlib/tests/device_tests/test_msg_loaddevice_xprv.py
 trezorlib/tests/device_tests/test_msg_nem_getaddress.py
 trezorlib/tests/device_tests/test_msg_nem_signtx.py
 trezorlib/tests/device_tests/test_msg_ping.py
 trezorlib/tests/device_tests/test_msg_recoverydevice.py
 trezorlib/tests/device_tests/test_msg_recoverydevice_dryrun.py
@@ -200,14 +203,15 @@
 trezorlib/tests/device_tests/test_zerosig.py
 trezorlib/tests/txcache/insight_bcash_tx_502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c.json
 trezorlib/tests/txcache/insight_bcash_tx_8b6db9b8ba24235d86b053ea2ccb484fc32b96f89c3c39f98d86f90db16076a0.json
 trezorlib/tests/txcache/insight_bcash_tx_bc37c28dfb467d2ecb50261387bf752a3977d7e5337915071bb4151e6b711a78.json
 trezorlib/tests/txcache/insight_bcash_tx_f68caf10df12d5b07a34601d88fa6856c6edcbf4d05ebef3486510ae1c293d5f.json
 trezorlib/tests/txcache/insight_bitcoin_tx_1570416eb4302cf52979afd5e6909e37d8fdd874301f7cc87e547e509cb1caa6.json
 trezorlib/tests/txcache/insight_bitcoin_tx_39a29e954977662ab3879c66fb251ef753e0912223a83d1dcb009111d28265e5.json
+trezorlib/tests/txcache/insight_bitcoin_tx_4a7b7e0403ae5607e473949cfa03f09f2cd8b0f404bf99ce10b7303d86280bf7.json
 trezorlib/tests/txcache/insight_bitcoin_tx_50f6f1209ca92d7359564be803cb2c932cde7d370f7cee50fd1fad6790f6206d.json
 trezorlib/tests/txcache/insight_bitcoin_tx_54aa5680dea781f45ebb536e53dffc526d68c0eb5c00547e323b2c32382dfba3.json
 trezorlib/tests/txcache/insight_bitcoin_tx_58497a7757224d1ff1941488d23087071103e5bf855f4c1c44e5c8d9d82ca46e.json
 trezorlib/tests/txcache/insight_bitcoin_tx_6189e3febb5a21cee8b725aa1ef04ffce7e609448446d3a8d6f483c634ef5315.json
 trezorlib/tests/txcache/insight_bitcoin_tx_a6e2829d089cee47e481b1a753a53081b40738cc87e38f1d9b23ab57d9ad4396.json
 trezorlib/tests/txcache/insight_bitcoin_tx_c6091adf4c0c23982a35899a6e58ae11e703eacd7954f588ed4b9cdefc4dba52.json
 trezorlib/tests/txcache/insight_bitcoin_tx_c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb.json
```

### Comparing `trezor-0.9.0/trezorlib/messages/CoinType.py` & `trezor-0.9.1/trezorlib/messages/CoinType.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/DebugLinkState.py` & `trezor-0.9.1/trezorlib/messages/DebugLinkState.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/EthereumSignTx.py` & `trezor-0.9.1/trezorlib/messages/EthereumSignTx.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/Features.py` & `trezor-0.9.1/trezorlib/messages/Features.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/GetAddress.py` & `trezor-0.9.1/trezorlib/messages/GetAddress.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/LoadDevice.py` & `trezor-0.9.1/trezorlib/messages/LoadDevice.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/MessageType.py` & `trezor-0.9.1/trezorlib/messages/MessageType.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 EntropyRequest = 35
 EntropyAck = 36
 SignMessage = 38
 VerifyMessage = 39
 MessageSignature = 40
 PassphraseRequest = 41
 PassphraseAck = 42
+PassphraseStateRequest = 77
+PassphraseStateAck = 78
 EstimateTxSize = 43
 TxSize = 44
 RecoveryDevice = 45
 WordRequest = 46
 WordAck = 47
 CipheredKeyValue = 48
 EncryptMessage = 49
```

### Comparing `trezor-0.9.0/trezorlib/messages/NEMMosaicDefinition.py` & `trezor-0.9.1/trezorlib/messages/NEMMosaicDefinition.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/NEMSignTx.py` & `trezor-0.9.1/trezorlib/messages/NEMSignTx.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/RecoveryDevice.py` & `trezor-0.9.1/trezorlib/messages/RecoveryDevice.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/ResetDevice.py` & `trezor-0.9.1/trezorlib/messages/ResetDevice.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/SignTx.py` & `trezor-0.9.1/trezorlib/messages/SignTx.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/SimpleSignTx.py` & `trezor-0.9.1/trezorlib/messages/SimpleSignTx.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/TransactionType.py` & `trezor-0.9.1/trezorlib/messages/TransactionType.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/TxInputType.py` & `trezor-0.9.1/trezorlib/messages/TxInputType.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/TxOutputType.py` & `trezor-0.9.1/trezorlib/messages/TxOutputType.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/messages/__init__.py` & `trezor-0.9.1/trezorlib/messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 from .NEMDecryptMessage import *
 from .NEMDecryptedMessage import *
 from .NEMGetAddress import *
 from .NEMSignTx import *
 from .NEMSignedTx import *
 from .PassphraseAck import *
 from .PassphraseRequest import *
+from .PassphraseStateAck import *
+from .PassphraseStateRequest import *
 from .PinMatrixAck import *
 from .PinMatrixRequest import *
 from .Ping import *
 from .PublicKey import *
 from .RecoveryDevice import *
 from .ResetDevice import *
 from .SelfTest import *
```

### Comparing `trezor-0.9.0/trezorlib/qt/pinmatrix.py` & `trezor-0.9.1/trezorlib/qt/pinmatrix.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/common.py` & `trezor-0.9.1/trezorlib/tests/device_tests/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         debuglink = devices[0].find_debug()
 
     elif PIPE_ENABLED and pipe_exists('/tmp/pipe.trezor.to'):
         wirelink = PipeTransport('/tmp/pipe.trezor', False)
         debuglink = PipeTransport('/tmp/pipe.trezor_debug', False)
 
     elif UDP_ENABLED:
-        wirelink = UdpTransport()
-        debuglink = UdpTransport()
+        wirelink = UdpTransport('127.0.0.1:21324')
+        debuglink = UdpTransport('127.0.0.1:21325')
 
     return wirelink, debuglink
 
 
 if HID_ENABLED and HidTransport.enumerate():
     print('Using TREZOR')
 elif WEBUSB_ENABLED and WebUsbTransport.enumerate():
@@ -127,14 +127,17 @@
 
     def setup_mnemonic_allallall(self):
         self.client.load_device_by_mnemonic(mnemonic=self.mnemonic_all, pin='', passphrase_protection=False, label='test', language='english')
 
     def setup_mnemonic_nopin_nopassphrase(self):
         self.client.load_device_by_mnemonic(mnemonic=self.mnemonic12, pin='', passphrase_protection=False, label='test', language='english')
 
+    def setup_mnemonic_nopin_passphrase(self):
+        self.client.load_device_by_mnemonic(mnemonic=self.mnemonic12, pin='', passphrase_protection=True, label='test', language='english')
+
     def setup_mnemonic_pin_nopassphrase(self):
         self.client.load_device_by_mnemonic(mnemonic=self.mnemonic12, pin=self.pin4, passphrase_protection=False, label='test', language='english')
 
     def setup_mnemonic_pin_passphrase(self):
         self.client.load_device_by_mnemonic(mnemonic=self.mnemonic12, pin=self.pin4, passphrase_protection=True, label='test', language='english')
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_basic.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 from trezorlib import messages
 
 
 class TestBasic(TrezorTest):
 
     def test_features(self):
-        features = self.client.call(messages.Initialize())
-        assert features == self.client.features
+        f0 = self.client.features
+        f1 = self.client.call(messages.Initialize())
+        assert f0 == f1
 
     def test_ping(self):
         ping = self.client.call(messages.Ping(message='ahoj!'))
         assert ping == messages.Success(message='ahoj!')
 
     def test_device_id_same(self):
         id1 = self.client.get_device_id()
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_bip32_speed.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_bip32_speed.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             start = time.time()
             self.client.get_address('Bitcoin', range(-depth, 0))
             delay = time.time() - start
             expected = (depth + 1) * 0.26
             print("DEPTH", depth, "EXPECTED DELAY", expected, "REAL DELAY", delay)
             assert delay <= expected
 
+    @pytest.mark.skip_t2
     def test_cache(self):
         self.setup_mnemonic_nopin_nopassphrase()
 
         start = time.time()
         for x in range(10):
             self.client.get_address('Bitcoin', [x, 2, 3, 4, 5, 6, 7, 8])
         nocache_time = time.time() - start
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_cosi.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_cosi.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_debuglink.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_debuglink.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_applysettings.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_applysettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,30 +17,32 @@
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 
 from trezorlib import messages as proto
 
 
-@pytest.mark.skip_t2
 class TestMsgApplysettings(TrezorTest):
 
     def test_apply_settings(self):
         self.setup_mnemonic_pin_passphrase()
         assert self.client.features.label == 'test'
 
         with self.client:
             self.client.set_expected_responses([proto.PinMatrixRequest(),
                                                 proto.ButtonRequest(),
                                                 proto.Success(),
                                                 proto.Features()])
+            if self.client.features.major_version >= 2:
+                self.client.expected_responses.pop(0)  # skip PinMatrixRequest
             self.client.apply_settings(label='new label')
 
         assert self.client.features.label == 'new label'
 
+    @pytest.mark.skip_t2
     def test_invalid_language(self):
         self.setup_mnemonic_pin_passphrase()
         assert self.client.features.language == 'english'
 
         with self.client:
             self.client.set_expected_responses([proto.PinMatrixRequest(),
                                                 proto.ButtonRequest(),
@@ -56,14 +58,16 @@
         assert self.client.features.passphrase_protection is False
 
         with self.client:
             self.client.set_expected_responses([proto.PinMatrixRequest(),
                                                 proto.ButtonRequest(),
                                                 proto.Success(),
                                                 proto.Features()])
+            if self.client.features.major_version >= 2:
+                self.client.expected_responses.pop(0)  # skip PinMatrixRequest
             self.client.apply_settings(use_passphrase=True)
 
         assert self.client.features.passphrase_protection is True
 
         with self.client:
             self.client.set_expected_responses([proto.ButtonRequest(),
                                                 proto.Success(),
@@ -76,14 +80,15 @@
             self.client.set_expected_responses([proto.ButtonRequest(),
                                                 proto.Success(),
                                                 proto.Features()])
             self.client.apply_settings(use_passphrase=True)
 
         assert self.client.features.passphrase_protection is True
 
+    @pytest.mark.skip_t2
     def test_apply_homescreen(self):
         self.setup_mnemonic_pin_passphrase()
 
         img = b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"\x00\x00\x00\x00\x04\x80\x00\x00\x00\x00\x00\x00\x00\x00\x04\x88\x02\x00\x00\x00\x02\x91\x00\x00\x00\x00\x00\x00\x80\x00\x00\x00\x00\x90@\x00\x11@\x00\x00\x00\x00\x00\x00\x08\x00\x10\x92\x12\x04\x00\x00\x05\x12D\x00\x00\x00\x00\x00 \x00\x00\x08\x00Q\x00\x00\x02\xc0\x00\x00\x00\x00\x00\x00\x00\x10\x02 \x01\x04J\x00)$\x00\x00\x00\x00\x80\x00\x00\x00\x00\x08\x10\xa1\x00\x00\x02\x81 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00\tP\x00\x00\x00\x00\x00\x00 \x00\x00\xa0\x00\xa0R \x12\x84\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\t\x08\x00\tP\x00\x00\x00\x00 \x00\x04 \x00\x80\x02\x00@\x02T\xc2 \x00\x00\x00\x00\x00\x00\x00\x10@\x00)\t@\n\xa0\x80\x00\x00\x00\x00\x00\x00\x00\x00\x10\x00\x80@\x14\xa9H\x04\x00\x00\x88@\x00\x00\x00\x00\x00\x02\x02$\x00\x15B@\x00\nP\x00\x00\x00\x00\x00\x80\x00\x00\x91\x01UP\x00\x00 \x02\x00\x00\x00\x00\x00\x00\x02\x08@ Z\xa5 \x00\x00\x80\x00\x00\x00\x00\x00\x00\x08\xa1%\x14*\xa0\x00\x00\x02\x08\x00\x00\x00\x00\x00\x00\x00\x00\x00@\xaa\x91 \x00\x05E\x80\x00\x00\x00\x00\x00\x02*T\x05-D\x00\x00\x05 @\x00\x00\x00\x00\x00%@\x80\x11V\xa0\x88\x00\x05@\xb0\x00\x00\x00\x00\x00\x818$\x04\xabD \x00\x06\xa1T\x00\x00\x00\x00\x02\x03\xb8\x01R\xd5\x01\x00\x00\x05AP\x00\x00\x00\x00\x08\xadT\x00\x05j\xa4@\x00\x87ah\x00\x00\x00\x00\x02\x8d\xb8\x08\x00.\x01\x00\x00\x02\xa5\xa8\x10\x00\x00\x00*\xc1\xec \n\xaa\x88 \x02@\xf6\xd0\x02\x00\x00\x00\x0bB\xb6\x14@U"\x80\x00\x01{`\x00\x00\x00\x00M\xa3\xf8 \x15*\x00\x00\x00\x10n\xc0\x04\x00\x00\x02\x06\xc2\xa8)\x00\x96\x84\x80\x00\x00\x1b\x00\x00\x80@\x10\x87\xa7\xf0\x84\x10\xaa\x10\x00\x00D\x00\x00\x02 \x00\x8a\x06\xfa\xe0P\n-\x02@\x00\x12\x00\x00\x00\x00\x10@\x83\xdf\xa0\x00\x08\xaa@\x00\x00\x01H\x00\x05H\x04\x12\x01\xf7\x81P\x02T\t\x00\x00\x00 \x00\x00\x84\x10\x00\x00z\x00@)* \x00\x00\x01\n\xa0\x02 \x05\n\x00\x00\x05\x10\x84\xa8\x84\x80\x00\x00@\x14\x00\x92\x10\x80\x00\x04\x11@\tT\x00\x00\x00\x00\n@\x00\x08\x84@$\x00H\x00\x12Q\x02\x00\x00\x00\x00\x90\x02A\x12\xa8\n\xaa\x92\x10\x04\xa8\x10@\x00\x00\x04\x04\x00\x04I\x00\x04\x14H\x80"R\x01\x00\x00\x00!@\x00\x00$\xa0EB\x80\x08\x95hH\x00\x00\x00\x84\x10 \x05Z\x00\x00(\x00\x02\x00\xa1\x01\x00\x00\x04\x00@\x82\x00\xadH*\x92P\x00\xaaP\x00\x00\x00\x00\x11\x02\x01*\xad\x01\x00\x01\x01"\x11D\x08\x00\x00\x10\x80 \x00\x81W\x80J\x94\x04\x08\xa5 !\x00\x00\x00\x02\x00B*\xae\xa1\x00\x80\x10\x01\x08\xa4\x00\x00\x00\x00\x00\x84\x00\t[@"HA\x04E\x00\x84\x00\x00\x00\x10\x00\x01J\xd5\x82\x90\x02\x00!\x02\xa2\x00\x00\x00\x00\x00\x00\x00\x05~\xa0\x00 \x10\n)\x00\x11\x00\x00\x00\x00\x00\x00!U\x80\xa8\x88\x82\x80\x01\x00\x00\x00\x00\x00\x00H@\x11\xaa\xc0\x82\x00 *\n\x00\x00\x00\x00\x00\x00\x00\x00\n\xabb@ \x04\x00! \x84\x00\x00\x00\x00\x02@\xa5\x15A$\x04\x81(\n\x00\x00\x00\x00\x00\x00 \x01\x10\x02\xe0\x91\x02\x00\x00\x04\x00\x00\x00\x00\x00\x00\x01 \xa9\tQH@\x91 P\x00\x00\x00\x00\x00\x00\x08\x00\x00\xa0T\xa5\x00@\x80\x08\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"\x00\x00\x00\x00\xa2\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00 T\xa0\t\x00\x08\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x00\x00@\x02\xa0\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00*\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x00\x00\x10\x00\x00\x10\x02\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\t\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00@\x04\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00@\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x00\x00\x08@\x10\x00\x00\x00\x00'
 
         with self.client:
             self.client.set_expected_responses([proto.PinMatrixRequest(),
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_changepin.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_changepin.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_cipherkeyvalue.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_cipherkeyvalue.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_clearsession.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_clearsession.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_getaddress.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_getaddress.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_signmessage.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_signmessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 
 
+@pytest.mark.skip_t2
 class TestMsgEthereumSignmessage(TrezorTest):
 
     def test_sign(self):
         self.setup_mnemonic_nopin_nopassphrase()
         sig = self.client.ethereum_sign_message([0], 'This is an example of a signed message.')
         assert hexlify(sig.address) == b'cb3864960e8db1a751212c580af27ee8867d688f'
         assert hexlify(sig.signature) == b'95b64a7b3aa492f0cc1668a24097004562cc2b4f0e755e3c0d60dd791b9f9e285f95b618258ff97036b8419d0a0dd1af3751c625b4d248ee6deff84eba21b8ee1c'
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_signtx.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_signtx.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,48 @@
 
 from .common import *
 from trezorlib import messages as proto
 
 
 class TestMsgEthereumSigntx(TrezorTest):
 
+    def test_ethereum_signtx_erc20_token(self):
+        self.setup_mnemonic_nopin_nopassphrase()
+
+        with self.client:
+            self.client.set_expected_responses([
+                proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
+                proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
+                proto.EthereumTxRequest(data_length=None),
+            ])
+
+            data = bytearray()
+            # method id signalizing `transfer(address _to, uint256 _value)` function
+            data.extend(unhexlify('a9059cbb'))
+            # 1st function argument (to - the receiver)
+            data.extend(unhexlify('000000000000000000000000574bbb36871ba6b78e27f4b4dcfb76ea0091880b'))
+            # 2nd function argument (value - amount to be transferred)
+            data.extend(unhexlify('0000000000000000000000000000000000000000000000000000000000000123'))
+
+            sig_v, sig_r, sig_s = self.client.ethereum_sign_tx(
+                n=[0, 0],
+                nonce=0,
+                gas_price=20,
+                gas_limit=20,
+                # ALTS token address
+                to=b'\x63\x8a\xc1\x49\xea\x8e\xf9\xa1\x28\x6c\x41\xb9\x77\x01\x7a\xa7\x35\x9e\x6c\xfa',
+                chain_id=1,
+                # value needs to be 0, token value is set in the contract (data)
+                value=0,
+                data=data)
+
+            # taken from T1 might not be 100% correct but still better than nothing
+            assert hexlify(sig_r) == b'28bf1b621be9a85d2905fa36511dfbd52ec4b67ba4ad6cb2bd08753c72b93b77'
+            assert hexlify(sig_s) == b'2fa605244f80a56cb438df55eb9835489288ec2c0ac0280ada2ccaccfe2b7e38'
+
     def test_ethereum_signtx_nodata(self):
         self.setup_mnemonic_nopin_nopassphrase()
 
         with self.client:
             self.client.set_expected_responses([
                 proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
                 proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ethereum_verifymessage.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ethereum_verifymessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 
 
+@pytest.mark.skip_t2
 class TestMsgEthereumVerifymessage(TrezorTest):
 
     def test_verify(self):
         self.setup_mnemonic_nopin_nopassphrase()
         res = self.client.ethereum_verify_message(
             unhexlify('cb3864960e8db1a751212c580af27ee8867d688f'),
             unhexlify('95b64a7b3aa492f0cc1668a24097004562cc2b4f0e755e3c0d60dd791b9f9e285f95b618258ff97036b8419d0a0dd1af3751c625b4d248ee6deff84eba21b8ee1c'),
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     def test_bch(self):
         self.setup_mnemonic_allallall()
         assert self.client.get_address('Bcash', self.client.expand_path("44'/145'/0'/0/0")) == '1MH9KKcvdCTY44xVDC2k3fjBbX5Cz29N1q'
         assert self.client.get_address('Bcash', self.client.expand_path("44'/145'/0'/0/1")) == '1LRspCZNFJcbuNKQkXgHMDucctFRQya5a3'
         assert self.client.get_address('Bcash', self.client.expand_path("44'/145'/0'/1/0")) == '1HADRPJpgqBzThepERpVXNi6qRgiLQRNoE'
 
-    @pytest.mark.skip_t2
     def test_bch_multisig(self):
         self.setup_mnemonic_allallall()
         xpubs = []
         for n in map(lambda index: self.client.get_public_node(self.client.expand_path("44'/145'/" + str(index) + "'")), range(1, 4)):
             xpubs.append(n.xpub)
 
         def getmultisig(chain, nr, signatures=[b'', b'', b''], xpubs=xpubs):
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_segwit.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_segwit.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_segwit_native.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_segwit_native.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getaddress_show.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getaddress_show.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 import trezorlib.ckd_public as bip32
 from trezorlib import messages as proto
 
 
-@pytest.mark.skip_t2
 class TestMsgGetaddressShow(TrezorTest):
 
     def test_show(self):
         self.setup_mnemonic_nopin_nopassphrase()
         assert self.client.get_address('Bitcoin', [1], show_display=True) == '1CK7SJdcb8z9HuvVft3D91HLpLC6KSsGb'
         assert self.client.get_address('Bitcoin', [2], show_display=True) == '15AeAhtNJNKyowK8qPHwgpXkhsokzLtUpG'
         assert self.client.get_address('Bitcoin', [3], show_display=True) == '1CmzyJp9w3NafXMSEFH4SLYUPAVCSUrrJ5'
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_getentropy.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_getentropy.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_loaddevice.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_loaddevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 
 
+@pytest.mark.skip_t2
 class TestDeviceLoad(TrezorTest):
     def test_load_device_1(self):
         self.setup_mnemonic_nopin_nopassphrase()
 
         mnemonic = self.client.debug.read_mnemonic()
         assert mnemonic == self.mnemonic12
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_loaddevice_xprv.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_loaddevice_xprv.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_nem_getaddress.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_nem_getaddress.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_nem_signtx.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_nem_signtx.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_ping.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_ping.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_recoverydevice.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_recoverydevice.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_recoverydevice_dryrun.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_recoverydevice_dryrun.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_resetdevice.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_resetdevice.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .common import *
 
 from trezorlib import messages as proto
 from mnemonic import Mnemonic
 
 
+@pytest.mark.skip_t2
 class TestMsgResetDevice(TrezorTest):
 
     def test_reset_device(self):
 
         # No PIN, no passphrase
         external_entropy = b'zlutoucky kun upel divoke ody' * 2
         strength = 128
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_resetdevice_skipbackup.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_resetdevice_skipbackup.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signidentity.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signidentity.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage_segwit.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage_segwit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 from trezorlib import messages as proto
 
 
-@pytest.mark.skip_t2
 class TestMsgSignmessageSegwit(TrezorTest):
 
     def test_sign(self):
         self.setup_mnemonic_nopin_nopassphrase()
         sig = self.client.sign_message('Bitcoin', [0], "This is an example of a signed message.", script_type=proto.InputScriptType.SPENDP2SHWITNESS)
         assert sig.address == '3CwYaeWxhpXXiHue3ciQez1DLaTEAXcKa1'
         assert hexlify(sig.signature) == b'249e23edf0e4e47ff1dec27f32cd78c50e74ef018ee8a6adf35ae17c7a9b0dd96f48b493fd7dbab03efb6f439c6383c9523b3bbc5f1a7d158a6af90ab154e9be80'
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signmessage_segwit_native.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signmessage_segwit_native.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 from trezorlib import messages as proto
 
 
-@pytest.mark.skip_t2
 class TestMsgSignmessageSegwitNative(TrezorTest):
 
     def test_sign(self):
         self.setup_mnemonic_nopin_nopassphrase()
         sig = self.client.sign_message('Bitcoin', [0], "This is an example of a signed message.", script_type=proto.InputScriptType.SPENDWITNESS)
         assert sig.address == 'bc1qyjjkmdpu7metqt5r36jf872a34syws33s82q2j'
         assert hexlify(sig.signature) == b'289e23edf0e4e47ff1dec27f32cd78c50e74ef018ee8a6adf35ae17c7a9b0dd96f48b493fd7dbab03efb6f439c6383c9523b3bbc5f1a7d158a6af90ab154e9be80'
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx.py`

 * *Files 10% similar despite different names*

```diff
@@ -600,30 +600,38 @@
 
             if req.details.tx_hash is not None:
                 return msg
 
             if req.details.request_index != 1:
                 return msg
 
+            if req.request_type != proto.RequestType.TXOUTPUT:
+                return msg
+
             if not run_attack:
                 run_attack = True
                 return msg
 
             msg.outputs[0].amount = 9999999  # Sign output with another amount
             return msg
 
         # Test if the transaction can be signed normally
         (_, serialized_tx) = self.client.sign_tx('Bitcoin', [inp1, inp2], [out1, out2])
 
         # Accepted by network: tx c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb
         assert hexlify(serialized_tx) == b'01000000021c032e5715d1da8115a2fe4f57699e15742fe113b0d2d1ca3b594649d322bec6010000006b483045022100f773c403b2f85a5c1d6c9c4ad69c43de66930fff4b1bc818eb257af98305546a0220443bde4be439f276a6ce793664b463580e210ec6c9255d68354449ac0443c76501210338d78612e990f2eea0c426b5e48a8db70b9d7ed66282b3b26511e0b1c75515a6ffffffff6ea42cd8d9c8e5441c4c5f85bfe50311078730d2881494f11f4d2257777a4958010000006b48304502210090cff1c1911e771605358a8cddd5ae94c7b60cc96e50275908d9bf9d6367c79f02202bfa72e10260a146abd59d0526e1335bacfbb2b4401780e9e3a7441b0480c8da0121038caebd6f753bbbd2bb1f3346a43cd32140648583673a31d62f2dfb56ad0ab9e3ffffffff02a0860100000000001976a9142f4490d5263906e4887ca2996b9e207af3e7824088aca0860100000000001976a914812c13d97f9159e54e326b481b8f88a73df8507a88ac00000000'
 
         # Now run the attack, must trigger the exception
-        with pytest.raises(CallException):
+        try:
             self.client.sign_tx('Bitcoin', [inp1, inp2], [out1, out2], debug_processor=attack_processor)
+        except CallException as exc:
+            assert exc.args[0] == proto.FailureType.ProcessError
+            assert exc.args[1] == 'Transaction has changed during signing'
+        else:
+            assert False  # exception expected
 
     def test_attack_change_input_address(self):
         # This unit test attempts to modify input address after the Trezor checked
         # that it matches the change output
 
         self.setup_mnemonic_allallall()
         self.client.set_tx_api(TxApiTestnet)
@@ -648,15 +656,14 @@
             script_type=proto.OutputScriptType.PAYTOADDRESS,
         )
 
         global run_attack
         run_attack = True
 
         def attack_processor(req, msg):
-            import sys
             global run_attack
 
             if req.details.tx_hash is not None:
                 return msg
 
             if req.request_type != proto.RequestType.TXINPUT:
                 return msg
@@ -687,16 +694,22 @@
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
                 proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.Failure(code=proto.FailureType.ProcessError),
             ])
-            with pytest.raises(CallException):
+            # Now run the attack, must trigger the exception
+            try:
                 self.client.sign_tx('Testnet', [inp1], [out1, out2], debug_processor=attack_processor)
+            except CallException as exc:
+                assert exc.args[0] == proto.FailureType.ProcessError
+                assert exc.args[1] == 'Transaction has changed during signing'
+            else:
+                assert False  # exception expected
 
     def test_spend_coinbase(self):
         # 25 TEST generated to m/1 (mfiGQVPcRcaEvQPYDErR34DcCovtxYvUUV)
         # tx: d6da21677d7cca5f42fbc7631d062c9ae918a0254f7c6c22de8e8cb7fd5b8236
         # input 0: 25.0027823 BTC
 
         self.setup_mnemonic_nopin_nopassphrase()
@@ -729,7 +742,117 @@
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.TxRequest(request_type=proto.RequestType.TXFINISHED),
             ])
             (signatures, serialized_tx) = self.client.sign_tx('Testnet', [inp1, ], [out1, ])
 
         # Accepted by network: tx
         assert hexlify(serialized_tx) == b'010000000136825bfdb78c8ede226c7c4f25a018e99a2c061d63c7fb425fca7c7d6721dad6000000006a473044022047845c366eb24f40be315c7815a154513c444c7989eb80f7ce7ff6aeb703d26a022007c1f5efadf67c5889634fd7ac39a7ce78bffac291673e8772ecd8389c901d9f01210338d78612e990f2eea0c426b5e48a8db70b9d7ed66282b3b26511e0b1c75515a6ffffffff01c6100795000000001976a9143d2496e67f5f57a924353da42d4725b318e7a8ea88ac00000000'
+
+    def test_two_changes(self):
+        self.setup_mnemonic_allallall()
+        # see 87be0736f202f7c2bff0781b42bad3e0cdcb54761939da69ea793a3735552c56
+
+        # tx: e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd
+        # input 0: 0.31 BTC
+        inp1 = proto.TxInputType(
+            address_n=self.client.expand_path("44'/1'/0'/0/0"),
+            # amount=31000000,
+            prev_hash=TXHASH_e5040e,
+            prev_index=0,
+        )
+
+        out1 = proto.TxOutputType(
+            address='msj42CCGruhRsFrGATiUuh25dtxYtnpbTx',
+            amount=30090000,
+            script_type=proto.OutputScriptType.PAYTOADDRESS,
+        )
+
+        out_change1 = proto.TxOutputType(
+            address_n=self.client.expand_path("44'/1'/0'/1/0"),
+            amount=900000,
+            script_type=proto.OutputScriptType.PAYTOADDRESS,
+        )
+
+        out_change2 = proto.TxOutputType(
+            address_n=self.client.expand_path("44'/1'/0'/1/1"),
+            amount=10000,
+            script_type=proto.OutputScriptType.PAYTOADDRESS,
+        )
+
+        with self.client:
+            self.client.set_tx_api(TxApiTestnet)
+            self.client.set_expected_responses([
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXMETA, details=proto.TxRequestDetailsType(tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1, tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=2)),
+                proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
+
+                proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=2)),
+
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=2)),
+                proto.TxRequest(request_type=proto.RequestType.TXFINISHED),
+            ])
+
+            self.client.sign_tx('Testnet', [inp1, ], [out1, out_change1, out_change2])
+
+    def test_change_on_main_chain_allowed(self):
+        self.setup_mnemonic_allallall()
+        # see 87be0736f202f7c2bff0781b42bad3e0cdcb54761939da69ea793a3735552c56
+
+        # tx: e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd
+        # input 0: 0.31 BTC
+        inp1 = proto.TxInputType(
+            address_n=self.client.expand_path("44'/1'/0'/0/0"),
+            # amount=31000000,
+            prev_hash=TXHASH_e5040e,
+            prev_index=0,
+        )
+
+        out1 = proto.TxOutputType(
+            address='msj42CCGruhRsFrGATiUuh25dtxYtnpbTx',
+            amount=30090000,
+            script_type=proto.OutputScriptType.PAYTOADDRESS,
+        )
+
+        # change on main chain is allowed => treated as a change
+        out_change = proto.TxOutputType(
+            address_n=self.client.expand_path("44'/1'/0'/0/0"),
+            amount=900000,
+            script_type=proto.OutputScriptType.PAYTOADDRESS,
+        )
+
+        with self.client:
+            self.client.set_tx_api(TxApiTestnet)
+            self.client.set_expected_responses([
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXMETA, details=proto.TxRequestDetailsType(tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_e5040e)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1, tx_hash=TXHASH_e5040e)),
+
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+
+                proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXFINISHED),
+            ])
+
+            self.client.sign_tx('Testnet', [inp1, ], [out1, out_change])
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_bcash.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_bcash.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from .common import *
 from trezorlib import messages as proto
 from trezorlib.tx_api import TxApiBcash
 from trezorlib.ckd_public import deserialize
 from trezorlib.client import CallException
 
 
-@pytest.mark.skip_t2
 class TestMsgSigntxBch(TrezorTest):
 
     def test_send_bch_change(self):
         self.setup_mnemonic_allallall()
         self.client.set_tx_api(TxApiBcash)
         inp1 = proto.TxInputType(
             address_n=self.client.expand_path("44'/145'/0'/0/0"),
@@ -104,68 +103,93 @@
 
     def test_attack_amount(self):
         self.setup_mnemonic_allallall()
         self.client.set_tx_api(TxApiBcash)
         inp1 = proto.TxInputType(
             address_n=self.client.expand_path("44'/145'/0'/1/0"),
             # 1HADRPJpgqBzThepERpVXNi6qRgiLQRNoE
-            amount=1896050 - 1,
+            amount=300,
             prev_hash=unhexlify('502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c'),
             prev_index=0,
             script_type=proto.InputScriptType.SPENDADDRESS,
         )
         inp2 = proto.TxInputType(
             address_n=self.client.expand_path("44'/145'/0'/0/1"),
             # 1LRspCZNFJcbuNKQkXgHMDucctFRQya5a3
-            amount=73452,
+            amount=70,
             prev_hash=unhexlify('502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c'),
             prev_index=1,
             script_type=proto.InputScriptType.SPENDADDRESS,
         )
         out1 = proto.TxOutputType(
             address='15pnEDZJo3ycPUamqP3tEDnEju1oW5fBCz',
-            amount=1934960,
+            amount=200,
             script_type=proto.OutputScriptType.PAYTOADDRESS,
         )
 
         global run_attack
         run_attack = True
 
         def attack_processor(req, msg):
-            import sys
             global run_attack
 
             if req.details.tx_hash is not None:
                 return msg
 
             if req.request_type != proto.RequestType.TXINPUT:
                 return msg
 
             if req.details.request_index != 0:
                 return msg
 
             if not run_attack:
                 return msg
 
-            msg.inputs[0].amount = 1896050
+            # 300 is lowered to 280 at the first run
+            # the user confirms 280 but the transaction
+            # is spending 300 => larger fee without the user knowing
+            msg.inputs[0].amount = 280
             run_attack = False
             return msg
 
+        # test if passes without modifications
         with self.client:
             self.client.set_expected_responses([
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=1)),
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
                 proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXFINISHED),
+            ])
+            self.client.sign_tx('Bcash', [inp1, inp2], [out1])
+
+        # now fails
+        with self.client:
+            self.client.set_expected_responses([
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=1)),
+                proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
+                proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
+                proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=1)),
                 proto.Failure(code=proto.FailureType.ProcessError),
             ])
-            with pytest.raises(CallException):
+
+            try:
                 self.client.sign_tx('Bcash', [inp1, inp2], [out1], debug_processor=attack_processor)
+            except CallException as exc:
+                assert exc.args[0] == proto.FailureType.ProcessError
+                assert exc.args[1] == 'Transaction has changed during signing'
+            else:
+                assert False  # exception expected
 
     def test_attack_change_input(self):
         self.setup_mnemonic_allallall()
         self.client.set_tx_api(TxApiBcash)
         inp1 = proto.TxInputType(
             address_n=self.client.expand_path("44'/145'/1000'/0/0"),
             # 1MH9KKcvdCTY44xVDC2k3fjBbX5Cz29N1q
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_decred.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_decred.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_segwit.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_segwit.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,9 +229,14 @@
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.ButtonRequest(code=proto.ButtonRequestType.ConfirmOutput),
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=1)),
                 proto.ButtonRequest(code=proto.ButtonRequestType.SignTx),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.Failure(code=proto.FailureType.ProcessError),
             ])
-            with pytest.raises(CallException):
+            try:
                 self.client.sign_tx('Testnet', [inp1], [out1, out2], debug_processor=attack_processor)
+            except CallException as exc:
+                assert exc.args[0] == proto.FailureType.ProcessError
+                assert exc.args[1] == 'Transaction has changed during signing'
+            else:
+                assert False  # exception expected
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_segwit_native.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_segwit_native.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_signtx_zcash.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_signtx_zcash.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage_segwit.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage_segwit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 import base64
 
 
-@pytest.mark.skip_t2
 class TestMsgVerifymessageSegwit(TrezorTest):
 
     def test_message_long(self):
         self.setup_mnemonic_nopin_nopassphrase()
         ret = self.client.verify_message(
             'Bitcoin',
             '3CwYaeWxhpXXiHue3ciQez1DLaTEAXcKa1',
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_verifymessage_segwit_native.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_verifymessage_segwit_native.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 from .common import *
 import base64
 
 
-@pytest.mark.skip_t2
 class TestMsgVerifymessageSegwitNative(TrezorTest):
 
     def test_message_long(self):
         self.setup_mnemonic_nopin_nopassphrase()
         ret = self.client.verify_message(
             'Bitcoin',
             'bc1qyjjkmdpu7metqt5r36jf872a34syws33s82q2j',
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_msg_wipedevice.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_msg_wipedevice.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_multisig.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_multisig.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 # Multisig howto:
 #
 # https://sx.dyne.org/multisig.html
 #
 
 
-@pytest.mark.skip_t2
 class TestMultisig(TrezorTest):
 
     def test_2_of_3(self):
         self.setup_mnemonic_nopin_nopassphrase()
 
         # key1 = self.client.get_public_node([1])
         # key2 = self.client.get_public_node([2])
@@ -246,11 +245,14 @@
 
         out1 = proto.TxOutputType(
             address='12iyMbUb4R2K3gre4dHSrbu5azG5KaqVss',
             amount=100000,
             script_type=proto.OutputScriptType.PAYTOADDRESS
         )
 
-        with self.client:
-            # It should throw Failure 'Pubkey not found in multisig script'
-            with pytest.raises(CallException):
-                self.client.sign_tx('Bitcoin', [inp1, ], [out1, ])
+        try:
+            self.client.sign_tx('Bitcoin', [inp1, ], [out1, ])
+        except CallException as exc:
+            assert exc.args[0] == proto.FailureType.DataError
+            assert exc.args[1] == 'Pubkey not found in multisig script'
+        else:
+            assert False  # exception expected
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_multisig_change.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_multisig_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from .common import *
 from trezorlib import messages as proto
 import trezorlib.ckd_public as bip32
 from trezorlib import tx_api
 
 
-@pytest.mark.skip_t2
 class TestMultisigChange(TrezorTest):
 
     def setup_method(self, method):
         super(TestMultisigChange, self).setup_method(method)
         self.client.set_tx_api(tx_api.TxApiTestnet)
 
     node_ext1 = bip32.deserialize('tpubDADHV9u9Y6gkggintTdMjJE3be58zKNLhpxBQyuEM6Pwx3sN9JVLmMCMN4DNVwL9AKec27z5TaWcWuHzMXiGAtcra5DjwWbvppGX4gaEGVN')
@@ -311,15 +310,15 @@
 
         with self.client:
             self.client.set_expected_responses(self._responses(self.inp1, self.inp2, change=2))
             (_, serialized_tx) = self.client.sign_tx('Testnet', [self.inp1, self.inp2, ], [out1, out2, ])
 
         assert hexlify(serialized_tx) == b'0100000002e53cf4e3fcd37f8c439286ce636476e1faeebf86bbb2f228a6b78d1b47c8c61601000000b400473044022059394e0dfcb2d2f4a6108703f801545ca5a820c0ac6a1859d0a3854813de55fa02207b6a57d70b82932ff58163336c461653a2dc82c78ed8157159e5178ac7325390014c69522103dc07026aacb5918dac4e09f9da8290d0ae22161699636c22cace78082116a7792103e70db185fad69c2971f0107a42930e5d82a9ed3a11b922a96fdfc4124b63e54c2103f3fe007a1e34ac76c1a2528e9149f90f9f93739929797afab6a8e18d682fa71053aeffffffff185315ae8050e18efa70d6ca96378a1194f57e2b102511f68b3a1414ee340cd800000000b40047304402205a911685f5b974b2fc4a19d5ce056218773a4d20b5eaae2c2f9594929308182002201e03449f5a8813ec19f408bf1b6f4f334886d6fcf9920e300fd7678ef0724f81014c6952210297ad8a5df42f9e362ef37d9a4ddced89d8f7a143690649aa0d0ff049c7daca842103ed1fd93989595d7ad4b488efd05a22c0239482c9a20923f2f214a38e54f6c41a2103f91460d79e4e463d7d90cb75254bcd62b515a99a950574c721efdc5f711dff3553aeffffffff02005a62020000000017a91466528dd543f94d162c8111d2ec248d25ba9b90948700639f020000000017a914f1fc92c0aed1712911c70a2e09ac15ff0922652f8700000000'
 
-    # inputs match, change mismatches (second is change)
+    # inputs match, change mismatches (second tries to be change but isn't)
     def test_multisig_mismatch_change(self):
         self.setup_mnemonic_nopin_nopassphrase()
 
         multisig_out2 = proto.MultisigRedeemScriptType(
             pubkeys=[
                 proto.HDNodePathType(node=self.node_ext1, address_n=[1, 0]),
                 proto.HDNodePathType(node=self.node_int, address_n=[1, 0]),
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_op_return.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_op_return.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,20 +85,14 @@
             address_n=[0],  # 14LmW5k4ssUrtbAB4255zdqv3b4w1TuX9e
             # amount=390000,
             prev_hash=TXHASH_d5f65e,
             prev_index=0,
         )
 
         out1 = proto.TxOutputType(
-            address='1MJ2tj2ThBE62zXbBYA5ZaN3fdve5CPAz1',
-            amount=390000 - 10000 - 10000,
-            script_type=proto.OutputScriptType.PAYTOADDRESS,
-        )
-
-        out1 = proto.TxOutputType(
             op_return_data=b'test of the op_return data',
             amount=10000,
             script_type=proto.OutputScriptType.PAYTOOPRETURN,
         )
 
         with self.client:
             self.client.set_expected_responses([
@@ -106,9 +100,15 @@
                 proto.TxRequest(request_type=proto.RequestType.TXMETA, details=proto.TxRequestDetailsType(tx_hash=TXHASH_d5f65e)),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_d5f65e)),
                 proto.TxRequest(request_type=proto.RequestType.TXINPUT, details=proto.TxRequestDetailsType(request_index=1, tx_hash=TXHASH_d5f65e)),
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0, tx_hash=TXHASH_d5f65e)),
                 proto.TxRequest(request_type=proto.RequestType.TXOUTPUT, details=proto.TxRequestDetailsType(request_index=0)),
                 proto.Failure()
             ])
-            with pytest.raises(CallException):
-                self.client.sign_tx('Bitcoin', [inp1, ], [out1, ])
+
+            try:
+                self.client.sign_tx('Bitcoin', [inp1], [out1])
+            except CallException as exc:
+                assert exc.args[0] == proto.FailureType.DataError
+                assert exc.args[1] == 'OP_RETURN output with non-zero amount'
+            else:
+                assert False  # exception expected
```

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_protect_call.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_protect_call.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_protection_levels.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_protection_levels.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/device_tests/test_zerosig.py` & `trezor-0.9.1/trezorlib/tests/device_tests/test_zerosig.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_502e8577b237b0152843a416f8f1ab0c63321b1be7a8cad7bf5c5c216fcf062c.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_8b6db9b8ba24235d86b053ea2ccb484fc32b96f89c3c39f98d86f90db16076a0.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_8b6db9b8ba24235d86b053ea2ccb484fc32b96f89c3c39f98d86f90db16076a0.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_bc37c28dfb467d2ecb50261387bf752a3977d7e5337915071bb4151e6b711a78.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_bc37c28dfb467d2ecb50261387bf752a3977d7e5337915071bb4151e6b711a78.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bcash_tx_f68caf10df12d5b07a34601d88fa6856c6edcbf4d05ebef3486510ae1c293d5f.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bcash_tx_f68caf10df12d5b07a34601d88fa6856c6edcbf4d05ebef3486510ae1c293d5f.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_1570416eb4302cf52979afd5e6909e37d8fdd874301f7cc87e547e509cb1caa6.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_1570416eb4302cf52979afd5e6909e37d8fdd874301f7cc87e547e509cb1caa6.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_39a29e954977662ab3879c66fb251ef753e0912223a83d1dcb009111d28265e5.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_39a29e954977662ab3879c66fb251ef753e0912223a83d1dcb009111d28265e5.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_50f6f1209ca92d7359564be803cb2c932cde7d370f7cee50fd1fad6790f6206d.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_50f6f1209ca92d7359564be803cb2c932cde7d370f7cee50fd1fad6790f6206d.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_54aa5680dea781f45ebb536e53dffc526d68c0eb5c00547e323b2c32382dfba3.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_54aa5680dea781f45ebb536e53dffc526d68c0eb5c00547e323b2c32382dfba3.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_58497a7757224d1ff1941488d23087071103e5bf855f4c1c44e5c8d9d82ca46e.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_58497a7757224d1ff1941488d23087071103e5bf855f4c1c44e5c8d9d82ca46e.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_6189e3febb5a21cee8b725aa1ef04ffce7e609448446d3a8d6f483c634ef5315.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_6189e3febb5a21cee8b725aa1ef04ffce7e609448446d3a8d6f483c634ef5315.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_a6e2829d089cee47e481b1a753a53081b40738cc87e38f1d9b23ab57d9ad4396.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_a6e2829d089cee47e481b1a753a53081b40738cc87e38f1d9b23ab57d9ad4396.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c6091adf4c0c23982a35899a6e58ae11e703eacd7954f588ed4b9cdefc4dba52.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c6091adf4c0c23982a35899a6e58ae11e703eacd7954f588ed4b9cdefc4dba52.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c63e24ed820c5851b60c54613fbc4bcb37df6cd49b4c96143e99580a472f79fb.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_c6be22d34946593bcad1d2b013e12f74159e69574ffea21581dad115572e031c.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_c6be22d34946593bcad1d2b013e12f74159e69574ffea21581dad115572e031c.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_d1d08ea63255af4ad16b098e9885a252632086fa6be53301521d05253ce8a73d.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_d1d08ea63255af4ad16b098e9885a252632086fa6be53301521d05253ce8a73d.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_d5f65ee80147b4bcc70b75e4bbf2d7382021b871bd8867ef8fa525ef50864882.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_d5f65ee80147b4bcc70b75e4bbf2d7382021b871bd8867ef8fa525ef50864882.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_bitcoin_tx_e4bc1ae5e5007a08f2b3926fe11c66612e8f73c6b00c69c7027213b84d259be3.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_bitcoin_tx_e4bc1ae5e5007a08f2b3926fe11c66612e8f73c6b00c69c7027213b84d259be3.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_16da185052740d85a630e79c140558215b64e26c500212b90e16b55d13ca06a8.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_16da185052740d85a630e79c140558215b64e26c500212b90e16b55d13ca06a8.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_3f7c395521d38387e7617565fe17628723ef6635a08537ad9c46cfb1619e4c3f.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_3f7c395521d38387e7617565fe17628723ef6635a08537ad9c46cfb1619e4c3f.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_5e6e3500a333c53c02f523db5f1a9b17538a8850b4c2c24ecb9b7ba48059b970.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_5e6e3500a333c53c02f523db5f1a9b17538a8850b4c2c24ecb9b7ba48059b970.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_ccf95b0fd220ef59ae2e5b17005a81e222758122682d522eff8ae1fcbc93bc74.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_ccf95b0fd220ef59ae2e5b17005a81e222758122682d522eff8ae1fcbc93bc74.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_e16248f0b39a0a0c0e53d6f2f84c2a944f0d50e017a82701e8e02e46e979d5ed.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_e16248f0b39a0a0c0e53d6f2f84c2a944f0d50e017a82701e8e02e46e979d5ed.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_decred_testnet_tx_f395ef3e72a831a766db15e7a38bc28025d4ee02234d68bdea2d8353b47a3113.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_decred_testnet_tx_f395ef3e72a831a766db15e7a38bc28025d4ee02234d68bdea2d8353b47a3113.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_09144602765ce3dd8f4329445b20e3684e948709c5cdcaf12da3bb079c99448a.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_09144602765ce3dd8f4329445b20e3684e948709c5cdcaf12da3bb079c99448a.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_16c6c8471b8db7a628f2b2bb86bfeefae1766463ce8692438c7fd3fce3f43ce5.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_16c6c8471b8db7a628f2b2bb86bfeefae1766463ce8692438c7fd3fce3f43ce5.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_20912f98ea3ed849042efed0fdac8cb4fc301961c5988cba56902d8ffb61c337.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_20912f98ea3ed849042efed0fdac8cb4fc301961c5988cba56902d8ffb61c337.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_31bc1c88ce6ae337a6b3057a16d5bad0b561ad1dfc047d0a7fbb8814668f91e5.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_31bc1c88ce6ae337a6b3057a16d5bad0b561ad1dfc047d0a7fbb8814668f91e5.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_65b811d3eca0fe6915d9f2d77c86c5a7f19bf66b1b1253c2c51cb4ae5f0c017b.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_65b811d3eca0fe6915d9f2d77c86c5a7f19bf66b1b1253c2c51cb4ae5f0c017b.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_6f90f3c7cbec2258b0971056ef3fe34128dbde30daa9c0639a898f9977299d54.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_6f90f3c7cbec2258b0971056ef3fe34128dbde30daa9c0639a898f9977299d54.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_9c31922be756c06d02167656465c8dc83bb553bf386a3f478ae65b5c021002be.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_9c31922be756c06d02167656465c8dc83bb553bf386a3f478ae65b5c021002be.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_b0946dc27ba308a749b11afecc2018980af18f79e89ad6b080b58220d856f739.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_b0946dc27ba308a749b11afecc2018980af18f79e89ad6b080b58220d856f739.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_c9348040bbc2024e12dcb4a0b4806b0398646b91acf314da028c3f03dd0179fc.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_c9348040bbc2024e12dcb4a0b4806b0398646b91acf314da028c3f03dd0179fc.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d2dcdaf547ea7f57a713c607f15e883ddc4a98167ee2c43ed953c53cb5153e24.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d2dcdaf547ea7f57a713c607f15e883ddc4a98167ee2c43ed953c53cb5153e24.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d6da21677d7cca5f42fbc7631d062c9ae918a0254f7c6c22de8e8cb7fd5b8236.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d6da21677d7cca5f42fbc7631d062c9ae918a0254f7c6c22de8e8cb7fd5b8236.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_d80c34ee14143a8bf61125102b7ef594118a3796cad670fa8ee15080ae155318.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_d80c34ee14143a8bf61125102b7ef594118a3796cad670fa8ee15080ae155318.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_e5040e1bc1ae7667ffb9e5248e90b2fb93cd9150234151ce90e14ab2f5933bcd.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/txcache/insight_testnet_tx_f41cbedd8becee05a830f418d13aa665125464547db5c7a6cd28f21639fe1228.json` & `trezor-0.9.1/trezorlib/tests/txcache/insight_testnet_tx_f41cbedd8becee05a830f418d13aa665125464547db5c7a6cd28f21639fe1228.json`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/unit_tests/test_ckd_public.py` & `trezor-0.9.1/trezorlib/tests/unit_tests/test_ckd_public.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tests/unit_tests/test_tx_api.py` & `trezor-0.9.1/trezorlib/tests/unit_tests/test_tx_api.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/ckd_public.py` & `trezor-0.9.1/trezorlib/ckd_public.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/client.py` & `trezor-0.9.1/trezorlib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from mnemonic import Mnemonic
 
 from . import messages as proto
 from . import tools
 from . import mapping
 from .coins import coins_slip44
 from .debuglink import DebugLink
+from .protobuf import MessageType
 
 # Python2 vs Python3
 try:
     input = raw_input
 except NameError:
     pass
 
@@ -82,35 +83,73 @@
 
 
 def get_buttonrequest_value(code):
     # Converts integer code to its string representation of ButtonRequestType
     return [k for k in dir(proto.ButtonRequestType) if getattr(proto.ButtonRequestType, k) == code][0]
 
 
+def format_protobuf(pb, indent=0, sep=' ' * 4):
+    def pformat_value(value, indent):
+        level = sep * indent
+        leadin = sep * (indent + 1)
+        if isinstance(value, MessageType):
+            return format_protobuf(value, indent, sep)
+        if isinstance(value, list):
+            lines = []
+            lines.append('[')
+            lines += [leadin + pformat_value(x, indent + 1) + ',' for x in value]
+            lines.append(level + ']')
+            return '\n'.join(lines)
+        if isinstance(value, dict):
+            lines = []
+            lines.append('{')
+            for key, val in sorted(value.items()):
+                if val is None or val == []:
+                    continue
+                if key == 'address_n' and isinstance(val, list):
+                    lines.append(leadin + key + ': ' + repr(val) + ',')
+                else:
+                    lines.append(leadin + key + ': ' + pformat_value(val, indent + 1) + ',')
+            lines.append(level + '}')
+            return '\n'.join(lines)
+        if isinstance(value, bytearray):
+            return 'bytearray(0x{})'.format(value.hex())
+
+        return repr(value)
+
+    return pb.__class__.__name__ + ' ' + pformat_value(pb.__dict__, indent)
+
+
 def pprint(msg):
     msg_class = msg.__class__.__name__
     msg_size = msg.ByteSize()
-    if isinstance(msg, proto.FirmwareUpload) or isinstance(msg, proto.SelfTest):
-        return "<%s> (%d bytes):\n" % (msg_class, msg_size)
+    if isinstance(msg, proto.FirmwareUpload) or isinstance(msg, proto.SelfTest) \
+            or isinstance(msg, proto.Features):
+        return "<%s> (%d bytes)" % (msg_class, msg_size)
     else:
-        return "<%s> (%d bytes):\n%s" % (msg_class, msg_size, msg)
+        return "<%s> (%d bytes):\n%s" % (msg_class, msg_size, format_protobuf(msg))
 
 
 def log(msg):
     sys.stderr.write(msg)
     sys.stderr.write('\n')
     sys.stderr.flush()
 
 
 class CallException(Exception):
     def __init__(self, code, message):
         super(CallException, self).__init__()
         self.args = [code, message]
 
 
+class AssertionException(Exception):
+    def __init__(self, code, message):
+        self.args = [code, message]
+
+
 class PinException(CallException):
     pass
 
 
 class field(object):
     # Decorator extracts single value from
     # protobuf object. If the field is not
@@ -274,14 +313,17 @@
         log("Please enter %s: " % desc)
         pin = getpass.getpass('')
         if not pin.isdigit():
             raise ValueError('Non-numerical PIN provided')
         return proto.PinMatrixAck(pin=pin)
 
     def callback_PassphraseRequest(self, msg):
+        if msg.on_device is True:
+            return proto.PassphraseAck()
+
         if os.getenv("PASSPHRASE") is not None:
             log("Passphrase required. Using PASSPHRASE environment variable.")
             passphrase = Mnemonic.normalize_string(os.getenv("PASSPHRASE"))
             return proto.PassphraseAck(passphrase=passphrase)
 
         log("Passphrase required: ")
         passphrase = getpass.getpass('')
@@ -289,14 +331,17 @@
         if passphrase == getpass.getpass(''):
             passphrase = Mnemonic.normalize_string(passphrase)
             return proto.PassphraseAck(passphrase=passphrase)
         else:
             log("Passphrase did not match! ")
             exit()
 
+    def callback_PassphraseStateRequest(self, msg):
+        return proto.PassphraseStateAck()
+
     def callback_WordRequest(self, msg):
         if msg.type in (proto.WordRequestType.Matrix9,
                         proto.WordRequestType.Matrix6):
             return self.callback_RecoveryMatrix(msg)
         log("Enter one word of mnemonic: ")
         word = input()
         if self.expand:
@@ -398,27 +443,27 @@
         return resp
 
     def _check_request(self, msg):
         if self.expected_responses is not None:
             try:
                 expected = self.expected_responses.pop(0)
             except IndexError:
-                raise CallException(proto.FailureType.UnexpectedMessage,
-                                    "Got %s, but no message has been expected" % pprint(msg))
+                raise AssertionException(proto.FailureType.UnexpectedMessage,
+                                         "Got %s, but no message has been expected" % pprint(msg))
 
             if msg.__class__ != expected.__class__:
-                raise CallException(proto.FailureType.UnexpectedMessage,
-                                    "Expected %s, got %s" % (pprint(expected), pprint(msg)))
+                raise AssertionException(proto.FailureType.UnexpectedMessage,
+                                         "Expected %s, got %s" % (pprint(expected), pprint(msg)))
 
             for field, value in expected.__dict__.items():
                 if value is None or value == []:
                     continue
                 if getattr(msg, field) != value:
-                    raise CallException(proto.FailureType.UnexpectedMessage,
-                                        "Expected %s, got %s" % (pprint(expected), pprint(msg)))
+                    raise AssertionException(proto.FailureType.UnexpectedMessage,
+                                             "Expected %s, got %s" % (pprint(expected), pprint(msg)))
 
     def callback_ButtonRequest(self, msg):
         log("ButtonRequest code: " + get_buttonrequest_value(msg.code))
 
         log("Pressing button " + str(self.button))
         if self.button_wait:
             log("Waiting %d seconds " % self.button_wait)
@@ -433,14 +478,17 @@
             pin = '444222'
         return proto.PinMatrixAck(pin=pin)
 
     def callback_PassphraseRequest(self, msg):
         log("Provided passphrase: '%s'" % self.passphrase)
         return proto.PassphraseAck(passphrase=self.passphrase)
 
+    def callback_PassphraseStateRequest(self, msg):
+        return proto.PassphraseStateAck()
+
     def callback_WordRequest(self, msg):
         (word, pos) = self.debug.read_recovery_word()
         if word != '':
             return proto.WordAck(word=word)
         if pos != 0:
             return proto.WordAck(word=self.mnemonic[pos - 1])
 
@@ -925,33 +973,41 @@
                 res = self.call(proto.TxAck(tx=msg))
                 continue
 
             elif res.request_type == proto.RequestType.TXINPUT:
                 msg = proto.TransactionType()
                 msg._extend_inputs([current_tx.inputs[res.details.request_index], ])
                 if debug_processor is not None:
+                    # msg needs to be deep copied so when it's modified
+                    # the other messages stay intact
+                    from copy import deepcopy
+                    msg = deepcopy(msg)
                     # If debug_processor function is provided,
                     # pass thru it the request and prepared response.
-                    # This is useful for unit tests, see test_msg_signtx
+                    # This is useful for tests, see test_msg_signtx
                     msg = debug_processor(res, msg)
 
                 res = self.call(proto.TxAck(tx=msg))
                 continue
 
             elif res.request_type == proto.RequestType.TXOUTPUT:
                 msg = proto.TransactionType()
                 if res.details.tx_hash:
                     msg._extend_bin_outputs([current_tx.bin_outputs[res.details.request_index], ])
                 else:
                     msg._extend_outputs([current_tx.outputs[res.details.request_index], ])
 
                 if debug_processor is not None:
+                    # msg needs to be deep copied so when it's modified
+                    # the other messages stay intact
+                    from copy import deepcopy
+                    msg = deepcopy(msg)
                     # If debug_processor function is provided,
                     # pass thru it the request and prepared response.
-                    # This is useful for unit tests, see test_msg_signtx
+                    # This is useful for tests, see test_msg_signtx
                     msg = debug_processor(res, msg)
 
                 res = self.call(proto.TxAck(tx=msg))
                 continue
 
             elif res.request_type == proto.RequestType.TXEXTRADATA:
                 o, l = res.details.extra_data_offset, res.details.extra_data_len
```

### Comparing `trezor-0.9.0/trezorlib/debuglink.py` & `trezor-0.9.1/trezorlib/debuglink.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/device.py` & `trezor-0.9.1/trezorlib/device.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/ed25519cosi.py` & `trezor-0.9.1/trezorlib/ed25519cosi.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/ed25519raw.py` & `trezor-0.9.1/trezorlib/ed25519raw.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/mapping.py` & `trezor-0.9.1/trezorlib/mapping.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/protobuf.py` & `trezor-0.9.1/trezorlib/protobuf.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/protocol_v1.py` & `trezor-0.9.1/trezorlib/protocol_v1.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/protocol_v2.py` & `trezor-0.9.1/trezorlib/protocol_v2.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/tools.py` & `trezor-0.9.1/trezorlib/tools.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/transport.py` & `trezor-0.9.1/trezorlib/transport.py`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/trezorlib/transport_bridge.py` & `trezor-0.9.1/trezorlib/transport_bridge.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 class BridgeTransport(Transport):
     '''
     BridgeTransport implements transport through TREZOR Bridge (aka trezord).
     '''
 
     PATH_PREFIX = 'bridge'
+    HEADERS = {'Origin': 'https://python.trezor.io'}
 
     def __init__(self, device):
         super(BridgeTransport, self).__init__()
 
         self.device = device
         self.conn = requests.Session()
         self.session = None
@@ -53,18 +54,18 @@
 
     def __str__(self):
         return self.get_path()
 
     def get_path(self):
         return '%s:%s' % (self.PATH_PREFIX, self.device['path'])
 
-    @staticmethod
-    def enumerate():
+    @classmethod
+    def enumerate(cls):
         try:
-            r = requests.post(TREZORD_HOST + '/enumerate')
+            r = requests.post(TREZORD_HOST + '/enumerate', headers=cls.HEADERS)
             if r.status_code != 200:
                 raise TransportException('trezord: Could not enumerate devices' + get_error(r))
             return [BridgeTransport(dev) for dev in r.json()]
         except:
             return []
 
     @classmethod
@@ -75,35 +76,35 @@
 
         for transport in BridgeTransport.enumerate():
             if path is None or transport.device['path'] == path:
                 return transport
         raise TransportException('Bridge device not found')
 
     def open(self):
-        r = self.conn.post(TREZORD_HOST + '/acquire/%s/null' % self.device['path'])
+        r = self.conn.post(TREZORD_HOST + '/acquire/%s/null' % self.device['path'], headers=self.HEADERS)
         if r.status_code != 200:
             raise TransportException('trezord: Could not acquire session' + get_error(r))
         self.session = r.json()['session']
 
     def close(self):
         if not self.session:
             return
-        r = self.conn.post(TREZORD_HOST + '/release/%s' % self.session)
+        r = self.conn.post(TREZORD_HOST + '/release/%s' % self.session, headers=self.HEADERS)
         if r.status_code != 200:
             raise TransportException('trezord: Could not release session' + get_error(r))
         self.session = None
 
     def write(self, msg):
         data = BytesIO()
         protobuf.dump_message(data, msg)
         ser = data.getvalue()
         header = struct.pack(">HL", mapping.get_type(msg), len(ser))
         data = binascii.hexlify(header + ser).decode()
         r = self.conn.post(
-            TREZORD_HOST + '/call/%s' % self.session, data=data)
+            TREZORD_HOST + '/call/%s' % self.session, data=data, headers=self.HEADERS)
         if r.status_code != 200:
             raise TransportException('trezord: Could not write message' + get_error(r))
         self.response = r.text
 
     def read(self):
         if self.response is None:
             raise TransportException('No response stored')
```

### Comparing `trezor-0.9.0/trezorlib/transport_hid.py` & `trezor-0.9.1/trezorlib/transport_hid.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
     def __init__(self, device, protocol=None, hid_handle=None):
         super(HidTransport, self).__init__()
 
         if hid_handle is None:
             hid_handle = HidHandle(device['path'])
 
         if protocol is None:
-            force_v1 = os.environ.get('TREZOR_TRANSPORT_V1', '0')
+            # force_v1 = os.environ.get('TREZOR_TRANSPORT_V1', '0')
+            force_v1 = True
 
             if is_trezor2(device) and not int(force_v1):
                 protocol = ProtocolV2()
             else:
                 protocol = ProtocolV1()
 
         self.device = device
```

### Comparing `trezor-0.9.0/trezorlib/transport_udp.py` & `trezor-0.9.1/trezorlib/transport_udp.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,14 @@
             host = UdpTransport.DEFAULT_HOST
             port = UdpTransport.DEFAULT_PORT
         else:
             devparts = device.split(':')
             host = devparts[0]
             port = int(devparts[1]) if len(devparts) > 1 else UdpTransport.DEFAULT_PORT
         if not protocol:
-            '''
-            force_v1 = os.environ.get('TREZOR_TRANSPORT_V1', '0')
-            if not int(force_v1):
-                protocol = ProtocolV2()
-            else:
-                protocol = ProtocolV1()
-            '''
             protocol = ProtocolV1()
         self.device = (host, port)
         self.protocol = protocol
         self.socket = None
 
     def __str__(self):
         return self.get_path()
```

### Comparing `trezor-0.9.0/trezorlib/transport_webusb.py` & `trezor-0.9.1/trezorlib/transport_webusb.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
     def __init__(self, device, protocol=None, handle=None, debug=False):
         super(WebUsbTransport, self).__init__()
 
         if handle is None:
             handle = WebUsbHandle(device)
 
         if protocol is None:
-            force_v1 = os.environ.get('TREZOR_TRANSPORT_V1', '0')
+            # force_v1 = os.environ.get('TREZOR_TRANSPORT_V1', '0')
+            force_v1 = True
 
             if is_trezor2(device) and not int(force_v1):
                 protocol = ProtocolV2()
             else:
                 protocol = ProtocolV1()
 
         self.device = device
```

### Comparing `trezor-0.9.0/trezorlib/tx_api.py` & `trezor-0.9.1/trezorlib/tx_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,7 +189,8 @@
 TxApiLitecoin = TxApiInsight(network='insight_litecoin', url='https://ltc-bitcore1.trezor.io/api/')
 TxApiDash = TxApiInsight(network='insight_dash', url='https://dash-bitcore1.trezor.io/api/')
 TxApiZcash = TxApiInsight(network='insight_zcash', url='https://zec-bitcore1.trezor.io/api/', zcash=True)
 TxApiBcash = TxApiInsight(network='insight_bcash', url='https://bch-bitcore2.trezor.io/api/')
 TxApiDecredTestnet = TxApiInsight(network='insight_decred_testnet', url='https://testnet.decred.org/api/')
 TxApiDogecoin = TxApiBlockCypher(network='blockcypher_dogecoin', url='https://api.blockcypher.com/v1/doge/main/')
 TxApiSegnet = TxApiSmartbit(network='smartbit_segnet', url='https://segnet-api.smartbit.com.au/v1/blockchain/')
+TxApiMonacoin = TxApiInsight(network='insight_monacoin', url='https://mona.insight.monaco-ex.org/insight-api-monacoin/')
```

### Comparing `trezor-0.9.0/COPYING` & `trezor-0.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/README.rst` & `trezor-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `trezor-0.9.0/setup.py` & `trezor-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 install_requires = [
     'setuptools>=19.0',
     'ecdsa>=0.9',
     'mnemonic>=0.17',
     'requests>=2.4.0',
     'click>=6.2',
     'pyblake2>=0.9.3',
+    'rlp>=0.6.0',
 ]
 
 import sys
 if '--disable-hidapi' in sys.argv:
     sys.argv.remove('--disable-hidapi')
 else:
     install_requires.append('hidapi>=0.7.99.post20')
@@ -35,16 +36,18 @@
         'trezorlib.messages',
         'trezorlib.qt',
         'trezorlib.tests.device_tests',
         'trezorlib.tests.unit_tests',
     ],
     scripts=['trezorctl'],
     install_requires=install_requires,
+    python_requires='>=3.3',
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS :: MacOS X',
+        'Programming Language :: Python :: 3 :: Only',
     ],
 )
```

### Comparing `trezor-0.9.0/trezorctl` & `trezor-0.9.1/trezorctl`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 # along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 import base64
 import binascii
 import click
 import functools
 import json
+import os
 import sys
 
-from trezorlib.client import TrezorClient, TrezorClientVerbose, CallException
+from trezorlib.client import TrezorClient, TrezorClientVerbose, CallException, format_protobuf
 from trezorlib.device import TrezorDevice
 from trezorlib import messages as proto
 from trezorlib import protobuf
 from trezorlib.coins import coins_txapi
 from trezorlib.ckd_public import PRIME_DERIVATION_FLAG
 
 
@@ -59,45 +60,47 @@
 CHOICE_OUTPUT_SCRIPT_TYPE = ChoiceType({
     'address':    proto.OutputScriptType.PAYTOADDRESS,
     'segwit':     proto.OutputScriptType.PAYTOWITNESS,
     'p2shsegwit': proto.OutputScriptType.PAYTOP2SHWITNESS,
 })
 
 
-@click.group()
-@click.option('-p', '--path', help='Select device by specific path.')
+@click.group(context_settings={'max_content_width': 400})
+@click.option('-p', '--path', help='Select device by specific path.', default=os.environ.get('TREZOR_PATH'))
 @click.option('-v', '--verbose', is_flag=True, help='Show communication messages.')
 @click.option('-j', '--json', 'is_json', is_flag=True, help='Print result as JSON object')
 @click.pass_context
 def cli(ctx, path, verbose, is_json):
     if ctx.invoked_subcommand != 'list':
         if verbose:
             ctx.obj = lambda: TrezorClientVerbose(TrezorDevice.find_by_path(path))
         else:
             ctx.obj = lambda: TrezorClient(TrezorDevice.find_by_path(path))
 
 
 @cli.resultcallback()
 def print_result(res, path, verbose, is_json):
     if is_json:
-        if issubclass(res.__class__, protobuf.MessageType):
+        if isinstance(res, protobuf.MessageType):
             click.echo(json.dumps({res.__class__.__name__: res.__dict__}))
         else:
             click.echo(json.dumps(res, sort_keys=True, indent=4))
     else:
         if isinstance(res, list):
             for line in res:
                 click.echo(line)
         elif isinstance(res, dict):
             for k, v in res.items():
                 if isinstance(v, dict):
                     for kk, vv in v.items():
                         click.echo('%s.%s: %s' % (k, kk, vv))
                 else:
                     click.echo('%s: %s' % (k, v))
+        elif isinstance(res, protobuf.MessageType):
+            click.echo(format_protobuf(res))
         else:
             click.echo(res)
 
 
 #
 # Common functions
 #
@@ -300,24 +303,25 @@
         rec_type,
         expand,
         dry_run
     )
 
 
 @cli.command(help='Perform device setup and generate new seed.')
+@click.option('-e', '--entropy', is_flag=True)
 @click.option('-t', '--strength', type=click.Choice(['128', '192', '256']), default='256')
-@click.option('-p', '--pin-protection', is_flag=True)
 @click.option('-r', '--passphrase-protection', is_flag=True)
+@click.option('-p', '--pin-protection', is_flag=True)
 @click.option('-l', '--label')
 @click.option('-u', '--u2f-counter', default=0)
 @click.option('-s', '--skip-backup', is_flag=True)
 @click.pass_obj
-def reset_device(connect, strength, pin_protection, passphrase_protection, label, u2f_counter, skip_backup):
+def reset_device(connect, entropy, strength, passphrase_protection, pin_protection, label, u2f_counter, skip_backup):
     return connect().reset_device(
-        True,
+        entropy,
         int(strength),
         passphrase_protection,
         pin_protection,
         label,
         'english',
         u2f_counter,
         skip_backup
@@ -576,17 +580,17 @@
         'signature': '0x%s' % binascii.hexlify(ret.signature).decode()
     }
     return output
 
 
 def ethereum_decode_hex(value):
     if value.startswith('0x') or value.startswith('0X'):
-        return value[2:].decode('hex')
+        return binascii.unhexlify(value[2:])
     else:
-        return value.decode('hex')
+        return binascii.unhexlify(value)
 
 
 @cli.command(help='Verify message signed with Ethereum address.')
 @click.argument('address')
 @click.argument('signature')
 @click.argument('message')
 @click.pass_obj
@@ -725,15 +729,15 @@
     if gas_limit is not None:
         gas_limit = int(gas_limit)
 
     to_address = ethereum_decode_hex(to)
 
     client = connect()
     address_n = client.expand_path(address)
-    address = '0x%s' % (binascii.hexlify(client.ethereum_get_address(address_n)),)
+    address = '0x%s' % (binascii.hexlify(client.ethereum_get_address(address_n)).decode())
 
     if gas_price is None or gas_limit is None or nonce is None:
         host, port = host.split(':')
         eth = EthJsonRpc(host, int(port))
 
     if not data:
         data = ''
@@ -743,15 +747,15 @@
         gas_price = eth.eth_gasPrice()
 
     if gas_limit is None:
         gas_limit = eth.eth_estimateGas(
             to_address=to,
             from_address=address,
             value=('0x%x' % value),
-            data='0x' + data)
+            data='0x%s' % (binascii.hexlify(data).decode()))
 
     if nonce is None:
         nonce = eth.eth_getTransactionCount(address)
 
     sig = client.ethereum_sign_tx(
         n=address_n,
         nonce=nonce,
@@ -760,15 +764,15 @@
         to=to_address,
         value=value,
         data=data,
         chain_id=chain_id)
 
     transaction = rlp.encode(
         (nonce, gas_price, gas_limit, to_address, value, data) + sig)
-    tx_hex = '0x%s' % binascii.hexlify(transaction)
+    tx_hex = '0x%s' % binascii.hexlify(transaction).decode()
 
     if publish:
         tx_hash = eth.eth_sendRawTransaction(tx_hex)
         return 'Transaction published with ID: %s' % tx_hash
     else:
         return 'Signed raw transaction: %s' % tx_hex
```

### Comparing `trezor-0.9.0/PKG-INFO` & `trezor-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: trezor
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python library for communicating with TREZOR Hardware Wallet
 Home-page: https://github.com/trezor/python-trezor
 Author: TREZOR
 Author-email: info@trezor.io
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.3
```


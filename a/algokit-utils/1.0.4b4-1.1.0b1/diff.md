# Comparing `tmp/algokit_utils-1.0.4b4-py3-none-any.whl.zip` & `tmp/algokit_utils-1.1.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31633 bytes, number of entries: 14
--rw-r--r--  2.0 unx     3667 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
--rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
+Zip file size: 32450 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     3767 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+-rw-r--r--  2.0 unx     7366 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     5019 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b4.dist-info/RECORD
-14 files, 121578 bytes uncompressed, 29679 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b1.dist-info/RECORD
+14 files, 125476 bytes uncompressed, 30496 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.4b4.dist-info/LICENSE
+Filename: algokit_utils-1.1.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.4b4.dist-info/METADATA
+Filename: algokit_utils-1.1.0b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.4b4.dist-info/WHEEL
+Filename: algokit_utils-1.1.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.4b4.dist-info/RECORD
+Filename: algokit_utils-1.1.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -1,9 +1,11 @@
 from algokit_utils._transfer import (
+    EnsureBalanceParameters,
     TransferParameters,
+    ensure_funded,
     transfer,
 )
 from algokit_utils.account import (
     create_kmd_wallet_account,
     get_account,
     get_account_from_mnemonic,
     get_dispenser_account,
@@ -140,10 +142,12 @@
     "get_algonode_config",
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
     "is_sandbox",
+    "EnsureBalanceParameters",
     "TransferParameters",
+    "ensure_funded",
     "transfer",
 ]
```

## algokit_utils/_transfer.py

```diff
@@ -8,15 +8,15 @@
 from algosdk.transaction import PaymentTxn, SuggestedParams
 
 from algokit_utils.models import Account
 
 if TYPE_CHECKING:
     from algosdk.v2client.algod import AlgodClient
 
-__all__ = ["TransferParameters", "transfer"]
+__all__ = ["EnsureBalanceParameters", "TransferParameters", "ensure_funded", "transfer"]
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass(kw_only=True)
 class TransferParameters:
     """Parameters for transferring µALGOs between accounts"""
 
@@ -33,14 +33,46 @@
     fee_micro_algos: int | None = None
     """(optional) The flat fee you want to pay, useful for covering extra fees in a transaction group or app call"""
     max_fee_micro_algos: int | None = None
     """(optional)The maximum fee that you are happy to pay (default: unbounded) -
     if this is set it's possible the transaction could get rejected during network congestion"""
 
 
+@dataclasses.dataclass(kw_only=True)
+class EnsureBalanceParameters:
+    """Parameters for ensuring an account has a minimum number of µALGOs"""
+
+    account_to_fund: Account | AccountTransactionSigner | str
+    """The account address that will receive the µALGOs"""
+
+    funding_source: Account | AccountTransactionSigner
+    """The account (with private key) or signer that will send the µALGOs"""
+
+    min_spending_balance_micro_algos: int
+    """The minimum balance of ALGOs that the account should have available to spend (i.e. on top of
+    minimum balance requirement)"""
+
+    min_funding_increment_micro_algos: int = 0
+    """When issuing a funding amount, the minimum amount to transfer (avoids many small transfers if this gets
+    called often on an active account)"""
+
+    suggested_params: SuggestedParams | None = None
+    """(optional) transaction parameters"""
+
+    note: str | bytes | None = None
+    """The (optional) transaction note, default: "Funding account to meet minimum requirement"""
+
+    fee_micro_algos: int | None = None
+    """(optional) The flat fee you want to pay, useful for covering extra fees in a transaction group or app call"""
+
+    max_fee_micro_algos: int | None = None
+    """(optional)The maximum fee that you are happy to pay (default: unbounded) -
+    if this is set it's possible the transaction could get rejected during network congestion"""
+
+
 def _check_fee(transaction: PaymentTxn, max_fee: int | None) -> None:
     if max_fee is not None:
         # Once a transaction has been constructed by algosdk, transaction.fee indicates what the total transaction fee
         # Will be based on the current suggested fee-per-byte value.
         if transaction.fee > max_fee:
             raise Exception(
                 f"Cancelled transaction due to high network congestion fees. "
@@ -78,7 +110,55 @@
     txid = transaction.get_txid()  # type: ignore[no-untyped-call]
     logger.debug(
         f"Sent transaction {txid} type={transaction.type} from "
         f"{address_from_private_key(from_account.private_key)}"  # type: ignore[no-untyped-call]
     )
 
     return transaction
+
+
+def ensure_funded(
+    client: "AlgodClient",
+    parameters: EnsureBalanceParameters,
+) -> None | PaymentTxn:
+    """
+    Funds a given account using a funding source such that it has a certain amount of algos free to spend
+    (accounting for ALGOs locked in minimum balance requirement)
+    see <https://developer.algorand.org/docs/get-details/accounts/#minimum-balance>
+
+    :return None | PaymentTxn: None if balance was sufficient or the payment transaction used to increase the balance
+    """
+    sender_address = address_from_private_key(parameters.funding_source.private_key)  # type: ignore[no-untyped-call]
+    address_to_fund = (
+        parameters.account_to_fund
+        if isinstance(parameters.account_to_fund, str)
+        else address_from_private_key(parameters.account_to_fund.private_key)  # type: ignore[no-untyped-call]
+    )
+
+    account_info = client.account_info(address_to_fund)
+    assert isinstance(account_info, dict)
+
+    balance_micro_algos = account_info.get("amount", 0)
+    minimum_balance_micro_algos = account_info.get("min-balance")
+    current_spending_balance_micro_algos = balance_micro_algos - minimum_balance_micro_algos
+    if parameters.min_spending_balance_micro_algos > current_spending_balance_micro_algos:
+        min_fund_amount_micro_algos = parameters.min_spending_balance_micro_algos - current_spending_balance_micro_algos
+        fund_amount_micro_algos = max(min_fund_amount_micro_algos, parameters.min_funding_increment_micro_algos)
+        logger.info(
+            f"Funding {address_to_fund} {fund_amount_micro_algos}µ from {sender_address} to reach "
+            f"minimum spend amount of {parameters.min_spending_balance_micro_algos}µ (balance = "
+            f"{balance_micro_algos}µ, requirement = {minimum_balance_micro_algos}µ)"
+        )
+        return transfer(
+            client,
+            TransferParameters(
+                from_account=parameters.funding_source,
+                to_address=address_to_fund,
+                micro_algos=fund_amount_micro_algos,
+                note=parameters.note or "Funding account to meet minimum requirement",
+                suggested_params=parameters.suggested_params,
+                max_fee_micro_algos=parameters.max_fee_micro_algos,
+                fee_micro_algos=parameters.fee_micro_algos,
+            ),
+        )
+
+    return None
```

## Comparing `algokit_utils-1.0.4b4.dist-info/LICENSE` & `algokit_utils-1.1.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.4b4.dist-info/METADATA` & `algokit_utils-1.1.0b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.4b4
+Version: 1.1.0b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.0.4b4.dist-info/RECORD` & `algokit_utils-1.1.0b1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-algokit_utils/__init__.py,sha256=9dK3nmp6w9OgS_aEhGwpKp17v7G0IsD6N1Ru9Zfhzrg,3667
-algokit_utils/_transfer.py,sha256=MAu9lLMK_g9GB40X2pb5zzDDsrDkqge1Onx5_CDSwwg,3568
+algokit_utils/__init__.py,sha256=LqrX0lRiO7ZAYprbuh2D-9BlCIrDiY2MqWcQ3BiJJb0,3767
+algokit_utils/_transfer.py,sha256=MhulT8NjKun6LIifHYf-KLBQRx_dTs8ePX3SEh7kmik,7366
 algokit_utils/account.py,sha256=-OQn9mhKxZkgXhab_ugRlKt18LRvK6KxJkH5bhFb-6k,7709
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=Vg5K7xDSp7F8ImwT9FyboZDZFHeq_HeZgZyU26lvjE0,29956
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
 algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
 algokit_utils/network_clients.py,sha256=OvPBtv79bMBPh_Pn0YgS1xkBVKuWl_nGLq42hskpokk,5019
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.4b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.4b4.dist-info/METADATA,sha256=NdxSdv2Q94ATnGCcsdsNyOkUo9S-1W-XUSR3EfkqNX8,2037
-algokit_utils-1.0.4b4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.4b4.dist-info/RECORD,,
+algokit_utils-1.1.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.1.0b1.dist-info/METADATA,sha256=pC9Cb2n6vL8UR8vTQHZQipX2KrUQDa6LSGjwy7K6gR0,2037
+algokit_utils-1.1.0b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.1.0b1.dist-info/RECORD,,
```


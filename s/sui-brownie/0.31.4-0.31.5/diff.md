# Comparing `tmp/sui_brownie-0.31.4-py3-none-any.whl.zip` & `tmp/sui_brownie-0.31.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27601 bytes, number of entries: 16
+Zip file size: 27648 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    91352 b- defN 23-Apr-23 09:38 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    92385 b- defN 23-Apr-25 07:20 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/RECORD
-16 files, 157160 bytes uncompressed, 25459 bytes compressed:  83.8%
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-26 06:07 sui_brownie-0.31.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 06:07 sui_brownie-0.31.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-26 06:07 sui_brownie-0.31.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-26 06:07 sui_brownie-0.31.5.dist-info/RECORD
+16 files, 158193 bytes uncompressed, 25506 bytes compressed:  83.9%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.31.4.dist-info/METADATA
+Filename: sui_brownie-0.31.5.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.31.4.dist-info/WHEEL
+Filename: sui_brownie-0.31.5.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.31.4.dist-info/top_level.txt
+Filename: sui_brownie-0.31.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.31.4.dist-info/RECORD
+Filename: sui_brownie-0.31.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -278,15 +278,16 @@
     def __repr__(self):
         return str(self.abi)
 
     def __call__(self, *args, **kwargs):
         return self.package.project.execute(self.package.package_id, self.abi, *args, **kwargs)
 
     def __getattr__(self, item):
-        assert item in ["simulate", "inspect", "unsafe", "with_gas_coin"], f"{item} attribute not found"
+        assert item in ["simulate", "inspect", "unsafe", "with_gas_coin",
+                        "with_gas_coin_inspect"], f"{item} attribute not found"
         return functools.partial(getattr(self.package.project, item), self.package.package_id, self.abi)
 
 
 class ModuleAttributeDict(AttributeDict):
     def __getattr__(self, item):
         if len(_load_project) == 0:
             return []
@@ -1523,14 +1524,18 @@
             for k in replace_tomls:
                 replace_tomls[k].restore()
             traceback.print_exc()
             raise
         return result
 
 
+def get_project() -> List[SuiObject]:
+    return _load_project
+
+
 class SuiProject:
     def __init__(
             self,
             project_path: Union[Path, str] = Path.cwd(),
             network: str = "sui-testnet"
     ):
         self.project_path = project_path
@@ -2395,14 +2400,45 @@
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction {abi["module_name"]}::{abi["func_name"]}, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module=abi["module_name"], function=abi["func_name"])
 
+    def with_gas_coin_inspect(
+            self,
+            package_id,
+            abi: dict,
+            *arguments,
+            type_arguments: List[str] = None,
+            gas_price=None,
+            gas_budget=None,
+    ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
+        # Construct
+        msg = TransactionBuild.move_call_with_gas_coin(
+            self.account.account_address,
+            package_id,
+            abi,
+            type_arguments,
+            arguments,
+            gas_price=gas_price,
+            gas_budget=gas_budget
+        )
+        tx_bytes = base64.b64encode(msg.value.value.kind.encode).decode("ascii")
+        return self.client.sui_devInspectTransactionBlock(
+            self.account.account_address,
+            tx_bytes,
+            None,
+            None
+        )
+
     def estimate_gas_price(self):
         try:
             result = self.client.suix_getReferenceGasPrice()
             return int(result)
         except Exception as e:
             print(f"Estimate gas price fail:{e}, using default 1000")
             return 1000
```

## Comparing `sui_brownie-0.31.4.dist-info/METADATA` & `sui_brownie-0.31.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.31.4
+Version: 0.31.5
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


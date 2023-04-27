# Comparing `tmp/starknet_devnet-0.5.0a2.tar.gz` & `tmp/starknet_devnet-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.0a2.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.1.tar", max compression
```

## Comparing `starknet_devnet-0.5.0a2.tar` & `starknet_devnet-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1046 2023-04-05 11:29:38.195896 starknet_devnet-0.5.0a2/README.md
--rw-r--r--   0        0        0     1795 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32743 2023-04-05 11:29:38.207896 starknet_devnet-0.5.0a2/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2563 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2130 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/account.py
--rw-r--r--   0        0        0     3784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2692 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    11423 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7067 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    13712 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2167 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2120 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2136 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2375 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     5341 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4958 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0    79264 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     7466 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0     7264 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    23046 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6528 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3075 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     7298 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3328 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    17030 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0      877 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     2851 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1134 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    13802 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/dump.py
--rw-r--r--   0        0        0     5592 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     6872 2023-04-05 11:29:38.211896 starknet_devnet-0.5.0a2/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1732 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     8643 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10193 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     2005 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4275 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/server.py
--rw-r--r--   0        0        0    38350 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/state.py
--rw-r--r--   0        0        0     2113 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11173 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1626 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/udc.py
--rw-r--r--   0        0        0     7968 2023-04-05 11:29:38.215896 starknet_devnet-0.5.0a2/starknet_devnet/util.py
--rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a2/setup.py
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 starknet_devnet-0.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 08:59:02.988418 starknet_devnet-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1054 2023-04-27 08:59:02.988418 starknet_devnet-0.5.1/README.md
+-rw-r--r--   0        0        0     1820 2023-04-27 08:59:03.000419 starknet_devnet-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-04-27 08:59:03.000419 starknet_devnet-0.5.1/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32743 2023-04-27 08:59:03.000419 starknet_devnet-0.5.1/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2833 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2130 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/account.py
+-rw-r--r--   0        0        0     3784 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2692 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12337 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7523 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2228 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2136 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2455 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     5643 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4878 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0    79264 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     7466 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0     7264 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    22110 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6703 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3069 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     6736 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3328 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    23908 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0      877 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     2972 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1134 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    13802 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-04-27 08:59:03.004418 starknet_devnet-0.5.1/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     5592 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     6872 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1732 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     8643 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10193 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2005 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4275 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/server.py
+-rw-r--r--   0        0        0    39151 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11617 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1626 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/udc.py
+-rw-r--r--   0        0        0     7968 2023-04-27 08:59:03.008419 starknet_devnet-0.5.1/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 starknet_devnet-0.5.1/setup.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 starknet_devnet-0.5.1/PKG-INFO
```

### Comparing `starknet_devnet-0.5.0a2/README.md` & `starknet_devnet-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 Aims to mimic Starknet's Alpha testnet, but with simplified functionality.
 
 ## 🌐 Docs
 
 On the following links you can find the documentation of:
 
-- [the latest official release](https://shard-labs.github.io/starknet-devnet/)
-- [the latest master commit (not officially released)](https://github.com/Shard-Labs/starknet-devnet/tree/master/page/docs)
+- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)
+- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)
 
 ## ✏️ Contributing
 
 We ❤️ and encourage all contributions!
 
-[Click here](https://shard-labs.github.io/starknet-devnet/docs/guide/development) for the development guide.
+[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.
 
 ## 🙌 Special Thanks
 
-Special thanks to all the [contributors](https://github.com/Shard-Labs/starknet-devnet/graphs/contributors)!
+Special thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!
```

### Comparing `starknet_devnet-0.5.0a2/pyproject.toml` & `starknet_devnet-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.0a2"
+version = "0.5.1"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
-license = "ISC"
+license = "MIT"
 
 readme = "README.md"
-repository = "https://github.com/Shard-Labs/starknet-devnet"
-homepage = "https://github.com/Shard-Labs/starknet-devnet"
+repository = "https://github.com/0xSpaceShard/starknet-devnet"
+homepage = "https://github.com/0xSpaceShard/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
 cairo-lang = "0.11.0.2"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
-crypto-cpp-py = "~1.2.0"
+crypto-cpp-py = "~1.3.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
 jsonschema = "~4.17.0"
 web3 = "~6.0.0"
+poseidon-py = "~0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "~2.12.2"
 psutil = "~5.9.1"
 pytest-xdist = "~2.5.0"
 pylint-quotes = "~0.2.3"
 black = "~22.6"
 requests = "~2.28"
 isort = "^5.10.1"
 
 [tool.poetry.group.vm.dependencies]
-cairo-rs-py = "~0.1.1"
+cairo-rs-py = "~0.2.0"
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.1/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.1/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.1/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/account.py` & `starknet_devnet-0.5.1/starknet_devnet/account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/account_util.py` & `starknet_devnet-0.5.1/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/accounts.py` & `starknet_devnet-0.5.1/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.1/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.1/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blocks.py` & `starknet_devnet-0.5.1/starknet_devnet/blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,42 +73,41 @@
 # pylint: disable=too-many-instance-attributes
 class DevnetBlocks:
     """This class is used to store the generated blocks of the devnet."""
 
     def __init__(self, origin: Origin, lite=False) -> None:
         self.origin = origin
         self.lite = lite
-        self.__num2block: Dict[int, StarknetBlock] = {}
+        self.__hash2block: Dict[int, StarknetBlock] = {}
         self.__state_updates: Dict[int, BlockStateUpdate] = {}
-        self.__hash2num: Dict[str, int] = {}
+        self.__num2hash: Dict[int, int] = {}
         self.__pending_block: StarknetBlock = None
         self.__pending_state_update: BlockStateUpdate = None
         self.__pending_signatures: Sequence[List[int]] = None
         self.__state_archive = MemoryStateArchive()
 
     async def get_last_block(self) -> StarknetBlock:
         """Returns the last block stored so far."""
-        number_of_blocks = self.get_number_of_blocks()
-        return await self.get_by_number(number_of_blocks - 1)
+        return await self.get_by_number(self.get_number_of_accepted_blocks() - 1)
 
-    def get_number_of_blocks(self) -> int:
-        """Returns the number of blocks stored so far."""
-        return len(self.__num2block) + self.origin.get_number_of_blocks()
+    def get_number_of_accepted_blocks(self) -> int:
+        """Returns the number of not aborted blocks."""
+        return len(self.__num2hash) + self.origin.get_number_of_blocks()
 
     def __assert_block_number_in_range(self, block_number: BlockIdentifier):
         if block_number < 0:
             message = (
                 f"Block number must be a non-negative integer; got: {block_number}."
             )
             raise StarknetDevnetException(
                 code=StarkErrorCode.MALFORMED_REQUEST, message=message
             )
-
-        if block_number >= self.get_number_of_blocks():
-            message = f"Block number too high. There are currently {len(self.__num2block)} blocks; got: {block_number}."
+        number_of_accepted_blocks = self.get_number_of_accepted_blocks()
+        if block_number >= number_of_accepted_blocks:
+            message = f"Block number too high. There are currently {number_of_accepted_blocks} blocks; got: {block_number}."
             raise StarknetDevnetException(
                 code=StarknetErrorCode.BLOCK_NOT_FOUND, message=message
             )
 
     async def get_by_number(self, block_number: Optional[str]) -> StarknetBlock:
         """Returns the block whose block_number is provided"""
         block_number = _parse_block_number(block_number)
@@ -116,70 +115,70 @@
         if block_number == PENDING_BLOCK_ID:
             if self.__pending_block:
                 return self.__pending_block
             # if no pending, default to latest
             block_number = LATEST_BLOCK_ID
 
         if block_number == LATEST_BLOCK_ID:
-            if self.__num2block:
+            if self.__num2hash:
                 return await self.get_last_block()
             return await self.origin.get_block_by_number(block_number)
 
         self.__assert_block_number_in_range(block_number)
-        if block_number in self.__num2block:
-            return self.__num2block[block_number]
+        if block_number in self.__num2hash:
+            return self.__hash2block[self.__num2hash[block_number]]
 
         return await self.origin.get_block_by_number(block_number)
 
     async def get_by_hash(self, block_hash: str) -> StarknetBlock:
         """
         Returns the block with the given block hash.
         """
         numeric_hash = _parse_block_hash(block_hash)
 
-        if numeric_hash in self.__hash2num:
-            block_number = self.__hash2num[int(block_hash, 16)]
-            return await self.get_by_number(block_number)
+        if numeric_hash in self.__hash2block:
+            return self.__hash2block[numeric_hash]
 
         return await self.origin.get_block_by_hash(block_hash)
 
     async def get_state_update(
         self, block_hash: str = None, block_number: Any = None
     ) -> BlockStateUpdate:
         """
         Returns state update for the provided block hash or block number.
         It will return the last state update if block is not provided.
         """
         if block_hash:
             numeric_hash = _parse_block_hash(block_hash)
 
-            if numeric_hash not in self.__hash2num:
+            if numeric_hash not in self.__hash2block:
                 return await self.origin.get_state_update(block_hash=block_hash)
 
-            block_number = self.__hash2num[numeric_hash]
+            block_number = self.__hash2block[numeric_hash].block_number
 
         block_number = _parse_block_number(block_number)
 
         if block_number == PENDING_BLOCK_ID:
             if self.__pending_state_update:
                 return self.__pending_state_update
             # if no pending, default to latest
             block_number = LATEST_BLOCK_ID
 
         # now either an int or "latest"
         if block_number != LATEST_BLOCK_ID:
             self.__assert_block_number_in_range(block_number)
-            if block_number in self.__state_updates:
-                return self.__state_updates[block_number]
+            numeric_hash = self.__num2hash[block_number]
+            if numeric_hash in self.__state_updates:
+                return self.__state_updates[numeric_hash]
 
-            return await self.origin.get_state_update(block_number=block_number)
+            return await self.origin.get_state_update(block_hash=numeric_hash)
 
-        # now we know the block ID is "latest"
+        # now it's the latest
         return (
-            self.__state_updates.get(self.get_number_of_blocks() - 1)
+            self.__state_updates.get((await self.get_last_block()).block_hash)
             or await self.origin.get_state_update()
         )
 
     async def generate_pending(
         self,
         transactions: List[DevnetTransaction],
         state: StarknetState,
@@ -190,15 +189,15 @@
         The method `store_pending` can be used after this method.
         """
         timestamp = state.state.block_info.block_timestamp
         signatures = [tx.get_signature() for tx in transactions or []]
         internal_transactions = [tx.internal_tx for tx in transactions or []]
         transaction_receipts = tuple(tx.get_execution() for tx in transactions or ())
 
-        block_number = self.get_number_of_blocks()
+        block_number = self.get_number_of_accepted_blocks()
         if block_number == 0:
             parent_block_hash = 0
         else:
             last_block = await self.get_last_block()
             parent_block_hash = last_block.block_hash
 
         self.__pending_block = StarknetBlock.create(
@@ -268,41 +267,64 @@
 
         block_dict = self.__pending_block.dump()
 
         block_dict["status"] = BlockStatus.ACCEPTED_ON_L2.name
         state_root = DUMMY_STATE_ROOT
         block_dict["state_root"] = state_root.hex()
 
-        block_number = self.get_number_of_blocks()
+        block_number = self.get_number_of_accepted_blocks()
         block_dict["block_number"] = block_number
 
         if self.lite or is_empty_block:
             block_hash = block_number
         elif block_hash is None:
             block_hash = await self.__calculate_pending_block_hash(
                 state, block_number, state_root
             )
 
         block_dict["block_hash"] = hex(block_hash)
-        self.__hash2num[block_hash] = block_number
+        self.__num2hash[block_number] = block_hash
 
         if self.__pending_state_update is not None:
             self.__pending_state_update = BlockStateUpdate(
                 block_hash=block_hash,
                 old_root=self.__pending_state_update.old_root,
                 new_root=self.__pending_state_update.new_root,
                 state_diff=self.__pending_state_update.state_diff,
             )
-        self.__state_updates[block_number] = self.__pending_state_update
+        self.__state_updates[block_hash] = self.__pending_state_update
         self.__pending_state_update = None
 
         block = StarknetBlock.load(block_dict)
-        self.__num2block[block_number] = block
-        self.__state_archive.store(block_number, state)
+        self.__hash2block[block.block_hash] = block
+        self.__state_archive.store(block_hash, state)
 
         self.__pending_block = None
         self.__pending_signatures = None
         return block
 
-    def get_state(self, block_number: int) -> StarknetState:
+    def get_state(self, block_hash: int) -> StarknetState:
         """Return state at block with `number`"""
-        return self.__state_archive.get(block_number)
+        return self.__state_archive.get(block_hash)
+
+    @staticmethod
+    def get_numeric_hash(block_hash: int):
+        """Get numeric hash."""
+        return _parse_block_hash(block_hash)
+
+    async def abort_latest_block(self, block_hash: str) -> str:
+        """
+        Abort latest block.
+        """
+        numeric_hash = _parse_block_hash(block_hash)
+        block = self.__hash2block[numeric_hash]
+
+        # This is done like this because the block object's properties cannot be modified
+        block_dict = block.dump()
+        block_dict["status"] = BlockStatus.ABORTED.name
+        block_dict["transaction_receipts"] = None
+        del self.__num2hash[block_dict["block_number"]]
+        block_dict["block_number"] = None
+        self.__hash2block[numeric_hash] = StarknetBlock.load(block_dict)
+        self.__state_archive.remove(numeric_hash)
+
+        return block.block_hash
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,7 +217,19 @@
 @base.route("/fork_status", methods=["GET"])
 async def fork_status():
     """Get fork status"""
     config = state.starknet_wrapper.config
     if config.fork_network:
         return jsonify({"url": config.fork_network.url, "block": config.fork_block})
     return jsonify({})
+
+
+@base.route("/abort_blocks", methods=["POST"])
+async def abort_blocks():
+    """Abort blocks and transactions from given block hash to last block."""
+    request_json = request.json or {}
+    starting_block = await state.starknet_wrapper.blocks.get_by_hash(
+        hex(hex_converter(request_json, "startingBlockHash"))
+    )
+    aborted_blocks = await state.starknet_wrapper.abort_blocks(starting_block)
+
+    return jsonify({"aborted": aborted_blocks})
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,21 @@
 
 
 @feeder_gateway.route("/get_block", methods=["GET"])
 async def get_block():
     """Endpoint for retrieving a block identified by its hash or number."""
 
     block = await _get_block_object(request.args)
-    return jsonify(block.dump())
+    block_dump = block.dump()
+
+    # This is a hack to fix StarknetBlock.loads(data=raw_response)
+    if "transaction_receipts" not in block_dump:
+        block_dump["transaction_receipts"] = None
+
+    return jsonify(block_dump)
 
 
 @feeder_gateway.route("/get_block_traces", methods=["GET"])
 async def get_block_traces():
     """Returns the traces of the transactions in the specified block."""
 
     block = await _get_block_object(request.args)
@@ -197,21 +203,25 @@
 
 @feeder_gateway.route("/get_full_contract", methods=["GET"])
 async def get_full_contract():
     """
     Returns the contract class of the contract whose contractAddress is provided.
     """
     block_id = _get_block_id(request.args)
-
     contract_address = request.args.get("contractAddress", type=parse_hex_string)
-
     contract_class = await state.starknet_wrapper.get_class_by_address(
         contract_address, block_id
     )
-    return jsonify(contract_class.remove_debug_info().dump())
+
+    # strip debug_info if cairo 0 class
+    class_program = contract_class.get("program")
+    if class_program and class_program.get("debug_info"):
+        class_program["debug_info"] = None
+
+    return jsonify(contract_class)
 
 
 @feeder_gateway.route("/get_class_hash_at", methods=["GET"])
 async def get_class_hash_at():
     """Get contract class hash by contract address"""
 
     contract_address = request.args.get("contractAddress", type=parse_hex_string)
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/gateway.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Gateway routes
 """
 
 from flask import Blueprint, jsonify, request
+from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.definitions.transaction_type import TransactionType
 from starkware.starkware_utils.error_handling import StarkErrorCode
 
 from starknet_devnet.devnet_config import DumpOn
 from starknet_devnet.state import state
 from starknet_devnet.util import StarknetDevnetException, fixed_length_hex
 
@@ -36,18 +37,18 @@
         (
             contract_address,
             transaction_hash,
         ) = await state.starknet_wrapper.deploy_account(transaction)
         response_dict["address"] = fixed_length_hex(contract_address)
 
     elif tx_type == TransactionType.DEPLOY:
-        contract_address, transaction_hash = await state.starknet_wrapper.deploy(
-            transaction
+        raise StarknetDevnetException(
+            code=StarknetErrorCode.DEPRECATED_TRANSACTION,
+            message="Deploy transaction is no longer supported.",
         )
-        response_dict["address"] = fixed_length_hex(contract_address)
 
     elif tx_type == TransactionType.INVOKE_FUNCTION:
         (contract_address, transaction_hash) = await state.starknet_wrapper.invoke(
             transaction
         )
         response_dict["address"] = fixed_length_hex(contract_address)
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
 
 @validate_schema("blockNumber")
 async def block_number() -> int:
     """
     Get the most recent accepted block number
     """
-    number_of_blocks = state.starknet_wrapper.blocks.get_number_of_blocks()
+    number_of_blocks = state.starknet_wrapper.blocks.get_number_of_accepted_blocks()
     if number_of_blocks == 0:
         raise RpcError.from_spec_name("NO_BLOCKS")
 
     return number_of_blocks - 1
 
 
 @validate_schema("blockHashAndNumber")
 async def block_hash_and_number() -> dict:
     """
     Get the most recent accepted block hash and number
     """
-    number_of_blocks = state.starknet_wrapper.blocks.get_number_of_blocks()
+    number_of_blocks = state.starknet_wrapper.blocks.get_number_of_accepted_blocks()
     if number_of_blocks == 0:
         raise RpcError.from_spec_name("NO_BLOCKS")
 
     last_block_number = number_of_blocks - 1
     last_block = await state.starknet_wrapper.blocks.get_by_number(last_block_number)
 
     result = {
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 async def get_class_at(block_id: BlockId, contract_address: Address) -> dict:
     """
     Get the contract class definition in the given block at the given address
     """
     await assert_block_id_is_valid(block_id)
 
     try:
-        result = await state.starknet_wrapper.get_class_by_address(
+        result_dict = await state.starknet_wrapper.get_class_by_address(
             int(contract_address, 16), block_id
         )
+        contract_class = DeprecatedCompiledClass.load(result_dict)
     except StarkException as ex:
         raise RpcError.from_spec_name("CONTRACT_NOT_FOUND") from ex
 
-    return rpc_contract_class(result)
+    return rpc_contract_class(contract_class)
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     StarknetBlock,
 )
 
 from starknet_devnet.blueprints.rpc.schema import validate_schema
 from starknet_devnet.blueprints.rpc.structures.responses import (
     EmittedEvent,
     RpcEventsResult,
+    RpcEventsResultWithoutContinuationToken,
 )
 from starknet_devnet.blueprints.rpc.structures.types import (
     Address,
     BlockId,
     Felt,
     PredefinedRpcErrorCode,
     RpcError,
@@ -108,15 +109,17 @@
 
     return events_range
 
 
 # pylint: disable=redefined-builtin
 # filter name is determined by current RPC implementation and starknet specification
 @validate_schema("getEvents")
-async def get_events(filter) -> RpcEventsResult:
+async def get_events(
+    filter,
+) -> Union[RpcEventsResult, RpcEventsResultWithoutContinuationToken]:
     """
     Returns all events matching the given filters.
 
     In our implementation continuation_token is just a number.
 
     In state.starknet_wrapper.get_state().events there is no relation between blocks.
     This is why we need to iterate block by block, take all events,
@@ -145,21 +148,25 @@
     for block_number in block_range:
         block = await state.starknet_wrapper.blocks.get_by_number(block_number)
         if block.transaction_receipts:
             events.extend(_get_events_from_block(block, address, keys))
 
     # Chunking
     start_index = continuation_token * chunk_size
-    events = events[start_index : start_index + chunk_size]
+    chunked_events = events[start_index : start_index + chunk_size]
+    remaining_events_length = len(events) - start_index
 
     # Continuation_token should be increased only if events are not empty
-    if events:
+    if remaining_events_length > chunk_size:
         continuation_token = continuation_token + 1
+        return RpcEventsResult(
+            events=chunked_events, continuation_token=str(continuation_token)
+        )
 
-    return RpcEventsResult(events=events, continuation_token=str(continuation_token))
+    return RpcEventsResultWithoutContinuationToken(events=chunked_events)
 
 
 @validate_schema("getNonce")
 async def get_nonce(block_id: BlockId, contract_address: Address) -> Felt:
     """
     Get the nonce associated with the given address in the given block
     """
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     GATEWAY_TO_RPC_ERROR,
     PredefinedRpcErrorCode,
     RpcError,
 )
 from starknet_devnet.blueprints.rpc.transactions import (
     add_declare_transaction,
     add_deploy_account_transaction,
-    add_deploy_transaction,
     add_invoke_transaction,
     estimate_fee,
     get_transaction_by_block_id_and_index,
     get_transaction_by_hash,
     get_transaction_receipt,
     pending_transactions,
 )
@@ -69,15 +68,14 @@
     "chainId": chain_id,
     "pendingTransactions": pending_transactions,
     "syncing": syncing,
     "getEvents": get_events,
     "getNonce": get_nonce,
     "addInvokeTransaction": add_invoke_transaction,
     "addDeclareTransaction": add_declare_transaction,
-    "addDeployTransaction": add_deploy_transaction,
     "addDeployAccountTransaction": add_deploy_account_transaction,
 }
 
 rpc = Blueprint("rpc", __name__, url_prefix="/rpc")
 
 
 @rpc.route("", methods=["POST"])
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     InvokeSpecificInfo,
     L1HandlerSpecificInfo,
     StarknetBlock,
     TransactionSpecificInfo,
     TransactionType,
 )
 from starkware.starknet.services.api.gateway.transaction import (
-    Deploy,
     DeployAccount,
     DeprecatedDeclare,
     InvokeFunction,
 )
 from starkware.starknet.services.api.gateway.transaction_utils import (
     compress_program,
     decompress_program,
@@ -453,39 +452,14 @@
         version=int(declare_transaction["version"], 16),
         max_fee=int(declare_transaction["max_fee"], 16),
         signature=[int(sig, 16) for sig in declare_transaction["signature"]],
     )
     return declare_tx
 
 
-def make_deploy(deploy_transaction: RpcBroadcastedDeployTxn) -> Deploy:
-    """
-    Convert RpcBroadcastedDeployTxn to Deploy
-    """
-    contract_class = deploy_transaction["contract_class"]
-    if "abi" not in contract_class:
-        contract_class["abi"] = []
-
-    try:
-        contract_class["program"] = decompress_program(contract_class["program"])
-        contract_class = DeprecatedCompiledClass.load(contract_class)
-    except (StarkException, TypeError, MarshmallowError) as ex:
-        raise RpcError(code=50, message="Invalid contract class") from ex
-
-    deploy_tx = Deploy(
-        contract_address_salt=int(deploy_transaction["contract_address_salt"], 16),
-        constructor_calldata=[
-            int(data, 16) for data in deploy_transaction["constructor_calldata"]
-        ],
-        contract_definition=contract_class,
-        version=int(deploy_transaction["version"], 16),
-    )
-    return deploy_tx
-
-
 def make_deploy_account(
     deploy_account_transaction: RpcBroadcastedDeployAccountTxn,
 ) -> DeployAccount:
     """
     Convert RpcBroadcastedDeployAccountTxn to DeployAccount
     """
     deploy_account_tx = DeployAccount(
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,22 @@
     TypedDict for rpc get events result
     """
 
     events: List[EmittedEvent]
     continuation_token: str
 
 
+class RpcEventsResultWithoutContinuationToken(TypedDict):
+    """
+    TypedDict for rpc get events result without continuation token
+    """
+
+    events: List[EmittedEvent]
+
+
 class RpcBaseTransactionReceipt(TypedDict):
     """TypedDict for rpc transaction receipt"""
 
     transaction_hash: TxnHash
     actual_fee: Felt
     status: TxnStatus
     block_hash: BlockHash
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,9 +109,9 @@
     INVALID_PARAMS = -32602
     INTERNAL_ERROR = -32603
 
 
 RPC_ERRORS = json.loads(RPC_SPECIFICATION)["components"]["errors"]
 
 GATEWAY_TO_RPC_ERROR = {
-    StarknetErrorCode.OUT_OF_RANGE_BLOCK_ID: RPC_ERRORS["BLOCK_NOT_FOUND"],
+    StarknetErrorCode.BLOCK_NOT_FOUND: RPC_ERRORS["BLOCK_NOT_FOUND"],
 }
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,26 @@
 from starkware.starknet.services.api.gateway.transaction import AccountTransaction
 from starkware.starkware_utils.error_handling import StarkException
 
 from starknet_devnet.blueprints.rpc.schema import validate_schema
 from starknet_devnet.blueprints.rpc.structures.payloads import (
     RpcBroadcastedDeclareTxn,
     RpcBroadcastedDeployAccountTxn,
-    RpcBroadcastedDeployTxn,
     RpcBroadcastedInvokeTxn,
     RpcBroadcastedTxn,
     RpcTransaction,
     make_declare,
-    make_deploy,
     make_deploy_account,
     make_invoke_function,
     rpc_fee_estimate,
     rpc_transaction,
 )
 from starknet_devnet.blueprints.rpc.structures.responses import (
     RpcDeclareTransactionResult,
     RpcDeployAccountTransactionResult,
-    RpcDeployTransactionResult,
     RpcInvokeTransactionResult,
     rpc_transaction_receipt,
 )
 from starknet_devnet.blueprints.rpc.structures.types import BlockId, RpcError, TxnHash
 from starknet_devnet.blueprints.rpc.utils import (
     assert_block_id_is_valid,
     gateway_felt,
@@ -131,30 +128,14 @@
     )
     return RpcDeclareTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
         class_hash=rpc_felt(class_hash),
     )
 
 
-@validate_schema("addDeployTransaction")
-async def add_deploy_transaction(deploy_transaction: RpcBroadcastedDeployTxn) -> dict:
-    """
-    Submit a new deploy contract transaction
-    """
-    deploy_transaction = make_deploy(deploy_transaction)
-
-    contract_address, transaction_hash = await state.starknet_wrapper.deploy(
-        deploy_transaction=deploy_transaction
-    )
-    return RpcDeployTransactionResult(
-        transaction_hash=rpc_felt(transaction_hash),
-        contract_address=rpc_felt(contract_address),
-    )
-
-
 @validate_schema("addDeployAccountTransaction")
 async def add_deploy_account_transaction(
     deploy_account_transaction: RpcBroadcastedDeployAccountTxn,
 ) -> dict:
     """
     Submit a new deploy account transaction
     """
@@ -185,15 +166,15 @@
     """
     txn_type = txn["type"]
     if txn_type == "INVOKE":
         return make_invoke_function(txn)
     if txn_type == "DECLARE":
         return make_declare(txn)
     if txn_type == "DEPLOY":
-        return make_deploy(txn)
+        raise RpcError(code=-1, message="DEPLOY transactions are deprecated")
     if txn_type == "DEPLOY_ACCOUNT":
         return make_deploy_account(txn)
     raise NotImplementedError(f"Unexpected type {txn_type}.")
 
 
 @validate_schema("estimateFee")
 async def estimate_fee(request: RpcBroadcastedTxn, block_id: BlockId) -> dict:
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.1/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.1/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/compiler.py` & `starknet_devnet-0.5.1/starknet_devnet/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,27 @@
         raise NotImplementedError
 
 
 class DefaultContractClassCompiler(ContractClassCompiler):
     """Uses the default internal cairo-lang compiler"""
 
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
-        return compile_contract_class(contract_class)
+        return compile_contract_class(
+            contract_class,
+            compiler_args="--add-pythonic-hints --allowed-libfuncs-list-name experimental_v0.1.0",
+        )
 
 
 class CustomContractClassCompiler(ContractClassCompiler):
     """Uses the compiler according to the compiler_manifest provided in initialization"""
 
     def __init__(self, compiler_manifest: str):
         self.compiler_manifest = compiler_manifest
 
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
-
         with tempfile.TemporaryDirectory() as tmp_dir:
             contract_json = os.path.join(tmp_dir, "contract.json")
             contract_casm = os.path.join(tmp_dir, "contract.casm")
 
             with open(contract_json, mode="w", encoding="utf-8") as tmp_file:
                 contract_class_dumped = contract_class.dump()
                 contract_class_dumped["abi"] = json.loads(contract_class_dumped["abi"])
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/constants.py` & `starknet_devnet-0.5.1/starknet_devnet/constants.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.1/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.1/starknet_devnet/devnet_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/dump.py` & `starknet_devnet-0.5.1/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.1/starknet_devnet/fee_token.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.1/starknet_devnet/forked_state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/general_config.py` & `starknet_devnet-0.5.1/starknet_devnet/general_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/origin.py` & `starknet_devnet-0.5.1/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.1/starknet_devnet/postman_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.1/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/server.py` & `starknet_devnet-0.5.1/starknet_devnet/server.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.1/starknet_devnet/starknet_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=too-many-lines
 """
 This module introduces `StarknetWrapper`, a wrapper class of
 starkware.starknet.testing.starknet.Starknet.
 """
 from copy import deepcopy
 from types import TracebackType
 from typing import Dict, List, Optional, Set, Tuple, Type, Union
@@ -21,22 +22,18 @@
 )
 from starkware.starknet.core.os.contract_address.contract_address import (
     calculate_contract_address_from_hash,
 )
 from starkware.starknet.core.os.contract_class.compiled_class_hash import (
     compute_compiled_class_hash,
 )
-from starkware.starknet.core.os.transaction_hash.transaction_hash import (
-    calculate_deploy_transaction_hash,
-)
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.definitions.transaction_type import TransactionType
 from starkware.starknet.services.api.contract_class.contract_class import (
     CompiledClass,
-    CompiledClassBase,
     ContractClass,
     DeprecatedCompiledClass,
     EntryPointType,
 )
 from starkware.starknet.services.api.feeder_gateway.request_objects import (
     CallFunction,
     CallL1Handler,
@@ -51,15 +48,14 @@
     StateDiff,
     StorageEntry,
     TransactionStatus,
     TransactionTrace,
 )
 from starkware.starknet.services.api.gateway.transaction import (
     Declare,
-    Deploy,
     DeployAccount,
     DeprecatedDeclare,
     InvokeFunction,
 )
 from starkware.starknet.services.api.messages import StarknetMessageToL1
 from starkware.starknet.services.utils.sequencer_api_utils import (
     InternalInvokeFunctionForSimulate,
@@ -111,14 +107,15 @@
     warn,
 )
 
 enable_pickling()
 
 DEFAULT_BLOCK_ID = LATEST_BLOCK_ID
 
+
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-public-methods
 # pylint: disable=too-many-locals
 class StarknetWrapper:
     """
     Wraps a Starknet instance and stores data to be returned by the server:
     contract states, transactions, blocks, storages.
@@ -143,15 +140,15 @@
         self.fee_token = FeeToken(self)
         self.accounts = Accounts(self)
         self.__udc = UDC(self)
         self.pending_txs: List[DevnetTransaction] = []
         self.__latest_state = None
         self._contract_classes: Dict[int, Union[DeprecatedCompiledClass, ContractClass]]
         """If v2 - store sierra, otherwise store old class; needed for get_class_by_hash"""
-
+        self.genesis_block_number = None
         self._compiler = (
             CustomContractClassCompiler(config.cairo_compiler_manifest)
             if config.cairo_compiler_manifest
             else DefaultContractClassCompiler()
         )
 
         if config.start_time is not None:
@@ -212,14 +209,15 @@
             (UDC.HASH, UDC.ADDRESS),
             (self.config.account_class.hash, ChargeableAccount.ADDRESS),
         ]
         for account in self.accounts:
             deploy_data.append((account.class_hash, account.address))
 
         for class_hash, contract_address in deploy_data:
+            # this might be the only place where DEPLOY tx is used
             internal_deploy = create_empty_internal_deploy(
                 transaction_hash, class_hash, contract_address
             )
             deploy_transaction = create_genesis_block_transaction(
                 internal_deploy, TransactionType.DEPLOY
             )
             transactions.append(deploy_transaction)
@@ -227,14 +225,17 @@
 
         self._update_block_number()
         state = self.get_state()
         state_update = await self.update_pending_state()
         await self.blocks.generate_pending(transactions, state, state_update)
         block = await self.generate_latest_block(block_hash=0)
 
+        # Set the genesis block number
+        self.genesis_block_number = block.block_number
+
         for transaction in transactions:
             transaction.set_block(block=block)
             self.transactions.store(transaction.transaction_hash, transaction)
 
     async def create_empty_block(self) -> StarknetBlock:
         """Create empty block."""
         self._update_block_number()
@@ -540,61 +541,14 @@
             )
 
         return (
             account_address,
             tx_handler.internal_tx.hash_value,
         )
 
-    async def deploy(self, deploy_transaction: Deploy) -> Tuple[int, int]:
-        """
-        Deploys the contract specified with `deploy_transaction`.
-        Returns (contract_address, transaction_hash).
-        """
-
-        contract_class = deploy_transaction.contract_definition
-
-        internal_tx: InternalDeploy = InternalDeploy.from_external(
-            deploy_transaction, self.get_state().general_config
-        )
-
-        contract_address = internal_tx.contract_address
-
-        if await self.is_deployed(contract_address):
-            tx_hash = calculate_deploy_transaction_hash(
-                version=deploy_transaction.version,
-                contract_address=contract_address,
-                constructor_calldata=deploy_transaction.constructor_calldata,
-                chain_id=self.get_state().general_config.chain_id.value,
-            )
-            return contract_address, tx_hash
-
-        tx_hash = internal_tx.hash_value
-
-        async with self.__get_transaction_handler(
-            external_tx=deploy_transaction
-        ) as tx_handler:
-            tx_handler.internal_tx = internal_tx
-            state = self.get_state().state
-            state.contract_classes[internal_tx.class_hash] = contract_class
-            self._contract_classes[internal_tx.class_hash] = contract_class
-
-            tx_handler.execution_info = await self.__deploy(internal_tx)
-            tx_handler.internal_calls = (
-                tx_handler.execution_info.call_info.internal_calls
-            )
-
-            tx_handler.deployed_contracts.append(
-                ContractAddressHashPair(
-                    address=contract_address,
-                    class_hash=internal_tx.class_hash,
-                )
-            )
-
-        return contract_address, tx_hash
-
     async def invoke(self, external_tx: InvokeFunction):
         """Perform invoke according to specifications in `transaction`."""
         state = self.get_state()
         async with self.__get_transaction_handler(
             external_tx=external_tx
         ) as tx_handler:
             tx_handler.internal_tx = InternalInvokeFunction.from_external(
@@ -614,22 +568,21 @@
         if block_id == PENDING_BLOCK_ID:
             return self.get_state()
         if block_id == LATEST_BLOCK_ID:
             return self.__latest_state
 
         assert isinstance(block_id, dict)
         if block_id.get("block_hash"):
-            # takes care of parsing
-            block = await self.blocks.get_by_hash(block_id["block_hash"])
-            return self.blocks.get_state(block.block_number)
+            numeric_hash = self.blocks.get_numeric_hash(block_id.get("block_hash"))
+            return self.blocks.get_state(numeric_hash)
 
-        block_number = block_id.get("block_number")
         try:
-            parsed_id = int(block_number)
-            return self.blocks.get_state(parsed_id)
+            block_number = block_id.get("block_number")
+            block = await self.blocks.get_by_number(int(block_number))
+            return self.blocks.get_state(block.block_hash)
         except ValueError:
             pass
 
         raise StarknetDevnetException(
             code=StarknetErrorCode.INVALID_BLOCK_NUMBER,
             message=f"Invalid block id: {block_id}",
         )
@@ -725,30 +678,28 @@
                 code=StarknetErrorCode.UNINITIALIZED_CONTRACT,
                 message=f"Contract with address {contract_address} is not deployed.",
             )
         return class_hash
 
     async def get_class_by_address(
         self, contract_address: int, block_id: BlockId = DEFAULT_BLOCK_ID
-    ) -> CompiledClassBase:
+    ) -> dict:
         """Return contract class given the contract address"""
-        state = await self.__get_query_state(block_id)
-        cached_state = state.state
-        class_hash = await self.get_class_hash_at(contract_address)
-        return cached_state.contract_classes[class_hash]
+        class_hash = await self.get_class_hash_at(contract_address, block_id)
+        return await self.get_class_by_hash(class_hash)
 
     async def get_code(
         self, contract_address: int, block_id: BlockId = DEFAULT_BLOCK_ID
     ) -> dict:
         """Return code dict given the contract address"""
         try:
             contract_class = await self.get_class_by_address(contract_address, block_id)
             result_dict = {
-                "abi": contract_class.abi,
-                "bytecode": contract_class.dump()["program"]["data"],
+                "abi": contract_class["abi"],
+                "bytecode": contract_class["program"]["data"],
             }
         except StarkException as err:
             if err.code != StarknetErrorCode.UNINITIALIZED_CONTRACT:
                 raise
             result_dict = {"abi": {}, "bytecode": []}
 
         return result_dict
@@ -987,7 +938,75 @@
 
     async def is_deployed(self, address: int) -> bool:
         """Check if the contract is deployed."""
         assert isinstance(address, int)
         cached_state = self.get_state().state
         class_hash = await cached_state.get_class_hash_at(address)
         return bool(class_hash)
+
+    async def abort_blocks(self, starting_block: StarknetBlock) -> str:
+        """
+        Abort blocks.
+        """
+        # Check if genesis block can be aborted.
+        if starting_block.block_number == self.genesis_block_number:
+            raise StarknetDevnetException(
+                code=StarknetErrorCode.OUT_OF_RANGE_BLOCK_ID,
+                message="Aborting genesis block is not supported.",
+            )
+
+        # Check if blocks can be aborted in fork mode.
+        if (
+            self.config.fork_block
+            and self.config.fork_block >= starting_block.block_number
+        ):
+            raise StarknetDevnetException(
+                code=StarknetErrorCode.OUT_OF_RANGE_BLOCK_ID,
+                message="Aborting forked blocks is not supported.",
+            )
+
+        # Create new block with pending transactions if possible.
+        # We need to store them so later we can change the status to REJECTED.
+        if self.blocks.is_block_pending():
+            await self.generate_latest_block()
+
+        aborted_blocks = []
+        last_block = await self.blocks.get_last_block()
+
+        # Before the while loop to abort blocks, check if block numbers are set.
+        if not (last_block.block_number and starting_block.block_number):
+            raise StarknetDevnetException(
+                code=StarknetErrorCode.BLOCK_NOT_FOUND,
+                status_code=400,
+                message="Block cannot be aborted. Make sure you are aborting an accepted block.",
+            )
+
+        # Abort blocks from latest to starting (iterating backwards).
+        reached_starting_block = False
+        while not reached_starting_block:
+            reached_starting_block = (
+                last_block.block_number == starting_block.block_number
+            )
+
+            # Abort latest_block.
+            aborted_block_hash = await self.blocks.abort_latest_block(
+                hex(last_block.block_hash)
+            )
+
+            # Reject transactions.
+            for transaction in last_block.transactions:
+                await self.transactions.reject_transaction(
+                    tx_hash=transaction.transaction_hash
+                )
+
+            aborted_blocks.append(hex(aborted_block_hash))
+            parent = await self.blocks.get_by_hash(hex(last_block.parent_block_hash))
+
+            if parent.block_number is not None:
+                last_block = parent
+            else:
+                break
+
+        # Revert state.
+        self.starknet.state = self.blocks.get_state(last_block.block_hash)
+
+        return aborted_blocks
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/state.py` & `starknet_devnet-0.5.1/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.1/starknet_devnet/state_archive.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     Stores Starknet states
     """
 
     def store(self, number: int, state: StarknetState):
         """Store the state under the given number"""
         self._storage_write(number, state)
 
+    def remove(self, number: int):
+        """Remove the state under the given number"""
+        self._storage_remove(number)
+
     def get(self, number: int) -> StarknetState:
         """
         Returns the state stored under `number`.
         Raises if out of range.
         """
         try:
             return self._storage_read(number)
@@ -34,27 +38,33 @@
 
     def _storage_write(self, number: int, state: StarknetState):
         raise NotImplementedError
 
     def _storage_read(self, number: int) -> StarknetState:
         raise NotImplementedError
 
+    def _storage_remove(self, number: int) -> StarknetState:
+        raise NotImplementedError
+
 
 class MemoryStateArchive(StateArchive):
     """
     Stores Starknet states in memory
     """
 
     def __init__(self):
         super().__init__()
         self.__storage = {}
 
     def _storage_write(self, number: int, state: StarknetState):
         self.__storage[number] = state.copy()
 
+    def _storage_remove(self, number: int):
+        del self.__storage[number]
+
     def _storage_read(self, number: int) -> StarknetState:
         return self.__storage[number]
 
 
 class DiskStateArchive(StateArchive):
     """
     Stores Starknet states on disk
@@ -71,7 +81,11 @@
     def _storage_write(self, number: int, state: StarknetState):
         with shelve.open(self.PATH, flag="w") as storage:
             storage[str(number)] = state
 
     def _storage_read(self, number: int) -> StarknetState:
         with shelve.open(self.PATH, flag="r") as storage:
             return storage[str(number)]
+
+    def _storage_remove(self, number: int) -> StarknetState:
+        with shelve.open(self.PATH, flag="w") as storage:
+            del storage[str(number)]
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/transactions.py` & `starknet_devnet-0.5.1/starknet_devnet/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,25 @@
 
         # "tx_failure_reason" will only exist if the transaction was rejected.
         if transaction.status == TransactionStatus.REJECTED:
             status_response["tx_failure_reason"] = tx_info.transaction_failure_reason
 
         return status_response
 
+    async def reject_transaction(self, tx_hash: int):
+        """
+        Reject transaction in aborted block.
+        """
+        self.__instances[tx_hash].status = TransactionStatus.REJECTED
+        self.__instances[tx_hash].block = None
+        self.__instances[tx_hash].transaction_failure_reason = TransactionFailureReason(
+            code=StarknetErrorCode.TRANSACTION_FAILED.name,
+            error_message="Block aborted.",
+        )
+
 
 def create_empty_internal_declare(tx_hash: int, class_hash: int) -> InternalDeclare:
     "Create InternalDeclare used in the genesis block"
     return InternalDeclare(
         hash_value=tx_hash,
         version=0,
         max_fee=0,
```

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/udc.py` & `starknet_devnet-0.5.1/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/starknet_devnet/util.py` & `starknet_devnet-0.5.1/starknet_devnet/util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.0a2/setup.py` & `starknet_devnet-0.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,36 +12,37 @@
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
  'cairo-lang==0.11.0.2',
  'cloudpickle>=2.1.0,<2.2.0',
- 'crypto-cpp-py>=1.2.0,<1.3.0',
+ 'crypto-cpp-py>=1.3.0,<1.4.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
+ 'poseidon-py>=0.1.2,<0.2.0',
  'typing-extensions>=4.3.0,<4.4.0',
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.0a2',
+    'version': '0.5.1',
     'description': 'A local testnet for Starknet',
-    'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://shard-labs.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/Shard-Labs/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://shard-labs.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/Shard-Labs/starknet-devnet/graphs/contributors)!\n',
+    'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/Shard-Labs/starknet-devnet',
+    'url': 'https://github.com/0xSpaceShard/starknet-devnet',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<3.10',
 }
```

### Comparing `starknet_devnet-0.5.0a2/PKG-INFO` & `starknet_devnet-0.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.0a2
+Version: 0.5.1
 Summary: A local testnet for Starknet
-Home-page: https://github.com/Shard-Labs/starknet-devnet
-License: ISC
+Home-page: https://github.com/0xSpaceShard/starknet-devnet
+License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
-Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
 Requires-Dist: cairo-lang (==0.11.0.2)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
-Requires-Dist: crypto-cpp-py (>=1.2.0,<1.3.0)
+Requires-Dist: crypto-cpp-py (>=1.3.0,<1.4.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
+Requires-Dist: poseidon-py (>=0.1.2,<0.2.0)
 Requires-Dist: typing-extensions (>=4.3.0,<4.4.0)
 Requires-Dist: web3 (>=6.0.0,<6.1.0)
-Project-URL: Repository, https://github.com/Shard-Labs/starknet-devnet
+Project-URL: Repository, https://github.com/0xSpaceShard/starknet-devnet
 Description-Content-Type: text/markdown
 
 <!-- logo / title -->
 <p align="center" style="margin-bottom: 0px !important">
   <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">
 </p>
 <h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>
@@ -36,20 +37,20 @@
 
 Aims to mimic Starknet's Alpha testnet, but with simplified functionality.
 
 ## 🌐 Docs
 
 On the following links you can find the documentation of:
 
-- [the latest official release](https://shard-labs.github.io/starknet-devnet/)
-- [the latest master commit (not officially released)](https://github.com/Shard-Labs/starknet-devnet/tree/master/page/docs)
+- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)
+- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)
 
 ## ✏️ Contributing
 
 We ❤️ and encourage all contributions!
 
-[Click here](https://shard-labs.github.io/starknet-devnet/docs/guide/development) for the development guide.
+[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.
 
 ## 🙌 Special Thanks
 
-Special thanks to all the [contributors](https://github.com/Shard-Labs/starknet-devnet/graphs/contributors)!
+Special thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!
```


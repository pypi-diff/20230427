# Comparing `tmp/nonebot_plugin_mystool-0.2.5.tar.gz` & `tmp/nonebot_plugin_mystool-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-0.2.6.tar", max compression
```

## Comparing `nonebot_plugin_mystool-0.2.5.tar` & `nonebot_plugin_mystool-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/LICENSE
--rw-r--r--   0        0        0     3221 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/README.md
--rw-r--r--   0        0        0     1323 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     2077 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/addFriend.py
--rw-r--r--   0        0        0     6914 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    30682 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/bbsAPI.py
--rw-r--r--   0        0        0     7081 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/config.py
--rw-r--r--   0        0        0    15330 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/data.py
--rw-r--r--   0        0        0    22739 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    19698 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/exchangePlan.py
--rw-r--r--   0        0        0    15148 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/gameSign.py
--rw-r--r--   0        0        0     1893 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    14883 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    23277 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/mybMission.py
--rw-r--r--   0        0        0    23633 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0     9755 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    10836 2023-03-29 21:44:22.836148 nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4640 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3262 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/README.md
+-rw-r--r--   0        0        0     1317 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2802 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     2077 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/addFriend.py
+-rw-r--r--   0        0        0     6914 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    30682 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/bbsAPI.py
+-rw-r--r--   0        0        0     7081 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/config.py
+-rw-r--r--   0        0        0    15416 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/data.py
+-rw-r--r--   0        0        0    22802 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    19562 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchangePlan.py
+-rw-r--r--   0        0        0    15148 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/gameSign.py
+-rw-r--r--   0        0        0     1832 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    14883 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    23334 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/mybMission.py
+-rw-r--r--   0        0        0    23937 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0     9755 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    10836 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.6/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-0.2.5/LICENSE` & `nonebot_plugin_mystool-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/README.md` & `nonebot_plugin_mystool-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,136 +67,138 @@
 00000420: 6f74 2d70 6c75 6769 6e2d 6d79 7354 6f6f  ot-plugin-mysToo
 00000430: 6c3f 7374 796c 653d 666f 722d 7468 652d  l?style=for-the-
 00000440: 6261 6467 6522 3e0a 2020 3c2f 613e 0a3c  badge">.  </a>.<
 00000450: 2f64 6976 3e0a 0a23 206d 7973 546f 6f6c  /div>..# mysTool
 00000460: 202d 20e7 b1b3 e6b8 b8e7 a4be e8be 85e5   - .............
 00000470: 8aa9 e5b7 a5e5 85b7 e68f 92e4 bbb6 0a0a  ................
 00000480: 2a2a e789 88e6 9cac 202d 2076 302e 322e  **...... - v0.2.
-00000490: 352a 2a0a 0a23 2323 20f0 9f93 a320 e69b  5**..### .... ..
-000004a0: b4e6 96b0 e586 85e5 aeb9 0a23 2323 2320  ...........#### 
-000004b0: 3230 3233 2e33 2e33 300a 2d20 e4bf aee5  2023.3.30.- ....
-000004c0: a48d e987 8de5 8699 e985 8de7 bdae e696  ................
-000004d0: 87e4 bbb6 2060 706c 7567 696e 436f 6e66  .... `pluginConf
-000004e0: 6967 2e6a 736f 6e60 20e4 b88d e794 9fe6  ig.json` .......
-000004f0: 9588 e79a 84e9 97ae e9a2 980a 2d20 e4bf  ............- ..
-00000500: aee5 a48d e58d 95e8 b4a6 e688 b7e6 8385  ................
-00000510: e586 b5e4 b88b e697 a0e6 b395 e5a2 9ee5  ................
-00000520: 88a0 e585 91e6 8da2 e8ae a1e5 8892 e79a  ................
-00000530: 84e9 97ae e9a2 980a 2d20 e4bf aee5 a48d  ........- ......
-00000540: 2060 2fe5 8591 e68d a260 20e5 91bd e4bb   `/......` .....
-00000550: a4e5 8faf e883 bde4 b88e e585 b6e4 bb96  ................
-00000560: e68f 92e4 bbb6 e591 bde4 bba4 e586 b2e7  ................
-00000570: aa81 e79a 84e9 97ae e9a2 98ef bc8c e590  ................
-00000580: 8ce6 97b6 205b f09f 9497 e794 a8e6 b395  .... [..........
-00000590: e58f 98e6 9bb4 5d28 6874 7470 733a 2f2f  ......](https://
-000005a0: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
-000005b0: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
-000005c0: 696e 2d6d 7973 746f 6f6c 2f77 696b 692f  in-mystool/wiki/
-000005d0: 496e 666f 726d 6174 696f 6e2d 4578 6368  Information-Exch
-000005e0: 616e 6765 23e5 a29e e58a a0e5 88a0 e999  ange#...........
-000005f0: a4e5 8591 e68d a2e8 aea1 e588 9229 0a2d  .............).-
-00000600: 20e7 b2be e7ae 80e6 8ea5 e694 b6e7 9a84   ...............
-00000610: e591 bde4 bba4 0a2d 20e6 9bb4 e6ad a320  .......- ...... 
-00000620: 6064 6576 6963 655f 7361 7665 6020 22e8  `device_save` ".
-00000630: aebe e5a4 87e4 bf9d e5ad 9822 20e6 97a5  ..........." ...
-00000640: e5bf 97e6 9687 e69c ace7 9a84 e994 99e8  ................
-00000650: afaf 0a0a 2323 2323 2032 3032 332e 332e  ....#### 2023.3.
-00000660: 3138 0a2d 20e5 a29e e58a a0e5 afbc e587  18.- ...........
-00000670: ba43 6f6f 6b69 6573 e58a 9fe8 83bd 0a2d  .Cookies.......-
-00000680: 20e5 a29e e58a a0e5 88a0 e999 a4e8 b4a6   ...............
-00000690: e58f b7e6 95b0 e68d aee5 8a9f e883 bd0a  ................
-000006a0: 2d20 e59c a8e7 94a8 e688 b7e6 8980 e69c  - ..............
-000006b0: 89e8 b4a6 e58f b7e9 83bd e799 bbe5 bd95  ................
-000006c0: e5a4 b1e6 9588 e79a 84e6 8385 e586 b5e4  ................
-000006d0: b88b e585 b3e9 97ad e980 9ae7 9fa5 0a2d  ...............-
-000006e0: 20e4 bfae e5a4 8de5 8e9f e7a5 9ee6 b8b8   ...............
-000006f0: e688 8fe7 adbe e588 b0e5 a4b1 e8b4 a5e9  ................
-00000700: 97ae e9a2 980a 2d20 e8a7 84e8 8c83 e58c  ......- ........
-00000710: 96e4 bba3 e7a0 810a 0a23 2323 2320 3230  .........#### 20
-00000720: 3233 2e31 2e31 370a 2d20 e4bf aee5 a48d  23.1.17.- ......
-00000730: e7be a4e8 818a e4b8 ade6 898b e58a a8e7  ................
-00000740: adbe e588 b0e4 b88d e4bc 9ae6 a8a1 e7b3  ................
-00000750: 8ae5 a484 e790 86e6 898b e69c bae5 8fb7  ................
-00000760: e79a 84e9 97ae e9a2 980a 2d20 e985 8de7  ..........- ....
-00000770: bdae e4b8 ade5 8faf e68e a7e5 88b6 e58a  ................
-00000780: a0e5 a5bd e58f 8be6 98af e590 a6e5 8f91  ................
-00000790: e980 81e6 aca2 e8bf 8ee4 bba5 e58f 8ae4  ................
-000007a0: bdbf e794 a8e6 8c87 e5bc 95e4 bfa1 e681  ................
-000007b0: af0a 2d20 e585 a5e7 bea4 e590 8ee4 b88d  ..- ............
-000007c0: e586 8de8 87aa e58a a8e5 8f91 e980 81e6  ................
-000007d0: aca2 e8bf 8ee4 bfa1 e681 af0a 0a23 2323  .............###
-000007e0: 2320 3230 3232 2e31 322e 3234 0a2d 20e6  # 2022.12.24.- .
-000007f0: 94af e68c 81e7 bea4 e881 8ae4 bdbf e794  ................
-00000800: a80a 0a23 2320 e58a 9fe8 83bd e592 8ce7  ...## ..........
-00000810: 89b9 e680 a70a 0a2d 20e7 9fad e4bf a1e9  .......- .......
-00000820: aa8c e8af 81e7 99bb e5bd 95ef bc8c e585  ................
-00000830: 8de6 8a93 e58c 85e8 8eb7 e58f 9620 436f  ............. Co
-00000840: 6f6b 6965 0a2d 20e8 87aa e58a a8e5 ae8c  okie.- .........
-00000850: e688 90e6 af8f e697 a5e7 b1b3 e6b8 b8e5  ................
-00000860: b881 e4bb bbe5 8aa1 0a2d 20e8 87aa e58a  .........- .....
-00000870: a8e8 bf9b e8a1 8ce6 b8b8 e688 8fe7 adbe  ................
-00000880: e588 b00a 2d20 e58f afe5 88b6 e5ae 9ae7  ....- ..........
-00000890: b1b3 e6b8 b8e5 b881 e595 86e5 9381 e585  ................
-000008a0: 91e6 8da2 e8ae a1e5 8892 efbc 8ce5 88b0  ................
-000008b0: e782 b9e5 8591 e68d a20a 2d20 e58f afe6  ..........- ....
-000008c0: 94af e68c 81e5 a49a e4b8 aa20 5151 20e8  ........... QQ .
-000008d0: b4a6 e58f b7ef bc8c e6af 8fe4 b8aa 2051  .............. Q
-000008e0: 5120 e8b4 a6e5 8fb7 e58f afe7 bb91 e5ae  Q ..............
-000008f0: 9ae5 a49a e4b8 aae7 b1b3 e593 88e6 b8b8  ................
-00000900: e8b4 a6e6 88b7 0a2d 2051 5120 e68e a8e9  .......- QQ ....
-00000910: 8081 e689 a7e8 a18c e7bb 93e6 9e9c e980  ................
-00000920: 9ae7 9fa5 0a2d 20e5 8e9f e7a5 9ee6 a091  .....- .........
-00000930: e884 82e3 8081 e6b4 9ee5 a4a9 e5ae 9de9  ................
-00000940: 92b1 e380 81e8 b4a8 e987 8fe5 8f82 e58f  ................
-00000950: 98e4 bbaa e5b7 b2e6 bba1 e697 b6e6 8ea8  ................
-00000960: e980 81e9 809a e79f a50a 0a23 2320 e4bd  ...........## ..
-00000970: bfe7 94a8 e8af b4e6 988e 0a0a 2323 2320  ............### 
-00000980: f09f 9ba0 efb8 8f20 4e6f 6e65 426f 7432  ....... NoneBot2
-00000990: 20e6 9cba e599 a8e4 baba e983 a8e7 bdb2   ...............
-000009a0: e592 8ce6 8f92 e4bb b6e5 ae89 e8a3 850a  ................
-000009b0: 0ae8 afb7 e69f a5e7 9c8b 202d 3e20 5bf0  .......... -> [.
-000009c0: 9f94 9749 6e73 7461 6c6c 6174 696f 6e5d  ...Installation]
-000009d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009e0: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-000009f0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000a00: 6f6f 6c2f 7769 6b69 2f49 6e73 7461 6c6c  ool/wiki/Install
-00000a10: 6174 696f 6e29 0a0a 2323 2320 f09f 9396  ation)..### ....
-00000a20: 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4 bdbf   ...............
-00000a30: e794 a8e8 afb4 e698 8e0a 0ae8 afb7 e69f  ................
-00000a40: a5e7 9c8b 202d 3e20 5bf0 9f94 9757 696b  .... -> [....Wik
-00000a50: 6920 e696 87e6 a1a3 5d28 6874 7470 733a  i ......](https:
-00000a60: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-00000a70: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00000a80: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-00000a90: 6929 0a0a 2323 2320 e29d 9320 e88e b7e5  i)..### ... ....
-00000aa0: 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9 e4bf  ................
-00000ab0: a1e6 81af 0a0a 2323 2323 20e6 8f92 e4bb  ......#### .....
-00000ac0: b6e5 91bd e4bb a40a 0a60 6060 0a2f e5b8  .........```./..
-00000ad0: aee5 8aa9 0a60 6060 0a0a 3e20 e29a a0ef  .....```..> ....
-00000ae0: b88f 20e6 b3a8 e684 8f20 e6ad a4e5 a484  .. ...... ......
-00000af0: e6b2 a1e6 9c89 e4bd bfe7 94a8 205b f09f  ............ [..
-00000b00: 9497 20e6 8f92 e4bb b6e5 91bd e4bb a4e5  .. .............
-00000b10: a4b4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000b20: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000b30: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000b40: 7973 746f 6f6c 2f77 696b 692f 436f 6e66  ystool/wiki/Conf
-00000b50: 6967 7572 6174 696f 6e2d 436f 6e66 6967  iguration-Config
-00000b60: 2363 6f6d 6d61 6e64 5f73 7461 7274 290a  #command_start).
-00000b70: 0a23 2320 e585 b6e4 bb96 0a0a 2323 2320  .## ........### 
-00000b80: 5bf0 9f93 83e6 ba90 e7a0 81e8 afb4 e698  [...............
-00000b90: 8e5d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-00000ba0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000bb0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000bc0: 7374 6f6f 6c2f 7769 6b69 2f53 6f75 7263  stool/wiki/Sourc
-00000bd0: 652d 5374 7275 6374 7572 6529 0a23 2323  e-Structure).###
-00000be0: 20e9 8082 e985 8d20 5be7 bbaa e5b1 b1e7   ...... [.......
-00000bf0: 9c9f e5af bb42 6f74 5d28 6874 7470 733a  .....Bot](https:
-00000c00: 2f2f 6769 7468 7562 2e63 6f6d 2f48 6962  //github.com/Hib
-00000c10: 694b 6965 722f 7a68 656e 7875 6e5f 626f  iKier/zhenxun_bo
-00000c20: 7429 20e7 9a84 e588 86e6 94af 0a2d 2068  t) ..........- h
-00000c30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000c40: 6d2f 4d57 544a 432f 7a68 656e 7875 6e2d  m/MWTJC/zhenxun-
-00000c50: 706c 7567 696e 2d6d 7973 746f 6f6c 0a2d  plugin-mystool.-
-00000c60: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000c70: 636f 6d2f 6179 616b 6173 756b 692f 6e6f  com/ayakasuki/no
-00000c80: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000c90: 746f 6f6c 0a                             tool.
+00000490: 362a 2a0a 0a23 2323 20f0 9f93 a320 e69b  6**..### .... ..
+000004a0: b4e6 96b0 e586 85e5 aeb9 0a0a 2323 2323  ............####
+000004b0: 2032 3032 332e 342e 3238 0a2d 20e4 bfae   2023.4.28.- ...
+000004c0: e5a4 8de6 8f92 e4bb b6e5 91bd e4bb a4e8  ................
+000004d0: a2ab e585 b6e4 bb96 206e 6f6e 6562 6f74  ........ nonebot
+000004e0: 20e6 8f92 e4bb b6e6 8d95 e88e b7e7 9a84   ...............
+000004f0: e997 aee9 a298 0a2d 20e5 a29e e58a a0e6  .......- .......
+00000500: 94af e68c 81e6 989f e7a9 b9e9 9381 e981  ................
+00000510: 93e7 9a84 e595 86e5 9381 e585 91e6 8da2  ................
+00000520: 0a2d 20e6 af8f e697 a5e7 adbe e588 b0e3  .- .............
+00000530: 8081 e7b1 b3e6 b8b8 e5b8 81e4 bbbb e58a  ................
+00000540: a1e6 89a7 e8a1 8ce6 97b6 e997 b4e5 9ca8  ................
+00000550: e794 a8e6 88b7 e985 8de7 bdae e79a 84e5  ................
+00000560: 9fba e7a1 80e4 b88a e5a2 9ee5 8aa0 e99a  ................
+00000570: 8fe6 9cba e5bb b6e8 bf9f 0a2d 20e4 bfae  ...........- ...
+00000580: e5a4 8de5 a4a7 e588 abe9 878e e9a2 91e9  ................
+00000590: 8193 e6af 8fe6 97a5 e4bb bbe5 8aa1 e380  ................
+000005a0: 81e7 adbe e588 b0e6 89a7 e8a1 8ce5 a4b1  ................
+000005b0: e8b4 a5e7 9a84 e997 aee9 a298 0a0a 2323  ..............##
+000005c0: 2323 2032 3032 332e 332e 3330 0a2d 20e4  ## 2023.3.30.- .
+000005d0: bfae e5a4 8de9 878d e586 99e9 858d e7bd  ................
+000005e0: aee6 9687 e4bb b620 6070 6c75 6769 6e43  ....... `pluginC
+000005f0: 6f6e 6669 672e 6a73 6f6e 6020 e4b8 8de7  onfig.json` ....
+00000600: 949f e695 88e7 9a84 e997 aee9 a298 0a2d  ...............-
+00000610: 20e4 bfae e5a4 8de5 8d95 e8b4 a6e6 88b7   ...............
+00000620: e683 85e5 86b5 e4b8 8be6 97a0 e6b3 95e5  ................
+00000630: a29e e588 a0e5 8591 e68d a2e8 aea1 e588  ................
+00000640: 92e7 9a84 e997 aee9 a298 0a2d 20e4 bfae  ...........- ...
+00000650: e5a4 8d20 602f e585 91e6 8da2 6020 e591  ... `/......` ..
+00000660: bde4 bba4 e58f afe8 83bd e4b8 8ee5 85b6  ................
+00000670: e4bb 96e6 8f92 e4bb b6e5 91bd e4bb a4e5  ................
+00000680: 86b2 e7aa 81e7 9a84 e997 aee9 a298 efbc  ................
+00000690: 8ce5 908c e697 b620 5bf0 9f94 97e7 94a8  ....... [.......
+000006a0: e6b3 95e5 8f98 e69b b45d 2868 7474 7073  .........](https
+000006b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+000006c0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+000006d0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+000006e0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d45  ki/Information-E
+000006f0: 7863 6861 6e67 6523 e5a2 9ee5 8aa0 e588  xchange#........
+00000700: a0e9 99a4 e585 91e6 8da2 e8ae a1e5 8892  ................
+00000710: 290a 2d20 e7b2 bee7 ae80 e68e a5e6 94b6  ).- ............
+00000720: e79a 84e5 91bd e4bb a40a 2d20 e69b b4e6  ..........- ....
+00000730: ada3 2060 6465 7669 6365 5f73 6176 6560  .. `device_save`
+00000740: 2022 e8ae bee5 a487 e4bf 9de5 ad98 2220   "............" 
+00000750: e697 a5e5 bf97 e696 87e6 9cac e79a 84e9  ................
+00000760: 9499 e8af af0a 0a23 2323 2320 3230 3233  .......#### 2023
+00000770: 2e33 2e31 380a 2d20 e5a2 9ee5 8aa0 e5af  .3.18.- ........
+00000780: bce5 87ba 436f 6f6b 6965 73e5 8a9f e883  ....Cookies.....
+00000790: bd0a 2d20 e5a2 9ee5 8aa0 e588 a0e9 99a4  ..- ............
+000007a0: e8b4 a6e5 8fb7 e695 b0e6 8dae e58a 9fe8  ................
+000007b0: 83bd 0a2d 20e5 9ca8 e794 a8e6 88b7 e689  ...- ...........
+000007c0: 80e6 9c89 e8b4 a6e5 8fb7 e983 bde7 99bb  ................
+000007d0: e5bd 95e5 a4b1 e695 88e7 9a84 e683 85e5  ................
+000007e0: 86b5 e4b8 8be5 85b3 e997 ade9 809a e79f  ................
+000007f0: a50a 2d20 e4bf aee5 a48d e58e 9fe7 a59e  ..- ............
+00000800: e6b8 b8e6 888f e7ad bee5 88b0 e5a4 b1e8  ................
+00000810: b4a5 e997 aee9 a298 0a2d 20e8 a784 e88c  .........- .....
+00000820: 83e5 8c96 e4bb a3e7 a081 0a0a 2323 20e5  ............## .
+00000830: 8a9f e883 bde5 928c e789 b9e6 80a7 0a0a  ................
+00000840: 2d20 e79f ade4 bfa1 e9aa 8ce8 af81 e799  - ..............
+00000850: bbe5 bd95 efbc 8ce5 858d e68a 93e5 8c85  ................
+00000860: e88e b7e5 8f96 2043 6f6f 6b69 650a 2d20  ...... Cookie.- 
+00000870: e887 aae5 8aa8 e5ae 8ce6 8890 e6af 8fe6  ................
+00000880: 97a5 e7b1 b3e6 b8b8 e5b8 81e4 bbbb e58a  ................
+00000890: a10a 2d20 e887 aae5 8aa8 e8bf 9be8 a18c  ..- ............
+000008a0: e6b8 b8e6 888f e7ad bee5 88b0 0a2d 20e5  .............- .
+000008b0: 8faf e588 b6e5 ae9a e7b1 b3e6 b8b8 e5b8  ................
+000008c0: 81e5 9586 e593 81e5 8591 e68d a2e8 aea1  ................
+000008d0: e588 92ef bc8c e588 b0e7 82b9 e585 91e6  ................
+000008e0: 8da2 0a2d 20e5 8faf e694 afe6 8c81 e5a4  ...- ...........
+000008f0: 9ae4 b8aa 2051 5120 e8b4 a6e5 8fb7 efbc  .... QQ ........
+00000900: 8ce6 af8f e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
+00000910: b7e5 8faf e7bb 91e5 ae9a e5a4 9ae4 b8aa  ................
+00000920: e7b1 b3e5 9388 e6b8 b8e8 b4a6 e688 b70a  ................
+00000930: 2d20 5151 20e6 8ea8 e980 81e6 89a7 e8a1  - QQ ...........
+00000940: 8ce7 bb93 e69e 9ce9 809a e79f a50a 2d20  ..............- 
+00000950: e58e 9fe7 a59e e6a0 91e8 8482 e380 81e6  ................
+00000960: b49e e5a4 a9e5 ae9d e992 b1e3 8081 e8b4  ................
+00000970: a8e9 878f e58f 82e5 8f98 e4bb aae5 b7b2  ................
+00000980: e6bb a1e6 97b6 e68e a8e9 8081 e980 9ae7  ................
+00000990: 9fa5 0a0a 2323 20e4 bdbf e794 a8e8 afb4  ....## .........
+000009a0: e698 8e0a 0a23 2323 20f0 9f9b a0ef b88f  .....### .......
+000009b0: 204e 6f6e 6542 6f74 3220 e69c bae5 99a8   NoneBot2 ......
+000009c0: e4ba bae9 83a8 e7bd b2e5 928c e68f 92e4  ................
+000009d0: bbb6 e5ae 89e8 a385 0a0a e8af b7e6 9fa5  ................
+000009e0: e79c 8b20 2d3e 205b f09f 9497 496e 7374  ... -> [....Inst
+000009f0: 616c 6c61 7469 6f6e 5d28 6874 7470 733a  allation](https:
+00000a00: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
+00000a10: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
+00000a20: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
+00000a30: 692f 496e 7374 616c 6c61 7469 6f6e 290a  i/Installation).
+00000a40: 0a23 2323 20f0 9f93 9620 e68f 92e4 bbb6  .### .... ......
+00000a50: e585 b7e4 bd93 e4bd bfe7 94a8 e8af b4e6  ................
+00000a60: 988e 0a0a e8af b7e6 9fa5 e79c 8b20 2d3e  ............. ->
+00000a70: 205b f09f 9497 5769 6b69 20e6 9687 e6a1   [....Wiki .....
+00000a80: a35d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+00000a90: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000aa0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000ab0: 7374 6f6f 6c2f 7769 6b69 290a 0a23 2323  stool/wiki)..###
+00000ac0: 20e2 9d93 20e8 8eb7 e58f 96e6 8f92 e4bb   ... ...........
+00000ad0: b6e5 b8ae e58a a9e4 bfa1 e681 af0a 0a23  ...............#
+00000ae0: 2323 2320 e68f 92e4 bbb6 e591 bde4 bba4  ### ............
+00000af0: 0a0a 6060 600a 2fe5 b8ae e58a a90a 6060  ..```./.......``
+00000b00: 600a 0a3e 20e2 9aa0 efb8 8f20 e6b3 a8e6  `..> ...... ....
+00000b10: 848f 20e6 ada4 e5a4 84e6 b2a1 e69c 89e4  .. .............
+00000b20: bdbf e794 a820 5bf0 9f94 9720 e68f 92e4  ..... [.... ....
+00000b30: bbb6 e591 bde4 bba4 e5a4 b45d 2868 7474  ...........](htt
+00000b40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000b50: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000b60: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000b70: 7769 6b69 2f43 6f6e 6669 6775 7261 7469  wiki/Configurati
+00000b80: 6f6e 2d43 6f6e 6669 6723 636f 6d6d 616e  on-Config#comman
+00000b90: 645f 7374 6172 7429 0a0a 2323 20e5 85b6  d_start)..## ...
+00000ba0: e4bb 960a 0a23 2323 205b f09f 9383 e6ba  .....### [......
+00000bb0: 90e7 a081 e8af b4e6 988e 5d28 6874 7470  ..........](http
+00000bc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000bd0: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00000be0: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00000bf0: 696b 692f 536f 7572 6365 2d53 7472 7563  iki/Source-Struc
+00000c00: 7475 7265 290a 2323 2320 e980 82e9 858d  ture).### ......
+00000c10: 205b e7bb aae5 b1b1 e79c 9fe5 afbb 426f   [............Bo
+00000c20: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000c30: 622e 636f 6d2f 4869 6269 4b69 6572 2f7a  b.com/HibiKier/z
+00000c40: 6865 6e78 756e 5f62 6f74 2920 e79a 84e5  henxun_bot) ....
+00000c50: 8886 e694 af0a 2d20 6874 7470 733a 2f2f  ......- https://
+00000c60: 6769 7468 7562 2e63 6f6d 2f4d 5754 4a43  github.com/MWTJC
+00000c70: 2f7a 6865 6e78 756e 2d70 6c75 6769 6e2d  /zhenxun-plugin-
+00000c80: 6d79 7374 6f6f 6c0a 2d20 6874 7470 733a  mystool.- https:
+00000c90: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7961  //github.com/aya
+00000ca0: 6b61 7375 6b69 2f6e 6f6e 6562 6f74 2d70  kasuki/nonebot-p
+00000cb0: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a       lugin-mystool.
```

### Comparing `nonebot_plugin_mystool-0.2.5/pyproject.toml` & `nonebot_plugin_mystool-0.2.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v0.2.5"
+version = "v0.2.6"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
@@ -20,21 +20,21 @@
 ]
 packages = [
     { include = "nonebot_plugin_mystool", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-httpx = "~=0.23.3"
+httpx = "^0.24.0"
 nonebot_plugin_apscheduler = ">=0.2.0"
-ntplib = "~=0.4.0"
-Pillow = "~=9.4.0"
-requests = "~=2.28.2"
-nonebot_adapter_onebot = ">=2.1.3"
-tenacity = "~=8.2.2"
+ntplib = "^0.4.0"
+Pillow = "^9.5.0"
+requests = "^2.29.0"
+nonebot_adapter_onebot = "^2.2.3"
+tenacity = "^8.2.2"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.5**
+**版本 - v0.2.6**
 
 ## 使用说明
 
 ### 🛠️ NoneBot2 机器人部署和插件安装
 
 请查看 -> [🔗Installation](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Installation)
 
@@ -35,15 +35,15 @@
 import pkgutil
 from pathlib import Path
 
 from nonebot.plugin import PluginMetadata
 
 from .data import create_files
 
-VERSION = "v0.2.5"
+VERSION = "v0.2.6"
 '''插件版本号'''
 
 __plugin_meta__ = PluginMetadata(
     name=f"❖米游社小助手插件❖\n版本 - {VERSION}\n",
     description="米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录\n",
     usage="""
     \n🔐 {HEAD}登录 ➢ 登录绑定米游社账户\
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/addFriend.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/addFriend.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/bbsAPI.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/bbsAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/config.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/data.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,27 +109,30 @@
 class AccountUID:
     """
     米哈游游戏UID数据
     """
 
     def __init__(self) -> None:
         self.ys: str = ""
+        self.xq: str = ""
         self.bh3: str = ""
         self.bh2: str = ""
         self.wd: str = ""
 
     def get(self, uid: Dict[str, str]):
         self.ys: str = uid["ys"]
+        self.xq: str = uid["xq"]
         self.bh3: str = uid["bh3"]
         self.bh2: str = uid["bh2"]
         self.wd: str = uid["wd"]
 
     def to_dict(self) -> Dict[str, str]:
         return {
             "ys": self.ys,
+            "xq": self.xq,
             "bh3": self.bh3,
             "bh2": self.bh2,
             "wd": self.wd,
         }
 
 
 class UserAccount:
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,28 +218,30 @@
         logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
         logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
     except Exception:
         logger.error(f"{conf.LOG_HEAD}米游币商品兑换 - 获取商品详细信息: 网络请求失败")
         logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
 
 
-async def get_good_list(game: Literal["bh3", "ys", "bh2", "wd", "bbs"], retry: bool = True) -> Optional[List[Good]]:
+async def get_good_list(game: Literal["bh3", "ys", "bh2", "wd", "bbs", "xq"], retry: bool = True) -> Optional[List[Good]]:
     """
     获取商品信息列表，若获取失败则返回`None`
 
     :param game: 游戏简称
     :param retry: 是否允许重试
     :return: 商品信息列表
     """
     if game == "bh3":
         game = "bh3"
     elif game == "ys":
         game = "hk4e"
     elif game == "bh2":
         game = "bh2"
+    elif game == "xq":
+        game = "hkrpg"
     elif game == "wd":
         game = "nxx"
     elif game == "bbs":
         game = "bbs"
 
     good_list = []
     page = 1
@@ -283,15 +285,15 @@
     return result
 
 
 class Exchange:
     """
     米游币商品兑换相关(需两步初始化对象，先`__init__`，后异步`async_init`)\n
     示例:
-    `exchange = await Exchange(account, good_id, game_uid).async_init()`
+    >>> exchange = await Exchange(account, good_id, game_uid).async_init()
 
     - `result`属性为 `-1`: 用户登录失效，放弃兑换
     - `result`属性为 `-2`: 商品为游戏内物品，由于未配置stoken，放弃兑换
     - `result`属性为 `-3`: 商品为游戏内物品，由于stoken为\"v2\"类型，且未配置mid，放弃兑换
     - `result`属性为 `-4`: 暂不支持商品所属的游戏，放弃兑换
     - `result`属性为 `-5`: 获取商品的信息时，网络请求失败或服务器没有正确返回，放弃兑换
     - `result`属性为 `-6`: 获取用户游戏账户数据失败，放弃兑换
@@ -369,15 +371,15 @@
                     else:
                         if self.content["address_id"] is None:
                             logger.error(
                                 f"{conf.LOG_HEAD}米游币商品兑换 - 初始化兑换任务: 商品 {self.goodID} 为实体物品，由于未配置地址ID，放弃兑换")
                             self.result = -7
                         return self
 
-                    if good_info["game"] not in ("bh3", "hk4e", "bh2", "nxx"):
+                    if good_info["game"] not in ("bh3", "hk4e", "bh2", "nxx", "hkrpg"):
                         logger.warning(
                             f"{conf.LOG_HEAD}米游币商品兑换 - 初始化兑换任务: 暂不支持商品 {self.goodID} 所属的游戏")
                         self.result = -4
                         return self
 
                     record_list: List[GameRecord] = await get_game_record(self.account)
                     if record_list == -1:
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/exchangePlan.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchangePlan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,421 +1,425 @@
-"""
-### 米游社商品兑换前端以及计划任务相关
-"""
-import asyncio
-import io
-import os
-import time
-from copy import deepcopy
-from datetime import datetime
-from typing import List, Set, Union
-
-from nonebot import get_bot, on_command
-from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
-                                         PrivateMessageEvent, GroupMessageEvent)
-from nonebot.adapters.onebot.v11.message import Message
-from nonebot.matcher import Matcher
-from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
-from nonebot_plugin_apscheduler import scheduler
-
-from .bbsAPI import get_game_record
-from .config import config as conf
-from .data import UserData
-from .exchange import (Exchange, Good, UserAccount, get_good_detail,
-                       get_good_list, game_list_to_image)
-from .gameSign import GameInfo
-from .utils import NtpTime, COMMAND_BEGIN, logger, driver, get_last_command_sep
-
-
-class ExchangeStart:
-    """
-    异步多线程兑换
-    """
-
-    def __init__(self, account: UserAccount, qq: int, exchange_plan: Exchange, thread: int) -> None:
-        self.plans: List[Exchange] = []
-        self.tasks: Set[asyncio.Task] = set()
-        self.finishedCount = 0
-        self.account = account
-        self.qq = qq
-
-        for _ in range(thread):
-            self.plans.append(deepcopy(exchange_plan))
-
-    async def start(self):
-        """
-        执行兑换
-        """
-        # 在后台启动兑换操作
-        for plan in self.plans:
-            self.tasks.add(asyncio.create_task(plan.start()))
-        # 等待兑换线程全部结束
-        for task in self.tasks:
-            await task
-
-        bot = get_bot()
-
-        success_tasks: List[asyncio.Task] = list(filter(lambda task: isinstance(
-            task.result(), tuple) and task.result()[0], self.tasks))
-        if success_tasks:
-            await bot.send_private_msg(
-                user_id=self.qq, message=f"🎉用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换成功，可前往米游社查看")
-        else:
-            msg = f"⚠️用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换失败\n返回结果：\n"
-            num = 0
-            for task in self.tasks:
-                num += 1
-                msg += f"{num}: "
-                if isinstance(task.result(), tuple):
-                    msg += str(task.result()[1])
-                else:
-                    msg += f"异常，程序返回结果为 {task.result()}"
-                msg += "\n"
-            await bot.send_private_msg(user_id=self.qq, message=msg)
-        for plan in self.account.exchange:
-            if plan == (self.plans[0].goodID, self.plans[0].gameUID):
-                self.account.exchange.remove(plan)
-        UserData.set_account(self.account, self.qq,
-                             self.account.phone)
-
-
-myb_exchange_plan = on_command(f"{conf.COMMAND_START}兑换",
-                               aliases={(f"{conf.COMMAND_START}兑换", "+"), (f"{conf.COMMAND_START}兑换", "-")})
-myb_exchange_plan.name = "兑换"
-myb_exchange_plan.usage = f"跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，并使用『{COMMAND_BEGIN}地址』选择你要使用的地址。所需的商品ID可通过命令『{COMMAND_BEGIN}商品』获取。注意，不限兑换时间的商品将不会在此处显示。 "
-myb_exchange_plan.extra_usage = """\
-具体用法：
-{HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
-{HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
-{HEAD}商品 ➢ 查看米游社商品
-『{SEP}』为分隔符，使用NoneBot配置中的其他分隔符亦可\
-"""
-
-
-@myb_exchange_plan.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, command=Command(),
-            command_arg=CommandArg()):
-    """
-    主命令触发
-
-    :command: 主命令和二级命令的元组
-    :command_arg: 二级命令的参数，即商品ID，为Message
-    """
-    if command_arg and len(command) == 1:
-        # 如果没有二级命令，但是有参数，则说明用户没有意向使用本功能。
-        # 例如：/兑换码获取，识别到的参数为"码获取"，而用户可能有意使用其他插件。
-        await matcher.finish()
-    elif len(command) > 1 and command[1] in ["+", "-"]:
-        if not command_arg:
-            await matcher.reject('⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
-                                                                                          SEP=get_last_command_sep()))
-        elif not str(command_arg).isdigit():
-            await matcher.reject(
-                '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
-
-    if isinstance(event, GroupMessageEvent):
-        await matcher.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行操作")
-    qq_account = int(event.user_id)
-    user_account = UserData.read_account_all(qq_account)
-    if not user_account:
-        await matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}{conf.COMMAND_START}登录』进行登录")
-    state['qq_account'] = qq_account
-    state['user_account'] = user_account
-
-    # 如果使用了二级命令 + - 则跳转进下一步，通过phone选择账户进行设置
-    if len(command) > 1:
-        state['command_2'] = command[1]
-        matcher.set_arg("good_id", command_arg)
-        if len(user_account) == 1:
-            matcher.set_arg('phone', Message(str(user_account[0].phone)))
-        else:
-            phones = [str(user_account[i].phone)
-                      for i in range(len(user_account))]
-            msg = "您有多个账号，您要配置以下哪个账号的兑换计划？\n"
-            msg += "📱" + "\n📱".join(phones)
-            msg += "\n🚪发送“退出”即可退出"
-            await matcher.send(msg)
-    # 如果未使用二级命令，则进行查询操作，并结束交互
-    else:
-        msg = ""
-        for account in user_account:
-            for plan in account.exchange:
-                good = await get_good_detail(plan[0])
-                if not good:
-                    await matcher.finish("⚠️获取商品详情失败，请稍后再试")
-                msg += f"""\
-                \n-- 商品 {good.name}\
-                \n- 🔢商品ID：{good.good_id}\
-                \n- 💰商品价格：{good.price} 米游币\
-                \n- 📅兑换时间：{time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))}\
-                \n- 📱账户：{account.phone}""".strip()
-                msg += "\n\n"
-        if not msg:
-            msg = '您还没有兑换计划哦~\n\n'
-        await matcher.finish(msg + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
-
-
-@myb_exchange_plan.got('phone')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, phone=ArgStr('phone')):
-    """
-    请求用户输入手机号以对账户设置兑换计划
-    """
-    user_account: List[UserAccount] = state['user_account']
-
-    if phone == '退出':
-        await matcher.finish('🚪已成功退出')
-    try:
-        state["account"] = list(
-            filter(lambda account: account.phone == int(phone), user_account))[0]
-    except IndexError:
-        await matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
-    except ValueError:
-        await matcher.reject('⚠️您发送的账号不是手机号，请重新发送')
-
-
-@myb_exchange_plan.got('good_id')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, good_id=ArgPlainText('good_id')):
-    """
-    处理三级命令，即商品ID
-    """
-    account: UserAccount = state['account']
-    command_2 = state['command_2']
-    if command_2 == '+':
-        good_dict = {
-            'bh3': await get_good_list('bh3'),
-            'ys': await get_good_list('ys'),
-            'bh2': await get_good_list('bh2'),
-            'wd': await get_good_list('wd'),
-            'bbs': await get_good_list('bbs')
-        }
-        flag = True
-        break_flag = False
-        good = None
-        game = None
-        for game, good_list in good_dict.items():
-            for good in good_list:
-                if good.good_id == good_id:
-                    flag = False
-                    break_flag = True
-                    break
-            if break_flag:
-                break
-        if flag:
-            await matcher.finish('⚠️您发送的商品ID不在可兑换的商品列表内，程序已退出')
-        state['good'] = good
-        uids = []
-        if good.time:
-            # 若为实物商品，也进入下一步骤，但是传入uid为None
-            if good.is_visual:
-                game_records = await get_game_record(account)
-
-                if isinstance(game_records, int):
-                    pass
-                else:
-                    game_name = list(filter(lambda abbr: abbr[0] == game, GameInfo.ABBR_TO_ID.values()))[0][1]
-                    msg = f'您米游社账户下的『{game_name}』账号：'
-                    for record in game_records:
-                        if GameInfo.ABBR_TO_ID[record.game_id][0] == game:
-                            msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.uid}'
-                        uids.append(record.uid)
-                    if uids:
-                        await matcher.send("您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
-                        await asyncio.sleep(0.5)
-                        await matcher.send(msg)
-                    else:
-                        await matcher.finish(f"您还没有绑定『{game_name}』账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
-            else:
-                if not account.address:
-                    await matcher.finish('⚠️您还没有配置地址哦，请先配置地址')
-            state['uids'] = uids
-            matcher.set_arg('uid', Message())
-        else:
-            await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
-
-    elif command_2 == '-':
-        if account.exchange:
-            for exchange_good in account.exchange:
-                if exchange_good[0] == good_id:
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, event.user_id, account.phone)
-                    scheduler.remove_job(job_id=str(
-                        account.phone) + '_' + good_id)
-                    await matcher.finish('兑换计划删除成功')
-            await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
-        else:
-            await matcher.finish("您还没有配置兑换计划哦~")
-
-    else:
-        await matcher.reject(
-            '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
-
-
-@myb_exchange_plan.got('uid')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, uid=ArgPlainText('uid')):
-    """
-    初始化商品兑换任务，如果传入UID为None则为实物商品，仍可继续
-    """
-    account: UserAccount = state['account']
-    good: Good = state['good']
-    uids: List[str] = state['uids']
-    if good.is_visual:
-        if uid == '退出':
-            await matcher.finish('🚪已成功退出')
-        if uid not in uids:
-            await matcher.reject('⚠️您输入的UID不在上述账号内，请重新输入')
-
-    if (good.good_id, uid) in account.exchange:
-        await matcher.finish('⚠️您已经配置过该商品的兑换哦！')
-    else:
-        account.exchange.append((good.good_id, uid))
-
-    # 初始化兑换任务
-    exchange_plan = await Exchange(account, good.good_id, uid).async_init()
-    if exchange_plan.result == -1:
-        await matcher.finish(f"⚠️账户 {account.phone} 登录失效，请重新登录")
-    elif exchange_plan.result == -2:
-        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于未配置stoken，放弃兑换")
-    elif exchange_plan.result == -3:
-        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于stoken为\"v2\"类型，且未配置mid，放弃兑换")
-    elif exchange_plan.result == -4:
-        await matcher.finish(f"⚠️暂不支持商品 {good.good_id} 所属的游戏，放弃兑换")
-    elif exchange_plan.result == -5:
-        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，网络连接失败或服务器返回不正确，放弃兑换")
-    elif exchange_plan.result == -6:
-        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，获取用户游戏账户数据失败，放弃兑换")
-    else:
-        scheduler.add_job(id=str(account.phone) + '_' + good.good_id, replace_existing=True, trigger='date',
-                          func=ExchangeStart(
-                              account, event.user_id, exchange_plan, conf.EXCHANGE_THREAD).start,
-                          next_run_time=datetime.fromtimestamp(good.time))
-
-    UserData.set_account(account, event.user_id, account.phone)
-
-    await matcher.finish(
-        f'🎉设置兑换计划成功！将于 {time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))} 开始兑换，到时将会私聊告知您兑换结果')
-
-
-get_good_image = on_command(conf.COMMAND_START + '商品')
-get_good_image.name = "商品"
-get_good_image.usage = "获取当日米游币商品信息。添加自动兑换计划需要商品ID，请记下您要兑换的商品的ID。"
-
-
-@get_good_image.handle()
-async def _(_: MessageEvent, matcher: Matcher, arg=CommandArg()):
-    # 若有使用二级命令，即传入了想要查看的商品类别，则跳过询问
-    if arg:
-        matcher.set_arg("content", arg)
-
-
-@get_good_image.got("content", prompt="""\
-        \n请发送您要查看的商品类别:\
-        \n- 崩坏3\
-        \n- 原神\
-        \n- 崩坏2\
-        \n- 未定事件簿\
-        \n- 米游社\
-        \n若是商品图片与米游社商品不符或报错 请发送“更新”哦~\
-        \n—— 🚪发送“退出”以结束""".strip())
-async def _(event: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
-    """
-    根据传入的商品类别，发送对应的商品列表图片
-    """
-    if arg == '退出':
-        await matcher.finish('🚪已成功退出')
-    elif arg in ['原神', 'ys']:
-        arg = ('ys', '原神')
-    elif arg in ['崩坏3', '崩坏三', '崩3', '崩三', '崩崩崩', '蹦蹦蹦', 'bh3']:
-        arg = ('bh3', '崩坏3')
-    elif arg in ['崩坏2', '崩坏二', '崩2', '崩二', '崩崩', '蹦蹦', 'bh2']:
-        arg = ('bh2', '崩坏2')
-    elif arg in ['未定', '未定事件簿', 'wd']:
-        arg = ('wd', '未定事件簿')
-    elif arg in ['大别野', '米游社']:
-        arg = ('bbs', '米游社')
-    elif arg == '更新':
-        await get_good_image.send('⏳正在生成商品信息图片...')
-        await generate_image(is_auto=False)
-        await get_good_image.finish('商品信息图片刷新成功')
-    else:
-        await get_good_image.reject('⚠️您的输入有误，请重新输入')
-    good_list = await get_good_list(arg[0])
-    if good_list:
-        img_path = time.strftime(
-            f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
-        if os.path.exists(img_path):
-            with open(img_path, 'rb') as f:
-                image_bytes = io.BytesIO(f.read())
-            await get_good_image.finish(MessageSegment.image(image_bytes))
-        else:
-            await get_good_image.send('⏳请稍等，商品图片正在生成哦~')
-            await generate_image(is_auto=False)
-            img_path = time.strftime(
-                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
-            await get_good_image.finish(MessageSegment.image('file:///' + img_path))
-    else:
-        await get_good_image.finish(f"{arg[1]} 部分目前没有可兑换商品哦~")
-
-
-@driver.on_startup
-async def _():
-    """
-    启动机器人时自动初始化兑换任务
-    """
-    all_accounts = UserData.read_all()
-    for qq in all_accounts.keys():
-        qq = int(qq)
-        accounts = UserData.read_account_all(qq)
-        for account in accounts:
-            exchange_list = account.exchange
-            for exchange_good in exchange_list:
-                good_detail = await get_good_detail(exchange_good[0])
-                if good_detail == -1:
-                    # 若商品不存在则删除
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                    continue
-                if not good_detail.time:
-                    # 若商品已下架则删除
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                    continue
-                if good_detail.time < NtpTime.time():
-                    # 若重启时兑换超时则删除该兑换
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                else:
-                    exchange_plan = await Exchange(account, exchange_good[0], exchange_good[1]).async_init()
-                    scheduler.add_job(id=str(account.phone) + '_' + exchange_good[0], replace_existing=True,
-                                      trigger='date', func=ExchangeStart(
-                            account, qq, exchange_plan, conf.EXCHANGE_THREAD).start,
-                                      next_run_time=datetime.fromtimestamp(good_detail.time))
-
-
-@driver.on_startup
-async def generate_image(is_auto=True):
-    """
-    生成米游币商品信息图片。
-
-    :param is_auto: True为每日自动生成，False为用户手动更新
-    """
-    for root, _, files in os.walk(conf.goodListImage.SAVE_PATH, topdown=False):
-        for name in files:
-            date = time.strftime('%m-%d', time.localtime())
-            # 若图片开头为当日日期，则退出函数不执行
-            if name.startswith(date):
-                if is_auto:
-                    return
-            # 删除旧图片，以方便生成当日图片
-            if name.endswith('.jpg'):
-                os.remove(os.path.join(root, name))
-    for game in "bh3", "ys", "bh2", "wd", "bbs":
-        good_list = await get_good_list(game)
-        if good_list:
-            img_path = time.strftime(
-                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{game}.jpg', time.localtime())
-            image_bytes = await game_list_to_image(good_list)
-            if not image_bytes:
-                return
-            with open(img_path, 'wb') as f:
-                f.write(image_bytes)
-        else:
-            logger.info(f"{conf.LOG_HEAD}{game}分区暂时没有商品，跳过生成...")
+"""
+### 米游社商品兑换前端以及计划任务相关
+"""
+import asyncio
+import io
+import os
+import time
+from copy import deepcopy
+from datetime import datetime
+from typing import List, Set, Union
+
+from nonebot import get_bot, on_command
+from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
+                                         PrivateMessageEvent, GroupMessageEvent)
+from nonebot.adapters.onebot.v11.message import Message
+from nonebot.matcher import Matcher
+from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
+from nonebot_plugin_apscheduler import scheduler
+
+from .bbsAPI import get_game_record
+from .config import config as conf
+from .data import UserData
+from .exchange import (Exchange, Good, UserAccount, get_good_detail,
+                       get_good_list, game_list_to_image)
+from .gameSign import GameInfo
+from .utils import NtpTime, COMMAND_BEGIN, logger, driver, get_last_command_sep
+
+
+class ExchangeStart:
+    """
+    异步多线程兑换
+    """
+
+    def __init__(self, account: UserAccount, qq: int, exchange_plan: Exchange, thread: int) -> None:
+        self.plans: List[Exchange] = []
+        self.tasks: Set[asyncio.Task] = set()
+        self.finishedCount = 0
+        self.account = account
+        self.qq = qq
+
+        for _ in range(thread):
+            self.plans.append(deepcopy(exchange_plan))
+
+    async def start(self):
+        """
+        执行兑换
+        """
+        # 在后台启动兑换操作
+        for plan in self.plans:
+            self.tasks.add(asyncio.create_task(plan.start()))
+        # 等待兑换线程全部结束
+        for task in self.tasks:
+            await task
+
+        bot = get_bot()
+
+        success_tasks: List[asyncio.Task] = list(filter(lambda task: isinstance(
+            task.result(), tuple) and task.result()[0], self.tasks))
+        if success_tasks:
+            await bot.send_private_msg(
+                user_id=self.qq, message=f"🎉用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换成功，可前往米游社查看")
+        else:
+            msg = f"⚠️用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换失败\n返回结果：\n"
+            num = 0
+            for task in self.tasks:
+                num += 1
+                msg += f"{num}: "
+                if isinstance(task.result(), tuple):
+                    msg += str(task.result()[1])
+                else:
+                    msg += f"异常，程序返回结果为 {task.result()}"
+                msg += "\n"
+            await bot.send_private_msg(user_id=self.qq, message=msg)
+        for plan in self.account.exchange:
+            if plan == (self.plans[0].goodID, self.plans[0].gameUID):
+                self.account.exchange.remove(plan)
+        UserData.set_account(self.account, self.qq,
+                             self.account.phone)
+
+
+myb_exchange_plan = on_command(f"{conf.COMMAND_START}兑换",
+                               aliases={(f"{conf.COMMAND_START}兑换", "+"), (f"{conf.COMMAND_START}兑换", "-")}, priority=5, block=True)
+myb_exchange_plan.name = "兑换"
+myb_exchange_plan.usage = f"跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，并使用『{COMMAND_BEGIN}地址』选择你要使用的地址。所需的商品ID可通过命令『{COMMAND_BEGIN}商品』获取。注意，不限兑换时间的商品将不会在此处显示。 "
+myb_exchange_plan.extra_usage = """\
+具体用法：
+{HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
+{HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
+{HEAD}商品 ➢ 查看米游社商品
+『{SEP}』为分隔符，使用NoneBot配置中的其他分隔符亦可\
+"""
+
+
+@myb_exchange_plan.handle()
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, command=Command(),
+            command_arg=CommandArg()):
+    """
+    主命令触发
+
+    :command: 主命令和二级命令的元组
+    :command_arg: 二级命令的参数，即商品ID，为Message
+    """
+    if command_arg and len(command) == 1:
+        # 如果没有二级命令，但是有参数，则说明用户没有意向使用本功能。
+        # 例如：/兑换码获取，识别到的参数为"码获取"，而用户可能有意使用其他插件。
+        await matcher.finish()
+    elif len(command) > 1 and command[1] in ["+", "-"]:
+        if not command_arg:
+            await matcher.reject('⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
+                                                                                          SEP=get_last_command_sep()))
+        elif not str(command_arg).isdigit():
+            await matcher.reject(
+                '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+
+    if isinstance(event, GroupMessageEvent):
+        await matcher.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行操作")
+    qq_account = int(event.user_id)
+    user_account = UserData.read_account_all(qq_account)
+    if not user_account:
+        await matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}{conf.COMMAND_START}登录』进行登录")
+    state['qq_account'] = qq_account
+    state['user_account'] = user_account
+
+    # 如果使用了二级命令 + - 则跳转进下一步，通过phone选择账户进行设置
+    if len(command) > 1:
+        state['command_2'] = command[1]
+        matcher.set_arg("good_id", command_arg)
+        if len(user_account) == 1:
+            matcher.set_arg('phone', Message(str(user_account[0].phone)))
+        else:
+            phones = [str(user_account[i].phone)
+                      for i in range(len(user_account))]
+            msg = "您有多个账号，您要配置以下哪个账号的兑换计划？\n"
+            msg += "📱" + "\n📱".join(phones)
+            msg += "\n🚪发送“退出”即可退出"
+            await matcher.send(msg)
+    # 如果未使用二级命令，则进行查询操作，并结束交互
+    else:
+        msg = ""
+        for account in user_account:
+            for plan in account.exchange:
+                good = await get_good_detail(plan[0])
+                if not good:
+                    await matcher.finish("⚠️获取商品详情失败，请稍后再试")
+                msg += f"""\
+                \n-- 商品 {good.name}\
+                \n- 🔢商品ID：{good.good_id}\
+                \n- 💰商品价格：{good.price} 米游币\
+                \n- 📅兑换时间：{time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))}\
+                \n- 📱账户：{account.phone}""".strip()
+                msg += "\n\n"
+        if not msg:
+            msg = '您还没有兑换计划哦~\n\n'
+        await matcher.finish(msg + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+
+
+@myb_exchange_plan.got('phone')
+async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, phone=ArgStr('phone')):
+    """
+    请求用户输入手机号以对账户设置兑换计划
+    """
+    user_account: List[UserAccount] = state['user_account']
+
+    if phone == '退出':
+        await matcher.finish('🚪已成功退出')
+    try:
+        state["account"] = list(
+            filter(lambda account: account.phone == int(phone), user_account))[0]
+    except IndexError:
+        await matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
+    except ValueError:
+        await matcher.reject('⚠️您发送的账号不是手机号，请重新发送')
+
+
+@myb_exchange_plan.got('good_id')
+async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, good_id=ArgPlainText('good_id')):
+    """
+    处理三级命令，即商品ID
+    """
+    account: UserAccount = state['account']
+    command_2 = state['command_2']
+    if command_2 == '+':
+        good_dict = {
+            'bh3': await get_good_list('bh3'),
+            'ys': await get_good_list('ys'),
+            'bh2': await get_good_list('bh2'),
+            'xq': await get_good_list('xq'),
+            'wd': await get_good_list('wd'),
+            'bbs': await get_good_list('bbs')
+        }
+        flag = True
+        break_flag = False
+        good = None
+        game = None
+        for game, good_list in good_dict.items():
+            for good in good_list:
+                if good.good_id == good_id:
+                    flag = False
+                    break_flag = True
+                    break
+            if break_flag:
+                break
+        if flag:
+            await matcher.finish('⚠️您发送的商品ID不在可兑换的商品列表内，程序已退出')
+        state['good'] = good
+        uids = []
+        if good.time:
+            # 若为实物商品，也进入下一步骤，但是传入uid为None
+            if good.is_visual:
+                game_records = await get_game_record(account)
+
+                if isinstance(game_records, int):
+                    pass
+                else:
+                    game_name = list(filter(lambda abbr: abbr[0] == game, GameInfo.ABBR_TO_ID.values()))[0][1]
+                    msg = f'您米游社账户下的『{game_name}』账号：'
+                    for record in game_records:
+                        if GameInfo.ABBR_TO_ID[record.game_id][0] == game:
+                            msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.uid}'
+                        uids.append(record.uid)
+                    if uids:
+                        await matcher.send("您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
+                        await asyncio.sleep(0.5)
+                        await matcher.send(msg)
+                    else:
+                        await matcher.finish(f"您还没有绑定『{game_name}』账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
+            else:
+                if not account.address:
+                    await matcher.finish('⚠️您还没有配置地址哦，请先配置地址')
+            state['uids'] = uids
+            matcher.set_arg('uid', Message())
+        else:
+            await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
+
+    elif command_2 == '-':
+        if account.exchange:
+            for exchange_good in account.exchange:
+                if exchange_good[0] == good_id:
+                    account.exchange.remove(exchange_good)
+                    UserData.set_account(account, event.user_id, account.phone)
+                    scheduler.remove_job(job_id=str(
+                        account.phone) + '_' + good_id)
+                    await matcher.finish('兑换计划删除成功')
+            await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
+        else:
+            await matcher.finish("您还没有配置兑换计划哦~")
+
+    else:
+        await matcher.reject(
+            '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+
+
+@myb_exchange_plan.got('uid')
+async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, uid=ArgPlainText('uid')):
+    """
+    初始化商品兑换任务，如果传入UID为None则为实物商品，仍可继续
+    """
+    account: UserAccount = state['account']
+    good: Good = state['good']
+    uids: List[str] = state['uids']
+    if good.is_visual:
+        if uid == '退出':
+            await matcher.finish('🚪已成功退出')
+        if uid not in uids:
+            await matcher.reject('⚠️您输入的UID不在上述账号内，请重新输入')
+
+    if (good.good_id, uid) in account.exchange:
+        await matcher.finish('⚠️您已经配置过该商品的兑换哦！')
+    else:
+        account.exchange.append((good.good_id, uid))
+
+    # 初始化兑换任务
+    exchange_plan = await Exchange(account, good.good_id, uid).async_init()
+    if exchange_plan.result == -1:
+        await matcher.finish(f"⚠️账户 {account.phone} 登录失效，请重新登录")
+    elif exchange_plan.result == -2:
+        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于未配置stoken，放弃兑换")
+    elif exchange_plan.result == -3:
+        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于stoken为\"v2\"类型，且未配置mid，放弃兑换")
+    elif exchange_plan.result == -4:
+        await matcher.finish(f"⚠️暂不支持商品 {good.good_id} 所属的游戏，放弃兑换")
+    elif exchange_plan.result == -5:
+        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，网络连接失败或服务器返回不正确，放弃兑换")
+    elif exchange_plan.result == -6:
+        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，获取用户游戏账户数据失败，放弃兑换")
+    else:
+        scheduler.add_job(id=str(account.phone) + '_' + good.good_id, replace_existing=True, trigger='date',
+                          func=ExchangeStart(
+                              account, event.user_id, exchange_plan, conf.EXCHANGE_THREAD).start,
+                          next_run_time=datetime.fromtimestamp(good.time))
+
+    UserData.set_account(account, event.user_id, account.phone)
+
+    await matcher.finish(
+        f'🎉设置兑换计划成功！将于 {time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))} 开始兑换，到时将会私聊告知您兑换结果')
+
+
+get_good_image = on_command(conf.COMMAND_START + '商品', priority=5, block=True)
+get_good_image.name = "商品"
+get_good_image.usage = "获取当日米游币商品信息。添加自动兑换计划需要商品ID，请记下您要兑换的商品的ID。"
+
+
+@get_good_image.handle()
+async def _(_: MessageEvent, matcher: Matcher, arg=CommandArg()):
+    # 若有使用二级命令，即传入了想要查看的商品类别，则跳过询问
+    if arg:
+        matcher.set_arg("content", arg)
+
+
+@get_good_image.got("content", prompt="""\
+        \n请发送您要查看的商品类别:\
+        \n- 崩坏3\
+        \n- 原神\
+        \n- 崩坏2\
+        \n- 崩坏：星穹铁道\
+        \n- 未定事件簿\
+        \n- 米游社\
+        \n若是商品图片与米游社商品不符或报错 请发送“更新”哦~\
+        \n—— 🚪发送“退出”以结束""".strip())
+async def _(event: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
+    """
+    根据传入的商品类别，发送对应的商品列表图片
+    """
+    if arg == '退出':
+        await matcher.finish('🚪已成功退出')
+    elif arg in ['原神', 'ys']:
+        arg = ('ys', '原神')
+    elif arg in ['崩坏3', '崩坏三', '崩3', '崩三', '崩崩崩', '蹦蹦蹦', 'bh3']:
+        arg = ('bh3', '崩坏3')
+    elif arg in ['崩坏2', '崩坏二', '崩2', '崩二', '崩崩', '蹦蹦', 'bh2']:
+        arg = ('bh2', '崩坏2')
+    elif arg in ['崩坏：星穹铁道', '星铁', '星穹铁道', '铁道', '轨子', '星穹', 'xq']:
+        arg = ('xq', '崩坏：星穹铁道')
+    elif arg in ['未定', '未定事件簿', 'wd']:
+        arg = ('wd', '未定事件簿')
+    elif arg in ['大别野', '米游社']:
+        arg = ('bbs', '米游社')
+    elif arg == '更新':
+        await get_good_image.send('⏳正在生成商品信息图片...')
+        await generate_image(is_auto=False)
+        await get_good_image.finish('商品信息图片刷新成功')
+    else:
+        await get_good_image.reject('⚠️您的输入有误，请重新输入')
+    good_list = await get_good_list(arg[0])
+    if good_list:
+        img_path = time.strftime(
+            f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
+        if os.path.exists(img_path):
+            with open(img_path, 'rb') as f:
+                image_bytes = io.BytesIO(f.read())
+            await get_good_image.finish(MessageSegment.image(image_bytes))
+        else:
+            await get_good_image.send('⏳请稍等，商品图片正在生成哦~')
+            await generate_image(is_auto=False)
+            img_path = time.strftime(
+                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
+            await get_good_image.finish(MessageSegment.image('file:///' + img_path))
+    else:
+        await get_good_image.finish(f"{arg[1]} 部分目前没有可兑换商品哦~")
+
+
+@driver.on_startup
+async def _():
+    """
+    启动机器人时自动初始化兑换任务
+    """
+    all_accounts = UserData.read_all()
+    for qq in all_accounts.keys():
+        qq = int(qq)
+        accounts = UserData.read_account_all(qq)
+        for account in accounts:
+            exchange_list = account.exchange
+            for exchange_good in exchange_list:
+                good_detail = await get_good_detail(exchange_good[0])
+                if good_detail == -1:
+                    # 若商品不存在则删除
+                    account.exchange.remove(exchange_good)
+                    UserData.set_account(account, qq, account.phone)
+                    continue
+                if not good_detail.time:
+                    # 若商品已下架则删除
+                    account.exchange.remove(exchange_good)
+                    UserData.set_account(account, qq, account.phone)
+                    continue
+                if good_detail.time < NtpTime.time():
+                    # 若重启时兑换超时则删除该兑换
+                    account.exchange.remove(exchange_good)
+                    UserData.set_account(account, qq, account.phone)
+                else:
+                    exchange_plan = await Exchange(account, exchange_good[0], exchange_good[1]).async_init()
+                    scheduler.add_job(id=str(account.phone) + '_' + exchange_good[0], replace_existing=True,
+                                      trigger='date', func=ExchangeStart(
+                            account, qq, exchange_plan, conf.EXCHANGE_THREAD).start,
+                                      next_run_time=datetime.fromtimestamp(good_detail.time))
+
+
+@driver.on_startup
+async def generate_image(is_auto=True):
+    """
+    生成米游币商品信息图片。
+
+    :param is_auto: True为每日自动生成，False为用户手动更新
+    """
+    for root, _, files in os.walk(conf.goodListImage.SAVE_PATH, topdown=False):
+        for name in files:
+            date = time.strftime('%m-%d', time.localtime())
+            # 若图片开头为当日日期，则退出函数不执行
+            if name.startswith(date):
+                if is_auto:
+                    return
+            # 删除旧图片，以方便生成当日图片
+            if name.endswith('.jpg'):
+                os.remove(os.path.join(root, name))
+    for game in "bh3", "ys", "bh2", "xq", "wd", "bbs":
+        good_list = await get_good_list(game)
+        if good_list:
+            img_path = time.strftime(
+                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{game}.jpg', time.localtime())
+            image_bytes = await game_list_to_image(good_list)
+            if not image_bytes:
+                return
+            with open(img_path, 'wb') as f:
+                f.write(image_bytes)
+        else:
+            logger.info(f"{conf.LOG_HEAD}{game}分区暂时没有商品，跳过生成...")
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/gameSign.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/gameSign.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/help.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""
-### 帮助相关
-#### 参考了`nonebot-plugin-help`
-"""
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageEvent
-from nonebot.adapters.onebot.v11.message import Message
-from nonebot.matcher import Matcher
-from nonebot.params import Arg, CommandArg
-
-from .config import config as conf
-from .utils import PLUGIN, COMMAND_BEGIN
-
-helper = on_command(conf.COMMAND_START + "help", priority=1,
-                    aliases={conf.COMMAND_START + "帮助"})
-
-helper.name = '帮助'
-helper.usage = '''\
-    🍺欢迎使用米游社小助手帮助系统！\
-    \n{HEAD}帮助 ➢ 查看米游社小助手使用说明\
-    \n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明\
-'''.strip()
-
-
-@helper.handle()
-async def _(_: MessageEvent, matcher: Matcher, args: Message = CommandArg()):
-    """
-    主命令触发
-    """
-    # 二级命令
-    if args:
-        matcher.set_arg("content", args)
-    # 只有主命令“帮助”
-    else:
-        await matcher.finish(
-            PLUGIN.metadata.name +
-            PLUGIN.metadata.description +
-            "\n具体用法：\n" +
-            PLUGIN.metadata.usage.format(HEAD=COMMAND_BEGIN))
-
-
-@helper.got('content')
-async def _(_: MessageEvent, content: Message = Arg()):
-    """
-    二级命令触发。功能详细说明查询
-    """
-    arg = content.extract_plain_text().strip()
-
-    # 相似词
-    if arg == '登陆':
-        arg = '登录'
-
-    matchers = PLUGIN.matcher
-    for matcher in matchers:
-        try:
-            if arg.lower() == matcher.name:
-                await helper.finish(
-                    f"『{COMMAND_BEGIN}{matcher.name}』- 使用说明\n{matcher.usage.format(HEAD=COMMAND_BEGIN)}")
-        except AttributeError:
-            continue
-    await helper.finish("⚠️未查询到相关功能，请重新尝试")
+"""
+### 帮助相关
+#### 参考了`nonebot-plugin-help`
+"""
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import MessageEvent
+from nonebot.adapters.onebot.v11.message import Message
+from nonebot.matcher import Matcher
+from nonebot.params import Arg, CommandArg
+
+from .config import config as conf
+from .utils import PLUGIN, COMMAND_BEGIN
+
+helper = on_command(conf.COMMAND_START + "help", priority=1,
+                    aliases={conf.COMMAND_START + "帮助"})
+
+helper.name = '帮助'
+helper.usage = '''\
+    🍺欢迎使用米游社小助手帮助系统！\
+    \n{HEAD}帮助 ➢ 查看米游社小助手使用说明\
+    \n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明\
+'''.strip()
+
+
+@helper.handle()
+async def _(_: MessageEvent, matcher: Matcher, args: Message = CommandArg()):
+    """
+    主命令触发
+    """
+    # 二级命令
+    if args:
+        matcher.set_arg("content", args)
+    # 只有主命令“帮助”
+    else:
+        await matcher.finish(
+            PLUGIN.metadata.name +
+            PLUGIN.metadata.description +
+            "\n具体用法：\n" +
+            PLUGIN.metadata.usage.format(HEAD=COMMAND_BEGIN))
+
+
+@helper.got('content')
+async def _(_: MessageEvent, content: Message = Arg()):
+    """
+    二级命令触发。功能详细说明查询
+    """
+    arg = content.extract_plain_text().strip()
+
+    # 相似词
+    if arg == '登陆':
+        arg = '登录'
+
+    matchers = PLUGIN.matcher
+    for matcher in matchers:
+        try:
+            if arg.lower() == matcher.name:
+                await helper.finish(
+                    f"『{COMMAND_BEGIN}{matcher.name}』- 使用说明\n{matcher.usage.format(HEAD=COMMAND_BEGIN)}")
+        except AttributeError:
+            continue
+    await helper.finish("⚠️未查询到相关功能，请重新尝试")
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/mybMission.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/mybMission.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 
     def __init__(self, gids: int, fid: int):
         self.gids: int = gids
         self.fid: int = fid
 
 
 GAME_ID = {
+    "bbs": GameID(5, 0),
+    # TODO: bbs fid暂时未知
     "bh3": GameID(1, 1),
     "ys": GameID(2, 26),
     "bh2": GameID(3, 30),
     "wd": GameID(4, 37),
     "xq": GameID(5, 52),
 }
 '''所有的gid和fid'''
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 ### 计划任务相关
 """
 import asyncio
+import random
 from typing import List, Union
 
 from nonebot import get_bot, on_command
 from nonebot.adapters.onebot.v11 import (Bot, MessageSegment,
                                          PrivateMessageEvent, GroupMessageEvent)
 from nonebot_plugin_apscheduler import scheduler
 
@@ -14,15 +15,15 @@
 from .data import UserData
 from .exchangePlan import generate_image
 from .gameSign import GameSign, Info
 from .mybMission import Action, get_missions_state
 from .utils import blur_phone as blur
 from .utils import get_file, logger, COMMAND_BEGIN
 
-manually_game_sign = on_command(conf.COMMAND_START + '签到')
+manually_game_sign = on_command(conf.COMMAND_START + '签到', priority=5, block=True)
 manually_game_sign.name = '签到'
 manually_game_sign.usage = '手动进行游戏签到，查看本次签到奖励及本月签到天数'
 
 
 @manually_game_sign.handle()
 async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
     """
@@ -30,15 +31,15 @@
     """
     bot = get_bot(str(event.self_id))
     if not UserData.read_account_all(event.user_id):
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await perform_game_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
 
 
-manually_bbs_sign = on_command(conf.COMMAND_START + '任务')
+manually_bbs_sign = on_command(conf.COMMAND_START + '任务', priority=5, block=True)
 manually_bbs_sign.name = '任务'
 manually_bbs_sign.usage = '手动执行米游币每日任务，可以查看米游币任务完成情况'
 
 
 @manually_bbs_sign.handle()
 async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
     """
@@ -46,15 +47,15 @@
     """
     bot = get_bot(str(event.self_id))
     if not UserData.read_account_all(event.user_id):
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await perform_bbs_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
 
 
-manually_resin_check = on_command(conf.COMMAND_START + '便笺')
+manually_resin_check = on_command(conf.COMMAND_START + '便笺', priority=5, block=True)
 manually_resin_check.name = '便笺'
 manually_resin_check.usage = '手动查看原神实时便笺，即原神树脂、洞天财瓮等信息'
 HAS_CHECKED = {}
 qq_accounts = UserData.read_all().keys()
 for qq in qq_accounts:
     accounts = UserData.read_account_all(qq)
     for account in accounts:
@@ -410,30 +411,36 @@
     """
     每日图片生成函数
     """
     logger.info(f"{conf.LOG_HEAD}开始生成每日商品图片")
     await generate_image()
 
 
-@scheduler.scheduled_job("cron", hour=conf.SIGN_TIME.split(':')[0],
-                         minute=conf.SIGN_TIME.split(':')[1], id="daily_schedule")
+@scheduler.scheduled_job("cron",
+                         hour=conf.SIGN_TIME.split(':')[0],
+                         minute=conf.SIGN_TIME.split(':')[1],
+                         second=str(random.randint(0,59)),
+                         id="daily_schedule")
 async def daily_schedule():
     """
     自动米游币任务、游戏签到函数
     """
     logger.info(f"{conf.LOG_HEAD}开始执行每日自动任务")
     qq_accounts = UserData.read_all().keys()
     bot = get_bot()
     for qq in qq_accounts:
         await perform_bbs_sign(bot=bot, qq=qq, is_auto=True)
         await perform_game_sign(bot=bot, qq=qq, is_auto=True)
     logger.info(f"{conf.LOG_HEAD}每日自动任务执行完成")
 
 
-@scheduler.scheduled_job("interval", minutes=conf.RESIN_CHECK_INTERVAL, id="resin_check")
+@scheduler.scheduled_job("interval",
+                         minutes=conf.RESIN_CHECK_INTERVAL,
+                         second=str(random.randint(0,59)),
+                         id="resin_check")
 async def auto_resin_check():
     """
     自动查看实时便笺
     """
     qq_accounts = UserData.read_all().keys()
     bot = get_bot()
     for qq in qq_accounts:
```

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/setting.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.5/PKG-INFO` & `nonebot_plugin_mystool-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 0.2.5
+Version: 0.2.6
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -12,21 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: Pillow (>=9.4.0,<9.5.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: nonebot_adapter_onebot (>=2.1.3)
+Requires-Dist: Pillow (>=9.5.0,<10.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: nonebot_adapter_onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
-Requires-Dist: requests (>=2.28.2,<2.29.0)
-Requires-Dist: tenacity (>=8.2.2,<8.3.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues
 Project-URL: Documentation, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki
 Project-URL: Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 Description-Content-Type: text/markdown
 
 ```
  __    __     __  __     ______     ______   ______     ______     __
@@ -46,39 +46,38 @@
   <a href="https://github.com/Ljzd-PRO/nonebot-plugin-mystool/commits/" target="_blank">
     <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
   </a>
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.5**
+**版本 - v0.2.6**
 
 ### 📣 更新内容
+
+#### 2023.4.28
+- 修复插件命令被其他 nonebot 插件捕获的问题
+- 增加支持星穹铁道的商品兑换
+- 每日签到、米游币任务执行时间在用户配置的基础上增加随机延迟
+- 修复大别野频道每日任务、签到执行失败的问题
+
 #### 2023.3.30
 - 修复重写配置文件 `pluginConfig.json` 不生效的问题
 - 修复单账户情况下无法增删兑换计划的问题
 - 修复 `/兑换` 命令可能与其他插件命令冲突的问题，同时 [🔗用法变更](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-Exchange#增加删除兑换计划)
 - 精简接收的命令
 - 更正 `device_save` "设备保存" 日志文本的错误
 
 #### 2023.3.18
 - 增加导出Cookies功能
 - 增加删除账号数据功能
 - 在用户所有账号都登录失效的情况下关闭通知
 - 修复原神游戏签到失败问题
 - 规范化代码
 
-#### 2023.1.17
-- 修复群聊中手动签到不会模糊处理手机号的问题
-- 配置中可控制加好友是否发送欢迎以及使用指引信息
-- 入群后不再自动发送欢迎信息
-
-#### 2022.12.24
-- 支持群聊使用
-
 ## 功能和特性
 
 - 短信验证登录，免抓包获取 Cookie
 - 自动完成每日米游币任务
 - 自动进行游戏签到
 - 可制定米游币商品兑换计划，到点兑换
 - 可支持多个 QQ 账号，每个 QQ 账号可绑定多个米哈游账户
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.6 Summary:
 NoneBot2æä»¶|ç±³æ¸¸ç¤¾å·¥å·-
 æ¯æ¥ç±³æ¸¸å¸ä»»å¡ãæ¸¸æç­¾å°ãåååæ¢ãåæåç»å½ãåç¥æ èæé
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO Author-email: ljzd@office.ljzd-pro.ml Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Requires-Dist: Pillow (>=9.4.0,<9.5.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: nonebot_adapter_onebot
-(>=2.1.3) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0) Requires-Dist:
-ntplib (>=0.4.0,<0.5.0) Requires-Dist: requests (>=2.28.2,<2.29.0) Requires-
-Dist: tenacity (>=8.2.2,<8.3.0) Project-URL: Bug Tracker, https://github.com/
-Ljzd-PRO/nonebot-plugin-mystool/issues Project-URL: Documentation, https://
-github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki Project-URL: Repository, https:
-//github.com/Ljzd-PRO/nonebot-plugin-mystool Description-Content-Type: text/
-markdown ``` __ __ __ __ ______ ______ ______ ______ __ /\ "-./ \ /\ \_\ \ /
-\ ___\ /\__ _\ /\ __ \ /\ __ \ /\ \ \ \ \-./\ \ \ \____ \ \ \___ \ \/_/\ \/ \ \
-\/\ \ \ \ \/\ \ \ \ \____ \ \_\ \ \_\ \/\_____\ \/\_____\ \ \_\ \ \_____\ \
-\_____\ \ \_____\ \/_/ \/_/ \/_____/ \/_____/ \/_/ \/_____/ \/_____/ \/_____/
-```
+Programming Language :: Python :: 3 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: nonebot_adapter_onebot
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0) Requires-
+Dist: ntplib (>=0.4.0,<0.5.0) Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0) Project-URL: Bug Tracker, https://
+github.com/Ljzd-PRO/nonebot-plugin-mystool/issues Project-URL: Documentation,
+https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki Project-URL:
+Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool Description-
+Content-Type: text/markdown ``` __ __ __ __ ______ ______ ______ ______ __ /
+\ "-./ \ /\ \_\ \ /\ ___\ /\__ _\ /\ __ \ /\ __ \ /\ \ \ \ \-./\ \ \ \____ \ \
+\___ \ \/_/\ \/ \ \ \/\ \ \ \ \/\ \ \ \ \____ \ \_\ \ \_\ \/\_____\ \/\_____\ \
+\_\ \ \_____\ \ \_____\ \ \_____\ \/_/ \/_/ \/_____/ \/_____/ \/_/ \/_____/ \/
+_____/ \/_____/ ```
 [CodeFactor] [ææ°åè¡ç] [æåæäº¤]
-# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.5** ### ð£
-æ´æ°åå®¹ #### 2023.3.30 - ä¿®å¤éåéç½®æä»¶ `pluginConfig.json`
-ä¸çæçé®é¢ - ä¿®å¤åè´¦æ·æåµä¸æ æ³å¢å åæ¢è®¡åçé®é¢
-- ä¿®å¤ `/åæ¢` å½ä»¤å¯è½ä¸å¶ä»æä»¶å½ä»¤å²çªçé®é¢ï¼åæ¶
-[ðç¨æ³åæ´](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/
-Information-Exchange#å¢å å é¤åæ¢è®¡å) - ç²¾ç®æ¥æ¶çå½ä»¤ - æ´æ­£
+# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.6** ### ð£
+æ´æ°åå®¹ #### 2023.4.28 - ä¿®å¤æä»¶å½ä»¤è¢«å¶ä» nonebot
+æä»¶æè·çé®é¢ - å¢å æ¯ææç©¹ééçåååæ¢ -
+æ¯æ¥ç­¾å°ãç±³æ¸¸å¸ä»»å¡æ§è¡æ¶é´å¨ç¨æ·éç½®çåºç¡ä¸å¢å éæºå»¶è¿
+- ä¿®å¤å¤§å«éé¢éæ¯æ¥ä»»å¡ãç­¾å°æ§è¡å¤±è´¥çé®é¢ ####
+2023.3.30 - ä¿®å¤éåéç½®æä»¶ `pluginConfig.json` ä¸çæçé®é¢ -
+ä¿®å¤åè´¦æ·æåµä¸æ æ³å¢å åæ¢è®¡åçé®é¢ - ä¿®å¤ `/åæ¢`
+å½ä»¤å¯è½ä¸å¶ä»æä»¶å½ä»¤å²çªçé®é¢ï¼åæ¶ [ðç¨æ³åæ´]
+(https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-
+Exchange#å¢å å é¤åæ¢è®¡å) - ç²¾ç®æ¥æ¶çå½ä»¤ - æ´æ­£
 `device_save` "è®¾å¤ä¿å­" æ¥å¿ææ¬çéè¯¯ #### 2023.3.18 -
 å¢å å¯¼åºCookiesåè½ - å¢å å é¤è´¦å·æ°æ®åè½ -
 å¨ç¨æ·ææè´¦å·é½ç»å½å¤±æçæåµä¸å³é­éç¥ -
-ä¿®å¤åç¥æ¸¸æç­¾å°å¤±è´¥é®é¢ - è§èåä»£ç  #### 2023.1.17 -
-ä¿®å¤ç¾¤èä¸­æå¨ç­¾å°ä¸ä¼æ¨¡ç³å¤çææºå·çé®é¢ -
-éç½®ä¸­å¯æ§å¶å å¥½åæ¯å¦åéæ¬¢è¿ä»¥åä½¿ç¨æå¼ä¿¡æ¯ -
-å¥ç¾¤åä¸åèªå¨åéæ¬¢è¿ä¿¡æ¯ #### 2022.12.24 - æ¯æç¾¤èä½¿ç¨ ##
-åè½åç¹æ§ - ç­ä¿¡éªè¯ç»å½ï¼åæåè·å Cookie -
-èªå¨å®ææ¯æ¥ç±³æ¸¸å¸ä»»å¡ - èªå¨è¿è¡æ¸¸æç­¾å° -
+ä¿®å¤åç¥æ¸¸æç­¾å°å¤±è´¥é®é¢ - è§èåä»£ç  ## åè½åç¹æ§ -
+ç­ä¿¡éªè¯ç»å½ï¼åæåè·å Cookie - èªå¨å®ææ¯æ¥ç±³æ¸¸å¸ä»»å¡
+- èªå¨è¿è¡æ¸¸æç­¾å° -
 å¯å¶å®ç±³æ¸¸å¸åååæ¢è®¡åï¼å°ç¹åæ¢ - å¯æ¯æå¤ä¸ª QQ
 è´¦å·ï¼æ¯ä¸ª QQ è´¦å·å¯ç»å®å¤ä¸ªç±³åæ¸¸è´¦æ· - QQ
 æ¨éæ§è¡ç»æéç¥ -
 åç¥æ èãæ´å¤©å®é±ãè´¨éååä»ªå·²æ»¡æ¶æ¨ééç¥ ##
 ä½¿ç¨è¯´æ ### ð ï¸ NoneBot2 æºå¨äººé¨ç½²åæä»¶å®è£ è¯·æ¥ç ->
 [ðInstallation](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/
 Installation) ### ð æä»¶å·ä½ä½¿ç¨è¯´æ è¯·æ¥ç -> [ðWiki ææ¡£]
```


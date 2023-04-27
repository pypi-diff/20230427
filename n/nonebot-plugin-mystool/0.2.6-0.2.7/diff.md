# Comparing `tmp/nonebot_plugin_mystool-0.2.6.tar.gz` & `tmp/nonebot_plugin_mystool-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-0.2.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-0.2.7.tar", max compression
```

## Comparing `nonebot_plugin_mystool-0.2.6.tar` & `nonebot_plugin_mystool-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/LICENSE
--rw-r--r--   0        0        0     3262 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/README.md
--rw-r--r--   0        0        0     1317 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     2077 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/addFriend.py
--rw-r--r--   0        0        0     6914 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    30682 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/bbsAPI.py
--rw-r--r--   0        0        0     7081 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/config.py
--rw-r--r--   0        0        0    15416 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/data.py
--rw-r--r--   0        0        0    22802 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    19562 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchangePlan.py
--rw-r--r--   0        0        0    15148 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/gameSign.py
--rw-r--r--   0        0        0     1832 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    14883 2023-04-27 20:36:19.795683 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    23334 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/mybMission.py
--rw-r--r--   0        0        0    23937 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0     9755 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    10836 2023-04-27 20:36:19.799680 nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3262 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/README.md
+-rw-r--r--   0        0        0     1317 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2802 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     2077 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/addFriend.py
+-rw-r--r--   0        0        0     6914 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    30682 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/bbsAPI.py
+-rw-r--r--   0        0        0     7081 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/config.py
+-rw-r--r--   0        0        0    15416 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/data.py
+-rw-r--r--   0        0        0    22802 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    19562 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchangePlan.py
+-rw-r--r--   0        0        0    15148 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/gameSign.py
+-rw-r--r--   0        0        0     1832 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    14883 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    23334 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/mybMission.py
+-rw-r--r--   0        0        0    23885 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0     9755 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    10836 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-0.2.6/LICENSE` & `nonebot_plugin_mystool-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/README.md` & `nonebot_plugin_mystool-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 6f74 2d70 6c75 6769 6e2d 6d79 7354 6f6f  ot-plugin-mysToo
 00000430: 6c3f 7374 796c 653d 666f 722d 7468 652d  l?style=for-the-
 00000440: 6261 6467 6522 3e0a 2020 3c2f 613e 0a3c  badge">.  </a>.<
 00000450: 2f64 6976 3e0a 0a23 206d 7973 546f 6f6c  /div>..# mysTool
 00000460: 202d 20e7 b1b3 e6b8 b8e7 a4be e8be 85e5   - .............
 00000470: 8aa9 e5b7 a5e5 85b7 e68f 92e4 bbb6 0a0a  ................
 00000480: 2a2a e789 88e6 9cac 202d 2076 302e 322e  **...... - v0.2.
-00000490: 362a 2a0a 0a23 2323 20f0 9f93 a320 e69b  6**..### .... ..
+00000490: 372a 2a0a 0a23 2323 20f0 9f93 a320 e69b  7**..### .... ..
 000004a0: b4e6 96b0 e586 85e5 aeb9 0a0a 2323 2323  ............####
 000004b0: 2032 3032 332e 342e 3238 0a2d 20e4 bfae   2023.4.28.- ...
 000004c0: e5a4 8de6 8f92 e4bb b6e5 91bd e4bb a4e8  ................
 000004d0: a2ab e585 b6e4 bb96 206e 6f6e 6562 6f74  ........ nonebot
 000004e0: 20e6 8f92 e4bb b6e6 8d95 e88e b7e7 9a84   ...............
 000004f0: e997 aee9 a298 0a2d 20e5 a29e e58a a0e6  .......- .......
 00000500: 94af e68c 81e6 989f e7a9 b9e9 9381 e981  ................
```

### Comparing `nonebot_plugin_mystool-0.2.6/pyproject.toml` & `nonebot_plugin_mystool-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v0.2.6"
+version = "v0.2.7"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
```

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/addFriend.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/addFriend.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/bbsAPI.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/bbsAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/config.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/data.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchange.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/exchangePlan.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchangePlan.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/gameSign.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/gameSign.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/mybMission.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/mybMission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,32 +414,32 @@
     logger.info(f"{conf.LOG_HEAD}开始生成每日商品图片")
     await generate_image()
 
 
 @scheduler.scheduled_job("cron",
                          hour=conf.SIGN_TIME.split(':')[0],
                          minute=conf.SIGN_TIME.split(':')[1],
-                         second=str(random.randint(0,59)),
                          id="daily_schedule")
 async def daily_schedule():
     """
     自动米游币任务、游戏签到函数
     """
+    # 随机延迟
+    await asyncio.sleep(random.randint(0, 59))
     logger.info(f"{conf.LOG_HEAD}开始执行每日自动任务")
     qq_accounts = UserData.read_all().keys()
     bot = get_bot()
     for qq in qq_accounts:
         await perform_bbs_sign(bot=bot, qq=qq, is_auto=True)
         await perform_game_sign(bot=bot, qq=qq, is_auto=True)
     logger.info(f"{conf.LOG_HEAD}每日自动任务执行完成")
 
 
 @scheduler.scheduled_job("interval",
                          minutes=conf.RESIN_CHECK_INTERVAL,
-                         second=str(random.randint(0,59)),
                          id="resin_check")
 async def auto_resin_check():
     """
     自动查看实时便笺
     """
     qq_accounts = UserData.read_all().keys()
     bot = get_bot()
```

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/setting.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.6/PKG-INFO` & `nonebot_plugin_mystool-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 0.2.6
+Version: 0.2.7
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -46,15 +46,15 @@
   <a href="https://github.com/Ljzd-PRO/nonebot-plugin-mystool/commits/" target="_blank">
     <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
   </a>
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.6**
+**版本 - v0.2.7**
 
 ### 📣 更新内容
 
 #### 2023.4.28
 - 修复插件命令被其他 nonebot 插件捕获的问题
 - 增加支持星穹铁道的商品兑换
 - 每日签到、米游币任务执行时间在用户配置的基础上增加随机延迟
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.7 Summary:
 NoneBot2æä»¶|ç±³æ¸¸ç¤¾å·¥å·-
 æ¯æ¥ç±³æ¸¸å¸ä»»å¡ãæ¸¸æç­¾å°ãåååæ¢ãåæåç»å½ãåç¥æ èæé
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO Author-email: ljzd@office.ljzd-pro.ml Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -19,15 +19,15 @@
 Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool Description-
 Content-Type: text/markdown ``` __ __ __ __ ______ ______ ______ ______ __ /
 \ "-./ \ /\ \_\ \ /\ ___\ /\__ _\ /\ __ \ /\ __ \ /\ \ \ \ \-./\ \ \ \____ \ \
 \___ \ \/_/\ \/ \ \ \/\ \ \ \ \/\ \ \ \ \____ \ \_\ \ \_\ \/\_____\ \/\_____\ \
 \_\ \ \_____\ \ \_____\ \ \_____\ \/_/ \/_/ \/_____/ \/_____/ \/_/ \/_____/ \/
 _____/ \/_____/ ```
 [CodeFactor] [ææ°åè¡ç] [æåæäº¤]
-# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.6** ### ð£
+# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.7** ### ð£
 æ´æ°åå®¹ #### 2023.4.28 - ä¿®å¤æä»¶å½ä»¤è¢«å¶ä» nonebot
 æä»¶æè·çé®é¢ - å¢å æ¯ææç©¹ééçåååæ¢ -
 æ¯æ¥ç­¾å°ãç±³æ¸¸å¸ä»»å¡æ§è¡æ¶é´å¨ç¨æ·éç½®çåºç¡ä¸å¢å éæºå»¶è¿
 - ä¿®å¤å¤§å«éé¢éæ¯æ¥ä»»å¡ãç­¾å°æ§è¡å¤±è´¥çé®é¢ ####
 2023.3.30 - ä¿®å¤éåéç½®æä»¶ `pluginConfig.json` ä¸çæçé®é¢ -
 ä¿®å¤åè´¦æ·æåµä¸æ æ³å¢å åæ¢è®¡åçé®é¢ - ä¿®å¤ `/åæ¢`
 å½ä»¤å¯è½ä¸å¶ä»æä»¶å½ä»¤å²çªçé®é¢ï¼åæ¶ [ðç¨æ³åæ´]
```


# Comparing `tmp/nonebot_plugin_autoreply-0.2.7.tar.gz` & `tmp/nonebot_plugin_autoreply-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_autoreply-0.2.7.tar", last modified: Tue Apr 25 16:35:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_autoreply-0.2.8.tar", last modified: Thu Apr 27 14:44:43 2023, max compression
```

## Comparing `nonebot_plugin_autoreply-0.2.7.tar` & `nonebot_plugin_autoreply-0.2.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/LICENSE
--rw-r--r--   0        0        0    12495 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/README.md
--rw-r--r--   0        0        0      303 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__init__.py
--rw-r--r--   0        0        0     6387 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__main__.py
--rw-r--r--   0        0        0     3104 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/config.py
--rw-r--r--   0        0        0       49 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/cool_down.py
--rw-r--r--   0        0        0     1749 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/util.py
--rw-r--r--   0        0        0      610 2023-04-25 16:35:11.400227 nonebot_plugin_autoreply-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/LICENSE
+-rw-r--r--   0        0        0    13133 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/README.md
+-rw-r--r--   0        0        0      303 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__init__.py
+-rw-r--r--   0        0        0     6557 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__main__.py
+-rw-r--r--   0        0        0     3623 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/config.py
+-rw-r--r--   0        0        0       49 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/cool_down.py
+-rw-r--r--   0        0        0     2001 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/util.py
+-rw-r--r--   0        0        0      629 2023-04-27 14:44:43.583599 nonebot_plugin_autoreply-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    13701 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.8/PKG-INFO
```

### Comparing `nonebot_plugin_autoreply-0.2.7/LICENSE` & `nonebot_plugin_autoreply-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_autoreply-0.2.7/README.md` & `nonebot_plugin_autoreply-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 </details>
 
 ## ⚙️ 配置
 
 ### 回复配置
 
 插件的配置文件位于 `data/autoreply` 下  
-在里面新建一个 `json` 后缀文件即可开始配置
+在里面新建一个 `yml` 或 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
     // 该组配置是否阻塞其他回复配置
@@ -272,26 +272,30 @@
   }
 
   // ...
 ]
 ```
 
 插件提供了一些变量，他们可以被用在 `normal` 和 `array` 类型的消息，以及 `multi` 类型中嵌套的这两个类型的消息中；`plain` 类型的消息则无法使用变量  
-变量使用 `str.format()` 方法替换，所以如果想要转义 `{` 或 `}`，使用 `{{` 或 `}}` 即可
+变量使用 [`MessageTemplate.format_map()`](https://v2.nonebot.dev/docs/tutorial/message#%E4%BD%BF%E7%94%A8%E6%B6%88%E6%81%AF%E6%A8%A1%E6%9D%BF) 方法替换
 
 下面是插件提供的变量列表
 
+- `{bs}` - “`{`”，转义用
+- `{be}` - “`}`”，转义用
 - `{self_id}` - 机器人 QQ
 - `{message_id}` - 消息 ID _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 - `{user_id}` - 发送者 QQ
 - `{group_id}` - 消息来源群号 _（私聊等为 `None`）_
 - `{target_id}` - 被戳者 QQ _（仅当 `match` 的 `type` 为 `poke` 时有值，其他情况为 `None`）_
 - `{nickname}` - 发送者昵称
 - `{card}` - 发送者群名片
 - `{display_name}` - 发送者显示名称 _（优先群名片，当群名片为空时为昵称）_
+- `{at}` - 艾特发送者
+- `{reply}` - 回复发送者 _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 
 下面放出几个示例，帮助大家更好的理解如何使用变量
 
 ```jsonc
 [
   {
     "matches": [
@@ -338,17 +342,17 @@
           "[multi] 我刚刚 At 了一下你哦~ 收到了吗？"
         ]
       },
 
       // 无法在 plain 类型消息中使用，{user_id}、{nickname} 会原样显示
       "@[plain] [CQ:at,qq={user_id}] 啊咧？怎么 At 不了 {nickname}？",
 
-      // 可以在消息中使用 {{ 和 }} 来转义大括号
+      // 可以在消息中使用 {bs｝ 和 {be} 来转义大括号
       // 前面的 {{user_id}} 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
-      "[normal] [CQ:at,qq={{user_id}}] 啊咧？怎么 At 不了 {nickname}？"
+      "[normal] [CQ:at,qq={bs}user_id{be}] 啊咧？怎么 At 不了 {nickname}？"
     ]
   }
 ]
 ```
 
 ### 常规配置
 
@@ -386,20 +390,27 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.8
+
+- 支持解析 `yaml` 格式配置，会将 `.yml` 和 `.yaml` 的文件作为 `yaml` 格式配置加载
+- 现在会寻找 `data/autoreply` 文件夹下所有子文件夹中的配置并加载
+- 新增变量 `{at}`、`{reply}`
+- 换用 `MessageTemplate` 格式化变量；由于这玩意不支持 `{{` 及 `}}` 转义，所以加入了变量 `{bs}` 和 `{be}`
+
 ### 0.2.7
 
 - 新增了配置的 `block` 和 `priority` 属性
 - 新增 `type` 为 `poke` (双击头像，戳一戳) 的 `match`
 - 新增了 `match` 的 `possibility` 属性
-- 新增了 `{display_name}` 变量
+- 新增了 `{target_id}` 与 `{display_name}` 变量
 
 ### 0.2.6
 
 - 回复中可以使用变量了
 - 新增配置市场
 
 ### 0.2.5
```

#### html2text {}

```diff
@@ -22,16 +22,16 @@
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-autoreply ```   pdm ```bash pdm add nonebot-plugin-
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
-æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
-åç¼æä»¶å³å¯å¼å§éç½®
+æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `yml`
+æ `json` åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
 ```jsonc [ { // è¯¥ç»éç½®æ¯å¦é»å¡å¶ä»åå¤éç½® /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "block": true, /
 / è¯¥ç»éç½®çä¼åçº§ï¼è¶å¤§è¶é« // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1
 "priority": 1, // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
 / å¹éæ¨¡å¼ï¼å¯é `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`
 (æ­£åå¹é)ã`poke`(åå»å¤´åæ³ä¸æ³) // // ä½¿ç¨ `poke`
@@ -87,53 +87,63 @@
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå "users": { /
 / é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå) "type":
 "black", // è¦è¿æ»¤çQQå· "values": [ 1145141919, 9191415411 /
 / æ´å¤QQå·... ] } } // ... ] ```
 æä»¶æä¾äºä¸äºåéï¼ä»ä»¬å¯ä»¥è¢«ç¨å¨ `normal` å `array`
 ç±»åçæ¶æ¯ï¼ä»¥å `multi`
 ç±»åä¸­åµå¥çè¿ä¸¤ä¸ªç±»åçæ¶æ¯ä¸­ï¼`plain`
-ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ `str.format()`
-æ¹æ³æ¿æ¢ï¼æä»¥å¦ææ³è¦è½¬ä¹ `{` æ `}`ï¼ä½¿ç¨ `{{` æ `}}`
-å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ - `
-{message_id}` - æ¶æ¯ ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º
-`None`ï¼_ - `{user_id}` - åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å·
-_ï¼ç§èç­ä¸º `None`ï¼_ - `{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match`
-ç `type` ä¸º `poke` æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` -
-åéèæµç§° - `{card}` - åéèç¾¤åç - `{display_name}` -
-åéèæ¾ç¤ºåç§° _ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_
+ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ [`MessageTemplate.format_map
+()`](https://v2.nonebot.dev/docs/tutorial/
+message#%E4%BD%BF%E7%94%A8%E6%B6%88%E6%81%AF%E6%A8%A1%E6%9D%BF) æ¹æ³æ¿æ¢
+ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{bs}` - â`{`âï¼è½¬ä¹ç¨ - `{be}`
+- â`}`âï¼è½¬ä¹ç¨ - `{self_id}` - æºå¨äºº QQ - `{message_id}` - æ¶æ¯
+ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º `None`ï¼_ - `{user_id}` -
+åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å· _ï¼ç§èç­ä¸º `None`ï¼_ -
+`{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match` ç `type` ä¸º `poke`
+æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` - åéèæµç§° - `
+{card}` - åéèç¾¤åç - `{display_name}` - åéèæ¾ç¤ºåç§°
+_ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_ - `{at}` -
+è¾ç¹åéè - `{reply}` - åå¤åéè _ï¼å½ `match` ç `type` ä¸º
+`poke` æ¶ä¸º `None`ï¼_
 ä¸é¢æ¾åºå ä¸ªç¤ºä¾ï¼å¸®å©å¤§å®¶æ´å¥½ççè§£å¦ä½ä½¿ç¨åé
 ```jsonc [ { "matches": [ { "match": "^(@|at|è¾ç¹)æ$", "type": "regex" } ],
 "replies": [ // å¨ normal ç±»åæ¶æ¯ä¸­ä½¿ç¨ "[normal] Atäº [CQ:at,qq=
 {user_id}]", // å¨ array ç±»åæ¶æ¯ä¸­ä½¿ç¨ [ { "type": "text", "data":
 { "text": "[array] Atäº " } }, { "type": "at", "data": { "qq": "{user_id}" } }
 ], // å¨ multi ç±»åæ¶æ¯ä¸­ä½¿ç¨ { "type": "multi", "message": [ /
 / åµå¥ç array ç±»åæ¶æ¯ [ { "type": "at", "data": { "qq": "{user_id}" }
 } ], // åµå¥ç normal ç±»åæ¶æ¯ "[multi] æåå At äºä¸ä¸ä½ å¦~
 æ¶å°äºåï¼" ] }, // æ æ³å¨ plain ç±»åæ¶æ¯ä¸­ä½¿ç¨ï¼{user_id}ã
 {nickname} ä¼åæ ·æ¾ç¤º "@[plain] [CQ:at,qq={user_id}] åå§ï¼æä¹ At
-ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {{ å }} æ¥è½¬ä¹å¤§æ¬å·
-// åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
-{nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={{user_id}}] åå§ï¼æä¹ At
-ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
+ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {bsï½ å {be}
+æ¥è½¬ä¹å¤§æ¬å· // åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id}
+åéï¼èåé¢ç {nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={bs}user_id
+{be}] åå§ï¼æä¹ At ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
 ä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
 éç½®é¡¹è¯·åèä¸é¢çææ¬ ```ini # matcher æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤
 False AUTOREPLY_BLOCK=False # matcher ä¼åçº§ AUTOREPLY_PRIORITY=99 ``` ##
 ð¬ æä»¤ ### `éè½½èªå¨åå¤`
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.7 - æ°å¢äºéç½®ç `block`
-å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke` (åå»å¤´åï¼æ³ä¸æ³) ç
-`match` - æ°å¢äº `match` ç `possibility` å±æ§ - æ°å¢äº `
-{display_name}` åé ### 0.2.6 - åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº -
-æ°å¢éç½®å¸åº ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.8 - æ¯æè§£æ `yaml`
+æ ¼å¼éç½®ï¼ä¼å° `.yml` å `.yaml` çæä»¶ä½ä¸º `yaml`
+æ ¼å¼éç½®å è½½ - ç°å¨ä¼å¯»æ¾ `data/autoreply`
+æä»¶å¤¹ä¸ææå­æä»¶å¤¹ä¸­çéç½®å¹¶å è½½ - æ°å¢åé `{at}`ã`
+{reply}` - æ¢ç¨ `MessageTemplate` æ ¼å¼ååéï¼ç±äºè¿ç©æä¸æ¯æ
+`{{` å `}}` è½¬ä¹ï¼æä»¥å å¥äºåé `{bs}` å `{be}` ### 0.2.7 -
+æ°å¢äºéç½®ç `block` å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke`
+(åå»å¤´åï¼æ³ä¸æ³) ç `match` - æ°å¢äº `match` ç `possibility`
+å±æ§ - æ°å¢äº `{target_id}` ä¸ `{display_name}` åé ### 0.2.6 -
+åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº - æ°å¢éç½®å¸åº ### 0.2.5 -
+å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
 è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
 å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
```

### Comparing `nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__main__.py` & `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import asyncio
 import random
 import re
 from itertools import starmap
 from typing import (
-    Any,
     Callable,
-    Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
@@ -25,19 +23,15 @@
     PokeNotifyEvent,
 )
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 from typing_extensions import TypeVarTuple, Unpack
 
-from nonebot_plugin_autoreply.util import (
-    get_var_dict,
-    replace_segment_var,
-    replace_str_var,
-)
+from nonebot_plugin_autoreply.util import VarDictType, get_var_dict, replace_message_var
 
 from .config import (
     FilterModel,
     MatchModel,
     MatchType,
     MessageSegmentModel,
     ReplyModel,
@@ -69,15 +63,15 @@
     return ok
 
 
 def check_message(match: MatchModel, event: MessageEvent) -> bool:
     if match.type == "poke":
         return False
 
-    if not match.match:
+    if match.match is None:
         raise ValueError("存在 type 不为 poke，且 match 为空的不合法匹配规则")
 
     if match.to_me and (not event.is_tome()):
         return False
 
     msg_str = str(event.message)
     msg_plaintext = event.message.extract_plain_text()
@@ -163,15 +157,15 @@
 
     state["reply"] = state_reply
     return bool(state_reply)
 
 
 def get_reply_msgs(
     reply: ReplyType,
-    var_dict: Dict[str, Any],
+    var_dict: VarDictType,
     refuse_multi: bool = False,
 ) -> Tuple[List[Message], Optional[Tuple[int, int]]]:
     if isinstance(reply, str):
         str_is_plain = reply.startswith("@")
         if str_is_plain:
             reply = reply[1:]
 
@@ -183,28 +177,40 @@
     rt = reply.type
     msg = reply.message
 
     if rt == "plain":
         return [Message() + cast(str, msg)], None
 
     if rt == "array":
-        replaced = replace_segment_var(cast(List[MessageSegmentModel], msg), var_dict)
-        return [
-            Message([MessageSegment(type=x.type, data=x.data) for x in replaced]),
-        ], None
+        return (
+            [
+                replace_message_var(
+                    Message(
+                        MessageSegment(type=x.type, data=x.data)
+                        for x in cast(List[MessageSegmentModel], msg)
+                    ),
+                    var_dict,
+                ),
+            ],
+            None,
+        )
 
     if rt == "multi":
         if refuse_multi:
             raise ValueError("Nested `multi` is not allowed")
-        return [
-            get_reply_msgs(x, var_dict, True)[0][0] for x in cast(List[ReplyModel], msg)
-        ], reply.delay
+        return (
+            [
+                get_reply_msgs(x, var_dict, True)[0][0]
+                for x in cast(List[ReplyModel], msg)
+            ],
+            reply.delay,
+        )
 
     # default normal
-    return [Message(replace_str_var(cast(str, msg), var_dict))], None
+    return [replace_message_var(Message(cast(str, msg)), var_dict)], None
 
 
 message_matcher = on_message(
     rule=message_checker,
     block=config.autoreply_block,
     priority=config.autoreply_priority,
 )
```

### Comparing `nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/config.py` & `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import json
 from pathlib import Path
-from typing import Any, Dict, Generic, List, Literal, Optional, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
+import yaml
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
 DATA_PATH = Path.cwd() / "data" / "autoreply"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
+ALLOWED_SUFFIXES = (".json", ".yml", ".yaml")
 
 MatchType = Union[str, "MatchModel"]
 ReplyType = Union[str, List["MessageSegmentModel"], "ReplyModel"]
 MessageType = Union[str, List["MessageSegmentModel"], List[ReplyType]]
 
 
 class MatchModel(BaseModel):
@@ -74,30 +87,45 @@
     autoreply_priority: int = 99
 
 
 replies: List[ReplyEntryModel] = []
 config = ConfigModel.parse_obj(get_driver().config)
 
 
+def iter_config_path(root_path: Path = DATA_PATH) -> Iterator[Path]:
+    for path in root_path.iterdir():
+        if path.is_dir():
+            yield from iter_config_path(path)
+
+        if path.is_file() and (path.suffix in ALLOWED_SUFFIXES):
+            yield path
+
+
+def load_config(path: Path) -> List[ReplyEntryModel]:
+    content = path.read_text(encoding="u8")
+
+    if path.suffix in (".yml", ".yaml"):
+        obj: list = yaml.load(content, Loader=yaml.FullLoader)
+    else:
+        obj: list = json.loads(content)
+
+    return [ReplyEntryModel(**x) for x in obj]
+
+
 def reload_replies() -> Tuple[int, int]:
     replies.clear()
 
     success = 0
     fail = 0
 
-    for json_path in DATA_PATH.glob("*.json"):
-        file_name = json_path.name
+    for path in iter_config_path():
+        file_name = path.name
 
         try:
-            replies.extend(
-                [
-                    ReplyEntryModel(**x)
-                    for x in json.loads(json_path.read_text(encoding="u8"))
-                ],
-            )
+            replies.extend(load_config(path))
 
         except Exception:
             logger.opt(colors=True).exception(
                 f"加载回复配置 <y>{file_name}</y> <l><r>失败</r></l>",
             )
             fail += 1
```

### Comparing `nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/util.py` & `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Tuple, Union, cast
 
 from nonebot.adapters.onebot.v11 import (
     Bot,
     GroupMessageEvent,
+    Message,
     MessageEvent,
+    MessageSegment,
     PokeNotifyEvent,
 )
 
-from .config import MessageSegmentModel
+VarDictType = Tuple[Dict[str, Any], Dict[str, Any]]
 
 
 async def get_var_dict(
     bot: Bot,
     event: Union[MessageEvent, PokeNotifyEvent],
-) -> Dict[str, Any]:
+) -> VarDictType:
     is_message = isinstance(event, MessageEvent)
     is_group = isinstance(event, GroupMessageEvent)
     is_poke = isinstance(event, PokeNotifyEvent)
 
+    message_id = event.message_id if is_message else None
     user_id = event.user_id
     group_id = event.group_id if is_group or is_poke else None
 
     if is_poke:
         sender = (
             await bot.get_group_member_info(group_id=group_id, user_id=user_id)
             if group_id
@@ -31,35 +34,40 @@
         card = sender.get("card")
 
     else:
         sender = event.sender
         nickname = sender.nickname
         card = sender.card
 
-    return {
+    normal_var = {
+        "bs": "{",
+        "be": "}",
         "self_id": event.self_id,
-        "message_id": event.message_id if is_message else None,
+        "message_id": message_id,
         "user_id": user_id,
         "group_id": group_id,
         "target_id": event.target_id if is_poke else None,
         "nickname": nickname,
         "card": card,
         "display_name": card or nickname,
     }
+    seg_var = {
+        "at": MessageSegment.at(user_id),
+        "reply": MessageSegment.reply(message_id) if message_id else None,
+    }
+    return normal_var, seg_var
 
 
-def replace_str_var(string: str, var_dict: Dict[str, Any]) -> str:
-    return string.format(**var_dict)
-
-
-def replace_segment_var(
-    segments: Iterable[MessageSegmentModel],
-    var_dict: Dict[str, Any],
-) -> List[MessageSegmentModel]:
-    segments = [x.copy(deep=True) for x in segments]
-
-    for seg in segments:
-        for k, v in seg.data.items():
-            if isinstance(v, str):
-                seg.data[k] = replace_str_var(v, var_dict)
+def replace_message_var(message: Message, var_dict: VarDictType) -> Message:
+    normal_var, seg_var = var_dict
+    message = cast(
+        Message,
+        Message.template(message).format_map({**normal_var, **seg_var}),
+    )
+
+    for seg in message:
+        if not seg.is_text():
+            for k, v in seg.data.items():
+                if isinstance(v, str):
+                    seg.data[k] = v.format(**normal_var)
 
-    return segments
+    return message
```

### Comparing `nonebot_plugin_autoreply-0.2.7/pyproject.toml` & `nonebot_plugin_autoreply-0.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "nonebot-plugin-autoreply"
-version = "0.2.7"
+version = "0.2.8"
 description = "A powerful auto reply plugin for NoneBot2"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc1",
     "pydantic>=1.10.4",
     "nonebot-adapter-onebot>=2.1.0",
     "typing-extensions>=4.4.0",
+    "PyYAML>=6.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_autoreply-0.2.7/PKG-INFO` & `nonebot_plugin_autoreply-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-autoreply
-Version: 0.2.7
+Version: 0.2.8
 Summary: A powerful auto reply plugin for NoneBot2
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0rc1
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: nonebot-adapter-onebot>=2.1.0
 Requires-Dist: typing-extensions>=4.4.0
+Requires-Dist: PyYAML>=6.0
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
@@ -121,15 +122,15 @@
 </details>
 
 ## ⚙️ 配置
 
 ### 回复配置
 
 插件的配置文件位于 `data/autoreply` 下  
-在里面新建一个 `json` 后缀文件即可开始配置
+在里面新建一个 `yml` 或 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
     // 该组配置是否阻塞其他回复配置
@@ -287,26 +288,30 @@
   }
 
   // ...
 ]
 ```
 
 插件提供了一些变量，他们可以被用在 `normal` 和 `array` 类型的消息，以及 `multi` 类型中嵌套的这两个类型的消息中；`plain` 类型的消息则无法使用变量  
-变量使用 `str.format()` 方法替换，所以如果想要转义 `{` 或 `}`，使用 `{{` 或 `}}` 即可
+变量使用 [`MessageTemplate.format_map()`](https://v2.nonebot.dev/docs/tutorial/message#%E4%BD%BF%E7%94%A8%E6%B6%88%E6%81%AF%E6%A8%A1%E6%9D%BF) 方法替换
 
 下面是插件提供的变量列表
 
+- `{bs}` - “`{`”，转义用
+- `{be}` - “`}`”，转义用
 - `{self_id}` - 机器人 QQ
 - `{message_id}` - 消息 ID _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 - `{user_id}` - 发送者 QQ
 - `{group_id}` - 消息来源群号 _（私聊等为 `None`）_
 - `{target_id}` - 被戳者 QQ _（仅当 `match` 的 `type` 为 `poke` 时有值，其他情况为 `None`）_
 - `{nickname}` - 发送者昵称
 - `{card}` - 发送者群名片
 - `{display_name}` - 发送者显示名称 _（优先群名片，当群名片为空时为昵称）_
+- `{at}` - 艾特发送者
+- `{reply}` - 回复发送者 _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 
 下面放出几个示例，帮助大家更好的理解如何使用变量
 
 ```jsonc
 [
   {
     "matches": [
@@ -353,17 +358,17 @@
           "[multi] 我刚刚 At 了一下你哦~ 收到了吗？"
         ]
       },
 
       // 无法在 plain 类型消息中使用，{user_id}、{nickname} 会原样显示
       "@[plain] [CQ:at,qq={user_id}] 啊咧？怎么 At 不了 {nickname}？",
 
-      // 可以在消息中使用 {{ 和 }} 来转义大括号
+      // 可以在消息中使用 {bs｝ 和 {be} 来转义大括号
       // 前面的 {{user_id}} 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
-      "[normal] [CQ:at,qq={{user_id}}] 啊咧？怎么 At 不了 {nickname}？"
+      "[normal] [CQ:at,qq={bs}user_id{be}] 啊咧？怎么 At 不了 {nickname}？"
     ]
   }
 ]
 ```
 
 ### 常规配置
 
@@ -401,20 +406,27 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.8
+
+- 支持解析 `yaml` 格式配置，会将 `.yml` 和 `.yaml` 的文件作为 `yaml` 格式配置加载
+- 现在会寻找 `data/autoreply` 文件夹下所有子文件夹中的配置并加载
+- 新增变量 `{at}`、`{reply}`
+- 换用 `MessageTemplate` 格式化变量；由于这玩意不支持 `{{` 及 `}}` 转义，所以加入了变量 `{bs}` 和 `{be}`
+
 ### 0.2.7
 
 - 新增了配置的 `block` 和 `priority` 属性
 - 新增 `type` 为 `poke` (双击头像，戳一戳) 的 `match`
 - 新增了 `match` 的 `possibility` 属性
-- 新增了 `{display_name}` 变量
+- 新增了 `{target_id}` 与 `{display_name}` 变量
 
 ### 0.2.6
 
 - 回复中可以使用变量了
 - 新增配置市场
 
 ### 0.2.5
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.7 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.8 Summary: A
 powerful auto reply plugin for NoneBot2 Home-page: https://github.com/lgc-
 NB2Dev/nonebot-plugin-autoreply Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-autoreply Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0rc1 Requires-Dist: pydantic>=1.10.4 Requires-Dist: nonebot-
-adapter-onebot>=2.1.0 Requires-Dist: typing-extensions>=4.4.0 Description-
-Content-Type: text/markdown
+adapter-onebot>=2.1.0 Requires-Dist: typing-extensions>=4.4.0 Requires-Dist:
+PyYAML>=6.0 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-AutoReply _â¨ èªå¨åå¤ â¨_ [license] [pypi] [python]
                           [pypi_download] [wakatime]
 ## ð åå¤å¸åº ![market](https://raw.githubusercontent.com/lgc-NB2Dev/
 readme/main/autoreply/QQæªå¾20230423192951.png) ### [ç¹å»è¿å¥](https://
 autoreply.lgc2333.top) æä»¬çåå¤éç½®å¸åºä¸çº¿å¦~
@@ -30,16 +30,16 @@
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-autoreply ```   pdm ```bash pdm add nonebot-plugin-
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
-æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
-åç¼æä»¶å³å¯å¼å§éç½®
+æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `yml`
+æ `json` åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
 ```jsonc [ { // è¯¥ç»éç½®æ¯å¦é»å¡å¶ä»åå¤éç½® /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "block": true, /
 / è¯¥ç»éç½®çä¼åçº§ï¼è¶å¤§è¶é« // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1
 "priority": 1, // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
 / å¹éæ¨¡å¼ï¼å¯é `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`
 (æ­£åå¹é)ã`poke`(åå»å¤´åæ³ä¸æ³) // // ä½¿ç¨ `poke`
@@ -95,53 +95,63 @@
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå "users": { /
 / é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå) "type":
 "black", // è¦è¿æ»¤çQQå· "values": [ 1145141919, 9191415411 /
 / æ´å¤QQå·... ] } } // ... ] ```
 æä»¶æä¾äºä¸äºåéï¼ä»ä»¬å¯ä»¥è¢«ç¨å¨ `normal` å `array`
 ç±»åçæ¶æ¯ï¼ä»¥å `multi`
 ç±»åä¸­åµå¥çè¿ä¸¤ä¸ªç±»åçæ¶æ¯ä¸­ï¼`plain`
-ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ `str.format()`
-æ¹æ³æ¿æ¢ï¼æä»¥å¦ææ³è¦è½¬ä¹ `{` æ `}`ï¼ä½¿ç¨ `{{` æ `}}`
-å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ - `
-{message_id}` - æ¶æ¯ ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º
-`None`ï¼_ - `{user_id}` - åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å·
-_ï¼ç§èç­ä¸º `None`ï¼_ - `{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match`
-ç `type` ä¸º `poke` æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` -
-åéèæµç§° - `{card}` - åéèç¾¤åç - `{display_name}` -
-åéèæ¾ç¤ºåç§° _ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_
+ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ [`MessageTemplate.format_map
+()`](https://v2.nonebot.dev/docs/tutorial/
+message#%E4%BD%BF%E7%94%A8%E6%B6%88%E6%81%AF%E6%A8%A1%E6%9D%BF) æ¹æ³æ¿æ¢
+ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{bs}` - â`{`âï¼è½¬ä¹ç¨ - `{be}`
+- â`}`âï¼è½¬ä¹ç¨ - `{self_id}` - æºå¨äºº QQ - `{message_id}` - æ¶æ¯
+ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º `None`ï¼_ - `{user_id}` -
+åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å· _ï¼ç§èç­ä¸º `None`ï¼_ -
+`{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match` ç `type` ä¸º `poke`
+æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` - åéèæµç§° - `
+{card}` - åéèç¾¤åç - `{display_name}` - åéèæ¾ç¤ºåç§°
+_ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_ - `{at}` -
+è¾ç¹åéè - `{reply}` - åå¤åéè _ï¼å½ `match` ç `type` ä¸º
+`poke` æ¶ä¸º `None`ï¼_
 ä¸é¢æ¾åºå ä¸ªç¤ºä¾ï¼å¸®å©å¤§å®¶æ´å¥½ççè§£å¦ä½ä½¿ç¨åé
 ```jsonc [ { "matches": [ { "match": "^(@|at|è¾ç¹)æ$", "type": "regex" } ],
 "replies": [ // å¨ normal ç±»åæ¶æ¯ä¸­ä½¿ç¨ "[normal] Atäº [CQ:at,qq=
 {user_id}]", // å¨ array ç±»åæ¶æ¯ä¸­ä½¿ç¨ [ { "type": "text", "data":
 { "text": "[array] Atäº " } }, { "type": "at", "data": { "qq": "{user_id}" } }
 ], // å¨ multi ç±»åæ¶æ¯ä¸­ä½¿ç¨ { "type": "multi", "message": [ /
 / åµå¥ç array ç±»åæ¶æ¯ [ { "type": "at", "data": { "qq": "{user_id}" }
 } ], // åµå¥ç normal ç±»åæ¶æ¯ "[multi] æåå At äºä¸ä¸ä½ å¦~
 æ¶å°äºåï¼" ] }, // æ æ³å¨ plain ç±»åæ¶æ¯ä¸­ä½¿ç¨ï¼{user_id}ã
 {nickname} ä¼åæ ·æ¾ç¤º "@[plain] [CQ:at,qq={user_id}] åå§ï¼æä¹ At
-ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {{ å }} æ¥è½¬ä¹å¤§æ¬å·
-// åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
-{nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={{user_id}}] åå§ï¼æä¹ At
-ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
+ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {bsï½ å {be}
+æ¥è½¬ä¹å¤§æ¬å· // åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id}
+åéï¼èåé¢ç {nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={bs}user_id
+{be}] åå§ï¼æä¹ At ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
 ä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
 éç½®é¡¹è¯·åèä¸é¢çææ¬ ```ini # matcher æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤
 False AUTOREPLY_BLOCK=False # matcher ä¼åçº§ AUTOREPLY_PRIORITY=99 ``` ##
 ð¬ æä»¤ ### `éè½½èªå¨åå¤`
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.7 - æ°å¢äºéç½®ç `block`
-å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke` (åå»å¤´åï¼æ³ä¸æ³) ç
-`match` - æ°å¢äº `match` ç `possibility` å±æ§ - æ°å¢äº `
-{display_name}` åé ### 0.2.6 - åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº -
-æ°å¢éç½®å¸åº ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.8 - æ¯æè§£æ `yaml`
+æ ¼å¼éç½®ï¼ä¼å° `.yml` å `.yaml` çæä»¶ä½ä¸º `yaml`
+æ ¼å¼éç½®å è½½ - ç°å¨ä¼å¯»æ¾ `data/autoreply`
+æä»¶å¤¹ä¸ææå­æä»¶å¤¹ä¸­çéç½®å¹¶å è½½ - æ°å¢åé `{at}`ã`
+{reply}` - æ¢ç¨ `MessageTemplate` æ ¼å¼ååéï¼ç±äºè¿ç©æä¸æ¯æ
+`{{` å `}}` è½¬ä¹ï¼æä»¥å å¥äºåé `{bs}` å `{be}` ### 0.2.7 -
+æ°å¢äºéç½®ç `block` å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke`
+(åå»å¤´åï¼æ³ä¸æ³) ç `match` - æ°å¢äº `match` ç `possibility`
+å±æ§ - æ°å¢äº `{target_id}` ä¸ `{display_name}` åé ### 0.2.6 -
+åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº - æ°å¢éç½®å¸åº ### 0.2.5 -
+å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
 è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
 å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
```


# Comparing `tmp/nonebot_plugin_genshin_cos-0.1.5.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.1.5.tar` & `nonebot_plugin_genshin_cos-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.5/LICENSE
--rw-r--r--   0        0        0     5396 2023-04-01 02:27:29.605425 nonebot_plugin_genshin_cos-0.1.5/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      220 2023-03-31 05:27:22.348015 nonebot_plugin_genshin_cos-0.1.5/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0     4830 2023-04-03 05:26:02.301862 nonebot_plugin_genshin_cos-0.1.5/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      660 2023-04-03 07:35:15.863213 nonebot_plugin_genshin_cos-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2927 2023-03-31 05:31:42.641333 nonebot_plugin_genshin_cos-0.1.5/README.md
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8850 2023-04-27 04:40:34.852336 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-27 05:00:12.292105 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-04-08 07:01:06.461588 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    11030 2023-04-27 04:58:22.298726 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      661 2023-04-27 05:06:50.988254 nonebot_plugin_genshin_cos-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3634 2023-04-27 05:19:54.659437 nonebot_plugin_genshin_cos-0.1.6/README.md
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.1.5/LICENSE` & `nonebot_plugin_genshin_cos-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.5/pyproject.toml` & `nonebot_plugin_genshin_cos-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nonebot-plugin-genshin-cos"
-version = "0.1.5"
+version = "0.1.6"
 description = "米游社原神cos图获取"
-authors = ["divandia <106718176+Cvandia@users.noreply.github.com>"]
+authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_genshin_cos"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 nonebot2 = ">=2.0.0-beta.1"
 nonebot-adapter-onebot = ">=2.0.0-beta.1"
 httpx = ">=0.19.0"
 nonebot-plugin-apscheduler= ">=0.1.3"
 aiofiles = ">=0.7.0"
 pydantic = ">=1.10.2"
 pathlib = ">=1.0.1"
 ujson = ">=5.5.0"
-requests = ">=2.28.1"
+playwright = ">=1.30.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_genshin_cos-0.1.5/README.md` & `nonebot_plugin_genshin_cos-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 
-
-
 <div align="center">
 
-<a href="https://v2.nonebot.dev/store"><img src="https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+<a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 
 </div>
 
 <div align="center">
 
 # nonebot-plugin-genshin-cos
 
@@ -38,70 +36,89 @@
 <summary>安装</summary>
 
 pip 安装
 
 ```
 pip install nonebot-plugin-genshin-cos
 ```
+- 在nonebot的pyproject.toml中的plugins = ["xxx"]添加此插件
 
 nb-cli安装
 
 ```
 nb plugin install nonebot-plugin-genshin-cos --upgrade
 ```
+
+git clone安装(不推荐)
+
+- 运行
+```git clone https://github.com/Cvandia/nonebot_plugin_genshin_cos```
+- 在运行处
+把文件夹`nonebot-plugin-genshen-cos`复制到bot根目录下的`src/plugins`(或者你创建bot时的其他名称`xxx/plugins`)
+
  
  </details>
  
  <details>
  <summary>注意</summary>
  
  推荐镜像站下载
   
  清华源```https://pypi.tuna.tsinghua.edu.cn/simple```
  
  阿里源```https://mirrors.aliyun.com/pypi/simple/```
- 
+
+
+ 安装完后记得执行一下：
+ ```playwright install```
+~~懒，没写自动下载chrome~~ 
 </details>
 
 
 ## ⚙️ 配置
 ### 在env.中添加以下配置
 
 | 配置 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:---:|
 |cos_max|int|5|最大返回cos图片数量|
-|cos_path|str|无|不配置则默认下载到bot根目录的```"data/genshin_cos"```,支持绝对路劲如```"C:/Users/image"```和相对bot根目录路劲如```"coser/image"```
-|cos_cd|int|10|用户触发cd|
+|cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
+|cos_cd|int|30|用户触发cd|
+|cos_time_out|int|60|cosplus用户超时时间|
+|cos_swipe_time|int|1|获取页面的时间，时间越长图片越多|
 
 > 注意：绝对路劲中用`/`，用`\`可能会被转义
 
 ## ⭐ 使用
 
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
 |:-----:|:----:|:----:|:----:|:----:|
-|原神cos|否|私聊、群聊|随机发送x张cos图，如：/米游社cos x3|任何|
-|下载cos|否|私聊、群聊|爬取cos图片至本地,如：/下载cos|超管|
-
+|原神cos|否|私聊、群聊|随机发送x张cos图，如：米游社cos x3|任何|
+|下载cos|否|私聊、群聊|爬取cos图片至本地,如：下载cos|超管|
+|cosplus|否|私聊、群聊|通过playwright获取cos图|任何|
+|xmx|否|私聊、群聊|？？？？？s|超管|
 **注意**
 
-默认情况下, 您应该在指令前加上命令前缀, 通常是 /
+指令触发方式是正则匹配的，不需要加指令前缀
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
  - [x] 保存cos图
  - [x] 内置cd和用户触发上限
  - [x] 合并转发发送多张cos图
+ - [x] playwright获取cos图
  - [ ] 选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）
 
 
 --- 喜欢记得点个star⭐---
 
 ## ❗免责声明
 
 图片版权归米游社原神cos社区所属，请尊重
 coser的创作权
 
+
+
 ## 💝 鸣谢
 
-- [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
+- [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
```

#### html2text {}

```diff
@@ -5,29 +5,41 @@
 QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
                     img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» åå°[æç¨](https://juejin.cn/post/
 6990320268010848286)çå¯åï¼æä»¥åäºè¿ä¸ªæä»¶ï¼æ´å¤åè½åç»­æ´æ°~~æå¾æï¼å­¦ä¸é~~
   ### æèä½ æå¥å³äºè¯¥æä»¶çæ°æ³æ³çï¼å¯ä»¥æissueæèpr
                                      (>A<)
 ## ð¿ å®è£  å®è£ pip å®è£ ``` pip install nonebot-plugin-genshin-cos
-``` nb-cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ```
-æ³¨æ æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/
-simple``` é¿éæº```https://mirrors.aliyun.com/pypi/simple/```  ## âï¸
-éç½® ### å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ
-| |:-----:|:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
-|cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç```"data/
-genshin_cos"```,æ¯æç»å¯¹è·¯å²å¦```"C:/Users/
-image"```åç¸å¯¹botæ ¹ç®å½è·¯å²å¦```"coser/image"```
-|cos_cd|int|10|ç¨æ·è§¦åcd| > æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/
-`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ### æä»¤ï¼ | æä»¤ | éè¦@ |
-èå´ | è¯´æ |æé| |:-----:|:----:|:----:|:----:|:----:
-| |åç¥cos|å¦|ç§èãç¾¤è|éæºåéxå¼ coså¾ï¼å¦ï¼/ç±³æ¸¸ç¤¾cos
-x3|ä»»ä½| |ä¸è½½cos|å¦|ç§èãç¾¤è|ç¬åcoså¾çè³æ¬å°,å¦ï¼/
-ä¸è½½cos|è¶ç®¡| **æ³¨æ** é»è®¤æåµä¸,
-æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ## ð æªæ¥ - [x]
-ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
+``` - å¨nonebotçpyproject.tomlä¸­çplugins = ["xxx"]æ·»å æ­¤æä»¶ nb-
+cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ``` git
+cloneå®è£(ä¸æ¨è) - è¿è¡ ```git clone https://github.com/Cvandia/
+nonebot_plugin_genshin_cos``` - å¨è¿è¡å¤ ææä»¶å¤¹`nonebot-plugin-
+genshen-cos`å¤å¶å°botæ ¹ç®å½ä¸ç`src/plugins`
+(æèä½ åå»ºbotæ¶çå¶ä»åç§°`xxx/plugins`)   æ³¨æ
+æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/simple```
+é¿éæº```https://mirrors.aliyun.com/pypi/simple/```
+å®è£å®åè®°å¾æ§è¡ä¸ä¸ï¼ ```playwright install```
+~~æï¼æ²¡åèªå¨ä¸è½½chrome~~  ## âï¸ éç½® ###
+å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:
+|:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
+|cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç`"data/
+genshin_cos"`,æ¯æç»å¯¹è·¯å²å¦`"C:/Users/
+image"`åç¸å¯¹botæ ¹ç®å½è·¯å²å¦`"coser/image"`
+|cos_cd|int|30|ç¨æ·è§¦åcd| |cos_time_out|int|60|cosplusç¨æ·è¶æ¶æ¶é´|
+|cos_swipe_time|int|1|è·åé¡µé¢çæ¶é´ï¼æ¶é´è¶é¿å¾çè¶å¤| >
+æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ###
+æä»¤ï¼ | æä»¤ | éè¦@ | èå´ | è¯´æ |æé| |:-----:|:----:|:----:
+|:----:|:----:
+| |åç¥cos|å¦|ç§èãç¾¤è|éæºåéxå¼ coså¾ï¼å¦ï¼ç±³æ¸¸ç¤¾cos
+x3|ä»»ä½|
+|ä¸è½½cos|å¦|ç§èãç¾¤è|ç¬åcoså¾çè³æ¬å°,å¦ï¼ä¸è½½cos|è¶ç®¡|
+|cosplus|å¦|ç§èãç¾¤è|éè¿playwrightè·åcoså¾|ä»»ä½|
+|xmx|å¦|ç§èãç¾¤è|ï¼ï¼ï¼ï¼ï¼s|è¶ç®¡| **æ³¨æ**
+æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ## ð æªæ¥
+- [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
 ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é - [x]
-åå¹¶è½¬ååéå¤å¼ coså¾ - [ ] éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é)
-or å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼ --- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ##
-âåè´£å£°æ å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é
-coserçåä½æ ## ð é¸£è°¢ - [Nonebot](https://github.com/nonebot/
-nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
+åå¹¶è½¬ååéå¤å¼ coså¾ - [x] playwrightè·åcoså¾ - [ ]
+éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é) or å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼
+--- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ## âåè´£å£°æ
+å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é coserçåä½æ ##
+ð é¸£è°¢ - [x] [Nonebot](https://github.com/nonebot/nonebot2):
+æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
```

### Comparing `nonebot_plugin_genshin_cos-0.1.5/PKG-INFO` & `nonebot_plugin_genshin_cos-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.1.5
+Version: 0.1.6
 Summary: 米游社原神cos图获取
 License: MIT
-Author: divandia
+Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0)
 Requires-Dist: httpx (>=0.19.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.1.3)
 Requires-Dist: nonebot2 (>=2.0.0-beta.1)
 Requires-Dist: pathlib (>=1.0.1)
+Requires-Dist: playwright (>=1.30.0)
 Requires-Dist: pydantic (>=1.10.2)
-Requires-Dist: requests (>=2.28.1)
 Requires-Dist: ujson (>=5.5.0)
 Description-Content-Type: text/markdown
 
 
-
-
 <div align="center">
 
-<a href="https://v2.nonebot.dev/store"><img src="https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+<a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 
 </div>
 
 <div align="center">
 
 # nonebot-plugin-genshin-cos
 
@@ -63,71 +61,90 @@
 <summary>安装</summary>
 
 pip 安装
 
 ```
 pip install nonebot-plugin-genshin-cos
 ```
+- 在nonebot的pyproject.toml中的plugins = ["xxx"]添加此插件
 
 nb-cli安装
 
 ```
 nb plugin install nonebot-plugin-genshin-cos --upgrade
 ```
+
+git clone安装(不推荐)
+
+- 运行
+```git clone https://github.com/Cvandia/nonebot_plugin_genshin_cos```
+- 在运行处
+把文件夹`nonebot-plugin-genshen-cos`复制到bot根目录下的`src/plugins`(或者你创建bot时的其他名称`xxx/plugins`)
+
  
  </details>
  
  <details>
  <summary>注意</summary>
  
  推荐镜像站下载
   
  清华源```https://pypi.tuna.tsinghua.edu.cn/simple```
  
  阿里源```https://mirrors.aliyun.com/pypi/simple/```
- 
+
+
+ 安装完后记得执行一下：
+ ```playwright install```
+~~懒，没写自动下载chrome~~ 
 </details>
 
 
 ## ⚙️ 配置
 ### 在env.中添加以下配置
 
 | 配置 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:---:|
 |cos_max|int|5|最大返回cos图片数量|
-|cos_path|str|无|不配置则默认下载到bot根目录的```"data/genshin_cos"```,支持绝对路劲如```"C:/Users/image"```和相对bot根目录路劲如```"coser/image"```
-|cos_cd|int|10|用户触发cd|
+|cos_path|str|无|不配置则默认下载到bot根目录的`"data/genshin_cos"`,支持绝对路劲如`"C:/Users/image"`和相对bot根目录路劲如`"coser/image"`
+|cos_cd|int|30|用户触发cd|
+|cos_time_out|int|60|cosplus用户超时时间|
+|cos_swipe_time|int|1|获取页面的时间，时间越长图片越多|
 
 > 注意：绝对路劲中用`/`，用`\`可能会被转义
 
 ## ⭐ 使用
 
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
 |:-----:|:----:|:----:|:----:|:----:|
-|原神cos|否|私聊、群聊|随机发送x张cos图，如：/米游社cos x3|任何|
-|下载cos|否|私聊、群聊|爬取cos图片至本地,如：/下载cos|超管|
-
+|原神cos|否|私聊、群聊|随机发送x张cos图，如：米游社cos x3|任何|
+|下载cos|否|私聊、群聊|爬取cos图片至本地,如：下载cos|超管|
+|cosplus|否|私聊、群聊|通过playwright获取cos图|任何|
+|xmx|否|私聊、群聊|？？？？？s|超管|
 **注意**
 
-默认情况下, 您应该在指令前加上命令前缀, 通常是 /
+指令触发方式是正则匹配的，不需要加指令前缀
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
  - [x] 保存cos图
  - [x] 内置cd和用户触发上限
  - [x] 合并转发发送多张cos图
+ - [x] playwright获取cos图
  - [ ] 选择发送图库方式：离线 (迅速) or 在线（缓慢、目前是的）
 
 
 --- 喜欢记得点个star⭐---
 
 ## ❗免责声明
 
 图片版权归米游社原神cos社区所属，请尊重
 coser的创作权
 
+
+
 ## 💝 鸣谢
 
-- [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
+- [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
```

#### html2text {}

```diff
@@ -1,46 +1,58 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.5 Summary:
-ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: divandia Author-email:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.6 Summary:
+ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0-beta.1) Requires-Dist: nonebot-plugin-
 apscheduler (>=0.1.3) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
-pathlib (>=1.0.1) Requires-Dist: pydantic (>=1.10.2) Requires-Dist: requests
-(>=2.28.1) Requires-Dist: ujson (>=5.5.0) Description-Content-Type: text/
+pathlib (>=1.0.1) Requires-Dist: playwright (>=1.30.0) Requires-Dist: pydantic
+(>=1.10.2) Requires-Dist: ujson (>=5.5.0) Description-Content-Type: text/
 markdown
                               [NoneBotPluginLogo]
                          # nonebot-plugin-genshin-cos
           _â­åºäºNonebot2çä¸æ¬¾è·åç±³æ¸¸ç¤¾cosçæä»¶â­_
 [https://img.shields.io/badge/python-3.8+-blue] [https://img.shields.io/badge/
 QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
                     img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» åå°[æç¨](https://juejin.cn/post/
 6990320268010848286)çå¯åï¼æä»¥åäºè¿ä¸ªæä»¶ï¼æ´å¤åè½åç»­æ´æ°~~æå¾æï¼å­¦ä¸é~~
   ### æèä½ æå¥å³äºè¯¥æä»¶çæ°æ³æ³çï¼å¯ä»¥æissueæèpr
                                      (>A<)
 ## ð¿ å®è£  å®è£ pip å®è£ ``` pip install nonebot-plugin-genshin-cos
-``` nb-cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ```
-æ³¨æ æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/
-simple``` é¿éæº```https://mirrors.aliyun.com/pypi/simple/```  ## âï¸
-éç½® ### å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ
-| |:-----:|:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
-|cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç```"data/
-genshin_cos"```,æ¯æç»å¯¹è·¯å²å¦```"C:/Users/
-image"```åç¸å¯¹botæ ¹ç®å½è·¯å²å¦```"coser/image"```
-|cos_cd|int|10|ç¨æ·è§¦åcd| > æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/
-`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ### æä»¤ï¼ | æä»¤ | éè¦@ |
-èå´ | è¯´æ |æé| |:-----:|:----:|:----:|:----:|:----:
-| |åç¥cos|å¦|ç§èãç¾¤è|éæºåéxå¼ coså¾ï¼å¦ï¼/ç±³æ¸¸ç¤¾cos
-x3|ä»»ä½| |ä¸è½½cos|å¦|ç§èãç¾¤è|ç¬åcoså¾çè³æ¬å°,å¦ï¼/
-ä¸è½½cos|è¶ç®¡| **æ³¨æ** é»è®¤æåµä¸,
-æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ## ð æªæ¥ - [x]
-ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
+``` - å¨nonebotçpyproject.tomlä¸­çplugins = ["xxx"]æ·»å æ­¤æä»¶ nb-
+cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ``` git
+cloneå®è£(ä¸æ¨è) - è¿è¡ ```git clone https://github.com/Cvandia/
+nonebot_plugin_genshin_cos``` - å¨è¿è¡å¤ ææä»¶å¤¹`nonebot-plugin-
+genshen-cos`å¤å¶å°botæ ¹ç®å½ä¸ç`src/plugins`
+(æèä½ åå»ºbotæ¶çå¶ä»åç§°`xxx/plugins`)   æ³¨æ
+æ¨èéåç«ä¸è½½ æ¸åæº```https://pypi.tuna.tsinghua.edu.cn/simple```
+é¿éæº```https://mirrors.aliyun.com/pypi/simple/```
+å®è£å®åè®°å¾æ§è¡ä¸ä¸ï¼ ```playwright install```
+~~æï¼æ²¡åèªå¨ä¸è½½chrome~~  ## âï¸ éç½® ###
+å¨env.ä¸­æ·»å ä»¥ä¸éç½® | éç½® | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:
+|:----:|:----:|:---:| |cos_max|int|5|æå¤§è¿åcoså¾çæ°é|
+|cos_path|str|æ |ä¸éç½®åé»è®¤ä¸è½½å°botæ ¹ç®å½ç`"data/
+genshin_cos"`,æ¯æç»å¯¹è·¯å²å¦`"C:/Users/
+image"`åç¸å¯¹botæ ¹ç®å½è·¯å²å¦`"coser/image"`
+|cos_cd|int|30|ç¨æ·è§¦åcd| |cos_time_out|int|60|cosplusç¨æ·è¶æ¶æ¶é´|
+|cos_swipe_time|int|1|è·åé¡µé¢çæ¶é´ï¼æ¶é´è¶é¿å¾çè¶å¤| >
+æ³¨æï¼ç»å¯¹è·¯å²ä¸­ç¨`/`ï¼ç¨`\`å¯è½ä¼è¢«è½¬ä¹ ## â­ ä½¿ç¨ ###
+æä»¤ï¼ | æä»¤ | éè¦@ | èå´ | è¯´æ |æé| |:-----:|:----:|:----:
+|:----:|:----:
+| |åç¥cos|å¦|ç§èãç¾¤è|éæºåéxå¼ coså¾ï¼å¦ï¼ç±³æ¸¸ç¤¾cos
+x3|ä»»ä½|
+|ä¸è½½cos|å¦|ç§èãç¾¤è|ç¬åcoså¾çè³æ¬å°,å¦ï¼ä¸è½½cos|è¶ç®¡|
+|cosplus|å¦|ç§èãç¾¤è|éè¿playwrightè·åcoså¾|ä»»ä½|
+|xmx|å¦|ç§èãç¾¤è|ï¼ï¼ï¼ï¼ï¼s|è¶ç®¡| **æ³¨æ**
+æä»¤è§¦åæ¹å¼æ¯æ­£åå¹éçï¼ä¸éè¦å æä»¤åç¼ ## ð æªæ¥
+- [x] ç¼æ¢æ´æ°ï¼æè¿å­¦ä¸ç¹å¿å¦~ - [x] éæºåécoså¾ç - [x]
 ä¿å­coså¾ - [x] åç½®cdåç¨æ·è§¦åä¸é - [x]
-åå¹¶è½¬ååéå¤å¼ coså¾ - [ ] éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é)
-or å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼ --- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ##
-âåè´£å£°æ å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é
-coserçåä½æ ## ð é¸£è°¢ - [Nonebot](https://github.com/nonebot/
-nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
+åå¹¶è½¬ååéå¤å¼ coså¾ - [x] playwrightè·åcoså¾ - [ ]
+éæ©åéå¾åºæ¹å¼ï¼ç¦»çº¿ (è¿é) or å¨çº¿ï¼ç¼æ¢ãç®åæ¯çï¼
+--- åæ¬¢è®°å¾ç¹ä¸ªstarâ­--- ## âåè´£å£°æ
+å¾ççæå½ç±³æ¸¸ç¤¾åç¥cosç¤¾åºæå±ï¼è¯·å°é coserçåä½æ ##
+ð é¸£è°¢ - [x] [Nonebot](https://github.com/nonebot/nonebot2):
+æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
```


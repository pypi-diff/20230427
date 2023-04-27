# Comparing `tmp/binance_candle-1.0.6.tar.gz` & `tmp/binance_candle-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/binance_candle-1.0.6.tar", last modified: Mon Mar  6 04:08:29 2023, max compression
+gzip compressed data, was "dist/binance_candle-1.0.7.tar", last modified: Thu Apr 27 05:55:45 2023, max compression
```

## Comparing `binance_candle-1.0.6.tar` & `binance_candle-1.0.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.984458 binance_candle-1.0.6/
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.965870 binance_candle-1.0.6/.idea/
--rw-r--r--   0 kzlknight   (501) staff       (20)      176 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/.gitignore
--rw-r--r--   0 kzlknight   (501) staff       (20)      284 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/binance_candle.iml
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.966607 binance_candle-1.0.6/.idea/inspectionProfiles/
--rw-r--r--   0 kzlknight   (501) staff       (20)     2511 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 kzlknight   (501) staff       (20)      174 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 kzlknight   (501) staff       (20)      186 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/misc.xml
--rw-r--r--   0 kzlknight   (501) staff       (20)      280 2023-02-01 07:19:35.000000 binance_candle-1.0.6/.idea/modules.xml
--rw-r--r--   0 kzlknight   (501) staff       (20)      180 2023-02-01 07:20:51.000000 binance_candle-1.0.6/.idea/vcs.xml
--rw-r--r--   0 kzlknight   (501) staff       (20)    45879 2023-03-06 04:08:29.984170 binance_candle-1.0.6/PKG-INFO
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.967412 binance_candle-1.0.6/binance_candle/
--rw-r--r--   0 kzlknight   (501) staff       (20)      296 2023-03-06 04:05:40.000000 binance_candle-1.0.6/binance_candle/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.970039 binance_candle-1.0.6/binance_candle/cmd/
--rw-r--r--   0 kzlknight   (501) staff       (20)       63 2023-01-28 22:40:46.000000 binance_candle-1.0.6/binance_candle/cmd/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.970401 binance_candle-1.0.6/binance_candle/code/
--rw-r--r--   0 kzlknight   (501) staff       (20)      580 2023-01-27 07:42:58.000000 binance_candle-1.0.6/binance_candle/code/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.976110 binance_candle-1.0.6/binance_candle/exception/
--rw-r--r--   0 kzlknight   (501) staff       (20)      193 2023-01-27 07:46:24.000000 binance_candle-1.0.6/binance_candle/exception/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      118 2023-01-27 07:43:48.000000 binance_candle-1.0.6/binance_candle/exception/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      164 2023-01-27 07:44:01.000000 binance_candle-1.0.6/binance_candle/exception/param.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      285 2023-01-27 07:44:20.000000 binance_candle-1.0.6/binance_candle/exception/req.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      164 2023-01-27 07:44:42.000000 binance_candle-1.0.6/binance_candle/exception/rule.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.977754 binance_candle-1.0.6/binance_candle/market/
--rw-r--r--   0 kzlknight   (501) staff       (20)     1081 2023-02-10 03:20:46.000000 binance_candle-1.0.6/binance_candle/market/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1580 2023-02-10 03:21:38.000000 binance_candle-1.0.6/binance_candle/market/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5181 2023-02-01 02:59:15.000000 binance_candle-1.0.6/binance_candle/market/exchange_info.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    20111 2023-03-06 04:05:20.000000 binance_candle-1.0.6/binance_candle/market/history_candle.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     3685 2023-02-07 09:32:27.000000 binance_candle-1.0.6/binance_candle/market/ticker.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.978610 binance_candle-1.0.6/binance_candle/server/
--rw-r--r--   0 kzlknight   (501) staff       (20)      611 2023-02-10 03:22:48.000000 binance_candle-1.0.6/binance_candle/server/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1743 2023-03-03 03:27:57.000000 binance_candle-1.0.6/binance_candle/server/rule.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    25918 2023-03-03 03:27:39.000000 binance_candle-1.0.6/binance_candle/server/server.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     2584 2023-01-30 03:08:21.000000 binance_candle-1.0.6/binance_candle/utils.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.969677 binance_candle-1.0.6/binance_candle.egg-info/
--rw-r--r--   0 kzlknight   (501) staff       (20)    45879 2023-03-06 04:08:29.000000 binance_candle-1.0.6/binance_candle.egg-info/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)     1441 2023-03-06 04:08:29.000000 binance_candle-1.0.6/binance_candle.egg-info/SOURCES.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-03-06 04:08:29.000000 binance_candle-1.0.6/binance_candle.egg-info/dependency_links.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       47 2023-03-06 04:08:29.000000 binance_candle-1.0.6/binance_candle.egg-info/requires.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       15 2023-03-06 04:08:29.000000 binance_candle-1.0.6/binance_candle.egg-info/top_level.txt
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.981487 binance_candle-1.0.6/example/
--rw-r--r--   0 kzlknight   (501) staff       (20)      475 2023-02-07 09:21:09.000000 binance_candle-1.0.6/example/1. Market 交易规范.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      851 2023-02-07 09:41:04.000000 binance_candle-1.0.6/example/10. Server 维护实时历史K线数据.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      398 2023-02-07 09:22:11.000000 binance_candle-1.0.6/example/2. Market  产品列表.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      474 2023-02-07 09:24:03.000000 binance_candle-1.0.6/example/3. Market 最佳挂单.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      488 2023-02-07 09:28:13.000000 binance_candle-1.0.6/example/4. Market 最新价格.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      335 2023-02-07 09:35:26.000000 binance_candle-1.0.6/example/5. Market 产品深度.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1045 2023-02-07 09:36:59.000000 binance_candle-1.0.6/example/6. Market 历史K线.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      758 2023-02-07 09:37:55.000000 binance_candle-1.0.6/example/7. Utils candle与df的转化.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      427 2023-02-07 09:38:44.000000 binance_candle-1.0.6/example/8. Server 下载历史K线.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      429 2023-02-07 09:39:56.000000 binance_candle-1.0.6/example/9. Server 每日下载历史K线.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    45253 2023-03-06 04:08:20.000000 binance_candle-1.0.6/readme.md
--rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-03-06 04:08:29.984540 binance_candle-1.0.6/setup.cfg
--rw-r--r--   0 kzlknight   (501) staff       (20)     2793 2023-03-06 04:06:08.000000 binance_candle-1.0.6/setup.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 04:08:29.983317 binance_candle-1.0.6/vx_images/
--rw-r--r--   0 kzlknight   (501) staff       (20)   184133 2023-02-01 06:47:17.000000 binance_candle-1.0.6/vx_images/176016628950838.png
--rw-r--r--   0 kzlknight   (501) staff       (20)    33022 2023-02-08 02:37:24.000000 binance_candle-1.0.6/vx_images/244075001625094.png
--rw-r--r--   0 kzlknight   (501) staff       (20)   319035 2023-02-08 02:32:48.000000 binance_candle-1.0.6/vx_images/480313210278479.png
--rw-r--r--   0 kzlknight   (501) staff       (20)   151185 2023-02-08 02:33:49.000000 binance_candle-1.0.6/vx_images/495193492836002.png
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.857876 binance_candle-1.0.7/
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.828137 binance_candle-1.0.7/.idea/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      176 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/.gitignore
+-rw-r--r--   0 kzlknight   (501) staff       (20)      284 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/binance_candle.iml
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.829033 binance_candle-1.0.7/.idea/inspectionProfiles/
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2511 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 kzlknight   (501) staff       (20)      174 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 kzlknight   (501) staff       (20)      186 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/misc.xml
+-rw-r--r--   0 kzlknight   (501) staff       (20)      280 2023-02-01 07:19:35.000000 binance_candle-1.0.7/.idea/modules.xml
+-rw-r--r--   0 kzlknight   (501) staff       (20)      180 2023-02-01 07:20:51.000000 binance_candle-1.0.7/.idea/vcs.xml
+-rw-r--r--   0 kzlknight   (501) staff       (20)    45879 2023-04-27 05:55:45.857372 binance_candle-1.0.7/PKG-INFO
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.830064 binance_candle-1.0.7/binance_candle/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      296 2023-04-27 05:40:49.000000 binance_candle-1.0.7/binance_candle/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.833454 binance_candle-1.0.7/binance_candle/cmd/
+-rw-r--r--   0 kzlknight   (501) staff       (20)       63 2023-01-28 22:40:46.000000 binance_candle-1.0.7/binance_candle/cmd/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.834092 binance_candle-1.0.7/binance_candle/code/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      580 2023-01-27 07:42:58.000000 binance_candle-1.0.7/binance_candle/code/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.836698 binance_candle-1.0.7/binance_candle/exception/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      193 2023-01-27 07:46:24.000000 binance_candle-1.0.7/binance_candle/exception/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      118 2023-01-27 07:43:48.000000 binance_candle-1.0.7/binance_candle/exception/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      164 2023-01-27 07:44:01.000000 binance_candle-1.0.7/binance_candle/exception/param.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      285 2023-01-27 07:44:20.000000 binance_candle-1.0.7/binance_candle/exception/req.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      164 2023-01-27 07:44:42.000000 binance_candle-1.0.7/binance_candle/exception/rule.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.839310 binance_candle-1.0.7/binance_candle/market/
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1081 2023-02-10 03:20:46.000000 binance_candle-1.0.7/binance_candle/market/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1580 2023-02-10 03:21:38.000000 binance_candle-1.0.7/binance_candle/market/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     6147 2023-03-08 05:12:53.000000 binance_candle-1.0.7/binance_candle/market/exchange_info.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    20111 2023-03-06 04:05:20.000000 binance_candle-1.0.7/binance_candle/market/history_candle.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     3685 2023-02-07 09:32:27.000000 binance_candle-1.0.7/binance_candle/market/ticker.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.840692 binance_candle-1.0.7/binance_candle/server/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      611 2023-02-10 03:22:48.000000 binance_candle-1.0.7/binance_candle/server/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1743 2023-03-03 03:27:57.000000 binance_candle-1.0.7/binance_candle/server/rule.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    28114 2023-04-27 05:29:25.000000 binance_candle-1.0.7/binance_candle/server/server.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2584 2023-01-30 03:08:21.000000 binance_candle-1.0.7/binance_candle/utils.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.832879 binance_candle-1.0.7/binance_candle.egg-info/
+-rw-r--r--   0 kzlknight   (501) staff       (20)    45879 2023-04-27 05:55:45.000000 binance_candle-1.0.7/binance_candle.egg-info/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1441 2023-04-27 05:55:45.000000 binance_candle-1.0.7/binance_candle.egg-info/SOURCES.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-04-27 05:55:45.000000 binance_candle-1.0.7/binance_candle.egg-info/dependency_links.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       47 2023-04-27 05:55:45.000000 binance_candle-1.0.7/binance_candle.egg-info/requires.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       15 2023-04-27 05:55:45.000000 binance_candle-1.0.7/binance_candle.egg-info/top_level.txt
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.851246 binance_candle-1.0.7/example/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      475 2023-02-07 09:21:09.000000 binance_candle-1.0.7/example/1. Market 交易规范.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      851 2023-02-07 09:41:04.000000 binance_candle-1.0.7/example/10. Server 维护实时历史K线数据.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      398 2023-02-07 09:22:11.000000 binance_candle-1.0.7/example/2. Market  产品列表.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      474 2023-02-07 09:24:03.000000 binance_candle-1.0.7/example/3. Market 最佳挂单.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      488 2023-02-07 09:28:13.000000 binance_candle-1.0.7/example/4. Market 最新价格.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      335 2023-02-07 09:35:26.000000 binance_candle-1.0.7/example/5. Market 产品深度.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1045 2023-02-07 09:36:59.000000 binance_candle-1.0.7/example/6. Market 历史K线.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      758 2023-02-07 09:37:55.000000 binance_candle-1.0.7/example/7. Utils candle与df的转化.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      427 2023-02-07 09:38:44.000000 binance_candle-1.0.7/example/8. Server 下载历史K线.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      429 2023-02-07 09:39:56.000000 binance_candle-1.0.7/example/9. Server 每日下载历史K线.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    45253 2023-03-06 04:08:20.000000 binance_candle-1.0.7/readme.md
+-rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-04-27 05:55:45.858011 binance_candle-1.0.7/setup.cfg
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2793 2023-04-27 05:40:36.000000 binance_candle-1.0.7/setup.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-04-27 05:55:45.856239 binance_candle-1.0.7/vx_images/
+-rw-r--r--   0 kzlknight   (501) staff       (20)   184133 2023-02-01 06:47:17.000000 binance_candle-1.0.7/vx_images/176016628950838.png
+-rw-r--r--   0 kzlknight   (501) staff       (20)    33022 2023-02-08 02:37:24.000000 binance_candle-1.0.7/vx_images/244075001625094.png
+-rw-r--r--   0 kzlknight   (501) staff       (20)   319035 2023-02-08 02:32:48.000000 binance_candle-1.0.7/vx_images/480313210278479.png
+-rw-r--r--   0 kzlknight   (501) staff       (20)   151185 2023-02-08 02:33:49.000000 binance_candle-1.0.7/vx_images/495193492836002.png
```

### Comparing `binance_candle-1.0.6/.idea/inspectionProfiles/Project_Default.xml` & `binance_candle-1.0.7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/PKG-INFO` & `binance_candle-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance_candle
-Version: 1.0.6
+Version: 1.0.7
 Summary: Binance local and real-time market candle server
 Home-page: https://github.com/pyted/binance_candle
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `binance_candle-1.0.6/binance_candle/code/__init__.py` & `binance_candle-1.0.7/binance_candle/code/__init__.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/market/__init__.py` & `binance_candle-1.0.7/binance_candle/market/__init__.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/market/_base.py` & `binance_candle-1.0.7/binance_candle/market/_base.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/market/exchange_info.py` & `binance_candle-1.0.7/binance_candle/market/exchange_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,7 +152,39 @@
         # [RETURN]
         result = {
             'code': 200,
             'data': symbols,
             'msg': ''
         }
         return result
+
+    # 获取全部的产品列表
+    # Weight: 现货10 合约1 使用缓存0
+    def get_symbols_all(
+            self,
+            expire_seconds: int = 60 * 5
+    ) -> dict:
+        '''
+        :param expire_seconds: 缓存时间（秒）
+        '''
+
+        exchangeInfos_result = self.get_exchangeInfos(expire_seconds)
+        # [ERROR RETURN] 异常交易规则与交易
+        if exchangeInfos_result['code'] != 200:
+            return exchangeInfos_result
+        # 不可交易的产品名称 status != 'TRADING'
+        if self.instType == 'CM':  # 币本位合约交易的状态名称特殊
+            status_name = 'contractStatus'
+        else:
+            status_name = 'status'
+
+        symbols = [
+            data['symbol']
+            for data in exchangeInfos_result['data']['symbols']
+        ]
+        # [RETURN]
+        result = {
+            'code': 200,
+            'data': symbols,
+            'msg': ''
+        }
+        return result
```

### Comparing `binance_candle-1.0.6/binance_candle/market/history_candle.py` & `binance_candle-1.0.7/binance_candle/market/history_candle.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/market/ticker.py` & `binance_candle-1.0.7/binance_candle/market/ticker.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/server/__init__.py` & `binance_candle-1.0.7/binance_candle/server/__init__.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/server/rule.py` & `binance_candle-1.0.7/binance_candle/server/rule.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle/server/server.py` & `binance_candle-1.0.7/binance_candle/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,34 +46,53 @@
         self.lite = self.binanceLite
         self._run_candle_map_thread = None
         self.__close_run_candle_map_signal = False
         self._download_daily_thread = None
         self.__close_download_daily_thread = False
 
     # 获取过滤后的产品名称
-    def get_symbols_filtered(self) -> dict:
+    def get_symbols_filtered(
+            self,
+            type='trading_on'  #
+    ) -> dict:
         '''
+        :param type:
+            trading_on:     正在交易的
+            trading_off:    不在交易的
+            trading_all:    全部
         过滤内容：
             1. rule.SYMBOLS_FILTER
             2. rule.SYMBOLS_CONTAINS
             3. rule.SYMBOL_ENDSWITH
             4. CandleServer.filter
         '''
         # 验证self.symbols
         if not (
                 self.rule.SYMBOLS == 'all' or
                 isinstance(self.rule.SYMBOLS, list)
         ):
             msg = 'rule.SYMBOLS must be "all" or list type'
             raise exception.RuleException(msg)
+        if type not in ['trading_on', 'trading_off', 'trading_all']:
+            msg = 'type must in ["trading_on","trading_off","trading_all"].'
+            raise exception.ParamException(msg)
         # 产品为全部 self.rule.SYMBOLS = 'all'
         if isinstance(self.rule.SYMBOLS, str) and self.rule.SYMBOLS.lower() == 'all':
-            symbols_trading_result = self.market.get_symbols_trading_on(
-                expire_seconds=60 * 60,  # 使用的缓存过期时间
-            )
+            if type == 'trading_on':
+                symbols_trading_result = self.market.get_symbols_trading_on(
+                    expire_seconds=60 * 60,  # 使用的缓存过期时间
+                )
+            elif type == 'trading_off':
+                symbols_trading_result = self.market.get_symbols_trading_off(
+                    expire_seconds=60 * 60,  # 使用的缓存过期时间
+                )
+            else:
+                symbols_trading_result = self.market.get_symbols_all(
+                    expire_seconds=60 * 60,  # 使用的缓存过期时间
+                )
             if symbols_trading_result['code'] != 200:
                 return symbols_trading_result
             symbols = symbols_trading_result['data']
         # 产品类型为列表
         else:
             symbols = self.rule.SYMBOLS
         # 第一次过滤 使用rule中的条件 -> symbols_filtered1
@@ -86,34 +105,43 @@
             if self.rule.SYMBOLS_FILTER and symbol in self.rule.SYMBOLS_FILTER:
                 continue
             if self.rule.SYMBOL_CONTAINS and not self.rule.SYMBOL_CONTAINS in symbol:
                 continue
             if self.rule.SYMBOL_ENDSWITH and not symbol.endswith(self.rule.SYMBOL_ENDSWITH):
                 continue
             symbols_filtered1.append(symbol)
-        # 第二次过滤 self.filter 过滤数据不足，请求错误的symbol -> symbols_filtered2
-        symbols_filtered2 = []
-        for symbol in symbols_filtered1:
-            symbol: str
-            if self.filter.check(symbol):  # True 不过滤
-                symbols_filtered2.append(symbol)
-        result = {'code': 200, 'data': symbols_filtered2, 'msg': ''}
+        # 仅当trading-on是否进行第二次过滤
+        if type == 'trading_on':
+            # 第二次过滤 self.filter 过滤数据不足，请求错误的symbol -> symbols_filtered2
+            symbols_filtered2 = []
+            for symbol in symbols_filtered1:
+                symbol: str
+                if self.filter.check(symbol):  # True 不过滤
+                    symbols_filtered2.append(symbol)
+            result = {'code': 200, 'data': symbols_filtered2, 'msg': ''}
+        else:
+            result = {'code': 200, 'data': symbols_filtered1, 'msg': ''}
         return result
 
     # 按照日期下载历史K线
     def download_candles_by_date(
             self,
             start: Union[str, int, float, datetime.date],
             end: Union[str, int, float, datetime.date, None] = None,
+            type: str = 'trading_on',
             replace=False,
     ):
         '''
         :param start: 起始日期
         :param end: 终止日期
             None 使用昨日日期
+        :param type: 产品交易类型
+            trading_on      正在交易的产品
+            trading_off     不可交易的产品
+            trading_all     全部产品
         :param replace: 是否替换本地文件
         '''
         # 执行下载使用的临时过滤器，过滤数据异常的产品
         self._download_filter = _filter.Filter()
         # 日期终点
         if not end:
             end = pendulum.yesterday(tz=self.rule.TIMEZONE)
@@ -121,47 +149,54 @@
         date_range = _date.get_range_dates(start=start, end=end, timezone=self.rule.TIMEZONE)
         # 反转日期序列，用于加速
         date_range = sorted(date_range, reverse=True)
         # 按照日期下载
         for date in date_range:
             self.__download_candles_by_date(
                 date=date,
+                type=type,
                 replace=replace,
             )
         # 删除临时过滤器
         del self._download_filter
 
     # 下载某一天多产品历史K线数据
     def __download_candles_by_date(
             self,
             date: Union[str, int, float, datetime.date],
+            type='trading_on',
             replace=False,
     ):
         '''
         :param date: 日期
+        :param type: 产品交易类型
+            trading_on      正在交易的产品
+            trading_off     不可交易的产品
+            trading_all     全部产品
         :param replace: 是否替换本地文件
         '''
         # 日期字符串，用于控制台打印
         if self.rule.TIMEZONE == 'America/New_York':
             date_str = _date.to_fmt(date, self.rule.TIMEZONE, '%d/%m/%Y')
         else:
             date_str = _date.to_fmt(date, self.rule.TIMEZONE, '%Y-%m-%d')
         # 获取产品列表
-        get_symbols_filtered_result = self.get_symbols_filtered()
+        get_symbols_filtered_result = self.get_symbols_filtered(type=type, )
         # **[ERROR RAISE]** 产品列表有误
         if get_symbols_filtered_result['code'] != 200:
             msg = '[get_symbols_filtered] code={code} msg={msg}'.format(
                 msg=get_symbols_filtered_result['msg'],
                 code=get_symbols_filtered_result['code'],
             )
             self.log.error(msg)
             raise exception.CodeException(msg)
         symbols = get_symbols_filtered_result['data']
-        # 过滤下载异常的产品
-        symbols = [symbol for symbol in symbols if self._download_filter.check(symbol)]
+        # 过滤下载异常的产品(仅当下载正在运行交易的产品，进行过滤）
+        if type == 'trading_on':
+            symbols = [symbol for symbol in symbols if self._download_filter.check(symbol)]
         # 产品逐个下载
         download_detail = {
             'all': len(symbols),  # 总数
             'skip': 0,  # 跳过的个数
             'suc': 0,  # 成功的个数
             'warn': 0,  # 警告的个数
             'error': 0,  # 失败的个数
@@ -524,54 +559,68 @@
             print(msg)
 
     # 每天定时下载以天为单位的历史数据
     @_thread.thread_wrapper
     def _download_daily(
             self,
             start: Union[str, int, float, datetime.date, None] = None,
-            replace: bool = False
+            replace: bool = False,
+            type='trading_on',
     ):
         # 下载补充数据
         yesterday = pendulum.yesterday(tz=self.rule.TIMEZONE)
         last_day = yesterday
         # 如果有start 下载start ~ yesterday的数据
         if start == None:
             start = yesterday
-        self.download_candles_by_date(start=start, end=yesterday, replace=replace)
+        # v1.0.7 防止下载start~yesterday的时间过长，中间的数据缺失
+        while True:
+            self.download_candles_by_date(start=start, end=yesterday, replace=replace, type=type)
+            if pendulum.yesterday(tz=self.rule.TIMEZONE) == yesterday:
+                break
+            else:
+                yesterday = pendulum.yesterday(tz=self.rule.TIMEZONE)
+
         while True:
             if self.__close_download_daily_thread == True:
                 break
             time.sleep(0.5)
             # 下载的时间条件
             if not pendulum.now(tz=self.rule.TIMEZONE).time().strftime('%H:%M:%S') >= self.rule.DOWNLOAD_TIME:
                 continue
             # 下载的日期条件
             yesterday = pendulum.yesterday(tz=self.rule.TIMEZONE)
             if (yesterday - last_day).days > 0:
                 self.download_candles_by_date(
                     start=yesterday,
                     end=yesterday,
+                    type=type,
                 )
                 last_day = yesterday
         self.__close_download_daily_thread = False
 
     def download_daily(self,
                        start: Union[str, int, float, datetime.date, None] = None,
-                       replace: bool = False
+                       replace: bool = False,
+                       type='trading_on',
                        ):
         '''
         :param start: 起始日期
             start != None 补充下载start ~ yesterday 的历史K线数据
         :param replace: 是否替换本地数据
+        :param type: 产品交易类型
+            trading_on      正在交易的产品
+            trading_off     不可交易的产品
+            trading_all     全部产品
         '''
         if self._download_daily_thread and self._download_daily_thread.isAlive():
             msg = 'Server download daily thread is running. Cannot run repeatedly.'
             print(msg)
             return None
-        t = self._download_daily(start=start, replace=replace)
+        t = self._download_daily(start=start, replace=replace, type=type)
         self._download_daily_thread = t
         time.sleep(1)
 
     # 获得candle的最新时间与当前时间查小于security_seconds的k线数据
     def get_candle_security(self, symbol: str, security_seconds=60 * 3) -> np.ndarray:
         '''
         :param symbol: 产品
```

### Comparing `binance_candle-1.0.6/binance_candle/utils.py` & `binance_candle-1.0.7/binance_candle/utils.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/binance_candle.egg-info/PKG-INFO` & `binance_candle-1.0.7/binance_candle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-candle
-Version: 1.0.6
+Version: 1.0.7
 Summary: Binance local and real-time market candle server
 Home-page: https://github.com/pyted/binance_candle
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `binance_candle-1.0.6/binance_candle.egg-info/SOURCES.txt` & `binance_candle-1.0.7/binance_candle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/example/10. Server 维护实时历史K线数据.py` & `binance_candle-1.0.7/example/10. Server 维护实时历史K线数据.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/example/6. Market 历史K线.py` & `binance_candle-1.0.7/example/6. Market 历史K线.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/example/7. Utils candle与df的转化.py` & `binance_candle-1.0.7/example/7. Utils candle与df的转化.py`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/readme.md` & `binance_candle-1.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/setup.py` & `binance_candle-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'binance_candle'
 DESCRIPTION = 'Binance local and real-time market candle server'
 URL = "https://github.com/pyted/binance_candle"
 EMAIL = 'pyted@outlook.com'
 AUTHOR = 'pyted'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 REQUIRED = [
     'pendulum',
     'numpy',
     'pandas',
     'candlelite',
     'paux',
```

### Comparing `binance_candle-1.0.6/vx_images/176016628950838.png` & `binance_candle-1.0.7/vx_images/176016628950838.png`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/vx_images/244075001625094.png` & `binance_candle-1.0.7/vx_images/244075001625094.png`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/vx_images/480313210278479.png` & `binance_candle-1.0.7/vx_images/480313210278479.png`

 * *Files identical despite different names*

### Comparing `binance_candle-1.0.6/vx_images/495193492836002.png` & `binance_candle-1.0.7/vx_images/495193492836002.png`

 * *Files identical despite different names*


# Comparing `tmp/ejtraderIQ-1.1.0.tar.gz` & `tmp/ejtraderIQ-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderIQ-1.1.0.tar", last modified: Sat Sep  3 16:43:00 2022, max compression
+gzip compressed data, was "ejtraderIQ-1.1.1.tar", last modified: Thu Apr 27 19:13:41 2023, max compression
```

## Comparing `ejtraderIQ-1.1.0.tar` & `ejtraderIQ-1.1.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.686680 ejtraderIQ-1.1.0/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      227 2022-09-03 16:43:00.686448 ejtraderIQ-1.1.0/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4025 2022-09-03 02:38:37.000000 ejtraderIQ-1.1.0/README.md
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.659031 ejtraderIQ-1.1.0/ejtraderIQ/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      460 2022-08-22 22:31:12.000000 ejtraderIQ-1.1.0/ejtraderIQ/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    28217 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/api.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     6108 2022-08-22 22:17:08.000000 ejtraderIQ-1.1.0/ejtraderIQ/constants.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     3145 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/country_id.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     8993 2022-09-03 16:41:25.000000 ejtraderIQ-1.1.0/ejtraderIQ/easyapi.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2600 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/expiration.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      401 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/global_value.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.666266 ejtraderIQ-1.1.0/ejtraderIQ/http/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       47 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      687 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/appinit.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      231 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/auth.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      233 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/billing.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      872 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/buyback.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      905 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/changebalance.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      950 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/events.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      654 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/getprofile.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      726 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/getregdata.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      973 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/login.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      320 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/loginv2.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      613 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/logout.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      233 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/profile.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      237 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/register.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      897 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/resource.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      760 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/http/token.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    56231 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/stable_api.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.667631 ejtraderIQ-1.1.0/ejtraderIQ/ws/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       42 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/__init__.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.679854 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       50 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      615 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/api_game_betinfo.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      833 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/api_game_getoptions.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      718 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/base.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2015 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buy_place_order_temp.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      361 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buyback.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2521 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buyv2.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     3139 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buyv3.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      379 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/cancel_order.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1222 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/candles.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      464 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/change_auto_margin_call.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      923 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/change_tpsl.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      683 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/changebalance.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      392 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/close_position.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      966 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/digital_option.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      467 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_available_leverages.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      350 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_balances.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      582 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_deferred_orders.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1294 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_financial_information.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      466 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_order.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      494 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_overnight_fee.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2221 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_positions.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      441 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/heartbeat.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      425 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/instruments.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1312 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/leaderboard.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      612 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/sell_option.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      515 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/setactives.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      442 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/ssid.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1033 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/strike_list.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4659 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/subscribe.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1186 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/traders_mood.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4194 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/unsubscribe.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1503 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/user.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    15300 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/client.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.682350 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       50 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      395 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/base.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      696 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/betinfo.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2814 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/candles.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      662 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/listinfodata.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2287 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/profile.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1822 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/timesync.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.660568 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      227 2022-09-03 16:43:00.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2488 2022-09-03 16:43:00.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/SOURCES.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2022-09-03 16:43:00.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/dependency_links.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2022-09-02 09:16:19.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/not-zip-safe
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       39 2022-09-03 16:43:00.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/requires.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       17 2022-09-03 16:43:00.000000 ejtraderIQ-1.1.0/ejtraderIQ.egg-info/top_level.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       38 2022-09-03 16:43:00.686760 ejtraderIQ-1.1.0/setup.cfg
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      528 2022-09-03 16:42:41.000000 ejtraderIQ-1.1.0/setup.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2022-09-03 16:43:00.686082 ejtraderIQ-1.1.0/tests/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/tests/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      170 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/tests/iq.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1410 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/tests/test_Binary_Option.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      923 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/tests/test_Candle.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      370 2022-08-22 22:04:31.000000 ejtraderIQ-1.1.0/tests/test_Login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.391200 ejtraderIQ-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 19:13:41.387200 ejtraderIQ-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.379200 ejtraderIQ-1.1.1/ejtraderIQ/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28217 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/country_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/easyapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/global_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.383200 ejtraderIQ-1.1.1/ejtraderIQ/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/appinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/buyback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/changebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/getprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/getregdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/loginv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/http/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56231 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/stable_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.383200 ejtraderIQ-1.1.1/ejtraderIQ/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.387200 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/api_game_betinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/api_game_getoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buy_place_order_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buyback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buyv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buyv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/candles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/change_auto_margin_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/change_tpsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/changebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/close_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/digital_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_available_leverages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_deferred_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_financial_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_overnight_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/sell_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/setactives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/ssid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/strike_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/traders_mood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/unsubscribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.387200 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/betinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/candles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/listinfodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/timesync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.383200 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 19:13:41.000000 ejtraderIQ-1.1.1/ejtraderIQ.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:13:41.391200 ejtraderIQ-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:41.387200 ejtraderIQ-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/tests/iq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/tests/test_Binary_Option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/tests/test_Candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 19:13:27.000000 ejtraderIQ-1.1.1/tests/test_Login.py
```

### Comparing `ejtraderIQ-1.1.0/README.md` & `ejtraderIQ-1.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderIQ/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderIQ)
+
 # IQoption API
 
 ### ToDo
 
 - [x] Account Balance 
 - [x] trade buy and sell "Digital & Turbo"
 - [x] Check Win
@@ -166,23 +169,35 @@
 
 ```
 
 ##### Check Win
 ```python
 api.checkwin(id)
 
-# example check win
+# example check win Digital 
 id = api.buy(volume,symbol,timeframe)
 win = api.checkwin(id)
 
 if win > 0:
     print(("WIN"+'\n'))
 elif win < 0:                                            
     print(("LOSS"+'\n'))
 else:
+    print(('Tied '+'\n'))
+    
+    
+# example check win Turbo
+id = api.buy(volume,symbol,timeframe,turbo=True)
+win = api.checkwin(id,turbo=True)
+
+if win > 0:
+    print(("WIN"+'\n'))
+elif win < 0:                                            
+    print(("LOSS"+'\n'))
+else:
     print(('Tied '+'\n'))    
 ```
 
 ##### Check markets state
 ```python
 markets = api.isOpen()
 print(markets)
```

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/api.py` & `ejtraderIQ-1.1.1/ejtraderIQ/api.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/constants.py` & `ejtraderIQ-1.1.1/ejtraderIQ/constants.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/country_id.py` & `ejtraderIQ-1.1.1/ejtraderIQ/country_id.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/easyapi.py` & `ejtraderIQ-1.1.1/ejtraderIQ/easyapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         candles = candles + 1
         timestamp = self.iq.get_server_timestamp()
         timeframe = self.timeframe_to_seconds(timeframe)
         
 
        
         x = self.iq.get_candles(symbol, int(timeframe), candles, timestamp)
-        timestamp = int(x[0]["from"]) -1
+        
         
 
         dataframe = pd.DataFrame(x)
         dataframe.sort_values(by=["from"], inplace=True, ascending=True)
         dataframe.drop(dataframe.tail(1).index, inplace=True)
         dataframe = dataframe.rename(columns = {'from': 'date', 'min': 'low','max':'high'})
         dataframe = dataframe.set_index(['date'])
```

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/expiration.py` & `ejtraderIQ-1.1.1/ejtraderIQ/expiration.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/appinit.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/appinit.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/buyback.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/buyback.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/changebalance.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/changebalance.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/events.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/events.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/getprofile.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/getprofile.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/getregdata.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/getregdata.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/login.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/login.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/logout.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/logout.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/resource.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/resource.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/http/token.py` & `ejtraderIQ-1.1.1/ejtraderIQ/http/token.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/stable_api.py` & `ejtraderIQ-1.1.1/ejtraderIQ/stable_api.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/api_game_betinfo.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/api_game_betinfo.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/api_game_getoptions.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/api_game_getoptions.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/base.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/base.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buy_place_order_temp.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buy_place_order_temp.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buyv2.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buyv2.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/buyv3.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/buyv3.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/candles.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/candles.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/change_tpsl.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/change_tpsl.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/changebalance.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/changebalance.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/digital_option.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/digital_option.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_deferred_orders.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_deferred_orders.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_financial_information.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_financial_information.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/get_positions.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/get_positions.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/leaderboard.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/leaderboard.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/sell_option.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/sell_option.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/setactives.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/setactives.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/strike_list.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/strike_list.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/subscribe.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/subscribe.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/traders_mood.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/traders_mood.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/unsubscribe.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/chanels/user.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/chanels/user.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/client.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/client.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/betinfo.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/betinfo.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/candles.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/candles.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/listinfodata.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/listinfodata.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/profile.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/profile.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ/ws/objects/timesync.py` & `ejtraderIQ-1.1.1/ejtraderIQ/ws/objects/timesync.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/ejtraderIQ.egg-info/SOURCES.txt` & `ejtraderIQ-1.1.1/ejtraderIQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/setup.py` & `ejtraderIQ-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The python wrapper for IQ Option API package setup."""
 from setuptools import (setup, find_packages)
 
 
 setup(
     name="ejtraderIQ",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     install_requires=["pylint","requests","websocket-client==0.56"],
     include_package_data = True,
     description="IQ Option API for python",
     long_description="IQ Option API for python",
     url="https://github.com/ejtraderLabs/ejtraderIQ",
     author="Emerson Pedroso",
```

### Comparing `ejtraderIQ-1.1.0/tests/test_Binary_Option.py` & `ejtraderIQ-1.1.1/tests/test_Binary_Option.py`

 * *Files identical despite different names*

### Comparing `ejtraderIQ-1.1.0/tests/test_Candle.py` & `ejtraderIQ-1.1.1/tests/test_Candle.py`

 * *Files identical despite different names*


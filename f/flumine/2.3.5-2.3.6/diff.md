# Comparing `tmp/flumine-2.3.5.tar.gz` & `tmp/flumine-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flumine-2.3.5.tar", last modified: Thu Mar 16 09:10:16 2023, max compression
+gzip compressed data, was "dist/flumine-2.3.6.tar", last modified: Thu Apr 27 08:39:23 2023, max compression
```

## Comparing `flumine-2.3.5.tar` & `flumine-2.3.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-16 09:10:16.000000 flumine-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-03-16 09:09:40.000000 flumine-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/baseflumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/betconnectclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/betfairclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/clients/simulatedclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/controls/clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/controls/loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/controls/tradingcontrols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/execution/baseexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/execution/betfairexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/execution/simulatedexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/execution/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/flumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/markets/blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/markets/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/markets/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/order/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/simulation/simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/strategy/runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/strategy/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/basestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/historicalstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/marketstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/orderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/simulatedorderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/sportsdatastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-03-16 09:09:40.000000 flumine-2.3.5/flumine/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-16 09:10:15.000000 flumine-2.3.5/flumine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-16 09:10:16.000000 flumine-2.3.5/flumine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:10:15.000000 flumine-2.3.5/flumine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-16 09:10:15.000000 flumine-2.3.5/flumine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-16 09:10:15.000000 flumine-2.3.5/flumine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 09:10:16.000000 flumine-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-16 09:09:40.000000 flumine-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:10:16.000000 flumine-2.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_baseflumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_flumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_fluminesimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21058 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_simulated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57435 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_tradingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-03-16 09:09:40.000000 flumine-2.3.5/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-27 08:39:23.000000 flumine-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-27 08:39:01.000000 flumine-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/baseflumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/betconnectclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/betfairclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/simulatedclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/tradingcontrols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/baseexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/betfairexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/simulatedexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/flumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/basestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/historicalstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/marketstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/orderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/sportsdatastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:39:23.000000 flumine-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-27 08:39:01.000000 flumine-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_baseflumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_flumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_fluminesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_simulated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60568 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_tradingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_worker.py
```

### Comparing `flumine-2.3.5/PKG-INFO` & `flumine-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.5
+Version: 2.3.6
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.3.5 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.3.6 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.5/README.md` & `flumine-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/__init__.py` & `flumine-2.3.6/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/baseflumine.py` & `flumine-2.3.6/flumine/baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/clients/baseclient.py` & `flumine-2.3.6/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/clients/betconnectclient.py` & `flumine-2.3.6/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/clients/betfairclient.py` & `flumine-2.3.6/flumine/clients/betfairclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/clients/clients.py` & `flumine-2.3.6/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/clients/simulatedclient.py` & `flumine-2.3.6/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/config.py` & `flumine-2.3.6/flumine/config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/controls/__init__.py` & `flumine-2.3.6/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/controls/clientcontrols.py` & `flumine-2.3.6/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/controls/loggingcontrols.py` & `flumine-2.3.6/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/controls/tradingcontrols.py` & `flumine-2.3.6/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/events/events.py` & `flumine-2.3.6/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/exceptions.py` & `flumine-2.3.6/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/execution/baseexecution.py` & `flumine-2.3.6/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/execution/betfairexecution.py` & `flumine-2.3.6/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/execution/simulatedexecution.py` & `flumine-2.3.6/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/execution/transaction.py` & `flumine-2.3.6/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/flumine.py` & `flumine-2.3.6/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/markets/blotter.py` & `flumine-2.3.6/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/markets/market.py` & `flumine-2.3.6/flumine/markets/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,20 @@
     ) -> bool:
         with self.transaction(client=order.client) as t:
             return t.replace_order(order, new_price, market_version, force)
 
     @property
     def event(self) -> dict:
         event = defaultdict(list)
-        for market in self.flumine.markets:
+        market_start_datetime = self.market_start_datetime
+        event_type_id = self.event_type_id
+        for market in self.flumine.markets.events[self.event_id]:
             if (
-                self.event_id == market.event_id
-                and self.market_start_datetime == market.market_start_datetime
+                market_start_datetime == market.market_start_datetime
+                or event_type_id == "1"
             ):
                 event[market.market_type].append(market)
         return event
 
     @property
     def event_type_id(self) -> str:
         if self.market_catalogue:
```

### Comparing `flumine-2.3.5/flumine/markets/markets.py` & `flumine-2.3.6/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/markets/middleware.py` & `flumine-2.3.6/flumine/markets/middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/order.py` & `flumine-2.3.6/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/orderpackage.py` & `flumine-2.3.6/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/ordertype.py` & `flumine-2.3.6/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/process.py` & `flumine-2.3.6/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/responses.py` & `flumine-2.3.6/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/order/trade.py` & `flumine-2.3.6/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/patching.py` & `flumine-2.3.6/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/simulation/simulatedorder.py` & `flumine-2.3.6/flumine/simulation/simulatedorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,32 +117,32 @@
                     )
                 elif time_in_force == "FILL_OR_KILL":
                     available_size = get_size(runner.ex.available_to_back, 0) or 0
                     if price > available_to_back:
                         self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                     elif price == available_to_back:
-                        if available_size < min_fill_size:
-                            self.size_lapsed += self.size_remaining
-                            return self._create_place_response(bet_id)
-                        self._process_price_matched(
-                            market_book.publish_time_epoch,
-                            price,
-                            size,
-                            runner.ex.available_to_back,
-                        )
+                        if available_size >= min_fill_size:
+                            self._process_price_matched(
+                                market_book.publish_time_epoch,
+                                price,
+                                size,
+                                runner.ex.available_to_back,
+                            )
+                        self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                     else:
                         self._process_price_matched_vwap(
                             market_book.publish_time_epoch,
                             price,
                             size,
                             runner.ex.available_to_back,
                             min_fill_size=min_fill_size,
                         )
+                        self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                 elif available_to_back >= price:
                     self._process_price_matched(
                         market_book.publish_time_epoch,
                         price,
                         size,
                         runner.ex.available_to_back,
@@ -163,32 +163,32 @@
                     )
                 elif time_in_force == "FILL_OR_KILL":
                     available_size = get_size(runner.ex.available_to_lay, 0) or 0
                     if price < available_to_lay:
                         self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                     elif price == available_to_lay:
-                        if available_size < min_fill_size:
-                            self.size_lapsed += self.size_remaining
-                            return self._create_place_response(bet_id)
-                        self._process_price_matched(
-                            market_book.publish_time_epoch,
-                            price,
-                            size,
-                            runner.ex.available_to_lay,
-                        )
+                        if available_size >= min_fill_size:
+                            self._process_price_matched(
+                                market_book.publish_time_epoch,
+                                price,
+                                size,
+                                runner.ex.available_to_lay,
+                            )
+                        self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                     else:
                         self._process_price_matched_vwap(
                             market_book.publish_time_epoch,
                             price,
                             size,
                             runner.ex.available_to_lay,
                             min_fill_size=min_fill_size,
                         )
+                        self.size_lapsed += self.size_remaining
                         return self._create_place_response(bet_id)
                 elif available_to_lay <= price:
                     self._process_price_matched(
                         market_book.publish_time_epoch,
                         price,
                         size,
                         runner.ex.available_to_lay,
```

### Comparing `flumine-2.3.5/flumine/simulation/simulation.py` & `flumine-2.3.6/flumine/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/simulation/utils.py` & `flumine-2.3.6/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/strategy/runnercontext.py` & `flumine-2.3.6/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/strategy/strategy.py` & `flumine-2.3.6/flumine/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/basestream.py` & `flumine-2.3.6/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/datastream.py` & `flumine-2.3.6/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/historicalstream.py` & `flumine-2.3.6/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/marketstream.py` & `flumine-2.3.6/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/orderstream.py` & `flumine-2.3.6/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/simulatedorderstream.py` & `flumine-2.3.6/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/sportsdatastream.py` & `flumine-2.3.6/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/streams/streams.py` & `flumine-2.3.6/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/utils.py` & `flumine-2.3.6/flumine/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine/worker.py` & `flumine-2.3.6/flumine/worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/flumine.egg-info/PKG-INFO` & `flumine-2.3.6/flumine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.5
+Version: 2.3.6
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.3.5 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.3.6 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.5/flumine.egg-info/SOURCES.txt` & `flumine-2.3.6/flumine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/setup.py` & `flumine-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_baseflumine.py` & `flumine-2.3.6/tests/test_baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_blotter.py` & `flumine-2.3.6/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_clientcontrols.py` & `flumine-2.3.6/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_clients.py` & `flumine-2.3.6/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_config.py` & `flumine-2.3.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_events.py` & `flumine-2.3.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_execution.py` & `flumine-2.3.6/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_flumine.py` & `flumine-2.3.6/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_fluminesimulation.py` & `flumine-2.3.6/tests/test_fluminesimulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_integration.py` & `flumine-2.3.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_loggingcontrols.py` & `flumine-2.3.6/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_markets.py` & `flumine-2.3.6/tests/test_markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 import datetime
 from unittest import mock
+from collections import defaultdict
 
 from flumine.markets.markets import Markets
 from flumine.markets.market import Market
 from flumine import config
 
 
 class MarketsTest(unittest.TestCase):
@@ -217,24 +218,27 @@
         self.assertTrue(self.market.replace_order(mock_order, 2, False, force=True))
         mock_transaction.assert_called_with(client=mock_order.client)
         mock_transaction.replace_order.assert_called_with(mock_order, 2, False, True)
 
     def test_event(self):
         self.market.market_catalogue.event.id = 12
         self.market.market_book.market_definition.market_time = 12
-
-        self.market.flumine.markets = []
+        self.market.flumine.markets.events = defaultdict(list)
         self.assertEqual(self.market.event, {})
 
         m_one = mock.Mock(market_type=1, event_id=12, market_start_datetime=12)
         m_two = mock.Mock(market_type=2, event_id=12, market_start_datetime=12)
         m_three = mock.Mock(market_type=3, event_id=123, market_start_datetime=12)
         m_four = mock.Mock(market_type=1, event_id=12, market_start_datetime=12)
         m_five = mock.Mock(market_type=2, event_id=12, market_start_datetime=13)
-        self.market.flumine.markets = [m_one, m_two, m_three, m_four, m_five]
+        self.market.flumine.markets.events[m_one.event_id].append(m_one)
+        self.market.flumine.markets.events[m_two.event_id].append(m_two)
+        self.market.flumine.markets.events[m_three.event_id].append(m_three)
+        self.market.flumine.markets.events[m_four.event_id].append(m_four)
+        self.market.flumine.markets.events[m_five.event_id].append(m_five)
         self.assertEqual(self.market.event, {1: [m_one, m_four], 2: [m_two]})
 
     def test_event_type_id_mc(self):
         mock_market_catalogue = mock.Mock()
         self.market.market_catalogue = mock_market_catalogue
         self.assertEqual(self.market.event_type_id, mock_market_catalogue.event_type.id)
```

### Comparing `flumine-2.3.5/tests/test_middleware.py` & `flumine-2.3.6/tests/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from pathlib import Path
 from unittest import mock
 
 from flumine.markets.middleware import (
     Middleware,
     SimulatedMiddleware,
     RunnerAnalytics,
     OrderStatus,
@@ -473,15 +474,15 @@
     @mock.patch(
         "flumine.markets.middleware.SimulatedSportsDataMiddleware._create_generator"
     )
     def test_add_market(self, mock__create_generator):
         mock_market = mock.Mock(market_id="marketId")
         self.assertIsNone(self.middleware.add_market(mock_market))
         mock__create_generator.assert_called_with(
-            "test/marketId", "cricketSubscription", 123
+            str(Path("test/marketId")), "cricketSubscription", 123
         )
         self.assertEqual(self.middleware._gen, mock__create_generator()())
         self.assertEqual(self.middleware._next, next(mock__create_generator()()))
 
     def test_remove_market(self):
         self.middleware.remove_market(mock.Mock())
         self.assertIsNone(self.middleware._gen)
```

### Comparing `flumine-2.3.5/tests/test_order.py` & `flumine-2.3.6/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_orderpackage.py` & `flumine-2.3.6/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_ordertype.py` & `flumine-2.3.6/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_process.py` & `flumine-2.3.6/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_responses.py` & `flumine-2.3.6/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_runnercontext.py` & `flumine-2.3.6/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_simulated_utils.py` & `flumine-2.3.6/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_simulatedorder.py` & `flumine-2.3.6/tests/test_simulatedorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unittest
 from unittest import mock
 
 from flumine.simulation import simulatedorder
 from flumine.order.ordertype import OrderTypes
 
+EXECUTION_COMPLETE = "EXECUTION_COMPLETE"
+
 
 class SimulatedOrderTest(unittest.TestCase):
     def setUp(self) -> None:
         self.mock_order_type = mock.Mock(
             price=12, size=2.00, ORDER_TYPE=OrderTypes.LIMIT
         )
         mock_client = mock.Mock(
@@ -176,17 +178,19 @@
         )
         self.assertEqual(self.simulated.market_version, mock_market_book.version)
         self.assertEqual(resp.average_price_matched, 12)
         self.assertEqual(resp.size_matched, 1)
         self.assertEqual(
             self.simulated.matched, [[mock_market_book.publish_time_epoch, 12, 1]]
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
-    def test_place_limit_back_fill_or_kill_cancelled(self, mock__get_runner):
+    def test_place_limit_back_fill_or_kill_lapsed(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         mock_market_book = mock.Mock(status="OPEN")
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 11, "size": 1}]
         mock_runner.ex.available_to_lay = [{"price": 13, "size": 120}]
         mock__get_runner.return_value = mock_runner
@@ -194,14 +198,39 @@
         resp = self.simulated.place(
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(self.simulated.market_version, mock_market_book.version)
         self.assertEqual(resp.average_price_matched, 0)
         self.assertEqual(resp.size_matched, 0)
         self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
+
+    @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
+    def test_place_limit_back_fill_or_kill_no_price(self, mock__get_runner):
+        self.mock_order.order_type.price = 1.01
+        mock_client = mock.Mock(best_price_execution=True)
+        mock_order_package = mock.Mock(client=mock_client, market_version=None)
+        mock_market_book = mock.Mock(status="OPEN")
+        mock_runner = mock.Mock()
+        mock_runner.ex.available_to_back = []
+        mock_runner.ex.available_to_lay = []
+        mock__get_runner.return_value = mock_runner
+        instruction = {"limitOrder": {"timeInForce": "FILL_OR_KILL"}}
+        resp = self.simulated.place(
+            mock_order_package, mock_market_book, instruction, 1
+        )
+        self.assertEqual(self.simulated.market_version, mock_market_book.version)
+        self.assertEqual(resp.average_price_matched, 0)
+        self.assertEqual(resp.size_matched, 0)
+        self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_limit_back_fill_or_kill_min_fill_size_matched(
         self, mock__get_runner
     ):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
@@ -216,19 +245,20 @@
         )
         self.assertEqual(self.simulated.market_version, mock_market_book.version)
         self.assertEqual(resp.average_price_matched, 12)
         self.assertEqual(resp.size_matched, 1)
         self.assertEqual(
             self.simulated.matched, [[mock_market_book.publish_time_epoch, 12, 1]]
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
-    def test_place_limit_back_fill_or_kill_min_fill_size_cancelled(
-        self, mock__get_runner
-    ):
+    def test_place_limit_back_fill_or_kill_min_fill_size_lapsed(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         mock_market_book = mock.Mock(status="OPEN")
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 12, "size": 1}]
         mock_runner.ex.available_to_lay = [{"price": 13, "size": 120}]
         mock__get_runner.return_value = mock_runner
@@ -238,21 +268,24 @@
         resp = self.simulated.place(
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(self.simulated.market_version, mock_market_book.version)
         self.assertEqual(resp.average_price_matched, 0)
         self.assertEqual(resp.size_matched, 0)
         self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_limit_back_fill_or_kill_vwap(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         mock_market_book = mock.Mock(status="OPEN")
-        self.mock_order.order_type.size = 3
+        self.mock_order.order_type.size = 4
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [
             {"price": 13, "size": 1},
             {"price": 12, "size": 1},
             {"price": 11, "size": 1},
         ]
         mock_runner.ex.available_to_lay = [{"price": 13, "size": 120}]
@@ -268,14 +301,17 @@
             self.simulated.matched,
             [
                 [mock_market_book.publish_time_epoch, 13, 1],
                 [mock_market_book.publish_time_epoch, 12, 1],
                 [mock_market_book.publish_time_epoch, 11, 1],
             ],
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_market_status(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=False)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         mock_market_book = mock.Mock(status="SUSPENDED")
         resp = self.simulated.place(mock_order_package, mock_market_book, {}, 1)
@@ -364,17 +400,20 @@
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(resp.average_price_matched, 12)
         self.assertEqual(resp.size_matched, 1)
         self.assertEqual(
             self.simulated.matched, [[mock_market_book.publish_time_epoch, 12, 1]]
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
-    def test_place_limit_lay_fill_or_kill_cancelled(self, mock__get_runner):
+    def test_place_limit_lay_fill_or_kill_lapsed(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
         mock_market_book = mock.Mock(status="OPEN")
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 11, "size": 120}]
         mock_runner.ex.available_to_lay = [{"price": 13, "size": 1}]
@@ -382,14 +421,17 @@
         instruction = {"limitOrder": {"timeInForce": "FILL_OR_KILL"}}
         resp = self.simulated.place(
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(resp.average_price_matched, 0)
         self.assertEqual(resp.size_matched, 0)
         self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_limit_lay_fill_or_kill_no_price(self, mock__get_runner):
         self.mock_order.order_type.price = 1000
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
@@ -401,17 +443,20 @@
         instruction = {"limitOrder": {"timeInForce": "FILL_OR_KILL"}}
         resp = self.simulated.place(
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(resp.average_price_matched, 0)
         self.assertEqual(resp.size_matched, 0)
         self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
-    def test_place_limit_lay_fill_or_kill_min_fill_size(self, mock__get_runner):
+    def test_place_limit_lay_fill_or_kill_min_fill_size_matched(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
         mock_market_book = mock.Mock(status="OPEN")
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 11, "size": 120}]
         mock_runner.ex.available_to_lay = [{"price": 12, "size": 1}]
@@ -421,19 +466,20 @@
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(resp.average_price_matched, 12)
         self.assertEqual(resp.size_matched, 1)
         self.assertEqual(
             self.simulated.matched, [[mock_market_book.publish_time_epoch, 12, 1]]
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
-    def test_place_limit_lay_fill_or_kill_min_fill_size_cancelled(
-        self, mock__get_runner
-    ):
+    def test_place_limit_lay_fill_or_kill_min_fill_size_lapsed(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
         mock_market_book = mock.Mock(status="OPEN")
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 11, "size": 120}]
         mock_runner.ex.available_to_lay = [{"price": 12, "size": 1}]
@@ -443,22 +489,25 @@
         }
         resp = self.simulated.place(
             mock_order_package, mock_market_book, instruction, 1
         )
         self.assertEqual(resp.average_price_matched, 0)
         self.assertEqual(resp.size_matched, 0)
         self.assertEqual(self.simulated.matched, [])
+        self.assertEqual(self.simulated.size_lapsed, 2)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_limit_lay_fill_or_kill_vwap(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
         mock_market_book = mock.Mock(status="OPEN")
-        self.mock_order.order_type.size = 3
+        self.mock_order.order_type.size = 4
         mock_runner = mock.Mock()
         mock_runner.ex.available_to_back = [{"price": 11, "size": 120}]
         mock_runner.ex.available_to_lay = [
             {"price": 11, "size": 1},
             {"price": 12, "size": 1},
             {"price": 13, "size": 1},
         ]
@@ -473,14 +522,17 @@
             self.simulated.matched,
             [
                 [mock_market_book.publish_time_epoch, 11, 1],
                 [mock_market_book.publish_time_epoch, 12, 1],
                 [mock_market_book.publish_time_epoch, 13, 1],
             ],
         )
+        self.assertEqual(self.simulated.size_lapsed, 1)
+        self.assertEqual(self.simulated.size_remaining, 0)
+        self.assertEqual(self.simulated.status, EXECUTION_COMPLETE)
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     def test_place_limit_lay_unmatched(self, mock__get_runner):
         mock_client = mock.Mock(best_price_execution=True)
         mock_order_package = mock.Mock(client=mock_client, market_version=None)
         self.simulated.order.side = "LAY"
         mock_market_book = mock.Mock(status="OPEN")
```

### Comparing `flumine-2.3.5/tests/test_strategy.py` & `flumine-2.3.6/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_streams.py` & `flumine-2.3.6/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_trade.py` & `flumine-2.3.6/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_tradingcontrols.py` & `flumine-2.3.6/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_transaction.py` & `flumine-2.3.6/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_utils.py` & `flumine-2.3.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.5/tests/test_worker.py` & `flumine-2.3.6/tests/test_worker.py`

 * *Files identical despite different names*


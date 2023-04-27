# Comparing `tmp/robotmk-0.0.60.tar.gz` & `tmp/robotmk-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.60.tar", last modified: Wed Apr 26 21:03:02 2023, max compression
+gzip compressed data, was "robotmk-0.0.61.tar", last modified: Wed Apr 26 21:44:50 2023, max compression
```

## Comparing `robotmk-0.0.60.tar` & `robotmk-0.0.61.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      110 2023-04-26 21:02:30.989966 robotmk-0.0.60/.bumpversion.cfg
--rw-r--r--   0        0        0      279 2023-04-26 20:43:31.679551 robotmk-0.0.60/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.60/README.md
--rw-r--r--   0        0        0      755 2023-04-26 20:37:47.847759 robotmk-0.0.60/pyproject.toml
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.60/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.60/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-26 21:02:30.989966 robotmk-0.0.60/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-26 09:17:32.607360 robotmk-0.0.60/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.60/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.60/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    18059 2023-04-26 20:43:34.683477 robotmk-0.0.60/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.60/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.60/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.60/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.60/src/robotmk/context/agent/__init__.py
--rw-r--r--   0        0        0     2086 2023-04-26 12:58:54.634165 robotmk-0.0.60/src/robotmk/context/agent/agent.py
--rw-r--r--   0        0        0     1579 2023-04-26 20:43:34.683477 robotmk-0.0.60/src/robotmk/context/agent/cli.py
--rw-r--r--   0        0        0      681 2023-04-26 12:37:20.188228 robotmk-0.0.60/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.60/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.60/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.60/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.60/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-26 12:27:48.266927 robotmk-0.0.60/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.60/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.60/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3995 2023-04-26 20:37:47.847759 robotmk-0.0.60/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.60/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     7380 2023-04-26 20:37:47.847759 robotmk-0.0.60/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     2849 2023-04-26 19:52:00.628070 robotmk-0.0.60/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      135 2023-04-26 13:29:57.729591 robotmk-0.0.60/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-26 17:05:40.456944 robotmk-0.0.60/src/robotmk/context/suite/target/abstract.py
--rw-r--r--   0        0        0     1604 2023-04-26 13:40:32.915503 robotmk-0.0.60/src/robotmk/context/suite/target/factory.py
--rw-r--r--   0        0        0     2686 2023-04-26 16:31:12.211225 robotmk-0.0.60/src/robotmk/context/suite/target/local.py
--rw-r--r--   0        0        0     5628 2023-04-26 20:37:47.847759 robotmk-0.0.60/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0     2245 2023-04-26 20:43:34.683477 robotmk-0.0.60/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6339 2023-04-26 13:35:01.378678 robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4877 2023-04-26 18:10:20.939058 robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     3878 2023-04-26 13:32:58.143863 robotmk-0.0.60/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0     3932 2023-04-26 18:38:03.011146 robotmk-0.0.60/src/robotmk/emitter.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.60/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.60/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.60/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.60/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.60/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.60/src/robotmk/logger.py
--rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.60/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.60/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.60/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.60/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.60/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.60/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.60/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.60/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.60/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.60/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.60/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.60/tests/context/test_cli.py
--rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.60/tests/test_robotmk.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.60/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.60/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-26 21:44:38.777869 robotmk-0.0.61/.bumpversion.cfg
+-rw-r--r--   0        0        0      279 2023-04-26 20:43:31.679551 robotmk-0.0.61/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.61/README.md
+-rw-r--r--   0        0        0      755 2023-04-26 20:37:47.847759 robotmk-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.61/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.61/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-26 21:44:38.777869 robotmk-0.0.61/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-26 09:17:32.607360 robotmk-0.0.61/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.61/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.61/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    18059 2023-04-26 20:43:34.683477 robotmk-0.0.61/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.61/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.61/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.61/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.61/src/robotmk/context/agent/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-26 12:58:54.634165 robotmk-0.0.61/src/robotmk/context/agent/agent.py
+-rw-r--r--   0        0        0     1579 2023-04-26 20:43:34.683477 robotmk-0.0.61/src/robotmk/context/agent/cli.py
+-rw-r--r--   0        0        0      681 2023-04-26 12:37:20.188228 robotmk-0.0.61/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.61/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.61/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.61/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.61/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-26 12:27:48.266927 robotmk-0.0.61/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.61/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.61/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-26 20:37:47.847759 robotmk-0.0.61/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.61/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     7380 2023-04-26 20:37:47.847759 robotmk-0.0.61/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     2746 2023-04-26 21:37:26.834077 robotmk-0.0.61/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      180 2023-04-26 21:36:37.534644 robotmk-0.0.61/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     1432 2023-04-26 17:05:40.456944 robotmk-0.0.61/src/robotmk/context/suite/target/abstract.py
+-rw-r--r--   0        0        0     1604 2023-04-26 13:40:32.915503 robotmk-0.0.61/src/robotmk/context/suite/target/factory.py
+-rw-r--r--   0        0        0     2686 2023-04-26 16:31:12.211225 robotmk-0.0.61/src/robotmk/context/suite/target/local.py
+-rw-r--r--   0        0        0     5628 2023-04-26 20:37:47.847759 robotmk-0.0.61/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0     2248 2023-04-26 21:40:21.648234 robotmk-0.0.61/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6339 2023-04-26 13:35:01.378678 robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4877 2023-04-26 18:10:20.939058 robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     3878 2023-04-26 13:32:58.143863 robotmk-0.0.61/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0     3932 2023-04-26 18:38:03.011146 robotmk-0.0.61/src/robotmk/emitter.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.61/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.61/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.61/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.61/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.61/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.61/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.61/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.61/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.61/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.61/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.61/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.61/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.61/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.61/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.61/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.61/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.61/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.61/tests/context/test_cli.py
+-rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.61/tests/test_robotmk.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.61/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.61/PKG-INFO
```

### Comparing `robotmk-0.0.60/pyproject.toml` & `robotmk-0.0.61/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/categories.json` & `robotmk-0.0.61/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/click_tutorial.py` & `robotmk-0.0.61/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/cli/cli.py` & `robotmk-0.0.61/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.61/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/config/config.py` & `robotmk-0.0.61/src/robotmk/config/config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/config/yml.py` & `robotmk-0.0.61/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/abstract.py` & `robotmk-0.0.61/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/agent/agent.py` & `robotmk-0.0.61/src/robotmk/context/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/agent/cli.py` & `robotmk-0.0.61/src/robotmk/context/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/context.py` & `robotmk-0.0.61/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.61/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.61/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/cli.py` & `robotmk-0.0.61/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.61/src/robotmk/context/suite/strategies/run.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/suite.py` & `robotmk-0.0.61/src/robotmk/context/suite/suite.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 execution, either against a local target (RCC/RF) or against a remote one (API)."""
 
 from uuid import uuid4
 from pathlib import Path
 from ..abstract import AbstractContext
 
 from robotmk.config import Config, RobotmkConfigSchema
+from .target import Target, TargetFactory
 
-# from .target import Target, RobotFrameworkTarget, RCCTarget, RemoteTarget
-from .target import Target
-from .target.factory import TargetFactory
 import time, os
 
 
 class SuiteContext(AbstractContext):
     def __init__(self):
         super().__init__()
         # the target object
```

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/abstract.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/factory.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/factory.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/local.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/rcc.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/remote.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .local import Target
+from .abstract import Target
 from ..strategies import RunStrategy
 from robotmk.logger import RobotmkLogger
 
 
 class RemoteTarget(Target):
     def __init__(self, suiteuname: str, config: dict, logger: RobotmkLogger):
         super().__init__(suiteuname, config, logger)
```

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.61/src/robotmk/context/suite/target/target.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/emitter.py` & `robotmk-0.0.61/src/robotmk/emitter.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/executor/scheduler.py` & `robotmk-0.0.61/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.61/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/logger.py` & `robotmk-0.0.61/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/src/robotmk/main.py` & `robotmk-0.0.61/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/config/robotmk.yml` & `robotmk-0.0.61/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/config/test_config.py` & `robotmk-0.0.61/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/context/local/test_local_cli.py` & `robotmk-0.0.61/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.61/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/context/suite/robotmk.yml` & `robotmk-0.0.61/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.61/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/context/test_cli.py` & `robotmk-0.0.61/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/test_robotmk.py` & `robotmk-0.0.61/tests/test_robotmk.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/tests/yml/robotmk.yml` & `robotmk-0.0.61/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.60/PKG-INFO` & `robotmk-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.60
+Version: 0.0.61
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```


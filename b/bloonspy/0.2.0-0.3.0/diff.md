# Comparing `tmp/bloonspy-0.2.0.tar.gz` & `tmp/bloonspy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloonspy-0.2.0.tar", last modified: Thu Apr  6 14:22:22 2023, max compression
+gzip compressed data, was "bloonspy-0.3.0.tar", last modified: Thu Apr 27 14:43:53 2023, max compression
```

## Comparing `bloonspy-0.2.0.tar` & `bloonspy-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.732745 bloonspy-0.2.0/
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1073 2023-03-20 22:51:50.000000 bloonspy-0.2.0/LICENSE
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1113 2023-04-06 14:22:22.732345 bloonspy-0.2.0/PKG-INFO
--rw-r--r--   0 riccardosartori   (501) staff       (20)      658 2023-03-26 13:17:54.000000 bloonspy-0.2.0/README.md
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.695235 bloonspy-0.2.0/bloonspy/
--rw-r--r--   0 riccardosartori   (501) staff       (20)     9087 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/Client.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      125 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/__init__.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      209 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/exceptions.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.702175 bloonspy-0.2.0/bloonspy/model/
--rw-r--r--   0 riccardosartori   (501) staff       (20)      164 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/Asset.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     3035 2023-03-26 19:33:02.000000 bloonspy-0.2.0/bloonspy/model/Event.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      633 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/GameVersion.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1679 2023-03-26 19:33:02.000000 bloonspy-0.2.0/bloonspy/model/Loadable.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      118 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/__init__.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.713568 bloonspy-0.2.0/bloonspy/model/btd6/
--rw-r--r--   0 riccardosartori   (501) staff       (20)    10824 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/Boss.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)    14129 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/Challenge.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     5732 2023-03-26 19:33:02.000000 bloonspy-0.2.0/bloonspy/model/btd6/ContestedTerritory.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1735 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/Gamemode.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     3330 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/btd6/Medals.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     8596 2023-03-26 19:33:02.000000 bloonspy-0.2.0/bloonspy/model/btd6/Odyssey.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1261 2023-03-20 21:26:25.000000 bloonspy-0.2.0/bloonspy/model/btd6/Power.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     4981 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/Race.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      643 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/btd6/Restriction.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      465 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/btd6/Rewards.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     3304 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/model/btd6/Team.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     3299 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/Tower.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)    12230 2023-04-06 14:21:53.000000 bloonspy-0.2.0/bloonspy/model/btd6/User.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      277 2023-03-22 14:15:23.000000 bloonspy-0.2.0/bloonspy/model/btd6/__init__.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.717794 bloonspy-0.2.0/bloonspy/utils/
--rw-r--r--   0 riccardosartori   (501) staff       (20)      467 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/utils/Infinity.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)       31 2023-03-21 12:50:39.000000 bloonspy-0.2.0/bloonspy/utils/__init__.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1182 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/utils/api.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      761 2023-03-26 12:46:39.000000 bloonspy-0.2.0/bloonspy/utils/decorators.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      705 2023-03-21 21:08:10.000000 bloonspy-0.2.0/bloonspy/utils/dictionaries.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.698085 bloonspy-0.2.0/bloonspy.egg-info/
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1113 2023-04-06 14:22:22.000000 bloonspy-0.2.0/bloonspy.egg-info/PKG-INFO
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1495 2023-04-06 14:22:22.000000 bloonspy-0.2.0/bloonspy.egg-info/SOURCES.txt
--rw-r--r--   0 riccardosartori   (501) staff       (20)        1 2023-04-06 14:22:22.000000 bloonspy-0.2.0/bloonspy.egg-info/dependency_links.txt
--rw-r--r--   0 riccardosartori   (501) staff       (20)       15 2023-04-06 14:22:22.000000 bloonspy-0.2.0/bloonspy.egg-info/top_level.txt
--rw-r--r--   0 riccardosartori   (501) staff       (20)       38 2023-04-06 14:22:22.732895 bloonspy-0.2.0/setup.cfg
--rw-r--r--   0 riccardosartori   (501) staff       (20)      932 2023-04-06 14:21:53.000000 bloonspy-0.2.0/setup.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.718783 bloonspy-0.2.0/tests/
--rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:43.000000 bloonspy-0.2.0/tests/__init__.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.724714 bloonspy-0.2.0/tests/integration/
--rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:59.000000 bloonspy-0.2.0/tests/integration/__init__.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     2265 2023-04-06 14:21:53.000000 bloonspy-0.2.0/tests/integration/test_boss_leaderboard.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      886 2023-04-06 14:21:53.000000 bloonspy-0.2.0/tests/integration/test_challenge_browser.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      728 2023-03-26 11:28:22.000000 bloonspy-0.2.0/tests/integration/test_challenge_creator.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1780 2023-03-26 12:46:39.000000 bloonspy-0.2.0/tests/integration/test_ct_leaderboard.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      691 2023-03-26 12:46:39.000000 bloonspy-0.2.0/tests/integration/test_fetch_odyssey.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      904 2023-03-26 12:46:39.000000 bloonspy-0.2.0/tests/integration/test_fetch_user.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1166 2023-03-26 12:46:39.000000 bloonspy-0.2.0/tests/integration/test_race_leaderboard.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)      644 2023-03-22 12:23:42.000000 bloonspy-0.2.0/tests/integration/test_team_owner.py
-drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-06 14:22:22.731670 bloonspy-0.2.0/tests/unit/
--rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:51.000000 bloonspy-0.2.0/tests/unit/__init__.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     2060 2023-03-22 14:41:08.000000 bloonspy-0.2.0/tests/unit/test_boss.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     4057 2023-03-24 16:11:59.000000 bloonspy-0.2.0/tests/unit/test_challenge.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1381 2023-03-23 10:34:38.000000 bloonspy-0.2.0/tests/unit/test_ct.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     3679 2023-03-24 11:25:25.000000 bloonspy-0.2.0/tests/unit/test_odyssey.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1307 2023-03-21 20:52:03.000000 bloonspy-0.2.0/tests/unit/test_race.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     1831 2023-03-26 12:46:39.000000 bloonspy-0.2.0/tests/unit/test_team.py
--rw-r--r--   0 riccardosartori   (501) staff       (20)     7569 2023-04-06 14:21:53.000000 bloonspy-0.2.0/tests/unit/test_user.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.959954 bloonspy-0.3.0/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1073 2023-03-20 22:51:50.000000 bloonspy-0.3.0/LICENSE
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1108 2023-04-27 14:43:53.959467 bloonspy-0.3.0/PKG-INFO
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      653 2023-04-27 14:42:42.000000 bloonspy-0.3.0/README.md
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.904214 bloonspy-0.3.0/bloonspy/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     9087 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/Client.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      125 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/__init__.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      209 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/exceptions.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.914802 bloonspy-0.3.0/bloonspy/model/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      164 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/Asset.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     3257 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/model/Event.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      633 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/GameVersion.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1901 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/model/Loadable.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      118 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/__init__.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.930097 bloonspy-0.3.0/bloonspy/model/btd6/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)    10824 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/model/btd6/Boss.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)    14420 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/model/btd6/Challenge.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     5732 2023-03-26 19:33:02.000000 bloonspy-0.3.0/bloonspy/model/btd6/ContestedTerritory.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1735 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/model/btd6/Gamemode.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     3330 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/btd6/Medals.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     9272 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/model/btd6/Odyssey.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1261 2023-03-20 21:26:25.000000 bloonspy-0.3.0/bloonspy/model/btd6/Power.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     4981 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/model/btd6/Race.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      643 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/btd6/Restriction.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      510 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/model/btd6/Rewards.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     3304 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/model/btd6/Team.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     3299 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/model/btd6/Tower.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)    12230 2023-04-06 14:21:53.000000 bloonspy-0.3.0/bloonspy/model/btd6/User.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      277 2023-03-22 14:15:23.000000 bloonspy-0.3.0/bloonspy/model/btd6/__init__.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.935604 bloonspy-0.3.0/bloonspy/utils/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      467 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/utils/Infinity.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)       31 2023-03-21 12:50:39.000000 bloonspy-0.3.0/bloonspy/utils/__init__.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1976 2023-04-27 14:42:42.000000 bloonspy-0.3.0/bloonspy/utils/api.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      761 2023-03-26 12:46:39.000000 bloonspy-0.3.0/bloonspy/utils/decorators.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      705 2023-03-21 21:08:10.000000 bloonspy-0.3.0/bloonspy/utils/dictionaries.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.909267 bloonspy-0.3.0/bloonspy.egg-info/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1108 2023-04-27 14:43:53.000000 bloonspy-0.3.0/bloonspy.egg-info/PKG-INFO
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1532 2023-04-27 14:43:53.000000 bloonspy-0.3.0/bloonspy.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardosartori   (501) staff       (20)        1 2023-04-27 14:43:53.000000 bloonspy-0.3.0/bloonspy.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardosartori   (501) staff       (20)       15 2023-04-27 14:43:53.000000 bloonspy-0.3.0/bloonspy.egg-info/top_level.txt
+-rw-r--r--   0 riccardosartori   (501) staff       (20)       38 2023-04-27 14:43:53.960136 bloonspy-0.3.0/setup.cfg
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      932 2023-04-06 14:21:53.000000 bloonspy-0.3.0/setup.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.937629 bloonspy-0.3.0/tests/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:43.000000 bloonspy-0.3.0/tests/__init__.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.948208 bloonspy-0.3.0/tests/integration/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:59.000000 bloonspy-0.3.0/tests/integration/__init__.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      886 2023-04-11 18:26:03.000000 bloonspy-0.3.0/tests/integration/_test_ratelimit.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     2265 2023-04-06 14:21:53.000000 bloonspy-0.3.0/tests/integration/test_boss_leaderboard.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      886 2023-04-06 14:21:53.000000 bloonspy-0.3.0/tests/integration/test_challenge_browser.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      728 2023-03-26 11:28:22.000000 bloonspy-0.3.0/tests/integration/test_challenge_creator.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1780 2023-03-26 12:46:39.000000 bloonspy-0.3.0/tests/integration/test_ct_leaderboard.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      691 2023-03-26 12:46:39.000000 bloonspy-0.3.0/tests/integration/test_fetch_odyssey.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      904 2023-03-26 12:46:39.000000 bloonspy-0.3.0/tests/integration/test_fetch_user.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1166 2023-03-26 12:46:39.000000 bloonspy-0.3.0/tests/integration/test_race_leaderboard.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)      644 2023-03-22 12:23:42.000000 bloonspy-0.3.0/tests/integration/test_team_owner.py
+drwxr-xr-x   0 riccardosartori   (501) staff       (20)        0 2023-04-27 14:43:53.958418 bloonspy-0.3.0/tests/unit/
+-rw-r--r--   0 riccardosartori   (501) staff       (20)        0 2023-03-21 15:24:51.000000 bloonspy-0.3.0/tests/unit/__init__.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     2060 2023-03-22 14:41:08.000000 bloonspy-0.3.0/tests/unit/test_boss.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     4086 2023-04-27 14:42:42.000000 bloonspy-0.3.0/tests/unit/test_challenge.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1381 2023-03-23 10:34:38.000000 bloonspy-0.3.0/tests/unit/test_ct.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     3725 2023-04-27 14:42:42.000000 bloonspy-0.3.0/tests/unit/test_odyssey.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1307 2023-03-21 20:52:03.000000 bloonspy-0.3.0/tests/unit/test_race.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     1831 2023-03-26 12:46:39.000000 bloonspy-0.3.0/tests/unit/test_team.py
+-rw-r--r--   0 riccardosartori   (501) staff       (20)     7569 2023-04-06 14:21:53.000000 bloonspy-0.3.0/tests/unit/test_user.py
```

### Comparing `bloonspy-0.2.0/LICENSE` & `bloonspy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/PKG-INFO` & `bloonspy-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bloonspy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python wrapper for the Ninja Kiwi Open Data API
 Home-page: https://github.com/SartoRiccardo/bloonspy
 Author: TheSartorsss
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BloonsPy
 
-BloonsPy is a Python wrapper for the [Ninja Kiwi Open Data API](https://data.ninjakiwi.com/).
+BloonsPy is a Python wrapper for the [Ninja Kiwi Open Data API](https://data.ninjakiwi.com/),
+that makes you write more readable code and handles rate limiting automatically.
 
 ## Installing
 
 **Python 3.10 or higher is required**
 
 ```bash
 python3 -m pip install bloonspy
@@ -28,16 +29,16 @@
 ## Quick example
 
 ```python
 from bloonspy import Client
 
 boss_event = Client.bosses()[0].standard()
 boss_standard_top_3 = boss_event.leaderboard()[:3]
-for player in boss_standard_top_3:
-    minutes, seconds = int(player.score.seconds/60), int(player.score.seconds%60) 
-    print(f"{player.name} - {minutes}:{seconds}")
+for player in boss_standard_top_3: 
+    print(f"{player.name} - {player.score}")
 ```
 
 ## Resources
 + [Documentation](https://bloonspy.readthedocs.io/en/latest/)
 + [Github](https://github.com/SartoRiccardo/bloonspy)
 
+
```

### Comparing `bloonspy-0.2.0/bloonspy/Client.py` & `bloonspy-0.3.0/bloonspy/Client.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/Event.py` & `bloonspy-0.3.0/bloonspy/model/Event.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 from ..utils.dictionaries import has_all_keys
 from ..utils.decorators import fetch_property, exception_handler
 from ..utils.api import get
 from ..exceptions import NotFound
 
 
 class Event:
-    """A game event."""
+    """A game event.
+
+    .. container:: operations
+
+       .. describe:: x == y
+
+          Checks if the Event is equal to another Event.
+    """
 
     event_endpoint: str = "/..."
     event_dict_keys: List[str] = ["name", "start", "end"]
     event_name: str = "event"
 
     def __init__(self, event_id: str, eager: bool = False, event_json: Dict[str, Any] = None):
         self._id = event_id
@@ -85,7 +92,10 @@
         return self._data["start"]
 
     @property
     @fetch_property(load_event, should_load=_should_load_property("end"))
     def end(self) -> datetime:
         """When the event ends."""
         return self._data["end"]
+
+    def __eq__(self, other):
+        return isinstance(other, type(self)) and other.id == self.id
```

### Comparing `bloonspy-0.2.0/bloonspy/model/GameVersion.py` & `bloonspy-0.3.0/bloonspy/model/GameVersion.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/Loadable.py` & `bloonspy-0.3.0/bloonspy/model/Loadable.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from typing import Dict, Any
 from ..utils.api import get
 from ..utils.decorators import exception_handler
 
 
 class Loadable:
-    """Represents a resource that can be loaded."""
+    """Represents a resource that can be loaded.
+
+    .. container:: operations
+
+       .. describe:: x == y
+
+          Checks if the Event is equal to another Event.
+    """
     endpoint = "{}"
 
     def __init__(self, resource_id: str, eager: bool = False):
         self._id = resource_id
         self._data = {}
         self._loaded = False
         if eager:
@@ -50,7 +57,10 @@
         """The unique ID of the resource."""
         return self._id
 
     @property
     def loaded(self) -> bool:
         """`True` if the resource is loaded."""
         return self._loaded
+
+    def __eq__(self, other):
+        return isinstance(other, type(self)) and other.id == self.id
```

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Boss.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Boss.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Challenge.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def _parse_json(self, raw_challenge: Dict[str, Any]) -> None:
         self._loaded = False
 
         copy_keys = [
             "name", "disableDoubleCash", "disableInstas", "disableMK", "disablePowers", "disableSelling",
             "startingCash", "noContinues", "seed", "roundSets", "lives", "maxLives",
             "startRound", "endRound", "maxTowers", "maxParagons", "plays", "wins", "losses", "upvotes", "playsUnique",
-            "winsUnique", "lossesUnique"
+            "winsUnique", "lossesUnique", "restarts"
         ]
         for key in copy_keys:
             self._data[key] = raw_challenge[key]
 
         # self._data["maxTowers"] = Infinity() if raw_challenge["maxTowers"] == 9999 else raw_challenge["maxTowers"]
         # self._data["maxParagons"] = Infinity() if raw_challenge["maxParagons"] == 10 else raw_challenge["maxParagons"]
         self._data["leastCash"] = Infinity() if raw_challenge["leastCashUsed"] == -1 else raw_challenge["leastCashUsed"]
@@ -168,15 +168,15 @@
 
     @property
     @fetch_property(Loadable.load_resource, should_load=Loadable._should_load_property("creatorId"))
     def creator_id(self) -> str:
         """The ID of the challenge's creator. `None` if there isn't one (e.g. Odyssey challenges)."""
         return self._data["creatorId"]
 
-    @fetch_property(Loadable.load_resource)
+    @fetch_property(Loadable.load_resource, should_load=Loadable._should_load_property("creatorId"))
     def creator(self) -> User or None:
         """Fetch the creator of the challenge.
 
         .. warning::
            This function needs the property :attr:`~bloonspy.model.btd6.Challenge.creator_id` to be
            loaded, or it will make another API call to fetch that first.
 
@@ -311,14 +311,22 @@
     @fetch_property(Loadable.load_resource)
     def losses_unique(self) -> int:
         """Amount of unique people that have lost the challenge."""
         return self._data["lossesUnique"]
 
     @property
     @fetch_property(Loadable.load_resource)
+    def restarts(self) -> int:
+        """*New in 0.3.0*
+
+        The number of times users have restarted the challenge."""
+        return self._data["restarts"]
+
+    @property
+    @fetch_property(Loadable.load_resource)
     def upvotes(self) -> int:
         """Amount of upvotes the challenge has."""
         return self._data["upvotes"]
 
     @property
     @fetch_property(Loadable.load_resource)
     def least_cash_used(self) -> Union[int, Infinity]:
```

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/ContestedTerritory.py` & `bloonspy-0.3.0/bloonspy/model/btd6/ContestedTerritory.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Gamemode.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Gamemode.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Medals.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Medals.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Odyssey.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Odyssey.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
 
 class Odyssey(Loadable):
     """Represents a single Odyssey. Inherits from :class:`~bloonspy.model.Loadable`."""
     endpoint = "/btd6/odyssey/{}/:difficulty:"
     map_endpoint = "/btd6/odyssey/{}/:difficulty:/maps"
 
-    def __init__(self, resource_id: str, name: str, difficulty: OdysseyDifficulty, eager: bool = False):
+    def __init__(self, resource_id: str, name: str, description: str,
+                 difficulty: OdysseyDifficulty, eager: bool = False):
         self.endpoint = self.endpoint.replace(":difficulty:", difficulty.value)
         self.map_endpoint = self.map_endpoint.replace(":difficulty:", difficulty.value)
         super().__init__(resource_id, eager)
         self._name = name
+        self._description = description
         self._difficulty = difficulty
 
     def _parse_json(self, raw_odyssey: Dict[str, Any]) -> None:
         self._loaded = False
 
         copy_keys = [
             "isExtreme", "maxMonkeySeats", "maxMonkeysOnBoat", "maxPowerSlots", "startingHealth",
@@ -85,14 +87,21 @@
 
     @property
     def name(self) -> str:
         """The Odyssey's name"""
         return self._name
 
     @property
+    def description(self) -> str:
+        """*New in 0.3.0*
+
+        The Odyssey's description"""
+        return self._description
+
+    @property
     def difficulty(self) -> OdysseyDifficulty:
         """The Odysseys's difficulty"""
         return self._difficulty
 
     @property
     @fetch_property(Loadable.load_resource)
     def is_extreme(self) -> bool:
@@ -160,14 +169,26 @@
 
 
 class OdysseyEvent(Event):
     """An Odyssey event. Inherits from :class:`~bloonspy.model.Event`."""
     event_endpoint = "/btd6/odyssey"
     event_name = "Odyssey"
 
+    def _parse_event(self, data: Dict[str, Any]) -> None:
+        self._data["description"] = data["description"]
+        super()._parse_event(data)
+
+    @property
+    @fetch_property(Event.load_event, should_load=Event._should_load_property("description"))
+    def description(self) -> str:
+        """*New in 0.3.0*
+
+        The Odyssey's description."""
+        return self._data["description"]
+
     def easy(self, eager: bool = False) -> Odyssey:
         """Get the easy mode version of the Odyssey.
 
         .. note::
            If lazily loaded, the returned :class:`~bloonspy.model.btd6.Odyssey` object will only
            have the properties :attr:`~bloonspy.model.Loadable.id`, :attr:`~bloonspy.model.btd6.Odyssey.name`,
            and :attr:`~bloonspy.model.Odyssey.difficulty` loaded.
@@ -175,15 +196,15 @@
         :param eager: If `True`, it loads all of the data right away. Set it to `False`
             if you want to limit API calls and don't need all the data. For more information,
             please read `Lazy and Eager Loading <async.html#lazy-and-eager-loading>`_.
         :type eager: bool
         :return: The easy mode of the odyssey.
         :rtype: ~bloonspy.model.btd6.Odyssey
         """
-        return Odyssey(self.id, self.name, OdysseyDifficulty.EASY, eager=eager)
+        return Odyssey(self.id, self.name, self.description, OdysseyDifficulty.EASY, eager=eager)
 
     def medium(self, eager: bool = False) -> Odyssey:
         """Get the medium mode version of the Odyssey.
 
         .. note::
            If lazily loaded, the returned :class:`~bloonspy.model.btd6.Odyssey` object will only
            have the properties :attr:`~bloonspy.model.Loadable.id`, :attr:`~bloonspy.model.btd6.Odyssey.name`,
@@ -192,15 +213,15 @@
         :param eager: If `True`, it loads all of the data right away. Set it to `False`
             if you want to limit API calls and don't need all the data. For more information,
             please read `Lazy and Eager Loading <async.html#lazy-and-eager-loading>`_.
         :type eager: bool
         :return: The medium mode of the odyssey.
         :rtype: ~bloonspy.model.btd6.Odyssey
         """
-        return Odyssey(self.id, self.name, OdysseyDifficulty.EASY, eager=eager)
+        return Odyssey(self.id, self.name, self.description, OdysseyDifficulty.MEDIUM, eager=eager)
 
     def hard(self, eager: bool = False) -> Odyssey:
         """Get the hard mode version of the Odyssey.
 
         .. note::
            If lazily loaded, the returned :class:`~bloonspy.model.btd6.Odyssey` object will only
            have the properties :attr:`~bloonspy.model.Loadable.id`, :attr:`~bloonspy.model.btd6.Odyssey.name`,
@@ -209,8 +230,8 @@
         :param eager: If `True`, it loads all of the data right away. Set it to `False`
             if you want to limit API calls and don't need all the data. For more information,
             please read `Lazy and Eager Loading <async.html#lazy-and-eager-loading>`_.
         :type eager: bool
         :return: The hard mode of the odyssey.
         :rtype: ~bloonspy.model.btd6.Odyssey
         """
-        return Odyssey(self.id, self.name, OdysseyDifficulty.EASY, eager=eager)
+        return Odyssey(self.id, self.name, self.description, OdysseyDifficulty.HARD, eager=eager)
```

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Power.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Power.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Race.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Race.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Restriction.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Restriction.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Team.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Team.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/Tower.py` & `bloonspy-0.3.0/bloonspy/model/btd6/Tower.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/model/btd6/User.py` & `bloonspy-0.3.0/bloonspy/model/btd6/User.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/utils/decorators.py` & `bloonspy-0.3.0/bloonspy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy/utils/dictionaries.py` & `bloonspy-0.3.0/bloonspy/utils/dictionaries.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/bloonspy.egg-info/PKG-INFO` & `bloonspy-0.3.0/bloonspy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bloonspy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python wrapper for the Ninja Kiwi Open Data API
 Home-page: https://github.com/SartoRiccardo/bloonspy
 Author: TheSartorsss
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BloonsPy
 
-BloonsPy is a Python wrapper for the [Ninja Kiwi Open Data API](https://data.ninjakiwi.com/).
+BloonsPy is a Python wrapper for the [Ninja Kiwi Open Data API](https://data.ninjakiwi.com/),
+that makes you write more readable code and handles rate limiting automatically.
 
 ## Installing
 
 **Python 3.10 or higher is required**
 
 ```bash
 python3 -m pip install bloonspy
@@ -28,16 +29,16 @@
 ## Quick example
 
 ```python
 from bloonspy import Client
 
 boss_event = Client.bosses()[0].standard()
 boss_standard_top_3 = boss_event.leaderboard()[:3]
-for player in boss_standard_top_3:
-    minutes, seconds = int(player.score.seconds/60), int(player.score.seconds%60) 
-    print(f"{player.name} - {minutes}:{seconds}")
+for player in boss_standard_top_3: 
+    print(f"{player.name} - {player.score}")
 ```
 
 ## Resources
 + [Documentation](https://bloonspy.readthedocs.io/en/latest/)
 + [Github](https://github.com/SartoRiccardo/bloonspy)
 
+
```

### Comparing `bloonspy-0.2.0/bloonspy.egg-info/SOURCES.txt` & `bloonspy-0.3.0/bloonspy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 bloonspy/utils/Infinity.py
 bloonspy/utils/__init__.py
 bloonspy/utils/api.py
 bloonspy/utils/decorators.py
 bloonspy/utils/dictionaries.py
 tests/__init__.py
 tests/integration/__init__.py
+tests/integration/_test_ratelimit.py
 tests/integration/test_boss_leaderboard.py
 tests/integration/test_challenge_browser.py
 tests/integration/test_challenge_creator.py
 tests/integration/test_ct_leaderboard.py
 tests/integration/test_fetch_odyssey.py
 tests/integration/test_fetch_user.py
 tests/integration/test_race_leaderboard.py
```

### Comparing `bloonspy-0.2.0/setup.py` & `bloonspy-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_boss_leaderboard.py` & `bloonspy-0.3.0/tests/integration/test_boss_leaderboard.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_challenge_browser.py` & `bloonspy-0.3.0/tests/integration/test_challenge_browser.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_challenge_creator.py` & `bloonspy-0.3.0/tests/integration/test_challenge_creator.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_ct_leaderboard.py` & `bloonspy-0.3.0/tests/integration/test_ct_leaderboard.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_fetch_odyssey.py` & `bloonspy-0.3.0/tests/integration/test_fetch_odyssey.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_fetch_user.py` & `bloonspy-0.3.0/tests/integration/test_fetch_user.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_race_leaderboard.py` & `bloonspy-0.3.0/tests/integration/test_race_leaderboard.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/integration/test_team_owner.py` & `bloonspy-0.3.0/tests/integration/test_team_owner.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/unit/test_boss.py` & `bloonspy-0.3.0/tests/unit/test_boss.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/unit/test_challenge.py` & `bloonspy-0.3.0/tests/unit/test_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             ("starting_lives", 150),
             ("max_lives", 9999),
             ("start_round", 1),
             ("end_round", 51),
             ("max_towers", 9999),
             ("max_paragons", 10),
             ("round_sets", ["default"]),
+            ("restarts", 0),
             # All values are defaults on this challenge anyway
             ("modifiers", btd6.ChallengeModifier()),
         ]
         for attr_name, attr_expected_value in expected_results:
             self.assertEqual(
                 getattr(challenge, attr_name), attr_expected_value,
                 msg=f"Asserting challenge.{attr_name}"
```

### Comparing `bloonspy-0.2.0/tests/unit/test_ct.py` & `bloonspy-0.3.0/tests/unit/test_ct.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/unit/test_odyssey.py` & `bloonspy-0.3.0/tests/unit/test_odyssey.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,27 @@
         Test that an odyssey event is loaded correctly.
         """
         odysseys = requests.get("https://data.ninjakiwi.com/btd6/odyssey")
         odyssey_id = odysseys.json()["body"][0]["id"]
         odyssey = btd6.OdysseyEvent(odyssey_id)
 
         check_instance = [
-            ("name", str), ("start", datetime), ("end", datetime), ("id", str)
+            ("name", str), ("start", datetime), ("end", datetime), ("id", str), ("description", str),
         ]
         for attr_name, attr_type in check_instance:
             self.assertIsInstance(getattr(odyssey, attr_name), attr_type,
                                   msg=f"Assert if OdysseyEvent.{attr_name} is {attr_type}")
 
         easy_mode = odyssey.easy()
         medium_mode = odyssey.medium(eager=True)
         hard_mode = odyssey.hard()
 
         check_instance = [
             ("name", str), ("difficulty", btd6.OdysseyDifficulty), ("is_extreme", bool), ("max_monkey_seats", int),
-            ("max_boat_seats", int), ("max_power_slots", int), ("starting_lives", int)
+            ("max_boat_seats", int), ("max_power_slots", int), ("starting_lives", int), ("description", str),
         ]
         for attr_name, attr_type in check_instance:
             self.assertIsInstance(getattr(hard_mode, attr_name), attr_type,
                                   msg=f"Assert if Odyssey.{attr_name} is {attr_type}")
 
         for power in medium_mode.available_powers.keys():
             self.assertIsInstance(power, btd6.Power,
```

### Comparing `bloonspy-0.2.0/tests/unit/test_race.py` & `bloonspy-0.3.0/tests/unit/test_race.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/unit/test_team.py` & `bloonspy-0.3.0/tests/unit/test_team.py`

 * *Files identical despite different names*

### Comparing `bloonspy-0.2.0/tests/unit/test_user.py` & `bloonspy-0.3.0/tests/unit/test_user.py`

 * *Files identical despite different names*


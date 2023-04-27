# Comparing `tmp/QuasarCode-0.7.4.tar.gz` & `tmp/QuasarCode-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-2yl3qifs\QuasarCode-0.7.4.tar", last modified: Wed Mar 29 21:34:32 2023, max compression
+gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-dl633exp\QuasarCode-0.7.5.tar", last modified: Thu Apr 27 10:38:29 2023, max compression
```

## Comparing `QuasarCode-0.7.4.tar` & `QuasarCode-0.7.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/
--rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/LICENSE.txt
--rw-rw-rw-   0        0        0      826 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/README.md
--rw-rw-rw-   0        0        0      920 2023-03-29 21:34:03.000000 QuasarCode-0.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Games/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/
--rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardGroup.py
--rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardQueue.py
--rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardStack.py
--rw-rw-rw-   0        0        0     4886 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_Deck.py
--rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_IPlayingCard.py
--rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_PlayingCard.py
--rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Cards/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/
--rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_Dice12.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_Dice6.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_Dice8.py
--rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_DiceCup.py
--rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_IDice.py
--rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_NDice.py
--rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Dice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/
--rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/_ISpinner.py
--rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/_Spinner.py
--rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/__init__.py
--rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/IO/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/
--rw-rw-rw-   0        0        0     3470 2023-03-28 00:46:45.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_ConfigsBase.py
--rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/__init__.py
--rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_json.py
--rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_properties.py
--rw-rw-rw-   0        0        0     1765 2023-03-28 00:45:09.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_yaml.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Text/
--rw-rw-rw-   0        0        0       23 2023-03-26 16:23:05.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Text/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-03-26 16:33:38.000000 QuasarCode-0.7.4/src/QuasarCode/IO/Text/console.py
--rw-rw-rw-   0        0        0       50 2023-03-26 01:12:29.000000 QuasarCode-0.7.4/src/QuasarCode/IO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/MPI/
--rw-rw-rw-   0        0        0      989 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/MPI/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/MPI/_mpi_configs.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Science/
--rw-rw-rw-   0        0        0      290 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Science/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Science/data.py
--rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Science/figure.py
--rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Science/fitline.py
--rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Science/graph.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/
--rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/StringLiterals.py
--rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/Validators.py
--rw-rw-rw-   0        0        0      210 2023-03-26 01:50:12.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/__init__.py
--rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/_async.py
--rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/_directorys_and_imports.py
--rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/_multiItterator.py
--rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/_networking.py
--rw-rw-rw-   0        0        0    12109 2023-03-29 21:30:30.000000 QuasarCode-0.7.4/src/QuasarCode/Tools/_script_wrapper.py
--rw-rw-rw-   0        0        0      697 2023-03-29 21:34:03.000000 QuasarCode-0.7.4/src/QuasarCode/__init__.py
--rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.7.4/src/QuasarCode/_global_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode/edp/
--rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/edp/_Event.py
--rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/edp/_NotEnoughArgumentsError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/edp/_SubscriberNotPresentError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.4/src/QuasarCode/edp/_UndersubscribedEventError.py
--rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.7.4/src/QuasarCode/edp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/
--rw-rw-rw-   0        0        0      826 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2052 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 21:34:32.000000 QuasarCode-0.7.4/src/QuasarCode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/
+-rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      826 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/README.md
+-rw-rw-rw-   0        0        0      920 2023-04-27 10:35:36.000000 QuasarCode-0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Games/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/
+-rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardGroup.py
+-rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardQueue.py
+-rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardStack.py
+-rw-rw-rw-   0        0        0     4886 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_Deck.py
+-rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_IPlayingCard.py
+-rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_PlayingCard.py
+-rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Cards/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/
+-rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_Dice12.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_Dice6.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_Dice8.py
+-rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_DiceCup.py
+-rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_IDice.py
+-rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_NDice.py
+-rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Dice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/
+-rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/_ISpinner.py
+-rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/_Spinner.py
+-rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/IO/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/
+-rw-rw-rw-   0        0        0     3931 2023-04-27 10:32:41.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_ConfigsBase.py
+-rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/__init__.py
+-rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_json.py
+-rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_properties.py
+-rw-rw-rw-   0        0        0     1765 2023-03-28 00:45:09.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Text/
+-rw-rw-rw-   0        0        0       23 2023-03-26 16:23:05.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Text/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-03-26 16:33:38.000000 QuasarCode-0.7.5/src/QuasarCode/IO/Text/console.py
+-rw-rw-rw-   0        0        0       50 2023-03-26 01:12:29.000000 QuasarCode-0.7.5/src/QuasarCode/IO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/MPI/
+-rw-rw-rw-   0        0        0      989 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/MPI/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/MPI/_mpi_configs.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Science/
+-rw-rw-rw-   0        0        0      290 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Science/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Science/data.py
+-rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Science/figure.py
+-rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Science/fitline.py
+-rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Science/graph.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/
+-rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/StringLiterals.py
+-rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/Validators.py
+-rw-rw-rw-   0        0        0      210 2023-03-26 01:50:12.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/_async.py
+-rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/_directorys_and_imports.py
+-rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/_multiItterator.py
+-rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/_networking.py
+-rw-rw-rw-   0        0        0    12109 2023-03-29 21:30:30.000000 QuasarCode-0.7.5/src/QuasarCode/Tools/_script_wrapper.py
+-rw-rw-rw-   0        0        0      697 2023-04-27 10:35:44.000000 QuasarCode-0.7.5/src/QuasarCode/__init__.py
+-rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.7.5/src/QuasarCode/_global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode/edp/
+-rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/edp/_Event.py
+-rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/edp/_NotEnoughArgumentsError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/edp/_SubscriberNotPresentError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.5/src/QuasarCode/edp/_UndersubscribedEventError.py
+-rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.7.5/src/QuasarCode/edp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/
+-rw-rw-rw-   0        0        0      826 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 10:38:29.000000 QuasarCode-0.7.5/src/QuasarCode.egg-info/top_level.txt
```

### Comparing `QuasarCode-0.7.4/LICENSE.txt` & `QuasarCode-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/PKG-INFO` & `QuasarCode-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.7.4
+Version: 0.7.5
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.7.4/pyproject.toml` & `QuasarCode-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
 
 [project]
 name = "QuasarCode"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="Christopher Rowe", email="thequasarx1@gmail.com" },
 ]
 description = "A general purpose library for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardGroup.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardGroup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardQueue.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardQueue.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_CardStack.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_CardStack.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_Deck.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_Deck.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_IPlayingCard.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_IPlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Cards/_PlayingCard.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Cards/_PlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_DiceCup.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_DiceCup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Dice/_NDice.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Dice/_NDice.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/_ISpinner.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/_ISpinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Games/Spinners/_Spinner.py` & `QuasarCode-0.7.5/src/QuasarCode/Games/Spinners/_Spinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_json.py` & `QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_json.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_properties.py` & `QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_properties.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/IO/Configurations/_yaml.py` & `QuasarCode-0.7.5/src/QuasarCode/IO/Configurations/_yaml.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/IO/Text/console.py` & `QuasarCode-0.7.5/src/QuasarCode/IO/Text/console.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/MPI/__init__.py` & `QuasarCode-0.7.5/src/QuasarCode/MPI/__init__.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/MPI/_mpi_configs.py` & `QuasarCode-0.7.5/src/QuasarCode/MPI/_mpi_configs.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Science/data.py` & `QuasarCode-0.7.5/src/QuasarCode/Science/data.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Science/figure.py` & `QuasarCode-0.7.5/src/QuasarCode/Science/figure.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Science/fitline.py` & `QuasarCode-0.7.5/src/QuasarCode/Science/fitline.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Science/graph.py` & `QuasarCode-0.7.5/src/QuasarCode/Science/graph.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/StringLiterals.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/StringLiterals.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/Validators.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/Validators.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/_directorys_and_imports.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/_directorys_and_imports.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/_multiItterator.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/_multiItterator.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/_networking.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/_networking.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/Tools/_script_wrapper.py` & `QuasarCode-0.7.5/src/QuasarCode/Tools/_script_wrapper.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/__init__.py` & `QuasarCode-0.7.5/src/QuasarCode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Adds functionality to Python along with wrapers for existing modules for ease of use
 
 Credits:
     Written by Christopher Rowe
     Notable contribusions taken from code written by Tim Greenshaw 10/2018
 
-Version: 0.7.4
+Version: 0.7.5
 """
 
 from ._global_settings import settings_object as Settings
 
 from . import edp
 
 from . import Games
```

### Comparing `QuasarCode-0.7.4/src/QuasarCode/_global_settings.py` & `QuasarCode-0.7.5/src/QuasarCode/_global_settings.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode/edp/_Event.py` & `QuasarCode-0.7.5/src/QuasarCode/edp/_Event.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.4/src/QuasarCode.egg-info/PKG-INFO` & `QuasarCode-0.7.5/src/QuasarCode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.7.4
+Version: 0.7.5
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.7.4/src/QuasarCode.egg-info/SOURCES.txt` & `QuasarCode-0.7.5/src/QuasarCode.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pgx-0.5.3.tar.gz` & `tmp/pgx-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.5.3.tar", last modified: Wed Apr 26 02:23:28 2023, max compression
+gzip compressed data, was "pgx-6.0.0.tar", last modified: Thu Apr 27 07:07:19 2023, max compression
```

## Comparing `pgx-0.5.3.tar` & `pgx-6.0.0.tar`

### file list

```diff
@@ -1,140 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.324855 pgx-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 02:23:18.000000 pgx-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-26 02:23:28.324855 pgx-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-26 02:23:18.000000 pgx-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.308855 pgx-0.5.3/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26088 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 02:23:19.000000 pgx-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:23:28.324855 pgx-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-26 02:23:19.000000 pgx-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.324855 pgx-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39645 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.850134 pgx-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 07:07:03.000000 pgx-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-27 07:07:19.850134 pgx-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-27 07:07:03.000000 pgx-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.834133 pgx-6.0.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.834133 pgx-6.0.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.838134 pgx-6.0.0/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.838134 pgx-6.0.0/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.838134 pgx-6.0.0/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.842134 pgx-6.0.0/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.842134 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37401 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.846134 pgx-6.0.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.846134 pgx-6.0.0/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-04-27 07:07:03.000000 pgx-6.0.0/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.834133 pgx-6.0.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-27 07:07:19.000000 pgx-6.0.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-27 07:07:19.000000 pgx-6.0.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:07:19.000000 pgx-6.0.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 07:07:19.000000 pgx-6.0.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 07:07:19.000000 pgx-6.0.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 07:07:03.000000 pgx-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:07:19.850134 pgx-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 07:07:03.000000 pgx-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:19.850134 pgx-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61899 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29758 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39651 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-27 07:07:03.000000 pgx-6.0.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.5.3/LICENSE` & `pgx-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/PKG-INFO` & `pgx-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.3
+Version: 6.0.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.3 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 6.0.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.3/README.md` & `pgx-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_mahjong/_hand.py` & `pgx-6.0.0/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_mahjong/_meld.py` & `pgx-6.0.0/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_mahjong/_shanten.py` & `pgx-6.0.0/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_mahjong/_yaku.py` & `pgx-6.0.0/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/api_test.py` & `pgx-6.0.0/pgx/_src/api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from pgx.experimental.utils import act_randomly
 from pgx.v1 import Env, State, available_games
 
 act_randomly = jax.jit(act_randomly)
 
 
-def api_test(env: Env, num: int = 100):
+def v1_api_test(env: Env, num: int = 100):
     api_test_single(env, num)
     api_test_batch(env, num)
 
 
 def api_test_single(env: Env, num: int = 100):
     """validate checks these items:
 
@@ -151,15 +151,14 @@
 
     # check public attributes
     public_attributes = [
         "current_player",
         "observation",
         "reward",
         "terminated",
-        "truncated",
         "legal_action_mask",
     ]
     for k, v in state.__dict__.items():
         if k.startswith("_"):  # internal
             continue
         assert k in public_attributes
```

### Comparing `pgx-0.5.3/pgx/_src/chess_utils.py` & `pgx-6.0.0/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/animalshogi.py` & `pgx-6.0.0/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/backgammon.py` & `pgx-6.0.0/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/bridge_bidding.py` & `pgx-6.0.0/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/chess.py` & `pgx-6.0.0/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/connect_four.py` & `pgx-6.0.0/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/go.py` & `pgx-6.0.0/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/hex.py` & `pgx-6.0.0/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/LICENSE` & `pgx-6.0.0/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-6.0.0/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-6.0.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/kuhn_poker.py` & `pgx-6.0.0/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/leduc_holdem.py` & `pgx-6.0.0/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/othello.py` & `pgx-6.0.0/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/play2048.py` & `pgx-6.0.0/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/shogi.py` & `pgx-6.0.0/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-6.0.0/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/dwg/tictactoe.py` & `pgx-6.0.0/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/shogi_utils.py` & `pgx-6.0.0/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/struct.py` & `pgx-6.0.0/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/_src/visualizer.py` & `pgx-6.0.0/pgx/_src/visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/animal_shogi.py` & `pgx-6.0.0/pgx/animal_shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(132, dtype=jnp.bool_)  # (132,)
     observation: jnp.ndarray = jnp.zeros((4, 3, 22), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     _board: jnp.ndarray = INIT_BOARD  # (12,)
@@ -76,17 +75,17 @@
             is_drop,
             lambda: Action(is_drop=TRUE, to=sq, drop_piece=x - 8),  # type: ignore
             lambda: Action(is_drop=FALSE, from_=sq, to=_to(sq, x)),  # type: ignore
         )
 
 
 class AnimalShogi(v1.Env):
-    def __init__(self, max_termination_steps: int = 200):
-        super().__init__()
-        self.max_termination_steps = max_termination_steps
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
+        self.max_termination_steps: int = 200
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         state = state.replace(legal_action_mask=_legal_action_mask(state))  # type: ignore
         return state
```

### Comparing `pgx-0.5.3/pgx/backgammon.py` & `pgx-6.0.0/pgx/backgammon.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(34, dtype=jnp.int8)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     # micro action = 6 * src + die
     legal_action_mask: jnp.ndarray = jnp.zeros(6 * 26 + 6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Backgammon specific ---
     # 各point(24) bar(2) off(2)にあるcheckerの数. 黒+, 白-
     _board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
@@ -51,18 +50,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "backgammon"
 
 
 class Backgammon(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/bridge_bidding.py` & `pgx-6.0.0/pgx/bridge_bidding.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(-1)
     observation: jnp.ndarray = jnp.zeros(478, dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0, 0, 0, 0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(38, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # turn 現在のターン数
     _turn: jnp.ndarray = jnp.int16(0)
     # シャッフルされたプレイヤーの並び
     _shuffled_players: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
@@ -87,16 +86,21 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "bridge_bidding"
 
 
 class BridgeBidding(v1.Env):
-    def __init__(self, *, dds_hash_table_path: Optional[str] = None):
-        super().__init__()
+    def __init__(
+        self,
+        *,
+        auto_reset: bool = False,
+        dds_hash_table_path: Optional[str] = None
+    ):
+        super().__init__(auto_reset=auto_reset)
         if dds_hash_table_path is None:
             dds_hash_table_path = os.path.join(
                 os.getcwd(), "dds_hash_table.npz"
             )
         try:
             self.hash_keys, self.hash_values = jnp.load(dds_hash_table_path)
         except FileNotFoundError as e:
@@ -138,17 +142,17 @@
 
 
 @jax.jit
 def init(rng: jax.random.KeyArray) -> State:
     rng1, rng2, rng3, rng4, rng5, rng6 = jax.random.split(rng, num=6)
     hand = jnp.arange(0, 52)
     hand = jax.random.permutation(rng2, hand)
-    vul_NS = jax.random.randint(rng3, (1,), 0, 2)[0]
-    vul_EW = jax.random.randint(rng4, (1,), 0, 2)[0]
-    dealer = jax.random.randint(rng5, (1,), 0, 4)[0]
+    vul_NS = jax.random.choice(rng3, jnp.bool_([False, True]))
+    vul_EW = jax.random.choice(rng4, jnp.bool_([False, True]))
+    dealer = jax.random.randint(rng5, (1,), 0, 4, dtype=jnp.int8)[0]
     # shuffled players and arrange in order of NESW
     shuffled_players = _shuffle_players(rng6)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
     legal_actions = legal_actions.at[36].set(False)
     legal_actions = legal_actions.at[37].set(False)
@@ -165,17 +169,17 @@
 
 
 @jax.jit
 def _init_by_key(key: jnp.ndarray, rng: jax.random.KeyArray) -> State:
     """Make init state from key"""
     rng1, rng2, rng3, rng4, rng5 = jax.random.split(rng, num=5)
     hand = _key_to_hand(key)
-    vul_NS = jax.random.randint(rng2, (1,), 0, 2)[0]
-    vul_EW = jax.random.randint(rng3, (1,), 0, 2)[0]
-    dealer = jax.random.randint(rng4, (1,), 0, 4)[0]
+    vul_NS = jax.random.choice(rng2, jnp.bool_([False, True]))
+    vul_EW = jax.random.choice(rng3, jnp.bool_([False, True]))
+    dealer = jax.random.randint(rng4, (1,), 0, 4, dtype=jnp.int8)[0]
     # shuffled players and arrange in order of NESW
     shuffled_players = _shuffle_players(rng5)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
     legal_actions = legal_actions.at[36].set(False)
     legal_actions = legal_actions.at[37].set(False)
```

### Comparing `pgx-0.5.3/pgx/chess.py` & `pgx-6.0.0/pgx/chess.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # 64 * 73 = 4672
     observation: jnp.ndarray = jnp.zeros((8, 8, 19), dtype=jnp.float32)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Chess specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     _board: jnp.ndarray = INIT_BOARD  # 左上からFENと同じ形式で埋めていく
@@ -180,16 +179,16 @@
     def _to_label(self):
         plane = PLANE_MAP[self.from_, self.to]
         # plane = jax.lax.select(self.underpromotion >= 0, ..., plane)
         return jnp.int32(self.from_) * 73 + jnp.int32(plane)
 
 
 class Chess(v1.Env):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
         # AlphaZero paper does not mention the number of max termination steps
         # but we believe 1000 is large enough for Chess.
         self.max_termination_steps = 1000
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
@@ -584,16 +583,20 @@
         & (jnp.abs(a.to - a.from_) > 2)
         & (state._board[a.to] >= 0)
     )
     return (a.to >= 0) & ok
 
 
 def _possible_piece_positions(state):
-    my_pos = jnp.nonzero(state._board > 0, size=16, fill_value=-1)[0]
-    opp_pos = jnp.nonzero(_flip(state)._board > 0, size=16, fill_value=-1)[0]
+    my_pos = jnp.nonzero(state._board > 0, size=16, fill_value=-1)[0].astype(
+        jnp.int8
+    )
+    opp_pos = jnp.nonzero(_flip(state)._board > 0, size=16, fill_value=-1)[
+        0
+    ].astype(jnp.int8)
     return jnp.vstack((my_pos, opp_pos))
 
 
 def _observe(state: State):
     """Our observation design is very similar to OpenSpiel
     except two differences:
```

### Comparing `pgx-0.5.3/pgx/connect_four.py` & `pgx-6.0.0/pgx/connect_four.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((6, 7, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(7, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Connect Four specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 6x7 board
     # [[ 0,  1,  2,  3,  4,  5,  6],
@@ -46,18 +45,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "connect_four"
 
 
 class ConnectFour(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/experimental/bridge_bidding.py` & `pgx-6.0.0/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/experimental/gym.py` & `pgx-6.0.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/experimental/pettingzoo.py` & `pgx-6.0.0/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/experimental/visualize.py` & `pgx-6.0.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/go.py` & `pgx-6.0.0/pgx/go.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(19 * 19 + 1, dtype=jnp.bool_)
     observation: jnp.ndarray = jnp.zeros((19, 19, 17), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Go specific ---
     _size: jnp.ndarray = jnp.int32(19)  # NOTE: require 19 * 19 > int8
     # ids of representative stone id (smallest) in the connected stones
@@ -59,19 +58,20 @@
         return f"go-{size}x{size}"  # type: ignore
 
 
 class Go(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         size: int = 19,
         komi: float = 7.5,
         history_length: int = 8,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         assert isinstance(size, int)
         self.size = size
         self.komi = komi
         self.history_length = history_length
         self.max_termination_steps = self.size * self.size * 2
 
     def _init(self, key: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.5.3/pgx/hex.py` & `pgx-6.0.0/pgx/hex.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((11, 11, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(11 * 11, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Hex specific ---
     _size: jnp.ndarray = jnp.int8(11)
     # 0(black), 1(white)
     _turn: jnp.ndarray = jnp.int8(0)
@@ -51,20 +50,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "hex"
 
 
 class Hex(v1.Env):
-    def __init__(
-        self,
-        *,
-        size: int = 11,
-    ):
-        super().__init__()
+    def __init__(self, *, size: int = 11, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
         assert isinstance(size, int)
         self.size = size
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return partial(_init, size=self.size)(rng=key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
```

### Comparing `pgx-0.5.3/pgx/kuhn_poker.py` & `pgx-6.0.0/pgx/kuhn_poker.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Kuhn poker specific ---
     _cards: jnp.ndarray = jnp.int8([-1, -1])
     # [(player 0),(player 1)]
     _last_action: jnp.ndarray = jnp.int8(-1)
@@ -45,18 +44,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "kuhn_poker"
 
 
 class KuhnPoker(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/leduc_holdem.py` & `pgx-6.0.0/pgx/leduc_holdem.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Leduc Hold'Em specific ---
     _first_player: jnp.ndarray = jnp.int8(0)
     # [(player 0), (player 1), (public)]
     _cards: jnp.ndarray = jnp.int8([-1, -1, -1])
@@ -51,18 +50,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "leduc_holdem"
 
 
 class LeducHoldem(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/minatar/asterix.py` & `pgx-6.0.0/pgx/minatar/asterix.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(5, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Asterix specific ---
     _player_x: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _player_y: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _entities: jnp.ndarray = jnp.ones((8, 4), dtype=jnp.int32) * INF
@@ -74,18 +73,19 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarAsterix(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
```

### Comparing `pgx-0.5.3/pgx/minatar/breakout.py` & `pgx-6.0.0/pgx/minatar/breakout.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Breakout specific ---
     _ball_y: jnp.ndarray = THREE
     _ball_x: jnp.ndarray = ZERO
     _ball_dir: jnp.ndarray = TWO
@@ -75,18 +74,19 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarBreakout(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 3])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
```

### Comparing `pgx-0.5.3/pgx/minatar/freeway.py` & `pgx-6.0.0/pgx/minatar/freeway.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 7), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Freeway specific ---
     _cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
     _pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
     _move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
@@ -65,18 +64,19 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarFreeway(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 2, 4])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
```

### Comparing `pgx-0.5.3/pgx/minatar/seaquest.py` & `pgx-6.0.0/pgx/minatar/seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 10), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Seaquest specific ---
     _oxygen: jnp.ndarray = MAX_OXYGEN
     _diver_count: jnp.ndarray = ZERO
     _sub_x: jnp.ndarray = jnp.int32(5)
@@ -86,18 +85,19 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSeaquest(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4, 5])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
```

### Comparing `pgx-0.5.3/pgx/minatar/space_invaders.py` & `pgx-6.0.0/pgx/minatar/space_invaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 6), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar SpaceInvaders specific ---
     _pos: jnp.ndarray = jnp.int32(5)
     _f_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
     _e_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
@@ -75,18 +74,19 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSpaceInvaders(v1.Env):
     def __init__(
         self,
         *,
+        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__()
+        super().__init__(auto_reset=auto_reset)
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 3, 5])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
```

### Comparing `pgx-0.5.3/pgx/minatar/utils.py` & `pgx-6.0.0/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/pgx/othello.py` & `pgx-6.0.0/pgx/othello.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(64 + 1, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Othello specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 8x8 board
     # [[ 0,  1,  2,  3,  4,  5,  6,  7],
@@ -48,18 +47,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "othello"
 
 
 class Othello(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/play2048.py` & `pgx-6.0.0/pgx/play2048.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(16, dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- 2048 specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 4x4 board
     # [[ 0,  1,  2,  3],
@@ -56,18 +55,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "2048"
 
 
 class Play2048(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/shogi.py` & `pgx-6.0.0/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # (27 * 81,)
     observation: jnp.ndarray = jnp.zeros((119, 9, 9), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Shogi specific ---
     _turn: jnp.ndarray = jnp.int8(0)  # 0 or 1
     _board: jnp.ndarray = INIT_PIECE_BOARD  # (81,) 後手のときにはflipする
@@ -111,16 +110,18 @@
 
     def _to_sfen(self):
         state = self if self._turn % 2 == 0 else _flip(self)
         return _to_sfen(state)
 
 
 class Shogi(v1.Env):
-    def __init__(self, max_termination_steps: int = 1000):
-        super().__init__()
+    def __init__(
+        self, *, auto_reset: bool = False, max_termination_steps: int = 1000
+    ):
+        super().__init__(auto_reset=auto_reset)
         self.max_termination_steps = max_termination_steps
 
     def _init(self, key: jax.random.KeyArray) -> State:
         state = _init_board()
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         return state.replace(current_player=current_player)  # type: ignore
```

### Comparing `pgx-0.5.3/pgx/sparrow_mahjong.py` & `pgx-6.0.0/pgx/sparrow_mahjong.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((15, 11), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(3, dtype=jnp.float32)
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Sparrow Mahjong specific ---
     _turn: jnp.ndarray = jnp.int32(0)  # 0 = dealer
     _rivers: jnp.ndarray = -jnp.ones(
         (N_PLAYER, MAX_RIVER_LENGTH), dtype=jnp.int32
@@ -90,18 +89,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
 
 class SparrowMahjong(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key, subkey = jax.random.split(key)
         state = _init(subkey)
 
         def f(x):
             k, _subkey = jax.random.split(x[0])
```

### Comparing `pgx-0.5.3/pgx/tic_tac_toe.py` & `pgx-6.0.0/pgx/tic_tac_toe.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((3, 3, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
-    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Tic-tac-toe specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 0 1 2
     # 3 4 5
@@ -41,18 +40,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
 
 class TicTacToe(v1.Env):
-    def __init__(
-        self,
-    ):
-        super().__init__()
+    def __init__(self, *, auto_reset: bool = False):
+        super().__init__(auto_reset=auto_reset)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
```

### Comparing `pgx-0.5.3/pgx/v1.py` & `pgx-6.0.0/pgx/v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,24 +79,22 @@
             `Env.observe` is called to compute.
         reward (jnp.ndarray): the `i`-th element indicates the intermediate reward for
             the agent with player-id `i`. If `Env.step` is called for a terminal state,
             the following `state.reward` is zero for all players.
         terminated (jnp.ndarray): denotes that the state is termianl state. Note that
             some environments (e.g., Go) have an `max_termination_steps` parameter inside
             and will terminates within a limited number of states (following AlphaGo).
-        truncated (jnp.ndarray): so far, not used as all Pgx environments are finite horizon
         legal_action_mask (jnp.ndarray): Boolean array of legal actions. If illegal action is taken,
             the game will terminate immediately with the penalty to the palyer.
     """
 
     current_player: jnp.ndarray
     observation: jnp.ndarray
     reward: jnp.ndarray
     terminated: jnp.ndarray
-    truncated: jnp.ndarray  # so far, not used as all Pgx environments are finite horizon
     legal_action_mask: jnp.ndarray
     # NOTE: _rng_key is
     #   - used for stochastic env and auto reset
     #   - updated only when actually used
     #   - supposed NOT to be used by agent
     _rng_key: jax.random.KeyArray
     _step_count: jnp.ndarray
@@ -162,16 +160,16 @@
         state = env.init(jax.random.PRNGKey(0))
         action = jax.random.int32(4)
         state = env.step(state, action)
         ```
 
     """
 
-    def __init__(self):
-        ...
+    def __init__(self, *, auto_reset: bool = False):
+        self.auto_reset = auto_reset
 
     def init(self, key: jax.random.KeyArray) -> State:
         """Return the initial state. Note that no internal state of
         environment changes.
 
         Args:
             key: pseudo-random generator key in JAX
@@ -187,18 +185,29 @@
         return state.replace(observation=observation)  # type: ignore
 
     def step(self, state: State, action: jnp.ndarray) -> State:
         """Step function."""
         is_illegal = ~state.legal_action_mask[action]
         current_player = state.current_player
 
+        # auto reset
+        state = jax.lax.cond(
+            self.auto_reset & state.terminated,
+            lambda: state.replace(  # type: ignore
+                _step_count=jnp.int32(0),
+                terminated=FALSE,
+                reward=jnp.zeros_like(state.reward),
+            ),
+            lambda: state,
+        )
+
         # If the state is already terminated or truncated, environment does not take usual step,
         # but return the same state with zero-rewards for all players
         state = jax.lax.cond(
-            (state.terminated | state.truncated),
+            state.terminated,
             lambda: state.replace(reward=jnp.zeros_like(state.reward)),  # type: ignore
             lambda: self._step(state.replace(_step_count=state._step_count + 1), action),  # type: ignore
         )
 
         # Taking illegal action leads to immediate game terminal with negative reward
         state = jax.lax.cond(
             is_illegal,
@@ -206,23 +215,49 @@
             lambda: state,
         )
 
         # All legal_action_mask elements are **TRUE** at terminal state
         # This is to avoid zero-division error when normalizing action probability
         # Taking any action at terminal state does not give any effect to the state
         state = jax.lax.cond(
-            (state.terminated | state.truncated),
+            state.terminated,
             lambda: state.replace(  # type: ignore
                 legal_action_mask=jnp.ones_like(state.legal_action_mask)
             ),
             lambda: state,
         )
 
         observation = self.observe(state, state.current_player)
-        return state.replace(observation=observation)  # type: ignore
+        state = state.replace(observation=observation)  # type: ignore
+
+        # auto reset
+        state = jax.lax.cond(
+            self.auto_reset & state.terminated,
+            # state is replaced by initial state,
+            # but preserve (terminated, truncated, reward)
+            lambda: self.init(state._rng_key).replace(  # type: ignore
+                terminated=state.terminated,
+                reward=state.reward,
+            ),
+            lambda: state,
+        )
+        # NOTE on final observation
+        # When auto reset happened, the terminal (or truncated) observation is replaced by initial observation,
+        # This is NOT problematic if it's termination.
+        # However, when truncation happened, final observation might be used by agent (for bootstrap)
+        # So we have to preserve the final observation somewhere. For example, in Gymnasium,
+        #
+        # https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/wrappers/autoreset.py#L59
+        #
+        # However, currently, truncation does **NOT** actually happens in Pgx environments because
+        # all of Pgx environments (games) are finite-horizon and terminates within reasonable # of steps.
+        # (NOTE: Chess, Shogi, and Go have `max_termination_steps` parameter following AlphaZero paper)
+        # So we believe current implementation is sufficient (final observation is not necessary).
+
+        return state
 
     def observe(self, state: State, player_id: jnp.ndarray) -> jnp.ndarray:
         """Observation function."""
         obs = self._observe(state, player_id)
         return jax.lax.stop_gradient(obs)
 
     @abc.abstractmethod
@@ -291,93 +326,93 @@
         return state.replace(reward=reward, terminated=TRUE)  # type: ignore
 
 
 def available_games() -> Tuple[EnvId, ...]:
     return get_args(EnvId)
 
 
-def make(env_id: EnvId):  # noqa: C901
+def make(env_id: EnvId, *, auto_reset: bool = False):  # noqa: C901
     if env_id == "2048":
         from pgx.play2048 import Play2048
 
-        return Play2048()
+        return Play2048(auto_reset=auto_reset)
     elif env_id == "animal_shogi":
         from pgx.animal_shogi import AnimalShogi
 
-        return AnimalShogi()
+        return AnimalShogi(auto_reset=auto_reset)
     elif env_id == "backgammon":
         from pgx.backgammon import Backgammon
 
-        return Backgammon()
+        return Backgammon(auto_reset=auto_reset)
     elif env_id == "bridge_bidding":
         from pgx.bridge_bidding import BridgeBidding
 
-        return BridgeBidding(dds_hash_table_path=None)
+        return BridgeBidding(auto_reset=auto_reset, dds_hash_table_path=None)
     elif env_id == "chess":
         from pgx.chess import Chess
 
-        return Chess()
+        return Chess(auto_reset=auto_reset)
     elif env_id == "connect_four":
         from pgx.connect_four import ConnectFour
 
-        return ConnectFour()
+        return ConnectFour(auto_reset=auto_reset)
     elif env_id == "go-9x9":
         from pgx.go import Go
 
-        return Go(size=9, komi=7.5)
+        return Go(auto_reset=auto_reset, size=9, komi=7.5)
     elif env_id == "go-19x19":
         from pgx.go import Go
 
-        return Go(size=19, komi=7.5)
+        return Go(auto_reset=auto_reset, size=19, komi=7.5)
     elif env_id == "hex":
         from pgx.hex import Hex
 
-        return Hex()
+        return Hex(auto_reset=auto_reset)
     elif env_id == "kuhn_poker":
         from pgx.kuhn_poker import KuhnPoker
 
-        return KuhnPoker()
+        return KuhnPoker(auto_reset=auto_reset)
     elif env_id == "leduc_holdem":
         from pgx.leduc_holdem import LeducHoldem
 
-        return LeducHoldem()
+        return LeducHoldem(auto_reset=auto_reset)
     elif env_id == "minatar/asterix":
         from pgx.minatar.asterix import MinAtarAsterix
 
-        return MinAtarAsterix()
+        return MinAtarAsterix(auto_reset=auto_reset)
     elif env_id == "minatar/breakout":
         from pgx.minatar.breakout import MinAtarBreakout
 
-        return MinAtarBreakout()
+        return MinAtarBreakout(auto_reset=auto_reset)
     elif env_id == "minatar/freeway":
         from pgx.minatar.freeway import MinAtarFreeway
 
-        return MinAtarFreeway()
+        return MinAtarFreeway(auto_reset=auto_reset)
     elif env_id == "minatar/seaquest":
         from pgx.minatar.seaquest import MinAtarSeaquest
 
-        return MinAtarSeaquest()
+        return MinAtarSeaquest(auto_reset=auto_reset)
     elif env_id == "minatar/space_invaders":
         from pgx.minatar.space_invaders import MinAtarSpaceInvaders
 
-        return MinAtarSpaceInvaders()
+        return MinAtarSpaceInvaders(auto_reset=auto_reset)
     elif env_id == "othello":
         from pgx.othello import Othello
 
-        return Othello()
+        return Othello(auto_reset=auto_reset)
     elif env_id == "shogi":
         from pgx.shogi import Shogi
 
-        return Shogi()
+        return Shogi(auto_reset=auto_reset)
     elif env_id == "sparrow_mahjong":
         from pgx.sparrow_mahjong import SparrowMahjong
 
-        return SparrowMahjong()
+        return SparrowMahjong(auto_reset=auto_reset)
     elif env_id == "tic_tac_toe":
         from pgx.tic_tac_toe import TicTacToe
 
-        return TicTacToe()
+        return TicTacToe(auto_reset=auto_reset)
     else:
         available_envs = "\n".join(available_games())
         raise ValueError(
             f"Wrong env_id is passed. Available ids are: \n{available_envs}"
         )
```

### Comparing `pgx-0.5.3/pgx.egg-info/PKG-INFO` & `pgx-6.0.0/pgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.3
+Version: 6.0.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.3 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 6.0.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.3/pgx.egg-info/SOURCES.txt` & `pgx-6.0.0/pgx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 pgx/_src/dwg/images/sparrow_mahjong/rd.svg
 pgx/experimental/__init__.py
 pgx/experimental/bridge_bidding.py
 pgx/experimental/gym.py
 pgx/experimental/pettingzoo.py
 pgx/experimental/utils.py
 pgx/experimental/visualize.py
-pgx/experimental/wrappers.py
 pgx/minatar/__init__.py
 pgx/minatar/asterix.py
 pgx/minatar/breakout.py
 pgx/minatar/freeway.py
 pgx/minatar/seaquest.py
 pgx/minatar/space_invaders.py
 pgx/minatar/utils.py
```

### Comparing `pgx-0.5.3/setup.py` & `pgx-6.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.5.3",
+    version="6.0.0",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
-    package_data={"": ["LICENSE", "*.svg"]},
+    package_data={"": ["LICENSE", "*.svg", "*.npy"]},
     include_package_data=True,
     install_requires=[
         "jax>=0.3.25",  # JAX version on Colab (TPU)
         "svgwrite",
         "typing_extensions"
     ],
     classifiers=[
```

### Comparing `pgx-0.5.3/tests/minatar_utils.py` & `pgx-6.0.0/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/tests/test_animal_shogi.py` & `pgx-6.0.0/tests/test_animal_shogi.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,8 @@
                           False, False])
     assert (state.observation[0, 0, 10:] == expected).all()
 
 
 def test_api():
     import pgx
     env = pgx.make("animal_shogi")
-    pgx.api_test(env, 5)
+    pgx.v1_api_test(env, 5)
```

### Comparing `pgx-0.5.3/tests/test_asterix.py` & `pgx-6.0.0/tests/test_asterix.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,8 +104,8 @@
     state = jax.jit(env.step)(state, 0)
     assert state.legal_action_mask.shape == (5,)
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/asterix")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_backgammon.py` & `pgx-6.0.0/tests/test_backgammon.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,8 +570,8 @@
     playable_dice = jnp.array([1, 1, -1, -1])
     legal_action_mask = _legal_action_mask(board, playable_dice)
     print("1, 1", jnp.where(legal_action_mask != 0)[0])
 
 def test_api():
     import pgx
     env = pgx.make("backgammon")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_breakout.py` & `pgx-6.0.0/tests/test_breakout.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,8 +93,8 @@
     state = jax.jit(env.step)(state, 0)
     assert state.legal_action_mask.shape == (3,)
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/breakout")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_bridge_bidding.py` & `pgx-6.0.0/tests/test_bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1746,15 +1746,15 @@
 
 def test_api():
     import pgx
 
     env = pgx.bridge_bidding.BridgeBidding(
         dds_hash_table_path=DDS_HASH_TABLE_PATH
     )
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
 
 
 def to_value(sample: list) -> jnp.ndarray:
     """Convert sample to value
     >>> sample = ['0', '1', '0', '4', '0', '13', '12', '13', '9', '13', '0', '1', '0', '4', '0', '13', '12', '13', '9', '13']
     >>> to_value(sample)
     Array([  4160, 904605,   4160, 904605], dtype=int32)
```

### Comparing `pgx-0.5.3/tests/test_chess.py` & `pgx-6.0.0/tests/test_chess.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,8 +738,8 @@
     # color
     assert (state.observation[:, :, 13] == 1).all()
 
 
 def test_api():
     import pgx
     env = pgx.make("chess")
-    pgx.api_test(env, 5)
+    pgx.v1_api_test(env, 5)
```

### Comparing `pgx-0.5.3/tests/test_connect_four.py` & `pgx-6.0.0/tests/test_connect_four.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,8 +133,8 @@
          [False, True,  False, False, False, False, False]]
     )).all()
     assert obs[:, :, 1].sum() == 0
 
 def test_api():
     import pgx
     env = pgx.make("connect_four")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_freeway.py` & `pgx-6.0.0/tests/test_freeway.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,8 +99,8 @@
     state = jax.jit(env.step)(state, 0)
     assert state.legal_action_mask.shape == (3,)
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/freeway")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_go.py` & `pgx-6.0.0/tests/test_go.py`

 * *Files 0% similar despite different names*

```diff
@@ -1128,10 +1128,10 @@
             break
     assert state._passed or state._turn > 100
 
 
 def test_api():
     import pgx
     env = pgx.make("go-9x9")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
     env = pgx.make("go-19x19")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_hex.py` & `pgx-6.0.0/tests/test_hex.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,8 +124,8 @@
         done = state.terminated
         rewards += state.reward
 
 
 def test_api():
     import pgx
     env = pgx.make("hex")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_kuhn_poker.py` & `pgx-6.0.0/tests/test_kuhn_poker.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,8 +126,8 @@
             done = state.terminated
 
 
 def test_api():
     import pgx
 
     env = pgx.make("kuhn_poker")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_leduc_holdem.py` & `pgx-6.0.0/tests/test_leduc_holdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,8 +172,8 @@
             done = state.terminated
 
 
 def test_api():
     import pgx
 
     env = pgx.make("leduc_holdem")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_mahjong.py` & `pgx-6.0.0/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.3/tests/test_othello.py` & `pgx-6.0.0/tests/test_othello.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
         rewards += state.reward
 
 
 def test_api():
     import pgx
 
     env = pgx.make("othello")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_play2048.py` & `pgx-6.0.0/tests/test_play2048.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,8 @@
         done = state.terminated
 
 
 def test_api():
     import pgx
 
     env = pgx.make("2048")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_seaquest.py` & `pgx-6.0.0/tests/test_seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             obs_pgx,
         )
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/seaquest")
-    pgx.api_test(env)
+    pgx.v1_api_test(env)
 
 
 def test_buggy_sample():
     state = seaquest.State(
         _oxygen=jnp.int32(187),
         _diver_count=jnp.int32(0),
         _sub_x=jnp.int32(0),
@@ -186,8 +186,8 @@
     state = jax.jit(env.step)(state, 0)
     assert state.legal_action_mask.shape == (6,)
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/seaquest")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_shogi.py` & `pgx-6.0.0/tests/test_shogi.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,8 +401,8 @@
     assert s._to_sfen() == sfen
 
 
 def test_api():
     import pgx
     # env = pgx.make("shogi")
     env = Shogi(max_termination_steps=50)
-    pgx.api_test(env, 5)
+    pgx.v1_api_test(env, 5)
```

### Comparing `pgx-0.5.3/tests/test_space_invaders.py` & `pgx-6.0.0/tests/test_space_invaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,8 @@
     assert state.legal_action_mask.shape == (4,)
     state = jax.jit(env.step)(state, 0)
     assert state.legal_action_mask.shape == (4,)
 
 def test_api():
     import pgx
     env = pgx.make("minatar/space_invaders")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_sparrow_mahjong.py` & `pgx-6.0.0/tests/test_sparrow_mahjong.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,8 +583,8 @@
     assert jnp.all(obs[13] == jnp.bool_([0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0]))
     assert jnp.all(obs[14] == jnp.bool_([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]))
 
 
 def test_api():
     import pgx
     env = pgx.make("sparrow_mahjong")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.5.3/tests/test_tic_tac_toe.py` & `pgx-6.0.0/tests/test_tic_tac_toe.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,8 +188,8 @@
     assert (obs == init_obs.at[0, 1, 0].set(1)).all(), obs
 
 
 
 def test_api():
     import pgx
     env = pgx.make("tic_tac_toe")
-    pgx.api_test(env, 10)
+    pgx.v1_api_test(env, 10)
```


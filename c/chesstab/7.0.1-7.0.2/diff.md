# Comparing `tmp/chesstab-7.0.1.tar.gz` & `tmp/chesstab-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesstab-7.0.1.tar", last modified: Wed Apr 26 13:08:40 2023, max compression
+gzip compressed data, was "chesstab-7.0.2.tar", last modified: Thu Apr 27 10:14:25 2023, max compression
```

## Comparing `chesstab-7.0.1.tar` & `chesstab-7.0.2.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.815984 chesstab-7.0.1/
--rw-r--r--   0 roger     (1001) roger     (1001)     1493 2023-01-10 17:52:02.000000 chesstab-7.0.1/LICENCE
--rw-r--r--   0 roger     (1001) roger     (1001)       15 2023-01-10 17:52:02.000000 chesstab-7.0.1/MANIFEST.in
--rw-r--r--   0 roger     (1001) roger     (1001)     6221 2023-04-26 13:08:40.815984 chesstab-7.0.1/PKG-INFO
--rw-r--r--   0 roger     (1001) roger     (1001)     5452 2023-01-10 17:52:02.000000 chesstab-7.0.1/README
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.585984 chesstab-7.0.1/chesstab/
--rw-r--r--   0 roger     (1001) roger     (1001)     5167 2023-03-07 21:53:47.000000 chesstab-7.0.1/chesstab/__init__.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.595983 chesstab-7.0.1/chesstab/apsw/
--rw-r--r--   0 roger     (1001) roger     (1001)      239 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/apsw/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2169 2023-03-07 21:54:24.000000 chesstab-7.0.1/chesstab/apsw/chessapsw.py
--rw-r--r--   0 roger     (1001) roger     (1001)      981 2023-03-07 21:54:43.000000 chesstab-7.0.1/chesstab/apsw/chessapswdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1185 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/apsw/runchessapswdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.605987 chesstab-7.0.1/chesstab/basecore/
--rw-r--r--   0 roger     (1001) roger     (1001)      149 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4064 2023-03-07 21:55:52.000000 chesstab-7.0.1/chesstab/basecore/analysis_index.py
--rw-r--r--   0 roger     (1001) roger     (1001)      547 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/analysisds.py
--rw-r--r--   0 roger     (1001) roger     (1001)      667 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/cqlds.py
--rw-r--r--   0 roger     (1001) roger     (1001)    26881 2023-03-07 21:56:23.000000 chesstab-7.0.1/chesstab/basecore/cqlgames.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6238 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/database.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1391 2023-03-07 21:56:47.000000 chesstab-7.0.1/chesstab/basecore/fullposition.py
--rw-r--r--   0 roger     (1001) roger     (1001)      554 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/fullpositionds.py
--rw-r--r--   0 roger     (1001) roger     (1001)     7254 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/rayfilter.py
--rw-r--r--   0 roger     (1001) roger     (1001)      809 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/selection.py
--rw-r--r--   0 roger     (1001) roger     (1001)      530 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/basecore/selectionds.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.605987 chesstab-7.0.1/chesstab/berkeleydb/
--rw-r--r--   0 roger     (1001) roger     (1001)      391 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/berkeleydb/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2269 2023-03-07 21:57:35.000000 chesstab-7.0.1/chesstab/berkeleydb/chessberkeleydb.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1417 2023-03-07 21:57:57.000000 chesstab-7.0.1/chesstab/berkeleydb/chessberkeleydbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      962 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/berkeleydb/runchessberkeleydbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2822 2023-04-24 19:31:05.000000 chesstab-7.0.1/chesstab/chessgames.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3038 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/chessgames_winedptchunk.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2315 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/chessgames_winedptmulti.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.615984 chesstab-7.0.1/chesstab/core/
--rw-r--r--   0 roger     (1001) roger     (1001)      408 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6476 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/analysis.py
--rw-r--r--   0 roger     (1001) roger     (1001)    33364 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/chessrecord.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3176 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/constants.py
--rw-r--r--   0 roger     (1001) roger     (1001)    28616 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/cqlnode.py
--rw-r--r--   0 roger     (1001) roger     (1001)     7326 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/cqlstatement.py
--rw-r--r--   0 roger     (1001) roger     (1001)     7188 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/engine.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2650 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/export_chessql.py
--rw-r--r--   0 roger     (1001) roger     (1001)    36588 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/export_game.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4284 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/export_pgn_import_format.py
--rw-r--r--   0 roger     (1001) roger     (1001)    12599 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/export_repertoire.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1501 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/export_selection_rule.py
--rw-r--r--   0 roger     (1001) roger     (1001)    13252 2023-03-07 21:58:42.000000 chesstab-7.0.1/chesstab/core/filespec.py
--rw-r--r--   0 roger     (1001) roger     (1001)    22176 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/pgn.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5181 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/querystatement.py
--rw-r--r--   0 roger     (1001) roger     (1001)    24882 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/uci.py
--rw-r--r--   0 roger     (1001) roger     (1001)     9197 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/core/uci_to_pgn.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.625984 chesstab-7.0.1/chesstab/db/
--rw-r--r--   0 roger     (1001) roger     (1001)      393 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/db/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2275 2023-03-07 21:59:34.000000 chesstab-7.0.1/chesstab/db/chessdb.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1392 2023-03-07 21:59:57.000000 chesstab-7.0.1/chesstab/db/chessdbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      924 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/db/runchessdbdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.625984 chesstab-7.0.1/chesstab/db_tkinter/
--rw-r--r--   0 roger     (1001) roger     (1001)      242 2023-01-15 18:20:52.000000 chesstab-7.0.1/chesstab/db_tkinter/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1888 2023-03-07 22:00:51.000000 chesstab-7.0.1/chesstab/db_tkinter/chessdbtkinter.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1167 2023-03-07 22:01:29.000000 chesstab-7.0.1/chesstab/db_tkinter/chessdbtkinterdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      946 2023-01-15 18:20:52.000000 chesstab-7.0.1/chesstab/db_tkinter/runchessdbtkinterdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.635983 chesstab-7.0.1/chesstab/dpt/
--rw-r--r--   0 roger     (1001) roger     (1001)      617 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)      555 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/analysisds.py
--rw-r--r--   0 roger     (1001) roger     (1001)    15114 2023-03-07 22:02:13.000000 chesstab-7.0.1/chesstab/dpt/chessdpt.py
--rw-r--r--   0 roger     (1001) roger     (1001)    25152 2023-03-07 22:02:32.000000 chesstab-7.0.1/chesstab/dpt/chessdptdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      674 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/cqlds.py
--rw-r--r--   0 roger     (1001) roger     (1001)      580 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/fullpositionds.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1758 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/runchessdptdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1837 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/runchessdptduchunk.py
--rw-r--r--   0 roger     (1001) roger     (1001)      537 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/dpt/selectionds.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.655983 chesstab-7.0.1/chesstab/fonts/
--rwxr-xr-x   0 roger     (1001) roger     (1001)    35476 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/CASEFONT.TTF
--rwxr-xr-x   0 roger     (1001) roger     (1001)    41360 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/LUCEFONT.TTF
--rwxr-xr-x   0 roger     (1001) roger     (1001)    49504 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/MERIFONT.TTF
--rwxr-xr-x   0 roger     (1001) roger     (1001)    39732 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/MOTIFONT.TTF
--rw-r--r--   0 roger     (1001) roger     (1001)    27052 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/cases.zip
--rw-r--r--   0 roger     (1001) roger     (1001)    29402 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/lucen.zip
--rw-r--r--   0 roger     (1001) roger     (1001)    27687 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/merid.zip
--rw-r--r--   0 roger     (1001) roger     (1001)    22959 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/fonts/motif.zip
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.655983 chesstab-7.0.1/chesstab/gnu/
--rw-r--r--   0 roger     (1001) roger     (1001)      255 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gnu/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1996 2023-03-07 22:03:12.000000 chesstab-7.0.1/chesstab/gnu/chessgnu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      966 2023-03-07 22:03:31.000000 chesstab-7.0.1/chesstab/gnu/chessgnudu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      923 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gnu/runchessgnudu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.735983 chesstab-7.0.1/chesstab/gui/
--rw-r--r--   0 roger     (1001) roger     (1001)      612 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)      970 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/_lead_trail.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5166 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/_score_scaffold.py
--rw-r--r--   0 roger     (1001) roger     (1001)    18543 2023-04-26 08:13:05.000000 chesstab-7.0.1/chesstab/gui/analysisscore.py
--rw-r--r--   0 roger     (1001) roger     (1001)    11656 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/blanktext.py
--rw-r--r--   0 roger     (1001) roger     (1001)     9154 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/board.py
--rw-r--r--   0 roger     (1001) roger     (1001)    78979 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/chess.py
--rw-r--r--   0 roger     (1001) roger     (1001)    82152 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/chess_ui.py
--rw-r--r--   0 roger     (1001) roger     (1001)    32188 2023-03-07 22:04:03.000000 chesstab-7.0.1/chesstab/gui/chessdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)    28692 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/colourscheme.py
--rw-r--r--   0 roger     (1001) roger     (1001)     9831 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/constants.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5572 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cql.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5078 2023-03-07 22:05:00.000000 chesstab-7.0.1/chesstab/gui/cqldbdelete.py
--rw-r--r--   0 roger     (1001) roger     (1001)     7093 2023-03-07 22:05:20.000000 chesstab-7.0.1/chesstab/gui/cqldbedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2566 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqldbshow.py
--rw-r--r--   0 roger     (1001) roger     (1001)    29778 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqldisplay.py
--rw-r--r--   0 roger     (1001) roger     (1001)      886 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqledit.py
--rw-r--r--   0 roger     (1001) roger     (1001)    18529 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqlgrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3770 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqlrow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6847 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqltext.py
--rw-r--r--   0 roger     (1001) roger     (1001)      880 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/cqltoplevel.py
--rw-r--r--   0 roger     (1001) roger     (1001)     8195 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/display.py
--rw-r--r--   0 roger     (1001) roger     (1001)    12181 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/displayitems.py
--rw-r--r--   0 roger     (1001) roger     (1001)    21302 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/displaypgn.py
--rw-r--r--   0 roger     (1001) roger     (1001)    13516 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/displaytext.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3863 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/engine.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2924 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginedbdelete.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5146 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginedbedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2904 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginedbshow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2393 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/engineedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     9848 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginegrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3786 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginerow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6312 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginetext.py
--rw-r--r--   0 roger     (1001) roger     (1001)      837 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/enginetoplevel.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4161 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/eventbinding.py
--rw-r--r--   0 roger     (1001) roger     (1001)    24236 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/eventspec.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4049 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/fonts.py
--rw-r--r--   0 roger     (1001) roger     (1001)    29759 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/game.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4063 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamedbdelete.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5439 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamedbedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3532 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamedbshow.py
--rw-r--r--   0 roger     (1001) roger     (1001)    11808 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamedisplay.py
--rw-r--r--   0 roger     (1001) roger     (1001)   191548 2023-04-26 12:13:48.000000 chesstab-7.0.1/chesstab/gui/gameedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)    33489 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamegrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)    10598 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamelistgrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     7885 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gamerow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1087 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/gametoplevel.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1026 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/help_.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4915 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/options.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5184 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/positionrow.py
--rw-r--r--   0 roger     (1001) roger     (1001)    20216 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/positionscore.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5275 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/query.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2808 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querydbdelete.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4989 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querydbedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2717 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querydbshow.py
--rw-r--r--   0 roger     (1001) roger     (1001)    27356 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querydisplay.py
--rw-r--r--   0 roger     (1001) roger     (1001)      834 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/queryedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)    19038 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querygrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3775 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/queryrow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5532 2023-03-07 22:05:45.000000 chesstab-7.0.1/chesstab/gui/querytext.py
--rw-r--r--   0 roger     (1001) roger     (1001)      815 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/querytoplevel.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2613 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoire.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3361 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiredbdelete.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4474 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiredbedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3342 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiredbshow.py
--rw-r--r--   0 roger     (1001) roger     (1001)    11341 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiredisplay.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2770 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoireedit.py
--rw-r--r--   0 roger     (1001) roger     (1001)    27910 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiregrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5278 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoirerow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1147 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/repertoiretoplevel.py
--rw-r--r--   0 roger     (1001) roger     (1001)    96417 2023-04-26 08:23:32.000000 chesstab-7.0.1/chesstab/gui/score.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3276 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/scorepgn.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6459 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/sharedtext.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5076 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/gui/toplevelpgn.py
--rw-r--r--   0 roger     (1001) roger     (1001)     4863 2023-01-15 18:13:59.000000 chesstab-7.0.1/chesstab/gui/topleveltext.py
--rw-r--r--   0 roger     (1001) roger     (1001)    30729 2023-01-12 19:08:19.000000 chesstab-7.0.1/chesstab/gui/uci.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.735983 chesstab-7.0.1/chesstab/help_/
--rw-r--r--   0 roger     (1001) roger     (1001)     1234 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1123 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/aboutchesstab.rst
--rw-r--r--   0 roger     (1001) roger     (1001)     1780 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/chesstab.rst
--rw-r--r--   0 roger     (1001) roger     (1001)     3444 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/filesize.rst
--rw-r--r--   0 roger     (1001) roger     (1001)    11921 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/guide.rst
--rw-r--r--   0 roger     (1001) roger     (1001)     3716 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/help_/selection.rst
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.745983 chesstab-7.0.1/chesstab/lmdb/
--rw-r--r--   0 roger     (1001) roger     (1001)      383 2023-03-07 22:22:41.000000 chesstab-7.0.1/chesstab/lmdb/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1776 2023-03-07 22:22:41.000000 chesstab-7.0.1/chesstab/lmdb/chesslmdb.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1840 2023-03-07 22:22:41.000000 chesstab-7.0.1/chesstab/lmdb/chesslmdbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      929 2023-03-07 22:22:41.000000 chesstab-7.0.1/chesstab/lmdb/runchesslmdbdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.745983 chesstab-7.0.1/chesstab/ndbm/
--rw-r--r--   0 roger     (1001) roger     (1001)      252 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/ndbm/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2012 2023-03-07 22:06:28.000000 chesstab-7.0.1/chesstab/ndbm/chessndbm.py
--rw-r--r--   0 roger     (1001) roger     (1001)      977 2023-03-07 22:07:02.000000 chesstab-7.0.1/chesstab/ndbm/chessndbmdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      927 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/ndbm/runchessndbmdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.775983 chesstab-7.0.1/chesstab/samples/
--rw-r--r--   0 roger     (1001) roger     (1001)      335 2023-03-07 22:08:01.000000 chesstab-7.0.1/chesstab/samples/apswdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      299 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/apswdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2622 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/chessboard.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3789 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/chessgame.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3765 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/chessscore.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2878 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/chessscoreboard.py
--rw-r--r--   0 roger     (1001) roger     (1001)      454 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/chesstab.py
--rw-r--r--   0 roger     (1001) roger     (1001)      323 2023-03-07 22:08:25.000000 chesstab-7.0.1/chesstab/samples/dbdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      287 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/dbdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)      359 2023-03-07 22:08:49.000000 chesstab-7.0.1/chesstab/samples/dbtkinterdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      323 2023-01-15 18:16:21.000000 chesstab-7.0.1/chesstab/samples/dbtkinterdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1318 2023-03-07 22:09:30.000000 chesstab-7.0.1/chesstab/samples/directory_widget.py
--rw-r--r--   0 roger     (1001) roger     (1001)      317 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/dptdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2335 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/dptdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1246 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/dptduchunk.py
--rw-r--r--   0 roger     (1001) roger     (1001)      919 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/dptdumulti.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1916 2023-03-07 22:09:49.000000 chesstab-7.0.1/chesstab/samples/file_widget.py
--rw-r--r--   0 roger     (1001) roger     (1001)      333 2023-03-07 22:10:21.000000 chesstab-7.0.1/chesstab/samples/gnudu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      297 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/gnudu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)      364 2023-03-07 22:21:44.000000 chesstab-7.0.1/chesstab/samples/lmdbdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      328 2023-03-07 22:22:03.000000 chesstab-7.0.1/chesstab/samples/lmdbdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)      762 2023-03-07 22:10:51.000000 chesstab-7.0.1/chesstab/samples/ndbmdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      303 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/ndbmdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)      321 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/read_pgn.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1100 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/read_pgn_profile.py
--rw-r--r--   0 roger     (1001) roger     (1001)      351 2023-03-07 22:11:18.000000 chesstab-7.0.1/chesstab/samples/sqlite3du_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      315 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/sqlite3du_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)      353 2023-03-07 22:11:39.000000 chesstab-7.0.1/chesstab/samples/unqlitedu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      317 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/unqlitedu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2365 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/update_players_sqlite3.py
--rw-r--r--   0 roger     (1001) roger     (1001)      341 2023-03-07 22:12:23.000000 chesstab-7.0.1/chesstab/samples/vedisdu_dir.py
--rw-r--r--   0 roger     (1001) roger     (1001)      305 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/vedisdu_file.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1484 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/view_players_bsddb3.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2960 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/samples/view_raw_records_bsddb3.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.795983 chesstab-7.0.1/chesstab/shared/
--rw-r--r--   0 roger     (1001) roger     (1001)      159 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3844 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/alldu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6258 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/allgrid.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1175 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/allrow.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2472 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/archivedu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     5590 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/cql_gamelist_query.py
--rw-r--r--   0 roger     (1001) roger     (1001)     6954 2023-03-07 22:13:09.000000 chesstab-7.0.1/chesstab/shared/dbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      420 2023-01-15 18:10:38.000000 chesstab-7.0.1/chesstab/shared/dbdudb.py
--rw-r--r--   0 roger     (1001) roger     (1001)      692 2023-01-15 18:11:01.000000 chesstab-7.0.1/chesstab/shared/dbdutcl.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1291 2023-01-15 18:09:50.000000 chesstab-7.0.1/chesstab/shared/dptcompatdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1446 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/game_position.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2579 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/litedu.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3014 2023-03-07 22:13:41.000000 chesstab-7.0.1/chesstab/shared/lmdbdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      410 2023-03-07 22:13:58.000000 chesstab-7.0.1/chesstab/shared/lmdbdudb.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3093 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/shared/rundu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.795983 chesstab-7.0.1/chesstab/sqlite/
--rw-r--r--   0 roger     (1001) roger     (1001)      360 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/sqlite/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2186 2023-03-07 22:15:13.000000 chesstab-7.0.1/chesstab/sqlite/chesssqlite3.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1002 2023-03-07 22:15:34.000000 chesstab-7.0.1/chesstab/sqlite/chesssqlite3du.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1193 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/sqlite/runchesssqlite3du.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.805983 chesstab-7.0.1/chesstab/tools/
--rw-r--r--   0 roger     (1001) roger     (1001)      796 2023-03-07 15:46:28.000000 chesstab-7.0.1/chesstab/tools/berkeleydb_du_splice_fix.py
--rw-r--r--   0 roger     (1001) roger     (1001)   182081 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/tools/chesstab-4-1-1_castling-option-correction.py
--rw-r--r--   0 roger     (1001) roger     (1001)     3720 2023-03-07 22:18:35.000000 chesstab-7.0.1/chesstab/tools/create_chesstab_database.py
--rw-r--r--   0 roger     (1001) roger     (1001)      427 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/tools/upgrade_3_to_4.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.805983 chesstab-7.0.1/chesstab/unqlite/
--rw-r--r--   0 roger     (1001) roger     (1001)      242 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/unqlite/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2016 2023-03-07 22:16:29.000000 chesstab-7.0.1/chesstab/unqlite/chessunqlite.py
--rw-r--r--   0 roger     (1001) roger     (1001)     1002 2023-03-07 22:17:00.000000 chesstab-7.0.1/chesstab/unqlite/chessunqlitedu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      935 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/unqlite/runchessunqlitedu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.805983 chesstab-7.0.1/chesstab/vedis/
--rw-r--r--   0 roger     (1001) roger     (1001)      238 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/vedis/__init__.py
--rw-r--r--   0 roger     (1001) roger     (1001)     2000 2023-03-07 22:17:31.000000 chesstab-7.0.1/chesstab/vedis/chessvedis.py
--rw-r--r--   0 roger     (1001) roger     (1001)      980 2023-03-07 22:20:50.000000 chesstab-7.0.1/chesstab/vedis/chessvedisdu.py
--rw-r--r--   0 roger     (1001) roger     (1001)      927 2023-01-10 17:52:02.000000 chesstab-7.0.1/chesstab/vedis/runchessvedisdu.py
-drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-26 13:08:40.585984 chesstab-7.0.1/chesstab.egg-info/
--rw-r--r--   0 roger     (1001) roger     (1001)     6221 2023-04-26 13:08:40.000000 chesstab-7.0.1/chesstab.egg-info/PKG-INFO
--rw-r--r--   0 roger     (1001) roger     (1001)     6831 2023-04-26 13:08:40.000000 chesstab-7.0.1/chesstab.egg-info/SOURCES.txt
--rw-r--r--   0 roger     (1001) roger     (1001)      325 2023-04-26 13:08:40.000000 chesstab-7.0.1/chesstab.egg-info/dependency_links.txt
--rw-r--r--   0 roger     (1001) roger     (1001)      109 2023-04-26 13:08:40.000000 chesstab-7.0.1/chesstab.egg-info/requires.txt
--rw-r--r--   0 roger     (1001) roger     (1001)        9 2023-04-26 13:08:40.000000 chesstab-7.0.1/chesstab.egg-info/top_level.txt
--rw-r--r--   0 roger     (1001) roger     (1001)      135 2023-01-10 17:52:02.000000 chesstab-7.0.1/pyproject.toml
--rw-r--r--   0 roger     (1001) roger     (1001)     1296 2023-04-26 13:08:40.815984 chesstab-7.0.1/setup.cfg
--rw-r--r--   0 roger     (1001) roger     (1001)     1338 2023-01-10 17:52:02.000000 chesstab-7.0.1/setup.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.555983 chesstab-7.0.2/
+-rw-r--r--   0 roger     (1001) roger     (1001)     1493 2023-01-10 17:52:02.000000 chesstab-7.0.2/LICENCE
+-rw-r--r--   0 roger     (1001) roger     (1001)       15 2023-01-10 17:52:02.000000 chesstab-7.0.2/MANIFEST.in
+-rw-r--r--   0 roger     (1001) roger     (1001)     6221 2023-04-27 10:14:25.555983 chesstab-7.0.2/PKG-INFO
+-rw-r--r--   0 roger     (1001) roger     (1001)     5452 2023-01-10 17:52:02.000000 chesstab-7.0.2/README
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.385984 chesstab-7.0.2/chesstab/
+-rw-r--r--   0 roger     (1001) roger     (1001)     5167 2023-03-07 21:53:47.000000 chesstab-7.0.2/chesstab/__init__.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.385984 chesstab-7.0.2/chesstab/apsw/
+-rw-r--r--   0 roger     (1001) roger     (1001)      239 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/apsw/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2169 2023-03-07 21:54:24.000000 chesstab-7.0.2/chesstab/apsw/chessapsw.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      981 2023-03-07 21:54:43.000000 chesstab-7.0.2/chesstab/apsw/chessapswdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1185 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/apsw/runchessapswdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.395984 chesstab-7.0.2/chesstab/basecore/
+-rw-r--r--   0 roger     (1001) roger     (1001)      149 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4064 2023-03-07 21:55:52.000000 chesstab-7.0.2/chesstab/basecore/analysis_index.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      547 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/analysisds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      667 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/cqlds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    26881 2023-03-07 21:56:23.000000 chesstab-7.0.2/chesstab/basecore/cqlgames.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6238 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/database.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1391 2023-03-07 21:56:47.000000 chesstab-7.0.2/chesstab/basecore/fullposition.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      554 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/fullpositionds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     7254 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/rayfilter.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      809 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/selection.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      530 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/basecore/selectionds.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.405983 chesstab-7.0.2/chesstab/berkeleydb/
+-rw-r--r--   0 roger     (1001) roger     (1001)      391 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/berkeleydb/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2269 2023-03-07 21:57:35.000000 chesstab-7.0.2/chesstab/berkeleydb/chessberkeleydb.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1417 2023-03-07 21:57:57.000000 chesstab-7.0.2/chesstab/berkeleydb/chessberkeleydbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      962 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/berkeleydb/runchessberkeleydbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2822 2023-04-24 19:31:05.000000 chesstab-7.0.2/chesstab/chessgames.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3038 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/chessgames_winedptchunk.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2315 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/chessgames_winedptmulti.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.415983 chesstab-7.0.2/chesstab/core/
+-rw-r--r--   0 roger     (1001) roger     (1001)      408 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6476 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/analysis.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    33364 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/chessrecord.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3176 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/constants.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    28616 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/cqlnode.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     7326 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/cqlstatement.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     7188 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/engine.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2650 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/export_chessql.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    36588 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/export_game.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4284 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/export_pgn_import_format.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    12599 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/export_repertoire.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1501 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/export_selection_rule.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    13252 2023-03-07 21:58:42.000000 chesstab-7.0.2/chesstab/core/filespec.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    22176 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/pgn.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5181 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/querystatement.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    24882 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/uci.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     9197 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/core/uci_to_pgn.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.415983 chesstab-7.0.2/chesstab/db/
+-rw-r--r--   0 roger     (1001) roger     (1001)      393 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/db/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2275 2023-03-07 21:59:34.000000 chesstab-7.0.2/chesstab/db/chessdb.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1392 2023-03-07 21:59:57.000000 chesstab-7.0.2/chesstab/db/chessdbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      924 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/db/runchessdbdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.425984 chesstab-7.0.2/chesstab/db_tkinter/
+-rw-r--r--   0 roger     (1001) roger     (1001)      242 2023-01-15 18:20:52.000000 chesstab-7.0.2/chesstab/db_tkinter/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1888 2023-03-07 22:00:51.000000 chesstab-7.0.2/chesstab/db_tkinter/chessdbtkinter.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1167 2023-03-07 22:01:29.000000 chesstab-7.0.2/chesstab/db_tkinter/chessdbtkinterdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      946 2023-01-15 18:20:52.000000 chesstab-7.0.2/chesstab/db_tkinter/runchessdbtkinterdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.425984 chesstab-7.0.2/chesstab/dpt/
+-rw-r--r--   0 roger     (1001) roger     (1001)      617 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      555 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/analysisds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    15114 2023-03-07 22:02:13.000000 chesstab-7.0.2/chesstab/dpt/chessdpt.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    25152 2023-03-07 22:02:32.000000 chesstab-7.0.2/chesstab/dpt/chessdptdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      674 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/cqlds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      580 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/fullpositionds.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1758 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/runchessdptdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1837 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/runchessdptduchunk.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      537 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/dpt/selectionds.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.435983 chesstab-7.0.2/chesstab/fonts/
+-rwxr-xr-x   0 roger     (1001) roger     (1001)    35476 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/CASEFONT.TTF
+-rwxr-xr-x   0 roger     (1001) roger     (1001)    41360 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/LUCEFONT.TTF
+-rwxr-xr-x   0 roger     (1001) roger     (1001)    49504 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/MERIFONT.TTF
+-rwxr-xr-x   0 roger     (1001) roger     (1001)    39732 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/MOTIFONT.TTF
+-rw-r--r--   0 roger     (1001) roger     (1001)    27052 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/cases.zip
+-rw-r--r--   0 roger     (1001) roger     (1001)    29402 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/lucen.zip
+-rw-r--r--   0 roger     (1001) roger     (1001)    27687 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/merid.zip
+-rw-r--r--   0 roger     (1001) roger     (1001)    22959 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/fonts/motif.zip
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.435983 chesstab-7.0.2/chesstab/gnu/
+-rw-r--r--   0 roger     (1001) roger     (1001)      255 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gnu/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1996 2023-03-07 22:03:12.000000 chesstab-7.0.2/chesstab/gnu/chessgnu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      966 2023-03-07 22:03:31.000000 chesstab-7.0.2/chesstab/gnu/chessgnudu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      923 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gnu/runchessgnudu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.505984 chesstab-7.0.2/chesstab/gui/
+-rw-r--r--   0 roger     (1001) roger     (1001)      612 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      970 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/_lead_trail.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5166 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/_score_scaffold.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    18543 2023-04-26 08:13:05.000000 chesstab-7.0.2/chesstab/gui/analysisscore.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    11656 2023-04-27 08:10:19.000000 chesstab-7.0.2/chesstab/gui/blanktext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     9154 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/board.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    78979 2023-04-27 08:19:39.000000 chesstab-7.0.2/chesstab/gui/chess.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    82152 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/chess_ui.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    32188 2023-03-07 22:04:03.000000 chesstab-7.0.2/chesstab/gui/chessdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    28692 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/colourscheme.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     9831 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/constants.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5572 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cql.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5078 2023-03-07 22:05:00.000000 chesstab-7.0.2/chesstab/gui/cqldbdelete.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     7093 2023-03-07 22:05:20.000000 chesstab-7.0.2/chesstab/gui/cqldbedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2566 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqldbshow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    29778 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqldisplay.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      886 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqledit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    18529 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqlgrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3770 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqlrow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6847 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqltext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      880 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/cqltoplevel.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     8195 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/display.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    12181 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/displayitems.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    21302 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/displaypgn.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    13516 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/displaytext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3863 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/engine.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2924 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginedbdelete.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5146 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginedbedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2904 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginedbshow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2393 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/engineedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     9848 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginegrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3786 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginerow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6312 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginetext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      837 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/enginetoplevel.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4161 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/eventbinding.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    24236 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/eventspec.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4049 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/fonts.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    29759 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/game.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4063 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamedbdelete.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5439 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamedbedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3532 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamedbshow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    11808 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamedisplay.py
+-rw-r--r--   0 roger     (1001) roger     (1001)   192420 2023-04-27 10:05:39.000000 chesstab-7.0.2/chesstab/gui/gameedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    33489 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamegrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    10598 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamelistgrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     7885 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gamerow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1087 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/gametoplevel.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1026 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/help_.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4915 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/options.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5184 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/positionrow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    20216 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/positionscore.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5275 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/query.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2808 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querydbdelete.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4989 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querydbedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2717 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querydbshow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    27356 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querydisplay.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      834 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/queryedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    19038 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querygrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3775 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/queryrow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5532 2023-03-07 22:05:45.000000 chesstab-7.0.2/chesstab/gui/querytext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      815 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/querytoplevel.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2613 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoire.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3361 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiredbdelete.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4474 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiredbedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3342 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiredbshow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    11341 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiredisplay.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2770 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoireedit.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    27910 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiregrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5278 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoirerow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1147 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/repertoiretoplevel.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    96417 2023-04-26 08:23:32.000000 chesstab-7.0.2/chesstab/gui/score.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3276 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/scorepgn.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6459 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/sharedtext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5076 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/gui/toplevelpgn.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     4863 2023-01-15 18:13:59.000000 chesstab-7.0.2/chesstab/gui/topleveltext.py
+-rw-r--r--   0 roger     (1001) roger     (1001)    30729 2023-01-12 19:08:19.000000 chesstab-7.0.2/chesstab/gui/uci.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.505984 chesstab-7.0.2/chesstab/help_/
+-rw-r--r--   0 roger     (1001) roger     (1001)     1234 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1123 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/aboutchesstab.rst
+-rw-r--r--   0 roger     (1001) roger     (1001)     1780 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/chesstab.rst
+-rw-r--r--   0 roger     (1001) roger     (1001)     3444 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/filesize.rst
+-rw-r--r--   0 roger     (1001) roger     (1001)    11921 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/guide.rst
+-rw-r--r--   0 roger     (1001) roger     (1001)     3716 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/help_/selection.rst
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.505984 chesstab-7.0.2/chesstab/lmdb/
+-rw-r--r--   0 roger     (1001) roger     (1001)      383 2023-03-07 22:22:41.000000 chesstab-7.0.2/chesstab/lmdb/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1776 2023-03-07 22:22:41.000000 chesstab-7.0.2/chesstab/lmdb/chesslmdb.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1840 2023-03-07 22:22:41.000000 chesstab-7.0.2/chesstab/lmdb/chesslmdbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      929 2023-03-07 22:22:41.000000 chesstab-7.0.2/chesstab/lmdb/runchesslmdbdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.515983 chesstab-7.0.2/chesstab/ndbm/
+-rw-r--r--   0 roger     (1001) roger     (1001)      252 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/ndbm/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2012 2023-03-07 22:06:28.000000 chesstab-7.0.2/chesstab/ndbm/chessndbm.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      977 2023-03-07 22:07:02.000000 chesstab-7.0.2/chesstab/ndbm/chessndbmdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      927 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/ndbm/runchessndbmdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.535984 chesstab-7.0.2/chesstab/samples/
+-rw-r--r--   0 roger     (1001) roger     (1001)      335 2023-03-07 22:08:01.000000 chesstab-7.0.2/chesstab/samples/apswdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      299 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/apswdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2622 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/chessboard.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3789 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/chessgame.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3765 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/chessscore.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2878 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/chessscoreboard.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      454 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/chesstab.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      323 2023-03-07 22:08:25.000000 chesstab-7.0.2/chesstab/samples/dbdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      287 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/dbdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      359 2023-03-07 22:08:49.000000 chesstab-7.0.2/chesstab/samples/dbtkinterdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      323 2023-01-15 18:16:21.000000 chesstab-7.0.2/chesstab/samples/dbtkinterdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1318 2023-03-07 22:09:30.000000 chesstab-7.0.2/chesstab/samples/directory_widget.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      317 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/dptdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2335 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/dptdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1246 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/dptduchunk.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      919 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/dptdumulti.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1916 2023-03-07 22:09:49.000000 chesstab-7.0.2/chesstab/samples/file_widget.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      333 2023-03-07 22:10:21.000000 chesstab-7.0.2/chesstab/samples/gnudu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      297 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/gnudu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      364 2023-03-07 22:21:44.000000 chesstab-7.0.2/chesstab/samples/lmdbdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      328 2023-03-07 22:22:03.000000 chesstab-7.0.2/chesstab/samples/lmdbdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      762 2023-03-07 22:10:51.000000 chesstab-7.0.2/chesstab/samples/ndbmdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      303 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/ndbmdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      321 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/read_pgn.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1100 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/read_pgn_profile.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      351 2023-03-07 22:11:18.000000 chesstab-7.0.2/chesstab/samples/sqlite3du_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      315 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/sqlite3du_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      353 2023-03-07 22:11:39.000000 chesstab-7.0.2/chesstab/samples/unqlitedu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      317 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/unqlitedu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2365 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/update_players_sqlite3.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      341 2023-03-07 22:12:23.000000 chesstab-7.0.2/chesstab/samples/vedisdu_dir.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      305 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/vedisdu_file.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1484 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/view_players_bsddb3.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2960 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/samples/view_raw_records_bsddb3.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.545982 chesstab-7.0.2/chesstab/shared/
+-rw-r--r--   0 roger     (1001) roger     (1001)      159 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3844 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/alldu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6258 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/allgrid.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1175 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/allrow.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2472 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/archivedu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     5590 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/cql_gamelist_query.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     6954 2023-03-07 22:13:09.000000 chesstab-7.0.2/chesstab/shared/dbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      420 2023-01-15 18:10:38.000000 chesstab-7.0.2/chesstab/shared/dbdudb.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      692 2023-01-15 18:11:01.000000 chesstab-7.0.2/chesstab/shared/dbdutcl.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1291 2023-01-15 18:09:50.000000 chesstab-7.0.2/chesstab/shared/dptcompatdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1446 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/game_position.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2579 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/litedu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3014 2023-03-07 22:13:41.000000 chesstab-7.0.2/chesstab/shared/lmdbdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      410 2023-03-07 22:13:58.000000 chesstab-7.0.2/chesstab/shared/lmdbdudb.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3093 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/shared/rundu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.555983 chesstab-7.0.2/chesstab/sqlite/
+-rw-r--r--   0 roger     (1001) roger     (1001)      360 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/sqlite/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2186 2023-03-07 22:15:13.000000 chesstab-7.0.2/chesstab/sqlite/chesssqlite3.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1002 2023-03-07 22:15:34.000000 chesstab-7.0.2/chesstab/sqlite/chesssqlite3du.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1193 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/sqlite/runchesssqlite3du.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.555983 chesstab-7.0.2/chesstab/tools/
+-rw-r--r--   0 roger     (1001) roger     (1001)      796 2023-03-07 15:46:28.000000 chesstab-7.0.2/chesstab/tools/berkeleydb_du_splice_fix.py
+-rw-r--r--   0 roger     (1001) roger     (1001)   182081 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/tools/chesstab-4-1-1_castling-option-correction.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     3720 2023-03-07 22:18:35.000000 chesstab-7.0.2/chesstab/tools/create_chesstab_database.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      427 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/tools/upgrade_3_to_4.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.555983 chesstab-7.0.2/chesstab/unqlite/
+-rw-r--r--   0 roger     (1001) roger     (1001)      242 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/unqlite/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2016 2023-03-07 22:16:29.000000 chesstab-7.0.2/chesstab/unqlite/chessunqlite.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     1002 2023-03-07 22:17:00.000000 chesstab-7.0.2/chesstab/unqlite/chessunqlitedu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      935 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/unqlite/runchessunqlitedu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.555983 chesstab-7.0.2/chesstab/vedis/
+-rw-r--r--   0 roger     (1001) roger     (1001)      238 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/vedis/__init__.py
+-rw-r--r--   0 roger     (1001) roger     (1001)     2000 2023-03-07 22:17:31.000000 chesstab-7.0.2/chesstab/vedis/chessvedis.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      980 2023-03-07 22:20:50.000000 chesstab-7.0.2/chesstab/vedis/chessvedisdu.py
+-rw-r--r--   0 roger     (1001) roger     (1001)      927 2023-01-10 17:52:02.000000 chesstab-7.0.2/chesstab/vedis/runchessvedisdu.py
+drwxr-xr-x   0 roger     (1001) roger     (1001)        0 2023-04-27 10:14:25.385984 chesstab-7.0.2/chesstab.egg-info/
+-rw-r--r--   0 roger     (1001) roger     (1001)     6221 2023-04-27 10:14:25.000000 chesstab-7.0.2/chesstab.egg-info/PKG-INFO
+-rw-r--r--   0 roger     (1001) roger     (1001)     6831 2023-04-27 10:14:25.000000 chesstab-7.0.2/chesstab.egg-info/SOURCES.txt
+-rw-r--r--   0 roger     (1001) roger     (1001)      325 2023-04-27 10:14:25.000000 chesstab-7.0.2/chesstab.egg-info/dependency_links.txt
+-rw-r--r--   0 roger     (1001) roger     (1001)      109 2023-04-27 10:14:25.000000 chesstab-7.0.2/chesstab.egg-info/requires.txt
+-rw-r--r--   0 roger     (1001) roger     (1001)        9 2023-04-27 10:14:25.000000 chesstab-7.0.2/chesstab.egg-info/top_level.txt
+-rw-r--r--   0 roger     (1001) roger     (1001)      135 2023-01-10 17:52:02.000000 chesstab-7.0.2/pyproject.toml
+-rw-r--r--   0 roger     (1001) roger     (1001)     1296 2023-04-27 10:14:25.565983 chesstab-7.0.2/setup.cfg
+-rw-r--r--   0 roger     (1001) roger     (1001)     1338 2023-01-10 17:52:02.000000 chesstab-7.0.2/setup.py
```

### Comparing `chesstab-7.0.1/LICENCE` & `chesstab-7.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/PKG-INFO` & `chesstab-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesstab
-Version: 7.0.1
+Version: 7.0.2
 Summary: Database for chess games
 Home-page: http://www.solentware.co.uk
 Author: Roger Marsh
 Author-email: roger.marsh@solentware.co.uk
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `chesstab-7.0.1/README` & `chesstab-7.0.2/README`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/__init__.py` & `chesstab-7.0.2/chesstab/__init__.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/apsw/chessapsw.py` & `chesstab-7.0.2/chesstab/apsw/chessapsw.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/apsw/chessapswdu.py` & `chesstab-7.0.2/chesstab/apsw/chessapswdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/apsw/runchessapswdu.py` & `chesstab-7.0.2/chesstab/apsw/runchessapswdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/analysis_index.py` & `chesstab-7.0.2/chesstab/basecore/analysis_index.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/analysisds.py` & `chesstab-7.0.2/chesstab/basecore/analysisds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/cqlds.py` & `chesstab-7.0.2/chesstab/basecore/cqlds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/cqlgames.py` & `chesstab-7.0.2/chesstab/basecore/cqlgames.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/database.py` & `chesstab-7.0.2/chesstab/basecore/database.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/fullposition.py` & `chesstab-7.0.2/chesstab/basecore/fullposition.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/fullpositionds.py` & `chesstab-7.0.2/chesstab/basecore/fullpositionds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/rayfilter.py` & `chesstab-7.0.2/chesstab/basecore/rayfilter.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/selection.py` & `chesstab-7.0.2/chesstab/basecore/selection.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/basecore/selectionds.py` & `chesstab-7.0.2/chesstab/basecore/selectionds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/berkeleydb/chessberkeleydb.py` & `chesstab-7.0.2/chesstab/berkeleydb/chessberkeleydb.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/berkeleydb/chessberkeleydbdu.py` & `chesstab-7.0.2/chesstab/berkeleydb/chessberkeleydbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/berkeleydb/runchessberkeleydbdu.py` & `chesstab-7.0.2/chesstab/berkeleydb/runchessberkeleydbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/chessgames.py` & `chesstab-7.0.2/chesstab/chessgames.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/chessgames_winedptchunk.py` & `chesstab-7.0.2/chesstab/chessgames_winedptchunk.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/chessgames_winedptmulti.py` & `chesstab-7.0.2/chesstab/chessgames_winedptmulti.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/analysis.py` & `chesstab-7.0.2/chesstab/core/analysis.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/chessrecord.py` & `chesstab-7.0.2/chesstab/core/chessrecord.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/constants.py` & `chesstab-7.0.2/chesstab/core/constants.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/cqlnode.py` & `chesstab-7.0.2/chesstab/core/cqlnode.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/cqlstatement.py` & `chesstab-7.0.2/chesstab/core/cqlstatement.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/engine.py` & `chesstab-7.0.2/chesstab/core/engine.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/export_chessql.py` & `chesstab-7.0.2/chesstab/core/export_chessql.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/export_game.py` & `chesstab-7.0.2/chesstab/core/export_game.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/export_pgn_import_format.py` & `chesstab-7.0.2/chesstab/core/export_pgn_import_format.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/export_repertoire.py` & `chesstab-7.0.2/chesstab/core/export_repertoire.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/export_selection_rule.py` & `chesstab-7.0.2/chesstab/core/export_selection_rule.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/filespec.py` & `chesstab-7.0.2/chesstab/core/filespec.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/pgn.py` & `chesstab-7.0.2/chesstab/core/pgn.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/querystatement.py` & `chesstab-7.0.2/chesstab/core/querystatement.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/uci.py` & `chesstab-7.0.2/chesstab/core/uci.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/core/uci_to_pgn.py` & `chesstab-7.0.2/chesstab/core/uci_to_pgn.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db/chessdb.py` & `chesstab-7.0.2/chesstab/db/chessdb.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db/chessdbdu.py` & `chesstab-7.0.2/chesstab/db/chessdbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db/runchessdbdu.py` & `chesstab-7.0.2/chesstab/db/runchessdbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db_tkinter/chessdbtkinter.py` & `chesstab-7.0.2/chesstab/db_tkinter/chessdbtkinter.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db_tkinter/chessdbtkinterdu.py` & `chesstab-7.0.2/chesstab/db_tkinter/chessdbtkinterdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/db_tkinter/runchessdbtkinterdu.py` & `chesstab-7.0.2/chesstab/db_tkinter/runchessdbtkinterdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/__init__.py` & `chesstab-7.0.2/chesstab/dpt/__init__.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/analysisds.py` & `chesstab-7.0.2/chesstab/dpt/analysisds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/chessdpt.py` & `chesstab-7.0.2/chesstab/dpt/chessdpt.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/chessdptdu.py` & `chesstab-7.0.2/chesstab/dpt/chessdptdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/cqlds.py` & `chesstab-7.0.2/chesstab/dpt/cqlds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/fullpositionds.py` & `chesstab-7.0.2/chesstab/dpt/fullpositionds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/runchessdptdu.py` & `chesstab-7.0.2/chesstab/dpt/runchessdptdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/runchessdptduchunk.py` & `chesstab-7.0.2/chesstab/dpt/runchessdptduchunk.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/dpt/selectionds.py` & `chesstab-7.0.2/chesstab/dpt/selectionds.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/CASEFONT.TTF` & `chesstab-7.0.2/chesstab/fonts/CASEFONT.TTF`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/LUCEFONT.TTF` & `chesstab-7.0.2/chesstab/fonts/LUCEFONT.TTF`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/MERIFONT.TTF` & `chesstab-7.0.2/chesstab/fonts/MERIFONT.TTF`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/MOTIFONT.TTF` & `chesstab-7.0.2/chesstab/fonts/MOTIFONT.TTF`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/cases.zip` & `chesstab-7.0.2/chesstab/fonts/cases.zip`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/lucen.zip` & `chesstab-7.0.2/chesstab/fonts/lucen.zip`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/merid.zip` & `chesstab-7.0.2/chesstab/fonts/merid.zip`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/fonts/motif.zip` & `chesstab-7.0.2/chesstab/fonts/motif.zip`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gnu/chessgnu.py` & `chesstab-7.0.2/chesstab/gnu/chessgnu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gnu/chessgnudu.py` & `chesstab-7.0.2/chesstab/gnu/chessgnudu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gnu/runchessgnudu.py` & `chesstab-7.0.2/chesstab/gnu/runchessgnudu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/__init__.py` & `chesstab-7.0.2/chesstab/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/_lead_trail.py` & `chesstab-7.0.2/chesstab/gui/_lead_trail.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/_score_scaffold.py` & `chesstab-7.0.2/chesstab/gui/_score_scaffold.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/analysisscore.py` & `chesstab-7.0.2/chesstab/gui/analysisscore.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/blanktext.py` & `chesstab-7.0.2/chesstab/gui/blanktext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/board.py` & `chesstab-7.0.2/chesstab/gui/board.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/chess.py` & `chesstab-7.0.2/chesstab/gui/chess.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/chess_ui.py` & `chesstab-7.0.2/chesstab/gui/chess_ui.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/chessdu.py` & `chesstab-7.0.2/chesstab/gui/chessdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/colourscheme.py` & `chesstab-7.0.2/chesstab/gui/colourscheme.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/constants.py` & `chesstab-7.0.2/chesstab/gui/constants.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cql.py` & `chesstab-7.0.2/chesstab/gui/cql.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqldbdelete.py` & `chesstab-7.0.2/chesstab/gui/cqldbdelete.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqldbedit.py` & `chesstab-7.0.2/chesstab/gui/cqldbedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqldbshow.py` & `chesstab-7.0.2/chesstab/gui/cqldbshow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqldisplay.py` & `chesstab-7.0.2/chesstab/gui/cqldisplay.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqledit.py` & `chesstab-7.0.2/chesstab/gui/cqledit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqlgrid.py` & `chesstab-7.0.2/chesstab/gui/cqlgrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqlrow.py` & `chesstab-7.0.2/chesstab/gui/cqlrow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqltext.py` & `chesstab-7.0.2/chesstab/gui/cqltext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/cqltoplevel.py` & `chesstab-7.0.2/chesstab/gui/cqltoplevel.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/display.py` & `chesstab-7.0.2/chesstab/gui/display.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/displayitems.py` & `chesstab-7.0.2/chesstab/gui/displayitems.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/displaypgn.py` & `chesstab-7.0.2/chesstab/gui/displaypgn.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/displaytext.py` & `chesstab-7.0.2/chesstab/gui/displaytext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/engine.py` & `chesstab-7.0.2/chesstab/gui/engine.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginedbdelete.py` & `chesstab-7.0.2/chesstab/gui/enginedbdelete.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginedbedit.py` & `chesstab-7.0.2/chesstab/gui/enginedbedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginedbshow.py` & `chesstab-7.0.2/chesstab/gui/enginedbshow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/engineedit.py` & `chesstab-7.0.2/chesstab/gui/engineedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginegrid.py` & `chesstab-7.0.2/chesstab/gui/enginegrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginerow.py` & `chesstab-7.0.2/chesstab/gui/enginerow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginetext.py` & `chesstab-7.0.2/chesstab/gui/enginetext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/enginetoplevel.py` & `chesstab-7.0.2/chesstab/gui/enginetoplevel.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/eventbinding.py` & `chesstab-7.0.2/chesstab/gui/eventbinding.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/eventspec.py` & `chesstab-7.0.2/chesstab/gui/eventspec.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/fonts.py` & `chesstab-7.0.2/chesstab/gui/fonts.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/game.py` & `chesstab-7.0.2/chesstab/gui/game.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamedbdelete.py` & `chesstab-7.0.2/chesstab/gui/gamedbdelete.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamedbedit.py` & `chesstab-7.0.2/chesstab/gui/gamedbedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamedbshow.py` & `chesstab-7.0.2/chesstab/gui/gamedbshow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamedisplay.py` & `chesstab-7.0.2/chesstab/gui/gamedisplay.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gameedit.py` & `chesstab-7.0.2/chesstab/gui/gameedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,16 +327,28 @@
 
         # Define popup menu for '\n%...\n' escape whole line tokens.
         self.escape_whole_line_popup = None
 
         # Define popup menu for '<...>' reserved tokens.
         self.reserved_popup = None
 
+        # Prevent drag relocation of insertion cursor, including scrolling
+        # after pointer leaves widget at top or bottom.  This avoids some
+        # exceptions when inserting or editing moves.
+        # Prevent drag stroking out a selection with consequential visible
+        # effect on Windows.
+        self.score.bind("<Button1-Motion>", self._suppress_class_binding)
+        self.score.bind("<Button1-Leave>", self._suppress_class_binding)
+
     # These methods define event bindings.
 
+    def _suppress_class_binding(self, event):
+        """Return 'break'"""
+        return "break"
+
     def _set_primary_activity_bindings(self, switch=True):
         """Delegate then set bindings for primary activity.
 
         The primary activity is inserting moves and traversing all tokens.
 
         Moves, including RAVs can only be inserted if the game termination
         marker is present.
@@ -429,14 +441,23 @@
         )
         if include_ooo:
             function = self._insert_castle_queenside_command  # Line count.
             self.set_event_bindings_score(
                 ((EventSpec.gameedit_insert_castle_queenside, function),),
                 switch=switch,
             )
+
+        # "<Control-o>" may insert a newline at the wrong place, breaking
+        # things if typing newline is inhibited.
+        if not include_ooo or not switch:
+            self.score.bind(
+                EventSpec.gameedit_insert_castle_queenside[0],
+                self._suppress_class_binding
+            )
+
         self.set_event_bindings_score(
             self._get_button_events(
                 buttonpress1=self._go_to_token, buttonpress3=popup_pointer
             ),
             switch=switch,
         )
         self.set_event_bindings_score(
```

### Comparing `chesstab-7.0.1/chesstab/gui/gamegrid.py` & `chesstab-7.0.2/chesstab/gui/gamegrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamelistgrid.py` & `chesstab-7.0.2/chesstab/gui/gamelistgrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gamerow.py` & `chesstab-7.0.2/chesstab/gui/gamerow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/gametoplevel.py` & `chesstab-7.0.2/chesstab/gui/gametoplevel.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/help_.py` & `chesstab-7.0.2/chesstab/gui/help_.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/options.py` & `chesstab-7.0.2/chesstab/gui/options.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/positionrow.py` & `chesstab-7.0.2/chesstab/gui/positionrow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/positionscore.py` & `chesstab-7.0.2/chesstab/gui/positionscore.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/query.py` & `chesstab-7.0.2/chesstab/gui/query.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querydbdelete.py` & `chesstab-7.0.2/chesstab/gui/querydbdelete.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querydbedit.py` & `chesstab-7.0.2/chesstab/gui/querydbedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querydbshow.py` & `chesstab-7.0.2/chesstab/gui/querydbshow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querydisplay.py` & `chesstab-7.0.2/chesstab/gui/querydisplay.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/queryedit.py` & `chesstab-7.0.2/chesstab/gui/queryedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querygrid.py` & `chesstab-7.0.2/chesstab/gui/querygrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/queryrow.py` & `chesstab-7.0.2/chesstab/gui/queryrow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querytext.py` & `chesstab-7.0.2/chesstab/gui/querytext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/querytoplevel.py` & `chesstab-7.0.2/chesstab/gui/querytoplevel.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoire.py` & `chesstab-7.0.2/chesstab/gui/repertoire.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiredbdelete.py` & `chesstab-7.0.2/chesstab/gui/repertoiredbdelete.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiredbedit.py` & `chesstab-7.0.2/chesstab/gui/repertoiredbedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiredbshow.py` & `chesstab-7.0.2/chesstab/gui/repertoiredbshow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiredisplay.py` & `chesstab-7.0.2/chesstab/gui/repertoiredisplay.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoireedit.py` & `chesstab-7.0.2/chesstab/gui/repertoireedit.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiregrid.py` & `chesstab-7.0.2/chesstab/gui/repertoiregrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoirerow.py` & `chesstab-7.0.2/chesstab/gui/repertoirerow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/repertoiretoplevel.py` & `chesstab-7.0.2/chesstab/gui/repertoiretoplevel.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/score.py` & `chesstab-7.0.2/chesstab/gui/score.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/scorepgn.py` & `chesstab-7.0.2/chesstab/gui/scorepgn.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/sharedtext.py` & `chesstab-7.0.2/chesstab/gui/sharedtext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/toplevelpgn.py` & `chesstab-7.0.2/chesstab/gui/toplevelpgn.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/topleveltext.py` & `chesstab-7.0.2/chesstab/gui/topleveltext.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/gui/uci.py` & `chesstab-7.0.2/chesstab/gui/uci.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/__init__.py` & `chesstab-7.0.2/chesstab/help_/__init__.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/aboutchesstab.rst` & `chesstab-7.0.2/chesstab/help_/aboutchesstab.rst`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/chesstab.rst` & `chesstab-7.0.2/chesstab/help_/chesstab.rst`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/filesize.rst` & `chesstab-7.0.2/chesstab/help_/filesize.rst`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/guide.rst` & `chesstab-7.0.2/chesstab/help_/guide.rst`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/help_/selection.rst` & `chesstab-7.0.2/chesstab/help_/selection.rst`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/lmdb/chesslmdb.py` & `chesstab-7.0.2/chesstab/lmdb/chesslmdb.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/lmdb/chesslmdbdu.py` & `chesstab-7.0.2/chesstab/lmdb/chesslmdbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/lmdb/runchesslmdbdu.py` & `chesstab-7.0.2/chesstab/lmdb/runchesslmdbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/ndbm/chessndbm.py` & `chesstab-7.0.2/chesstab/ndbm/chessndbm.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/ndbm/chessndbmdu.py` & `chesstab-7.0.2/chesstab/ndbm/chessndbmdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/ndbm/runchessndbmdu.py` & `chesstab-7.0.2/chesstab/ndbm/runchessndbmdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/chessboard.py` & `chesstab-7.0.2/chesstab/samples/chessboard.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/chessgame.py` & `chesstab-7.0.2/chesstab/samples/chessgame.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/chessscore.py` & `chesstab-7.0.2/chesstab/samples/chessscore.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/chessscoreboard.py` & `chesstab-7.0.2/chesstab/samples/chessscoreboard.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/directory_widget.py` & `chesstab-7.0.2/chesstab/samples/directory_widget.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/dptdu_file.py` & `chesstab-7.0.2/chesstab/samples/dptdu_file.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/dptduchunk.py` & `chesstab-7.0.2/chesstab/samples/dptduchunk.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/dptdumulti.py` & `chesstab-7.0.2/chesstab/samples/dptdumulti.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/file_widget.py` & `chesstab-7.0.2/chesstab/samples/file_widget.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/ndbmdu_dir.py` & `chesstab-7.0.2/chesstab/samples/ndbmdu_dir.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/read_pgn_profile.py` & `chesstab-7.0.2/chesstab/samples/read_pgn_profile.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/update_players_sqlite3.py` & `chesstab-7.0.2/chesstab/samples/update_players_sqlite3.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/view_players_bsddb3.py` & `chesstab-7.0.2/chesstab/samples/view_players_bsddb3.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/samples/view_raw_records_bsddb3.py` & `chesstab-7.0.2/chesstab/samples/view_raw_records_bsddb3.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/alldu.py` & `chesstab-7.0.2/chesstab/shared/alldu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/allgrid.py` & `chesstab-7.0.2/chesstab/shared/allgrid.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/allrow.py` & `chesstab-7.0.2/chesstab/shared/allrow.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/archivedu.py` & `chesstab-7.0.2/chesstab/shared/archivedu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/cql_gamelist_query.py` & `chesstab-7.0.2/chesstab/shared/cql_gamelist_query.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/dbdu.py` & `chesstab-7.0.2/chesstab/shared/dbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/dbdutcl.py` & `chesstab-7.0.2/chesstab/shared/dbdutcl.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/dptcompatdu.py` & `chesstab-7.0.2/chesstab/shared/dptcompatdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/game_position.py` & `chesstab-7.0.2/chesstab/shared/game_position.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/litedu.py` & `chesstab-7.0.2/chesstab/shared/litedu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/lmdbdu.py` & `chesstab-7.0.2/chesstab/shared/lmdbdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/shared/rundu.py` & `chesstab-7.0.2/chesstab/shared/rundu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/sqlite/chesssqlite3.py` & `chesstab-7.0.2/chesstab/sqlite/chesssqlite3.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/sqlite/chesssqlite3du.py` & `chesstab-7.0.2/chesstab/sqlite/chesssqlite3du.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/sqlite/runchesssqlite3du.py` & `chesstab-7.0.2/chesstab/sqlite/runchesssqlite3du.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/tools/berkeleydb_du_splice_fix.py` & `chesstab-7.0.2/chesstab/tools/berkeleydb_du_splice_fix.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/tools/chesstab-4-1-1_castling-option-correction.py` & `chesstab-7.0.2/chesstab/tools/chesstab-4-1-1_castling-option-correction.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/tools/create_chesstab_database.py` & `chesstab-7.0.2/chesstab/tools/create_chesstab_database.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/unqlite/chessunqlite.py` & `chesstab-7.0.2/chesstab/unqlite/chessunqlite.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/unqlite/chessunqlitedu.py` & `chesstab-7.0.2/chesstab/unqlite/chessunqlitedu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/unqlite/runchessunqlitedu.py` & `chesstab-7.0.2/chesstab/unqlite/runchessunqlitedu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/vedis/chessvedis.py` & `chesstab-7.0.2/chesstab/vedis/chessvedis.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/vedis/chessvedisdu.py` & `chesstab-7.0.2/chesstab/vedis/chessvedisdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab/vedis/runchessvedisdu.py` & `chesstab-7.0.2/chesstab/vedis/runchessvedisdu.py`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/chesstab.egg-info/PKG-INFO` & `chesstab-7.0.2/chesstab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesstab
-Version: 7.0.1
+Version: 7.0.2
 Summary: Database for chess games
 Home-page: http://www.solentware.co.uk
 Author: Roger Marsh
 Author-email: roger.marsh@solentware.co.uk
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `chesstab-7.0.1/chesstab.egg-info/SOURCES.txt` & `chesstab-7.0.2/chesstab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chesstab-7.0.1/setup.cfg` & `chesstab-7.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chesstab
-version = 7.0.1
+version = 7.0.2
 description = Database for chess games
 author = Roger Marsh
 author_email = roger.marsh@solentware.co.uk
 url = http://www.solentware.co.uk
 long_description = file: README
 license = BSD
 classifiers =
```

### Comparing `chesstab-7.0.1/setup.py` & `chesstab-7.0.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/starkinfra-0.6.0.tar.gz` & `tmp/starkinfra-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkinfra-0.6.0.tar", last modified: Fri Dec  2 14:22:48 2022, max compression
+gzip compressed data, was "starkinfra-0.7.0.tar", last modified: Thu Apr 27 20:26:45 2023, max compression
```

## Comparing `starkinfra-0.6.0.tar` & `starkinfra-0.7.0.tar`

### file list

```diff
@@ -1,190 +1,199 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.802082 starkinfra-0.6.0/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.6.0/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.6.0/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)    68753 2022-12-02 14:22:48.801790 starkinfra-0.6.0/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)    68335 2022-11-23 18:02:54.000000 starkinfra-0.6.0/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-12-02 14:22:48.802154 starkinfra-0.6.0/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      828 2022-07-08 01:03:22.000000 starkinfra-0.6.0/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.675541 starkinfra-0.6.0/starkinfra/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3200 2022-12-02 14:20:40.000000 starkinfra-0.6.0/starkinfra/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.690894 starkinfra-0.6.0/starkinfra/brcodepreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     4797 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/brcodepreview/__brcodepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/brcodepreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.691878 starkinfra-0.6.0/starkinfra/cardmethod/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1306 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/cardmethod/__cardmethod.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/cardmethod/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.694321 starkinfra-0.6.0/starkinfra/creditnote/
--rw-r--r--   0 caiodottori   (501) staff       (20)    12232 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditnote/__creditnote.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/creditnote/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.6.0/starkinfra/creditnote/__transfer.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.696375 starkinfra-0.6.0/starkinfra/creditnote/invoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.6.0/starkinfra/creditnote/invoice/__description.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.6.0/starkinfra/creditnote/invoice/__discount.py
--rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.6.0/starkinfra/creditnote/invoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5405 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditnote/invoice/__invoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.697129 starkinfra-0.6.0/starkinfra/creditnote/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/creditnote/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5149 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditnote/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.701657 starkinfra-0.6.0/starkinfra/creditpreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3422 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditpreview/__creditnotepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditpreview/__creditpreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/creditpreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.704990 starkinfra-0.6.0/starkinfra/creditsigner/
--rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/creditsigner/__creditsigner.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/creditsigner/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.705895 starkinfra-0.6.0/starkinfra/dynamicbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)    15775 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/dynamicbrcode/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.706722 starkinfra-0.6.0/starkinfra/event/
--rw-r--r--   0 caiodottori   (501) staff       (20)     8832 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/event/__event.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/event/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.707823 starkinfra-0.6.0/starkinfra/event/attempt/
--rw-r--r--   0 caiodottori   (501) staff       (20)     4967 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/event/attempt/__attempt.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/event/attempt/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.708991 starkinfra-0.6.0/starkinfra/individualdocument/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7072 2022-11-11 22:04:07.000000 starkinfra-0.6.0/starkinfra/individualdocument/__individualdocument.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualdocument/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.710552 starkinfra-0.6.0/starkinfra/individualdocument/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualdocument/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5243 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualdocument/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.712469 starkinfra-0.6.0/starkinfra/individualidentity/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7897 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualidentity/__individualidentity.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualidentity/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.713476 starkinfra-0.6.0/starkinfra/individualidentity/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.6.0/starkinfra/individualidentity/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5235 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/individualidentity/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.715448 starkinfra-0.6.0/starkinfra/issuingbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingbalance/__issuingbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.718498 starkinfra-0.6.0/starkinfra/issuingcard/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/issuingcard/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    11181 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingcard/__issuingcard.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.719830 starkinfra-0.6.0/starkinfra/issuingcard/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingcard/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5246 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingcard/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.720946 starkinfra-0.6.0/starkinfra/issuingdesign/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingdesign/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4382 2022-12-02 14:18:37.000000 starkinfra-0.6.0/starkinfra/issuingdesign/__issuingdesign.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.722391 starkinfra-0.6.0/starkinfra/issuingembossingrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingembossingrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8942 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.723404 starkinfra-0.6.0/starkinfra/issuingembossingrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingembossingrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5987 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingembossingrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.729348 starkinfra-0.6.0/starkinfra/issuingholder/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/issuingholder/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8089 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingholder/__issuingholder.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.730450 starkinfra-0.6.0/starkinfra/issuingholder/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingholder/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5211 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingholder/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.731194 starkinfra-0.6.0/starkinfra/issuinginvoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/issuinginvoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6639 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuinginvoice/__issuinginvoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.732841 starkinfra-0.6.0/starkinfra/issuinginvoice/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/issuinginvoice/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4925 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuinginvoice/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.735972 starkinfra-0.6.0/starkinfra/issuingproduct/
--rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/issuingproduct/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingproduct/__issuingproduct.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.737220 starkinfra-0.6.0/starkinfra/issuingpurchase/
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/issuingpurchase/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13004 2022-12-02 14:18:37.000000 starkinfra-0.6.0/starkinfra/issuingpurchase/__issuingpurchase.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.738232 starkinfra-0.6.0/starkinfra/issuingpurchase/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingpurchase/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5972 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingpurchase/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.739236 starkinfra-0.6.0/starkinfra/issuingrestock/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingrestock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingrestock/__issuingrestock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.739998 starkinfra-0.6.0/starkinfra/issuingrestock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingrestock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5228 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingrestock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.740661 starkinfra-0.6.0/starkinfra/issuingrule/
--rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/issuingrule/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3940 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingrule/__issuingrule.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.742820 starkinfra-0.6.0/starkinfra/issuingstock/
--rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingstock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5617 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingstock/__issuingstock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.744457 starkinfra-0.6.0/starkinfra/issuingstock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingstock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5256 2022-11-23 18:02:54.000000 starkinfra-0.6.0/starkinfra/issuingstock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.745495 starkinfra-0.6.0/starkinfra/issuingtransaction/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingtransaction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5409 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingtransaction/__issuingtransaction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.750030 starkinfra-0.6.0/starkinfra/issuingwithdrawal/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/issuingwithdrawal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6027 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.752582 starkinfra-0.6.0/starkinfra/merchantcategory/
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/merchantcategory/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/merchantcategory/__merchantcategory.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.753846 starkinfra-0.6.0/starkinfra/merchantcountry/
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/merchantcountry/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/merchantcountry/__merchantcountry.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.755766 starkinfra-0.6.0/starkinfra/pixbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/pixbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1632 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixbalance/__pixbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.757014 starkinfra-0.6.0/starkinfra/pixchargeback/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixchargeback/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9879 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixchargeback/__pixchargeback.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.764005 starkinfra-0.6.0/starkinfra/pixchargeback/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixchargeback/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5356 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixchargeback/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.766863 starkinfra-0.6.0/starkinfra/pixclaim/
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/pixclaim/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10002 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixclaim/__pixclaim.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.768737 starkinfra-0.6.0/starkinfra/pixclaim/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/pixclaim/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5504 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixclaim/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.769750 starkinfra-0.6.0/starkinfra/pixdirector/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/pixdirector/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2259 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixdirector/__pixdirector.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.772546 starkinfra-0.6.0/starkinfra/pixdomain/
--rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixdomain/__certificate.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixdomain/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixdomain/__pixdomain.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.776695 starkinfra-0.6.0/starkinfra/pixinfraction/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixinfraction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9579 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixinfraction/__pixinfraction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.778451 starkinfra-0.6.0/starkinfra/pixinfraction/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixinfraction/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5354 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixinfraction/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.780760 starkinfra-0.6.0/starkinfra/pixkey/
--rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/pixkey/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10081 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixkey/__pixkey.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.782537 starkinfra-0.6.0/starkinfra/pixkey/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/pixkey/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5093 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixkey/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.783431 starkinfra-0.6.0/starkinfra/pixrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/pixrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13817 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixrequest/__pixrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.784883 starkinfra-0.6.0/starkinfra/pixrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/pixrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5506 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.785935 starkinfra-0.6.0/starkinfra/pixreversal/
--rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/pixreversal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10403 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixreversal/__pixreversal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.786802 starkinfra-0.6.0/starkinfra/pixreversal/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/pixreversal/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5124 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixreversal/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.789398 starkinfra-0.6.0/starkinfra/pixstatement/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/pixstatement/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5771 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/pixstatement/__pixstatement.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.790577 starkinfra-0.6.0/starkinfra/staticbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/staticbrcode/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6626 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/staticbrcode/__staticbrcode.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.799807 starkinfra-0.6.0/starkinfra/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/utils/bacenid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/utils/endtoendid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.6.0/starkinfra/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/utils/relay.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.6.0/starkinfra/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.6.0/starkinfra/utils/returnid.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.801004 starkinfra-0.6.0/starkinfra/webhook/
--rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.6.0/starkinfra/webhook/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4720 2022-08-26 19:22:07.000000 starkinfra-0.6.0/starkinfra/webhook/__webhook.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-12-02 14:22:48.688968 starkinfra-0.6.0/starkinfra.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)    68753 2022-12-02 14:22:48.000000 starkinfra-0.6.0/starkinfra.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)     4941 2022-12-02 14:22:48.000000 starkinfra-0.6.0/starkinfra.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2022-12-02 14:22:48.000000 starkinfra-0.6.0/starkinfra.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2022-12-02 14:22:48.000000 starkinfra-0.6.0/starkinfra.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2022-12-02 14:22:48.000000 starkinfra-0.6.0/starkinfra.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.038408 starkinfra-0.7.0/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.7.0/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.7.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71265 2023-04-27 20:26:45.038200 starkinfra-0.7.0/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)    70847 2023-04-27 20:24:01.000000 starkinfra-0.7.0/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-04-27 20:26:45.038472 starkinfra-0.7.0/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      828 2023-04-27 20:25:01.000000 starkinfra-0.7.0/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.843866 starkinfra-0.7.0/starkinfra/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3392 2023-04-27 20:25:35.000000 starkinfra-0.7.0/starkinfra/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.849030 starkinfra-0.7.0/starkinfra/brcodepreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5010 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/brcodepreview/__brcodepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/brcodepreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.851991 starkinfra-0.7.0/starkinfra/cardmethod/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1297 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/cardmethod/__cardmethod.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/cardmethod/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.854830 starkinfra-0.7.0/starkinfra/creditholmes/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6542 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditholmes/__creditholmes.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       98 2022-12-21 18:15:18.000000 starkinfra-0.7.0/starkinfra/creditholmes/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.859603 starkinfra-0.7.0/starkinfra/creditholmes/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-12-21 18:15:18.000000 starkinfra-0.7.0/starkinfra/creditholmes/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5157 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditholmes/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.864526 starkinfra-0.7.0/starkinfra/creditnote/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    12152 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/__creditnote.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditnote/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/__transfer.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.867993 starkinfra-0.7.0/starkinfra/creditnote/invoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__description.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__discount.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5403 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__invoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.871217 starkinfra-0.7.0/starkinfra/creditnote/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/creditnote/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5163 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.875616 starkinfra-0.7.0/starkinfra/creditpreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3364 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditpreview/__creditnotepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/creditpreview/__creditpreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/creditpreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.878677 starkinfra-0.7.0/starkinfra/creditsigner/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditsigner/__creditsigner.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditsigner/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.882003 starkinfra-0.7.0/starkinfra/dynamicbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    15774 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/dynamicbrcode/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.884835 starkinfra-0.7.0/starkinfra/event/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8846 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/event/__event.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/event/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.887791 starkinfra-0.7.0/starkinfra/event/attempt/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4981 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/event/attempt/__attempt.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/event/attempt/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.890840 starkinfra-0.7.0/starkinfra/individualdocument/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7065 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualdocument/__individualdocument.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualdocument/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.892232 starkinfra-0.7.0/starkinfra/individualdocument/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualdocument/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5257 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualdocument/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.895715 starkinfra-0.7.0/starkinfra/individualidentity/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7874 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualidentity/__individualidentity.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualidentity/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.896889 starkinfra-0.7.0/starkinfra/individualidentity/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualidentity/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5249 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualidentity/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.902204 starkinfra-0.7.0/starkinfra/issuingbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/issuingbalance/__issuingbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.904526 starkinfra-0.7.0/starkinfra/issuingcard/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuingcard/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    11393 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingcard/__issuingcard.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.907710 starkinfra-0.7.0/starkinfra/issuingcard/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingcard/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5260 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingcard/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.910615 starkinfra-0.7.0/starkinfra/issuingdesign/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingdesign/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4754 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingdesign/__issuingdesign.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.911343 starkinfra-0.7.0/starkinfra/issuingembossingkit/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       52 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingkit/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5269 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingkit/__issuingembossingkit.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.914503 starkinfra-0.7.0/starkinfra/issuingembossingrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8738 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.917301 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6001 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.920475 starkinfra-0.7.0/starkinfra/issuingholder/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuingholder/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8239 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingholder/__issuingholder.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.923956 starkinfra-0.7.0/starkinfra/issuingholder/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingholder/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5225 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingholder/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.927588 starkinfra-0.7.0/starkinfra/issuinginvoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6663 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/__issuinginvoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.930260 starkinfra-0.7.0/starkinfra/issuinginvoice/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4939 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.935080 starkinfra-0.7.0/starkinfra/issuingproduct/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingproduct/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/issuingproduct/__issuingproduct.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.936380 starkinfra-0.7.0/starkinfra/issuingpurchase/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13027 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/__issuingpurchase.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.939320 starkinfra-0.7.0/starkinfra/issuingpurchase/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5986 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.943562 starkinfra-0.7.0/starkinfra/issuingrestock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/__issuingrestock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.945689 starkinfra-0.7.0/starkinfra/issuingrestock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5242 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingrestock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.948749 starkinfra-0.7.0/starkinfra/issuingrule/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingrule/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3925 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingrule/__issuingrule.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.951424 starkinfra-0.7.0/starkinfra/issuingstock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingstock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5619 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingstock/__issuingstock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.954105 starkinfra-0.7.0/starkinfra/issuingstock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingstock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5270 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingstock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.957213 starkinfra-0.7.0/starkinfra/issuingtransaction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingtransaction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5402 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingtransaction/__issuingtransaction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.960296 starkinfra-0.7.0/starkinfra/issuingwithdrawal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingwithdrawal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6033 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.966311 starkinfra-0.7.0/starkinfra/merchantcategory/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/merchantcategory/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/merchantcategory/__merchantcategory.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.969455 starkinfra-0.7.0/starkinfra/merchantcountry/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/merchantcountry/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/merchantcountry/__merchantcountry.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.970503 starkinfra-0.7.0/starkinfra/pixbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1635 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixbalance/__pixbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.974118 starkinfra-0.7.0/starkinfra/pixchargeback/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixchargeback/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10153 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixchargeback/__pixchargeback.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.977151 starkinfra-0.7.0/starkinfra/pixchargeback/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixchargeback/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5370 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixchargeback/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.980720 starkinfra-0.7.0/starkinfra/pixclaim/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixclaim/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10003 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixclaim/__pixclaim.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.983140 starkinfra-0.7.0/starkinfra/pixclaim/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixclaim/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5518 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixclaim/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.987767 starkinfra-0.7.0/starkinfra/pixdirector/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixdirector/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2165 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixdirector/__pixdirector.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.992582 starkinfra-0.7.0/starkinfra/pixdomain/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixdomain/__certificate.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixdomain/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/pixdomain/__pixdomain.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.993730 starkinfra-0.7.0/starkinfra/pixinfraction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixinfraction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9589 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixinfraction/__pixinfraction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.996248 starkinfra-0.7.0/starkinfra/pixinfraction/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixinfraction/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5368 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixinfraction/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.999068 starkinfra-0.7.0/starkinfra/pixkey/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixkey/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10238 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixkey/__pixkey.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.002188 starkinfra-0.7.0/starkinfra/pixkey/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixkey/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5107 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixkey/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.005134 starkinfra-0.7.0/starkinfra/pixrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/pixrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13971 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixrequest/__pixrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.008265 starkinfra-0.7.0/starkinfra/pixrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5534 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.012456 starkinfra-0.7.0/starkinfra/pixreversal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/pixreversal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10438 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixreversal/__pixreversal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.015397 starkinfra-0.7.0/starkinfra/pixreversal/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixreversal/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5138 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixreversal/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.018096 starkinfra-0.7.0/starkinfra/pixstatement/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixstatement/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5856 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixstatement/__pixstatement.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.021134 starkinfra-0.7.0/starkinfra/staticbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/staticbrcode/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6859 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/staticbrcode/__staticbrcode.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.035839 starkinfra-0.7.0/starkinfra/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/bacenid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/endtoendid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/utils/relay.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/returnid.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.037825 starkinfra-0.7.0/starkinfra/webhook/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/webhook/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4765 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/webhook/__webhook.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.845649 starkinfra-0.7.0/starkinfra.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71265 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5195 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/top_level.txt
```

### Comparing `starkinfra-0.6.0/LICENSE.txt` & `starkinfra-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/PKG-INFO` & `starkinfra-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkinfra
-Version: 0.6.0
+Version: 0.7.0
 Summary: SDK to facilitate Python integrations with Stark Infra
 Home-page: https://github.com/starkinfra/sdk-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
 Platform: UNKNOWN
@@ -35,14 +35,15 @@
 - [Testing in Sandbox](#testing-in-sandbox) 
 - [Usage](#usage)
     - [Issuing](#issuing)
         - [Products](#query-issuingproducts): View available sub-issuer card products (a.k.a. card number ranges or BINs)
         - [Holders](#create-issuingholders): Manage card holders
         - [Cards](#create-issuingcards): Create virtual and/or physical cards
         - [Design](#query-issuingdesigns): View your current card or package designs
+        - [EmbossingKit](#query-issuingembossingkits): View your current embossing kits
         - [Stock](#query-issuingstocks): View your current stock of a certain IssuingDesign linked to an Embosser on the workspace
         - [Restock](#create-issuingrestocks): Create restock orders of a specific IssuingStock object
         - [EmbossingRequest](#create-issuingembossingrequests): Create embossing requests
         - [Purchases](#process-purchase-authorizations): Authorize and view your past purchases
         - [Invoices](#create-issuinginvoices): Add money to your issuing balance
         - [Withdrawals](#create-issuingwithdrawals): Send money back to your Workspace from your issuing balance
         - [Balance](#get-your-issuingbalance): View your issuing balance
@@ -61,14 +62,15 @@
         - [PixDomain](#query-pixdomains): View registered SPI participants certificates
         - [StaticBrcode](#create-staticbrcodes): Create static Pix BR codes
         - [DynamicBrcode](#create-dynamicbrcodes): Create dynamic Pix BR codes
         - [BrcodePreview](#create-brcodepreviews): Read data from BR Codes before paying them
     - [Lending](#lending)
         - [CreditNote](#create-creditnotes): Create credit notes
         - [CreditPreview](#create-creditpreviews): Create credit previews
+        - [CreditHolmes](#create-creditholmes): Create credit holmes debt verification
     - [Identity](#identity)
         - [IndividualIdentity](#create-individualidentities): Create individual identities
         - [IndividualDocument](#create-individualdocuments): Create individual documents
     - [Webhook](#webhook):
         - [Webhook](#create-a-webhook-subscription): Configure your webhook endpoints and subscriptions
         - [WebhookEvents](#process-webhook-events): Manage Webhook events
         - [WebhookEventAttempts](#query-failed-webhook-event-delivery-attempts-information): Query failed webhook event deliveries
@@ -416,27 +418,27 @@
 holder = starkinfra.issuingholder.cancel("5155165527080960")
 
 print(holder)
 ```
 
 ### Get an IssuingHolder
 
-To get a single Issuing Holder by its id, run:
+To get a specific Issuing Holder by its id, run:
 
 ```python
 import starkinfra
 
 holder = starkinfra.issuingholder.get("5155165527080960")
 
 print(holder)
 ```
 
 ### Query IssuingHolder logs
 
-You can query holder logs to better understand holder life cycles.
+You can query IssuingHolder logs to better understand IssuingHolder life cycles.
 
 ```python
 import starkinfra
 
 logs = starkinfra.issuingholder.log.query(limit=50)
 
 for log in logs:
@@ -570,15 +572,14 @@
 
 ### Query IssuingDesigns
 
 You can get a list of available designs given some filters.
 
 ```python
 import starkinfra
-from datetime import date
 
 designs = starkinfra.issuingdesign.query(
     limit=1
 )
 
 for design in designs:
     print(design)
@@ -592,14 +593,43 @@
 import starkinfra
 
 design = starkinfra.issuingdesign.get("5747368922185728")
 
 print(design)
 ```
 
+### Query IssuingEmbossingKits
+
+You can get a list of existing embossing kits given some filters.
+
+```python
+import starkinfra
+from datetime import date
+
+kits = starkinfra.issuingembossingkit.query(
+    after=date(2022, 11, 1),
+    before=date(2022, 12, 1)
+)
+
+for kit in kits:
+    print(kit)
+```
+
+### Get an IssuingEmbossingKit
+
+After its creation, information on an embossing kit may be retrieved by its id.
+
+```python
+import starkinfra
+
+kit = starkinfra.issuingembossingkit.get("5664445921492992")
+
+print(kit)
+```
+
 ### Query IssuingStocks
 
 You can get a list of available stocks given some filters.
 
 ```python
 import starkinfra
 from datetime import date
@@ -727,16 +757,15 @@
 You can create a request to emboss a physical card.
 
 ```python
 import starkinfra
 
 embossing_requests = starkinfra.issuingembossingrequest.create([
     starkinfra.IssuingEmbossingRequest(
-        card_design_id="5648359658356736", 
-        envelope_design_id="5747368922185728", 
+        kit_id="5648359658356736", 
         card_id="5714424132272128", 
         display_name_1="Antonio Stark", 
         shipping_city="Sao Paulo",
         shipping_country_code="BRA",
         shipping_district="Bela Vista",
         shipping_service="loggi",
         shipping_state_code="SP",
@@ -968,15 +997,15 @@
 
 print(log)
 ```
 
 ### Create IssuingWithdrawals
 
 You can create withdrawals to send cash back from your Issuing balance to your Banking balance
-by using the Withdrawal resource.
+by using the IssuingWithdrawal resource.
 
 ```python
 import starkinfra
 
 withdrawal = starkinfra.issuingwithdrawal.create(
     withdrawal=starkinfra.IssuingWithdrawal(
         amount=10000,
@@ -1987,15 +2016,15 @@
     uuids=["5ddde28043a245c2848b08cf315effa2"]
 )
 
 for brcode in brcodes:
     print(brcode)
 ```
 
-### Get a StaticBrcodes
+### Get a StaticBrcode
 
 After its creation, information on a StaticBrcode may be retrieved by its UUID.
 
 ```python
 import starkinfra
 
 brcode = starkinfra.staticbrcode.get("5ddde28043a245c2848b08cf315effa2")
@@ -2058,15 +2087,15 @@
 brcode = starkinfra.dynamicbrcode.get("ac7caa14e601461dbd6b12bf7e4cc48e")
 
 print(brcode)
 ```
 
 ### Verify a DynamicBrcode read
 
-When a DynamicBrcode is read by your user, a GET request will be made to the your regitered URL to 
+When a DynamicBrcode is read by your user, a GET request will be made to your registered URL to 
 retrieve additional information needed to complete the transaction.
 Use this method to verify the authenticity of a GET request received at your registered endpoint.
 If the provided digital signature does not check out with the StarkInfra public key, a stark.exception.InvalidSignatureException will be raised.
 
 ```python
 import starkinfra
 
@@ -2151,14 +2180,15 @@
         cashier_bank_code=invoice.cashier_bank_code,
         cash_amount=invoice.cash_amount
     )
 )
 ```
 
 ## Create BrcodePreviews
+
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
@@ -2186,14 +2216,15 @@
  3. (Optional) Create a [Credit Simulation](#create-creditpreviews) 
 with the desired installment plan to display information for the credit receiver
  4. Create a [Credit Note](#create-creditnotes)
 with the desired installment plan
 
 
 ### Create CreditNotes
+
 For lending operations, you can create a CreditNote to generate a CCB contract.
 
 Note that you must have recently created an identity check for that same Tax ID before
 being able to create a credit operation for them.
 
 ```python
 import starkinfra
@@ -2290,15 +2321,15 @@
 note = starkinfra.creditnote.cancel("5155165527080960")
 
 print(note)
 ```
   
 ### Query CreditNote logs
 
-You can query credit note logs to better understand credit note life cycles. 
+You can query credit note logs to better understand CreditNote life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
 
 logs = starkinfra.creditnote.log.query(
     limit=50, 
@@ -2319,14 +2350,15 @@
 
 log = starkinfra.creditnote.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create CreditPreviews
+
 You can preview a credit operation before creating them (Currently we only have CreditNote / CCB previews):
 
 ```python
 import starkinfra
 from datetime import date
 
 previews = starkinfra.creditpreview.create([
@@ -2404,26 +2436,119 @@
 
 for preview in previews:
     print(preview)
 ```
 
 **Note**: Instead of using CreditPreview objects, you can also pass each element in dictionary format
 
+### Create CreditHolmes
+
+Before you request a credit operation, you may want to check previous credit operations
+the credit receiver has taken.
+
+For that, open up a CreditHolmes investigation to receive information on all debts and credit
+operations registered for that individual or company inside the Central Bank's SCR.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.create([
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-09"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-08"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-07"
+    )
+])
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Query CreditHolmes
+
+You can query multiple credit holmes according to filters.
+
+```python
+import starkinfra
+from datetime import date
+
+holmes = starkinfra.creditholmes.query(
+    after=date(2022, 6, 1),
+    before=date(2022, 10, 30),
+    status="success"
+)
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Get a CreditHolmes
+
+After its creation, information on a credit holmes may be retrieved by its id.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.get("5657818854064128")
+
+print(holmes)
+```
+
+### Query CreditHolmes logs
+
+You can query credit holmes logs to better understand their life cycles. 
+
+```python
+import starkinfra
+from datetime import date
+
+logs = starkinfra.creditholmes.log.query(
+    limit=50, 
+    ids=["5729405850615808"],
+    after=date(2022, 1, 1),
+    before=date(2022, 1, 20),
+    types=["created"]
+)
+
+for log in logs:
+    print(log)
+```
+
+### Get a CreditHolmes log
+
+You can also get a specific log by its id.
+
+```python
+import starkinfra
+
+log = starkinfra.creditholmes.log.get("5155165527080960")
+
+print(log)
+```
+
 ## Identity
 Several operations, especially credit ones, require that the identity
 of a person or business is validated beforehand.
 
 Identities are validated according to the following sequence:
 1. The Identity resource is created for a specific Tax ID
 2. Documents are attached to the Identity resource
 3. The Identity resource is updated to indicate that all documents have been attached
 4. The Identity is sent for validation and returns a webhook notification to reflect
 the success or failure of the operation
 
 ### Create IndividualIdentities
+
 You can create an IndividualIdentity to validate a document of a natural person
 
 ```python
 import starkinfra
 
 identities = starkinfra.individualidentity.create([
     starkinfra.IndividualIdentity(
@@ -2481,28 +2606,26 @@
 identity = starkinfra.individualidentity.update("5155165527080960", status="processing")
 
 print(identity)
 ```
 
 **Note**: Before sending your individual identity to validation by patching its status, you must send all the required documents using the create method of the CreditDocument resource. Note that you must reference the individual identity in the create method of the CreditDocument resource by its id.
 
-
 ### Cancel an IndividualIdentity
 
 You can cancel an individual identity before updating its status to processing.
 
-
 ```python
 import starkinfra
 
 identity = starkinfra.individualidentity.cancel("5155165527080960")
 
 print(identity)
 ```
-  
+
 ### Query IndividualIdentity logs
 
 You can query individual identity logs to better understand individual identity life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
@@ -2526,14 +2649,15 @@
 
 log = starkinfra.individualidentity.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create IndividualDocuments
+
 You can create an individual document to attach images of documents to a specific individual Identity.
 You must reference the desired individual identity by its id.
 
 ```python
 import starkinfra
 
 documents = starkinfra.individualdocument.create([
@@ -2559,15 +2683,15 @@
 
 for document in documents:
     print(document)
 ```
 
 **Note**: Instead of using IndividualDocument objects, you can also pass each element in dictionary format
 
-### Query IndividualDocument
+### Query IndividualDocuments
 
 You can query multiple individual documents according to filters.
 
 ```python
 import starkinfra
 from datetime import date
 
@@ -2642,42 +2766,42 @@
         "pix-request.in", "pix-request.out", "pix-reversal.in", "pix-reversal.out", "pix-claim", "pix-key", "pix-chargeback", "pix-infraction",
     ],
 )
 
 print(webhook)
 ```
 
-### Query webhooks
+### Query webhook subscriptions
 
-To search for registered webhooks, run:
+To search for registered webhook subscriptions, run:
 
 ```python
 import starkinfra
 
 webhooks = starkinfra.webhook.query()
 
 for webhook in webhooks:
     print(webhook)
 ```
 
-### Get a webhook
+### Get a webhook subscription
 
-You can get a specific webhook by its id.
+You can get a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.get("1082736198236817")
 
 print(webhook)
 ```
 
-### Delete a webhook
+### Delete a webhook subscription
 
-You can also delete a specific webhook by its id.
+You can also delete a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.delete("1082736198236817")
 
 print(webhook)
```

### Comparing `starkinfra-0.6.0/README.md` & `starkinfra-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 - [Testing in Sandbox](#testing-in-sandbox) 
 - [Usage](#usage)
     - [Issuing](#issuing)
         - [Products](#query-issuingproducts): View available sub-issuer card products (a.k.a. card number ranges or BINs)
         - [Holders](#create-issuingholders): Manage card holders
         - [Cards](#create-issuingcards): Create virtual and/or physical cards
         - [Design](#query-issuingdesigns): View your current card or package designs
+        - [EmbossingKit](#query-issuingembossingkits): View your current embossing kits
         - [Stock](#query-issuingstocks): View your current stock of a certain IssuingDesign linked to an Embosser on the workspace
         - [Restock](#create-issuingrestocks): Create restock orders of a specific IssuingStock object
         - [EmbossingRequest](#create-issuingembossingrequests): Create embossing requests
         - [Purchases](#process-purchase-authorizations): Authorize and view your past purchases
         - [Invoices](#create-issuinginvoices): Add money to your issuing balance
         - [Withdrawals](#create-issuingwithdrawals): Send money back to your Workspace from your issuing balance
         - [Balance](#get-your-issuingbalance): View your issuing balance
@@ -48,14 +49,15 @@
         - [PixDomain](#query-pixdomains): View registered SPI participants certificates
         - [StaticBrcode](#create-staticbrcodes): Create static Pix BR codes
         - [DynamicBrcode](#create-dynamicbrcodes): Create dynamic Pix BR codes
         - [BrcodePreview](#create-brcodepreviews): Read data from BR Codes before paying them
     - [Lending](#lending)
         - [CreditNote](#create-creditnotes): Create credit notes
         - [CreditPreview](#create-creditpreviews): Create credit previews
+        - [CreditHolmes](#create-creditholmes): Create credit holmes debt verification
     - [Identity](#identity)
         - [IndividualIdentity](#create-individualidentities): Create individual identities
         - [IndividualDocument](#create-individualdocuments): Create individual documents
     - [Webhook](#webhook):
         - [Webhook](#create-a-webhook-subscription): Configure your webhook endpoints and subscriptions
         - [WebhookEvents](#process-webhook-events): Manage Webhook events
         - [WebhookEventAttempts](#query-failed-webhook-event-delivery-attempts-information): Query failed webhook event deliveries
@@ -403,27 +405,27 @@
 holder = starkinfra.issuingholder.cancel("5155165527080960")
 
 print(holder)
 ```
 
 ### Get an IssuingHolder
 
-To get a single Issuing Holder by its id, run:
+To get a specific Issuing Holder by its id, run:
 
 ```python
 import starkinfra
 
 holder = starkinfra.issuingholder.get("5155165527080960")
 
 print(holder)
 ```
 
 ### Query IssuingHolder logs
 
-You can query holder logs to better understand holder life cycles.
+You can query IssuingHolder logs to better understand IssuingHolder life cycles.
 
 ```python
 import starkinfra
 
 logs = starkinfra.issuingholder.log.query(limit=50)
 
 for log in logs:
@@ -557,15 +559,14 @@
 
 ### Query IssuingDesigns
 
 You can get a list of available designs given some filters.
 
 ```python
 import starkinfra
-from datetime import date
 
 designs = starkinfra.issuingdesign.query(
     limit=1
 )
 
 for design in designs:
     print(design)
@@ -579,14 +580,43 @@
 import starkinfra
 
 design = starkinfra.issuingdesign.get("5747368922185728")
 
 print(design)
 ```
 
+### Query IssuingEmbossingKits
+
+You can get a list of existing embossing kits given some filters.
+
+```python
+import starkinfra
+from datetime import date
+
+kits = starkinfra.issuingembossingkit.query(
+    after=date(2022, 11, 1),
+    before=date(2022, 12, 1)
+)
+
+for kit in kits:
+    print(kit)
+```
+
+### Get an IssuingEmbossingKit
+
+After its creation, information on an embossing kit may be retrieved by its id.
+
+```python
+import starkinfra
+
+kit = starkinfra.issuingembossingkit.get("5664445921492992")
+
+print(kit)
+```
+
 ### Query IssuingStocks
 
 You can get a list of available stocks given some filters.
 
 ```python
 import starkinfra
 from datetime import date
@@ -714,16 +744,15 @@
 You can create a request to emboss a physical card.
 
 ```python
 import starkinfra
 
 embossing_requests = starkinfra.issuingembossingrequest.create([
     starkinfra.IssuingEmbossingRequest(
-        card_design_id="5648359658356736", 
-        envelope_design_id="5747368922185728", 
+        kit_id="5648359658356736", 
         card_id="5714424132272128", 
         display_name_1="Antonio Stark", 
         shipping_city="Sao Paulo",
         shipping_country_code="BRA",
         shipping_district="Bela Vista",
         shipping_service="loggi",
         shipping_state_code="SP",
@@ -955,15 +984,15 @@
 
 print(log)
 ```
 
 ### Create IssuingWithdrawals
 
 You can create withdrawals to send cash back from your Issuing balance to your Banking balance
-by using the Withdrawal resource.
+by using the IssuingWithdrawal resource.
 
 ```python
 import starkinfra
 
 withdrawal = starkinfra.issuingwithdrawal.create(
     withdrawal=starkinfra.IssuingWithdrawal(
         amount=10000,
@@ -1974,15 +2003,15 @@
     uuids=["5ddde28043a245c2848b08cf315effa2"]
 )
 
 for brcode in brcodes:
     print(brcode)
 ```
 
-### Get a StaticBrcodes
+### Get a StaticBrcode
 
 After its creation, information on a StaticBrcode may be retrieved by its UUID.
 
 ```python
 import starkinfra
 
 brcode = starkinfra.staticbrcode.get("5ddde28043a245c2848b08cf315effa2")
@@ -2045,15 +2074,15 @@
 brcode = starkinfra.dynamicbrcode.get("ac7caa14e601461dbd6b12bf7e4cc48e")
 
 print(brcode)
 ```
 
 ### Verify a DynamicBrcode read
 
-When a DynamicBrcode is read by your user, a GET request will be made to the your regitered URL to 
+When a DynamicBrcode is read by your user, a GET request will be made to your registered URL to 
 retrieve additional information needed to complete the transaction.
 Use this method to verify the authenticity of a GET request received at your registered endpoint.
 If the provided digital signature does not check out with the StarkInfra public key, a stark.exception.InvalidSignatureException will be raised.
 
 ```python
 import starkinfra
 
@@ -2138,14 +2167,15 @@
         cashier_bank_code=invoice.cashier_bank_code,
         cash_amount=invoice.cash_amount
     )
 )
 ```
 
 ## Create BrcodePreviews
+
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
@@ -2173,14 +2203,15 @@
  3. (Optional) Create a [Credit Simulation](#create-creditpreviews) 
 with the desired installment plan to display information for the credit receiver
  4. Create a [Credit Note](#create-creditnotes)
 with the desired installment plan
 
 
 ### Create CreditNotes
+
 For lending operations, you can create a CreditNote to generate a CCB contract.
 
 Note that you must have recently created an identity check for that same Tax ID before
 being able to create a credit operation for them.
 
 ```python
 import starkinfra
@@ -2277,15 +2308,15 @@
 note = starkinfra.creditnote.cancel("5155165527080960")
 
 print(note)
 ```
   
 ### Query CreditNote logs
 
-You can query credit note logs to better understand credit note life cycles. 
+You can query credit note logs to better understand CreditNote life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
 
 logs = starkinfra.creditnote.log.query(
     limit=50, 
@@ -2306,14 +2337,15 @@
 
 log = starkinfra.creditnote.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create CreditPreviews
+
 You can preview a credit operation before creating them (Currently we only have CreditNote / CCB previews):
 
 ```python
 import starkinfra
 from datetime import date
 
 previews = starkinfra.creditpreview.create([
@@ -2391,26 +2423,119 @@
 
 for preview in previews:
     print(preview)
 ```
 
 **Note**: Instead of using CreditPreview objects, you can also pass each element in dictionary format
 
+### Create CreditHolmes
+
+Before you request a credit operation, you may want to check previous credit operations
+the credit receiver has taken.
+
+For that, open up a CreditHolmes investigation to receive information on all debts and credit
+operations registered for that individual or company inside the Central Bank's SCR.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.create([
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-09"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-08"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-07"
+    )
+])
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Query CreditHolmes
+
+You can query multiple credit holmes according to filters.
+
+```python
+import starkinfra
+from datetime import date
+
+holmes = starkinfra.creditholmes.query(
+    after=date(2022, 6, 1),
+    before=date(2022, 10, 30),
+    status="success"
+)
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Get a CreditHolmes
+
+After its creation, information on a credit holmes may be retrieved by its id.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.get("5657818854064128")
+
+print(holmes)
+```
+
+### Query CreditHolmes logs
+
+You can query credit holmes logs to better understand their life cycles. 
+
+```python
+import starkinfra
+from datetime import date
+
+logs = starkinfra.creditholmes.log.query(
+    limit=50, 
+    ids=["5729405850615808"],
+    after=date(2022, 1, 1),
+    before=date(2022, 1, 20),
+    types=["created"]
+)
+
+for log in logs:
+    print(log)
+```
+
+### Get a CreditHolmes log
+
+You can also get a specific log by its id.
+
+```python
+import starkinfra
+
+log = starkinfra.creditholmes.log.get("5155165527080960")
+
+print(log)
+```
+
 ## Identity
 Several operations, especially credit ones, require that the identity
 of a person or business is validated beforehand.
 
 Identities are validated according to the following sequence:
 1. The Identity resource is created for a specific Tax ID
 2. Documents are attached to the Identity resource
 3. The Identity resource is updated to indicate that all documents have been attached
 4. The Identity is sent for validation and returns a webhook notification to reflect
 the success or failure of the operation
 
 ### Create IndividualIdentities
+
 You can create an IndividualIdentity to validate a document of a natural person
 
 ```python
 import starkinfra
 
 identities = starkinfra.individualidentity.create([
     starkinfra.IndividualIdentity(
@@ -2468,28 +2593,26 @@
 identity = starkinfra.individualidentity.update("5155165527080960", status="processing")
 
 print(identity)
 ```
 
 **Note**: Before sending your individual identity to validation by patching its status, you must send all the required documents using the create method of the CreditDocument resource. Note that you must reference the individual identity in the create method of the CreditDocument resource by its id.
 
-
 ### Cancel an IndividualIdentity
 
 You can cancel an individual identity before updating its status to processing.
 
-
 ```python
 import starkinfra
 
 identity = starkinfra.individualidentity.cancel("5155165527080960")
 
 print(identity)
 ```
-  
+
 ### Query IndividualIdentity logs
 
 You can query individual identity logs to better understand individual identity life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
@@ -2513,14 +2636,15 @@
 
 log = starkinfra.individualidentity.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create IndividualDocuments
+
 You can create an individual document to attach images of documents to a specific individual Identity.
 You must reference the desired individual identity by its id.
 
 ```python
 import starkinfra
 
 documents = starkinfra.individualdocument.create([
@@ -2546,15 +2670,15 @@
 
 for document in documents:
     print(document)
 ```
 
 **Note**: Instead of using IndividualDocument objects, you can also pass each element in dictionary format
 
-### Query IndividualDocument
+### Query IndividualDocuments
 
 You can query multiple individual documents according to filters.
 
 ```python
 import starkinfra
 from datetime import date
 
@@ -2629,42 +2753,42 @@
         "pix-request.in", "pix-request.out", "pix-reversal.in", "pix-reversal.out", "pix-claim", "pix-key", "pix-chargeback", "pix-infraction",
     ],
 )
 
 print(webhook)
 ```
 
-### Query webhooks
+### Query webhook subscriptions
 
-To search for registered webhooks, run:
+To search for registered webhook subscriptions, run:
 
 ```python
 import starkinfra
 
 webhooks = starkinfra.webhook.query()
 
 for webhook in webhooks:
     print(webhook)
 ```
 
-### Get a webhook
+### Get a webhook subscription
 
-You can get a specific webhook by its id.
+You can get a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.get("1082736198236817")
 
 print(webhook)
 ```
 
-### Delete a webhook
+### Delete a webhook subscription
 
-You can also delete a specific webhook by its id.
+You can also delete a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.delete("1082736198236817")
 
 print(webhook)
```

### Comparing `starkinfra-0.6.0/setup.py` & `starkinfra-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     license="MIT License",
     url="https://github.com/starkinfra/sdk-python",
     author="Stark Infra",
     author_email="developers@starkbank.com",
     keywords=["stark infra", "starkinfra", "sdk", "open banking", "openbanking", "banking", "open", "stark"],
     version=version,
     install_requires=[
-        "starkcore>=0.0.2",
+        "starkcore>=0.1.0",
     ],
 )
```

### Comparing `starkinfra-0.6.0/starkinfra/__init__.py` & `starkinfra-0.7.0/starkinfra/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = "0.6.0"
+version = "0.7.0"
 language = "en-US"
 timeout = 15
 user = None
 
 from starkcore import Project, Organization, key, error
 
 from . import event
@@ -49,14 +49,17 @@
 
 from . import creditsigner
 from .creditsigner.__creditsigner import CreditSigner
 
 from . import creditpreview
 from .creditpreview.__creditpreview import CreditPreview
 
+from . import creditholmes
+from .creditholmes.__creditholmes import CreditHolmes
+
 from . import individualidentity
 from .individualidentity.__individualidentity import IndividualIdentity
 
 from . import individualdocument
 from .individualdocument.__individualdocument import IndividualDocument
 
 from . import dynamicbrcode
@@ -97,14 +100,17 @@
 
 from . import issuingdesign
 from .issuingdesign.__issuingdesign import IssuingDesign
 
 from . import issuingembossingrequest
 from .issuingembossingrequest.__issuingembossingrequest import IssuingEmbossingRequest
 
+from . import issuingembossingkit
+from .issuingembossingkit.__issuingembossingkit import IssuingEmbossingKit
+
 from . import merchantcategory
 from .merchantcategory.__merchantcategory import MerchantCategory
 
 from . import merchantcountry
 from .merchantcountry.__merchantcountry import MerchantCountry
 
 from . import cardmethod
```

### Comparing `starkinfra-0.6.0/starkinfra/brcodepreview/__brcodepreview.py` & `starkinfra-0.7.0/starkinfra/brcodepreview/__brcodepreview.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from starkcore.utils.resource import Resource
 from starkcore.utils.checks import check_datetime_or_date
 
 
 class BrcodePreview(Resource):
     """# BrcodePreview object
     The BrcodePreview object is used to preview information from a BR Code before paying it.
+    When you initialize a BrcodePreview, the entity will not be automatically
+    created in the Stark Infra API. The 'create' function sends the objects
+    to the Stark Infra API and returns the created object.
     ## Parameters (required):
     - id [string]: BR Code from a Pix payment. This is also de information directly encoded in a QR Code. ex: "00020126580014br.gov.bcb.pix0136a629532e-7693-4846-852d-1bbff817b5a8520400005303986540510.005802BR5908T'Challa6009Sao Paulo62090505123456304B14A"
     ## Attributes (return-only):
     - account_number [string]: Payment receiver account number. ex: "1234567"
     - account_type [string]: Payment receiver account type. ex: "checking"
     - amount [integer]: Value in cents that this payment is expecting to receive. If 0, any value is accepted. ex: 123 (= R$1,23)
     - amount_type [string]: amount type of the Brcode. If the amount type is "custom" the Brcode's amount can be changed by the sender at the moment of payment. Options: "fixed" or "custom"
```

### Comparing `starkinfra-0.6.0/starkinfra/cardmethod/__cardmethod.py` & `starkinfra-0.7.0/starkinfra/cardmethod/__cardmethod.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 
 _resource = {"class": CardMethod, "name": "CardMethod"}
 
 
 def query(search=None, user=None):
     """# Retrieve CardMethods
-    Receive a generator of CardMethod objects previously created in the Stark Infra API
+    Receive a generator of CardMethod objects available in the Stark Infra API
     ## Parameters (optional):
-    - search [string, default None]: keyword to search for code, name, number or short_code
+    - search [string, default None]: keyword to search for code, name or number. ex:"token"
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of CardMethod objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         search=search,
```

### Comparing `starkinfra-0.6.0/starkinfra/creditnote/__creditnote.py` & `starkinfra-0.7.0/starkinfra/creditnote/__creditnote.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 class CreditNote(Resource):
     """# CreditNote object
     CreditNotes are used to generate CCB contracts between you and your customers.
     When you initialize a CreditNote, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the list of created objects.
     ## Parameters (required):
-    - template_id [string]: ID of the contract template on which the CreditNote will be based. ex: template_id="0123456789101112"
-    - name [string]: credit receiver's full name. ex: name="Edward Stark"
+    - template_id [string]: ID of the contract template on which the CreditNote will be based. ex: "0123456789101112"
+    - name [string]: credit receiver's full name. ex: "Edward Stark"
     - tax_id [string]: credit receiver's tax ID (CPF or CNPJ). ex: "20.018.183/0001-80"
-    - nominal_amount [integer]: amount in cents transferred to the credit receiver, before deductions. ex: nominal_amount=11234 (= R$ 112.34)
-    - scheduled [datetime.date, datetime.datetime or string]: date of transfer execution. ex: scheduled=datetime(2020, 3, 10)
-    - invoices [list of Invoice objects]: list of Invoice objects to be created and sent to the credit receiver. ex: invoices=[Invoice(), Invoice()]
-    - payment [creditnote.Transfer]: payment entity to be created and sent to the credit receiver. ex: payment=creditnote.Transfer()
-    - signers [list of CreditSigner objects]: signer's name, contact and delivery method for the signature request. ex: signers=[CreditSigner(), CreditSigner()]
+    - nominal_amount [integer]: amount in cents transferred to the credit receiver, before deductions. ex: 11234 (= R$ 112.34)
+    - scheduled [datetime.date, datetime.datetime or string]: date of transfer execution. ex: datetime(2020, 3, 10)
+    - invoices [list of Invoice objects]: list of Invoice objects to be created and sent to the credit receiver. ex: [Invoice(), Invoice()]
+    - payment [creditnote.Transfer]: payment entity to be created and sent to the credit receiver. ex: creditnote.Transfer()
+    - signers [list of CreditSigner objects]: signer's name, contact and delivery method for the signature request. ex: [CreditSigner(), CreditSigner()]
     - external_id [string]: a string that must be unique among all your CreditNotes, used to avoid resource duplication. ex: "my-internal-id-123456"
     - street_line_1 [string]: credit receiver main address. ex: "Av. Paulista, 200"
     - street_line_2 [string]: credit receiver address complement. ex: "Apto. 123"
     - district [string]: credit receiver address district / neighbourhood. ex: "Bela Vista"
     - city [string]: credit receiver address city. ex: "Rio de Janeiro"
     - state_code [string]: credit receiver address state. ex: "GO"
     - zip_code [string]: credit receiver address zip code. ex: "01311-200"
     ## Parameters (conditionally required):
     - payment_type [string]: payment type, inferred from the payment parameter if it is not a dictionary. ex: "transfer"
-    Parameters (optional):
-    - rebate_amount [integer, default 0]: credit analysis fee deducted from lent amount. ex: rebate_amount=11234 (= R$ 112.34)
-    - tags [list of strings, default []]: list of strings for reference when searching for CreditNotes. ex: tags=["employees", "monthly"]
+    ## Parameters (optional):
+    - rebate_amount [integer, default 0]: credit analysis fee deducted from lent amount. ex: 11234 (= R$ 112.34)
+    - tags [list of strings, default []]: list of strings for reference when searching for CreditNotes. ex: ["employees", "monthly"]
     - expiration [integer or datetime.timedelta, default 604800 (7 days)]: time interval in seconds between scheduled date and expiration date. ex 123456789
-    Attributes (return-only):
+    ## Attributes (return-only):
     - id [string]: unique id returned when the CreditNote is created. ex: "5656565656565656"
     - amount [integer]: CreditNote value in cents. ex: 1234 (= R$ 12.34)
     - document_id [string]: ID of the signed document to execute this CreditNote. ex: "4545454545454545"
     - status [string]: current status of the CreditNote. ex: "canceled", "created", "expired", "failed", "processing", "signed", "success"
     - transaction_ids [list of strings]: ledger transaction ids linked to this CreditNote. ex: ["19827356981273"]
     - workspace_id [string]: ID of the Workspace that generated this CreditNote. ex: "4545454545454545"
     - tax_amount [integer]: tax amount included in the CreditNote. ex: 100
```

### Comparing `starkinfra-0.6.0/starkinfra/creditnote/__transfer.py` & `starkinfra-0.7.0/starkinfra/creditnote/__transfer.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/creditnote/invoice/__description.py` & `starkinfra-0.7.0/starkinfra/creditnote/invoice/__description.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/creditnote/invoice/__invoice.py` & `starkinfra-0.7.0/starkinfra/creditnote/invoice/__invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Invoice issued after the contract is signed, to be paid by the credit receiver.
     ## Parameters (required):
     - amount [integer]: Invoice value in cents. Minimum = 1 (any value will be accepted). ex: 1234 (= R$ 12.34)
     ## Parameters (optional):
     - due [datetime.datetime or datetime.date or string, default now + 2 days]: Invoice due date in UTC ISO format. ex: "2020-10-28T17:59:26.249976+00:00" for immediate invoices and "2020-10-28" for scheduled invoices
     - expiration [integer or datetime.timedelta, default 5097600 (59 days)]: time interval in seconds between due date and expiration date. ex 123456789
     - tags [list of strings, default []]: list of strings for tagging
-    - descriptions [list of creditnote.invoice.Description objects or dictionaries, default None]: list Description objects
+    - descriptions [list of creditnote.invoice.Description objects or dictionaries, default []]: list Description objects
     ## Attributes (return-only):
     - id [string]: unique id returned when Invoice is created. ex: "5656565656565656"
     - name [string]: payer name. ex: "Iron Bank S.A."
     - tax_id [string]: payer tax ID (CPF or CNPJ) with or without formatting. ex: "01234567890" or "20.018.183/0001-80"
     - pdf [string]: public Invoice PDF URL. ex: "https://invoice.starkbank.com/pdf/d454fa4e524441c1b0c1a729457ed9d8"
     - link [string]: public Invoice webpage URL. ex: "https://my-workspace.sandbox.starkbank.com/invoicelink/d454fa4e524441c1b0c1a729457ed9d8"
     - fine [float]: Invoice fine for overdue payment in %. ex: 2.5
```

### Comparing `starkinfra-0.6.0/starkinfra/creditnote/log/__log.py` & `starkinfra-0.7.0/starkinfra/creditnote/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# creditnote.Log object
     Every time a CreditNote entity is updated, a corresponding creditnote.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the CreditNote.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - note [CreditNote]: CreditNote entity to which the log refers to.
     - errors [list of strings]: list of errors linked to this CreditNote event
     - type [string]: type of the CreditNote event which triggered the log creation. ex: "canceled", "created", "expired", "failed", "refunded", "registered", "sending", "sent", "signed", "success"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/creditpreview/__creditnotepreview.py` & `starkinfra-0.7.0/starkinfra/creditpreview/__creditnotepreview.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     """# CreditNotePreview object
     A CreditNotePreview is used to preview a CCB contract between the borrower and lender with a specific table type.
     When you initialize a CreditNotePreview, the entity will be automatically sent to the Stark Infra API.
     The 'create' function sends the objects
     to the Stark Infra API and returns the list of preview data.
     ## Parameters (required):
     - type [string]: table type that defines the amortization system. Options: "sac", "price", "american", "bullet", "custom"
-    - nominal_amount [integer]: amount in cents transferred to the credit receiver, before deductions. ex: nominal_amount=11234 (= R$ 112.34)
-    - scheduled [datetime.date, datetime.datetime or string]: date of transfer execution. ex: scheduled=datetime(2020, 3, 10)
+    - nominal_amount [integer]: amount in cents transferred to the credit receiver, before deductions. ex: 11234 (= R$ 112.34)
+    - scheduled [datetime.date, datetime.datetime or string]: date of transfer execution. ex: datetime(2020, 3, 10)
     - tax_id [string]: credit receiver's tax ID (CPF or CNPJ). ex: "20.018.183/0001-80"
     ## Parameters (conditionally required):
-    - invoices [list of Invoice objects]: list of Invoice objects to be created and sent to the credit receiver. ex: invoices=[Invoice(), Invoice()]
+    - invoices [list of Invoice objects]: list of Invoice objects to be created and sent to the credit receiver. ex: [Invoice(), Invoice()]
     - nominal_interest [float]: yearly nominal interest rate of the credit note, in percentage. ex: 12.5
-    - initial_due [datetime.date, datetime.datetime or string]: date of the first invoice. ex: scheduled=datetime(2020, 3, 10)
+    - initial_due [datetime.date, datetime.datetime or string]: date of the first invoice. ex: datetime(2020, 3, 10)
     - count [integer]: quantity of invoices for payment. ex: 12
     - initial_amount [integer]: value of the first invoice in cents. ex: 1234 (= R$12.34)
     - interval [string]: interval between invoices. ex: "year", "month"
     ## Parameters (optional):
-    - rebate_amount [integer, default None]: credit analysis fee deducted from lent amount. ex: rebate_amount=11234 (= R$ 112.34)
+    - rebate_amount [integer, default None]: credit analysis fee deducted from lent amount. ex: 11234 (= R$ 112.34)
     ## Attributes (return-only):
     - amount [integer]: CreditNote value in cents. ex: 1234 (= R$ 12.34)
     - interest [float]: yearly effective interest rate of the credit note, in percentage. ex: 12.5
     - tax_amount [integer]: tax amount included in the CreditNote. ex: 100
     """
 
     def __init__(self, type, nominal_amount, scheduled, tax_id, invoices=None, nominal_interest=None,
```

### Comparing `starkinfra-0.6.0/starkinfra/creditpreview/__creditpreview.py` & `starkinfra-0.7.0/starkinfra/creditpreview/__creditpreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/creditsigner/__creditsigner.py` & `starkinfra-0.7.0/starkinfra/creditsigner/__creditsigner.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/dynamicbrcode/__dynamicbrcode.py` & `starkinfra-0.7.0/starkinfra/dynamicbrcode/__dynamicbrcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                  receiver_street_line, receiver_city, receiver_state_code, receiver_zip_code, expiration=None,
                  sender_tax_id=None, receiver_tax_id=None, fine=None, interest=None, discounts=None,
                  description=None):
     """# Helps you respond to a due DynamicBrcode Read
     When a Due DynamicBrcode is read by your user, a GET request containing the Brcode's 
     UUID will be made to your registered URL to retrieve additional information needed 
     to complete the transaction.
-    The get request must be answered in the following format, within 5 seconds, and with 
+    The GET request must be answered in the following format, within 5 seconds, and with
     an HTTP status code 200.
     ## Parameters (required):
     - version [integer]: integer that represents how many times the BR code was updated.
     - created [datetime.datetime or string]: creation datetime in ISO format of the DynamicBrcode. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - due [datetime.datetime or string]: requested payment due datetime in ISO format. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - key_id [string]: receiver's PixKey id. Can be a tax_id (CPF/CNPJ), a phone number, an email or an alphanumeric sequence (EVP). ex: "+5511989898989"
     - status [string]: BR code status. Options: "created", "overdue", "paid", "canceled" or "expired"
@@ -193,15 +193,15 @@
 
 
 def response_instant(version, created, key_id, status, reconciliation_id, amount, expiration=None, sender_name=None, sender_tax_id=None,
                     description=None, amount_type=None, cash_amount=None, cashier_type=None, cashier_bank_code=None):
     """# Helps you respond to an instant DynamicBrcode Read
     When an instant DynamicBrcode is read by your user, a GET request containing the BR code's UUID will be made
     to your registered URL to retrieve additional information needed to complete the transaction.
-    The get request must be answered in the following format within 5 seconds and with an HTTP status code 200.
+    The GET request must be answered in the following format within 5 seconds and with an HTTP status code 200.
     ## Parameters (required):
     - version [integer]: integer that represents how many times the BR code was updated.
     - created [datetime.datetime or string]: creation datetime of the DynamicBrcode. ex: "2022-05-17"
     - key_id [string]: receiver's PixKey id. Can be a tax_id (CPF/CNPJ), a phone number, an email or an alphanumeric sequence (EVP). ex: "+5511989898989"
     - status [string]: BR code status. Options: "created", "overdue", "paid", "canceled" or "expired"
     - reconciliation_id [string]: id to be used for conciliation of the resulting Pix transaction. ex: "cd65c78aeb6543eaaa0170f68bd741ee"
     - amount [integer]: positive integer that represents the amount in cents of the resulting Pix transaction. ex: 1234 (= R$ 12.34)
```

### Comparing `starkinfra-0.6.0/starkinfra/event/__event.py` & `starkinfra-0.7.0/starkinfra/event/__event.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 class Event(Resource):
     """# Webhook Event object
     An Event is the notification received from the subscription to the Webhook.
     Events cannot be created, but may be retrieved from the Stark Infra API to
     list all generated updates on entities.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the Event is created. ex: "5656565656565656"
     - log [Log]: a Log object from one of the subscribed services (PixRequestLog, PixReversalLog)
     - created [datetime.datetime]: creation datetime for the notification Event. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - is_delivered [bool]: true if the Event has been successfully delivered to the user url. ex: False
     - subscription [string]: service that triggered this Event. Options: "pix-request.in", "pix-request.out", "pix-reversal.in", "pix-reversal.out", "pix-key", "pix-claim", "pix-infraction", "pix-chargeback", "issuing-card", "issuing-invoice", "issuing-purchase", "credit-note"
     - workspace_id [string]: ID of the Workspace that generated this Event. Mostly used when multiple Workspaces have Webhooks registered to the same endpoint. ex: "4545454545454545"
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/event/attempt/__attempt.py` & `starkinfra-0.7.0/starkinfra/event/attempt/__attempt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from starkcore.utils.checks import check_datetime, check_date
 
 
 class Attempt(Resource):
     """# Event.Attempt object
     When an Event delivery fails, an event attempt will be registered.
     It carries information meant to help you debug event reception issues.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id that identifies the delivery attempt. ex: "5656565656565656"
     - code [string]: delivery error code. ex: badHttpStatus, badConnection, timeout
     - message [string]: delivery error full description. ex: "HTTP POST request returned status 404"
     - event_id [string]: ID of the Event whose delivery failed. ex: "4848484848484848"
     - webhook_id [string]: ID of the Webhook that triggered this event. ex: "5656565656565656"
     - created [datetime.datetime]: datetime representing the moment when the attempt was made. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/individualdocument/__individualdocument.py` & `starkinfra-0.7.0/starkinfra/individualdocument/__individualdocument.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 
 
 class IndividualDocument(Resource):
     """# IndividualDocument object
     Individual documents are images containing either side of a document or a selfie
     to be used in a matching validation. When created, they must be attached to an individual
     identity to be used for its validation.
-
     When you initialize a IndividualDocument, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the list of created objects.
     ## Parameters (required):
     - type [string]: type of the IndividualDocument. Options: "drivers-license-front", "drivers-license-back", "identity-front", "identity-back" or "selfie"
     - content [string]: Base64 data url of the picture. ex: data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIAAD...
     - content_type [string]: content MIME type. This parameter is required as input only. ex: "image/png" or "image/jpeg"
-    - identity_id [string]: Unique id of IndividualIdentity. ex: "5656565656565656"
+    - identity_id [string]: unique id of IndividualIdentity. ex: "5656565656565656"
     ## Parameters (optional):
-    - tags [list of strings, default []]: list of strings for reference when searching for IndividualDocuments. ex: tags=["employees", "monthly"]
+    - tags [list of strings, default []]: list of strings for reference when searching for IndividualDocuments. ex: ["employees", "monthly"]
     ## Attributes (return-only):
     - id [string]: unique id returned when the IndividualDocument is created. ex: "5656565656565656"
     - status [string]: current status of the IndividualDocument. Options: "created", "canceled", "processing", "failed", "success"
     - created [datetime.datetime]: creation datetime for the IndividualDocument. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, type, content, identity_id, content_type=None, tags=None, id=None, status=None, created=None):
@@ -47,15 +46,15 @@
 _resource = {"class": IndividualDocument, "name": "IndividualDocument"}
 
 
 def create(documents, user=None):
     """# Create IndividualDocuments
     Send a list of IndividualDocument objects for creation at the Stark Infra API
     ## Parameters (required):
-    - identities [list of IndividualDocument objects]: list of IndividualDocument objects to be created in the API
+    - documents [list of IndividualDocument objects]: list of IndividualDocument objects to be created in the API
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of IndividualDocument objects with updated attributes
     """
     return rest.post_multi(resource=_resource, entities=documents, user=user)
```

### Comparing `starkinfra-0.6.0/starkinfra/individualdocument/log/__log.py` & `starkinfra-0.7.0/starkinfra/individualdocument/log/__log.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# individualdocument.Log object
     Every time a IndividualDocument entity is updated, a corresponding individualdocument.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IndividualDocument.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - document [IndividualDocument]: IndividualDocument entity to which the log refers to.
     - errors [list of strings]: list of errors linked to this IndividualDocument event
     - type [string]: type of the IndividualDocument event which triggered the log creation. ex: "created", "canceled", "processing", "failed", "success"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/individualidentity/__individualidentity.py` & `starkinfra-0.7.0/starkinfra/individualidentity/__individualidentity.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     documents must be attached to it using the created method of the individual document resource. When all the required
     individual documents are attached to an individual identity it can be sent to validation by patching its status to 
     processing.
     When you initialize a IndividualIdentity, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the list of created objects.
     ## Parameters (required):
-    - name [string]: individual's full name. ex: "Edward Stark". ex: name="Edward Stark"
+    - name [string]: individual's full name. ex: "Edward Stark".
     - tax_id [string]: individual's tax ID (CPF). ex: "594.739.480-42"
-    Parameters (optional):
-    - tags [list of strings, default []]: list of strings for reference when searching for IndividualIdentities. ex: tags=["employees", "monthly"]
-    Attributes (return-only):
+    ## Parameters (optional):
+    - tags [list of strings, default []]: list of strings for reference when searching for IndividualIdentities. ex: ["employees", "monthly"]
+    ## Attributes (return-only):
     - id [string]: unique id returned when the IndividualIdentity is created. ex: "5656565656565656"
     - status [string]: current status of the IndividualIdentity. ex: "created", "canceled", "processing", "failed", "success"
     - created [datetime.datetime]: creation datetime for the IndividualIdentity. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, name, tax_id, tags=None, id=None, status=None, created=None):
         Resource.__init__(self, id=id)
```

### Comparing `starkinfra-0.6.0/starkinfra/individualidentity/log/__log.py` & `starkinfra-0.7.0/starkinfra/individualidentity/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# individualidentity.Log object
     Every time a IndividualIdentity entity is updated, a corresponding individualidentity.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IndividualIdentity.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - identity [IndividualIdentity]: IndividualIdentity entity to which the log refers to.
     - errors [list of strings]: list of errors linked to this IndividualIdentity event
     - type [string]: type of the IndividualIdentity event which triggered the log creation. ex: "created", "canceled", "processing", "failed", "success"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingbalance/__issuingbalance.py` & `starkinfra-0.7.0/starkinfra/issuingbalance/__issuingbalance.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/issuingcard/__issuingcard.py` & `starkinfra-0.7.0/starkinfra/issuingcard/__issuingcard.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,36 +69,36 @@
 
 def create(cards, expand=None, user=None):
     """# Create IssuingCards
     Send a list of IssuingCard objects for creation at the Stark Infra API
     ## Parameters (required):
     - cards [list of IssuingCard objects]: list of IssuingCard objects to be created in the API
     ## Parameters (optional):
-    - expand [list of strings, default []]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
+    - expand [list of strings, default None]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of IssuingCard objects with updated attributes
     """
     return rest.post_multi(resource=_resource, entities=cards, expand=expand, user=user)
 
 
 def query(limit=None, ids=None, after=None, before=None, status=None, types=None, holder_ids=None, tags=None,
           expand=None, user=None):
     """# Retrieve IssuingCards
     Receive a generator of IssuingCard objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["active", "blocked", "canceled", "expired"]
     - types [list of strings, default None]: card type. ex: ["virtual"]
     - holder_ids [list of strings]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
-    - expand [list of strings, default []]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - expand [list of strings, default None]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of IssuingCard objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
@@ -117,22 +117,22 @@
 def page(cursor=None, limit=None, ids=None, after=None, before=None, status=None, types=None, holder_ids=None,
          tags=None, expand=None, user=None):
     """# Retrieve paged IssuingCards
     Receive a list of IssuingCard objects previously created in the Stark Infra API and the cursor to the next page.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["active", "blocked", "canceled", "expired"]
     - types [list of strings, default None]: card type. ex: ["virtual"]
     - holder_ids [list of strings]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
-    - expand [list of strings, default []]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
+    - expand [list of strings, default None]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of IssuingCard objects with updated attributes
     - cursor to retrieve the next page of IssuingCard objects
     """
     return rest.get_page(
         resource=_resource,
@@ -147,44 +147,46 @@
         tags=tags,
         expand=expand,
         user=user,
     )
 
 
 def get(id, expand=None, user=None):
-    """# Retrieve a specific IssuingCards
-    Receive a single IssuingCards object previously created in the Stark Infra API by its id
+    """# Retrieve a specific IssuingCard
+    Receive a single IssuingCard object previously created in the Stark Infra API by its id
     ## Parameters (required):
     - id [string]: object unique id. ex: "5656565656565656"
     ## Parameters (optional):
     - expand [list of strings, default None]: fields to expand information. ex: ["rules", "security_code", "number", "expiration"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - IssuingCards object with updated attributes
     """
     return rest.get_id(resource=_resource, id=id, expand=expand, user=user)
 
 
-def update(id, status=None, display_name=None, rules=None, tags=None, user=None):
+def update(id, status=None, pin=None, display_name=None, rules=None, tags=None, user=None):
     """# Update IssuingCard entity
     Update an IssuingCard by passing id.
     ## Parameters (required):
     - id [string]: IssuingCard id. ex: '5656565656565656'
     ## Parameters (optional):
     - status [string, default None]: You may block the IssuingCard by passing 'blocked' or activate by passing 'active' in the status
-    - display_name [string, default None]: card displayed name
+    - pin [string, default None]: You may unlock your physical card by passing its PIN. This is also the PIN you use to authorize a purhcase.
+    - display_name [string, default None]: card displayed name. ex: "ANTHONY EDWARD"
     - rules [list of dictionaries, default None]: list of dictionaries with "amount": int, "currencyCode": string, "id": string, "interval": string, "name": string pairs.
-    - tags [list of strings]: list of strings for tagging
+    - tags [list of strings, default None]: list of strings for tagging
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - target IssuingCard with updated attributes
     """
     payload = {
         "status": status,
         "display_name": display_name,
+        "pin": pin,
         "rules": rules,
         "tags": tags,
     }
     return rest.patch_id(resource=_resource, id=id, user=user, payload=payload)
 
 
 def cancel(id, user=None):
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingcard/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingcard/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# issuingcard.Log object
     Every time an IssuingCard entity is updated, a corresponding issuingcard.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingCard.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - card [IssuingCard]: IssuingCard entity to which the log refers to.
     - type [string]: type of the IssuingCard event which triggered the log creation. ex: "blocked", "canceled", "created", "expired", "unblocked", "updated"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, id, card, type, created):
@@ -42,20 +42,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, card_ids=None, types=None, after=None, before=None, limit=None, user=None):
     """# Retrieve issuingcard.Log
     Receive a generator of issuingcard.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["blocked", "canceled", "created", "expired", "unblocked", "updated"]
     - card_ids [list of strings, default None]: list of IssuingCard ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of issuingcard.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingdesign/__issuingdesign.py` & `starkinfra-0.7.0/starkinfra/issuingdesign/__issuingdesign.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from starkcore.utils.api import from_api_json
 from starkcore.utils.resource import Resource
 from starkcore.utils.checks import check_datetime
 from ..utils import rest
 
 
 class IssuingDesign(Resource):
     """# IssuingDesign object
@@ -24,14 +25,26 @@
         self.created = check_datetime(created)
         self.updated = check_datetime(updated)
 
 
 _resource = {"class": IssuingDesign, "name": "IssuingDesign"}
 
 
+def parse_designs(designs):
+    parsed_designs = []
+    if designs is None:
+        return designs
+    for design in designs:
+        if isinstance(design, IssuingDesign):
+            parsed_designs.append(design)
+            continue
+        parsed_designs.append(from_api_json(_resource, design))
+    return parsed_designs
+
+
 def query(limit=None, ids=None, user=None):
     """# Retrieve IssuingDesigns
     Receive a generator of IssuingDesign objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
@@ -72,15 +85,15 @@
     """# Retrieve a specific IssuingDesign
     Receive a single IssuingDesign object previously created in the Stark Infra API by its id
     ## Parameters (required):
     - id [string]: object unique id. ex: "5656565656565656"
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
-    - IssuingDesigns object with updated attributes
+    - IssuingDesign object with updated attributes
     """
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def pdf(id, user=None):
     """# Retrieve a specific IssuingDesign pdf file
     Receive a single IssuingDesign pdf file generated in the Stark Infra API by its id.
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py` & `starkinfra-0.7.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 
 class IssuingEmbossingRequest(Resource):
     """# IssuingEmbossingRequest object
     The IssuingEmbossingRequest object displays the information of embossing requests in your Workspace.
     ## Parameters (required):
     - card_id [string]: id of the IssuingCard to be embossed. ex "5656565656565656"
-    - card_design_id [string]: card IssuingDesign id. ex "5656565656565656"
-    - envelope_design_id [string]: envelope IssuingDesign id. ex "5656565656565656"
+    - kit_id [string]: card embossing kit id. ex "5656565656565656"
     - display_name_1 [string]: card displayed name. ex: "ANTHONY STARK"
     - shipping_city [string]: shipping city. ex: "NEW YORK"
     - shipping_country_code [string]: shipping country code. ex: "US"
     - shipping_district [string]: shipping district. ex: "NY"
     - shipping_state_code [string]: shipping state code. ex: "NY"
     - shipping_street_line_1 [string]: shipping main address. ex: "AVENUE OF THE AMERICAS"
     - shipping_street_line_2 [string]: shipping address complement. ex: "Apt. 6"
@@ -23,31 +22,30 @@
     ## Parameters (optional):
     - embosser_id [string]: id of the card embosser. ex: "5656565656565656"
     - display_name_2 [string]: card displayed name. ex: "IT Services"
     - display_name_3 [string]: card displayed name. ex: "StarkBank S.A."
     - shipping_phone [string]: shipping phone. ex: "+5511999999999"
     - tags [list of strings, default None]: list of strings for tagging. ex: ["card", "corporate"]
     ## Attributes (return-only):
-    - id [string, default None]: unique id returned when IssuingEmbossingRequest is created. ex: "5656565656565656"
+    - id [string]: unique id returned when IssuingEmbossingRequest is created. ex: "5656565656565656"
     - fee [integer]: fee charged when IssuingEmbossingRequest is created. ex: 1000
     - status [string]: status of the IssuingEmbossingRequest. ex: "created", "processing", "success", "failed"
     - updated [datetime.datetime]: latest update datetime for the IssuingEmbossingRequest. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the IssuingEmbossingRequest. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
-    def __init__(self, card_id, card_design_id, envelope_design_id, display_name_1, shipping_city, 
+    def __init__(self, card_id, kit_id, display_name_1, shipping_city,
                  shipping_country_code, shipping_district, shipping_state_code, shipping_street_line_1, 
                  shipping_street_line_2, shipping_service, shipping_tracking_number, shipping_zip_code, 
                  embosser_id=None, display_name_2=None, display_name_3=None, shipping_phone=None, 
                  tags=None, id=None, fee=None, status=None, updated=None, created=None):
         Resource.__init__(self, id=id)
 
         self.card_id = card_id
-        self.card_design_id = card_design_id
-        self.envelope_design_id = envelope_design_id
+        self.kit_id = kit_id
         self.display_name_1 = display_name_1
         self.shipping_city = shipping_city
         self.shipping_country_code = shipping_country_code
         self.shipping_district = shipping_district
         self.shipping_state_code = shipping_state_code
         self.shipping_street_line_1 = shipping_street_line_1
         self.shipping_street_line_2 = shipping_street_line_2
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingembossingrequest/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Log(Resource):
     """# issuingembossingrequest.Log object
     Every time an IssuingEmbossingRequest entity is updated, a corresponding issuingembossingrequest.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingEmbossingRequest.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - request [IssuingEmbossingRequest]: IssuingEmbossingRequest entity to which the log refers to.
     - errors [list of StarkCore.Error]: list of errors linked to this IssuingEmbossingRequest event.
     - type [string]: type of the IssuingEmbossingRequest event which triggered the log creation. ex: "created", "sending", "sent", "processing", "success", "failed"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
@@ -33,19 +33,19 @@
 
 
 def query(limit=None, ids=None, after=None, before=None, types=None, request_ids=None, user=None):
     """# Retrieve issuingembossingrequest.Log
     Receive a generator of issuingembossingrequest.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "sending", "sent", "processing", "success", "failed"]
     - request_ids [list of strings, default None]: list of IssuingEmbossingRequest ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of issuingembossingrequest.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingholder/__issuingholder.py` & `starkinfra-0.7.0/starkinfra/issuingholder/__issuingholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from ..issuingrule import parse_rules
 
 
 class IssuingHolder(Resource):
     """# IssuingHolder object
     The IssuingHolder describes a card holder that may group several cards.
     ## Parameters (required):
-    - name [string]: card holder name.
-    - tax_id [string]: card holder tax ID
-    - external_id [string] card holder external ID
+    - name [string]: card holder name. ex: "Tony Stark"
+    - tax_id [string]: card holder tax ID ex: "012.345.678-90"
+    - external_id [string] card holder unique id, generated by the user to avoid duplicated holders. ex: "my-entity/123"
     ## Parameters (optional):
     - rules [list of IssuingRule, default []]: [EXPANDABLE] list of holder spending rules
     - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: unique id returned when IssuingHolder is created. ex: "5656565656565656"
     - status [string]: current IssuingHolder status. ex: "active", "blocked", "canceled"
-    - updated [datetime.datetime]: latest update datetime for the IssuingHolder. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the IssuingHolder. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
+    - updated [datetime.datetime]: latest update datetime for the IssuingHolder. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, name, tax_id, external_id, rules=None, tags=None, id=None, status=None, updated=None, created=None):
         Resource.__init__(self, id=id)
 
         self.name = name
         self.tax_id = tax_id
@@ -39,15 +39,15 @@
 
 def create(holders, expand=None, user=None):
     """# Create IssuingHolder
     Send a list of IssuingHolder objects for creation at the Stark Infra API
     ## Parameters (required):
     - holders [list of IssuingHolder objects]: list of IssuingHolder objects to be created in the API
     ## Parameters (optional):
-    - expand [list of strings, default []]: fields to expand information. Options: ["rules"]
+    - expand [list of strings, default None]: fields to expand information. Options: ["rules"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of IssuingHolder objects with updated attributes
     """
     return rest.post_multi(resource=_resource, entities=holders, expand=expand, user=user)
 
 
@@ -66,20 +66,20 @@
 
 
 def query(limit=None, ids=None, after=None, before=None, status=None, tags=None, expand=None, user=None):
     """# Retrieve IssuingHolders
     Receive a generator of IssuingHolder objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["active", "blocked", "canceled"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
     - expand [string, default None]: fields to expand information. Options: ["rules"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of IssuingHolder objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
@@ -95,20 +95,20 @@
 
 def page(cursor=None, limit=None, ids=None, after=None, before=None, status=None, tags=None, expand=None, user=None):
     """# Retrieve IssuingHolders
     Receive a list of IssuingHolder objects previously created in the Stark Infra API and the cursor to the next page.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["active", "blocked", "canceled"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
     - expand [string, default None]: fields to expand information. Options: ["rules"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of IssuingHolder objects with updated attributes
     - cursor to retrieve the next page of IssuingHolder objects
     """
     return rest.get_page(
         resource=_resource,
@@ -127,16 +127,16 @@
 def update(id, status=None, name=None, rules=None, tags=None, user=None):
     """# Update IssuingHolder entity
     Update an IssuingHolder by passing id, if it hasn't been paid yet.
     ## Parameters (required):
     - id [string]: IssuingHolder id. ex: '5656565656565656'
     ## Parameters (optional):
     - status [string]: You may block the IssuingHolder by passing 'blocked' in the status
-    - name [string]: card holder name.
-    - tags [list of strings]: list of strings for tagging
+    - name [string]: card holder name. ex: "Tony Stark"
+    - tags [list of strings]: list of strings for tagging. ex: ["tony", "stark"]
     - rules [list of dictionaries, default None]: list of dictionaries with "amount": int, "currencyCode": string, "id": string, "interval": string, "name": string pairs
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - target IssuingHolder with updated attributes
     """
     payload = {
         "status": status,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingholder/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingholder/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# issuingholder.Log object
     Every time an IssuingHolder entity is updated, a corresponding issuingholder.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingHolder.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - holder [IssuingHolder]: IssuingHolder entity to which the log refers to.
     - type [string]: type of the IssuingHolder event which triggered the log creation. ex: "blocked", "canceled", "created", "unblocked", "updated"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, id, holder, type, created):
@@ -43,19 +43,19 @@
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, holder_ids=None, user=None):
     """# Retrieve issuingholder.Log
     Receive a generator of issuingholder.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "blocked"]
     - holder_ids [list of strings, default None]: list of IssuingHolder ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of issuingholder.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -70,20 +70,20 @@
 
 def page(cursor=None, ids=None, limit=None, after=None, before=None, types=None, holder_ids=None, user=None):
     """# Retrieve paged issuingholder.Log
     Receive a list of up to 100 issuingholder.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default 100]: maximum number of objects to be retrieved. It must be an integer between 1 and 100. ex: 50
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "blocked"]
     - holder_ids [list of strings, default None]: list of IssuingHolder ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of issuingholder.Log objects with updated attributes
     - cursor to retrieve the next page of issuingholder.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuinginvoice/__issuinginvoice.py` & `starkinfra-0.7.0/starkinfra/issuinginvoice/__issuinginvoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ..utils import rest
 
 
 class IssuingInvoice(Resource):
     """# IssuingInvoice object
     The IssuingInvoice objects created in your Workspace load your Issuing balance when paid.
     ## Parameters (required):
-    - amount [integer]: IssuingInvoice value in cents. ex: 1234 (= R$ 12.34)
+    - amount [integer]: IssuingInvoice value in cents. Minimum = 0 (R$0,00). ex: 1234 (= R$ 12.34)
     ## Parameters (optional):
     - tax_id [string, default sub-issuer tax ID]: payer tax ID (CPF or CNPJ) with or without formatting. ex: "01234567890" or "20.018.183/0001-80"
     - name [string, default sub-issuer name]: payer name. ex: "Iron Bank S.A."
     - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: unique id returned when IssuingInvoice is created. ex: "5656565656565656"
     - brcode [string]: BR Code for the Invoice payment. ex: "00020101021226930014br.gov.bcb.pix2571brcode-h.development.starkinfra.com/v2/d7f6546e194d4c64a153e8f79f1c41ac5204000053039865802BR5925Stark Bank S.A. - Institu6009Sao Paulo62070503***63042109"
@@ -40,15 +40,15 @@
         self.created = check_datetime(created)
 
 
 _resource = {"class": IssuingInvoice, "name": "IssuingInvoice"}
 
 
 def create(invoice, user=None):
-    """# Create IssuingInvoices
+    """# Create an IssuingInvoice
     Send an IssuingInvoice object for creation at the Stark Infra API
     ## Parameters (required):
     - invoice [IssuingInvoice object]: IssuingInvoice object to be created in the API.
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - IssuingInvoice object with updated attributes
```

### Comparing `starkinfra-0.6.0/starkinfra/issuinginvoice/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuinginvoice/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# issuinginvoice.Log object
     Every time an IssuingInvoice entity is updated, a corresponding issuinginvoice.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingInvoice.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - invoice [IssuingInvoice]: IssuingInvoice entity to which the log refers to.
     - type [string]: type of the IssuingInvoice event which triggered the log creation. ex: "created", "credited", "expired", "overdue", "paid"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, id, invoice, type, created):
@@ -42,19 +42,19 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, user=None):
     """# Retrieve issuinginvoice.Log
     Receive a generator of issuinginvoice.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: list of IssuingInvoice ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "credited", "expired", "overdue", "paid"]
+    - ids [list of strings, default None]: list of IssuingInvoice ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of issuinginvoice.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -68,19 +68,19 @@
 
 def page(cursor=None, ids=None, limit=None, after=None, before=None, types=None, user=None):
     """# Retrieve paged issuinginvoice.Log
     Receive a list of up to 100 issuinginvoice.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default None]: list of IssuingInvoice ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default 100]: maximum number of objects to be retrieved. It must be an integer between 1 and 100. ex: 50
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "credited", "expired", "overdue", "paid"]
+    - ids [list of strings, default None]: list of IssuingInvoice ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of issuinginvoice.Log objects with updated attributes
     - cursor to retrieve the next page of issuinginvoice.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingproduct/__issuingproduct.py` & `starkinfra-0.7.0/starkinfra/issuingproduct/__issuingproduct.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/issuingpurchase/__issuingpurchase.py` & `starkinfra-0.7.0/starkinfra/issuingpurchase/__issuingpurchase.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     - merchant_id [string]: merchant ID. ex: "5656565656565656"
     - merchant_name [string]: merchant name. ex: "Google Cloud Platform"
     - merchant_fee [integer]: fee charged by the merchant to cover specific costs, such as ATM withdrawal logistics, etc. ex: 200 (= R$ 2.00)
     - wallet_id [string]: virtual wallet ID. ex: "5656565656565656"
     - method_code [string]: method code. Options: "chip", "token", "server", "manual", "magstripe" or "contactless"
     - score [float]: internal score calculated for the authenticity of the purchase. None in case of insufficient data. ex: 7.6
     - end_to_end_id [string]: Unique id used to identify the transaction through all of its life cycle, even before the purchase is denied or approved and gets its usual id. ex: "679cd385-642b-49d0-96b7-89491e1249a5"
-    - tags [string]: list of strings for tagging returned by the sub-issuer during the authorization. ex: ["travel", "food"]
+    - tags [list of strings]: list of strings for tagging returned by the sub-issuer during the authorization. ex: ["travel", "food"]
     - zip_code [string]: zip code of the merchant location. ex: "02101234"
     ## Attributes (IssuingPurchase only):
-    - issuing_transaction_ids [string]: ledger transaction ids linked to this Purchase
+    - issuing_transaction_ids [list of strings]: ledger transaction ids linked to this Purchase
     - status [string]: current IssuingCard status. Options: "approved", "canceled", "denied", "confirmed", "voided"
     - updated [datetime.datetime]: latest update datetime for the IssuingPurchase. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the IssuingPurchase. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     ## Attributes (authorization request only):
     - is_partial_allowed [bool]: true if the merchant allows partial purchases. ex: False
     - card_tags [list of strings]: tags of the IssuingCard responsible for this purchase. ex: ["travel", "food"]
     - holder_tags [list of strings]: tags of the IssuingHolder responsible for this purchase. ex: ["technology", "john snow"]
@@ -107,22 +107,22 @@
 
 
 def query(ids=None, limit=None, after=None, before=None, end_to_end_ids=None, holder_ids=None, card_ids=None,
           status=None, user=None):
     """# Retrieve IssuingPurchase
     Receive a generator of IssuingPurchase objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default [], default None]: purchase IDs
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
-    - end_to_end_ids [list of strings, default []]: central bank's unique transaction ID. ex: "E79457883202101262140HHX553UPqeq"
-    - holder_ids [list of strings, default []]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
-    - card_ids [list of strings, default []]: card  IDs. ex: ["5656565656565656", "4545454545454545"]
+    - end_to_end_ids [list of strings, default None]: central bank's unique transaction ID. ex: "E79457883202101262140HHX553UPqeq"
+    - holder_ids [list of strings, default None]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
+    - card_ids [list of strings, default None]: card  IDs. ex: ["5656565656565656", "4545454545454545"]
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["approved", "canceled", "denied", "confirmed", "voided"]
+    - ids [list of strings, default None, default None]: purchase IDs
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of IssuingPurchase objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -135,26 +135,26 @@
         status=status,
         user=user,
     )
 
 
 def page(end_to_end_ids=None, holder_ids=None, card_ids=None, status=None, after=None, before=None, ids=None,
         cursor=None, limit=None, user=None):
-    """# Retrieve paged IssuingPurchase
+    """# Retrieve paged IssuingPurchases
     Receive a list of IssuingPurchase objects previously created in the Stark Infra API and the cursor to the next page.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default [], default None]: purchase IDs
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
-    - end_to_end_ids [list of strings, default []]: central bank's unique transaction ID. ex: "E79457883202101262140HHX553UPqeq"
-    - holder_ids [list of strings, default []]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
-    - card_ids [list of strings, default []]: card  IDs. ex: ["5656565656565656", "4545454545454545"]
+    - end_to_end_ids [list of strings, default None]: central bank's unique transaction ID. ex: "E79457883202101262140HHX553UPqeq"
+    - holder_ids [list of strings, default None]: card holder IDs. ex: ["5656565656565656", "4545454545454545"]
+    - card_ids [list of strings, default None]: card  IDs. ex: ["5656565656565656", "4545454545454545"]
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["approved", "canceled", "denied", "confirmed", "voided"]
+    - ids [list of strings, default None]: purchase IDs
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of IssuingPurchase objects with updated attributes
     - cursor to retrieve the next page of IssuingPurchase objects
     """
     return rest.get_page(
         resource=_resource,
@@ -199,15 +199,15 @@
     """# Helps you respond IssuingPurchase requests
     ## Parameters (required):
     - status [string]: sub-issuer response to the authorization. ex: "approved" or "denied"
     ## Parameters (conditionally required):
     - reason [string]: denial reason. Options: "other", "blocked", "lostCard", "stolenCard", "invalidPin", "invalidCard", "cardExpired", "issuerError", "concurrency", "standInDenial", "subIssuerError", "invalidPurpose", "invalidZipCode", "invalidWalletId", "inconsistentCard", "settlementFailed", "cardRuleMismatch", "invalidExpiration", "prepaidInstallment", "holderRuleMismatch", "insufficientBalance", "tooManyTransactions", "invalidSecurityCode", "invalidPaymentMethod", "confirmationDeadline", "withdrawalAmountLimit", "insufficientCardLimit", "insufficientHolderLimit"
     ## Parameters (optional):
     - amount [integer, default None]: amount in cents that was authorized. ex: 1234 (= R$ 12.34)
-    - tags [list of strings, default []]: tags to filter retrieved object. ex: ["tony", "stark"]
+    - tags [list of strings, default None]: tags to filter retrieved object. ex: ["tony", "stark"]
     ## Return:
     - Dumped JSON string that must be returned to us on the IssuingPurchase request
     """
     params = {"authorization": {
         "status": status,
         "amount": amount,
         "reason": reason,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingpurchase/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingpurchase/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Log(Resource):
     """# issuingpurchase.Log object
     Every time an IssuingPurchase entity is updated, a corresponding issuingpurchase.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingPurchase.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - purchase [IssuingPurchase]: IssuingPurchase entity to which the log refers to.
     - issuing_transaction_id [string]: transaction ID related to the IssuingCard.
     - errors [list of StarkCore.Error]: list of errors linked to this IssuingPurchase event.
     - type [string]: type of the IssuingPurchase event which triggered the log creation. ex: "approved", "canceled", "confirmed", "denied", "reversed", "voided"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
@@ -47,20 +47,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, purchase_ids=None, user=None):
     """# Retrieve issuingpurchase.Log
     Receive a generator of issuingpurchase.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: list of IssuingPurchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["approved", "canceled", "confirmed", "denied", "reversed", "voided"]
     - purchase_ids [list of strings, default None]: list of Purchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of IssuingPurchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of issuingpurchase.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -75,20 +75,20 @@
 
 def page(cursor=None, ids=None, limit=None, after=None, before=None, types=None, purchase_ids=None, user=None):
     """# Retrieve paged issuingpurchase.Log
     Receive a list of up to 100 issuingpurchase.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default None]: list of IssuingPurchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["approved", "canceled", "confirmed", "denied", "reversed", "voided"]
     - purchase_ids [list of strings, default None]: list of Purchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of IssuingPurchase ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of issuingpurchase.Log objects with updated attributes
     - cursor to retrieve the next page of issuingpurchase.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingrestock/__issuingrestock.py` & `starkinfra-0.7.0/starkinfra/issuingrestock/__issuingrestock.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/issuingrestock/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingrestock/log/__log.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# issuingrestock.Log object
     Every time an IssuingRestock entity is updated, a corresponding issuingrestock.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingRestock.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - restock [IssuingRestock]: IssuingRestock entity to which the log refers to.
     - type [string]: type of the IssuingRestock event which triggered the log creation. ex: "created", "processing", "confirmed"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, id, restock, type, created):
@@ -30,19 +30,19 @@
 
 
 def query(limit=None, ids=None, after=None, before=None, types=None, restock_ids=None, user=None):
     """# Retrieve issuingrestock.Log
     Receive a generator of issuingrestock.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "processing", "confirmed"]
     - restock_ids [list of strings, default None]: list of IssuingRestock ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of issuingrestock.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingrule/__issuingrule.py` & `starkinfra-0.7.0/starkinfra/issuingrule/__issuingrule.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from starkcore.utils.resource import Resource
 from starkinfra.cardmethod.__cardmethod import _resource as _method_resource, CardMethod
 from starkinfra.merchantcountry.__merchantcountry import _resource as _country_resource, MerchantCountry
 from starkinfra.merchantcategory.__merchantcategory import _resource as _category_resource, MerchantCategory
 
 
 class IssuingRule(Resource):
-
     """# IssuingRule object
     The IssuingRule object displays the spending rules of IssuingCards and IssuingHolders created in your Workspace.
     ## Parameters (required):
     - name [string]: rule name. ex: "Travel" or "Food"
     - amount [integer]: maximum amount that can be spent in the informed interval. ex: 200000 (= R$ 2000.00)
     ## Parameters (optional):
-    - id [string, default None]: unique id returned when an IssuingRule is created, used to update a specific IssuingRule. ex: "5656565656565656"
     - interval [string, default "lifetime"]: interval after which the rule amount counter will be reset to 0. ex: "instant", "day", "week", "month", "year" or "lifetime"
     - currency_code [string, default "BRL"]: code of the currency that the rule amount refers to. ex: "BRL" or "USD"
     - categories [list of MerchantCategories, default []]: merchant categories accepted by the rule. ex: [MerchantCategory(code="fastFoodRestaurants")]
     - countries [list of MerchantCountries, default []]: countries accepted by the rule. ex: [MerchantCountry(code="BRA")]
     - methods [list of CardMethods, default []]: card purchase methods accepted by the rule. ex: [CardMethod(code="magstripe")]
     ## Attributes (expanded return-only):
+    - id [string]: unique id returned when an IssuingRule is created, used to update a specific IssuingRule. ex: "5656565656565656"
     - counter_amount [integer]: current rule spent amount. ex: 1000
     - currency_symbol [string]: currency symbol. ex: "R$"
     - currency_name [string]: currency name. ex: "Brazilian Real"
     """
 
     def __init__(self, name, amount, id=None, interval=None, currency_code=None, categories=None, countries=None,
                  methods=None, counter_amount=None, currency_symbol=None, currency_name=None):
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingstock/__issuingstock.py` & `starkinfra-0.7.0/starkinfra/issuingstock/__issuingstock.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - design_ids [list of strings, default None]: IssuingDesign unique ids. ex: ["5656565656565656", "4545454545454545"]
     - embosser_ids [list of strings, default None]: Embosser unique ids. ex: ["5656565656565656", "4545454545454545"]
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
-    - expand [list of strings, default []]: fields to expand information. ex: ["balance"]
+    - expand [list of strings, default None]: fields to expand information. ex: ["balance"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of IssuingStock objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingstock/log/__log.py` & `starkinfra-0.7.0/starkinfra/issuingstock/log/__log.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Log(Resource):
     """# issuingstock.Log object
     Every time an IssuingStock entity is updated, a corresponding issuingstock.Log
     is generated for the entity. This log is never generated by the
     user, but it can be retrieved to check additional information
     on the IssuingStock.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - stock [IssuingStock]: IssuingStock entity to which the log refers to.
     - type [string]: type of the IssuingStock event which triggered the log creation. ex: "created", "spent", "restocked", "lost"
     - count [integer]: shift in stock balance. ex: 10
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
@@ -32,19 +32,19 @@
 
 
 def query(limit=None, ids=None, after=None, before=None, types=None, stock_ids=None, user=None):
     """# Retrieve issuingstock.Log
     Receive a generator of issuingstock.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "spent", "restocked", "lost"]
     - stock_ids [list of strings, default None]: list of IssuingStock ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of issuingstock.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         limit=limit,
@@ -60,19 +60,19 @@
 def page(cursor=None, limit=None, ids=None, after=None, before=None, types=None, stock_ids=None, user=None):
     """# Retrieve paged issuingstock.Log
     Receive a list of up to 100 issuingstock.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call.
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 50
-    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter for log event types. ex: ["created", "spent", "restocked", "lost"]
     - stock_ids [list of strings, default None]: list of IssuingStock ids to filter logs. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of issuingstock.Log objects with updated attributes
     - cursor to retrieve the next page of issuingstock.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingtransaction/__issuingtransaction.py` & `starkinfra-0.7.0/starkinfra/issuingtransaction/__issuingtransaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from starkcore.utils.resource import Resource
 from starkcore.utils.checks import check_datetime, check_date
 from ..utils import rest
 
 
 class IssuingTransaction(Resource):
     """# IssuingTransaction object
-    The IssuingTransaction objects created in your Workspace to represent each balance shift.
+    The IssuingTransaction object created in your Workspace to represent each balance shift.
     ## Attributes (return-only):
     - id [string]: unique id returned when IssuingTransaction is created. ex: "5656565656565656"
     - amount [integer]: IssuingTransaction value in cents. ex: 1234 (= R$ 12.34)
     - balance [integer]: balance amount of the Workspace at the instant of the Transaction in cents. ex: 200 (= R$ 2.00)
     - description [string]: IssuingTransaction description. ex: "Buying food"
     - source [string]: source of the transaction. ex: "issuing-purchase/5656565656565656"
     - tags [string]: list of strings inherited from the source resource. ex: ["tony", "stark"]
@@ -41,24 +41,24 @@
     - IssuingTransaction object with updated attributes
     """
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(source=None, tags=None, external_ids=None, after=None, before=None,
           ids=None, limit=None, user=None):
-    """# Retrieve IssuingTransaction
+    """# Retrieve IssuingTransactions
     Receive a generator of IssuingTransaction objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
-    - external_ids [list of strings, default []]: external IDs. ex: ["5656565656565656", "4545454545454545"]
+    - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
+    - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
+    - external_ids [list of strings, default None]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - status [string, default None]: filter for status of retrieved objects. ex: "approved", "canceled", "denied", "confirmed" or "voided"
-    - ids [list of strings, default [], default None]: purchase IDs
-    - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
+    - ids [list of strings, default None, default None]: purchase IDs
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of IssuingTransaction objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         source=source,
@@ -74,19 +74,19 @@
 
 def page(source=None, tags=None, external_ids=None, after=None, before=None,
          ids=None, limit=None, cursor=None, user=None):
     """# Retrieve paged IssuingTransaction
     Receive a list of IssuingTransaction objects previously created in the Stark Infra API and the cursor to the next page.
     ## Parameters (optional):
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
-    - external_ids [list of strings, default []]: external IDs. ex: ["5656565656565656", "4545454545454545"]
+    - external_ids [list of strings, default None]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - status [string, default None]: filter for status of retrieved objects. ex: "approved", "canceled", "denied", "confirmed" or "voided"
-    - ids [list of strings, default [], default None]: purchase IDs
+    - ids [list of strings,default None]: purchase IDs
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - cursor [string, default None]: cursor returned on the previous page function call
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of IssuingTransaction objects with updated attributes
     - cursor to retrieve the next page of IssuingPurchase objects
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py` & `starkinfra-0.7.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The IssuingWithdrawal objects created in your Workspace return cash from your Issuing balance to your
     Banking balance.
     ## Parameters (required):
     - amount [integer]: IssuingWithdrawal value in cents. Minimum = 0 (any value will be accepted). ex: 1234 (= R$ 12.34)
     - external_id [string] IssuingWithdrawal external ID. ex: "12345"
     - description [string]: IssuingWithdrawal description. ex: "sending money back"
     ## Parameters (optional):
-    - tags [list of strings, default []]: list of strings for tagging. ex: ["tony", "stark"]
+    - tags [list of strings, default None]: list of strings for tagging. ex: ["tony", "stark"]
     ## Attributes (return-only):
     - id [string]: unique id returned when IssuingWithdrawal is created. ex: "5656565656565656"
     - transaction_id [string]: Stark Bank ledger transaction ids linked to this IssuingWithdrawal
     - issuing_transaction_id [string]: issuing ledger transaction ids linked to this IssuingWithdrawal
     - updated [datetime.datetime]: latest update datetime for the IssuingWithdrawal. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the IssuingWithdrawal. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
@@ -65,18 +65,18 @@
 
 
 def query(external_ids=None, after=None, before=None, limit=None, tags=None, user=None):
     """# Retrieve IssuingWithdrawals
     Receive a generator of IssuingWithdrawal objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
-    - external_ids [list of strings, default []]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
+    - external_ids [list of strings, default None]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of IssuingWithdrawal objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         external_ids=external_ids,
@@ -90,17 +90,17 @@
 
 def page(external_ids=None, after=None, before=None, limit=None, tags=None, cursor=None, user=None):
     """# Retrieve paged IssuingWithdrawals
     Receive a list of IssuingWithdrawal objects previously created in the Stark Infra API and the cursor to the next page.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
-    - external_ids [list of strings, default []]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
+    - external_ids [list of strings, default None]: external IDs. ex: ["5656565656565656", "4545454545454545"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of IssuingWithdrawal objects with updated attributes
     - cursor to retrieve the next page of IssuingWithdrawal objects
     """
     return rest.get_page(
```

### Comparing `starkinfra-0.6.0/starkinfra/merchantcategory/__merchantcategory.py` & `starkinfra-0.7.0/starkinfra/merchantcategory/__merchantcategory.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/merchantcountry/__merchantcountry.py` & `starkinfra-0.7.0/starkinfra/merchantcountry/__merchantcountry.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/pixbalance/__pixbalance.py` & `starkinfra-0.7.0/starkinfra/pixbalance/__pixbalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 
 
 _resource = {"class": PixBalance, "name": "PixBalance"}
 
 
 def get(user=None):
     """# Retrieve the PixBalance object
-    Receive the Balance object linked to your Workspace in the Stark Infra API
+    Receive the PixBalance object linked to your Workspace in the Stark Infra API
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - PixBalance object with updated attributes
     """
     return next(rest.get_stream(resource=_resource, user=user))
```

### Comparing `starkinfra-0.6.0/starkinfra/pixchargeback/__pixchargeback.py` & `starkinfra-0.7.0/starkinfra/pixchargeback/__pixchargeback.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     to the Stark Infra API and returns the created object.
     ## Parameters (required):
     - amount [integer]: amount in cents to be reversed. ex: 11234 (= R$ 112.34)
     - reference_id [string]: end_to_end_id or return_id of the transaction to be reversed. ex: "E20018183202201201450u34sDGd19lz"
     - reason [string]: reason why the reversal was requested. Options: "fraud", "flaw", "reversalChargeback"
     ## Parameters (optional):
     - description [string, default None]: description for the PixChargeback.
-    - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
+    - tags [list of strings, default None]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: unique id returned when the PixChargeback is created. ex: "5656565656565656"
     - analysis [string]: analysis that led to the result.
     - sender_bank_code [string]: bank_code of the Pix participant that created the PixChargeback. ex: "20018183"
     - receiver_bank_code [string]: bank_code of the Pix participant that received the PixChargeback. ex: "20018183"
     - rejection_reason [string]: reason for the rejection of the Pix chargeback. Options: "noBalance", "accountClosed", "unableToReverse"
     - reversal_reference_id [string]: return_id or end_to_end_id of the reversal transaction. ex: "D20018183202202030109X3OoBHG74wo"
@@ -111,15 +111,16 @@
         tags=tags,
         user=user,
     )
 
 
 def page(cursor=None, limit=None, after=None, before=None, status=None, ids=None, flow=None, tags=None, user=None):
     """# Retrieve PixChargebacks
-    Receive a generator of PixChargeback objects previously created in the Stark Infra API
+    Receive a list of up to 100 PixChargeback objects previously created in the Stark Infra API and the cursor to the next page.
+    Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call.
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["created", "failed", "delivered", "closed", "canceled"]
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
@@ -151,14 +152,15 @@
     - id [string]: PixChargeback id. ex: '5656565656565656'
     - result [string]: result after the analysis of the PixChargeback. Options: "rejected", "accepted", "partiallyAccepted"
     ## Parameters (conditionally required):
     - rejection_reason [string, default None]: if the PixChargeback is rejected a reason is required. Options: "noBalance", "accountClosed", "unableToReverse",
     - reversal_reference_id [string, default None]: return_id of the reversal transaction. ex: "D20018183202201201450u34sDGd19lz"
     ## Parameters (optional):
     - analysis [string, default None]: description of the analysis that led to the result.
+    - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - PixChargeback with updated attributes
     """
     payload = {
         "result": result,
         "rejection_reason": rejection_reason,
         "reversal_reference_id": reversal_reference_id,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixchargeback/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixchargeback/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...utils import rest
 
 
 class Log(Resource):
     """# pixchargeback.Log object
     Every time a PixChargeback entity is modified, a corresponding PixChargeback.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - chargeback [PixChargeback]: PixChargeback entity to which the log refers to.
     - type [string]: type of the PixChargeback event which triggered the log creation. ex: "created", "failed", "delivering", "delivered", "closed", "canceled"
     - errors [list of strings]: list of errors linked to this PixChargeback event
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
     def __init__(self, id, chargeback, type, errors, created):
@@ -41,20 +41,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, chargeback_ids=None, user=None):
     """# Retrieve PixChargeback.Logs
     Receive a generator of PixChargeback.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: Log ids to filter PixChargeback Logs. ex: ["5656565656565656"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "failed", "delivering", "delivered", "closed", "canceled"]
     - chargeback_ids [list of strings, default None]: list of PixChargeback IDs to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixChargeback Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixChargeback.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixclaim/__pixclaim.py` & `starkinfra-0.7.0/starkinfra/pixclaim/__pixclaim.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     - account_created [datetime.date, datetime.datetime or string]: opening Date or DateTime for the account claiming the PixKey. ex: "2022-01-01"
     - account_number [string]: number of the account claiming the PixKey. ex: "76543"
     - account_type [string]: type of the account claiming the PixKey. Options: "checking", "savings", "salary" or "payment"
     - branch_code [string]: branch code of the account claiming the PixKey. ex: "1234"
     - name [string]: holder's name of the account claiming the PixKey. ex: "Jamie Lannister"
     - tax_id [string]: holder's taxId of the account claiming the PixKey (CPF/CNPJ). ex: "012.345.678-90"
     - key_id [string]: id of the registered Pix Key to be claimed. Allowed keyTypes are CPF, CNPJ, phone number or email. ex: "+5511989898989"
-    # Parameters (Options):
+    # Parameters (optional):
     - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: unique id returned when the PixClaim is created. ex: "5656565656565656"
     - status [string]: current PixClaim status. Options: "created", "failed", "delivered", "confirmed", "success", "canceled"
     - type [string]: type of Pix Claim. Options: "ownership", "portability"
     - key_type [string]: keyType of the claimed PixKey. Options: "CPF", "CNPJ", "phone" or "email"
     - flow [string]: direction of the Pix Claim. Options: "in" if you received the PixClaim or "out" if you created the PixClaim.
```

### Comparing `starkinfra-0.6.0/starkinfra/pixclaim/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixclaim/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..__pixclaim import _resource as _pixclaim_resource
 
 
 class Log(Resource):
     """# pixclaim.Log object
     Every time a PixClaim entity is modified, a corresponding PixClaim.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - claim [PixClaim]: PixClaim entity to which the log refers to.
     - type [string]: type of the PixClaim event which triggered the log creation. ex: "created", "failed", "delivering", "delivered", "confirming", "confirmed", "success", "canceling", "canceled"
     - errors [list of strings]: list of errors linked to this PixClaim event
     - reason [string]: reason why the PixClaim was modified, resulting in the Log. Options: "fraud", "userRequested", "accountClosure", "defaultOperation", "reconciliation"
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
@@ -44,20 +44,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, claim_ids=None, user=None):
     """# Retrieve PixClaim.Logs
     Receive a generator of PixClaim.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: Log ids to filter PixClaim Logs. ex: ["5656565656565656"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "failed", "delivering", "delivered", "confirming", "confirmed", "success", "canceling", "canceled"]
     - claim_ids [list of strings, default None]: list of PixClaim ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixClaim Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixClaim.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -72,20 +72,20 @@
 
 def page(cursor=None, ids=None, limit=None, after=None, before=None, types=None, claim_ids=None, user=None):
     """# Retrieve paged PixClaim.Logs
     Receive a list of up to 100 PixClaim.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your claims.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default None]: Log ids to filter PixClaim Logs. ex: ["5656565656565656"]
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "failed", "delivering", "delivered", "confirming", "confirmed", "success", "canceling", "canceled"]
     - claim_ids [list of strings, default None]: list of PixClaim IDs to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixClaim Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of PixClaim.Log objects with updated attributes
     - cursor to retrieve the next page of PixClaim.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixdirector/__pixdirector.py` & `starkinfra-0.7.0/starkinfra/pixdirector/__pixdirector.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     - tax_id [string]: tax ID (CPF) of the PixDirector. ex: "012.345.678-90"
     - phone [string]: phone of the PixDirector. ex: "+551198989898"
     - email [string]: email of the PixDirector. ex: "ned.stark@starkbank.com"
     - password [string]: password of the PixDirector. ex: "12345678"
     - team_email [string]: team email. ex: "pix.team@company.com"
     - team_phones [list of strings]: list of phones of the team. ex: ["+5511988889999", "+5511988889998"]
     ## Attributes (return-only):
-    - id [string]: unique id returned when the PixDirector is created. ex: "5656565656565656"
     - status [string]: current PixDirector status. ex: "success"
     """
 
     def __init__(self, name, tax_id, phone, email, password, team_email, team_phones, id=None, status=None):
         Resource.__init__(self, id=id)
 
         self.name = name
```

### Comparing `starkinfra-0.6.0/starkinfra/pixdomain/__pixdomain.py` & `starkinfra-0.7.0/starkinfra/pixdomain/__pixdomain.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/pixinfraction/__pixinfraction.py` & `starkinfra-0.7.0/starkinfra/pixinfraction/__pixinfraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,24 +81,23 @@
 def query(limit=None, after=None, before=None, status=None, ids=None, type=None, flow=None, tags=None, user=None):
     """# Retrieve PixInfractions
     Receive a generator of PixInfraction objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
-    - status [list of strings, default None]: filter for status of retrieved objects. ex: ["created", "failed", "delivered", "closed", "canceled"]
+    - status [list of strings, default None]: filter for status of retrieved objects. Options: ["created", "failed", "delivered", "closed", "canceled"]
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - type [list of strings, default None]: filter for the type of retrieved PixInfractions. Options: "fraud", "reversal", "reversalChargeback"
     - flow [string, default None]: direction of the PixInfraction flow. Options: "out" if you created the PixInfraction, "in" if you received the PixInfraction.
     - tags [list of strings, default None]: list of strings for tagging. ex: ["travel", "food"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixInfraction objects with updated attributes
     """
-
     return rest.get_stream(
         resource=_resource,
         limit=limit,
         after=check_date(after),
         before=check_date(before),
         status=status,
         ids=ids,
@@ -115,15 +114,15 @@
     Receive a list of up to 100 PixInfraction objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call.
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
-    - status [list of strings, default None]: filter for status of retrieved objects. ex: ["created", "failed", "delivered", "closed", "canceled"]
+    - status [list of strings, default None]: filter for status of retrieved objects. Options: ["created", "failed", "delivered", "closed", "canceled"]
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - type [list of strings, default None]: filter for the type of retrieved PixInfractions. Options: "fraud", "reversal", "reversalChargeback"
     - flow [string, default None]: direction of the PixInfraction flow. Options: "out" if you created the PixInfraction, "in" if you received the PixInfraction.
     - tags [list of strings, default None]: list of strings for tagging. ex: ["travel", "food"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of PixInfraction objects with updated attributes and cursor to retrieve the next page of PixInfraction objects
@@ -141,15 +140,15 @@
         tags=tags,
         user=user,
     )
 
 
 def update(id, result, analysis=None, user=None):
     """# Update PixInfraction entity
-    Respond to a received PixInfraction.
+    Update a PixInfraction by passing id.
     ## Parameters (required):
     - id [string]: PixInfraction id. ex: '5656565656565656'
     - result [string]: result after the analysis of the PixInfraction. Options: "agreed", "disagreed"
     ## Parameters (optional):
     - analysis [string, default None]: analysis that led to the result.
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
```

### Comparing `starkinfra-0.6.0/starkinfra/pixinfraction/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixinfraction/log/__log.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...utils import rest
 
 
 class Log(Resource):
     """# pixinfraction.Log object
     Every time a PixInfraction entity is modified, a corresponding PixInfraction.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - infraction [PixInfraction]: PixInfraction entity to which the log refers to.
     - type [string]: type of the PixInfraction event which triggered the log creation. ex: "created", "failed", "delivering", "delivered", "closed", "canceled"
     - errors [list of strings]: list of errors linked to this PixInfraction event
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
     def __init__(self, id, infraction, type, errors, created):
@@ -41,20 +41,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, infraction_ids=None, user=None):
     """# Retrieve PixInfraction.Logs
     Receive a generator of PixInfraction.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: Log ids to filter PixInfraction Logs. ex: ["5656565656565656"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "failed", "delivering", "delivered", "closed", "canceled"]
     - infraction_ids [list of strings, default None]: list of PixInfraction IDs to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixInfraction Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - generator of PixInfraction.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
@@ -69,20 +69,20 @@
 
 def page(cursor=None, ids=None, limit=None, after=None, before=None, types=None, infraction_ids=None, user=None):
     """# Retrieve paged PixInfraction.Logs
     Receive a list of up to 100 PixInfraction.Log objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your infractions.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
-    - ids [list of strings, default None]: Log ids to filter PixInfraction Logs. ex: ["5656565656565656"]
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "failed", "delivering", "delivered", "closed", "canceled"]
     - infraction_ids [list of strings, default None]: list of PixInfraction ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixInfraction Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call
     ## Return:
     - list of PixInfraction.Log objects with updated attributes
     - cursor to retrieve the next page of PixInfraction.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixkey/__pixkey.py` & `starkinfra-0.7.0/starkinfra/pixkey/__pixkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     - account_number [string]: number of the linked account. ex: "76543"
     - account_type [string]: type of the linked account. Options: "checking", "savings", "salary" or "payment"
     - branch_code [string]: branch code of the linked account. ex: 1234"
     - name [string]: holder's name of the linked account. ex: "Jamie Lannister"
     - tax_id [string]: holder's taxId (CPF/CNPJ) of the linked account. ex: "012.345.678-90"
     ## Parameters (optional):
     - id [string, default None]: id of the registered PixKey. Allowed types are: CPF, CNPJ, phone number or email. If this parameter is not passed, an EVP will be created. ex: "+5511989898989"
-    - tags [list of strings, default []]: list of strings for reference when searching for PixKeys. ex: ["employees", "monthly"]
+    - tags [list of strings, default []]]: list of strings for reference when searching for PixKeys. ex: ["employees", "monthly"]
     ## Attributes (return-only):
     - owned [datetime.datetime]: datetime when the key was owned by the holder. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - owner_type [string]: type of the owner of the PixKey. Options: "business" or "individual"
     - status [string]: current PixKey status. Options: "created", "registered", "canceled", "failed"
     - bank_code [string]: bank_code of the account linked to the Pix Key. ex: "20018183"
     - bank_name [string]: name of the bank that holds the account linked to the PixKey. ex: "StarkBank"
     - type [string]: type of the PixKey. Options: "cpf", "cnpj", "phone", "email" and "evp"
@@ -93,15 +93,14 @@
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - type [string, default None]: filter for the type of retrieved PixKeys. Options: "cpf", "cnpj", "phone", "email" and "evp"
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixKey objects with updated attributes
     """
-
     return rest.get_stream(
         resource=_resource,
         limit=limit,
         after=check_date(after),
         before=check_date(before),
         status=status,
         tags=tags,
@@ -109,15 +108,15 @@
         type=type,
         user=user,
     )
 
 
 def page(cursor=None, limit=None, after=None, before=None, status=None, tags=None, ids=None, type=None,
          user=None):
-    """# Retrieve PixKeys
+    """# Retrieve paged PixKeys
     Receive a generator of PixKey objects previously created in the Stark Infra API
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call.
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - status [list of strings, default None]: filter for status of retrieved objects. ex: ["created", "registered", "canceled", "failed"]
@@ -152,14 +151,15 @@
     - reason [string]: reason why the PixKey is being patched. Options: "branchTransfer", "reconciliation" or "userRequested"
     ## Parameters (optional):
     - account_created [datetime.date, datetime.datetime or string, default None]: opening Date or DateTime for the account to be linked. ex: "2022-01-01"
     - account_number [string, default None]: number of the account to be linked. ex: "76543"
     - account_type [string, default None]: type of the account to be linked. Options: "checking", "savings", "salary" or "payment"
     - branch_code [string, default None]: branch code of the account to be linked. ex: 1234"
     - name [string, default None]: holder's name of the account to be linked. ex: "Jamie Lannister"
+    - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - PixKey with updated attributes
     """
     payload = {
         "reason": reason,
         "account_created": account_created,
         "account_number": account_number,
@@ -167,16 +167,16 @@
         "branch_code": branch_code,
         "name": name,
     }
     return rest.patch_id(resource=_resource, id=id, user=user, payload=payload)
 
 
 def cancel(id, user=None):
-    """# Cancel a pixKey entity
-    Cancel a pixKey entity previously created in the Stark Infra API
+    """# Cancel a PixKey entity
+    Cancel a PixKey entity previously created in the Stark Infra API
     ## Parameters (required):
     - id [string]: object unique id. ex: "5656565656565656"
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - canceled pixKey object
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/pixkey/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixkey/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...utils import rest
 
 
 class Log(Resource):
     """# PixKey.Log object
     Every time a PixKey entity is modified, a corresponding PixKey.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - key [PixKey]: PixKey entity to which the log refers to.
     - type [string]: type of the PixKey event which triggered the log creation. ex: "created", "registered", "updated", "failed", "canceling", "canceled"
     - errors [list of strings]: list of errors linked to this PixKey event
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
     def __init__(self, id, key, type, errors, created):
@@ -41,20 +41,20 @@
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(ids=None, limit=None, after=None, before=None, types=None, key_ids=None, user=None):
     """# Retrieve PixKey.Logs
     Receive a generator of PixKey.Log objects previously created in the Stark Infra API
     ## Parameters (optional):
-    - ids [list of strings, default None]: Log ids to filter PixKey Logs. ex: ["5656565656565656"]
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. ex: ["created", "registered", "updated", "failed", "canceling", "canceled"]
     - key_ids [list of strings, default None]: list of PixKey IDs to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
+    - ids [list of strings, default None]: Log ids to filter PixKey Logs. ex: ["5656565656565656"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixKey.Log objects with updated attributes
     """
     return rest.get_stream(
         resource=_resource,
         ids=ids,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixrequest/__pixrequest.py` & `starkinfra-0.7.0/starkinfra/pixrequest/__pixrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,19 +208,21 @@
     request.external_id = request.external_id or ""
     request.description = request.description or ""
     
     return request
 
 
 def response(status, reason=None):
-    """# Helps you respond to a PixRequest authorization
+    """# Helps you respond to a PixRequest authorization.
+    Authorization requests will be posted at your registered
+    endpoint whenever inbound PixRequests are received.
     ## Parameters (required):
     - status [string]: response to the authorization. ex: "approved" or "denied"
     ## Parameters (conditionally required):
-    - reason [string, default None]: denial reason. Options: "invalidAccountNumber", "blockedAccount", "accountClosed", "invalidAccountType", "invalidTransactionType", "taxIdMismatch", "invalidTaxId", "orderRejected", "reversalTimeExpired", "settlementFailed"
+    - reason [string, default None]: denial reason. Required if the status is "denied". Options: "invalidAccountNumber", "blockedAccount", "accountClosed", "invalidAccountType", "invalidTransactionType", "taxIdMismatch", "invalidTaxId", "orderRejected", "reversalTimeExpired", "settlementFailed"
     ## Return:
     - Dumped JSON string that must be returned to us
     """
     params = {
         "authorization": {
             "status": status,
             "reason": reason,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixrequest/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixrequest/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..__pixrequest import _resource as _pixrequest_resource
 
 
 class Log(Resource):
     """# PixRequest.Log object
     Every time a PixRequest entity is modified, a corresponding PixRequest.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - request [PixRequest]: PixRequest entity to which the log refers to.
     - type [string]: type of the PixRequest event which triggered the log creation. ex: "sent", "denied", "failed", "created", "success", "approved", "credited", "refunded", "processing"
     - errors [list of strings]: list of errors linked to this PixRequest event
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
     def __init__(self, id, request, type, errors, created):
@@ -74,15 +74,15 @@
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None]: date filter for objects created after a specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None]: date filter for objects created before a specified date. ex: datetime.date(2020, 3, 10)
     - types [list of strings, default None]: filter retrieved objects by types. Options: ["sent", "denied", "failed", "created", "success", "approved", "credited", "refunded", "processing"]
     - request_ids [list of strings, default None]: list of PixRequest IDs to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
-    - reconciliation_id [string]: PixRequest reconciliation id to filter retrieved objects. ex: "b77f5236-7ab9-4487-9f95-66ee6eaf1781"
+    - reconciliation_id [string, default None]: PixRequest reconciliation id to filter retrieved objects. ex: "b77f5236-7ab9-4487-9f95-66ee6eaf1781"
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of PixRequest.Log objects with updated attributes
     - cursor to retrieve the next page of PixRequest.Log objects
     """
     return rest.get_page(
         resource=_resource,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixreversal/__pixreversal.py` & `starkinfra-0.7.0/starkinfra/pixreversal/__pixreversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     - return_ids [list of strings, default None]: central bank's unique reversal transaction IDs. ex: ["D20018183202202030109X3OoBHG74wo", "D20018183202202030109X3OoBHG72rd"].
     - external_ids [list of strings, default None]: url safe strings that must be unique among all your PixReversals. Duplicated external IDs will cause failures. By default, this parameter will block any PixReversal that repeats amount and receiver information on the same date. ex: ["my-internal-id-123456", "my-internal-id-654321"]
     - tags [list of strings, default None]: tags to filter retrieved objects. ex: ["tony", "stark"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixReversal objects with updated attributes
     """
-
     return rest.get_stream(
         resource=_resource,
         limit=limit,
         after=check_date(after),
         before=check_date(before),
         status=status,
         ids=ids,
@@ -172,15 +171,15 @@
 
 
 def response(status, reason=None):
     """# Helps you respond to a PixReversal authorization
     ## Parameters (required):
     - status [string]: response to the authorization. ex: "approved" or "denied"
     ## Parameters (conditionally required):
-    - reason [string, default None]: denial reason. Options: "invalidAccountNumber", "blockedAccount", "accountClosed", "invalidAccountType", "invalidTransactionType", "taxIdMismatch", "invalidTaxId", "orderRejected", "reversalTimeExpired", "settlementFailed"
+    - reason [string, default None]: denial reason. Required if the status is "denied". Options: "invalidAccountNumber", "blockedAccount", "accountClosed", "invalidAccountType", "invalidTransactionType", "taxIdMismatch", "invalidTaxId", "orderRejected", "reversalTimeExpired", "settlementFailed"
     ## Return:
     - Dumped JSON string that must be returned to us
     """
     params = {
         "authorization": {
             "status": status,
             "reason": reason,
```

### Comparing `starkinfra-0.6.0/starkinfra/pixreversal/log/__log.py` & `starkinfra-0.7.0/starkinfra/pixreversal/log/__log.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..__pixreversal import _resource as _pixreversal_resource
 
 
 class Log(Resource):
     """# PixReversal.Log object
     Every time a PixReversal entity is modified, a corresponding PixReversal.Log
     is generated for the entity. This log is never generated by the user.
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the log is created. ex: "5656565656565656"
     - reversal [PixReversal object]: PixReversal entity to which the log refers to.
     - type [string]: type of the PixReversal event which triggered the log creation. ex: "sent", "denied", "failed", "created", "success", "approved", "credited", "refunded", "processing"
     - errors [list of strings]: list of errors linked to this PixReversal event
     - created [datetime.datetime]: creation datetime for the log. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
     def __init__(self, id, reversal, type, errors, created):
```

### Comparing `starkinfra-0.6.0/starkinfra/pixstatement/__pixstatement.py` & `starkinfra-0.7.0/starkinfra/pixstatement/__pixstatement.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from starkcore.utils.resource import Resource
 from starkcore.utils.checks import check_datetime, check_date
 
 
 class PixStatement(Resource):
     """# PixStatement object
     The PixStatement object stores information about all the transactions that
-    happened on a specific day at your settlment account according to the Central Bank.
+    happened on a specific day at your settlement account according to the Central Bank.
     It must be created by the user before it can be accessed.
     This feature is only available for direct participants.
     When you initialize a PixStatement, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the created object.
     ## Parameters (required):
     - after [datetime.date]: transactions that happened at this date are stored in the PixStatement, must be the same as before. ex: datetime.date(2020, 3, 10)
     - before [datetime.date]: transactions that happened at this date are stored in the PixStatement, must be the same as after. ex: datetime.date(2020, 3, 10)
     - type [string]: types of entities to include in statement. Options: ["interchange", "interchangeTotal", "transaction"]
     ## Attributes (return-only):
     - id [string]: unique id returned when the PixStatement is created. ex: "5656565656565656"
-    - status [string]: current PixStatement status. ex: ["success", "failed"]
+    - status [string]: current PixStatement status. ex: "success" or "failed"
     - transaction_count [integer]: number of transactions that happened during the day that the PixStatement was requested. ex: 11
     - created [datetime.datetime]: creation datetime for the PixStatement. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - updated [datetime.datetime]: latest update datetime for the PixStatement. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, after, before, type, id=None, status=None, transaction_count=None, created=None, updated=None):
         Resource.__init__(self, id=id)
@@ -71,26 +71,26 @@
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of PixStatement objects with updated attributes
     """
-
     return rest.get_stream(
         resource=_resource,
         limit=limit,
         ids=ids,
         user=user,
     )
 
 
 def page(cursor=None, limit=None, ids=None, user=None):
     """# Retrieve paged PixStatements
     Receive a list of up to 100 PixStatement objects previously created in the Stark Infra API
+    Use this function instead of query if you want to manually page your statements.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - ids [list of strings, default None]: list of ids to filter retrieved objects. ex: ["5656565656565656", "4545454545454545"]
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of PixStatement objects with updated attributes
@@ -103,15 +103,15 @@
         ids=ids,
         user=user,
     )
 
 
 def csv(id, user=None):
     """# Retrieve a .csv PixStatement
-    Retrieve a specific PixStatement by its ID in a .csv file.
+    Retrieve a specific PixStatement by its id in a .csv file.
     ## Parameters (required):
     - id [string]: object unique id. ex: "5656565656565656"
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - .zip file containing a PixStatement in .csv format
     """
```

### Comparing `starkinfra-0.6.0/starkinfra/staticbrcode/__staticbrcode.py` & `starkinfra-0.7.0/starkinfra/staticbrcode/__staticbrcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,37 @@
     A StaticBrcode stores account information in the form of a PixKey and can be used to create 
     Pix transactions easily.
     When you initialize a StaticBrcode, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     ## Parameters (required):
     - name [string]: receiver's name. ex: "Tony Stark"
     - key_id [string]: receiver's Pixkey id. ex: "+5541999999999"
-    - city [string, default São Paulo]: receiver's city name. ex: "Rio de Janeiro"
+    - city [string]: receiver's city name. ex: "Rio de Janeiro"
     ## Parameters (optional):
     - amount [integer, default 0]: positive integer that represents the amount in cents of the resulting Pix transaction. ex: 1234 (= R$ 12.34)
+    - cashier_bank_code [string, default ""] Cashier's bank code. ex: "20018183".
     - reconciliation_id [string, default None]: id to be used for conciliation of the resulting Pix transaction. This id must have up to 25 alphanumeric characters ex: "ah27s53agj6493hjds6836v49"
     - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: id returned on creation, this is the BR code. ex: "00020126360014br.gov.bcb.pix0114+552840092118152040000530398654040.095802BR5915Jamie Lannister6009Sao Paulo620705038566304FC6C"
     - uuid [string]: unique uuid returned when a StaticBrcode is created. ex: "97756273400d42ce9086404fe10ea0d6"
     - url [string]: url link to the BR code image. ex: "https://brcode-h.development.starkinfra.com/static-qrcode/97756273400d42ce9086404fe10ea0d6.png"
     - updated [datetime.datetime]: latest update datetime for the StaticBrcode. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the StaticBrcode. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
-    def __init__(self, name, key_id, city, amount=None, reconciliation_id=None, tags=None, id=None, uuid=None, url=None,
-                    updated=None, created=None):
+    def __init__(self, name, key_id, city, amount=None, cashier_bank_code=None, reconciliation_id=None, tags=None,
+                 id=None, uuid=None, url=None, updated=None, created=None):
         Resource.__init__(self, id=id)
 
         self.name = name
         self.key_id = key_id
         self.city = city
         self.amount = amount
+        self.cashier_bank_code = cashier_bank_code
         self.reconciliation_id = reconciliation_id
         self.tags = tags
         self.uuid = uuid
         self.url = url
         self.updated = check_datetime(updated)
         self.created = check_datetime(created)
 
@@ -91,16 +93,17 @@
         uuids=uuids,
         tags=tags,
         user=user,
     )
 
 
 def page(cursor=None, limit=None, after=None, before=None, uuids=None, tags=None, user=None):
-    """# Retrieve StaticBrcodes
-    Receive a list of StaticBrcode objects previously created in the Stark Infra API and the cursor to the next page.
+    """# Retrieve paged StaticBrcodes
+    Receive a list of up to 100 StaticBrcode objects previously created in the Stark Infra API and the cursor to the next page.
+    Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. Max = 100. ex: 35
     - after [datetime.date or string, default None] date filter for objects created only after specified date. ex: datetime.date(2020, 3, 10)
     - before [datetime.date or string, default None] date filter for objects created only before specified date. ex: datetime.date(2020, 3, 10)
     - uuids [list of strings, default None]: list of uuids to filter retrieved objects. ex: ["97756273400d42ce9086404fe10ea0d6", "e3da0b6d56fa4045b9b295b2be82436e"]
     - tags [list of strings, default None]: list of tags to filter retrieved objects. ex: ["travel", "food"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `starkinfra-0.6.0/starkinfra/utils/relay.py` & `starkinfra-0.7.0/starkinfra/utils/relay.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.6.0/starkinfra/webhook/__webhook.py` & `starkinfra-0.7.0/starkinfra/webhook/__webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Webhook(Resource):
     """# Webhook subscription object
     A Webhook is used to subscribe to notification events on a user-selected endpoint.
     Currently, available services for subscription are credit-note, issuing-card, issuing-invoice, issuing-purchase, pix-request.in, pix-request.out, pix-reversal.in, pix-reversal.out, pix-claim, pix-key, pix-chargeback, pix-infraction,
     ## Parameters (required):
     - url [string]: Url that will be notified when an event occurs.
     - subscriptions [list of strings]: list of any non-empty combination of the available services. ex: ["contract", "credit-note", "signer", "issuing-card", "issuing-invoice", "issuing-purchase", "pix-request.in", "pix-request.out", "pix-reversal.in", "pix-reversal.out", "pix-claim", "pix-key", "pix-chargeback", "pix-infraction"]
-    ## Attributes:
+    ## Attributes (return-only):
     - id [string]: unique id returned when the webhook is created. ex: "5656565656565656"
     """
 
     def __init__(self, url, subscriptions, id=None):
         Resource.__init__(self, id=id)
 
         self.url = url
@@ -47,28 +47,28 @@
     ## Return:
     - Webhook object with updated attributes
     """
     return rest.get_id(resource=_resource, id=id, user=user)
 
 
 def query(limit=None, user=None):
-    """# Retrieve Webhook subcriptions
-    Receive a generator of Webhook subcription objects previously created in the Stark Infra API
+    """# Retrieve Webhook subscriptions
+    Receive a generator of Webhook subscription objects previously created in the Stark Infra API
     ## Parameters (optional):
     - limit [integer, default None]: maximum number of objects to be retrieved. Unlimited if None. ex: 35
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - generator of Webhook objects with updated attributes
     """
     return rest.get_stream(resource=_resource, limit=limit, user=user)
 
 
 def page(cursor=None, limit=None, user=None):
-    """# Retrieve paged Webhooks
-    Receive a list of up to 100 Webhook objects previously created in the Stark Infra API and the cursor to the next page.
+    """# Retrieve paged Webhooks subscriptions
+    Receive a list of up to 100 Webhook subscription objects previously created in the Stark Infra API and the cursor to the next page.
     Use this function instead of query if you want to manually page your requests.
     ## Parameters (optional):
     - cursor [string, default None]: cursor returned on the previous page function call
     - limit [integer, default 100]: maximum number of objects to be retrieved. It must be an integer between 1 and 100. ex: 50
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - list of Webhook objects with updated attributes
@@ -79,16 +79,16 @@
         cursor=cursor,
         limit=limit,
         user=user,
     )
 
 
 def delete(id, user=None):
-    """# Delete a Webhook subscription entity
-    Delete a Webhook subscription entity previously created in the Stark Infra API
+    """# Delete a Webhook subscriptions entity
+    Delete a Webhook subscriptions entity previously created in the Stark Infra API
     ## Parameters (required):
     - id [string]: Webhook unique id. ex: "5656565656565656"
     ## Parameters (optional):
     - user [Organization/Project object, default None]: Organization or Project object. Not necessary if starkinfra.user was set before function call.
     ## Return:
     - deleted Webhook object
     """
```

### Comparing `starkinfra-0.6.0/starkinfra.egg-info/PKG-INFO` & `starkinfra-0.7.0/starkinfra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkinfra
-Version: 0.6.0
+Version: 0.7.0
 Summary: SDK to facilitate Python integrations with Stark Infra
 Home-page: https://github.com/starkinfra/sdk-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
 Platform: UNKNOWN
@@ -35,14 +35,15 @@
 - [Testing in Sandbox](#testing-in-sandbox) 
 - [Usage](#usage)
     - [Issuing](#issuing)
         - [Products](#query-issuingproducts): View available sub-issuer card products (a.k.a. card number ranges or BINs)
         - [Holders](#create-issuingholders): Manage card holders
         - [Cards](#create-issuingcards): Create virtual and/or physical cards
         - [Design](#query-issuingdesigns): View your current card or package designs
+        - [EmbossingKit](#query-issuingembossingkits): View your current embossing kits
         - [Stock](#query-issuingstocks): View your current stock of a certain IssuingDesign linked to an Embosser on the workspace
         - [Restock](#create-issuingrestocks): Create restock orders of a specific IssuingStock object
         - [EmbossingRequest](#create-issuingembossingrequests): Create embossing requests
         - [Purchases](#process-purchase-authorizations): Authorize and view your past purchases
         - [Invoices](#create-issuinginvoices): Add money to your issuing balance
         - [Withdrawals](#create-issuingwithdrawals): Send money back to your Workspace from your issuing balance
         - [Balance](#get-your-issuingbalance): View your issuing balance
@@ -61,14 +62,15 @@
         - [PixDomain](#query-pixdomains): View registered SPI participants certificates
         - [StaticBrcode](#create-staticbrcodes): Create static Pix BR codes
         - [DynamicBrcode](#create-dynamicbrcodes): Create dynamic Pix BR codes
         - [BrcodePreview](#create-brcodepreviews): Read data from BR Codes before paying them
     - [Lending](#lending)
         - [CreditNote](#create-creditnotes): Create credit notes
         - [CreditPreview](#create-creditpreviews): Create credit previews
+        - [CreditHolmes](#create-creditholmes): Create credit holmes debt verification
     - [Identity](#identity)
         - [IndividualIdentity](#create-individualidentities): Create individual identities
         - [IndividualDocument](#create-individualdocuments): Create individual documents
     - [Webhook](#webhook):
         - [Webhook](#create-a-webhook-subscription): Configure your webhook endpoints and subscriptions
         - [WebhookEvents](#process-webhook-events): Manage Webhook events
         - [WebhookEventAttempts](#query-failed-webhook-event-delivery-attempts-information): Query failed webhook event deliveries
@@ -416,27 +418,27 @@
 holder = starkinfra.issuingholder.cancel("5155165527080960")
 
 print(holder)
 ```
 
 ### Get an IssuingHolder
 
-To get a single Issuing Holder by its id, run:
+To get a specific Issuing Holder by its id, run:
 
 ```python
 import starkinfra
 
 holder = starkinfra.issuingholder.get("5155165527080960")
 
 print(holder)
 ```
 
 ### Query IssuingHolder logs
 
-You can query holder logs to better understand holder life cycles.
+You can query IssuingHolder logs to better understand IssuingHolder life cycles.
 
 ```python
 import starkinfra
 
 logs = starkinfra.issuingholder.log.query(limit=50)
 
 for log in logs:
@@ -570,15 +572,14 @@
 
 ### Query IssuingDesigns
 
 You can get a list of available designs given some filters.
 
 ```python
 import starkinfra
-from datetime import date
 
 designs = starkinfra.issuingdesign.query(
     limit=1
 )
 
 for design in designs:
     print(design)
@@ -592,14 +593,43 @@
 import starkinfra
 
 design = starkinfra.issuingdesign.get("5747368922185728")
 
 print(design)
 ```
 
+### Query IssuingEmbossingKits
+
+You can get a list of existing embossing kits given some filters.
+
+```python
+import starkinfra
+from datetime import date
+
+kits = starkinfra.issuingembossingkit.query(
+    after=date(2022, 11, 1),
+    before=date(2022, 12, 1)
+)
+
+for kit in kits:
+    print(kit)
+```
+
+### Get an IssuingEmbossingKit
+
+After its creation, information on an embossing kit may be retrieved by its id.
+
+```python
+import starkinfra
+
+kit = starkinfra.issuingembossingkit.get("5664445921492992")
+
+print(kit)
+```
+
 ### Query IssuingStocks
 
 You can get a list of available stocks given some filters.
 
 ```python
 import starkinfra
 from datetime import date
@@ -727,16 +757,15 @@
 You can create a request to emboss a physical card.
 
 ```python
 import starkinfra
 
 embossing_requests = starkinfra.issuingembossingrequest.create([
     starkinfra.IssuingEmbossingRequest(
-        card_design_id="5648359658356736", 
-        envelope_design_id="5747368922185728", 
+        kit_id="5648359658356736", 
         card_id="5714424132272128", 
         display_name_1="Antonio Stark", 
         shipping_city="Sao Paulo",
         shipping_country_code="BRA",
         shipping_district="Bela Vista",
         shipping_service="loggi",
         shipping_state_code="SP",
@@ -968,15 +997,15 @@
 
 print(log)
 ```
 
 ### Create IssuingWithdrawals
 
 You can create withdrawals to send cash back from your Issuing balance to your Banking balance
-by using the Withdrawal resource.
+by using the IssuingWithdrawal resource.
 
 ```python
 import starkinfra
 
 withdrawal = starkinfra.issuingwithdrawal.create(
     withdrawal=starkinfra.IssuingWithdrawal(
         amount=10000,
@@ -1987,15 +2016,15 @@
     uuids=["5ddde28043a245c2848b08cf315effa2"]
 )
 
 for brcode in brcodes:
     print(brcode)
 ```
 
-### Get a StaticBrcodes
+### Get a StaticBrcode
 
 After its creation, information on a StaticBrcode may be retrieved by its UUID.
 
 ```python
 import starkinfra
 
 brcode = starkinfra.staticbrcode.get("5ddde28043a245c2848b08cf315effa2")
@@ -2058,15 +2087,15 @@
 brcode = starkinfra.dynamicbrcode.get("ac7caa14e601461dbd6b12bf7e4cc48e")
 
 print(brcode)
 ```
 
 ### Verify a DynamicBrcode read
 
-When a DynamicBrcode is read by your user, a GET request will be made to the your regitered URL to 
+When a DynamicBrcode is read by your user, a GET request will be made to your registered URL to 
 retrieve additional information needed to complete the transaction.
 Use this method to verify the authenticity of a GET request received at your registered endpoint.
 If the provided digital signature does not check out with the StarkInfra public key, a stark.exception.InvalidSignatureException will be raised.
 
 ```python
 import starkinfra
 
@@ -2151,14 +2180,15 @@
         cashier_bank_code=invoice.cashier_bank_code,
         cash_amount=invoice.cash_amount
     )
 )
 ```
 
 ## Create BrcodePreviews
+
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
@@ -2186,14 +2216,15 @@
  3. (Optional) Create a [Credit Simulation](#create-creditpreviews) 
 with the desired installment plan to display information for the credit receiver
  4. Create a [Credit Note](#create-creditnotes)
 with the desired installment plan
 
 
 ### Create CreditNotes
+
 For lending operations, you can create a CreditNote to generate a CCB contract.
 
 Note that you must have recently created an identity check for that same Tax ID before
 being able to create a credit operation for them.
 
 ```python
 import starkinfra
@@ -2290,15 +2321,15 @@
 note = starkinfra.creditnote.cancel("5155165527080960")
 
 print(note)
 ```
   
 ### Query CreditNote logs
 
-You can query credit note logs to better understand credit note life cycles. 
+You can query credit note logs to better understand CreditNote life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
 
 logs = starkinfra.creditnote.log.query(
     limit=50, 
@@ -2319,14 +2350,15 @@
 
 log = starkinfra.creditnote.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create CreditPreviews
+
 You can preview a credit operation before creating them (Currently we only have CreditNote / CCB previews):
 
 ```python
 import starkinfra
 from datetime import date
 
 previews = starkinfra.creditpreview.create([
@@ -2404,26 +2436,119 @@
 
 for preview in previews:
     print(preview)
 ```
 
 **Note**: Instead of using CreditPreview objects, you can also pass each element in dictionary format
 
+### Create CreditHolmes
+
+Before you request a credit operation, you may want to check previous credit operations
+the credit receiver has taken.
+
+For that, open up a CreditHolmes investigation to receive information on all debts and credit
+operations registered for that individual or company inside the Central Bank's SCR.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.create([
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-09"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-08"
+    ),
+    starkinfra.CreditHolmes(
+        tax_id="123.456.789-00",
+        competence="2022-07"
+    )
+])
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Query CreditHolmes
+
+You can query multiple credit holmes according to filters.
+
+```python
+import starkinfra
+from datetime import date
+
+holmes = starkinfra.creditholmes.query(
+    after=date(2022, 6, 1),
+    before=date(2022, 10, 30),
+    status="success"
+)
+
+for sherlock in holmes:
+    print(sherlock)
+```
+
+### Get a CreditHolmes
+
+After its creation, information on a credit holmes may be retrieved by its id.
+
+```python
+import starkinfra
+
+holmes = starkinfra.creditholmes.get("5657818854064128")
+
+print(holmes)
+```
+
+### Query CreditHolmes logs
+
+You can query credit holmes logs to better understand their life cycles. 
+
+```python
+import starkinfra
+from datetime import date
+
+logs = starkinfra.creditholmes.log.query(
+    limit=50, 
+    ids=["5729405850615808"],
+    after=date(2022, 1, 1),
+    before=date(2022, 1, 20),
+    types=["created"]
+)
+
+for log in logs:
+    print(log)
+```
+
+### Get a CreditHolmes log
+
+You can also get a specific log by its id.
+
+```python
+import starkinfra
+
+log = starkinfra.creditholmes.log.get("5155165527080960")
+
+print(log)
+```
+
 ## Identity
 Several operations, especially credit ones, require that the identity
 of a person or business is validated beforehand.
 
 Identities are validated according to the following sequence:
 1. The Identity resource is created for a specific Tax ID
 2. Documents are attached to the Identity resource
 3. The Identity resource is updated to indicate that all documents have been attached
 4. The Identity is sent for validation and returns a webhook notification to reflect
 the success or failure of the operation
 
 ### Create IndividualIdentities
+
 You can create an IndividualIdentity to validate a document of a natural person
 
 ```python
 import starkinfra
 
 identities = starkinfra.individualidentity.create([
     starkinfra.IndividualIdentity(
@@ -2481,28 +2606,26 @@
 identity = starkinfra.individualidentity.update("5155165527080960", status="processing")
 
 print(identity)
 ```
 
 **Note**: Before sending your individual identity to validation by patching its status, you must send all the required documents using the create method of the CreditDocument resource. Note that you must reference the individual identity in the create method of the CreditDocument resource by its id.
 
-
 ### Cancel an IndividualIdentity
 
 You can cancel an individual identity before updating its status to processing.
 
-
 ```python
 import starkinfra
 
 identity = starkinfra.individualidentity.cancel("5155165527080960")
 
 print(identity)
 ```
-  
+
 ### Query IndividualIdentity logs
 
 You can query individual identity logs to better understand individual identity life cycles. 
 
 ```python
 import starkinfra
 from datetime import date
@@ -2526,14 +2649,15 @@
 
 log = starkinfra.individualidentity.log.get("5155165527080960")
 
 print(log)
 ```
 
 ### Create IndividualDocuments
+
 You can create an individual document to attach images of documents to a specific individual Identity.
 You must reference the desired individual identity by its id.
 
 ```python
 import starkinfra
 
 documents = starkinfra.individualdocument.create([
@@ -2559,15 +2683,15 @@
 
 for document in documents:
     print(document)
 ```
 
 **Note**: Instead of using IndividualDocument objects, you can also pass each element in dictionary format
 
-### Query IndividualDocument
+### Query IndividualDocuments
 
 You can query multiple individual documents according to filters.
 
 ```python
 import starkinfra
 from datetime import date
 
@@ -2642,42 +2766,42 @@
         "pix-request.in", "pix-request.out", "pix-reversal.in", "pix-reversal.out", "pix-claim", "pix-key", "pix-chargeback", "pix-infraction",
     ],
 )
 
 print(webhook)
 ```
 
-### Query webhooks
+### Query webhook subscriptions
 
-To search for registered webhooks, run:
+To search for registered webhook subscriptions, run:
 
 ```python
 import starkinfra
 
 webhooks = starkinfra.webhook.query()
 
 for webhook in webhooks:
     print(webhook)
 ```
 
-### Get a webhook
+### Get a webhook subscription
 
-You can get a specific webhook by its id.
+You can get a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.get("1082736198236817")
 
 print(webhook)
 ```
 
-### Delete a webhook
+### Delete a webhook subscription
 
-You can also delete a specific webhook by its id.
+You can also delete a specific webhook subscription by its id.
 
 ```python
 import starkinfra
 
 webhook = starkinfra.webhook.delete("1082736198236817")
 
 print(webhook)
```

### Comparing `starkinfra-0.6.0/starkinfra.egg-info/SOURCES.txt` & `starkinfra-0.7.0/starkinfra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 starkinfra.egg-info/dependency_links.txt
 starkinfra.egg-info/requires.txt
 starkinfra.egg-info/top_level.txt
 starkinfra/brcodepreview/__brcodepreview.py
 starkinfra/brcodepreview/__init__.py
 starkinfra/cardmethod/__cardmethod.py
 starkinfra/cardmethod/__init__.py
+starkinfra/creditholmes/__creditholmes.py
+starkinfra/creditholmes/__init__.py
+starkinfra/creditholmes/log/__init__.py
+starkinfra/creditholmes/log/__log.py
 starkinfra/creditnote/__creditnote.py
 starkinfra/creditnote/__init__.py
 starkinfra/creditnote/__transfer.py
 starkinfra/creditnote/invoice/__description.py
 starkinfra/creditnote/invoice/__discount.py
 starkinfra/creditnote/invoice/__init__.py
 starkinfra/creditnote/invoice/__invoice.py
@@ -44,14 +48,16 @@
 starkinfra/issuingbalance/__issuingbalance.py
 starkinfra/issuingcard/__init__.py
 starkinfra/issuingcard/__issuingcard.py
 starkinfra/issuingcard/log/__init__.py
 starkinfra/issuingcard/log/__log.py
 starkinfra/issuingdesign/__init__.py
 starkinfra/issuingdesign/__issuingdesign.py
+starkinfra/issuingembossingkit/__init__.py
+starkinfra/issuingembossingkit/__issuingembossingkit.py
 starkinfra/issuingembossingrequest/__init__.py
 starkinfra/issuingembossingrequest/__issuingembossingrequest.py
 starkinfra/issuingembossingrequest/log/__init__.py
 starkinfra/issuingembossingrequest/log/__log.py
 starkinfra/issuingholder/__init__.py
 starkinfra/issuingholder/__issuingholder.py
 starkinfra/issuingholder/log/__init__.py
```


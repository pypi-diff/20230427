# Comparing `tmp/cnswd-5.0.0.tar.gz` & `tmp/cnswd-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnswd-5.0.0.tar", last modified: Thu Apr 27 07:50:23 2023, max compression
+gzip compressed data, was "cnswd-5.0.1.tar", last modified: Thu Apr 27 08:10:44 2023, max compression
```

## Comparing `cnswd-5.0.0.tar` & `cnswd-5.0.1.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.846163 cnswd-5.0.0/
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1060 2023-04-27 06:09:28.000000 cnswd-5.0.0/LICENSE
--rw-r--r--   0 ldf       (1000) ldf       (1000)      319 2023-04-27 07:50:23.846163 cnswd-5.0.0/PKG-INFO
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5403 2023-04-27 06:09:28.000000 cnswd-5.0.0/README.md
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.826163 cnswd-5.0.0/cnswd/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      526 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/_exceptions.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2389 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/_seleniumwire.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.826163 cnswd-5.0.0/cnswd/cninfo/
--rw-r--r--   0 ldf       (1000) ldf       (1000)      316 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     8923 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/base_driver.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6319 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/classify_tree.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2344 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/config.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1635 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/css.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)    10736 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/databrowser.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)    11217 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/ops.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3944 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/ts.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2780 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/cninfo/utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      209 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/connect.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      127 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/mongodb.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/cnswd/scripts/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1261 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/base.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2146 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/category.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      717 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/classify.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4999 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/cninfo.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      759 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/cninfo_meta.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4113 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/cninfo_yypl.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5255 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/command.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3074 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/disclosure.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      638 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/index_codes.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1665 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/ptrepack.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2146 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sgpx.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2524 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sina_margin.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1437 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sina_news.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3626 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sina_quote.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2773 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sina_quote_index.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2706 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sina_tzpj.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      250 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/sw_class.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1032 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/tct_gn.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1609 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/tct_minutely.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2429 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/ths_gn.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2116 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/ths_news.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3252 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/trading_calendar.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1580 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/trading_codes.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      576 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/treasury.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4257 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_cjmx.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4490 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_cwbg.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2480 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_fhpg.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3161 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_gszl.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2435 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_index.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2730 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_quote.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1347 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_quote_index.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2774 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_stock.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4079 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_yjyg.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4820 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/wy_zycwzb.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4208 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/yahoo.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2815 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/yahoo_fields.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      452 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/scripts/yahoo_utils.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/cnswd/setting/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/setting/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      577 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/setting/config.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     9697 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/setting/constants.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/cnswd/ths/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/ths/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3165 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/ths/base.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4271 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/ths/financial_analysis.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6724 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/ths/hq.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4088 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/ths/stock.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/cnswd/utils/
--rw-r--r--   0 ldf       (1000) ldf       (1000)      519 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2735 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/cache.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      565 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/db_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     8021 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/dt_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      747 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/log_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1242 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/loop_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1292 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/path_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3447 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/pd_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      737 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/proc_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4656 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/temp.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      479 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/temp_utils.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2985 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/utils/tools.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/cnswd/websource/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     3134 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/base.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4933 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/disclosures.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5687 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/nbsc.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)    15725 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/sina.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4014 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/sina_news.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     8690 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/sse.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1185 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/sw.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1878 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/szse.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4972 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/tencent.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5342 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/ths.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5288 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/ths_base.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1916 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/ths_news.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5359 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/treasuries.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)    19700 2023-04-27 06:09:28.000000 cnswd-5.0.0/cnswd/websource/wy.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.826163 cnswd-5.0.0/cnswd.egg-info/
--rw-r--r--   0 ldf       (1000) ldf       (1000)      319 2023-04-27 07:50:23.000000 cnswd-5.0.0/cnswd.egg-info/PKG-INFO
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2846 2023-04-27 07:50:23.000000 cnswd-5.0.0/cnswd.egg-info/SOURCES.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-04-27 07:50:23.000000 cnswd-5.0.0/cnswd.egg-info/dependency_links.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)       54 2023-04-27 07:50:23.000000 cnswd-5.0.0/cnswd.egg-info/entry_points.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)       14 2023-04-27 07:50:23.000000 cnswd-5.0.0/cnswd.egg-info/top_level.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)       38 2023-04-27 07:50:23.846163 cnswd-5.0.0/setup.cfg
--rw-r--r--   0 ldf       (1000) ldf       (1000)      628 2023-04-27 06:09:28.000000 cnswd-5.0.0/setup.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/testing/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      624 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/conftest.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/testing/test_cninfo/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_cninfo/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4799 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_cninfo/test_ad.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1849 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_cninfo/test_fast.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      438 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_cninfo/test_make_headless_browser.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      420 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_cninfo/test_ts.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/testing/test_uitls/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_uitls/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1388 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_uitls/test_ensure_dtypes.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     9712 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_uitls/test_next_update_time.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 07:50:23.836163 cnswd-5.0.0/testing/test_websource/
--rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_websource/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      207 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_websource/test_tencent.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      800 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_websource/test_treasury.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      838 2023-04-27 06:09:28.000000 cnswd-5.0.0/testing/test_websource/test_wy.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1060 2023-04-27 06:09:28.000000 cnswd-5.0.1/LICENSE
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      319 2023-04-27 08:10:44.056152 cnswd-5.0.1/PKG-INFO
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5403 2023-04-27 06:09:28.000000 cnswd-5.0.1/README.md
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.046152 cnswd-5.0.1/cnswd/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      526 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/_exceptions.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2389 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/_seleniumwire.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.046152 cnswd-5.0.1/cnswd/cninfo/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      316 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     8923 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/base_driver.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     6319 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/classify_tree.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2344 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/config.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1635 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/css.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    10736 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/databrowser.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    11217 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/ops.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3944 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/ts.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2780 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/cninfo/utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      209 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/connect.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      127 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/mongodb.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/cnswd/scripts/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1261 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/base.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2146 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/category.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      717 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/classify.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4999 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/cninfo.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      759 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/cninfo_meta.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4113 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/cninfo_yypl.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5255 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/command.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3074 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/disclosure.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      638 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/index_codes.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1665 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/ptrepack.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2146 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sgpx.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2524 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sina_margin.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1437 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sina_news.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3626 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sina_quote.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2773 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sina_quote_index.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2706 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sina_tzpj.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      250 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/sw_class.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1032 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/tct_gn.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1609 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/tct_minutely.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2429 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/ths_gn.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2116 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/ths_news.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3252 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/trading_calendar.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1580 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/trading_codes.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      576 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/treasury.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4257 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_cjmx.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4490 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_cwbg.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2480 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_fhpg.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3161 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_gszl.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2435 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_index.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2730 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_quote.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1347 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_quote_index.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2774 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_stock.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4079 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_yjyg.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4820 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/wy_zycwzb.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4208 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/yahoo.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2815 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/yahoo_fields.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      452 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/scripts/yahoo_utils.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/cnswd/setting/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/setting/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      577 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/setting/config.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     9697 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/setting/constants.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/cnswd/ths/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/ths/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3165 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/ths/base.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4271 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/ths/financial_analysis.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     6724 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/ths/hq.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4088 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/ths/stock.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/cnswd/utils/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      519 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2735 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/cache.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      565 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/db_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     8021 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/dt_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      747 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/log_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1242 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/loop_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1292 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/path_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3447 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/pd_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      737 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/proc_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4656 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/temp.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      479 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/temp_utils.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2985 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/utils/tools.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/cnswd/websource/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     3134 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/base.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4933 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/disclosures.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5687 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/nbsc.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    15725 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/sina.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4014 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/sina_news.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     8690 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/sse.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1185 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/sw.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1878 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/szse.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4972 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/tencent.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5342 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/ths.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5288 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/ths_base.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1916 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/ths_news.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5359 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/treasuries.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    19700 2023-04-27 06:09:28.000000 cnswd-5.0.1/cnswd/websource/wy.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.046152 cnswd-5.0.1/cnswd.egg-info/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      319 2023-04-27 08:10:44.000000 cnswd-5.0.1/cnswd.egg-info/PKG-INFO
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2861 2023-04-27 08:10:44.000000 cnswd-5.0.1/cnswd.egg-info/SOURCES.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-04-27 08:10:44.000000 cnswd-5.0.1/cnswd.egg-info/dependency_links.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       54 2023-04-27 08:10:44.000000 cnswd-5.0.1/cnswd.egg-info/entry_points.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       14 2023-04-27 08:10:44.000000 cnswd-5.0.1/cnswd.egg-info/top_level.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      115 2023-04-27 08:03:47.000000 cnswd-5.0.1/pyproject.toml
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       38 2023-04-27 08:10:44.056152 cnswd-5.0.1/setup.cfg
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      628 2023-04-27 08:10:36.000000 cnswd-5.0.1/setup.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/testing/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      624 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/conftest.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/testing/test_cninfo/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_cninfo/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4799 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_cninfo/test_ad.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1849 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_cninfo/test_fast.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      438 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_cninfo/test_make_headless_browser.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      420 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_cninfo/test_ts.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/testing/test_uitls/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_uitls/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1388 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_uitls/test_ensure_dtypes.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     9712 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_uitls/test_next_update_time.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:10:44.056152 cnswd-5.0.1/testing/test_websource/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        0 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_websource/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      207 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_websource/test_tencent.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      800 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_websource/test_treasury.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      838 2023-04-27 06:09:28.000000 cnswd-5.0.1/testing/test_websource/test_wy.py
```

### Comparing `cnswd-5.0.0/LICENSE` & `cnswd-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/README.md` & `cnswd-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/_exceptions.py` & `cnswd-5.0.1/cnswd/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/_seleniumwire.py` & `cnswd-5.0.1/cnswd/_seleniumwire.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/base_driver.py` & `cnswd-5.0.1/cnswd/cninfo/base_driver.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/classify_tree.py` & `cnswd-5.0.1/cnswd/cninfo/classify_tree.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/config.py` & `cnswd-5.0.1/cnswd/cninfo/config.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/css.py` & `cnswd-5.0.1/cnswd/cninfo/css.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/databrowser.py` & `cnswd-5.0.1/cnswd/cninfo/databrowser.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/ops.py` & `cnswd-5.0.1/cnswd/cninfo/ops.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/ts.py` & `cnswd-5.0.1/cnswd/cninfo/ts.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/cninfo/utils.py` & `cnswd-5.0.1/cnswd/cninfo/utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/base.py` & `cnswd-5.0.1/cnswd/scripts/base.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/category.py` & `cnswd-5.0.1/cnswd/scripts/category.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/classify.py` & `cnswd-5.0.1/cnswd/scripts/classify.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/cninfo.py` & `cnswd-5.0.1/cnswd/scripts/cninfo.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/cninfo_meta.py` & `cnswd-5.0.1/cnswd/scripts/cninfo_meta.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/cninfo_yypl.py` & `cnswd-5.0.1/cnswd/scripts/cninfo_yypl.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/command.py` & `cnswd-5.0.1/cnswd/scripts/command.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/disclosure.py` & `cnswd-5.0.1/cnswd/scripts/disclosure.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/index_codes.py` & `cnswd-5.0.1/cnswd/scripts/index_codes.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/ptrepack.py` & `cnswd-5.0.1/cnswd/scripts/ptrepack.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sgpx.py` & `cnswd-5.0.1/cnswd/scripts/sgpx.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sina_margin.py` & `cnswd-5.0.1/cnswd/scripts/sina_margin.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sina_news.py` & `cnswd-5.0.1/cnswd/scripts/sina_news.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sina_quote.py` & `cnswd-5.0.1/cnswd/scripts/sina_quote.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sina_quote_index.py` & `cnswd-5.0.1/cnswd/scripts/sina_quote_index.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/sina_tzpj.py` & `cnswd-5.0.1/cnswd/scripts/sina_tzpj.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/tct_gn.py` & `cnswd-5.0.1/cnswd/scripts/tct_gn.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/tct_minutely.py` & `cnswd-5.0.1/cnswd/scripts/tct_minutely.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/ths_gn.py` & `cnswd-5.0.1/cnswd/scripts/ths_gn.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/ths_news.py` & `cnswd-5.0.1/cnswd/scripts/ths_news.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/trading_calendar.py` & `cnswd-5.0.1/cnswd/scripts/trading_calendar.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/trading_codes.py` & `cnswd-5.0.1/cnswd/scripts/trading_codes.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/treasury.py` & `cnswd-5.0.1/cnswd/scripts/treasury.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_cjmx.py` & `cnswd-5.0.1/cnswd/scripts/wy_cjmx.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_cwbg.py` & `cnswd-5.0.1/cnswd/scripts/wy_cwbg.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_fhpg.py` & `cnswd-5.0.1/cnswd/scripts/wy_fhpg.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_gszl.py` & `cnswd-5.0.1/cnswd/scripts/wy_gszl.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_index.py` & `cnswd-5.0.1/cnswd/scripts/wy_index.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_quote.py` & `cnswd-5.0.1/cnswd/scripts/wy_quote.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_quote_index.py` & `cnswd-5.0.1/cnswd/scripts/wy_quote_index.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_stock.py` & `cnswd-5.0.1/cnswd/scripts/wy_stock.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_yjyg.py` & `cnswd-5.0.1/cnswd/scripts/wy_yjyg.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/wy_zycwzb.py` & `cnswd-5.0.1/cnswd/scripts/wy_zycwzb.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/yahoo.py` & `cnswd-5.0.1/cnswd/scripts/yahoo.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/scripts/yahoo_fields.py` & `cnswd-5.0.1/cnswd/scripts/yahoo_fields.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/setting/config.py` & `cnswd-5.0.1/cnswd/setting/config.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/setting/constants.py` & `cnswd-5.0.1/cnswd/setting/constants.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/ths/base.py` & `cnswd-5.0.1/cnswd/ths/base.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/ths/financial_analysis.py` & `cnswd-5.0.1/cnswd/ths/financial_analysis.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/ths/hq.py` & `cnswd-5.0.1/cnswd/ths/hq.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/ths/stock.py` & `cnswd-5.0.1/cnswd/ths/stock.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/__init__.py` & `cnswd-5.0.1/cnswd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/cache.py` & `cnswd-5.0.1/cnswd/utils/cache.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/db_utils.py` & `cnswd-5.0.1/cnswd/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/dt_utils.py` & `cnswd-5.0.1/cnswd/utils/dt_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/log_utils.py` & `cnswd-5.0.1/cnswd/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/loop_utils.py` & `cnswd-5.0.1/cnswd/utils/loop_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/path_utils.py` & `cnswd-5.0.1/cnswd/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/pd_utils.py` & `cnswd-5.0.1/cnswd/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/proc_utils.py` & `cnswd-5.0.1/cnswd/utils/proc_utils.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/temp.py` & `cnswd-5.0.1/cnswd/utils/temp.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/utils/tools.py` & `cnswd-5.0.1/cnswd/utils/tools.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/base.py` & `cnswd-5.0.1/cnswd/websource/base.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/disclosures.py` & `cnswd-5.0.1/cnswd/websource/disclosures.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/nbsc.py` & `cnswd-5.0.1/cnswd/websource/nbsc.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/sina.py` & `cnswd-5.0.1/cnswd/websource/sina.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/sina_news.py` & `cnswd-5.0.1/cnswd/websource/sina_news.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/sse.py` & `cnswd-5.0.1/cnswd/websource/sse.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/sw.py` & `cnswd-5.0.1/cnswd/websource/sw.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/szse.py` & `cnswd-5.0.1/cnswd/websource/szse.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/tencent.py` & `cnswd-5.0.1/cnswd/websource/tencent.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/ths.py` & `cnswd-5.0.1/cnswd/websource/ths.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/ths_base.py` & `cnswd-5.0.1/cnswd/websource/ths_base.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/ths_news.py` & `cnswd-5.0.1/cnswd/websource/ths_news.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/treasuries.py` & `cnswd-5.0.1/cnswd/websource/treasuries.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd/websource/wy.py` & `cnswd-5.0.1/cnswd/websource/wy.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/cnswd.egg-info/SOURCES.txt` & `cnswd-5.0.1/cnswd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 cnswd/__init__.py
 cnswd/_exceptions.py
 cnswd/_seleniumwire.py
 cnswd/connect.py
 cnswd/mongodb.py
 cnswd.egg-info/PKG-INFO
```

### Comparing `cnswd-5.0.0/setup.py` & `cnswd-5.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name="cnswd",
-    version="5.0.0",
+    version="5.0.1",
     packages=find_packages(),
     long_description="""
     股票网络数据工具包
     """,
     tests_require=["pytest", "parameterized"],
     include_package_data=True,
     entry_points={
-        'console_scripts': [
-            'stock = cnswd.scripts.command:stock',
+        "console_scripts": [
+            "stock = cnswd.scripts.command:stock",
         ],
     },
     author="LDF",
     author_email="liu.dengfeng@hotmail.com",
     description="Utilities for fetching Chinese stock webpage data",
     license="https://github.com/liudengfeng/cnswd/blob/master/LICENSE",
     keywords="china stock data tools",
```

### Comparing `cnswd-5.0.0/testing/conftest.py` & `cnswd-5.0.1/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_cninfo/test_ad.py` & `cnswd-5.0.1/testing/test_cninfo/test_ad.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_cninfo/test_fast.py` & `cnswd-5.0.1/testing/test_cninfo/test_fast.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_uitls/test_ensure_dtypes.py` & `cnswd-5.0.1/testing/test_uitls/test_ensure_dtypes.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_uitls/test_next_update_time.py` & `cnswd-5.0.1/testing/test_uitls/test_next_update_time.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_websource/test_treasury.py` & `cnswd-5.0.1/testing/test_websource/test_treasury.py`

 * *Files identical despite different names*

### Comparing `cnswd-5.0.0/testing/test_websource/test_wy.py` & `cnswd-5.0.1/testing/test_websource/test_wy.py`

 * *Files identical despite different names*


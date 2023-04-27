# Comparing `tmp/minium-1.3.dev2.tar.gz` & `tmp/minium-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minium-1.3.dev2.tar", last modified: Tue Jan  3 14:31:03 2023, max compression
+gzip compressed data, was "dist/minium-1.4.0.tar", last modified: Thu Apr 27 03:03:31 2023, max compression
```

## Comparing `minium-1.3.dev2.tar` & `minium-1.4.0.tar`

### file list

```diff
@@ -1,273 +1,277 @@
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.520075 minium-1.3.dev2/
--rw-r--r--   0 yopofeng   (501) staff       (20)      599 2023-01-03 14:31:03.519839 minium-1.3.dev2/PKG-INFO
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.446773 minium-1.3.dev2/minium/
--rw-r--r--   0 yopofeng   (501) staff       (20)      948 2023-01-03 14:30:09.000000 minium-1.3.dev2/minium/__init__.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.451306 minium-1.3.dev2/minium/framework/
--rw-r--r--   0 yopofeng   (501) staff       (20)       58 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    16488 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/assertbase.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1587 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/casedump.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     7702 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/caseinspect.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.451555 minium-1.3.dev2/minium/framework/dist/
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.451836 minium-1.3.dev2/minium/framework/dist/css/
--rw-r--r--   0 yopofeng   (501) staff       (20)      437 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/dist/css/app.87891bf0.css
--rw-r--r--   0 yopofeng   (501) staff       (20)   240799 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/dist/css/chunk-vendors.52eeca6f.css
--rw-r--r--   0 yopofeng   (501) staff       (20)     2108 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/dist/favicon.ico
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.452322 minium-1.3.dev2/minium/framework/dist/fonts/
--rw-r--r--   0 yopofeng   (501) staff       (20)    28200 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/dist/fonts/element-icons.535877f5.woff
--rw-r--r--   0 yopofeng   (501) staff       (20)    55956 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/dist/fonts/element-icons.732389de.ttf
--rw-r--r--   0 yopofeng   (501) staff       (20)      847 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/dist/index.html
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.452643 minium-1.3.dev2/minium/framework/dist/js/
--rw-r--r--   0 yopofeng   (501) staff       (20)    17537 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/dist/js/app.544bedf4.js
--rw-r--r--   0 yopofeng   (501) staff       (20)  1346000 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/dist/js/chunk-vendors.22ed339a.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     3573 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/errorReport.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1677 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/exception.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.453782 minium-1.3.dev2/minium/framework/libs/
--rw-r--r--   0 yopofeng   (501) staff       (20)        0 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/libs/__init__.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.454434 minium-1.3.dev2/minium/framework/libs/tgit/
--rw-r--r--   0 yopofeng   (501) staff       (20)      152 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/libs/tgit/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1007 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/libs/tgit/auth.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    97301 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/libs/tgit/client.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.455160 minium-1.3.dev2/minium/framework/libs/unittest/
--rw-r--r--   0 yopofeng   (501) staff       (20)      243 2023-01-03 14:30:09.000000 minium-1.3.dev2/minium/framework/libs/unittest/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     8084 2023-01-03 14:30:09.000000 minium-1.3.dev2/minium/framework/libs/unittest/case.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     5286 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/libs/unittest/suite.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    19830 2022-12-14 07:39:51.000000 minium-1.3.dev2/minium/framework/loader.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     9617 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/logcolor.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     5162 2022-12-14 07:39:51.000000 minium-1.3.dev2/minium/framework/miniconfig.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3427 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/miniddt.py
--rw-r--r--   0 yopofeng   (501) staff       (20)       22 2023-01-03 14:26:58.000000 minium-1.3.dev2/minium/framework/minidoctor.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1207 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/minilimit.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      832 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/miniprogram.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     6669 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/miniresult.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      608 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/miniretry.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3198 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/minisuite.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    24938 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/framework/minitest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    16050 2023-01-03 14:26:46.000000 minium-1.3.dev2/minium/framework/report.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3318 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/framework/session.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.455464 minium-1.3.dev2/minium/framework/tools/
--rw-r--r--   0 yopofeng   (501) staff       (20)       54 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/tools/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     2716 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/framework/tools/report_issue.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3974 2022-12-14 07:39:51.000000 minium-1.3.dev2/minium/framework/wording.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.455887 minium-1.3.dev2/minium/miniprogram/
--rw-r--r--   0 yopofeng   (501) staff       (20)      624 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/miniprogram/__init__.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.461631 minium-1.3.dev2/minium/miniprogram/base_driver/
--rw-r--r--   0 yopofeng   (501) staff       (20)      191 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/miniprogram/base_driver/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    33630 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/app.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3465 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/callback.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    12764 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/connection.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    44317 2022-11-07 03:37:28.000000 minium-1.3.dev2/minium/miniprogram/base_driver/element.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1615 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/minium.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     5400 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/minium_log.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    13133 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/minium_object.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    22417 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/miniprogram/base_driver/page.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      771 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/miniprogram/base_driver/prefixer.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      135 2023-01-03 14:31:01.000000 minium-1.3.dev2/minium/miniprogram/base_driver/version.json
--rw-r--r--   0 yopofeng   (501) staff       (20)      263 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/miniprogram/base_driver/waiter.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     6692 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/miniprogram/qq_minium.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    34857 2022-12-14 07:39:51.000000 minium-1.3.dev2/minium/miniprogram/wx_minium.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.461922 minium-1.3.dev2/minium/native/
--rw-r--r--   0 yopofeng   (501) staff       (20)     3218 2022-12-14 07:39:51.000000 minium-1.3.dev2/minium/native/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      344 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/exception.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.462210 minium-1.3.dev2/minium/native/lib/
--rw-r--r--   0 yopofeng   (501) staff       (20)       58 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/lib/__init__.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.462361 minium-1.3.dev2/minium/native/lib/android_base/
--rw-r--r--   0 yopofeng   (501) staff       (20)     1012 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/android_base/__init__.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.464716 minium-1.3.dev2/minium/native/lib/at/
--rw-r--r--   0 yopofeng   (501) staff       (20)     4087 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1755 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/apkapi.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     5609 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/atproxy.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.468098 minium-1.3.dev2/minium/native/lib/at/bin/
--rw-r--r--   0 yopofeng   (501) staff       (20)  3566862 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/bin/AtServer.apk
--rw-r--r--   0 yopofeng   (501) staff       (20)    95449 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/bin/AtStub.jar
--rw-r--r--   0 yopofeng   (501) staff       (20)     3222 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/command_line.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.471063 minium-1.3.dev2/minium/native/lib/at/core/
--rw-r--r--   0 yopofeng   (501) staff       (20)       37 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      951 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/accesshelper.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    46986 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/adbwrap.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    10763 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/basedriver.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    15919 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/case_repair_adapter.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      624 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/config.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    31731 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/element.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      669 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/exceptions.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    18740 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/javadriver.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3620 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/resguard.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.471453 minium-1.3.dev2/minium/native/lib/at/core/stf/
--rw-r--r--   0 yopofeng   (501) staff       (20)       56 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/stf/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1662 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/stf/mincap.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     5507 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/stf/minitouch.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    11600 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/uidevice.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    17965 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/uixml.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     2711 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/core/websocketcli.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     2186 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/eventmonitor.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1087 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/hook.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     8495 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/jlogcat.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    36015 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/keycode.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     9492 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/perfcollector.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.476924 minium-1.3.dev2/minium/native/lib/at/tests/
--rw-r--r--   0 yopofeng   (501) staff       (20)      690 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/AtEvent.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      326 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/AtSocket.py
--rw-r--r--   0 yopofeng   (501) staff       (20)       38 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      480 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/adbtest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      490 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/airtesttest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    10434 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/atdevicetest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      474 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/attestbase.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1022 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/drivertest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1768 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/elementtest.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.480374 minium-1.3.dev2/minium/native/lib/at/tests/images/
--rw-r--r--   0 yopofeng   (501) staff       (20)     7525 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/tests/images/1.jpg
--rw-r--r--   0 yopofeng   (501) staff       (20)     4388 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/tests/images/2.jpg
--rw-r--r--   0 yopofeng   (501) staff       (20)    80712 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/tests/images/image.jpg
--rw-r--r--   0 yopofeng   (501) staff       (20)      493 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/javadrivertest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      480 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/minicap_test.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      375 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/minitest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      843 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/minitouch_test.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      792 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/u2test.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1797 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/uixmltest.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      493 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/vs_test.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      989 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/tests/webdrivertest.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.482074 minium-1.3.dev2/minium/native/lib/at/utils/
--rw-r--r--   0 yopofeng   (501) staff       (20)       37 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     4896 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/apkinfo.py
--rw-r--r--   0 yopofeng   (501) staff       (20)   105609 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/axmlparser.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    27360 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/axmlparser3.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      526 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/commonhelper.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     8332 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/decorator.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      257 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/magic.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     2457 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/nbsp.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1435 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/utils/threadhelper.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.486282 minium-1.3.dev2/minium/native/lib/at/vision/
--rw-r--r--   0 yopofeng   (501) staff       (20)       56 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/vision/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      394 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/vision/template_match.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.488815 minium-1.3.dev2/minium/native/lib/at/webdriver/
--rw-r--r--   0 yopofeng   (501) staff       (20)       72 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    15310 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/driver.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      425 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/error.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1376 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/jsapi.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1519 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/miniapp.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    18973 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/stub.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      682 2022-04-15 13:12:21.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/tabdescription.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    13005 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/tabwebsocket.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     8904 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/webelement.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1638 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/webhelper.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1399 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/webdriver/wspools.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.489184 minium-1.3.dev2/minium/native/lib/at/wechat/
--rw-r--r--   0 yopofeng   (501) staff       (20)       79 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/wechat/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1421 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/wechat/activtiy.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      144 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/wechat/appvars.py
--rw-r--r--   0 yopofeng   (501) staff       (20)       80 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/at/wsimp.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.489428 minium-1.3.dev2/minium/native/lib/case_repair_sdk/
--rw-r--r--   0 yopofeng   (501) staff       (20)     7663 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/case_repair_sdk/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     2816 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/case_repair_sdk/default_trace.py
--rw-r--r--   0 yopofeng   (501) staff       (20)       22 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/lib/requirements.txt
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.489824 minium-1.3.dev2/minium/native/lib/wda/
--rw-r--r--   0 yopofeng   (501) staff       (20)    40664 2022-04-15 13:39:51.000000 minium-1.3.dev2/minium/native/lib/wda/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1297 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/lib/wda/screenhelper.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     1421 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/lib/wda/xcui_element_types.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.490204 minium-1.3.dev2/minium/native/lib/wx_wda/
--rw-r--r--   0 yopofeng   (501) staff       (20)      399 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/lib/wx_wda/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    13188 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/lib/wx_wda/wdaUI.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    16169 2022-04-15 13:39:51.000000 minium-1.3.dev2/minium/native/lib/wx_wda/webDriverTool.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.490724 minium-1.3.dev2/minium/native/qq_native/
--rw-r--r--   0 yopofeng   (501) staff       (20)      118 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/qq_native/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     6435 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/qq_native/qandroidnative.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      804 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/qq_native/qbasenative.py
--rwxr-xr-x   0 yopofeng   (501) staff       (20)    16882 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/qq_native/qiosnative.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.491395 minium-1.3.dev2/minium/native/wx_native/
--rw-r--r--   0 yopofeng   (501) staff       (20)       23 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/native/wx_native/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    38142 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/wx_native/androidnative.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    22644 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/wx_native/basenative.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     7761 2023-01-03 14:30:09.000000 minium-1.3.dev2/minium/native/wx_native/idenative.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    34463 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/native/wx_native/iosnative.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.492214 minium-1.3.dev2/minium/utils/
--rw-r--r--   0 yopofeng   (501) staff       (20)        0 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/utils/__init__.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      221 2022-01-17 06:18:17.000000 minium-1.3.dev2/minium/utils/emitter.py
--rw-r--r--   0 yopofeng   (501) staff       (20)      230 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/utils/eventloop.py
--rw-r--r--   0 yopofeng   (501) staff       (20)     3873 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/utils/injectjs.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.446406 minium-1.3.dev2/minium/utils/js/
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.508333 minium-1.3.dev2/minium/utils/js/es5/
--rw-r--r--   0 yopofeng   (501) staff       (20)      221 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/addCloudCallMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      255 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/addNetworkMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      277 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/callContextMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)       72 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/checkInject.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      217 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/cleanCloudCallMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      200 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/cleanNetworkMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      535 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/createContext.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      340 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/editEditorText.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      231 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/evalMockChooseImage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      147 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/getAppConfig.js
--rw-r--r--   0 yopofeng   (501) staff       (20)    38266 2023-01-03 14:30:51.000000 minium-1.3.dev2/minium/utils/js/es5/helpers.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      297 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/hookCurrentPageMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      807 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/hookWxMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      120 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideHandleAuthModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      207 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideHandleMap.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      120 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideHandleModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      487 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockAuth.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      216 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockAuthSetting.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1170 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockChooseLocation.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1196 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockGetLocation.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      459 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockGetUserProfile.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      689 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockGetWeRunData.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1480 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      441 2023-01-03 14:30:49.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockShowActionSheet.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      434 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockShowModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      501 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/ideMockSubscribeMessage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     5184 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/mockChooseImage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1346 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/mockCloudCall.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     2681 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/mockNetwork.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1198 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/networkPannel.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      300 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/releaseHookWxMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1153 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/requestStack.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      285 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/startGetPerformance.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      198 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/stopGetPerformance.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     7144 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/testAsync.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      307 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/uuid.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      181 2023-01-03 14:30:50.000000 minium-1.3.dev2/minium/utils/js/es5/waitUtil.js
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.519574 minium-1.3.dev2/minium/utils/js/min/
--rw-r--r--   0 yopofeng   (501) staff       (20)      195 2023-01-03 14:30:59.000000 minium-1.3.dev2/minium/utils/js/min/addCloudCallMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      256 2023-01-03 14:30:58.000000 minium-1.3.dev2/minium/utils/js/min/addNetworkMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      198 2023-01-03 14:30:58.000000 minium-1.3.dev2/minium/utils/js/min/callContextMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)       73 2023-01-03 14:30:56.000000 minium-1.3.dev2/minium/utils/js/min/checkInject.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      191 2023-01-03 14:30:55.000000 minium-1.3.dev2/minium/utils/js/min/cleanCloudCallMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      201 2023-01-03 14:30:53.000000 minium-1.3.dev2/minium/utils/js/min/cleanNetworkMockRule.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      412 2023-01-03 14:31:01.000000 minium-1.3.dev2/minium/utils/js/min/createContext.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      306 2023-01-03 14:30:54.000000 minium-1.3.dev2/minium/utils/js/min/editEditorText.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      183 2023-01-03 14:30:54.000000 minium-1.3.dev2/minium/utils/js/min/evalMockChooseImage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      146 2023-01-03 14:30:56.000000 minium-1.3.dev2/minium/utils/js/min/getAppConfig.js
--rw-r--r--   0 yopofeng   (501) staff       (20)    38266 2023-01-03 14:30:57.000000 minium-1.3.dev2/minium/utils/js/min/helpers.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      209 2023-01-03 14:30:56.000000 minium-1.3.dev2/minium/utils/js/min/hookCurrentPageMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      664 2023-01-03 14:30:58.000000 minium-1.3.dev2/minium/utils/js/min/hookWxMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      121 2023-01-03 14:30:57.000000 minium-1.3.dev2/minium/utils/js/min/ideHandleAuthModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      202 2023-01-03 14:30:54.000000 minium-1.3.dev2/minium/utils/js/min/ideHandleMap.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      121 2023-01-03 14:30:54.000000 minium-1.3.dev2/minium/utils/js/min/ideHandleModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      470 2023-01-03 14:30:53.000000 minium-1.3.dev2/minium/utils/js/min/ideMockAuth.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      154 2023-01-03 14:30:59.000000 minium-1.3.dev2/minium/utils/js/min/ideMockAuthSetting.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1118 2023-01-03 14:30:55.000000 minium-1.3.dev2/minium/utils/js/min/ideMockChooseLocation.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1202 2023-01-03 14:30:52.000000 minium-1.3.dev2/minium/utils/js/min/ideMockGetLocation.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      428 2023-01-03 14:30:52.000000 minium-1.3.dev2/minium/utils/js/min/ideMockGetUserProfile.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      695 2023-01-03 14:31:00.000000 minium-1.3.dev2/minium/utils/js/min/ideMockGetWeRunData.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1413 2023-01-03 14:30:56.000000 minium-1.3.dev2/minium/utils/js/min/ideMockModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      417 2023-01-03 14:30:59.000000 minium-1.3.dev2/minium/utils/js/min/ideMockShowActionSheet.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      417 2023-01-03 14:31:00.000000 minium-1.3.dev2/minium/utils/js/min/ideMockShowModal.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      494 2023-01-03 14:31:00.000000 minium-1.3.dev2/minium/utils/js/min/ideMockSubscribeMessage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     4322 2023-01-03 14:30:55.000000 minium-1.3.dev2/minium/utils/js/min/mockChooseImage.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1163 2023-01-03 14:31:00.000000 minium-1.3.dev2/minium/utils/js/min/mockCloudCall.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     2170 2023-01-03 14:30:53.000000 minium-1.3.dev2/minium/utils/js/min/mockNetwork.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1175 2023-01-03 14:30:59.000000 minium-1.3.dev2/minium/utils/js/min/networkPannel.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      282 2023-01-03 14:30:58.000000 minium-1.3.dev2/minium/utils/js/min/releaseHookWxMethod.js
--rw-r--r--   0 yopofeng   (501) staff       (20)     1000 2023-01-03 14:30:51.000000 minium-1.3.dev2/minium/utils/js/min/requestStack.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      284 2023-01-03 14:30:52.000000 minium-1.3.dev2/minium/utils/js/min/startGetPerformance.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      199 2023-01-03 14:30:53.000000 minium-1.3.dev2/minium/utils/js/min/stopGetPerformance.js
--rw-r--r--   0 yopofeng   (501) staff       (20)       94 2023-01-03 14:30:52.000000 minium-1.3.dev2/minium/utils/js/min/testAsync.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      300 2023-01-03 14:30:57.000000 minium-1.3.dev2/minium/utils/js/min/uuid.js
--rw-r--r--   0 yopofeng   (501) staff       (20)       67 2023-01-03 14:30:52.000000 minium-1.3.dev2/minium/utils/js/min/waitUtil.js
--rw-r--r--   0 yopofeng   (501) staff       (20)      162 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/utils/platforms.py
--rw-r--r--   0 yopofeng   (501) staff       (20)    13284 2022-10-25 02:48:12.000000 minium-1.3.dev2/minium/utils/utils.py
-drwxr-xr-x   0 yopofeng   (501) staff       (20)        0 2023-01-03 14:31:03.447964 minium-1.3.dev2/minium.egg-info/
--rw-r--r--   0 yopofeng   (501) staff       (20)      599 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/PKG-INFO
--rw-r--r--   0 yopofeng   (501) staff       (20)     8910 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/SOURCES.txt
--rw-r--r--   0 yopofeng   (501) staff       (20)        1 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/dependency_links.txt
--rw-r--r--   0 yopofeng   (501) staff       (20)      239 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/entry_points.txt
--rw-r--r--   0 yopofeng   (501) staff       (20)      101 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/requires.txt
--rw-r--r--   0 yopofeng   (501) staff       (20)        7 2023-01-03 14:31:03.000000 minium-1.3.dev2/minium.egg-info/top_level.txt
--rw-r--r--   0 yopofeng   (501) staff       (20)       38 2023-01-03 14:31:03.520134 minium-1.3.dev2/setup.cfg
--rw-r--r--   0 yopofeng   (501) staff       (20)     2438 2023-01-03 14:30:20.000000 minium-1.3.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.364473 minium-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-04-27 03:03:31.364473 minium-1.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.0/minium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18583 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/assertbase.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.0/minium/framework/casedump.py
+-rw-r--r--   0 root         (0) root         (0)     7702 2022-11-07 03:36:55.000000 minium-1.4.0/minium/framework/caseinspect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/css/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/css/app.87891bf0.css
+-rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/css/chunk-vendors.52eeca6f.css
+-rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/js/app.544bedf4.js
+-rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/js/chunk-vendors.22ed339a.js
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-01-16 03:26:29.000000 minium-1.4.0/minium/framework/errorReport.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/tgit/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/auth.py
+-rw-r--r--   0 root         (0) root         (0)    97301 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/unittest/
+-rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.0/minium/framework/libs/unittest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11757 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/libs/unittest/case.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/libs/unittest/suite.py
+-rw-r--r--   0 root         (0) root         (0)    19830 2022-12-19 02:27:07.000000 minium-1.4.0/minium/framework/loader.py
+-rw-r--r--   0 root         (0) root         (0)    10166 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/logcolor.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/miniconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/miniddt.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.0/minium/framework/minidoctor.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/minilimit.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/miniresult.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/minisuite.py
+-rw-r--r--   0 root         (0) root         (0)    29430 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/minitest.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/report.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/tools/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/tools/report_issue.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.0/minium/framework/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/miniprogram/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/miniprogram/base_driver/
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47762 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/app.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/callback.py
+-rw-r--r--   0 root         (0) root         (0)    28828 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)    46414 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/element.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/minium.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/minium_log.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/minium_object.py
+-rw-r--r--   0 root         (0) root         (0)    23560 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/page.py
+-rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/prefixer.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 03:03:26.000000 minium-1.4.0/minium/miniprogram/base_driver/version.json
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/version.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/qq_minium.py
+-rw-r--r--   0 root         (0) root         (0)    38928 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/wx_minium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/native/
+-rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.0/minium/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/native/lib/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.340473 minium-1.4.0/minium/native/lib/android_base/
+-rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/android_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.340473 minium-1.4.0/minium/native/lib/at/
+-rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/at/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/apkapi.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/atproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.344473 minium-1.4.0/minium/native/lib/at/bin/
+-rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/bin/AtServer.apk
+-rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/bin/AtStub.jar
+-rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.348473 minium-1.4.0/minium/native/lib/at/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/accesshelper.py
+-rw-r--r--   0 root         (0) root         (0)    46986 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/at/core/adbwrap.py
+-rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/case_repair_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/element.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/javadriver.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/resguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.348473 minium-1.4.0/minium/native/lib/at/core/stf/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/mincap.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/minitouch.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/uidevice.py
+-rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/uixml.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/websocketcli.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/eventmonitor.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/hook.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/jlogcat.py
+-rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/keycode.py
+-rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/perfcollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/tests/
+-rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/AtEvent.py
+-rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/AtSocket.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/adbtest.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/airtesttest.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/atdevicetest.py
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/attestbase.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/drivertest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/elementtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/tests/images/
+-rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/1.jpg
+-rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/2.jpg
+-rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/image.jpg
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/javadrivertest.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minicap_test.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minitest.py
+-rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minitouch_test.py
+-rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/u2test.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/uixmltest.py
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/vs_test.py
+-rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/webdrivertest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/utils/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/apkinfo.py
+-rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/axmlparser.py
+-rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/axmlparser3.py
+-rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/commonhelper.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/magic.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/nbsp.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/threadhelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/vision/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/vision/template_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/at/webdriver/
+-rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/driver.py
+-rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/error.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/jsapi.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/miniapp.py
+-rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/stub.js
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/tabdescription.py
+-rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/tabwebsocket.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/webelement.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/webhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/wspools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/at/wechat/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/activtiy.py
+-rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/appvars.py
+-rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wsimp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/case_repair_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/case_repair_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/case_repair_sdk/default_trace.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/wda/
+-rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/screenhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/xcui_element_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/wx_wda/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/wdaUI.py
+-rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/webDriverTool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/qq_native/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qandroidnative.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qbasenative.py
+-rwxr-xr-x   0 root         (0) root         (0)    16882 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qiosnative.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/wx_native/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/wx_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39339 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/androidnative.py
+-rw-r--r--   0 root         (0) root         (0)    23791 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/basenative.py
+-rw-r--r--   0 root         (0) root         (0)     8053 2023-02-07 11:55:46.000000 minium-1.4.0/minium/native/wx_native/idenative.py
+-rw-r--r--   0 root         (0) root         (0)    36096 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/iosnative.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.0/minium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/emitter.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.0/minium/utils/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.0/minium/utils/injectjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium/utils/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.360473 minium-1.4.0/minium/utils/js/es5/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      255 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      535 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      340 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-04-27 03:03:14.000000 minium-1.4.0/minium/utils/js/es5/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      807 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      459 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     5247 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)     7139 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/uuid.js
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/waitUtil.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.364473 minium-1.4.0/minium/utils/js/min/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-04-27 03:03:26.000000 minium-1.4.0/minium/utils/js/min/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      201 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-04-27 03:03:25.000000 minium-1.4.0/minium/utils/js/min/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      270 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-27 03:03:26.000000 minium-1.4.0/minium/utils/js/min/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-27 03:03:25.000000 minium-1.4.0/minium/utils/js/min/uuid.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/waitUtil.js
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/meta.py
+-rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.0/minium/utils/platforms.py
+-rw-r--r--   0 root         (0) root         (0)    15200 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9058 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 03:03:31.364473 minium-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-04-27 02:49:44.000000 minium-1.4.0/setup.py
```

### Comparing `minium-1.3.dev2/minium/__init__.py` & `minium-1.4.0/minium/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-06-24
-from .miniprogram.base_driver.minium import build_version
+from .miniprogram.base_driver.version import build_version
 from .miniprogram import get_minium_driver
 from .miniprogram.wx_minium import WXMinium
 from .miniprogram.qq_minium import QQMinium
 from .miniprogram.base_driver.page import Page
 from .miniprogram.base_driver.app import App
 from .miniprogram.base_driver.element import BaseElement
 from .miniprogram.base_driver.callback import Callback
 from .framework.minitest import MiniTest
 from .framework.assertbase import *
 from .framework.miniddt import *
-from .framework.miniretry import retry
+from .utils.utils import retry, catch
 from .framework.miniresult import MiniResult
 from .framework.exception import *
 from .framework.libs.unittest import *
 from .native import *
 
 
 def Minium(conf=None, *args, **kwargs):
```

### Comparing `minium-1.3.dev2/minium/framework/assertbase.py` & `minium-1.4.0/minium/framework/assertbase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,105 @@
 # -*- coding: utf-8 -*-
 """
 @author: 'xiazeng'
 @created: 2016/11/23
 """
 # import unittest
 import json
+import typing
 import os.path
 import inspect
 import time
+from functools import wraps
 from .logcolor import *
 import logging.handlers
 import traceback
 import datetime
 import re
 from minium.miniprogram.wx_minium import WXMinium
 from .miniconfig import MiniConfig, get_log_level
 from minium.framework.libs import unittest
 
 logger = logging.getLogger("minium")
 logger.propagate = False
 WORKSPACE_DIR = os.path.abspath(os.getcwd())
 # print("当前工作路径: %s" % WORKSPACE_DIR)
-LOG_FORMATTER = "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
+# LOG_FORMATTER = "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
 FILENAME_LOGGER = "loader{0}.log".format(datetime.datetime.now().strftime("%Y%m%d"))
 
-g_console_handler = None
 g_case_log_handler = None
 
 g_from_command = False
 
 __ALL__ = ["AssertBase", "exit_when_error"]
 
 
 def exit_when_error(test_item):
     setattr(test_item, "__stop_when_error", True)
     return test_item
 
+AssertBase = None
 
-class AssertBase(unittest.TestCase):
+def hook_wrapper(src):
+    @wraps(src)
+    def hook_assert(self: AssertBase, *args, **kwargs):
+        if not self._hook_assert:
+            return src(self, *args, **kwargs)
+        called_frame = inspect.getouterframes(inspect.currentframe(), 2)
+        called_name = called_frame[1][3]
+        signature = inspect.signature(src)
+        try:
+            msg_index = list(signature.parameters.keys()).index("msg")
+        except ValueError:
+            msg_index = -1
+        ret = True
+        print_msg = None
+        try:
+            return src(self, *args, **kwargs)
+        except AssertionError as e:
+            self._has_assert_error = True
+            ret = False
+            print_msg = str(e)
+            raise
+        finally:
+            # todo:
+            #  1. msg needed
+            if called_name and not called_name.startswith("assert"):
+                if msg_index < len(args) and msg_index > -1:
+                    name = args[msg_index]
+                else:
+                    name = kwargs.get("msg")
+                if name:
+                    name = re.sub(r"\W|^(?=\d)", "_", name)
+                self._add_assert_info(name or src.__name__, ret, print_msg)
+    return hook_assert
+
+class HookAssert(type):
+    def __new__(cls, name, base, attr_dict):
+        def search_parent(bases):
+            # print("search", bases)
+            for b in bases:
+                for k in b.__dict__.keys():
+                    if k not in attr_dict and k.startswith("assert") and callable(b.__dict__[k]):
+                        attr_dict[k] = b.__dict__[k]  # 算直接继承?
+                if not isinstance(b, HookAssert):  # 往上搜索
+                    search_parent(b.__bases__)
+        search_parent(base)
+        for k in attr_dict:
+            if k.startswith("assert") and callable(attr_dict[k]) and not hasattr(attr_dict[k], "__wrapped__"):
+                attr_dict[k] = hook_wrapper(attr_dict[k])
+        return super().__new__(cls, name, base, attr_dict)
+
+class AssertBase(unittest.TestCase, metaclass=HookAssert):
     DEVICE_INFO = {}
     CONFIG = None
 
     test_config: MiniConfig = None
 
-    __hook_assert = False
+    _hook_assert = False
 
     def _startTest(self):
         # 初始化配置
         self._setup_config()
         # 初始化hook assert
         self._setup_assert()
         # 初始化日志
@@ -85,24 +137,17 @@
         if cls.CONFIG.outputs is None:
             outputs = os.path.join(os.getcwd(), "outputs")
             if not os.path.exists(outputs):
                 os.makedirs(outputs)
             cls.CONFIG.outputs = outputs
         if cls.CONFIG.create_time is None:
             cls.CONFIG.create_time = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
-        global g_console_handler, g_case_log_handler
+        global g_case_log_handler
         log_level = get_log_level(cls.CONFIG.debug_mode)
-        if g_console_handler is None:  # 格式化 & 染色 -> 屏幕
-            console_handler = logging.StreamHandler()
-            console_handler.addFilter(colorfilter)
-            formatter = logging.Formatter(LOG_FORMATTER)
-            console_handler.setFormatter(formatter)
-            logger.addHandler(console_handler)
-            logger.setLevel(log_level)
-            g_console_handler = console_handler
+        g_console_handler.setLevel(log_level)
 
         if g_case_log_handler is None:  # 格式化 -> 固化到文件
             log_path = os.path.join(cls.CONFIG.outputs, FILENAME_LOGGER)
             case_log_handler = logging.handlers.RotatingFileHandler(
                 log_path, maxBytes=1024 * 1024, encoding="utf-8"
             )
             case_log_handler.addFilter(nofilter)
@@ -146,15 +191,15 @@
             self._testMethodName,
             dt,
         )
         if not os.path.exists(self.test_config.case_output):
             os.makedirs(self.test_config.case_output)
 
     def _setup_assert(self):
-        self.__hook_assert = True
+        self._hook_assert = True
         self._has_assert_error = False
         self.assert_list = []
         self.__assert_index = 0
 
     def _setup_log(self):
         # 保存日志到outputs
         # case_log_filename = self.wrap_filename("{0}.log".format(self._testMethodName))
@@ -171,14 +216,15 @@
         self._case_log_handler = case_log_handler
         logger.addHandler(self._case_log_handler)
         # logger.info(self.CONFIG)
 
     def _setup_results(self):
         self.setup_time = time.time()
         self.screen_info = []
+        self.step_info = []  # 录制回放用
         self.check_list = []
         desc = self._testMethodDoc
         if desc is not None:
             lines = desc.split("\n")
             lines = [l.strip() for l in lines if l]
             desc = "\n".join(lines)
         module_filename = inspect.getsourcefile(self.__class__)
@@ -213,88 +259,129 @@
             "failed_line_num": -1,
             "device": AssertBase.DEVICE_INFO,
             "log_filename": self._log_filename,
             "error_type": "",
             "error_value": "",
             "error_stages": [],
             "screen_info": self.screen_info,
+            "step_info": self.step_info,
             "check_list": self.check_list,
             "assert_list": self.assert_list,
         }
 
     # ===============================================================================================
     # Teardown
     # ===============================================================================================
     def _teardown_handle(self):
         """
         teardown收集数据前进行的操作
         """
         pass
 
-    def _get_error_info(self):
+    def _get_error_info(self) -> typing.Tuple[typing.Any, list, str]:
         if not self._outcome:
-            logger.error("self._outcome is None, it's not reasonable")
-            return getattr(
+            logger.error("self._outcome is None, maybe a class error")
+            sys_info = getattr(
                 self.__class__, "__class_setup_failure_why__", None
-            ), getattr(
+            )
+            error_stages = getattr(
                 self.__class__, "__class_setup_failure_stages__", []
-            )  # 看看是不是class失败了
-        length = len(self._outcome.errors)
-        if length == 1:
-            sys_info = self._outcome.errors[-1][-1]
-        elif length > 1:
-            while length:
-                length -= 1
-                sys_info = self._outcome.errors[length][-1]
-                if sys_info is not None:  # step success
-                    return sys_info, getattr(self._outcome, "error_stages", [])
+            )
+            stage = error_stages[-1] if error_stages and len(error_stages) > 0 else ""
+            return sys_info, error_stages, stage # 看看是不是class失败了
+        sys_info = None
+        error_stages = getattr(self._outcome, "error_stages", None)
+        stage = ""
+        if error_stages is not None:  # minium.unittest.outcome
+            stage_errors = getattr(self._outcome, "stage_errors", {})
+            if "testMethod" in error_stages and "testMethod" in stage_errors:  # case内容部分有错误
+                sys_info = stage_errors["testMethod"][-1]  # 优先处理case错误
+                stage = "testMethod"
+            else:
+                for i in range(len(error_stages)-1, -1, -1):
+                    if error_stages[i] in stage_errors:
+                        stage = error_stages[i]
+                        sys_info = stage_errors[stage][-1]
+                        break
+            return sys_info, error_stages, stage
+        else:
+            length = len(self._outcome.errors)
+            if length == 1:
+                sys_info = self._outcome.errors[-1][-1]
+            elif length > 1:
+                while length:
+                    length -= 1
+                    sys_info = self._outcome.errors[length][-1]
+                    if sys_info is not None:  # step success
+                        return sys_info, [], stage
+            return sys_info, [], stage
+        
+    def _get_source(self, stage) -> dict:
+        if not stage:
+            stage = "testMethod"
+        source_line = [[], 0]
+        test_method = getattr(self, self._testMethodName if stage == "testMethod" else stage, None)
+        if test_method:
+            source_line = inspect.getsourcelines(test_method)
+        return {"code": source_line[0], "start": source_line[1]}
+
+    def _get_stack_info(self, stage, sys_info):
+        if not sys_info:
+            return
+        failed_line_num = -1
+        isDdt = False
+        if stage == "testMethod":
+            test_method = getattr(self, self._testMethodName, None)
+            if test_method and getattr(test_method, "__wrapped__", None):
+                # testMethod.__wrapped__存在, 为ddt生成的方法
+                isDdt = True
+                logger.warn(f"{self._testMethodName} isDdt case")
         else:
-            sys_info = None
-        return sys_info, getattr(self._outcome, "error_stages", [])
+            test_method = getattr(self, stage, None)
+        e_type, e_value, e_traceback = sys_info
+        stack_lines = traceback.format_exception(e_type, e_value, e_traceback)
+        logger.exception(f"{test_method}", exc_info=sys_info)
+        if len(stack_lines) > 2:
+            r = re.compile(r"File [\'\"](.*)[\'\"], line (\d+), in (\S+)")
+            for stack_line in stack_lines[1:]:
+                m = r.search(stack_line)
+                if m and stage == "testMethod":
+                    if (
+                        m.group(1) == self._test_filename
+                        and (self._testMethodName.startswith(m.group(3)) if isDdt else m.group(3) == self._testMethodName)
+                    ):
+                        failed_line_num = int(m.group(2))
+                elif m and m.group(3) == stage:
+                    failed_line_num = int(m.group(2))
+        return {"failed_line_num": failed_line_num, "stack_lines": stack_lines, "error_type": e_type.__name__, "error_value": str(e_value.args[0]) if len(e_value.args) > 0 else ""}
 
     def _teardown_collect(self):
         """
         收集results数据
         """
         self.results["stop_timestamp"] = time.time()
-        sys_info, error_stages = self._get_error_info()
-        test_method = getattr(self, self._testMethodName)
-        source_line = inspect.getsourcelines(test_method)
+        sys_info, error_stages, stage = self._get_error_info()
 
         if not self.test_config.only_native:
             self.results["appId"] = self.appId
             self.results["appName"] = self.appName
         else:
             logger.warning("Only native mode, skip get APP id and APP nickname")
-        self.results["source"] = {"code": source_line[0], "start": source_line[1]}
+        self.results["source"] = self._get_source(stage)
         if sys_info:
-            e_type, e_value, e_traceback = sys_info
-            self.results["failed_line_num"] = -1
-            stack_lines = traceback.format_exception(e_type, e_value, e_traceback)
-            logger.exception(f"{test_method}", exc_info=sys_info)
-            if len(stack_lines) > 2:
-                r = re.compile(r"File [\'\"](.*)[\'\"], line (\d+), in (\w+)")
-                for stack_line in stack_lines[1:]:
-                    m = r.search(stack_line)
-                    if m:
-                        if (
-                            m.group(1) == self._test_filename
-                            and m.group(3) == self._testMethodName
-                        ):
-                            self.results["failed_line_num"] = int(m.group(2))
+            stack_info = self._get_stack_info(stage, sys_info)
+            self.results["failed_line_num"] = stack_info["failed_line_num"]
             if self._has_assert_error:
-                self.results["failures"] = "".join(stack_lines)
+                self.results["failures"] = "".join(stack_info["stack_lines"])
                 self.results["is_failure"] = True
             else:
-                self.results["errors"] = "".join(stack_lines)
+                self.results["errors"] = "".join(stack_info["stack_lines"])
                 self.results["is_error"] = True
-            self.results["error_type"] = e_type.__name__
-            self.results["error_value"] = (
-                str(e_value.args[0]) if len(e_value.args) > 0 else ""
-            )
+            self.results["error_type"] = stack_info["error_type"]
+            self.results["error_value"] = stack_info["error_value"]
             self.results["error_stages"] = error_stages
         else:
             self.results["success"] = True
 
     def _teardown_log(self):
         """
         落地log
@@ -332,54 +419,14 @@
                 "name": name,
                 "ret": ret,
                 "msg": reason,
                 **(hook_result if isinstance(hook_result, dict) else {}),
             }
         )
 
-    def __getattribute__(self, item):
-        attr = super().__getattribute__(item)
-        if item.startswith("assert") and self.__hook_assert and callable(attr):
-
-            def _hook_assert(*args, **kwargs):
-                called_frame = inspect.getouterframes(inspect.currentframe(), 2)
-                called_name = called_frame[1][3]
-                signature = inspect.signature(attr)
-                try:
-                    msg_index = list(signature.parameters.keys()).index("msg")
-                except ValueError:
-                    msg_index = -1
-                ret = True
-                print_msg = None
-                try:
-                    return attr(*args, **kwargs)
-                    # if getattr(type(mgr), "__enter__", None) and getattr(type(mgr), "__exit__", None):  # assertRaise等
-                    #     _enter = getattr(type(mgr), "__enter__", None)
-                    #     _exit = getattr(type(mgr), "__exit__", None)
-                except AssertionError as e:
-                    self._has_assert_error = True
-                    ret = False
-                    print_msg = str(e)
-                    raise
-                finally:
-                    # todo:
-                    #  1. msg needed
-                    if called_name and not called_name.startswith("assert"):
-                        if msg_index < len(args) and msg_index > -1:
-                            name = args[msg_index]
-                        else:
-                            name = kwargs.get("msg")
-                        if name:
-                            name = re.sub(r"\W|^(?=\d)", "_", name)
-                        self._add_assert_info(name or item, ret, print_msg)
-
-            return _hook_assert
-        else:
-            return attr
-
     @property
     def screen_dir(self):
         screen_dir = self.wrap_filename("images")
         if not os.path.exists(screen_dir):
             os.makedirs(screen_dir)
         return screen_dir
```

### Comparing `minium-1.3.dev2/minium/framework/casedump.py` & `minium-1.4.0/minium/framework/casedump.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/caseinspect.py` & `minium-1.4.0/minium/framework/caseinspect.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/css/chunk-vendors.52eeca6f.css` & `minium-1.4.0/minium/framework/dist/css/chunk-vendors.52eeca6f.css`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/favicon.ico` & `minium-1.4.0/minium/framework/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/fonts/element-icons.535877f5.woff` & `minium-1.4.0/minium/framework/dist/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/fonts/element-icons.732389de.ttf` & `minium-1.4.0/minium/framework/dist/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/index.html` & `minium-1.4.0/minium/framework/dist/index.html`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/js/app.544bedf4.js` & `minium-1.4.0/minium/framework/dist/js/app.544bedf4.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/dist/js/chunk-vendors.22ed339a.js` & `minium-1.4.0/minium/framework/dist/js/chunk-vendors.22ed339a.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/errorReport.py` & `minium-1.4.0/minium/framework/errorReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import json
 import argparse
 import tools.report_issue
 import requests
 
 work_root = os.path.abspath(".")
 
-# robot_url = "http://in.qyapi.weixin.qq.com/cgi-bin/webhook/send?key=71881e81-7f49-49ce-8ac3-6e00b8508ba4"
-
-
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-k",
         "--kao",
         dest="upload_failed_case",
         action="store_true",
```

### Comparing `minium-1.3.dev2/minium/framework/exception.py` & `minium-1.4.0/minium/framework/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,18 +22,52 @@
         Exception.__init__(self, msg)
 
 
 class MiniConnectError(MiniError):
     ...
 
 
+class MiniConnectSvrError(MiniConnectError):
+    ...
+
+
+class MiniReConnectSvrError(MiniConnectSvrError):
+    ...
+
+
 class MiniTimeoutError(MiniConnectError):
     ...
 
 
+# 链接断了
+class MiniConnectionClosedError(MiniConnectError):
+    ...
+
+
+# 小程序下线了
+class MiniClientOfflineError(MiniConnectError):
+    ...
+
+
+# 调试通道错误
+class MiniDebugConnectionError(MiniConnectError):
+    ...
+
+# 因断连造成的未收到指令回复
+class MiniTimeoutCauseByConnectionBreakError(
+    MiniTimeoutError, MiniConnectionClosedError
+):
+    ...
+
+
+# 因小程序下线造成的未收到指令回复
+class MiniTimeoutCauseByClientOffline(MiniTimeoutError, MiniClientOfflineError):
+    ...
+
+
 class MiniRefuseError(MiniConnectError):
     ...
 
 
 class MiniNotAttributeError(AttributeError):
     ...
 
@@ -78,7 +112,10 @@
     def __init__(self, *args: object, name: str = ..., path: str = ...) -> None:
         if len(args) > 0 and isinstance(args[0], ModuleNotFoundError):
             err = args[0]
             super().__init__(err.msg, *args[1:], name=err.name, path=err.path)
             self.with_traceback(err.__traceback__)
         else:
             super().__init__(*args, name=name, path=path)
+
+class RemoteDebugConnectionLost(MiniAppError):  # 远程调试服务掉线
+    ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `minium-1.3.dev2/minium/framework/libs/tgit/auth.py` & `minium-1.4.0/minium/framework/libs/tgit/auth.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/libs/tgit/client.py` & `minium-1.4.0/minium/framework/libs/tgit/client.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/libs/unittest/case.py` & `minium-1.4.0/minium/native/lib/at/jlogcat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,230 +1,257 @@
+# -*- coding: utf-8 -*-
+"""
+@author: 'xiazeng'
+@created: 2016/12/2 
+"""
+import re
+import time
+import datetime
+import threading
 import sys
-import types
-import contextlib
-from functools import wraps
-from unittest.case import (
-    addModuleCleanup,
-    FunctionTestCase,
-    SkipTest,
-    skip,
-    skipIf as skipIfSrc,
-    skipUnless,
-    expectedFailure,
-)
-from unittest.case import TestCase as TestCaseSrc
-from unittest.case import _Outcome, _ShouldStop, warnings, safe_repr
-
-
-class Outcome(_Outcome):
-    def __init__(self, result=None):
-        super().__init__(result)
-        # 兼容3.11
-        if not (getattr(self, "skipped")):
-            self.skipped = []
-        if not (getattr(self, "errors")):
-            self.errors = []
-        self.error_stages = (
-            []
-        )  # 失败发生在的步骤：_miniClassSetUp, _miniSetUp, _miniTearDown, setUpClass, tearDownClass, setUp, tearDown, testMethod
 
-    @contextlib.contextmanager
-    def testPartExecutor(self, test_case, isTest=False, error_stage=None):
-        """
-        rewrite for error_stages
-        :error_stage: current error stage name
-        """
-        old_success = self.success
-        self.success = True
+if sys.version_info[0] < 3:
+    from Queue import Queue, Empty
+else:
+    from queue import Queue, Empty
+
+import logging
+
+logger = logging.getLogger()
+
+
+def decode_bytes(bs):
+    ds = ['ascii', 'utf-8', 'gbk']
+    for d in ds:
         try:
-            yield
-        except KeyboardInterrupt:
-            raise
-        except SkipTest as e:
-            self.success = False
-            self.skipped.append((test_case, str(e)))
-        except _ShouldStop:
+            return bs.decode(d)
+        except UnicodeDecodeError:
             pass
-        except:
-            exc_info = sys.exc_info()
-            if self.expecting_failure:
-                self.expectedFailure = exc_info
-            else:
-                self.success = False
-                self.errors.append((test_case, exc_info))
-            # explicitly break a reference cycle:
-            # exc_info -> frame -> exc_info
-            exc_info = None
+    # 可能出现utf-8被截断的场景
+    # UnicodeDecodeError: 'utf-8' codec can't decode byte 0xe9 in position 4094: invalid continuation byte
+    return bs.decode("utf-8", 'ignore')
+
+
+class LogRecord(object):
+    reg_str = r"(?P<time>(\d{4}-)?\d{2}-\d{2}\s+\d{2}:\d{2}:\d{2}\.\d+)\s+" \
+              r"(?P<level>[VDIWEFS])\/" \
+              r"(?P<tag>.*(?=\(\s*\d+\s*\)))\(\s*" \
+              r"(?P<pid>\d+)\s*\)\s*:\s+" \
+              r"(?P<msg>.*)"
+    reg = re.compile(reg_str, flags=re.VERBOSE | re.MULTILINE)
+
+    def __init__(self, line):
+        self.raw_line = line
+        m = LogRecord.reg.match(line)
+        if m is None:
+            raise RuntimeError("invalided line:" + line)
+        self.time = m.group("time")
+        self.level = m.group("level")
+        self.tag = m.group("tag")
+        self.pid = m.group("pid")
+        self.msg = m.group("msg")
+
+    @property
+    def ts(self):
+        t = self.time.split(".")
+        if len(self.time.split("-")) != 3:
+            time_str = "%s-%s" % (datetime.datetime.now().year, t[0])
         else:
-            if self.result_supports_subtests and self.success:
-                self.errors.append((test_case, None))
-        finally:
-            if error_stage and (self.success == self.expecting_failure):
-                self.error_stages.append(error_stage)
-            self.success = self.success and old_success
-
-
-# 重写testcase
-class TestCase(TestCaseSrc):
-    def _callSetUp(self):
-        # self._miniSetUp()
-        self.setUp()
-
-    def _miniSetUp(self):
-        pass
-
-    def _callTearDown(self):
-        # self._miniTearDown()
-        self.tearDown()
-
-    def _miniTearDown(self):
-        pass
-
-    def run(self, result=None):
-        orig_result = result
-        if result is None:
-            result = self.defaultTestResult()
-            startTestRun = getattr(result, "startTestRun", None)
-            if startTestRun is not None:
-                startTestRun()
-
-        result.startTest(self)
-
-        testMethod = getattr(self, self._testMethodName)
-        if getattr(self.__class__, "__unittest_skip__", False) or getattr(
-            testMethod, "__unittest_skip__", False
-        ):
-            # If the class or method was skipped.
-            try:
-                skip_why = getattr(
-                    self.__class__, "__unittest_skip_why__", ""
-                ) or getattr(testMethod, "__unittest_skip_why__", "")
-                self._addSkip(result, self, skip_why)
-            finally:
-                result.stopTest(self)
-            return
-
-        expecting_failure_method = getattr(
-            testMethod, "__unittest_expecting_failure__", False
-        )
-        expecting_failure_class = getattr(self, "__unittest_expecting_failure__", False)
-        expecting_failure = expecting_failure_class or expecting_failure_method
-        outcome = Outcome(result)
-        try:
-            self._outcome = outcome
+            time_str = int(t[0])
+        timetuple = time.strptime(time_str, "%Y-%m-%d %H:%M:%S")
+        ts = time.mktime(timetuple) * 1000 + int(t[1])
+        return ts
+
+    @classmethod
+    def is_valid_line(cls, line):
+        m = cls.reg.match(line)
+        if not m:
+            logger.warning(line)
+        return m is not None
 
-            with outcome.testPartExecutor(self, error_stage="_miniSetUp"):
-                self._miniSetUp()
-            if outcome.success:
-                with outcome.testPartExecutor(self, error_stage="setUp"):
-                    self._callSetUp()
-                if outcome.success:
-                    outcome.expecting_failure = expecting_failure
-                    with outcome.testPartExecutor(
-                        self, isTest=True, error_stage="testMethod"
-                    ):
-                        self._callTestMethod(testMethod)
-                    outcome.expecting_failure = False
-                    with outcome.testPartExecutor(self, error_stage="tearDown"):
-                        self._callTearDown()
-            outcome.expecting_failure = False
-            with outcome.testPartExecutor(self, error_stage="_miniTearDown"):
-                self._miniTearDown()
-
-            self.doCleanups()
-            for test, reason in outcome.skipped:
-                self._addSkip(result, test, reason)
-            self._feedErrorsToResult(result, outcome.errors)
-            if outcome.success:
-                if expecting_failure:
-                    if outcome.expectedFailure:
-                        self._addExpectedFailure(result, outcome.expectedFailure)
-                    else:
-                        self._addUnexpectedSuccess(result)
-                else:
-                    result.addSuccess(self)
-            return result
-        finally:
-            result.stopTest(self)
-            if orig_result is None:
-                stopTestRun = getattr(result, "stopTestRun", None)
-                if stopTestRun is not None:
-                    stopTestRun()
-
-            # explicitly break reference cycles:
-            # outcome.errors -> frame -> outcome -> outcome.errors
-            # outcome.expectedFailure -> frame -> outcome -> outcome.expectedFailure
-            outcome.errors.clear()
-            outcome.expectedFailure = None
-
-            # clear the outcome, no more needed
-            self._outcome = None
-
-    def assertSetContainsSubset(self, subset: set, superset: set, msg=None):
-        """Checks whether superset is a superset of subset."""
-        warnings.warn("assertSetContainsSubset is deprecated", DeprecationWarning)
-        missing = []
-        for item in subset:
-            if item not in superset:
-                missing.append(item)
-
-        if not missing:
-            return
-
-        standardMsg = ""
-        if missing:
-            standardMsg = "Missing: %s" % ",".join(safe_repr(m) for m in missing)
-
-        self.fail(self._formatMessage(msg, standardMsg))
-
-def _whether_need_skip(func: types.FunctionType, *args, **kwargs):
-    if func.__code__.co_argcount == 0:
-        need_skip = func()
-    elif func.__code__.co_argcount == 1:
-        need_skip = func(args[0])  # just use TestCase
-    else:
-        need_skip = func(*args, **kwargs)  # mybe ddt case
-    return need_skip
+    def __repr__(self):
+        return "%s %s %s %s" % (self.time, self.level, self.tag, self.msg)
 
-def skipIf(func_or_condition: types.FunctionType or bool, reason=''):
+
+class AsynchronousFileReader(threading.Thread):
     """
-    Skip a test if the condition is true.
+    Helper class to implement asynchronous reading of a file
+    in a separate thread. Pushes read lines on a queue to
+    be consumed in another thread.
     """
-    if isinstance(func_or_condition, bool):
-        return skipIfSrc(func_or_condition, reason)
-    def wrapper(wrapped):
-        @wraps(wrapped)
-        def inner(*args, **kwargs):
-            if len(args) == 0:  # not TestCase
-                return wrapped(*args, **kwargs)
-            if isinstance(args[0], TestCaseSrc):  # is TestCase
-                self = args[0]
-                if _whether_need_skip(func_or_condition, *args, **kwargs):
-                    self.skipTest(reason)
-                return wrapped(*args, **kwargs)
-            # normal wrapped func
-            if _whether_need_skip(func_or_condition, *args, **kwargs):
-                raise SkipTest(reason)
-            return wrapped(*args, **kwargs)
-        return inner
-    return wrapper
-
-def expectedException(exception_or_type: Exception or type):
-    def wrapper(wrapped):
-        @wraps(wrapped)
-        def inner(*args, **kwargs):
-            if isinstance(exception_or_type, type):
-                _type = exception_or_type
-                _value = None
-            else:
-                _type = exception_or_type.__class__
-                _value = exception_or_type.__repr__()
-            try:
-                return wrapped(*args, **kwargs)
-            except _type as t:
-                if _value is None or _value == t.__repr__():
-                    return
-                raise t
-            else:
-                raise
-        return inner
-    return wrapper
+
+    def __init__(self, fd, process, queue):
+        assert isinstance(queue, Queue)
+        assert callable(fd.readline)
+        threading.Thread.__init__(self)
+        self._fd = fd
+        self._process = process
+        self.daemon = True
+        self._queue = queue
+        self._should_stop = False
+
+    def run(self):
+        """The body of the tread: read lines and put them on the queue."""
+        count = 0
+        next_count = 10000
+        start = time.time()
+        try:
+            while True:
+                if self._should_stop:
+                    break
+                if self._process.poll() is not None:
+                    logging.error("process stopped:%s, logcount:%s", self._process.poll(), count)
+                    break
+                line = self._fd.readline()
+                if line:
+                    count += 1
+                    self._queue.put(line)
+                    if count > next_count:
+                        t = time.time() - start
+                        logger.debug("total:%s, cost:%d, produce rate:%s per second", count, t, int(count / t))
+                        next_count += next_count
+                    if line == b'read: unexpected EOF!\n':
+                        break
+        except:
+            logger.exception("exception")
+
+        logger.info("read logcat finish: %s", self._should_stop)
+
+    def eof(self):
+        """Check whether there is no more content to expect."""
+        return not self.is_alive()
+
+    def stop(self):
+        self._should_stop = True
+        self.join(1)
+
+
+class JLogCat(threading.Thread):
+    def __init__(self, adb):
+        threading.Thread.__init__(self)
+        self._is_stop = False
+        self.adb = adb
+        # Launch the asynchronous readers of the process' stdout.
+        self.stdout_queue = Queue()
+        self._bg_run()
+        self.mutex = threading.Lock()
+        self.filter_map = {}
+        self.filter_values = []
+        self.names = []
+        self.redirect_file = None
+
+    def redirect_to_path(self, path):
+        self.redirect_file = open(path, "a")
+
+    def _bg_run(self, clear_logcat=True):
+        if clear_logcat:
+            self.adb.run_adb("logcat -c")
+        self.process = self.adb.run_adb("logcat  -v time", False)
+        logging.info("process_id:%s", self.process.pid)
+        stdout_reader = AsynchronousFileReader(self.process.stdout, self.process, self.stdout_queue)
+        stdout_reader.start()
+        self.stdout_reader = stdout_reader
+
+    def run(self):
+        # Check the queues if we received some output (until there is nothing more to get).
+        retype = type(re.compile('hello, world'))
+        line_count = 0
+        start = time.time()
+        next_count = 10000
+
+        while not self._is_stop:
+            if self.stdout_reader.eof():
+                self._bg_run(clear_logcat=False)
+            while not self.stdout_queue.empty() and not self._is_stop:
+                line = None
+                try:
+                    line = self.stdout_queue.get(timeout=0.1)
+                except Empty:
+                    logger.info("empty")
+                    pass
+                line = decode_bytes(line)
+                line_count += 1
+                if line_count > next_count:
+                    t = time.time() - start
+                    logger.debug("total:%s, cost:%d, consume rate:%s per second", line_count, t, int(line_count / t))
+                    next_count += next_count
+                if line:
+                    if self.redirect_file:
+                        self.redirect_file.write(line)
+                    for fm in self.filter_values:
+                        records = fm["records"]
+                        for keyword in fm["keywords"]:
+                            if isinstance(keyword, str):
+                                if keyword in line:
+                                    logger.debug("[%s]+logcat, %s", self.ident, line.strip())
+                                    records.append(line.strip())
+                            elif isinstance(keyword, retype):
+                                if keyword.match(line):
+                                    logger.debug("[%s]+logcat, %s", self.ident, line.strip())
+                                    records.append(line.strip())
+        logger.info("finished: %s", self._is_stop)
+
+    def start_record(self, name, *args):
+        """
+        开始等待，日志
+        :param name:标识名称，任意字符串，后面取日志要根据这个标识来区分
+        :param *args: 日志匹配的关键字
+        :return:
+        """
+        self.mutex.acquire()
+        self.filter_map[name] = {
+            "keywords": args,
+            "records": []
+        }
+        self.filter_values = list(self.filter_map.values())
+        self.mutex.release()
+
+    def _get_records(self, name):
+        self.mutex.acquire()
+        if name not in self.filter_map:
+            lines = []
+        else:
+            lines = self.filter_map[name]["records"]
+        records = [LogRecord(l) for l in lines if LogRecord.is_valid_line(l)]
+        self.mutex.release()
+        return records
+
+    def get_lines(self, name):
+        return self._get_records(name)
+
+    def wait_records(self, name, count=1, timeout=10):
+        s = time.time()
+        records = []
+        while time.time() - s < timeout:
+            records = self._get_records(name)
+            if len(records) >= count:
+                return records
+            time.sleep(0.1)
+        return records
+
+    def new_wait_records(self, name, count=1, timeout=20):
+        time.sleep(timeout)
+        records = self._get_records(name)
+        if len(records) < count:
+            time.sleep(5)
+            records = self._get_records(name)
+        return records
+
+    def stop_record(self, name):
+        records = self._get_records(name)
+        self.mutex.acquire()
+        del self.filter_map[name]
+        self.filter_values = list(self.filter_map.values())
+        self.mutex.release()
+        return records
+
+    def stop(self):
+        self._is_stop = True
+        self.stdout_reader.stop()
+        self.join()
+        self.adb.kill_pid(self.process.pid)
+        if self.redirect_file:
+            self.redirect_file.close()
+        logger.info("logcat finish")
+
+    def __del__(self):
+        self.stop()
```

### Comparing `minium-1.3.dev2/minium/framework/libs/unittest/suite.py` & `minium-1.4.0/minium/framework/libs/unittest/suite.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,37 +50,41 @@
             currentClass._classSetupFailed = False
         except TypeError:
             # test may actually be a function
             # so its class will be a builtin-type
             pass
 
         error_stages = []
+        stage_errors = {}
         # run _miniClassSetUp
         _miniClassSetUp = getattr(currentClass, "_miniClassSetUp", None)
         setattr(currentClass, "__is_minitest_suite__", True)
         if _miniClassSetUp is not None:
             _call_if_exists(result, "_setupStdout")
             try:
                 _miniClassSetUp()
             except Exception as e:
                 if isinstance(result, _DebugResult):
                     raise
                 currentClass._classSetupFailed = True
                 error_stages.append("_miniClassSetUp")
                 info = sys.exc_info()
+                stage_errors["_miniClassSetUp"] = [info,]
                 setattr(currentClass, "__class_setup_failure_why__", info)
                 setattr(currentClass, "__class_setup_failure_stages__", error_stages)
+                setattr(currentClass, "__class_setup_failure_errors__", stage_errors)
                 className = "%s.%s" % (
                     currentClass.__module__,
                     currentClass.__qualname__,
                 )
                 self._createClassFailure(test, result, e, info, error_stages)
                 # self._createClassOrModuleLevelException(result, e,
                 #                                         '_miniClassSetUp',
                 #                                         className)
+                info = None
                 return
             finally:
                 _call_if_exists(result, "_restoreStdout")
                 if currentClass._classSetupFailed is True:
                     currentClass.doClassCleanups()
                     if len(currentClass.tearDown_exceptions) > 0:
                         for exc in currentClass.tearDown_exceptions:
@@ -97,24 +101,27 @@
                 setUpClass()
             except Exception as e:
                 if isinstance(result, _DebugResult):
                     raise
                 currentClass._classSetupFailed = True
                 error_stages.append("setUpClass")
                 info = sys.exc_info()
+                stage_errors["_miniClassSetUp"] = [info,]
                 setattr(currentClass, "__class_setup_failure_why__", info)
                 setattr(currentClass, "__class_setup_failure_stages__", error_stages)
+                setattr(currentClass, "__class_setup_failure_errors__", stage_errors)
                 className = "%s.%s" % (
                     currentClass.__module__,
                     currentClass.__qualname__,
                 )
                 self._createClassFailure(test, result, e, info, error_stages)
                 # self._createClassOrModuleLevelException(result, e,
                 #                                         'setUpClass',
                 #                                         className)
+                info = None
             finally:
                 _call_if_exists(result, "_restoreStdout")
                 if currentClass._classSetupFailed is True:
                     currentClass.doClassCleanups()
                     if len(currentClass.tearDown_exceptions) > 0:
                         for exc in currentClass.tearDown_exceptions:
                             self._createClassOrModuleLevelException(
```

### Comparing `minium-1.3.dev2/minium/framework/loader.py` & `minium-1.4.0/minium/framework/loader.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/logcolor.py` & `minium-1.4.0/minium/framework/logcolor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 Description:
 
 """
 
 import logging
 import re
 
+logger = logging.getLogger("minium")
+logger.propagate = False
+LOG_FORMATTER = "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
+
+console_handler = logging.StreamHandler()
+formatter = logging.Formatter(LOG_FORMATTER)
+console_handler.setFormatter(formatter)
+logger.addHandler(console_handler)
+logger.setLevel(logging.DEBUG)
+g_console_handler = console_handler
+
 
 # now we patch Python code to add color support to logging.StreamHandler
 class CustomWindowsFilter(logging.Filterer):
     def _set_color(self, code):
         import ctypes
 
         # Constants from the Windows API
@@ -52,15 +63,20 @@
         BACKGROUND_MAGENTA = 0x0050
         BACKGROUND_YELLOW = 0x0060
         BACKGROUND_GREY = 0x0070
         BACKGROUND_INTENSITY = 0x0080  # background color is intensified.
         levelno = record.levelno
 
         if levelno >= 50:
-            color = BACKGROUND_YELLOW | FOREGROUND_RED | FOREGROUND_INTENSITY | BACKGROUND_INTENSITY
+            color = (
+                BACKGROUND_YELLOW
+                | FOREGROUND_RED
+                | FOREGROUND_INTENSITY
+                | BACKGROUND_INTENSITY
+            )
         elif levelno >= 40:
             color = FOREGROUND_RED | FOREGROUND_INTENSITY
         elif levelno >= 30:
             color = FOREGROUND_YELLOW | FOREGROUND_INTENSITY
         elif levelno >= 20:
             color = FOREGROUND_GREEN
         elif levelno >= 10:
@@ -98,15 +114,17 @@
         "App.logAdded": "",
     }
 
     def filter(self, record):
         if isinstance(record.msg, (str, bytes)):
             for key, value in CustomKeywordFilter.FILTER_MAP.items():
                 if value:
-                    if record.msg.find(key) >= 0 and re.match(".*(%s).*" % value, record.msg):
+                    if record.msg.find(key) >= 0 and re.match(
+                        ".*(%s).*" % value, record.msg
+                    ):
                         return 0
                 else:
                     if record.msg.find(key) >= 0:
                         return 0
         return record
 
 
@@ -268,21 +286,21 @@
 colorfilter = CustomMacFilter()
 global nofilter
 nofilter = CustomNoFilter()
 global kwfilter
 kwfilter = CustomKeywordFilter()
 global filefilter
 filefilter = CustomFileFilter()
+console_handler.addFilter(colorfilter)
 
 if __name__ == "__main__":
     import logging.handlers
+
     logger = logging.getLogger("yopo")
-    LOG_FORMATTER = (
-        "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
-    )
+    LOG_FORMATTER = "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
     FILENAME_LOGGER = "yopotest.log"
     # TO SCREEN
     console_handler = logging.StreamHandler()
     console_handler.addFilter(colorfilter)
     formatter = logging.Formatter(LOG_FORMATTER)
     console_handler.setFormatter(formatter)
     console_handler.setLevel(logging.INFO)
@@ -298,8 +316,8 @@
     case_log_handler.setFormatter(formatter)
     case_log_handler.setLevel(logging.DEBUG)
     logger.addHandler(case_log_handler)
     logger.setLevel(logging.DEBUG)
 
     logger.debug("debug msg")
     logger.info("info msg")
-    logger.warning("warn msg")
+    logger.warning("warn msg")
```

### Comparing `minium-1.3.dev2/minium/framework/miniconfig.py` & `minium-1.4.0/minium/framework/miniconfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,44 +10,47 @@
 
 
 class Path(str):
     pass
 
 
 default_config = {
-    "debug": False,  # debug模式
-    "base_dir": os.path.abspath(os.getcwd()),  # 如果没有配置, 默认工作目录, 如果通过文件生成则为文件所在目录
-    "platform": "ide",  # 平台: ide, android, ios
-    "app": "wx",  # 承载的app: wx
-    "debug_mode": "debug",  # 日志级别
-    "close_ide": False,  # 是否关闭IDE
-    "assert_capture": True,  # 断言时是否截图
-    "auto_relaunch": True,  # case开始时是否回到主页
-    "device_desire": {},  # 真机调试配置
-    "account_info": {},  # 账号配置
-    "report_usage": True,  # 是否需要报告
-    "remote_connect_timeout": 180,  # 真机调试中小程序在真机上打开的等待时间
-    "request_timeout": 60,  # 自动化控制指令请求超时时间
-    "use_push": True,  # 真机调试中是否使用推送形式打开小程序, false则需要扫调试二维码
-    "full_reset": False,  # 每个测试class结束，是否释放调试链接
-    "outputs": None,  # 测试产物输出路径
-    "enable_app_log": False,  # 记录小程序日志
-    "enable_network_panel": False,  # 记录小程序网络请求
-    "project_path": None,  # 小程序项目路径
-    "dev_tool_path": None,  # 开发者工具命令行工具路径
-    "test_port": 9420,  # 小程序自动化测试调试端口
-    "mock_native_modal": {},  # 仅在IDE生效, mock所有会有原生弹窗的接口
-    "mock_request": [],  # mock request接口，item结构为{rule: {}, success or fail}, 同app.mock_request参数
-    "auto_authorize": False,  # 自动处理授权弹窗
-    "audits": None,  # 开启体验评分，仅在IDE生效, None为不改变
-    "teardown_snapshot": False,  # teardown快照，纪录page.data & page.wxml
-    "mock_images_dir": Path(""),  # 需要进行"上传"操作的图片放置的目录
-    "mock_images": {},  # 需要进行"上传"操作的图片, key为图片名(标识用), value为base64格式的图片数据
-    "need_perf": False,  # 需要性能数据
-    "appid": None,  # 小程序appid
+    "debug": False,                             # debug模式
+    "base_dir": os.path.abspath(os.getcwd()),   # 如果没有配置, 默认工作目录, 如果通过文件生成则为文件所在目录
+    "platform": "ide",                          # 平台: ide, android, ios
+    "app": "wx",                                # 承载的app: wx
+    "debug_mode": "debug",                      # 日志级别
+    "close_ide": False,                         # 是否关闭IDE
+    # "assert_capture": True,                   # 断言时是否截图, 不再对外. 仍可使用, 如只想setup&teardown时截图, 可以配置auto_capture: auto & assert_capture: false
+    # "framework_capture": True,                # setup, teardown时自动截图
+    # "error_capture": True,                    # case报错时自动截图
+    "auto_capture": "auto",                     # auto: setup, teardown, assert时自动截图. error: 只有case报错时自动截图. assert: 断言时自动截图. False/"": 不截图
+    "auto_relaunch": True,                      # case开始时是否回到主页
+    "device_desire": {},                        # 真机调试配置
+    "account_info": {},                         # 账号配置
+    "report_usage": True,                       # 是否需要报告
+    "remote_connect_timeout": 180,              # 真机调试中小程序在真机上打开的等待时间
+    "request_timeout": 60,                      # 自动化控制指令请求超时时间
+    "use_push": True,                           # 真机调试中是否使用推送形式打开小程序, false则需要扫调试二维码
+    "full_reset": False,                        # 每个测试class结束，是否释放调试链接
+    "outputs": None,                            # 测试产物输出路径
+    "enable_app_log": False,                    # 记录小程序日志
+    "enable_network_panel": False,              # 记录小程序网络请求
+    "project_path": None,                       # 小程序项目路径
+    "dev_tool_path": None,                      # 开发者工具命令行工具路径
+    "test_port": 9420,                          # 小程序自动化测试调试端口
+    "mock_native_modal": {},                    # 仅在IDE生效, mock所有会有原生弹窗的接口
+    "mock_request": [],                         # mock request接口，item结构为{rule: {}, success or fail}, 同app.mock_request参数
+    "auto_authorize": False,                    # 自动处理授权弹窗
+    "audits": None,                             # 开启体验评分，仅在IDE生效, None为不改变
+    "teardown_snapshot": False,                 # teardown快照，纪录page.data & page.wxml
+    "mock_images_dir": Path(""),                # 需要进行"上传"操作的图片放置的目录
+    "mock_images": {},                          # 需要进行"上传"操作的图片, key为图片名(标识用), value为base64格式的图片数据
+    "need_perf": False,                         # 需要性能数据
+    "appid": None,                              # 小程序appid
 }
 
 
 def get_log_level(debug_mode):
     return {
         "info": logging.INFO,
         "debug": logging.DEBUG,
@@ -66,14 +69,37 @@
                         v = Path(v)
                     else:
                         v = Path(os.path.abspath(os.path.join(
                             from_dict.get("base_dir") or default_config["base_dir"],
                             v
                         )))
                 default[k] = v
+        # 特殊处理一下capture相关字段
+        def setValue(key: str, value: bool):
+            nonlocal default
+            # 如果default[key]已经是bool类型, 则不修改原属性
+            if isinstance(default.get(key), bool):
+                return
+            default[key] = value
+
+        for mode in (default["auto_capture"] or "").split(","):
+            if mode == "auto":
+                setValue("framework_capture", True)
+                setValue("error_capture", False)  # teardown时截图就不需要错误截图了
+                setValue("assert_capture", True)  # 默认开启
+            elif mode == "error":
+                setValue("error_capture", True)
+                setValue("framework_capture", False)
+            elif mode == "assert":
+                setValue("assert_capture", True)
+        else:
+            setValue("framework_capture", False)
+            setValue("error_capture", False)
+            setValue("assert_capture", False)
+            
         for k, v in default.items():
             setattr(self, k, v)
         super(MiniConfig, self).__init__(self.__dict__)
 
     def __getattr__(self, __k):
         try:
             return self[__k]
```

### Comparing `minium-1.3.dev2/minium/framework/miniddt.py` & `minium-1.4.0/minium/framework/miniddt.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/minilimit.py` & `minium-1.4.0/minium/framework/minilimit.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/miniprogram.py` & `minium-1.4.0/minium/framework/miniprogram.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/miniresult.py` & `minium-1.4.0/minium/framework/miniresult.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/minisuite.py` & `minium-1.4.0/minium/framework/minisuite.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
                     try:
                         self.__suite_json = json.loads(content.decode("utf8"))  # use utf8 encoding
                     except UnicodeDecodeError:
                         self.__suite_json = json.loads(content.decode("gbk"))
                 else:
                     self.__suite_json = json.loads(path_or_dict)
             except JSONDecodeError as e:
-                raise MiniParamsError(f"Suite param {path_or_dict} not file neither dict or formatted json string: {e}")
+                raise MiniParamsError(f"Suite param {path_or_dict} not file neither dict or formatted json string: {e}") from e
         elif isinstance(path_or_dict, dict):
             self.__suite_json = path_or_dict
         else:
-            raise MiniParamsError("Suite param not file neither dict or formatted json string")
+            raise MiniParamsError(f"Suite param should string or dict, not {type(path_or_dict).__name__}")
         self.__success_pkg = set()
         self.__fail_pkg = {}
 
     def __getattribute__(self, __name: str):
         try:
             return super().__getattribute__(__name)
         except AttributeError:
```

### Comparing `minium-1.3.dev2/minium/framework/minitest.py` & `minium-1.4.0/minium/framework/minitest.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,31 +9,36 @@
 import inspect
 
 import minium
 import minium.miniprogram.base_driver.minium_log
 import minium.native
 from minium.native.exception import *
 from .miniconfig import MiniConfig
-from .assertbase import AssertBase
+from .assertbase import AssertBase, HookAssert
 from .logcolor import *
 from .exception import *
 from ..utils.utils import retry, catch
 from ..utils.injectjs import getInjectJsCode
 from .miniprogram import MiniProgram
+from ..miniprogram import Minium
+from ..miniprogram.base_driver.app import App
+from ..native import BaseNative
+from typing import Tuple
 
 # import matplotlib.pyplot as plt
 
 logger = logging.getLogger("minium")
 
-g_minium = None
-g_native = None
+g_minium: Minium = None
+g_native: BaseNative = None
 g_log_message_list = []
 g_network_message_dict = {}  # 记录请求消息
 g_network_req_cache = {}  # 记录请求体消息(降低重复请求消息量)
 g_network_resp_cache = {}  # 记录请求返回消息(降低重复请求消息量)
+FRAMEWORK_RETRY = 1  # case失败, 框架针对错误进行重试的次数
 
 
 def full_reset():
     """
     在整个测试流程结束之后调用
     1. miniProgram 部分同 reset_minium()
     2. native 部分
@@ -61,34 +66,35 @@
     1. miniProgram 部分 release
         1.1 非 ide 运行退出小程序
     2. 释放所有观察者的事件监听
     3. 销毁与 ide 的连接
     :return:
     """
     global g_minium
-    g_minium.release()
+    if g_minium:
+        g_minium.release()
     g_minium = None
 
 
-def get_native(cfg: MiniConfig):
+def get_native(cfg: MiniConfig) -> BaseNative:
     """
     native 部分完全由配置中的 platform 参数控制
     为了确保不会过多地重启微信，已存在 g_native 则不创建,
     teardown 的时候也不会 release
     :param cfg: 配置
     :return:
     """
     global g_native
     if g_native is None:
         g_native = minium.native.get_native_driver(cfg.platform, cfg)
         g_native.start_wechat()
     return g_native
 
 
-def get_minium(cfg: MiniConfig):
+def get_minium(cfg: MiniConfig) -> Minium:
     """
     miniProgram 部分每次 classTearDown 是否 release 由配置 close_ide 控制
     初始化有如下工作：
         1. 处理配置
         2. 如果配置了 project_path 则启动 ide
         3. 连接 ide
         4. 根据配置 platform 判断是否需要远程调试
@@ -118,21 +124,21 @@
         if cfg.enable_network_panel:
             # 没有uuid库，随便注入一个随机ID库
             g_minium.app._evaluate_js("uuid")
             g_minium.app.expose_function("mini_request_callback", request_callback)
             g_minium.app.expose_function("mini_send_request", send_request)
             g_minium.app._evaluate_js("networkPannel")
 
-        if cfg.platform == "ide":
+        if cfg.platform == "ide" and g_native:
             g_native.mini = g_minium  # ide native接口通过minium实现
 
     return g_minium
 
 
-def init_miniprogram(cfg: MiniConfig):
+def init_miniprogram(cfg: MiniConfig) -> Tuple[BaseNative, Minium, MiniProgram]:
     """
     初始化小程序
     1. 初始化native
     2. 启动微信
     3. 拉起小程序
     4. 获取必要的小程序信息
     """
@@ -181,29 +187,28 @@
     if msg_id not in g_network_message_dict:
         g_network_message_dict[msg_id] = {"timestamp": time.time() * 1000}
     g_network_message_dict[msg_id]["start_timestamp"] = ms
     g_network_message_dict[msg_id]["request"] = json.loads(obj)
 
 
 def request_callback(message):
-    [msg_id, res, ms, hash_id] = message["args"]
+    [msg_id, res, ms, hash_id, mocked] = message["args"]
     if hash_id and res:  # 传了原始response res, 记录起来
         g_network_resp_cache[hash_id] = {"res": res, "timestamp": time.time()}
     elif hash_id and hash_id in g_network_resp_cache:
         res = g_network_resp_cache[hash_id]["res"]
         g_network_resp_cache[hash_id]["timestamp"] = time.time()
     if msg_id not in g_network_message_dict:
         g_network_message_dict[msg_id] = {"timestamp": time.time() * 1000}
     g_network_message_dict[msg_id]["end_timestamp"] = ms
     g_network_message_dict[msg_id]["response"] = json.loads(res)
+    g_network_message_dict[msg_id]["mocked"] = bool(mocked)
 
-
-class MetaMiniTest(type):
+class MetaMiniTest(HookAssert):
     def __new__(cls, name, bases, attrs):
-        cls.app = MetaMiniTest.app
         return super(MetaMiniTest, cls).__new__(cls, name, bases, attrs)
 
     @property
     def app(cls):
         if not inspect.isclass(cls):
             cls = type(cls)
         return cls._app or (cls.mini and cls.mini.app)
@@ -212,21 +217,27 @@
     def app(cls, value):
         if not inspect.isclass(cls):
             cls = type(cls)
         cls._app = value
 
 
 class MiniTest(AssertBase, metaclass=MetaMiniTest):
-    mini = None
-    native = None
+    mini: Minium = None
+    native: BaseNative = None
     appId = ""
     appName = ""
     logger = logger
 
-    _app = None
+    _app: App = None
+
+    def __init__(self, methodName: str = "runTest") -> None:
+        super().__init__(methodName)
+        # 这个case是否需要重试, 目前重试原则为
+        # 1. case运行过程中遇到断连的情况
+        self.__will_retry = None  
 
     @property
     def app(self) -> minium.App:
         return self._app or (self.mini and self.mini.app)
 
     @app.setter
     def app(self, value):
@@ -259,108 +270,142 @@
         if cls.CONFIG.full_reset:
             logger.info("full reset")
             if cls.CONFIG.audits and cls.mini and hasattr(cls.mini, "stop_audits"):
                 cls.mini.stop_audits(
                     os.path.join(cls.CONFIG.outputs, "audits_%s.html" % cls.__name__)
                 )
             full_reset()
+            cls.mini = None
+            cls.native = None
             return
         if g_minium and cls.CONFIG.close_ide and cls.CONFIG.platform == "ide":
             logger.info("close ide and reset minium")
             if cls.CONFIG.audits and cls.mini and hasattr(cls.mini, "stop_audits"):
                 cls.mini.stop_audits(
                     os.path.join(cls.CONFIG.outputs, "audits_%s.html" % cls.__name__)
                 )
             reset_minium()
+            cls.mini = None
+
+    def _check_debug_connection(self) -> ResetError:
+        """检查调试通道
+
+        :return None or Exception: None for ok
+        """
+        if self.native:
+            if not self.native.check_connection():
+                self.logger.warning("check native connection error, relaunch app")
+                return ResetError.RELAUNCH_APP
+        if self.mini: # 小程序异常退出和链接断连都会自动重连和重新拉起
+            if self.mini.is_app_relaunching:
+                self.logger.warning("app is relaunching, wait for it")
+                e = self.mini.wait_app_relaunch()
+                if e:
+                    self.logger.warning(e)
+                    return ResetError.RELAUNCH_APP
+            if self.mini.connection and self.mini.connection.is_reconnecting:
+                self.logger.warning("connection is reconnecting, wait for it")
+                e = self.mini.connection.wait_reconnect()
+                if e:
+                    self.logger.warning(e)
+                    return ResetError.RELAUNCH_APP
+        return ResetError.OK
+    
+    def _update_miniprogram(self, native, mini):
+        self.logger.debug(
+            "start update miniprogram, class is: %s" % self.__class__.__name__
+        )
+        self.__class__.native = native
+        self.__class__.mini = mini
+        self.mini = mini
+        self.native = native
+        self.logger.debug(
+            "finish update miniprogram, current native: %s, minium: %s"
+            % (id(self.mini), id(self.native))
+        )
+
+    def init_miniprogram(self):
+        """case中重新实例化小程序
+        """
+        try:
+            native, mini, _ = init_miniprogram(self.__class__.CONFIG)
+        except:
+            self._update_miniprogram(g_native, g_minium)
+            raise
+        else:
+            self._update_miniprogram(native, mini)
 
     def _miniSetUp(self):
         super(MiniTest, self)._miniSetUp()
         self._is_perf_setup = False
         self._is_audits_setup = False
         logger.info("=========Current case: %s=========" % self._testMethodName)
+        if self.__will_retry is not None:
+            self.logger.warning(f"第{FRAMEWORK_RETRY-self.__will_retry}次重试")
         logger.info(
             "package info: %s, case info: %s.%s"
             % (
                 self.results.get("module", ""),
                 self.__class__.__name__,
                 self._testMethodName,
             )
         )
         if self.test_config.only_native:
             logger.info(f"Only native: {self.test_config.only_native}, setUp complete")
             return
         else:
-            if self.test_config.auto_relaunch:
+            check_result = self._check_debug_connection()
+            if check_result != ResetError.OK:  # 调试通道不通
+                self.logger.warning("check debug connection fail")
+                if check_result == ResetError.RELAUNCH_APP:
+                    full_reset()
+                    self._update_miniprogram(None, None)
+                elif check_result == ResetError.RELAUNCH_MINIPROGRAM:
+                    reset_minium()
+                    self._update_miniprogram(self.native, None)
+                self.init_miniprogram()
+
+            if check_result == ResetError.OK and self.test_config.auto_relaunch:
                 ret = self.native and self.native.back_to_miniprogram()
                 if ret and ret != ResetError.OK:
                     if ret == ResetError.RELAUNCH_APP:
                         self.logger.warning(
                             "back_to_miniprogram error, reset app, post native: %s, minium: %s"
                             % (id(self.mini), id(self.native))
                         )
                         full_reset()
-                        self.logger.debug(
-                            "start init_miniprogram, class is: %s"
-                            % self.__class__.__name__
-                        )
-                        native, mini, miniprogram = init_miniprogram(
-                            self.__class__.CONFIG
-                        )
-                        self.__class__.native = native
-                        self.__class__.mini = mini
-                        self.logger.debug(
-                            "end init_miniprogram, class is: %s"
-                            % self.__class__.__name__
-                        )
-                        self.mini = mini
-                        self.native = native
-                        self.logger.debug(
-                            "finish init_miniprogram, current native: %s, minium: %s"
-                            % (id(self.mini), id(self.native))
-                        )
+                        self._update_miniprogram(None, None)
+                        self.init_miniprogram()
                     elif ret == ResetError.RELAUNCH_MINIPROGRAM:
                         self.logger.warning(
                             "back_to_miniprogram error, reset miniprogram, post minium: %s"
                             % id(self.native)
                         )
                         reset_minium()
-                        self.logger.debug(
-                            "start init_miniprogram, class is: %s"
-                            % self.__class__.__name__
-                        )
-                        native, mini, miniprogram = init_miniprogram(
-                            self.__class__.CONFIG
-                        )
-                        self.__class__.native = native
-                        self.__class__.mini = mini
-                        self.logger.debug(
-                            "end init_miniprogram, class is: %s"
-                            % self.__class__.__name__
-                        )
-                        self.mini = mini
-                        self.logger.debug(
-                            "finish init_miniprogram, current minium: %s"
-                            % id(self.mini)
-                        )
+                        self._update_miniprogram(self.native, None)
+                        self.init_miniprogram()
                 self.app.go_home()
         # 体验评分是个整体的评价，每个case太短了，没意义
         # if self.test_config.audits:
         #     self._is_audits_setup = self._setup_audits()
-        if self.test_config.assert_capture:
-            retry(2)(self.capture)("setup")
+        self._framework_capture("setup")
         self._is_perf_setup = self._setup_perf()
+        # update start_timestamp
+        self.results["start_timestamp"] = time.time()
+        logger.info("=========case: %s start=========" % self._testMethodName)
 
     def _setup_perf(self):
         self._get_perf_flag = False
         self.perf_data = ""
         if self.test_config.need_perf:
             # logger.debug("_setup_perf")
             self._get_perf_flag = bool(self.native.start_get_perf(timeinterval=0.8))
         return True
 
+    @catch
     def _teardown_perf(self):
         """
         落地性能相关数据
         """
         if not self._is_perf_setup:
             return
         perf_init = {
@@ -467,14 +512,15 @@
         if not self._is_audits_setup:
             return
         if self.start_audit:
             self.stop_audits()
         self.results["audit_html"] = self.audit_html
         self.results["audit_json"] = self.audit_json
 
+    @catch
     def _teardown_app_log(self):
         """
         落地小程序相关的log
         """
         global g_log_message_list, g_network_message_dict
         # 落地小程序log
         weapp_path = "weapp.log"
@@ -505,43 +551,73 @@
                     msg["request"] = None
                 if not msg.get("end_timestamp"):
                     msg["end_timestamp"] = msg["timestamp"]
                     msg["response"] = None
                 f.write(json.dumps(msg, ensure_ascii=False) + "\n")
         self.results["request_log_path"] = request_path
 
-    def _miniTearDown(self):
-        logger.debug("=========Current case Down: %s=========" % self._testMethodName)
+    def _teardown_snapshot(self):
         try:
-            # 更新小程序专属的数据
-            self._teardown_perf()
-            # if self.test_config.audits:
-            #     self._teardown_audits()
-            self._teardown_app_log()
-            if self.test_config.assert_capture:
-                retry(2)(self.capture)("teardown")
-            # todo: 加参数说明是否需要保存页面参数
             if self.test_config.teardown_snapshot:
-                self.results["page_data"] = self.page.data
                 self.results["page_wxml"] = self.page_wxml
-            elif self._outcome:
-                sys_info = self._get_error_info()[0]
-                if sys_info:  # case失败了
-                    if sys_info[0] is MiniElementNotFoundError:  # 找不到元素, 把wxml拿回来帮助用户排查
-                        self.results["page_wxml"] = self.page_wxml
+                self.results["page_data"] = self.page.data
         except Exception as e:
             logger.exception(e)
             self.results["page_data"] = None
             self.results["page_wxml"] = ""
-        finally:
-            super(MiniTest, self)._miniTearDown()
+
+    @catch
+    def _check_case_error(self, error: Exception):
+        """检查失败的case的错误, 决定是否需要重试或者获取更多信息
+
+        :param Exception error: case运行产生的错误
+        """
+        if not error:
+            return
+        if isinstance(error, (MiniConnectionClosedError, MiniReConnectSvrError)):
+            # 因为断连而产生的指令超时, 可尝试重试{1}次
+            if self.__will_retry is None:
+                self.__will_retry = FRAMEWORK_RETRY
+            return
+        if isinstance(error, MiniElementNotFoundError) and not self.test_config.teardown_snapshot:
+            # 找不到元素, 把wxml拿回来帮助用户排查. 如果配置了`teardown_snapshot`, 则已经获取过不需要再获取
+            self.results["page_wxml"] = self.page_wxml
+            return
+
+    def _miniTearDown(self):
+        logger.debug("=========Current case Down: %s=========" % self._testMethodName)
+        self._framework_capture("teardown")
+        sys_info = self._get_error_info()[0]
+        if sys_info:  # case失败了
+            self._check_case_error(sys_info[1])
+        # 更新小程序专属的数据
+        self._teardown_perf()
+        self._teardown_app_log()
+        self._teardown_snapshot()
+        super(MiniTest, self)._miniTearDown()
+
+    def _cleanup_before_retry(self):
+        # 清理一下输出路径(等于删除上一个结果)
+        if self.test_config.case_output and os.path.isdir(self.test_config.case_output):
+            shutil.rmtree(self.test_config.case_output)
+
+    def run(self, result=None):
+        ret = super().run(result)
+        if self.__will_retry is None:
+            return ret
+        while self.__will_retry > 0:
+            self.__will_retry -= 1
+            self._cleanup_before_retry()
+            self.logger.warning(f"第{FRAMEWORK_RETRY-self.__will_retry}次重试")
+            ret = super().run(result)
+        return ret
 
     @property
     def page(self) -> minium.Page:
-        return self.mini.app.get_current_page()
+        return self.mini.app.current_page
 
     @property
     def page_wxml(self) -> str:
         if not self.mini:
             return ""
         if self.mini.sdk_version > "2.19.5":
             wxml = self.page.get_element("/*").outer_wxml
@@ -550,14 +626,36 @@
         if wxml:
             filename = datetime.datetime.now().strftime("%d%H%M%S.wxml")
             filepath = self.wrap_filename(filename)
             with open(filepath, "w", encoding="utf8") as fd:
                 fd.write(wxml)
             return filename
         return wxml
+    
+    @catch
+    @retry(2)
+    def _framework_capture(self, name=""):
+        """框架截图, 尝试两次, 不报错
+
+        :param str name: 截图文件名, defaults to ""
+        """
+        if not self.test_config.framework_capture:
+            return ""
+        return self.capture(name)
+    
+    @catch
+    @retry(2)
+    def _error_capture(self, error: Exception):
+        """报错截图, 尝试两次, 不报错
+
+        :param Exception error: 具体报错, 截图文件名由报错类名定义
+        """
+        if not self.test_config.error_capture:
+            return ""
+        return self.capture(error.__class__.__name__)
 
     def capture(self, name=""):
         """
         :param name: 图片名称
         :return: str: image_path or ""
         """
         if name:
@@ -582,14 +680,29 @@
             )
             self.add_screen(name, path, page_path)
             return path
         else:
             logger.warning("%s not exists", path)
         return ""
 
+    def tap_capture(self, name, page_id):
+        """
+        点击截图
+        :param name: 截图文件名
+        :param page_id: 点击元素所属的页面id
+        """
+        raise NotImplementedError("仅云测支持")
+    
+    def tap_mark(self, name: str, point: Tuple, page_id):
+        """
+        给截图标记点击的点
+        :return: bool
+        """
+        raise NotImplementedError("仅云测支持")
+
     def stop_audits(self, format=None):
         """
         获取体验评分
         :return: 体验评分报告
         """
         format = ["html", "json"] if format is None else format
         ret = self.app._stop_audits()
@@ -620,14 +733,27 @@
                     j_f.write(json_result)
                 j_f.close()
                 self.audit_json = audits_json_file
                 logger.info("success create Audits.json")
             else:
                 pass
 
+    # 录制回放专用接口
+    def mark_step_start(self, key, **kwargs):
+        """录制回放步骤标记
+        1. 打日志
+        2. 额外信息加入`result.step_info`中
+
+        :param str key: 步骤键名
+        """
+        self.logger.debug("[minitest replay] %s" % key)
+        self.results.step_info.append(
+            {"key": key, "timestamp": int(time.time()), **kwargs}
+        )
+
     # 小程序定制化的校验
     def assertPageData(self, data, msg=None):
         """
 
         :param data:
         :param msg:
         :return:
```

### Comparing `minium-1.3.dev2/minium/framework/report.py` & `minium-1.4.0/minium/framework/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                             }
                         )
                         screen_info.sort(key=lambda x: x["ts"])
                         case_info["screen_info"] = screen_info
     return unfinished_case_datas
 
 
-def get_case_summary(case_datas):
+def get_case_summary(case_datas, unfinished_case_datas=None):
     success = 0
     failed = 0
     error = 0
     costs = 0
     pkg_info = {}
     detail = []
     start_time = None
@@ -270,14 +270,32 @@
                     "failed": 1 if c["is_failure"] else 0,
                     "error": 1 if c["is_error"] else 0,
                     "start_time": c["start_timestamp"],
                     "end_time": c.get("stop_timestamp", c["start_timestamp"]),
                     "costs": c.get("stop_timestamp", c["start_timestamp"])
                     - c["start_timestamp"],
                 }
+    if unfinished_case_datas:
+        for package_name in unfinished_case_datas:
+            for class_name in unfinished_case_datas[package_name]:
+                for case_name in unfinished_case_datas[package_name][class_name]:
+                    item = unfinished_case_datas[package_name][class_name][case_name]
+                    if item.get("start_timestamp"):
+                        start_time = (
+                            item["start_timestamp"]
+                            if start_time is None
+                            else min(item["start_timestamp"], start_time)
+                        )
+                    if item.get("stop_timestamp"):
+                        end_time = (
+                            item.get("stop_timestamp", item["start_timestamp"])
+                            if end_time is None
+                            else max(item.get("stop_timestamp", item["start_timestamp"]), end_time)
+                        )
+
     for package in pkg_info:
         pkg_info[package]["start_time"] = formatTimeFromTimestamp(
             "%Y/%m/%d %H:%M:%S", pkg_info[package]["start_time"]
         )
         pkg_info[package]["end_time"] = formatTimeFromTimestamp(
             "%Y/%m/%d %H:%M:%S", pkg_info[package]["end_time"]
         )
@@ -302,15 +320,16 @@
     case_datas = get_case_datas(filenames)
 
     # unfinished cases
     unfinished_case_datas = get_unfinished_case_datas(unfinished_filenames)
 
     # summary
     success, failed, error, costs, start_time, end_time, detail = get_case_summary(
-        case_datas
+        case_datas,
+        unfinished_case_datas
     )
 
     summary = {
         "case_num": len(case_datas),
         "success": success,
         "failed": failed,
         "error": error,
```

### Comparing `minium-1.3.dev2/minium/framework/session.py` & `minium-1.4.0/minium/framework/session.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/tools/report_issue.py` & `minium-1.4.0/minium/framework/tools/report_issue.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/framework/wording.py` & `minium-1.4.0/minium/framework/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/miniprogram/__init__.py` & `minium-1.4.0/minium/miniprogram/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 """
 Author:         lockerzhang
 Filename:       __init__.py
 Create time:    2019/11/28 15:59
 Description:
 
 """
-
+import typing
 from .wx_minium import WXMinium
 from .qq_minium import QQMinium
 
 
 # application
 APP_WX = "wx"
 APP_QQ = "qq"
 
 APP = {"wx": WXMinium, "qq": QQMinium}
 
-
-def get_minium_driver(conf, *args, **kwargs):
+Minium = typing.Union[WXMinium, QQMinium]
+def get_minium_driver(conf, *args, **kwargs) -> Minium:
     if conf is None:
         conf = {}
     application = conf.get("app", APP_WX)
     if application not in APP.keys():
         raise RuntimeError("the 'app' in your config file is not in predefine, not support yet")
     return APP[application](conf, *args, **kwargs)
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/app.py` & `minium-1.4.0/minium/miniprogram/base_driver/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 @Author: lockerzhang
 @LastEditors: lockerzhang
 @Description: 小程序层面的操作(包含 web 和 Native)
 @Date: 2019-03-11 14:41:43
 @LastEditTime: 2019-06-05 16:30:44
 """
 import typing
+import types
 from enum import Enum
 
 from minium.utils.utils import AsyncCondition
 from .page import Page
-from .minium_object import MiniumObject
+from .minium_object import MiniumObject, RetryableApi
 from ...framework.exception import *
 from ...utils.injectjs import getInjectJsCode, JsMode
 from ...utils.platforms import *
 from ...utils.emitter import ee
 from ...utils.eventloop import event_loop
-from ...utils.utils import get_result
-from .callback import AsyncCallback
+from ...utils.utils import get_result, WaitTimeoutError, retry, catch
+from .callback import AsyncCallback, Callback
 import os
 import json
 import threading
 import base64
 import io
 import time
 import datetime
@@ -46,15 +47,160 @@
 
 
 class MockCloudCallType(Enum):
     ALWAYS = 0
     ONCE = 1
 
 
-class App(MiniumObject):
+class RouteCommand:
+    def __init__(
+        self, open_type, path, route_done_lock=None, default_route_result=None
+    ) -> None:
+        """页面跳转指令
+
+        :param str open_type: 跳转操作: navigateTo/redirectTo/reLaunch/switchTab
+        :param str path: 路径: /pages/index/index?a=b&c=1
+        :param AsyncCondition route_done_lock: onAppRouteDone回调释放的异步锁, defaults to None(不需要等待route done)
+        :param bool default_route_result: _description_, defaults to None
+        """
+        self.open_type = open_type
+        self.path = path
+        self._open_id = None  # 调用异步接口返回的请求id
+
+        self._async_msg_lock: AsyncCondition = route_done_lock
+        self._open_callback = AsyncCallback(event_loop)
+        self._route_changed = None
+        self._error: Exception = None
+
+    @property
+    def open_id(self):
+        return self._open_id
+
+    @open_id.setter
+    def open_id(self, value):
+        if value == self._open_id:
+            return
+        self._open_id = value
+        ee.once(self._open_id, self.open_callback)
+
+    def on_connect_state_change(self, value: bool, error: Exception):
+        if not value:  # break
+            self._error = error
+
+    async def _wait_msg_lock(self, timeout=None):
+        await self._async_msg_lock.acquire()
+        ret = await self._async_msg_lock.wait(timeout=timeout)
+        self._async_msg_lock.release()
+        return ret
+
+    async def _wait_route_changed_async(self, timeout=None) -> bool:
+        if not timeout:
+            timeout = 5
+
+        ret = await self._wait_msg_lock(timeout)
+        return ret
+
+    def __enter__(self):
+        ee.on("connect_state_change", self.on_connect_state_change)
+        return self
+
+    def __exit__(self, *args):
+        ee.remove_listener("connect_state_change", self.on_connect_state_change)
+
+    def listen_route_change(self, timeout):
+        if not self._async_msg_lock:
+            return
+        self._route_changed = event_loop.run_coroutine(
+            self._wait_route_changed_async(timeout + 5)
+        )
+        return self._route_changed
+
+    def open_callback(self, *args):
+        return self._open_callback.callback(*args)
+
+    def cancel_open_callback(self):
+        if self._open_id:
+            ee.remove_listener(self._open_id, self.open_callback)
+        return self._open_callback.cancel()
+
+    def get_open_result(self, timeout):
+        """获取打开页面操作结果"""
+        try:
+            if self._open_callback.wait_called(timeout):
+                return self._open_callback.get_result()
+            raise MiniTimeoutError(
+                f"[{self._open_id}][{self.open_type}] receive from remote timeout"
+            )
+        except MiniClientOfflineError as co:
+            raise MiniTimeoutCauseByClientOffline(str(co)) from co
+        except MiniConnectionClosedError as cc:
+            raise MiniTimeoutCauseByConnectionBreakError(str(cc)) from cc
+
+    def get_route_result(self, timeout):
+        if not self._async_msg_lock:
+            # 不需要等待则认为已经route done
+            return True
+        if self._error:
+            raise self._error
+        try:
+            if get_result(self._route_changed, timeout):
+                return True
+            return False
+        except WaitTimeoutError as wt:
+            if self._error:
+                if isinstance(self._error, MiniClientOfflineError):
+                    raise MiniTimeoutCauseByClientOffline(str(self._error)) from wt
+                if isinstance(self._error, MiniConnectionClosedError):
+                    raise MiniTimeoutCauseByConnectionBreakError(
+                        str(self._error)
+                    ) from wt
+                raise self._error from wt
+            if self.open_type == "switchTab":
+                # switchTab方法可能没有on app route done
+                return False
+            raise wt
+        except MiniClientOfflineError as co:
+            raise MiniTimeoutCauseByClientOffline(str(co)) from co
+        except MiniConnectionClosedError as cc:
+            raise MiniTimeoutCauseByConnectionBreakError(str(cc)) from cc
+
+
+class App(MiniumObject, metaclass=RetryableApi):
+    __RETRY_API__ = [
+        "enable_log",
+        "screen_shot",
+        "expose_function",
+        "get_all_pages_path",
+        "get_current_page",
+        # "get_page_stack",  # _page_stack方法重试
+        "wait_util",
+        "hook_wx_method",
+        "release_hook_wx_method",
+        "hook_current_page_method",
+        "restore_wx_method",
+        "restore_request",
+        "mock_request",
+        # "mock_request_once",  #如果重试, 会影响once的逻辑
+        "restore_call_function",
+        "mock_call_function",
+        # "mock_call_function_once",  #如果重试, 会影响once的逻辑
+        "restore_call_container",
+        "mock_call_container",
+        # "mock_call_container_once",  #如果重试, 会影响once的逻辑
+        "edit_editor_text",
+        "reflesh_mocked_images",
+        "mock_choose_images",  # 重试可能遇上前面已经mock的情况, 但已经兼容
+        "mock_choose_image_with_name",
+        # protect(common method)
+        "_mock_wx_method",  # 各类mock方法都使用到
+        "_page_stack",
+        # private
+        "__get_pages_config",
+    ]
+
     def __init__(self, connection, relaunch=False, native=None, platform="ide"):
         """
         创建一个 APP 实例
         :param connection:
         """
         super().__init__()
         self.connection = connection
@@ -62,15 +208,15 @@
         self.platform = platform
         self.js_mode: JsMode = (
             JsMode.JUST_ES5 if platform in [OS_ANDROID, OS_IOS] else JsMode.ALL
         )  # 真机调试2.0环境下只支持es5语法
         self._msg_lock = threading.Condition()
         self._async_msg_lock = AsyncCondition(loop=event_loop)
         self._is_log_enable = False
-        self.main_page_path = None
+        self._main_page_path = None
         self.route_return_page = None
         self.route_return_page_update_time = None  # 监听到页面变化后由于是异步通信, 有可能出现两个相近信息重复顺序调乱
         self._appid = None
         self._current_page = None  # 只有调用 get_current_page 和 监听到 _on_route_changed 回调时更新
         self._mocked_images = None
         self._mocked_images_dir = None
         self._mocked_images_data = {}
@@ -82,15 +228,15 @@
         )  # 是否已经注入过了, 注入过的环境不需要重复注入, 防止出现多次回调等预期之外的情况
         self.pages = []
         self.tabbar_pages = {}
         self.__get_pages_config()
         if not self.__is_injected and self.js_mode is JsMode.JUST_ES5:  # 注入一些垫片
             self._evaluate_js("helpers")
         if relaunch:
-            self.go_home()
+            self.relaunch(self.main_page_path.path, self.main_page_path.query)
 
     @property
     def app_id(self):
         if not self._appid:
             self._appid = self._get_account_info_sync().result.result.miniProgram.appId
         return self._appid
 
@@ -104,14 +250,23 @@
         是否已经注入过, 如果没有, 则设置并进行注入操作
         """
         if self.__is_injected:
             return True
         self.__is_injected = True
         return False
 
+    @property
+    def main_page_path(self):
+        if self._main_page_path is None:
+            options = self._get_launch_options_sync().result.result
+            if options.path == "":
+                raise MiniLaunchError("get launch options failed")
+            self._main_page_path = Page(None, options.path, options.query, None)
+        return self._main_page_path
+
     def _evaluate_js(
         self,
         filename,
         args=None,
         sync=True,
         default=None,
         code_format_info=None,
@@ -129,21 +284,22 @@
         打开日志
         每次调用, 都会新增一个回调, 最好记录一下已经调用过
         """
         if not self._is_log_enable:
             self.connection.send("App.enableLog")
             self._is_log_enable = True
 
+    @catch(MiniClientOfflineError)
     def exit(self):
         """
         退出小程序
         :return: None
         """
         setattr(self.connection, "_is_close_app_by_cmd", True)
-        self.connection.send("App.exit")
+        self.connection.send_async("App.exit", ignore_response=True)
 
     def get_account_info_sync(self):
         """
         获取账号信息
         :return:
         """
         return self._get_account_info_sync()
@@ -250,54 +406,62 @@
         :param plugin_appid: 调用插件[${appid}]中的方法, auto时自动获取当前页面是否插件页
         :return:
         """
         if plugin_appid == "auto":
             plugin_appid = (self._current_page or self.get_current_page()).plugin_appid
         return self._call_wx_method(method=method, args=args, plugin_appid=plugin_appid)
 
-    def call_wx_method_async(self, method, args=None, plugin_appid="auto"):
+    def call_wx_method_async(
+        self, method, args=None, plugin_appid="auto", ignore_response=False
+    ):
         """
         调用 wx 的方法, 返回异步message id
         :param method:
         :param args:
         :param plugin_appid: 调用插件[${appid}]中的方法, auto时自动获取当前页面是否插件页
         :return: str(message_id)
         """
         if plugin_appid == "auto":
             plugin_appid = (self._current_page or self.get_current_page()).plugin_appid
         return self._call_wx_method(
-            method=method, args=args, plugin_appid=plugin_appid, sync=False
+            method=method,
+            args=args,
+            plugin_appid=plugin_appid,
+            sync=False,
+            ignore_response=ignore_response,
         )
 
     def get_all_pages_path(self):
         """
         获取所有已配置的页面路径
         :return:
         """
         return self._evaluate_js("getAllPagesPath")
 
     def __get_pages_config(self):
         """
         获取所有page相关信息
         """
         try:
-            ret = self.evaluate("""function(){return {"pages": __wxConfig.pages, "tabBar": __wxConfig.tabBar && __wxConfig.tabBar.list} }""", sync=True).result.result
+            ret = self.evaluate(
+                """function(){return {"pages": __wxConfig.pages, "tabBar": __wxConfig.tabBar && __wxConfig.tabBar.list} }""",
+                sync=True,
+            ).result.result
             self.pages = ret.get("pages", [])
             tabbar_list = ret.get("tabBar", None)
             if tabbar_list:
                 idx = 0
                 for tabbar in tabbar_list:
                     page_path = tabbar["pagePath"].rstrip(".html")
                     if not page_path.startswith("/"):
                         page_path = "/" + page_path
                     self.tabbar_pages[page_path] = tabbar
-                    self.tabbar_pages[page_path].update({
-                        "index": idx,
-                        "pagePath": page_path.lstrip("/")
-                    })
+                    self.tabbar_pages[page_path].update(
+                        {"index": idx, "pagePath": page_path.lstrip("/")}
+                    )
                     idx += 1
         except MiniAppError:
             return {}
         return ret
 
     def get_current_page(self) -> Page:
         """
@@ -311,28 +475,43 @@
                 raise Exception("Get current page fail, cause: %s" % ret.error)
             if not ret.result and cnt < 3:
                 # 返回信息有问题, 没拿到pageId等属性
                 return get_current_page(cnt + 1)
             return ret
 
         ret = get_current_page()
-        page = Page(
-            ret.result.pageId, ret.result.path, ret.result.query, self.connection
-        )
+        page = Page(ret.result.pageId, ret.result.path, ret.result.query, self)
         # 记录当前页面
         self._current_page = page
         return page
 
+    def evaluate(self, app_function: str, args=None, sync=False, desc=None):
+        """
+        向 app Service 层注入代码并执行
+        :param app_function:
+        :param args:
+        :param sync:
+        :param desc: 报错描述
+        :return:
+        """
+        return self._evaluate(
+            app_function=app_function, args=args, sync=sync, desc=desc
+        )
+
     def get_page_stack(self) -> typing.List[Page]:
         """
         获取当前小程序所有的页面
         :return: Page List
         """
         return self._page_stack()
 
+    # navigate_to不进行重试:
+    # 1. 小程序断线没有重试必要, 必须等待小程序重连。
+    # 2. ws链接断连在send的时候就已经检查并等待重连。
+    # 3. 如果是单纯没有回包, 不能确定指令是否已经生效, 如指令生效并重试, 会增加页面堆栈
     def navigate_to(self, url, params=None, is_wait_url_change=True):
         """
         以导航的方式跳转到指定页面, 但是不能跳到 tabbar 页面。支持相对路径和绝对路径, 小程序中页面栈最多十层
         支持相对路径和绝对路径
         /page/tabBar/API/index: 绝对路径,最前面为/
         tabBar/API/index: 相对路径, 会被拼接在当前页面的路径后面
         :param url:"/page/tabBar/API/index"
@@ -348,14 +527,16 @@
             )
         self.logger.info("NavigateTo: %s" % url)
         page = self._change_route_async("navigateTo", url, is_wait_url_change)
         if page != url.split("?")[0]:
             self.logger.warning("NavigateTo(%s) but(%s)" % (url, page.path))
         return page
 
+    # redirect_to因为不产生新的页面堆栈, ws断连引起的回报丢失可以尝试重试
+    @retry(2, (MiniTimeoutCauseByConnectionBreakError))
     def redirect_to(self, url, params=None, is_wait_url_change=True):
         """
         关闭当前页面, 重定向到应用内的某个页面。但是不允许跳转到 tabbar 页面
         :param url:"/page/tabBar/API/index"
         :param params: 页面参数
         :param is_wait_url_change: 是否等待页面变换完成
         :return:Page 对象
@@ -368,14 +549,16 @@
             )
         self.logger.info("RedirectTo: %s" % url)
         page = self._change_route_async("redirectTo", url, is_wait_url_change)
         if page != url.split("?")[0]:
             self.logger.warning("RedirectTo(%s) but(%s)" % (url, page.path))
         return page
 
+    # relaunch因为不产生新的页面堆栈, ws断连引起的回报丢失可以尝试重试
+    @retry(2, (MiniTimeoutCauseByConnectionBreakError))
     def relaunch(self, url, params=None, is_wait_url_change=True):
         """
         关闭所有页面, 打开到应用内的某个页面
         :param url: "/page/tabBar/API/index"
         :return:Page 对象
         """
         if params:
@@ -405,30 +588,39 @@
         self.logger.info("NavigateBack from:%s" % page.path)
         self._call_wx_method("navigateBack", [{"delta": delta}])
         if self._route_changed():
             return self.route_return_page
         else:
             self.logger.warning("route has not change, may be navigate back fail")
 
-    def switch_tab(self, url, is_wait_url_change=True, is_click=False):
+    # switch_tab因为不产生新的页面堆栈, ws断连引起的回报丢失可以尝试重试
+    @retry(2, (MiniTimeoutCauseByConnectionBreakError))
+    def switch_tab(
+        self, url, is_wait_url_change=True, is_click=False, wait_route_done_time=15
+    ):
         """
         跳转到 tabBar 页面, 并关闭其他所有非 tabBar 页面
         :param url: "/page/tabBar/API/index"
         :param is_click: 点击触发帮用户触发一下onTabItemTap
         :return:Page 对象
         """
-        page = self._change_route_async("switchTab", url, is_wait_url_change)
+        page = self._change_route_async(
+            "switchTab", url, is_wait_url_change, wait_route_done_time
+        )
         if is_click and page.path in self.tabbar_pages:  # is tabbar and is click
             # 需要触发 onTabItemTap
             try:
-                page.call_method("onTabItemTap", {
-                    "index": self.tabbar_pages[page.path]["index"],
-                    "pagePath": self.tabbar_pages[page.path]["pagePath"],
-                    "text": self.tabbar_pages[page.path]["text"]
-                })
+                page.call_method(
+                    "onTabItemTap",
+                    {
+                        "index": self.tabbar_pages[page.path]["index"],
+                        "pagePath": self.tabbar_pages[page.path]["pagePath"],
+                        "text": self.tabbar_pages[page.path]["text"],
+                    },
+                )
             except MiniAppError:
                 pass
         if page != url.split("?")[0]:
             self.logger.warning("Switch tab(%s) but(%s)" % (url, page.path))
         return page
 
     def stop_audits(self, path: str = None):
@@ -465,25 +657,33 @@
     def go_home(self, main_page_path=None):
         """
         跳转到首页
         :param main_page_path: 路径
         :return: Page 对象
         """
         if not main_page_path:
-            if self.main_page_path:
-                main_page_path = self.main_page_path
+            main_page_path = self.main_page_path
+        elif not isinstance(main_page_path, Page):
+            main_page_path = Page(None, main_page_path, None, None)
+
+        if main_page_path.path in self.tabbar_pages:
+            if (
+                self.current_page.path == main_page_path.path
+            ):  # switch will not route done
+                is_wait_url_change = False
             else:
-                main_page_path = (
-                    "/" + self._get_launch_options_sync().result.result.path
-                )
-                if main_page_path == "/":
-                    raise MiniLaunchError("get launch options failed")
-                self.main_page_path = main_page_path
-
-        page = self.relaunch(main_page_path)
+                is_wait_url_change = True
+            # switch_tab有可能没有route done回调, 最多等5s
+            page = self.switch_tab(
+                main_page_path.path,
+                is_wait_url_change=is_wait_url_change,
+                wait_route_done_time=5,
+            )
+        else:
+            page = self.relaunch(main_page_path.path, main_page_path.query)
         return page
 
     def get_async_response(self, msg_id: str, timeout=None) -> None or dict:
         """
         description: 获取异步调用的结果
         param {*} self
         param {str} msg_id 消息ID
@@ -502,23 +702,24 @@
         self._wait(get, timeout)
         return ret
 
     def wait_for_page(self, page_path=None, max_timeout=10):
         if not self._current_page or self._current_page != page_path:
             # 没有记录到当前页面/当前页面不是目标页面, 等待页面跳转成功的回调
             self._route_changed(max_timeout)
-            ret = (self.current_page == page_path)
+            ret = self.current_page == page_path
             # issue#144 如果等不到预期的页面, 考虑是否因为页面栈满了(自动化流程中, 用户可以直接调用navigate to, 很有可能会满的)
             if not ret:
                 if len(self._page_stack()) == 10:
                     self.logger.warning(
-"""
+                        """
 wait for page fail, probably because the page stack is exceeded 10
 more infomation see: https://developers.weixin.qq.com/miniprogram/dev/api/route/wx.navigateTo.html#功能描述
-""")
+"""
+                    )
             return ret
         return True
 
     def wait_util(self, cnt, max_timeout=10):
         """
         {max_timeout}秒内, 剩余没有完成的请求数 <= {cnt}个
         符合上述条件则返回 True, 否则 False
@@ -536,55 +737,57 @@
         """
         self.call_wx_method(open_type, [{"url": path}])
         if is_wait_url_change and self._route_changed():
             return self.route_return_page
         else:
             return self.current_page  # todo: 状态有BUG, 超时也认为可用的
 
-    def _change_route_async(self, open_type, path, is_wait_url_change=True):
+    def _change_route_async(
+        self, open_type, path, is_wait_url_change=True, wait_route_done_time=15
+    ):
         """
         跳转页面
         call wx method -> call result / on app route done -> on app route done / call result
         "call result" and "on app route done" should wait together
         """
         wait_timeout = self.connection.timeout
-        wait_route_changed = event_loop.run_coroutine(
-            self._wait_route_changed_async(wait_timeout + 5)
-        )
-        cb = AsyncCallback(event_loop)
-        req_id = self.call_wx_method_async(open_type, [{"url": path}])
-        ee.once(req_id, cb.callback)
-        # 理论上通过ee监听了不会再在这里获取到结果, 以防线程切换过程导致时序问题，这里做一个兜底
-        response = self.connection.get_aysnc_msg_return(req_id)
-        if response is None:
-            cb.get_result(wait_timeout)
-        else:
-            # ee.remove_listener(req_id, cb.callback)
-            cb.cancel()
-        if is_wait_url_change:
-            if get_result(wait_route_changed, 5):  # 接口调用成功后5s内应有on app route done
-                return self.route_return_page
+        with RouteCommand(
+            open_type,
+            path,
+            route_done_lock=self._async_msg_lock if is_wait_url_change else None,
+        ) as cmd:
+            cmd.listen_route_change(wait_timeout)
+
+            cmd.open_id = self.call_wx_method_async(open_type, [{"url": path}])
+            # 理论上RouteCommand中通过ee监听了不会再在这里获取到结果, 以防线程切换过程导致时序问题，这里做一个兜底
+            response = self.connection.get_aysnc_msg_return(cmd.open_id)
+            if response is None:
+                cmd.get_open_result(wait_timeout)
             else:
-                wait_route_changed.cancel()
-        return self.current_page  # todo: 状态有BUG, 超时也认为可用的
+                cmd.cancel_open_callback()
+
+            if cmd.get_route_result(wait_route_done_time):
+                return self.current_page
+            else:
+                return self.get_current_page()  # 没有等到route done, 直接获取当前页面
 
     def _on_route_changed(self, message):
         if not message.name == "onAppRouteDone":
             return
         args = message.args
         options = args[0]
         update_time = args[1] if len(args) > 1 else int(time.time() * 1000)
         if (
             self.route_return_page_update_time
             and self.route_return_page_update_time > update_time
         ):
             # 旧信息, 丢弃
             return
         self.route_return_page = Page(
-            options.webviewId, options.path, options.query, self.connection
+            options.webviewId, options.path, options.query, self
         )
         # 记录当前页面
         self._current_page = self.route_return_page
         self._notify_msg_lock()
         self.logger.info("Route changed, %s" % message)
 
     def _route_changed(self, timeout=None):
@@ -616,24 +819,14 @@
     async def _wait_route_changed_async(self, timeout=None):
         if not timeout:
             timeout = 5
 
         ret = await self._wait_msg_lock(timeout)
         return ret
 
-    # def _inject_global(self):
-    #     self._evaluate("""function() {
-    #         if (typeof global === "undefined") {
-    #             global = (function() {
-    #                 return this;
-    #             })();
-    #             if (typeof window === "object") global = window;
-    #         }
-    #     }""")
-
     def _route_change_listener(self):
         self._unregister("onAppRouteDone")
         self._expose_function("onAppRouteDone", self._on_route_changed)
         self._evaluate(
             """function () {
     if (!global.__minium_onAppRouteDone) {
         wx.onAppRouteDone(function (options) {
@@ -651,25 +844,217 @@
     def _get_account_info_sync(self):
         return self._call_wx_method("getAccountInfoSync")
 
     def _page_stack(self):
         ret = self.connection.send("App.getPageStack")
         page_stack = []
         for page in ret.result.pageStack:
-            page_stack.append(Page(page.pageId, page.path, page.query, self.connection))
+            page_stack.append(Page(page.pageId, page.path, page.query, self))
         return page_stack
 
+    # ws断连可重试
+    @retry(2, (MiniConnectionClosedError))
     def _stop_audits(self):
         ret = self.connection.send("Tool.stopAudits")
         return ret
 
+    def hook_wx_method(
+        self,
+        method: str,
+        before: Callback or types.FunctionType = None,
+        after: Callback or types.FunctionType = None,
+        callback: Callback or types.FunctionType = None,
+    ):
+        """
+        hook wx 方法
+        :param method: 需要 hook 的方法
+        :param before: 在需要 hook 的方法之前调用
+        :param after: 在需要 hook 的方法之后调用
+        :param callback: 在需要 hook 的方法回调之后调用
+        :return:
+        """
+        stages: typing.List[types.FunctionType] = []  # 完成的步骤
+        if isinstance(before, Callback):
+            before = before.callback
+        if isinstance(after, Callback):
+            after = after.callback
+        if isinstance(callback, Callback):
+            callback = callback.callback
+
+        if before and not callable(before):
+            self.logger.error(f"wx.{method} hook before method is non-callable")
+            return
+
+        if after and not callable(after):
+            self.logger.error(f"{method} hook after method is non-callable")
+            return
+
+        if callback and not callable(callback):
+            self.logger.error(f"{method} hook callback method is non-callable")
+            return
+        try:
+
+            def super_before(msg):
+                self.logger.debug(f"{method} before hook result: {msg['args']}")
+                if before:
+                    before(msg["args"])
+
+            if before:
+                stages.append(super_before)
+                self._expose_function(
+                    method + "_" + super_before.__name__, super_before
+                )
+
+            def super_after(msg):
+                self.logger.debug(f"wx.{method} after hook result: {msg['args']}")
+                if after:
+                    after(msg["args"])
+
+            if after:
+                stages.append(super_after)
+                self._expose_function(method + "_" + super_after.__name__, super_after)
+
+            def super_callback(msg):
+                self.logger.debug(f"wx.{method} callback hook result: {msg['args']}")
+                if callback:
+                    callback(msg["args"])
+
+            if callback and not method.endswith("Sync"):  # Sync方法没有callback，通过after回调
+                stages.append(super_callback)
+                self._expose_function(
+                    method + "_" + super_callback.__name__, super_callback
+                )
+            return self._evaluate_js(
+                "hookWxMethod",
+                code_format_info=dict(
+                    method=method,
+                    origin=method + "_MiniumOrigin",
+                    before=method + "_" + super_before.__name__,
+                    after=method + "_" + super_after.__name__,
+                    callback=method + "_" + super_callback.__name__,
+                ),
+            )
+        except MiniError:
+            for stage in stages:
+                self.remove_observer(method + "_" + stage.__name__, stage)
+            stages = []
+            raise
+
+    def release_hook_wx_method(self, method):
+        """
+        释放 hook wx 方法
+        :param method: 需要释放 hook 的方法
+        :return:
+        """
+        self._evaluate_js(
+            "releaseHookWxMethod",
+            code_format_info=dict(
+                origin=method + "_MiniumOrigin",
+                method=method,
+                before=method + "_super_before",
+                after=method + "_super_after",
+                callback=method + "_super_callback",
+            ),
+        )
+        # 移除监听函数
+        self.connection.remove(method + "_super_before")
+        self.connection.remove(method + "_super_after")
+        self.connection.remove(method + "_super_callback")
+
+    def hook_current_page_method(self, method, callback):
+        """
+        hook 当前页面的方法
+        :param method:  方法名
+        :param callback:    回调函数
+        """
+
+        if isinstance(callback, Callback):
+            callback = callback.callback
+
+        def super_callback(msg):
+            self.logger.debug(f"Page.{method} call hook result: {msg['args']}")
+            if callback:
+                callback(msg["args"])
+
+        if callback and not callable(callback):
+            self.logger.error(f"Page.{method} hook callback method is non-callable")
+            return
+        try:
+            if callback:
+                self._expose_function(
+                    "page_hook_" + method + "_" + super_callback.__name__,
+                    super_callback,
+                )
+            self._evaluate_js(
+                "hookCurrentPageMethod",
+                code_format_info={
+                    "method": method,
+                    "callback": "page_hook_" + method + "_" + super_callback.__name__,
+                },
+            )
+        except MiniError:
+            if callback:
+                self.remove_observer(
+                    "page_hook_" + method + "_" + super_callback.__name__,
+                    super_callback,
+                )
+            raise
+
+    def release_hook_current_page_method(self, method):
+        # 移除监听函数
+        self.connection.remove("page_hook_" + method + "_super_callback")
+
     ###
     # 各类 mock
     ###
 
+    def mock_wx_method(
+        self,
+        method,
+        functionDeclaration: str = None,
+        result=None,
+        args=None,
+        success=True,
+        plugin_appid="auto",
+    ):
+        """
+        mock wx method and return result
+        :param self:
+        :param method:
+        :param functionDeclaration:
+        :param result:
+        :param args:
+        :param success:
+        :return:
+        """
+        if plugin_appid == "auto":
+            plugin_appid = (self._current_page or self.get_current_page()).plugin_appid
+        self._mock_wx_method(
+            method=method,
+            functionDeclaration=functionDeclaration,
+            result=result,
+            args=args,
+            success=success,
+            plugin_appid=plugin_appid,
+        )
+
+    def restore_wx_method(self, method, plugin_appid="auto"):
+        """
+        恢复被 mock 的方法
+        :param method: mock的方法
+        :param plugin_appid: 插件appid
+        :return:
+        """
+        params = {"method": method}
+        if plugin_appid == "auto":
+            plugin_appid = (self._current_page or self.get_current_page()).plugin_appid
+        if plugin_appid:
+            params["pluginId"] = plugin_appid
+        self.connection.send("App.mockWxMethod", params)
+
     def _mock_network(
         self,
         interface: str,
         rule: str or dict,
         success=None,
         fail=None,
         mock_type=MockNetworkType.ALWAYS,
@@ -692,15 +1077,17 @@
         if mock_type == MockNetworkType.ONCE:
             # 保护字段, 保证不冲突
             _rule["_miniMockType"] = MockNetworkType.ONCE.value
         has_mock = self._evaluate_js(
             "addNetworkMockRule", [_rule], code_format_info={"interface": interface}
         )
         if not has_mock:
-            self._evaluate_js("mockNetwork", code_format_info={"interface": interface})
+            retry(self.__class__.__RETRY_CNT__, self.__class__.__RETRY_EXCEPTION__)(
+                self._evaluate_js
+            )("mockNetwork", code_format_info={"interface": interface})
 
     def _restore_network(self, interface: str):
         """
         恢复被mock的网络接口
         """
         return self._evaluate_js(
             "cleanNetworkMockRule", code_format_info={"interface": interface}
@@ -730,15 +1117,17 @@
                 fail = {"errMsg": "%s:fail %s" % (interface, fail)}
             _rule["fail"] = fail
         if mock_type == MockCloudCallType.ONCE:
             # 保护字段, 保证不冲突
             _rule["_miniMockType"] = MockCloudCallType.ONCE.value
         has_mock = self._evaluate_js("addCloudCallMockRule", [_rule, interface])
         if not has_mock:
-            self._evaluate_js("mockCloudCall")
+            retry(self.__class__.__RETRY_CNT__, self.__class__.__RETRY_EXCEPTION__)(
+                self._evaluate_js
+            )("mockCloudCall")
 
     def _restore_cloud_call(self, interface: str):
         """
         恢复被mock的云调用接口
         """
         return self._evaluate_js(
             "cleanCloudCallMockRule",
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/callback.py` & `minium-1.4.0/minium/miniprogram/base_driver/callback.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,30 +15,47 @@
         self.__callback = callback
         self.__called = threading.Semaphore(0)
         self.__is_called = False
         self.__callback_result = None
 
     def callback(self, args):
         self.__is_called = True
-        self.__callback_result = args[0] if args and len(args) == 1 else args
+        self.__callback_result = (
+            args[0] if isinstance(args, (tuple, list)) and len(args) == 1 else args
+        )
         self.__called.release()
         if self.__callback:
             self.__callback(*args)
 
     @property
     def is_called(self):
+        """callback曾被调用过
+
+        :return bool: True: called, False: never called
+        """
         return self.__is_called
 
+    @property
+    def result(self):
+        return self.__callback_result
+
+    def acquire(self, timeout=10):
+        """acquire next callback
+
+        :param int timeout: wait seconds, defaults to 10
+        """
+        return self.__called.acquire(timeout=timeout)
+
     def wait_called(self, timeout=10) -> bool:
         """
         等待回调调用, 默认等待最多10s
         """
         if self.__is_called:
             return True
-        return self.__called.acquire(timeout=timeout)
+        return self.acquire(timeout=timeout)
 
     def get_callback_result(self, timeout=0) -> any:
         """
         获取回调结果, 超时未获取到结果报AssertionError
         1. 回调参数只有一个的情况会解构
         2. 回调参数中有多个的情况会直接返回参数list
         """
@@ -81,15 +98,17 @@
         等待回调调用, 默认等待最多10s
         """
         if timeout == 0:
             return self._waiter.done()
         if self._waiter.done():
             return True
         try:
-            return self._loop.run_coroutine(async_wait(self._waiter, timeout, self._loop)).result()
+            return self._loop.run_coroutine(
+                async_wait(self._waiter, timeout, self._loop)
+            ).result()
         except WaitTimeoutError:
             return False
         except:
             return self._waiter.done()
 
     def get_callback_result(self, timeout=0) -> any:
         if self.wait_called(timeout):
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/element.py` & `minium-1.4.0/minium/miniprogram/base_driver/element.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 """
 @Author: lockerzhang
 @LastEditors: lockerzhang
 @Description: 元素相关的操作和信息获取
 @Date: 2019-03-11 14:42:10
 @LastEditTime: 2019-06-06 15:13:32
 """
+from __future__ import annotations
 import code
 from logging import Logger
 import typing
-from minium.framework.exception import MiniElementNotFoundError
-from .minium_object import MiniumObject
+from minium.framework.exception import MiniElementNotFoundError, MiniTimeoutCauseByConnectionBreakError
+from .minium_object import MiniumObject, RetryableApi
 from ...utils.utils import timeout
 from ...utils.emitter import ee
 import time
 from .prefixer import *
+from .connection import Command
 
 
 class Element:
     tagName: str
     elementId: str
     nodeId: typing.Optional[str]
 
@@ -37,26 +39,40 @@
         return self[name]
 
     def __getitem__(self, name):
         name = Rect.key_map.get(name, name)
         return super(Rect, self).__getitem__(name)
 
 
-class BaseElementType(MiniumObject):
-    def get_elements(*arg, **kwargs) -> typing.List[any]:
-        ...
-
-    def get_element(*arg, **kwargs) -> any:
-        ...
-
-
-class BaseElement(BaseElementType):
+class BaseElement(MiniumObject, metaclass=RetryableApi):
     """
     元素基类
     """
+    __RETRY_EXCEPTION__ = (MiniTimeoutCauseByConnectionBreakError,)  # 小程序掉线Element实例可能就没用了
+    __RETRY_API__ = [
+        "data",
+        # "size",
+        "offset",
+        # "rect",
+        # "page_scroll_x",
+        # "page_scroll_y",
+        # "page_offset",
+        # "value",
+        # "inner_text",
+        "inner_wxml",
+        "outer_text",
+        "styles",
+        "attribute",
+        "scroll_to",
+        # private
+        "_property",  # 属性相关
+        "_dom_property",  # dom属性相关
+        "_get_window_properties",  # window属性相关
+        "__get_elements",  # get element相关都经过该接口
+    ]
 
     def __init__(self, element: Element, page_id: str, connection):
         """
         初始化
         """
         super().__init__()
         self.element_id = element.elementId
@@ -167,14 +183,16 @@
     def inner_text(self):
         """
         get element text
         :return:
         """
         return self._dom_property("innerText")[0]
 
+    text = inner_text
+
     @property
     def inner_wxml(self):
         """
         get wxml for element
         :return:
         """
         return self._send("Element.getWXML", {"type": "inner"}).result.wxml
@@ -210,23 +228,23 @@
         """
         if not args:
             args = []
         return self._send(
             "Element.callFunction", {"functionName": func, "args": args}
         ).result
 
-    def tap(self):
+    def tap(self, *args, **kwargs):
         """
         点击
         :return: NULL
         """
         self._send("Element.tap")
         ee.emit("notify")
 
-    def click(self):
+    def click(self, *args, **kwargs):
         """
         点击, 同 tap
         :return: NULL
         """
         styles = self.styles("pointer-events")
         if styles and styles[0] == "none":
             self.logger.warning("can't click, because pointer-events is none")
@@ -348,15 +366,15 @@
         self,
         selector,
         max_timeout=0,
         inner_text=None,
         text_contains=None,
         value=None,
         index=-1,
-    ) -> typing.List[BaseElementType]:  # type: ignore # noqa: F811
+    ) -> typing.List[ElementType]:  # type: ignore # noqa: F811
         """
         find elements in current page
         目前支持的选择器有：
 
         选择器	              样例	                      样例描述
         .class	             .intro	                    选择所有拥有 class="intro" 的组件
         #id	                 #firstname	                选择拥有 id="firstname" 的组件
@@ -401,16 +419,16 @@
         for el in ret.result.elements:
             elements.append(create(el, self.page_id, self.connection))
             if len(elements) == (index + 1):  # index==-1时，不会match，就会全部返回
                 return elements
         return elements
 
     def __search_child(
-        self, selector_list: list, parent: BaseElementType = None, index=-1  # type: ignore # noqa: F811
-    ) -> typing.List[BaseElementType]:
+        self, selector_list: list, parent: ElementType = None, index=-1  # type: ignore # noqa: F811
+    ) -> typing.List[ElementType]:
         # index == -1: get所有, index >=0: get index+1个
         if len(selector_list) == 0:
             return []
         _selector = selector_list.pop()
         should_be_custom_element = bool(
             len(selector_list)
         )  # 出了最后一层selector，都需要是自定义组件，不然不能往下走
@@ -438,15 +456,15 @@
                 selector_list[0:], _el
             )  # selector_list[0:]相当于copy
             child_els += child_el
             if len(child_els) == (index + 1):
                 return child_els
         return child_els
 
-    def _get_elements_by_css(self, selector: str, max_timeout=0, index=-1) -> list:
+    def _get_elements_by_css(self, selector: str, max_timeout=0, index=-1) -> typing.List[ElementType]:
         """
         1. 现存自定义组件中的class会自动加前缀，但不包括slot占位的元素
         2. slot元素的class命名规则
         2.1 <page><test><view class="这个class不会加前缀"></view></test></page>
         2.2 <custom><test><view class="这个class会加上custom组件对应的前缀"></view></test></custom>
         3. 自定义组件中通过id获取元素失败
         """
@@ -477,14 +495,32 @@
         just a trigger
         :param trigger_type:
         :param detail:
         :return:
         """
         return self._trigger(trigger_type, detail)
 
+    def trigger_events(self, events):
+        """触发DOM事件序列, 录制回放用
+        touch事件可以只提供type, interval参数
+
+        :param [{type, interval?, touches?, changedTouches?, detail?}...] events: 事件列表
+        """
+        for event in events:
+            interval = event.get("interval", 0)
+            if event["type"] == "touchstart":
+                self._touch_start(event["touches"], event["changedTouches"])
+            elif event["type"] == "touchmove":
+                self._touch_move(event["touches"], event["changedTouches"])
+            elif event["type"] == "touchend":
+                self._touch_end(event["changedTouches"])
+            else:
+                self.trigger(event["type"], event["detail"])
+            time.sleep(interval)
+
     def dispatch_event(
         self,
         event_name,
         selector=None,
         touches=None,
         change_touches=None,
         detail=None,
@@ -551,21 +587,21 @@
         elif isinstance(names, str):
             result = self._send("Element." + method, {"names": [names]})
         else:
             raise Exception("invalid names type")
         ret = getattr(result.result, return_name)
         return ret
 
-    def _send(self, method, params=None):
+    def _send(self, method, params=None, extra_time=0):
         if params is None:
             params = {}
         params["elementId"] = self.element_id
         params["pageId"] = self.page_id
 
-        return self.connection.send(method, params)
+        return self.connection.send(method, params, max_timeout=Command.max_timeout+extra_time)
 
     def _move(self, x_offset, y_offset, move_delay=350, smooth=False):
         offset = self.offset
         size = self.size
         page_offset = self.page_offset
         changed_touch = touch = ori_changed_touch = ori_touch = {
             "identifier": 0,
@@ -650,79 +686,79 @@
     def _touch_end(self, changed_touches: list):
         touches = []
         self._send(
             "Element.touchend",
             params={"touches": touches, "changedTouches": changed_touches},
         )
 
-    def _get_elements(self, selector, max_timeout=0, index=-1):
-        @timeout(max_timeout)
-        def search_elements(_selector):
-            elements = []
-            ret = self._send("Element.getElements", {"selector": _selector})
-            if hasattr(ret, "error"):
-                raise Exception(
-                    "Error when finding elements[%s], %s" % (_selector, ret.error)
-                )
-            for el in ret.result.elements:
-                elements.append(create(el, self.page_id, self.connection))
-            return elements
-
-        def search_child(
-            selector_list: list, parent: BaseElement = None
-        ):  # index == -1: get所有, index >=0: get index+1个
-            if len(selector_list) == 0:
-                return
-            _selector = selector_list.pop()
-            should_be_custom_element = bool(
-                len(selector_list)
-            )  # 出了最后一层selector，都需要是自定义组件，不然不能往下走
-            if parent:
-                els = parent.get_elements(_selector)
-            else:
-                els = search_elements(_selector)
-            if len(els) == 0:
-                return []
-            real_els = []
-            for _el in els:
-                if should_be_custom_element and isinstance(_el, CustomElement):
-                    real_els.append(_el)
-                elif not should_be_custom_element:
-                    real_els.append(_el)
-                else:
-                    self.logger.warn("%s should be a custom element" % _selector)
-            if not real_els or len(selector_list) == 0:  # 找不到 或 没有子选择器了
-                return real_els
-            child_els = []
-            for _el in real_els:
-                child_el = search_child(selector_list[0:], _el)
-                child_els += child_el
-                if index == -1:
-                    continue
-                elif len(child_els) > index:
-                    return child_els
-            return child_els
-
-        try:
-            self.logger.info("try to find elements: %s" % selector)
-            _selector_list = selector.split(">>>")
-            if len(_selector_list) > 1:  # 新增处理【>>>】穿透自定义组件逻辑
-                _selector_list.reverse()
-                els = search_child(_selector_list)
-            else:
-                els = search_elements(selector)
-            if len(els) == 0:
-                self.logger.warning(
-                    f"Could not found any element '{selector}' you need"
-                )
-            else:
-                self.logger.info("find elements success: %s" % str(els))
-            return els
-        except Exception as e:
-            raise Exception("elements search fail cause: " + str(e))
+    # def _get_elements(self, selector, max_timeout=0, index=-1):
+    #     @timeout(max_timeout)
+    #     def search_elements(_selector):
+    #         elements = []
+    #         ret = self._send("Element.getElements", {"selector": _selector})
+    #         if hasattr(ret, "error"):
+    #             raise Exception(
+    #                 "Error when finding elements[%s], %s" % (_selector, ret.error)
+    #             )
+    #         for el in ret.result.elements:
+    #             elements.append(create(el, self.page_id, self.connection))
+    #         return elements
+
+    #     def search_child(
+    #         selector_list: list, parent: BaseElement = None
+    #     ):  # index == -1: get所有, index >=0: get index+1个
+    #         if len(selector_list) == 0:
+    #             return
+    #         _selector = selector_list.pop()
+    #         should_be_custom_element = bool(
+    #             len(selector_list)
+    #         )  # 出了最后一层selector，都需要是自定义组件，不然不能往下走
+    #         if parent:
+    #             els = parent.get_elements(_selector)
+    #         else:
+    #             els = search_elements(_selector)
+    #         if len(els) == 0:
+    #             return []
+    #         real_els = []
+    #         for _el in els:
+    #             if should_be_custom_element and isinstance(_el, CustomElement):
+    #                 real_els.append(_el)
+    #             elif not should_be_custom_element:
+    #                 real_els.append(_el)
+    #             else:
+    #                 self.logger.warn("%s should be a custom element" % _selector)
+    #         if not real_els or len(selector_list) == 0:  # 找不到 或 没有子选择器了
+    #             return real_els
+    #         child_els = []
+    #         for _el in real_els:
+    #             child_el = search_child(selector_list[0:], _el)
+    #             child_els += child_el
+    #             if index == -1:
+    #                 continue
+    #             elif len(child_els) > index:
+    #                 return child_els
+    #         return child_els
+
+    #     try:
+    #         self.logger.info("try to find elements: %s" % selector)
+    #         _selector_list = selector.split(">>>")
+    #         if len(_selector_list) > 1:  # 新增处理【>>>】穿透自定义组件逻辑
+    #             _selector_list.reverse()
+    #             els = search_child(_selector_list)
+    #         else:
+    #             els = search_elements(selector)
+    #         if len(els) == 0:
+    #             self.logger.warning(
+    #                 f"Could not found any element '{selector}' you need"
+    #             )
+    #         else:
+    #             self.logger.info("find elements success: %s" % str(els))
+    #         return els
+    #     except Exception as e:
+    #         raise Exception("elements search fail cause: " + str(e))
 
 
 class FormElement(BaseElement):
     """
     表单类型元素
     """
 
@@ -772,17 +808,27 @@
         if self._tag_name != "picker":
             self.logger.warning(
                 "Element's type is not fit for the method which you call"
             )
             return
         self.trigger("change", {"value": value})
         return
+    
+    def tap(self, force=False, **kwargs):
+        """input/picker点击事件会触发拉起键盘/选择器
 
-    def click(self):
-        if self._tag_name == "picker":
+        :param bool force: 组件绑定了bindtap事件, 一定需要触发tap操作, defaults to False
+        :return None: 
+        """
+        if self._tag_name in ("picker", "input") and not force:
+            return
+        return super().tap(**kwargs)
+
+    def click(self, force=False):
+        if self._tag_name in ("picker", "input") and not force:
             return
         return super(FormElement, self).click()
 
     #####################
     #       switch      #
     #####################
     def switch(self):
@@ -1483,26 +1529,27 @@
     "input": FormElement,
     "textarea": FormElement,
     "switch": FormElement,
     "slider": FormElement,
     "picker": FormElement,
 }
 
-Elements = typing.TypeVar(
-    "Elements",
+
+ElementType = typing.Union[
     BaseElement,
+    CustomElement,
     VideoElement,
     AudioElement,
     ViewElement,
     FormElement,
     LivePlayerElement,
     LivePusherElement,
-)
+]
 
 
-def create(element: Element, page_id: str, connection) -> Elements:
+def create(element: Element, page_id: str, connection) -> ElementType:
     if "nodeId" in element.keys():
         return CustomElement(element, page_id, connection)
     else:
         return ELEMENT_TYPE.get(element.tagName, BaseElement)(
             element, page_id, connection
         )
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/minium_log.py` & `minium-1.4.0/minium/miniprogram/base_driver/minium_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,32 +13,23 @@
 import types
 import json
 import requests
 import queue
 import threading
 import logging
 import os
+from .version import build_version
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 # logger = logging.getLogger("DataReport")
 
 REPORT_DOMAIN = "minitest.weixin.qq.com"
 REPORT_PATH = "xbeacon/user_report"
 
 
-def build_version():
-    config_path = os.path.join(os.path.dirname(__file__), "version.json")
-    if not os.path.exists(config_path):
-        return {}
-    else:
-        with open(config_path, "r", encoding="utf8") as f:
-            version = json.load(f)
-            return version
-
-
 def process_report():
     global existFlag
     while not existFlag:
         lock.acquire()
         lock.wait(10)
         lock.release()
         if not report_queue.empty():
@@ -192,22 +183,7 @@
                 and not k.startswith("notify")
                 and not k.startswith("remove")
             ):
                 attr_dict[k] = minium_log(v)
         return type.__new__(mcs, cls_name, bases, attr_dict)
 
 
-def singleton(cls):
-    """
-    单例装饰器
-    :param cls:
-    :return:
-    """
-    _instance = {}
-
-    @wraps(cls)
-    def inner(*args, **kwargs):
-        if cls not in _instance:
-            _instance[cls] = cls(*args, **kwargs)
-        return _instance[cls]
-
-    return inner
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/minium_object.py` & `minium-1.4.0/minium/native/lib/at/core/uidevice.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,405 +1,301 @@
-#!/usr/local/bin/python3
 # -*- coding: utf-8 -*-
 """
-Author:         lockerzhang
-Filename:       minium_object.py
-Create time:    2019/4/30 21:21
-Description:
-
+@author: 'xiazeng'
+@created: 2017/1/17 
 """
-
-from .minium_log import MonitorMetaClass
-from .callback import Callback
-from .connection import Command, Connection
-from ...utils.injectjs import getInjectJsCode
-import subprocess
-import time
+import base64
+import json
 import logging
-import types
+import time
+
+from at.core import element, javadriver, uixml, case_repair_adapter
+import at.utils.commonhelper as commonhelper
+
+logger = logging.getLogger()
+
 
-logger = logging.getLogger("minium")
+class PyUiDevice(object):
+    def __init__(self, jd):
+        self.jd = jd  # type: javadriver.JavaDriver
+        self.adb = jd.adb
+        self.input_interceptor = None
+        self._width = None
+        self._height = None
 
+    def set_input_interceptor(self, input_interceptor):
+        self.input_interceptor = input_interceptor
 
-class MiniumObject(object, metaclass=MonitorMetaClass):
-    _cant_use_interface = {}
+    def enter(self, text):
+        self.record(u"直接输入: %s", text)
+        self.request_method("setText", [text])
 
-    def __init__(self):
-        self.logger = logger
-        self.observers = {}
-        self.connection: Connection = None
+    def enter_zh(self, zh_text):
+        self.record(u"直接输入中文: %s", zh_text)
+        self.request_method("setChineseText", [zh_text])
 
-    def _do_shell(self, command, print_msg=True, input=b""):
+    def get_ui_view(self, selector, instance=0, views=None):
         """
-        执行 shell 语句
-        :param command:
-        :param print_msg:
-        :return:
+        :rtype: uixml.UiView
         """
-        self.logger.info("de shell: %s" % command)
-        p = subprocess.Popen(
-            command,
-            shell=True,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            stdin=subprocess.PIPE,
-        )
-        out, err = p.communicate(input)
-        try:
-            out = out.decode("utf8")
-        except UnicodeDecodeError:
-            out = out.decode("gbk")
-        try:
-            err = err.decode("utf8")
-        except UnicodeDecodeError:
-            err = err.decode("gbk")
-        if print_msg:
-            self.logger.info("err:\n%s" % err)
-            self.logger.info("out:\n%s" % out)
-        return out, err
-
-    @classmethod
-    def _can_i_use(cls, name):
-        return not cls._cant_use_interface.get(name, False)
-
-    @classmethod
-    def _unset_interface(cls, name):
-        cls._cant_use_interface[name] = True
-
-    def call_wx_method(self, method, args=None, plugin_appid="auto"):
-        """
-        调用 wx 的方法
-        :param method:
-        :param args:
-        :param plugin_appid: 调用插件[${appid}]中的方法
-        :return:
+        if views is None:
+            views = self.jd.get_ui_views()
+            if isinstance(selector, element.Element):
+                for view in views:
+                    if selector.match_ui_view(view):
+                        return view
+            else:
+                logger.error("unknown type: %s, %s", type(selector), selector)
+
+        return uixml.get_view(views, selector, instance)
+
+    def click_on_ui_view(self, ui_view):
         """
-        if plugin_appid == "auto":
-            plugin_appid = None
-        return self._call_wx_method(method=method, args=args, plugin_appid=plugin_appid)
-
-    def mock_wx_method(
-        self,
-        method,
-        functionDeclaration: str = None,
-        result=None,
-        args=None,
-        success=True,
-        plugin_appid="auto",
-    ):
-        """
-        mock wx method and return result
-        :param self:
-        :param method:
-        :param functionDeclaration:
-        :param result:
-        :param args:
-        :param success:
-        :return:
+        :type ui_view: uixml.UiView
+        :return: 
         """
-        if plugin_appid == "auto":
-            plugin_appid = None
-        self._mock_wx_method(
-            method=method,
-            functionDeclaration=functionDeclaration,
-            result=result,
-            args=args,
-            success=success,
-            plugin_appid=plugin_appid,
-        )
-
-    def restore_wx_method(self, method, plugin_appid="auto"):
-        """
-        恢复被 mock 的方法
-        :param method: mock的方法
-        :param plugin_appid: 插件appid
-        :return:
+        self.click_on_point(ui_view.center_x, ui_view.center_y)
+
+    def gesture(self, points):
+        self.record(u"手势: %s", json.dumps(points))
+        params = []
+        for point in points:
+            params.append(int(point[0]))
+            params.append(int(point[1]))
+        self.jd.request_at_device("gesture", params)
+
+    @case_repair_adapter.deco_do_action
+    def click_on_point(self, x, y):
+        self.record(u"点击坐标: %s, %s", int(x), int(y))
+        if self.input_interceptor:
+            return self.input_interceptor.click(x, y)
+        else:
+            self.request_method("click", [int(x), int(y)])
+
+    def click_on_list(self, xy_list, max_sleep=0.5, min_sleep=0.5):
         """
-        params = {"method": method}
-        if plugin_appid == "auto":
-            plugin_appid = None
-        if plugin_appid:
-            params["pluginId"] = plugin_appid
-        self.connection.send("App.mockWxMethod", params)
-
-    def hook_wx_method(
-        self,
-        method: str,
-        before: Callback or types.FunctionType = None,
-        after: Callback or types.FunctionType = None,
-        callback: Callback or types.FunctionType = None,
-    ):
-        """
-        hook wx 方法
-        :param method: 需要 hook 的方法
-        :param before: 在需要 hook 的方法之前调用
-        :param after: 在需要 hook 的方法之后调用
-        :param callback: 在需要 hook 的方法回调之后调用
+        点击列表
+        :param xy_list:
+        :param interval: 两次点击直接最大停顿时间
+        :param min_sleep: 两次点击直接最小停顿时间
         :return:
         """
+        self.jd.push_op(u"点击列表点:%s", xy_list)
+        for x, y in xy_list:
+            t = time.time()
+            self.request_method("click", [int(x), int(y)])
+            sleep_time = max_sleep - (time.time() - t)
+            if sleep_time > min_sleep:
+                time.sleep(sleep_time)
+            else:
+                time.sleep(min_sleep)
+
+    def screen_point_data(self, x, y, width, height, quality):
+        self.record(u"局部截图: %s, %s, %s, %s", int(x), int(y), int(width), int(height))
+        base64_str = self.request_method("screenPoint", [int(x), int(y), int(width), int(height), int(quality)])
+        # logger.info("base64_str is %s"%base64_str)
+        base64_data = base64.b64decode(base64_str)
+        return base64_data
+
+    def screen_point(self, filename, x, y, width, height, quality=30):
+        d = self.screen_point_data(x, y, width, height, quality)
+        open(filename, "wb").write(d)
+
+    def click_on_center(self):
+        self.click_on_point(self.width()/2, self.height()/2)
+
+    def swipe(self, x1, y1, x2, y2, steps):
+        self.record(u"滑动: %s,%s -> %s, %s", x1, y1, x2, y2)
+        if self.input_interceptor:
+            self.input_interceptor.swipe(x1, y1, x2, y2, steps)
+        else:
+            self.fast_scroll(x1, y1, x2, y2, 100, steps)
+            # self.request_method("swipe", [int(x1), int(y1), int(x2), int(y2), steps])
 
-        if isinstance(before, Callback):
-            before = before.callback
-        if isinstance(after, Callback):
-            after = after.callback
-        if isinstance(callback, Callback):
-            callback = callback.callback
-
-        def super_before(msg):
-            self.logger.debug(f"{method} before hook result: {msg['args']}")
-            if before:
-                before(msg["args"])
-
-        if before and not callable(before):
-            self.logger.error(f"wx.{method} hook before method is non-callable")
-            return
-        if before:
-            self._expose_function(method + "_" + super_before.__name__, super_before)
-
-        def super_after(msg):
-            self.logger.debug(f"wx.{method} after hook result: {msg['args']}")
-            if after:
-                after(msg["args"])
-
-        if after and not callable(after):
-            self.logger.error(f"{method} hook after method is non-callable")
-            return
-        if after:
-            self._expose_function(method + "_" + super_after.__name__, super_after)
-
-        def super_callback(msg):
-            self.logger.debug(f"wx.{method} callback hook result: {msg['args']}")
-            if callback:
-                callback(msg["args"])
-
-        if callback and not callable(callback):
-            self.logger.error(f"{method} hook callback method is non-callable")
-            return
-        if callback and not method.endswith("Sync"):  # Sync方法没有callback，通过after回调
-            self._expose_function(
-                method + "_" + super_callback.__name__, super_callback
-            )
-
-        return self._evaluate_js(
-            "hookWxMethod",
-            code_format_info=dict(
-                method=method,
-                origin=method + "_MiniumOrigin",
-                before=method + "_" + super_before.__name__,
-                after=method + "_" + super_after.__name__,
-                callback=method + "_" + super_callback.__name__,
-            ),
-        )
+    def swipe_left(self, rect, steps=10):
+        y = rect.top + rect.height / 2
+        x2, x1 = rect.left + rect.width / 4, rect.left + rect.width * 3 / 4
+        self.swipe(x1, y, x2, y, steps)
+
+    def swipe_right(self, rect, steps=20):
+        y = rect.top + rect.height / 2
+        x1, x2 = rect.left + rect.width / 4, rect.left + rect.width * 3 / 4
+        self.swipe(x1, y, x2, y, steps)
+
+    def long_click_on_point(self, x, y, duration=3*1000):
+        self.record(u"长按: %s, %s, 时间:%sms", int(x), int(y), duration)
+        if self.input_interceptor:
+            self.input_interceptor.long_click(x, y, duration/1000.0)
+        else:
+            self.request_method("longClick", [int(x), int(y), duration])
+
+    def long_click_on_center(self, duration=3*1000):
+        self.long_click_on_point(self.width()/2, self.height()/2, duration)
 
-    def release_hook_wx_method(self, method):
+    def get_rotation(self):
         """
-        释放 hook wx 方法
-        :param method: 需要释放 hook 的方法
-        :return:
+        https://developer.android.com/reference/android/view/Surface.html#ROTATION_0
+        :return: 0-3
         """
-        self._evaluate_js(
-            "releaseHookWxMethod",
-            code_format_info=dict(
-                origin=method + "_MiniumOrigin",
-                method=method,
-                before=method + "_super_before",
-                after=method + "_super_after",
-                callback=method + "_super_callback",
-            ),
-        )
-        # 移除监听函数
-        self.connection.remove(method + "_super_before")
-        self.connection.remove(method + "_super_after")
-        self.connection.remove(method + "_super_callback")
-
-    def evaluate(self, app_function: str, args=None, sync=False, desc=None):
-        """
-        向 app Service 层注入代码并执行
-        :param app_function:
-        :param args:
-        :param sync:
-        :param desc: 报错描述
-        :return:
+        return self.request_method("getRotation")
+
+    def status_bar_height(self):
+        """获取状态栏的高度"""
+        return self.request_method("getStatusBarHeight")
+
+    def height(self):
         """
-        return self._evaluate(
-            app_function=app_function, args=args, sync=sync, desc=desc
-        )
-
-    # protect method
-
-    def hook_current_page_method(self, method, callback):
-        """
-        hook 当前页面的方法
-        :param method:  方法名
-        :param callback:    回调函数
-        """
-
-        def super_callback(msg):
-            self.logger.debug(f"Page.{method} call hook result: {msg['args']}")
-            if callback:
-                callback(msg["args"])
-
-        if callback and not callable(callback):
-            self.logger.error(f"Page.{method} hook callback method is non-callable")
-            return
-        if callback:
-            self._expose_function(
-                "page_hook_" + method + "_" + super_callback.__name__, super_callback
-            )
-        self._evaluate_js(
-            "hookCurrentPageMethod",
-            code_format_info={
-                "method": method,
-                "callback": "page_hook_" + method + "_" + super_callback.__name__,
-            },
-        )
-
-    def release_hook_current_page_method(self, method):
-        # 移除监听函数
-        self.connection.remove("page_hook_" + method + "_super_callback")
-
-    # private method
-
-    def _wait(self, func, timeout, interval=1):
-        """
-        等待直到`func`为true
-        :func: callable function
-        :timeout: timeout
-        :interval: query step
-        :return: bool
-        """
-        # func = lambda :True or False
-        if not callable(func):
-            return False
-        s = time.time()
-        timeout = timeout or interval
-        while time.time() - s < timeout:
-            if func():
-                return True
-            time.sleep(interval)
-        return False
-
-    def _call_wx_method(self, method, args=None, plugin_appid=None, sync=True):
-        if args is None:
-            args = []
-        if not isinstance(args, list):
-            if isinstance(args, str):
-                # 如果是字符型参数，就可以不用管是否是 sync 方法，直接转数组传参即可
-                args = [args]
-            elif "Sync" in method:
-                # 如果是 sync 方法，则需要从字典里面提取所有的 value 成为一个数组进行传参
-                if isinstance(args, dict):
-                    temp_args = list()
-                    for key in args.keys():
-                        temp_args.append(args[key])
-                    args = temp_args
-            else:
-                # 异步方法的话无需管 args 是str 还是 dict，直接转成 list 即可
-                args = [args]
+        获取全屏幕大小（包括status_bar的高度）
+        """
+        if not self._height:
+            self._height = self.request_method("getDisplayHeight")
+        return self._height
 
-        params = {"method": method, "args": args}
-        if plugin_appid:
-            params["pluginId"] = plugin_appid
-        if not sync:
-            return self.connection.send_async("App.callWxMethod", params)
-        return self.connection.send("App.callWxMethod", params)
-
-    def _evaluate(self, app_function: str, args=None, sync=False, desc=None):
-        if not args:
-            args = []
-        if sync:
-            return self.connection.send(
-                Command(
-                    "App.callFunction",
-                    {"functionDeclaration": app_function, "args": args},
-                    desc=desc,
-                )
-            )
-        else:
-            return self.connection.send_async(
-                "App.callFunction", {"functionDeclaration": app_function, "args": args}
-            )
-
-    def _evaluate_js(
-        self,
-        filename,
-        args=None,
-        sync=True,
-        default=None,
-        code_format_info=None,
-        mode=None,
-        **kwargs,
-    ):
-        """
-        运行 js 代码
-        :param filename: {JS_PATH} 中 JS 文件名字（不需要后缀）
-        :param code_format_info: JS 内容中需要进行格式化的信息, 如内容中包含 `%s` `%(arg)s` 等的可格式化信息
-        :param args: 注入函数需要输入的参数列表
-        :param sync: 同步执行函数
-        :param mode: js mode: 仅支持es5还是都支持
-        :param default: 同步结果返回默认值
-        """
-        if args is None:
-            args = []
-        ret = self._evaluate(
-            getInjectJsCode(filename, format_info=code_format_info, mode=mode),
-            args,
-            sync=sync,
-            **kwargs,
-        )
-        if sync:
-            return ret.get("result", {}).get("result", default)
+    def width(self):
+        if not self._width:
+            self._width = self.request_method("getDisplayWidth")
+        return self._width
+
+    def device_size(self):
+        return self.width(), self.height()
+
+    def wait_window_update(self, pkg, timeout=10*1000):
+        ret = self.request_method("waitForWindowUpdate", [pkg, timeout])
+        if ret:
+            time.sleep(2)
         return ret
 
-    def _get_async_response(self, msg_id: str):
-        return self.connection.get_aysnc_msg_return(msg_id)
+    def wait_for_idle(self, timeout=10*1000):
+        """
+        等待一段时间内ui没有变化
+        """
+        return self.request_method("waitForIdle", [timeout])
+
+    def current_package(self):
+        return self.request_method("getCurrentPackageName")
+
+    def drag(self, x1, y1, x2, y2, steps=10, first_sleep=200, last_sleep=200):
+        """
+        拖动
+        """
+        self.record(u"拖动: %s,%s -> %s, %s", x1, y1, x2, y2)
+        self.custom_drag(x1, y1, x2, y2, [first_sleep]+steps*[50]+[last_sleep])
+
+    def scroll(self, x1, y1, x2, y2, steps=20):
+        """
+        滑动
+        """
+        self.record(u"滑动: %s,%s -> %s, %s", x1, y1, x2, y2)
+        self.jd.request_action(self.jd.ACTION_AT_DEVICE, "fastDrag", [int(x1), int(y1), int(x2), int(y2), 500, steps])
+
+    def fast_scroll_one_forth_page(self, direction='up', num=1, milliseconds=100, steps=10):
+        """
+        滑动1/4个屏幕
+        """
+        width = self.width()
+        height = self.height() - self.status_bar_height()
+        for i in range(num):
+            if direction == "up":
+                self.fast_scroll(width / 2, height * 5 / 8, width / 2, height * 3 / 8, milliseconds, steps)
+            elif direction == "down":
+                self.fast_scroll(width / 2, height * 3 / 8, width / 2, height * 5 / 8, milliseconds, steps)
+            elif direction == "left":
+                self.fast_scroll(width*5/8, height/2, width*3/8, height/2, milliseconds, steps)
+            elif direction == "right":
+                self.fast_scroll(width*3/8, height/2, width*5/8, height/2, milliseconds, steps)
+            else:
+                raise TypeError("%s direction" % direction)
+            time.sleep(0.1)
+
+    def scroll_one_forth_page(self, direction, num=1):
+        """
+        滑动1/4个屏幕,direction是方向：up是从下往上, down是从上往下，left是从右到左，right是从左到右
+        """
+        width = self.width()
+        height = self.height() - self.status_bar_height()
+        self.jd.set_capture_op(False)
+        for i in range(num):
+            if direction == "up":
+                self.scroll(width/2, height*5/8, width/2, height*3/8)
+            elif direction == "down":
+                self.scroll(width / 2, height*3/8, width / 2, height*5/8)
+            elif direction == "left":
+                self.scroll(width*5/8, height/2, width*3/8, height/2)
+            elif direction == "right":
+                self.scroll(width*3/8, height/2, width*5/8, height/2)
+            else:
+                raise TypeError("%s direction" % direction)
+            time.sleep(0.2)
+        self.jd.set_capture_op(True)
+        self.record("滑动:%s", direction)
+
+    def fast_scroll_one_page(self, direction, num=1, milliseconds=100, steps=1):
+        """
+        快速滑动一整屏幕
+        """
+        width = self.width()
+        height = self.height() - self.status_bar_height()
+        for i in range(num):
+            if direction == "up":
+                self.fast_scroll(width/2, height*7/8, width/2, height*1/8, milliseconds, steps)
+            elif direction == "down":
+                self.fast_scroll(width / 2, height*1/8, width / 2, height*7/8, milliseconds, steps)
+            elif direction == "left":
+                self.fast_scroll(width*7/8, height/2, width*1/8, height/2, milliseconds, steps)
+            elif direction == "right":
+                self.fast_scroll(width*1/8, height/2, width*7/8, height/2, milliseconds, steps)
+            else:
+                raise TypeError("%s direction" % direction)
+            time.sleep(0.1)
+
+    def scroll_one_page(self, direction):
+        return self.scroll_one_forth_page(direction, 4)
 
-    def _expose_function(self, name, binding_function):
-        self.connection.register(name, binding_function)
-        self.connection.send("App.addBinding", {"name": name})
-
-    def _unregister(self, name, binding_function=None):
-        self.connection.remove(name, binding_function)
-
-    def _mock_wx_method(
-        self,
-        method,
-        functionDeclaration: str = "",
-        result=None,
-        args=None,
-        success=True,
-        plugin_appid=None,
-    ):
-        if not args:
-            args = []
-        elif not isinstance(args, tuple):
-            args = [args]
-        callback_type = "ok" if success else "fail"
-        params = {"method": method}
-        if plugin_appid:
-            params["pluginId"] = plugin_appid
-        if functionDeclaration:
-            params.update({"functionDeclaration": functionDeclaration, "args": args})
-        elif isinstance(result, str):
-            params["result"] = {
-                "result": result,
-                "errMsg": "%s:%s" % (method, callback_type),
-            }
-        elif isinstance(result, dict):
-            params["result"] = result
+    def fast_scroll(self, x1, y1, x2, y2, milliseconds=500, steps=10):
+        self.record(u"快速滑动: %s,%s -> %s, %s 时间:%s", x1, y1, x2, y2, milliseconds)
+        self.jd.request_action(self.jd.ACTION_AT_DEVICE, "fastDrag", [int(x1), int(y1), int(x2), int(y2), milliseconds, steps])
+
+    def custom_drag(self, x1, y1, x2, y2, sleep_times):
+        self.jd.request_action(self.jd.ACTION_AT_DEVICE, "customDrag", [int(x1), int(y1), int(x2), int(y2), json.dumps(sleep_times)])
+
+    def request_method(self, method, params=None):
+        return self.jd.request_at_device(method, params)
+
+    def wake_up(self):
+        """
+        等待一段时间内ui没有变化
+        """
+        return self.request_method("wakeUp")
+
+    # 处理rect相关的操作
+    def screen_rect(self, filename, rect, quality=30):
+        d = self.screen_point_data(rect.left, rect.top, rect.width, rect.height, quality)
+        open(filename, "wb").write(d)
+
+    def click(self, rect):
+        self.click_on_point(rect.center_x, rect.center_y)
+
+    def long_click(self, rect, microseconds=3*1000):
+        self.long_click_on_point(rect.center_x, rect.center_y, microseconds)
+
+    def screen_shot(self, filename, scale=1.0, quality=-1, max_idle=200, display_id=None):
+        if display_id is None:
+            try:
+                scale = scale if 0 < scale < 1.0 else 1
+                quality = quality if 0 < quality < 100 else 30
+                res = self.jd.request_at_device("screen", [float(scale), quality, max_idle])
+                if not res:
+                    logger.error("uiautomator screen failed: response empty. filename: %s. try reconnect" % filename)
+                    self.jd.reconnect()
+                    raise RuntimeError("uiautomator screen response empty")
+                commonhelper.base64_to_file(res, filename)
+                return filename
+            except Exception:
+                logger.exception("uiautomator screen failed")
+        self.adb.screen(filename, display_id)
+        return filename
+
+    def record(self, msg, *args):
+        if self.input_interceptor:
+            self.jd.push_op(msg, *args, display=self.input_interceptor.display_id)
         else:
-            self.logger.warning("mock wx method accept str or dict result only")
-            return
-        return self.connection.send("App.mockWxMethod", params)
-
-    def _mock_wx_js(
-        self, method, filename, args=None, code_format_info=None, plugin_appid=None
-    ):
-        """
-        mock方法中定义的替换函数直接返回一个promise, promise不需要reject, 自动化协议会根据回调的errmsg来判断回调success/fail
-        """
-        return self._mock_wx_method(
-            method,
-            getInjectJsCode(filename, format_info=code_format_info),
-            args=args,
-            plugin_appid=plugin_appid,
-        )
+            self.jd.push_op(msg, *args)
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/page.py` & `minium-1.4.0/minium/miniprogram/base_driver/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,56 +3,86 @@
 """
 @Author: lockerzhang
 @LastEditors: lockerzhang
 @Description: 小程序页面
 @Date: 2019-03-11 14:42:29
 @LastEditTime: 2019-06-05 17:04:02
 """
+from __future__ import annotations
 import re
 from typing_extensions import Self
-from minium.framework.exception import MiniElementNotFoundError, MiniAppError
+from minium.framework.exception import MiniElementNotFoundError, MiniAppError, MiniTimeoutCauseByConnectionBreakError
 import typing
 from .element import *
-from .minium_object import MiniumObject
+from .minium_object import MiniumObject, RetryableApi
 from ...utils.utils import timeout
 from .connection import Command
 import json
+if typing.TYPE_CHECKING:
+    from .app import App
 
 # 需要在setup中加上cssselect库
 # from cssselect.xpath import HTMLTranslator
 # from cssselect.parser import SelectorError
 
 # translator = HTMLTranslator()
 
 
-class Page(MiniumObject):
+class Page(MiniumObject, metaclass=RetryableApi):
     """
     页面相关接口
     """
+    __RETRY_EXCEPTION__ = (MiniTimeoutCauseByConnectionBreakError,)  # 小程序掉线Page实例可能就没用了
+    __RETRY_API__ = [
+        "data",
+        "inner_size",
+        "scroll_height",
+        "scroll_width",
+        "scroll_x",
+        "scroll_y",
+        "scroll_to",
+        "_get_window_properties",
+        # "element_is_exists",
+        # "get_element",
+        # "get_elements",
+        # "_element_is_exists",
+        # "get_elements_by_xpath",
+        # "get_element_by_xpath",
+        # element 相关底层方法
+        "__get_elements",
+        "_get_element",
+        "_get_element_by_xpath",
+        "_get_elements_by_xpath",
+    ]
 
     PLUGIN_PATH_REG = r"^(plugin://|plugin-private://|/?__plugin__/)(\w+)/"
 
-    def __init__(self, page_id, path, query, connection):
+    def __init__(self, page_id, path, query, app: App):
         """
         初始化页面
         """
         super().__init__()
         self.page_id = page_id
         # 处理下path，普通page以"/"开头，插件以"plugin://" 或 "plugin-private://" 或 "__plugin__" 开头
         self.plugin_appid = None
         match = re.search(Page.PLUGIN_PATH_REG, path)
         if match:
             self.plugin_appid = match.group(2)
         elif not path.startswith("/"):
             path = "/" + path
         self.path = path
         self.query = query
-        self.connection = connection
+        self.app = app
+        if app:
+            self.connection = app.connection
         self.is_webview = None  # None: 未知，true: 是，false: 否
 
+    def __del__(self):
+        self.app = None
+
     def __repr__(self):
         return "Page(id={0}, path={1}, query={2})".format(
             self.page_id, self.path, self.query
         )
 
     def __eq__(self, page: Self or str):
         """
@@ -207,15 +237,15 @@
         self,
         selector: str,
         inner_text=None,
         text_contains=None,
         value=None,
         max_timeout=0,
         xpath=None,
-    ) -> Elements:
+    ) -> ElementType:
         """
         find elements in current page, by css selector or xpath
         目前支持的css选择器有:
 
         选择器	              样例	                      样例描述
         .class	             .intro	                    选择所有拥有 class="intro" 的组件
         #id	                 #firstname	                选择拥有 id="firstname" 的组件
@@ -313,15 +343,15 @@
         selector,
         max_timeout=0,
         inner_text=None,
         text_contains=None,
         value=None,
         index=-1,
         xpath=None,
-    ) -> typing.List[BaseElement]:
+    ) -> typing.List[ElementType]:
         """
         find elements in current page, by css selector
         :param selector: 选择器
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
         :param max_timeout: 超时时间
@@ -372,27 +402,29 @@
     def scroll_to(self, scroll_top, duration=300):
         """
         滚动到指定位置
         :param scroll_top:  位置 px
         :param duration:  滚动时长
         :return:
         """
-        self.call_wx_method(
+        if not self.app:
+            raise RuntimeError("please instantiate Page through App.get_current_page()")
+        self.app.call_wx_method(
             "pageScrollTo", [{"scrollTop": scroll_top, "duration": duration}]
         )
 
     def get_elements_by_xpath(
         self,
         xpath,
         max_timeout=10,
         inner_text=None,
         value=None,
         text_contains=None,
         index=-1,
-    ) -> Elements:
+    ) -> ElementType:
         """
         根据xpath查找元素
         :param xpath: xpath
         :param max_timeout: 超时时间
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
@@ -408,15 +440,15 @@
         def search_elements():
             return self._get_elements_by_xpath(xpath, index=index)
 
         return search_elements()
 
     def get_element_by_xpath(
         self, xpath, max_timeout=10, inner_text=None, value=None, text_contains=None
-    ) -> Elements:
+    ) -> ElementType:
         """
         根据xpath查找元素
         :param xpath: xpath
         :param max_timeout: 超时时间
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
@@ -466,16 +498,16 @@
         for el in ret.result.elements:
             elements.append(create(el, self.page_id, self.connection))
             if len(elements) == (index + 1):  # index==-1时，不会match，就会全部返回
                 return elements
         return elements
 
     def __search_child(
-        self, selector_list: list, parent: BaseElement = None, index=-1
-    ) -> typing.List[BaseElement]:
+        self, selector_list: list, parent: ElementType = None, index=-1
+    ) -> typing.List[ElementType]:
         # index == -1: get所有, index >=0: get index+1个
         if len(selector_list) == 0:
             return []
         _selector = selector_list.pop()
         should_be_custom_element = bool(
             len(selector_list)
         )  # 出了最后一层selector，都需要是自定义组件，不然不能往下走
@@ -492,28 +524,28 @@
             if should_be_custom_element and isinstance(_el, CustomElement):
                 real_els.append(_el)
             elif not should_be_custom_element:
                 real_els.append(_el)
             else:
                 self.logger.warn("%s should be a custom element" % _selector)
         if not real_els or len(selector_list) == 0:  # 找不到 或 没有子选择器了
-            return real_els
+            return real_els if index <= -1 else real_els[:index+1]
         child_els = []
         for _el in real_els:
             child_el = self.__search_child(
-                selector_list[0:], _el
+                selector_list[0:], _el, index=-1 if index <= -1 else index - len(child_els)
             )  # selector_list[0:]相当于copy
             child_els += child_el
             if len(child_els) == (index + 1):
                 return child_els
         return child_els
 
     def _get_elements_by_css(
         self, selector: str, max_timeout=0, index=-1
-    ) -> typing.List[BaseElement]:
+    ) -> typing.List[ElementType]:
         """
         1. 现存自定义组件中的class会自动加前缀，但不包括slot占位的元素
         2. slot元素的class命名规则
         2.1 <page><test><view class="这个class不会加前缀"></view></test></page>
         2.2 <custom><test><view class="这个class会加上custom组件对应的前缀"></view></test></custom>
         3. 自定义组件中通过id获取元素失败
         """
@@ -530,15 +562,15 @@
         els = search_elements(_selector_list)
         if len(els) == 0:
             self.logger.warning(f"Could not found any element '{selector}' you need")
         else:
             self.logger.info("find elements success: %s" % str(els))
         return els
 
-    def _get_element(self, selector, max_timeout=0) -> BaseElement:
+    def _get_element(self, selector, max_timeout=0) -> ElementType:
         def search_element():
             ret = self._send("Page.getElement", {"selector": selector})
             return create(ret.result, self.page_id, self.connection)
 
         self.logger.info("try to get element: %s" % selector)
         el = search_element()
         self.logger.info("find element success: %s" % str(el))
@@ -589,38 +621,38 @@
     #     try:
     #         translator.css_to_xpath(selector)
     #         return False
     #     except SelectorError:
     #         return True
     #     return False
 
-    def _get_element_by_xpath(self, xpath: str) -> Elements:
+    def _get_element_by_xpath(self, xpath: str) -> ElementType:
         """
         description: 通过xpath获取元素
         param {*} self
         param {str} xpath
-        return {*} Elements or None
+        return {*} ElementType or None
         """
         xpath = (
             xpath[5:] if xpath.find("/page/") == 0 else xpath
         )  # xpath不能以/page/开头（不存在的根节点）
         try:
             ret = self._send("Page.getElementByXpath", {"selector": xpath})
         except MiniAppError as e:
             if str(e) == "no such element":
                 return None
             raise
         return create(ret.result, self.page_id, self.connection)
 
-    def _get_elements_by_xpath(self, xpath: str, index=-1) -> typing.List[BaseElement]:
+    def _get_elements_by_xpath(self, xpath: str, index=-1) -> typing.List[ElementType]:
         """
         description: 通过xpath获取元素
         param {*} self
         param {str} xpath
-        return {*} List[BaseElement]
+        return {*} List[ElementType]
         """
         xpath = (
             xpath[5:] if xpath.find("/page/") == 0 else xpath
         )  # xpath不能以/page/开头（不存在的根节点）
         if not self._can_i_use("Page.getElementsByXpath"):
             el = self._get_element_by_xpath(xpath)  # 降级使用Page.getElementByXpath
             return [el] if el else []
```

### Comparing `minium-1.3.dev2/minium/miniprogram/base_driver/prefixer.py` & `minium-1.4.0/minium/miniprogram/base_driver/prefixer.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/miniprogram/qq_minium.py` & `minium-1.4.0/minium/miniprogram/qq_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/miniprogram/wx_minium.py` & `minium-1.4.0/minium/miniprogram/wx_minium.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,56 +12,49 @@
 import base64
 import json
 import re
 import threading
 from websocket import WebSocketConnectionClosedException
 
 from minium.utils.injectjs import getInjectJsCode, setInjectJsMode
+from .base_driver.version import build_version
+from .base_driver.minium import BaseMinium
 from .base_driver.app import App
 from .base_driver.connection import Connection
 from .base_driver.minium_object import MiniumObject
 from ..framework.miniconfig import MiniConfig, get_log_level
 from ..framework.exception import *
 from ..native import get_native_driver, BaseNative
 from ..utils.platforms import *
 from ..utils.utils import (
     isWindows,
     isMacOS,
     Version,
     WaitThread,
     WaitTimeoutError,
     add_path_to_env,
+    pick_unuse_port,
+    catch,
 )
-
-LOG_FORMATTER = "%(levelname)-5.5s %(asctime)s %(filename)-10s %(funcName)-15s %(lineno)-3d %(message)s"
+from ..utils.emitter import ee
 
 MAC_DEVTOOL_PATH = "/Applications/wechatwebdevtools.app/Contents/MacOS/cli"
 WINDOWS_DEVTOOL_PATH = "C:/Program Files (x86)/Tencent/微信web开发者工具/cli.bat"
 TEST_PORT = 9420
 UPLOAD_URL = "https://stream.weixin.qq.com/weapp/UploadFile"
 
 
 class LogLevel(object):
     INFO = 20
     DEBUG_SEND = 12
     METHOD_TRACE = 11
     DEBUG = 9
 
 
-def build_version():
-    config_path = os.path.join(os.path.dirname(__file__), "version.json")
-    if not os.path.exists(config_path):
-        return {}
-    else:
-        with open(config_path, "r", encoding="utf8") as f:
-            version = json.load(f)
-            return version
-
-
-class WXMinium(MiniumObject):
+class WXMinium(BaseMinium):
     """
     自动化入口
     """
 
     def __init__(
         self,
         conf: MiniConfig = None,
@@ -81,46 +74,60 @@
         # 公有变量
         if not conf:
             conf = MiniConfig()
         elif isinstance(conf, dict):
             conf = MiniConfig(conf)
         self.conf = conf
         self.logger.setLevel(get_log_level(conf.debug_mode))
-        if native is None and (conf.device_desire or conf.platform == OS_IDE) and conf.platform:
-            self.native = get_native_driver(conf.platform, conf)
-        else:
-            self.native = native
+        self.native = native
+        if native is None and conf.platform:
+            try:
+                self.native = get_native_driver(conf.platform, conf)
+            except KeyError as ke:  # 配置不全
+                self.logger.error(ke)
+            except:
+                self.logger.warning(f"instantiate {conf.platform} native driver fail")
         self.version = build_version().get("version", "1.2.0")
         self.sdk_version: Version = Version("0.0.0")
         self.dev_tool_version: Version = Version("0.0.0")
         self.platform = "ide"  # ide, android, ios
         # self.logger.info(self.version)
         self.start_cmd = ""
         self._app = None
         self.connection = None
         test_port = (
             str(conf.test_port) if conf.get("test_port", None) else str(TEST_PORT)
         )
+        if test_port == "rand":
+            test_port = str(pick_unuse_port())
         self.uri = uri + ":" + test_port
         self.test_port = test_port
         self.open_id = conf.get("account_info", {}).get("open_id", None)
         self.ticket = conf.get("account_info", {}).get("ticket", None)
         self.project_path = conf.get("project_path", None)
         self.is_remote = False
         self.is_connected = False
         self.is_audits_running = False  # 体验评分在跑
+        self.launch_app_lock = threading.RLock()  # 全局只需有一个launch app的线程
+        self.__is_app_relaunching = False
+        self.last_launch_cost_time = 1  # 最后一次拉起小程序需要的时间
+        self.last_launch_error = None  # 成功为none
 
-        self.launch_weapp()
+        try:
+            self.launch_weapp()
 
-        # IdeNative实例有mini属性，因为IdeNative接口通过minium实现
-        if self.platform == "ide" and self.native and hasattr(self.native, "mini"):
-            self.native.mini = self
-        # 根据配置注入一些必要的代码
-        if self.app and not self.app.is_injected:
-            self._inject()
+            # IdeNative实例有mini属性，因为IdeNative接口通过minium实现
+            if self.platform == "ide" and self.native and hasattr(self.native, "mini"):
+                self.native.mini = self
+            # 根据配置注入一些必要的代码
+            if self.app and not self.app.is_injected:
+                self._inject()
+        except:
+            ee.remove_listener("ide_closed", self._relaunch_ide)  # 防止创建失败的minium实例仍引起relaunch
+            raise
 
     @property
     def app(self) -> App:
         return self._app
 
     @app.setter
     def app(self, v: App or None):
@@ -200,15 +207,15 @@
         self.native = None
 
     def __getattr__(self, name):
         """
         当minium中方法不存在且native中存在，返回native的方法
         """
         if name != "native" and self.native:
-            item = getattr(self.native, name)
+            item = getattr(self.native, name, None)
             if callable(item):
                 return item
         raise AttributeError(
             "'%s' object has no attribute '%s'" % (self.__class__.__name__, name)
         )
 
     def __wait_app_initialized(self, timeout, signal):
@@ -308,14 +315,15 @@
                 # mock getUserProfile, 基础库2.10.4后才支持
                 if self.sdk_version >= Version("2.10.4"):
                     not use_native and self._mock_get_user_profile(
                         self.conf.mock_native_modal.get("userInfo", {})
                     )
 
         # conf.mock_request
+        self._evaluate_js("mockNetwork", code_format_info={"interface": "request"})  # 先mock, 再打开network panel才能记录mock的请求
         if self.conf.mock_request and isinstance(self.conf.mock_request, (list, tuple)):
             for item in self.conf.mock_request:
                 try:
                     self.app.mock_request(**item)
                 except Exception as e:
                     self.logger.exception(
                         "mock_request config error, configure item is %s, error is %s"
@@ -426,38 +434,104 @@
         """
         description: 获取当前系统信息，更新platform/sdk_version
         param {*} self
         return {*}
         """
         try:
             system_info = self.get_system_info()
-        except MiniTimeoutError:
+        except MiniTimeoutCauseByConnectionBreakError:
+            # 链接断链了
+            raise
+        except MiniTimeoutError as te:
             # 命令没响应，应该是基础库版本问题
             if self.sdk_version < Version("2.7.3"):
-                raise MiniLaunchError("基础库版本[%s]过低，请确认基础库版本>=2.7.3" % self.sdk_version)
+                raise MiniLaunchError("基础库版本[%s]过低，请确认基础库版本>=2.7.3" % self.sdk_version) from te
             raise
         self.sdk_version = Version(
             system_info.get("SDKVersion", None) or self.sdk_version.version
         )
         platform = system_info.get("platform", "ide").lower()
         self.platform = "ide" if platform == "devtools" else platform
 
     def launch_weapp(self):
         """
         拉起小程序
         """
         self.__setup_dev_tool()
+        stime = time.time()
         self.launch_dev_tool()
         if self.conf.get("platform", None) != "ide" and self.platform  == "ide":
             # launch/connect后仍然是ide, 需要启动远程调试
-            path = self.enable_remote_debug(
-                use_push=self.conf.get("use_push", True),
-                connect_timeout=self.conf.get("remote_connect_timeout", 180),
-            )
+            try:
+                path = self.enable_remote_debug(
+                    use_push=self.conf.get("use_push", True),
+                    connect_timeout=self.conf.get("remote_connect_timeout", 180),
+                )
+            except RemoteDebugConnectionLost:  # 远程连接建立后仍然报 remote lost, 可能是小程序挂了
+                self.release()
+                raise
+            except MiniLaunchError as ml:  # 怎么都拉不起, 尝试重启小程序
+                if self.native:
+                    self.native.start_wechat()
+                raise ml
             self.qr_code = path
+        self.last_launch_cost_time = time.time() - stime
+
+    @property
+    def is_app_relaunching(self):
+        return self.__is_app_relaunching
+
+    def _relaunch_ide(self, *args):
+        """重新拉起ide
+        """
+        if not self.app:
+            self.logger.error("relaunch app but app is never launch successfully, pass")
+            return
+        def _relaunch():
+            if not self.launch_app_lock.acquire(False):
+                self.logger.info("other thread relaunching app")
+                # 已经有线程在 launch weapp
+                return
+            self.logger.info("start relaunch app %d" % threading.get_ident())
+            self.__is_app_relaunching = True
+            stime = time.time()
+            try:
+                if self.connection:
+                    self.connection.destroy()
+                self.close_project()
+                self.launch_dev_tool()
+                if self.conf.get("platform", None) != "ide" and self.platform  == "ide":
+                    # launch/connect后仍然是ide, 需要启动远程调试
+                    try:
+                        path = self.enable_remote_debug(
+                            use_push=self.conf.get("use_push", True),
+                            connect_timeout=self.conf.get("remote_connect_timeout", 180),
+                        )
+                    except RemoteDebugConnectionLost:
+                        self.release()
+                        raise
+                    except MiniLaunchError as ml:  # 怎么都拉不起, 尝试重启小程序
+                        if self.native:
+                            self.native.start_wechat()
+                        raise ml
+                    self.qr_code = path
+                self.last_launch_cost_time = time.time() - stime
+                self.last_launch_error = None
+            except Exception as e:
+                self.last_launch_error = e
+                self.logger.exception(e)
+                if self.connection:
+                    self.connection.destroy()
+            finally:
+                self.logger.info("end relaunch app")
+                self.__is_app_relaunching = False
+                self.launch_app_lock.release()
+        t = threading.Thread(target=_relaunch)
+        t.setDaemon(True)
+        t.start()
 
     def __update_project_config(self):
         project_config_path = os.path.join(self.project_path, "project.config.json")
         if os.path.isfile(project_config_path):
             conf = {}
             setting = {}
             with open(project_config_path, "r", encoding="UTF-8") as fd:
@@ -475,14 +549,20 @@
             ):  # 即使工具启动了，修改config.json依然会开始运行体验评分，所以每次launch认为audit running
                 setting["autoAudits"] = self.conf.audits
             if conf:  # 需要更新
                 j.update(conf)
                 j["setting"].update(setting)
                 json.dump(j, open(project_config_path, "w", encoding="UTF-8"), indent=2)
 
+    def close_project(self):
+        if not self.start_cmd:
+            return
+        if self.project_path and "--auto-account" not in self.start_cmd:
+            self._dev_cli(f'close --project "{self.project_path}"')
+
     def launch_dev_tool(self):
         # start dev tool with minium model
         self.logger.info("Starting dev tool and launch MiniProgram project ...")
         is_port_in_use = False
         if self.project_path:
             if not os.path.exists(self.project_path):
                 raise MiniConfigError("project_path: %s not exists" % self.project_path)
@@ -542,26 +622,26 @@
             # ws连接不上
             self.logger.error(f"{str(e)}, restart now...")
             if is_port_in_use:
                 # 端口被占用，先尝试关掉项目再重试
                 if self.connection:
                     self.connection.send("Tool.close")
                 elif "--auto-account" not in self.start_cmd:
-                    self._dev_cli(f'close --project "{self.project_path}"')
+                    self.close_project()
                 else:
                     raise MiniLaunchError(
                         "In the case with multi-account mode and no connection with dev tool,"
                         " please close devtools by your self"
-                    )
+                    ) from e
                 time.sleep(5)
             if self.start_cmd:  # 重启一次
                 self.logger.info("Starting dev tool again...")
                 err_msg = self._dev_cli(self.start_cmd, input=b"y")
                 if err_msg:
-                    raise MiniLaunchError(err_msg)
+                    raise MiniLaunchError(err_msg) from e
                 else:
                     self.logger.info("Restart success")
                     # launch success, wait ide init
                     if isWindows:
                         # windows更卡
                         time.sleep(10)
                     else:
@@ -574,26 +654,28 @@
             raise
 
     def connect_dev_tool(self):
         i = 3
         while i:
             try:
                 self.logger.info("Trying to connect Dev tool ...")
-                connection = Connection(
+                self.connection = Connection.create(
                     self.uri, timeout=self.conf.get("request_timeout")
                 )
-                self.connection = connection
                 self.__get_dev_tool_info()
                 self._get_system_info()
                 self.app = App(
-                    connection,
+                    self.connection,
                     self.conf.get("auto_relaunch"),
                     native=self.native,
                     platform=self.platform,
                 )
+                ee.on("ide_closed", self._relaunch_ide)
+            except RemoteDebugConnectionLost:  # 链接上了, 但小程序没有响应
+                raise
             except MiniLaunchError:
                 raise
             except Exception as e:
                 self.logger.exception(e)
                 i -= 1
                 if i == 0:
                     raise MiniConnectError(
@@ -628,15 +710,15 @@
 
     def get_system_info(self):
         """
         获取系统信息
         :return:
         """
         return (
-            self.call_wx_method("getSystemInfoSync")
+            self._call_wx_method("getSystemInfoSync")
             .get("result", {"result": {}})
             .get("result", None)
         )
 
     def enable_remote_debug(self, use_push=True, path=None, connect_timeout=180):
         """
         开启真机调试
@@ -713,15 +795,15 @@
                         raise MiniLaunchError("Launch APP Error")
                     if ret1 is True or ret2 is True:
                         break
                     else:
                         # 等不到App.initialized一般就是白屏，通道不通，exit会报错，跳出重试，需要catch
                         try:
                             self.app.exit()
-                        except MiniTimeoutError:
+                        except (MiniTimeoutError, MiniConnectionClosedError):
                             # 白屏的时候切换一下扫码编译，有时会有意想不到效果
                             self.connection.send(
                                 "Tool.enableRemoteDebug",
                                 params={"auto": False},
                                 max_timeout=connect_timeout,
                             )
             # 远程调试开启成功后，小程序运行态已经转到手机，需要重新实例化app
@@ -742,14 +824,15 @@
             "Tool.enableRemoteDebug", max_timeout=connect_timeout
         ).result.qrCode
         with open(path, "wb") as qr_img:
             qr_img.write(base64.b64decode(qr_data))
 
         return path
 
+    @catch
     def reset_remote_debug(self):
         """
         重置远程调试，解决真机调试二维码扫码界面报-50003 等常见错误
         :return:
         """
         return self.connection.send("Tool.resetRemoteDebug")
 
@@ -772,26 +855,50 @@
         return self.connection.send("Tool.getTestAccounts").result.accounts
 
     def shutdown(self):
         """
         关闭 Driver, 释放native引用
         :return: status
         """
-        if getattr(self.native, "mini", None):
+        ee.remove_listener("ide_closed", self._relaunch_ide)
+        if self.native and getattr(self.native, "mini", None):
             self.native.mini = None  # IDE native借用minium通信通道交互
         self.native = None
-        try:
-            if self.is_remote:
+        # 释放app
+        if self.is_remote and self.app:
+            try:
                 self.logger.info("MiniProgram closing")
                 self.app.exit()
-            self.logger.info("Project window closing")
-            self.connection.send("Tool.close")
-            self._wait(lambda: not self.connection._is_connected, 5, 1)
-        except (MiniTimeoutError, MiniAppError) as e:
-            self.logger.exception(f"Shutdown Excrption:{e}")
+            except (
+                MiniTimeoutError,
+                MiniAppError,
+                WebSocketConnectionClosedException,
+                MiniConnectionClosedError,
+            ) as e:
+                self.logger.exception(f"Close app excrption:{e}")
+            finally:
+                self.is_remote = False
+                if self.app is not None:
+                    self.app.native = None
+                    self.app = None
+        # 释放connection
+        if self.connection:
+            try:
+                setattr(self.connection, "_is_close_by_cmd", True)
+                self.connection.send_async("Tool.close", ignore_response=True)
+            except (WebSocketConnectionClosedException, MiniConnectionClosedError, MiniClientOfflineError):
+                pass
+            finally:
+                if self._wait(
+                    lambda: not self.connection._is_connected, 5, 1
+                ):  # already closed
+                    self.connection.remove_all_observers()
+                else:
+                    self.connection.destroy()
+                self.connection = None
 
     def stop_audits(self, report_path=None):
         """
         停止体验评分
         """
         if self.is_audits_running and self.app.platform == "ide":  # 仅工具上有意义
             self.logger.info("stopping audits")
@@ -804,63 +911,39 @@
                         and os.path.join(self.conf.outputs, "audits.html")
                     )
                 )
             except (
                 MiniTimeoutError,
                 MiniAppError,
                 WebSocketConnectionClosedException,
+                MiniConnectionClosedError,
             ) as e:
                 self.logger.exception(f"Stop audits excrption:{e}")
 
     def release(self):
         """
         释放所有资源, 不允许在case中调用
         :return: None
         """
+        native = self.native
         # 停止体验评分, 结果存outputs目录
         self.stop_audits()
-        # 释放native
-        if getattr(self.native, "mini", None):
-            self.native.mini = None  # IDE native借用minium通信通道交互
-        native = self.native
-        self.native = None
-        # 释放app
-        if self.is_remote:
-            try:
-                self.logger.info("MiniProgram closing")
-                self.app.exit()
-            except (
-                MiniTimeoutError,
-                MiniAppError,
-                WebSocketConnectionClosedException,
-            ) as e:
-                self.logger.exception(f"Close app excrption:{e}")
-            finally:
-                if self.app is not None:
-                    self.app.native = None
-                    self.app = None
-        # 释放connection
-        try:
-            self.connection.send_async("Tool.close")
-        except WebSocketConnectionClosedException:
-            pass
-        finally:
-            if self._wait(
-                lambda: not self.connection._is_connected, 5, 1
-            ):  # already closed
-                self.connection.remove_all_observers()
-            else:
-                self.connection.destroy()
+        self.shutdown()
         # 清理一下手机弹窗
         if self.conf.platform != "ide" and native:
-            if not native.handle_modal(
-                btn_text="确定", title="本地调试已结束", force_title=True
-            ):
-                native.handle_modal(
-                    btn_text="OK", title="Local debugging ended", force_title=True
-                )
+            native.close_local_debug_modal()
         native = None
 
+    def wait_app_relaunch(self, timeout=None) -> None or Exception:
+        wait_launch_time = self.last_launch_cost_time + 20 if timeout is None else timeout
+        self.logger.warning(f"app is relaunching, wait {wait_launch_time} seconds for it")
+        if not self.launch_app_lock.acquire(timeout=wait_launch_time):
+            return TimeoutError(f"app did not relaunch within {wait_launch_time} seconds")
+        self.logger.warning("app is relaunch complete")
+        self.launch_app_lock.release()
+        if self.last_launch_error:
+            return self.last_launch_error
+
 
 if __name__ == "__main__":
 
     mini = WXMinium()
```

### Comparing `minium-1.3.dev2/minium/native/__init__.py` & `minium-1.4.0/minium/native/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/android_base/__init__.py` & `minium-1.4.0/minium/native/lib/android_base/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/__init__.py` & `minium-1.4.0/minium/native/lib/at/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/apkapi.py` & `minium-1.4.0/minium/native/lib/at/apkapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/atproxy.py` & `minium-1.4.0/minium/native/lib/at/atproxy.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/bin/AtServer.apk` & `minium-1.4.0/minium/native/lib/at/bin/AtServer.apk`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/bin/AtStub.jar` & `minium-1.4.0/minium/native/lib/at/bin/AtStub.jar`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/command_line.py` & `minium-1.4.0/minium/native/lib/at/command_line.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/accesshelper.py` & `minium-1.4.0/minium/native/lib/at/core/accesshelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/adbwrap.py` & `minium-1.4.0/minium/native/lib/at/core/adbwrap.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/basedriver.py` & `minium-1.4.0/minium/native/lib/at/core/basedriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/case_repair_adapter.py` & `minium-1.4.0/minium/native/lib/at/core/case_repair_adapter.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/config.py` & `minium-1.4.0/minium/native/lib/at/core/config.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/element.py` & `minium-1.4.0/minium/native/lib/at/core/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/exceptions.py` & `minium-1.4.0/minium/native/lib/at/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/javadriver.py` & `minium-1.4.0/minium/native/lib/at/core/javadriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/resguard.py` & `minium-1.4.0/minium/native/lib/at/core/resguard.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/stf/mincap.py` & `minium-1.4.0/minium/native/lib/at/core/stf/mincap.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/stf/minitouch.py` & `minium-1.4.0/minium/native/lib/at/core/stf/minitouch.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/uixml.py` & `minium-1.4.0/minium/native/lib/at/core/uixml.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/core/websocketcli.py` & `minium-1.4.0/minium/native/lib/at/core/websocketcli.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/eventmonitor.py` & `minium-1.4.0/minium/native/lib/at/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/hook.py` & `minium-1.4.0/minium/native/lib/at/hook.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/jlogcat.py` & `minium-1.4.0/minium/native/lib/at/webdriver/webelement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,257 +1,275 @@
 # -*- coding: utf-8 -*-
 """
 @author: 'xiazeng'
-@created: 2016/12/2 
+@created: 2016/12/22 
 """
-import re
+import logging
 import time
-import datetime
-import threading
-import sys
-
-if sys.version_info[0] < 3:
-    from Queue import Queue, Empty
-else:
-    from queue import Queue, Empty
+import at
+from at.webdriver import jsapi
 
-import logging
 
 logger = logging.getLogger()
+MM_X5_CLASS_NAME = "com.tencent.smtt.webkit.WebView"#这个是X5的
+ANDROID_WEBKIT_CLASS_NAME = "android.webkit.WebView"
 
 
-def decode_bytes(bs):
-    ds = ['ascii', 'utf-8', 'gbk']
-    for d in ds:
-        try:
-            return bs.decode(d)
-        except UnicodeDecodeError:
-            pass
-    # 可能出现utf-8被截断的场景
-    # UnicodeDecodeError: 'utf-8' codec can't decode byte 0xe9 in position 4094: invalid continuation byte
-    return bs.decode("utf-8", 'ignore')
-
-
-class LogRecord(object):
-    reg_str = r"(?P<time>(\d{4}-)?\d{2}-\d{2}\s+\d{2}:\d{2}:\d{2}\.\d+)\s+" \
-              r"(?P<level>[VDIWEFS])\/" \
-              r"(?P<tag>.*(?=\(\s*\d+\s*\)))\(\s*" \
-              r"(?P<pid>\d+)\s*\)\s*:\s+" \
-              r"(?P<msg>.*)"
-    reg = re.compile(reg_str, flags=re.VERBOSE | re.MULTILINE)
-
-    def __init__(self, line):
-        self.raw_line = line
-        m = LogRecord.reg.match(line)
-        if m is None:
-            raise RuntimeError("invalided line:" + line)
-        self.time = m.group("time")
-        self.level = m.group("level")
-        self.tag = m.group("tag")
-        self.pid = m.group("pid")
-        self.msg = m.group("msg")
-
-    @property
-    def ts(self):
-        t = self.time.split(".")
-        if len(self.time.split("-")) != 3:
-            time_str = "%s-%s" % (datetime.datetime.now().year, t[0])
+class WebElementNotFound(RuntimeError):
+    pass
+
+
+class WebElement(object):
+    def __init__(self, page, web_view_bounds=None, hid=None, css=None, text=None, cls_name=None, xpath=None, tag_name=None, name=None, text_contains=None, shadow_roots=None,
+                          shadow_root=None):
+        self.page = page
+        self.ws_url = ""
+        self.wrap_view_cls = MM_X5_CLASS_NAME
+        serial = self.page.serial
+        self.at = page.at
+        self.web_view_rect = web_view_bounds
+        #print "web_view_rect",self.web_view_rect
+        self._json_element = None
+        self._js_element = None
+        if hid:
+            word = "id"
+            selector = hid
+            self._selector = "#%s" % hid#根据id来进行css_selector查找
+        elif css:
+            word = "cssSelector"
+            selector = css
+            self._selector = css #css语句
+        elif text:
+            word = "textContent"
+            selector = text
+            self._selector = ':text("%s")' % text #输入文字
+        elif cls_name:
+            word = "className"
+            selector = cls_name
+            self._selector = '.%s' % text  #根据.来输入类名
+        elif xpath:
+            word = "xpath"
+            selector = xpath
+        elif tag_name:
+            word = "tagName"
+            selector = tag_name
+            self._selector = tag_name
+        elif name:
+            word = "name"
+            selector = name
+            self._selector = name
+        else:
+            raise AssertionError("no way to go")
+        self.word = word
+        self.selector = selector
+
+        self._instance = 0
+
+    def instance(self, num):#相同元素中的第几个
+        self._instance = num
+        return self
+
+    def word_big_first_letter(self):#转第一个字母为大写字母
+        return self.word[0].upper()+self.word[1:]
+
+    def wait_exists(self, timeout=10):#等待出现
+        s = time.time()
+        while time.time() - s < timeout:
+            if self.exists():
+                return True
+            time.sleep(1)
+        return False
+
+    def screen(self, filename, quality=100):
+        """
+        截图，并且圈出对应的坐标点
+        """
+        x, y, width, height = self.rect()
+        self.at.device.screen_point(filename, x, y, width, height, quality)
+
+    def scroll_to(self, x, y):
+        self.page.invoke_js(jsapi.SCROLL_TO, x, y)
+
+    def click(self):
+        if not self.page.click_by_ui:
+            raise RuntimeError("not implementation")
+        else:
+            # self.wait_exists()
+            self.find_json_element()
+            if not self._js_element['in_screen']:
+                self.call_js("scrollIntoView", [])
+                # self.scroll_to(self._js_element['rect']['left'], self._js_element['rect']['top'])
+                time.sleep(2)
+                self.find_json_element(True)
+            # if not self._js_element['in_screen']:
+            #     raise RuntimeError(u"element invisible")
+            x, y, width, height = self.rect()
+            x = x + width / 2
+            y = y + height / 2
+
+            time.sleep(1)
+            self.at.device.click_on_point(x, y)#点击元素的中心点
+            time.sleep(1)
+
+    def get_center_position(self):
+        if not self.page.click_by_ui:
+            raise RuntimeError("not implementation")
         else:
-            time_str = int(t[0])
-        timetuple = time.strptime(time_str, "%Y-%m-%d %H:%M:%S")
-        ts = time.mktime(timetuple) * 1000 + int(t[1])
-        return ts
-
-    @classmethod
-    def is_valid_line(cls, line):
-        m = cls.reg.match(line)
-        if not m:
-            logger.warning(line)
-        return m is not None
-
-    def __repr__(self):
-        return "%s %s %s %s" % (self.time, self.level, self.tag, self.msg)
-
-
-class AsynchronousFileReader(threading.Thread):
-    """
-    Helper class to implement asynchronous reading of a file
-    in a separate thread. Pushes read lines on a queue to
-    be consumed in another thread.
-    """
-
-    def __init__(self, fd, process, queue):
-        assert isinstance(queue, Queue)
-        assert callable(fd.readline)
-        threading.Thread.__init__(self)
-        self._fd = fd
-        self._process = process
-        self.daemon = True
-        self._queue = queue
-        self._should_stop = False
-
-    def run(self):
-        """The body of the tread: read lines and put them on the queue."""
-        count = 0
-        next_count = 10000
-        start = time.time()
+            # self.wait_exists()
+            self.find_json_element()
+            if not self._js_element['in_screen']:
+                self.call_js("scrollIntoView", [])
+                # self.scroll_to(self._js_element['rect']['left'], self._js_element['rect']['top'])
+                time.sleep(2)
+                self.find_json_element(True)
+            if not self._js_element['in_screen']:
+                raise RuntimeError(u"element invisible")
+            x, y, width, height = self.rect()
+            x = x + width / 2
+            y = y + height / 2
+            return x, y
+
+    def long_click(self, duration=3000):
+        method_name = self.word
+        if not self.page.click_by_ui:
+            raise RuntimeError("not implementation")
+        else:
+            # self.wait_exists()
+            x, y, width, height = self.rect()
+            x = x + width / 2
+            y = y + height / 2
+            time.sleep(1)
+            self.at.device.long_click_on_point(x, y, duration)
+            time.sleep(1)
+
+    def web_rect(self):
+        ret = self.find_json_element()
+        json_rect = ret['rect']
+        return json_rect["left"], json_rect['top'], json_rect["width"], json_rect["height"]
+
+    def rect(self):
+        x, y, width, height = self.web_rect()
+        target_x, target_y = self.transfer_web_point(x, y)
+        target_width, target_height = self.transfer_web_distance(width, height)
+        return target_x, target_y, target_width, target_height
+
+    def call_js(self, sub_method, args, timeout=10):
+        r = None
+        t = time.time()
+        end_time = time.time()
+        while end_time - t < timeout:
+            try:
+                r = self.page.invoke_js(jsapi.ELEMENT_OPERATION, self.selector, sub_method, args, self._instance)
+                break
+            except jsapi.ElementNotExists as e:
+                end_time = time.time()
+                if end_time - t < timeout:
+                    time.sleep(2)
+                else:
+                    raise e
+        return r
+
+    def find_json_element(self, is_refresh=False, timeout=10):
+        if self._js_element is None or is_refresh:
+            self._js_element = self.call_js(None, [], timeout)
+        return self._js_element
+
+    def point_rate(self):
+        rect = self.web_view_rect
+        page_width = self.page.width
+        page_height = self.page.height
+        view_width = rect[2] - rect[0]
+        view_height = rect[3] - rect[1]
+        return view_width*1.0/page_width, view_height*1.0/page_height
+
+    def transfer_web_distance(self, x, y):
+        x_rate, y_rate = self.point_rate()
+        return x*x_rate, y * y_rate
+
+    def transfer_web_point(self, x, y):
+        x = x if x > 0 else 0
+        y = y if y > 0 else 0
+        rect = self.web_view_rect
+        #print "rect:",rect
+        x_rate, y_rate = self.point_rate()
+        target_x = int(rect[0] + x * x_rate)
+        target_y = int(rect[1] + y * y_rate)
+        logger.info("%d, %d" % (target_x, target_y))
+        return target_x, target_y
+
+    def exists(self, timeout=3):
         try:
-            while True:
-                if self._should_stop:
-                    break
-                if self._process.poll() is not None:
-                    logging.error("process stopped:%s, logcount:%s", self._process.poll(), count)
-                    break
-                line = self._fd.readline()
-                if line:
-                    count += 1
-                    self._queue.put(line)
-                    if count > next_count:
-                        t = time.time() - start
-                        logger.debug("total:%s, cost:%d, produce rate:%s per second", count, t, int(count / t))
-                        next_count += next_count
-                    if line == b'read: unexpected EOF!\n':
-                        break
+            self.find_json_element(timeout=timeout)
         except:
-            logger.exception("exception")
+            return False
+        return True
 
-        logger.info("read logcat finish: %s", self._should_stop)
+    def scroll_to_screen(self, max_scroll_num=10):
+        for i in range(max_scroll_num):
+            if self.is_in_screen():
+                return True
+            time.sleep(1)
+        raise RuntimeError(u"scroll over %d", max_scroll_num)
 
-    def eof(self):
-        """Check whether there is no more content to expect."""
-        return not self.is_alive()
-
-    def stop(self):
-        self._should_stop = True
-        self.join(1)
-
-
-class JLogCat(threading.Thread):
-    def __init__(self, adb):
-        threading.Thread.__init__(self)
-        self._is_stop = False
-        self.adb = adb
-        # Launch the asynchronous readers of the process' stdout.
-        self.stdout_queue = Queue()
-        self._bg_run()
-        self.mutex = threading.Lock()
-        self.filter_map = {}
-        self.filter_values = []
-        self.names = []
-        self.redirect_file = None
-
-    def redirect_to_path(self, path):
-        self.redirect_file = open(path, "a")
-
-    def _bg_run(self, clear_logcat=True):
-        if clear_logcat:
-            self.adb.run_adb("logcat -c")
-        self.process = self.adb.run_adb("logcat  -v time", False)
-        logging.info("process_id:%s", self.process.pid)
-        stdout_reader = AsynchronousFileReader(self.process.stdout, self.process, self.stdout_queue)
-        stdout_reader.start()
-        self.stdout_reader = stdout_reader
-
-    def run(self):
-        # Check the queues if we received some output (until there is nothing more to get).
-        retype = type(re.compile('hello, world'))
-        line_count = 0
-        start = time.time()
-        next_count = 10000
-
-        while not self._is_stop:
-            if self.stdout_reader.eof():
-                self._bg_run(clear_logcat=False)
-            while not self.stdout_queue.empty() and not self._is_stop:
-                line = None
-                try:
-                    line = self.stdout_queue.get(timeout=0.1)
-                except Empty:
-                    logger.info("empty")
-                    pass
-                line = decode_bytes(line)
-                line_count += 1
-                if line_count > next_count:
-                    t = time.time() - start
-                    logger.debug("total:%s, cost:%d, consume rate:%s per second", line_count, t, int(line_count / t))
-                    next_count += next_count
-                if line:
-                    if self.redirect_file:
-                        self.redirect_file.write(line)
-                    for fm in self.filter_values:
-                        records = fm["records"]
-                        for keyword in fm["keywords"]:
-                            if isinstance(keyword, str):
-                                if keyword in line:
-                                    logger.debug("[%s]+logcat, %s", self.ident, line.strip())
-                                    records.append(line.strip())
-                            elif isinstance(keyword, retype):
-                                if keyword.match(line):
-                                    logger.debug("[%s]+logcat, %s", self.ident, line.strip())
-                                    records.append(line.strip())
-        logger.info("finished: %s", self._is_stop)
-
-    def start_record(self, name, *args):
+    def is_in_screen(self):
         """
-        开始等待，日志
-        :param name:标识名称，任意字符串，后面取日志要根据这个标识来区分
-        :param *args: 日志匹配的关键字
-        :return:
+        元素是否在屏幕内部，但是不一定可见
         """
-        self.mutex.acquire()
-        self.filter_map[name] = {
-            "keywords": args,
-            "records": []
-        }
-        self.filter_values = list(self.filter_map.values())
-        self.mutex.release()
-
-    def _get_records(self, name):
-        self.mutex.acquire()
-        if name not in self.filter_map:
-            lines = []
+        if not self.exists():
+            return False
+        json_ret = self.find_json_element(True)
+        return json_ret['in_screen']
+
+    def is_visible(self):
+        '''
+        元素是否在屏幕上可见
+        :return:
+        '''
+        if not self.exists():
+            return False
+        json_ret = self.find_json_element(True)
+        return json_ret['visible']
+
+    def get_element(self):
+        json_e = self.find_json_element()
+        if json_e:
+            return json_e
         else:
-            lines = self.filter_map[name]["records"]
-        records = [LogRecord(l) for l in lines if LogRecord.is_valid_line(l)]
-        self.mutex.release()
-        return records
+            raise RuntimeError(u"Not Found")
 
-    def get_lines(self, name):
-        return self._get_records(name)
+    def get_text(self):
+        json_e = self.find_json_element()
+        if json_e:
+            return json_e.get('text')
+
+    def enter(self, text):
+        raise RuntimeError("not implementation")
+
+
+    #富文本输入方法
+    def innerHtml(self,text = None):
+        '''
+        设置content中的innerHTML
+        :param text:
+        :return:
+        '''
+        if text:
+            return self.call_js(jsapi.ELEMENT_OPERATION_SUPPLY_METHOD.SET_PROPERTY,["innerHTML",text])
+        else:
+            return self.call_js(jsapi.ELEMENT_OPERATION_SUPPLY_METHOD.SET_PROPERTY,["innerHTML"])
 
-    def wait_records(self, name, count=1, timeout=10):
-        s = time.time()
-        records = []
-        while time.time() - s < timeout:
-            records = self._get_records(name)
-            if len(records) >= count:
-                return records
-            time.sleep(0.1)
-        return records
-
-    def new_wait_records(self, name, count=1, timeout=20):
-        time.sleep(timeout)
-        records = self._get_records(name)
-        if len(records) < count:
-            time.sleep(5)
-            records = self._get_records(name)
-        return records
-
-    def stop_record(self, name):
-        records = self._get_records(name)
-        self.mutex.acquire()
-        del self.filter_map[name]
-        self.filter_values = list(self.filter_map.values())
-        self.mutex.release()
-        return records
-
-    def stop(self):
-        self._is_stop = True
-        self.stdout_reader.stop()
-        self.join()
-        self.adb.kill_pid(self.process.pid)
-        if self.redirect_file:
-            self.redirect_file.close()
-        logger.info("logcat finish")
+    def val(self, text=None):
+        """
+        直接设置dom节点的value值
+        :param text:
+        :return:
+        """
+        if text:
+            return self.call_js(jsapi.ELEMENT_OPERATION_SUPPLY_METHOD.SET_PROPERTY, ["value", text])
+        else:
+            return self.call_js(jsapi.ELEMENT_OPERATION_SUPPLY_METHOD.SET_PROPERTY, ["value"])
 
-    def __del__(self):
-        self.stop()
+    def attr(self, name, value=None):
+        if value:
+            return self.call_js("setAttribute", [name, value])
+        else:
+            return self.call_js("getAttribute", [name])
```

### Comparing `minium-1.3.dev2/minium/native/lib/at/keycode.py` & `minium-1.4.0/minium/native/lib/at/keycode.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/perfcollector.py` & `minium-1.4.0/minium/native/lib/at/perfcollector.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/AtEvent.py` & `minium-1.4.0/minium/native/lib/at/tests/AtEvent.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/atdevicetest.py` & `minium-1.4.0/minium/native/lib/at/tests/atdevicetest.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/drivertest.py` & `minium-1.4.0/minium/native/lib/at/tests/drivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/elementtest.py` & `minium-1.4.0/minium/native/lib/at/tests/elementtest.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/images/1.jpg` & `minium-1.4.0/minium/native/lib/at/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/images/2.jpg` & `minium-1.4.0/minium/native/lib/at/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/images/image.jpg` & `minium-1.4.0/minium/native/lib/at/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/minitouch_test.py` & `minium-1.4.0/minium/native/lib/at/tests/minitouch_test.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/u2test.py` & `minium-1.4.0/minium/native/lib/at/tests/u2test.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/uixmltest.py` & `minium-1.4.0/minium/native/lib/at/tests/uixmltest.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/tests/webdrivertest.py` & `minium-1.4.0/minium/native/lib/at/tests/webdrivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/apkinfo.py` & `minium-1.4.0/minium/native/lib/at/utils/apkinfo.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/axmlparser.py` & `minium-1.4.0/minium/native/lib/at/utils/axmlparser.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/axmlparser3.py` & `minium-1.4.0/minium/native/lib/at/utils/axmlparser3.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/commonhelper.py` & `minium-1.4.0/minium/native/lib/at/utils/commonhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/decorator.py` & `minium-1.4.0/minium/native/lib/at/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/nbsp.py` & `minium-1.4.0/minium/native/lib/at/utils/nbsp.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/utils/threadhelper.py` & `minium-1.4.0/minium/native/lib/at/utils/threadhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/driver.py` & `minium-1.4.0/minium/native/lib/at/webdriver/driver.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/jsapi.py` & `minium-1.4.0/minium/native/lib/at/webdriver/jsapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/miniapp.py` & `minium-1.4.0/minium/native/lib/at/webdriver/miniapp.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/stub.js` & `minium-1.4.0/minium/native/lib/at/webdriver/stub.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/tabdescription.py` & `minium-1.4.0/minium/native/lib/at/webdriver/tabdescription.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/tabwebsocket.py` & `minium-1.4.0/minium/native/lib/at/webdriver/tabwebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/webhelper.py` & `minium-1.4.0/minium/native/lib/at/webdriver/webhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/webdriver/wspools.py` & `minium-1.4.0/minium/native/lib/at/webdriver/wspools.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/at/wechat/activtiy.py` & `minium-1.4.0/minium/native/lib/at/wechat/activtiy.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/case_repair_sdk/__init__.py` & `minium-1.4.0/minium/native/lib/case_repair_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/case_repair_sdk/default_trace.py` & `minium-1.4.0/minium/native/lib/case_repair_sdk/default_trace.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/wda/__init__.py` & `minium-1.4.0/minium/native/lib/wda/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/wda/screenhelper.py` & `minium-1.4.0/minium/native/lib/wda/screenhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/wda/xcui_element_types.py` & `minium-1.4.0/minium/native/lib/wda/xcui_element_types.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/wx_wda/wdaUI.py` & `minium-1.4.0/minium/native/lib/wx_wda/wdaUI.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/lib/wx_wda/webDriverTool.py` & `minium-1.4.0/minium/native/lib/wx_wda/webDriverTool.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/qq_native/qandroidnative.py` & `minium-1.4.0/minium/native/qq_native/qandroidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/qq_native/qbasenative.py` & `minium-1.4.0/minium/native/qq_native/qbasenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/qq_native/qiosnative.py` & `minium-1.4.0/minium/native/qq_native/qiosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/native/wx_native/androidnative.py` & `minium-1.4.0/minium/native/wx_native/androidnative.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import threading
 import shutil
 import ssl
 import requests
 import re
 from enum import Enum
 from ..lib.android_base import UiDefine, ScreenType
+from .wording import Language, WORDING
 
 ssl._create_default_https_context = ssl._create_unverified_context
 
 WECHAT_PACKAGE = "com.tencent.mm"
 WECHAT_ACTIVITY = "ui.LauncherUI"
 MINIPROGRAM_ACTIVITY = "plugin.appbrand.ui.AppBrandUI"
 MINIPROGRAM_PLUGIN_ACTIVITY = "plugin.appbrand.ui.AppBrandPluginUI"
@@ -147,14 +148,17 @@
             # self.e.text("从相册选取二维码").click()
             self.e.text("所有图片").click()
             self.e.text(gallery_name).click()
             self.e.desc_contains("图片 1").click()
             self.e.text_contains("扫描中").wait_disappear()
 
     def screen_shot(self, filename, quality=30):
+        return self._screen_shot(filename, quality)
+
+    def _screen_shot(self, filename, quality=30):
         """
         安卓截图有两种方式：
         1. via at
         2. via adb screencap
         via at现存问题: 可能因为网络、at进程被kill等问题, 截图时间超长
         """
         if self.screen_type == ScreenType.AT:
@@ -330,15 +334,15 @@
         """
         if answer:
             return self._handle_btn("", timeout=5.0, text_matches="允许|确定")
         else:
             return self._handle_btn("取消", timeout=5.0)
 
     def _handle_btn(self, btn_text="确定", timeout=0.5, text_matches=None):
-        logger.debug("handle android.widget.Button[%s]" % text_matches or btn_text)
+        logger.debug("handle android.widget.Button[%s]" % (text_matches or btn_text))
 
         def do():
             e = self.e.cls_name("android.widget.Button").focusable(True)
             if text_matches:
                 e.text_matches(text_matches)
             else:
                 e.text(btn_text)
@@ -369,16 +373,16 @@
     def forward_miniprogram(self, name, text=None, create_new_chat=True):
         self.ui.action_menu.click()
         if not self.e.text("发送给朋友").click_if_exists():
             assert self.e.text("转发给朋友").click_if_exists(0.5), "找不到转发按钮"
         return self.forward_miniprogram_inside(name, text, create_new_chat)
 
     def _create_new_chat(self, timeout=0.5):
-        # 点击"创建新聊天"
-        return self.e.text_matches("创建新的?聊天").click_if_exists(timeout)
+        # 点击"创建新聊天"/"创建聊天"/"创建新的聊天"
+        return self.e.text_matches("创建(新的)?聊天").click_if_exists(timeout)
 
     def forward_miniprogram_inside(self, name, text=None, create_new_chat=True):
         if create_new_chat and self._create_new_chat():
             self.e.edit_text().enter(name)
             time.sleep(1)
             self.e.text_contains(name).click(True)
             if self.e.text("确定(1)").exists():
@@ -470,14 +474,30 @@
 
     def start_wechat(self):
         if self.at.adb.app_is_running(WECHAT_PACKAGE):
             if self.debug:
                 return
             self.at.adb.stop_app(WECHAT_PACKAGE)  # 先关掉
         self.at.adb.start_app(WECHAT_PACKAGE, WECHAT_ACTIVITY)
+        # 检测微信画面, 10s
+        timeout = time.time() + 10
+        while time.time() < timeout:
+            views = self.at.java_driver.dump_ui(1)
+            texts = set([v.text for v in views])
+            if texts.issuperset(WORDING.COMMON.LOGIN_WORDS.zh):
+                WORDING.setLanguage(Language.zh)
+                logger.info("wechat language: %s" % Language.zh.name)
+                break
+            elif texts.issuperset(WORDING.COMMON.LOGIN_WORDS.en):
+                WORDING.setLanguage(Language.en)
+                logger.info("wechat language: %s" % Language.en.name)
+                break
+        else:
+            logger.info("wechat language use default: %s" % WORDING.language.name)
+        
 
     def fold_keybroad(self):
         self.at.adb.press_back()
 
     def to_main_ui(self, timeout=3):
         el1 = self.e.pkg(WECHAT_PACKAGE).desc("返回")
         el2 = self.e.pkg(WECHAT_PACKAGE).desc("关闭")
@@ -501,15 +521,15 @@
 
     def click_point(self, x, y):
         """
         Alias for click_coordinate
         """
         return self.click_coordinate(x, y)
 
-    def get_mem_used_new(self, pkg_name, pid):
+    def _get_mem_used_new(self, pkg_name, pid):
         used = 0
         i = 0
         m = None
         m1 = None
         m2 = None
         cmd = "dumpsys meminfo %s" % pkg_name
         # logger.info(cmd)
@@ -564,27 +584,27 @@
             for line in ls:
                 if line.find(tag) > -1:
                     used_str = line.split("K: ")[0]
                     used = int(used_str.replace(",", "")) / 1024
                     break
         return used
 
-    def get_cpu_rate_by_file(
+    def _get_cpu_rate_by_file(
         self, mPid, mLastPidUserCpuTime, mLastPidKernelCpuTime, mLastTotalCpuTime
     ):
         # 计算cpu，读取/proc/stat的数据，计算cpuTime
         # 读取/proc/mPid/stat的数据，计算当前小程序的cpu数据
         pid_stat_file = "/proc/" + str(mPid) + "/stat"
         outputs = self.at.adb.run_shell("cat %s" % (pid_stat_file))
         # logger.info(outputs)
         pid_cpu_info_list = outputs.split(" ")
         # logger.info(pid_cpu_info_list)
         if len(pid_cpu_info_list) < 17:
             return 0, mLastPidUserCpuTime, mLastPidKernelCpuTime, mLastTotalCpuTime
-        cpuTime = self.get_cpu_time()
+        cpuTime = self._get_cpu_time()
         # logger.info(cpuTime)
         # 该进程处于用户态的时间
         pidUTime = int(pid_cpu_info_list[13])
         # logger.info(pidUTime)
         # 该进程处于内核态的时间
         pidSTime = int(pid_cpu_info_list[14])
         # logger.info(pidSTime)
@@ -610,15 +630,15 @@
         return (
             pidCpuUsage,
             mLastPidUserCpuTime,
             mLastPidKernelCpuTime,
             mLastTotalCpuTime,
         )
 
-    def get_cpu_time(self):
+    def _get_cpu_time(self):
         stat_file = "/proc/stat"
         outputs = self.at.adb.run_shell("cat %s" % (stat_file))
         # logger.info(outputs)
         lines = outputs.split("\n")
         list = lines[0].split(" ")
         # logger.info(list)
         if len(list) < 9:
@@ -644,15 +664,15 @@
             stime = time.time()
             # get cpu
             (
                 perf_cpu,
                 mLastPidUserCpuTime,
                 mLastPidKernelCpuTime,
                 mLastTotalCpuTime,
-            ) = self.get_cpu_rate_by_file(
+            ) = self._get_cpu_rate_by_file(
                 pid, mLastPidUserCpuTime, mLastPidKernelCpuTime, mLastTotalCpuTime
             )
             # get fps
             if curview:
                 fps_lines = self.at.adb.get_fps(curview)
                 if len(fps_lines) <= 8:
                     doudi_currentview = (
@@ -666,15 +686,15 @@
                     logger.error(e)
                     # logger.info(fps_lines)
                     fps_data = 0
 
             else:
                 fps_data = 0
             # get mem
-            perf_mem = self.get_mem_used_new(processname, pid)
+            perf_mem = self._get_mem_used_new(processname, pid)
 
             # record
             logger.info(
                 "perf_cpu: %s, fps_data: %s, perf_mem: %s"
                 % (perf_cpu, fps_data, perf_mem)
             )
             timestamp = int(time.time())
@@ -682,15 +702,15 @@
                 {
                     "cpu": perf_cpu,
                     "mem": float(perf_mem),
                     "fps": fps_data,
                     "timestamp": timestamp,
                 }
             )
-            self._screen_shot("%d.png" % timestamp)
+            self._screen_shot(os.path.join(self.outputs_screen, "%d.png" % timestamp))
             etime = time.time()
             if etime - stime > timeinterval:
                 continue
             time.sleep(etime - stime)
 
     def _start_get_perf(self, timeinterval=15):
         self.perf_flag = True
@@ -1039,17 +1059,14 @@
             return 0
         return int(round((frame_count - 1) / seconds))
 
     @property
     def e(self):
         return self.at.e
 
-    def _screen_shot(self, filename):
-        return self.screen_shot(os.path.join(self.outputs_screen, filename))
-
     # 云环境上莫名其妙卡死在这里了。。。
     @wait(60, False)
     def check_connection(self, *args):
         # 检查atsub链接
         if self.at.java_driver.ping():
             return True
         # reconnect
@@ -1057,12 +1074,19 @@
             self.at.java_driver.close_remote()
             time.sleep(1)
             self.at.java_driver._init(True)
         except Exception as e:
             logger.exception(e)
             return False
         return self.at.java_driver.is_remote_running()
+    
+    def close_local_debug_modal(self):
+        self.handle_modal(
+            btn_text=WORDING.COMMON.MODAL_CONFIRM.value, title=WORDING.COMMON.LOCAL_DEBUG_MODAL_TITLE.value, force_title=True
+        ) or self.handle_modal(
+            btn_text=WORDING.COMMON.MODAL_CONFIRM.value, title=WORDING.COMMON.LOCAL_DEBUG_MODAL_TITLE2.value, force_title=True
+        )
 
 
 if __name__ == "__main__":
     n = WXAndroidNative({"lang": "en"})
     n.handle_modal("queding", "")
```

### Comparing `minium-1.3.dev2/minium/native/wx_native/basenative.py` & `minium-1.4.0/minium/native/wx_native/basenative.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import logging
 import time
 import os
 import shutil
 import json
 import threading
 import types
+import typing
 from functools import wraps
 
 from minium.utils.utils import timeout
 from ..exception import *
 from ...utils.emitter import ee
+from .wording import Language, WORDING
 
 logger = logging.getLogger("minium")
 
 
 def call_funtion_log(func, name: str):
     @wraps(func)
     def wrapper(*args, **kwargs):
@@ -35,22 +37,42 @@
         for k, v in attr_dict.items():
             if isinstance(v, types.FunctionType) and not k.startswith("_"):
                 attr_dict[k] = call_funtion_log(v, f"{cls_name}.{k}")
         return type.__new__(mcs, cls_name, bases, attr_dict)
 
 
 class BaseNative(object, metaclass=NativeMetaClass):
+    _require_conf_: typing.List[typing.Union[str, tuple, list]] = []  # 配置必要的字段
     def __init__(self, json_conf):
+        self._check_config(json_conf or {})  # 检查必要的配置字段
         self.json_conf = json_conf
         self.perf_data = []
         self.__auto_authorize_thread = None
         self.__auto_authorize_lock = threading.Condition()
         self.__auto_authorize_flag = False
         self.__last_notify_time = time.time()
         self.auto_authorize = False  # 是否自动授权
+        self.language = Language.zh  # 默认中文, start wechat时检测
+
+    def _check_config(self, conf):
+        """检查配置必要字段
+
+        :param dict conf: 配置dict
+        """
+        for key in self._require_conf_:
+            if isinstance(key, (tuple, list)):
+                conform = False
+                for k in key:
+                    if k in conf:
+                        conform = True
+                        break
+                if not conform:
+                    raise KeyError(f"({' or '.join(key)}) is required in instantiate {self.__class__.__name__}")
+            elif key not in conf:
+                raise KeyError(f"{key} is required in instantiate {self.__class__.__name__}")
 
     def release(self):
         self.release_auto_authorize()
 
     def start_wechat(self):
         """
         启动微信
@@ -630,14 +652,19 @@
             self.__auto_authorize_flag = False
             self.__notify()
             logger.info("stopping auto authorize thread")
             self.__auto_authorize_thread.join()
             logger.info("stop auto authorize thread")
             self.__auto_authorize_thread = None
 
+    def close_local_debug_modal(self):
+        self.handle_modal(
+            btn_text=WORDING.COMMON.MODAL_CONFIRM.value, title=WORDING.COMMON.LOCAL_DEBUG_MODAL_TITLE.value, force_title=True
+        )
+
     # protect method
     def _wait(self, func, timeout, interval=1):
         """
         等待直到`func`为true
         :func: callable function
         :timeout: timeout
         :interval: query step
```

### Comparing `minium-1.3.dev2/minium/native/wx_native/idenative.py` & `minium-1.4.0/minium/native/wx_native/idenative.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         try:
             result = self._mini.connection.send("Tool.getInfo", max_timeout=3).result
         except:
             # not support Tool.getInfo
             return
         if Version(result.SDKVersion) < Version("2.7.3"):
             raise MiniLaunchError("基础库版本[%s]过低，请确认基础库版本>=2.7.3" % self.sdk_version)
-        if Version(result.version) >= "1.06.2211072":
+        if str(result.version).endswith("2") and Version(result.version) >= "1.06.2211072":  # nightly
+            self.use_native = True
+        elif str(result.version).endswith("1") and Version(result.version) >= "1.06.2212011":  # RC
+            self.use_native = True
+        elif Version(result.version) >= "1.06.2301160":  # Stable
             self.use_native = True
 
     def send(self, method, data=None):
         if self.use_native and self.mini:
             ret = self.mini.connection.send("Tool.native", {
                 "method": method,
                 "data": data
@@ -105,15 +109,15 @@
         original=False,
         duration=5.0,
         names=None,
     ):
         raise NotImplementedError("ide not implemented")
 
     def allow_authorize(self, answer=True, title=None):
-        self._allow_authorize(answer)
+        return self._allow_authorize(answer)
 
     def _allow_authorize(self, answer):
         """
         mock实现, 所有接口引发的原生弹窗授权理论上都可以使用
         """
         if self.use_native:
             return self.send("authorizeAllow" if answer else "authorizeCancel")
```

### Comparing `minium-1.3.dev2/minium/native/wx_native/iosnative.py` & `minium-1.4.0/minium/native/wx_native/iosnative.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Created by xiazeng on 2019-05-22
 import json
 import logging
 import threading
 import platform
 from .basenative import BaseNative
 from ..lib.wx_wda import *
+from .wording import WORDING, Language
 
 tidevice = None
 OTHER_PACKAGE = "com.others.app"
 WECHAT_PACKAGE = "com.tencent.xin"
 WECHAT_ACTIVITY = "MainFrameViewController"
 MINIPROGRAM_ACTIVITY = "WAWebViewController"
 OTHER_ACTIVITY = "OtherActivity"
@@ -18,14 +19,17 @@
 if "Windows" in platform.platform():
     isWindows = True
 else:
     isWindows = False
 
 
 class WXIOSNative(BaseNative):
+    _require_conf_ = [
+        # ("wda_project_path", "wda_bundle")
+    ]
     useTIDevice = False
 
     def __init__(self, json_conf: dict):
         if json_conf is None:
             json_conf = {}
         super(WXIOSNative, self).__init__(json_conf)
         # 目标设备, 目标app
@@ -53,14 +57,17 @@
         self.check_done = True
         # screen_shot
         self.outputs_screen = os.path.join(
             json_conf.get("outputs") or os.path.dirname(os.path.realpath(__file__)),
             "image",
         )
         self._empty_base_screen_dir(self.outputs_screen)
+        # 分享小程序相关
+        self._forward_wording = None
+        self._new_chat_wording = None
 
     ###############################
     #                    interface                        #
     ###############################
     def start_wechat(self):
         """
         启动微信
@@ -89,14 +96,29 @@
                     while self.app.session(
                         class_name="Button", text="下一步"
                     ).click_if_exists(timeout=3.0):
                         time.sleep(1)
                     self.app.session(class_name="Button", text="进入微信").click_if_exists(
                         timeout=3.0
                     )
+                lan = True
+                for text in WORDING.COMMON.LOGIN_WORDS.zh:
+                    if not self.app.session(text=text).exists:
+                        lan = False
+                        break
+                if lan is False:
+                    lan = True
+                    for text in WORDING.COMMON.LOGIN_WORDS.en:
+                        if not self.app.session(text=text).exists:
+                            lan = False
+                            break
+                    if lan is True:
+                        WORDING.setLanguage(Language.en)
+                else:
+                    WORDING.setLanguage(Language.zh)
                 return
             except Exception as e:
                 if i == 2:
                     # e.args += "setup error: 第 %d 次启动微信失败" % (i + 1)
                     raise
                 logger.error("setup error: 第 %d 次启动微信失败: %s" % ((i + 1), str(e)))
                 if "Connection refused" in str(e):
@@ -456,19 +478,23 @@
         通过右上角更多菜单转发小程序
         ps: 好友太多会有性能问题
         :type text: 分享携带的内容
         :param names: 要分享的人
         :param create_new_chat: 是否创建群聊
         :return:
         """
-        self.app.session(class_name="Button", text="更多").click(timeout=10.0)
-        if self.app.session(class_name="Button", partial_text="转发").exists:
-            self.app.session(class_name="Button", partial_text="转发").click(timeout=10.0)
-        elif self.app.session(class_name="Button", partial_text="发送").exists:
-            self.app.session(class_name="Button", partial_text="发送").click(timeout=10.0)
+        self.app.session(class_name="Button", text=WORDING.COMMON.MORE.value).click(timeout=10.0)
+        time.sleep(1)
+        if self._forward_wording is None:  # 不同客户端版本有不同wording
+            for word in [ WORDING.IOS.FORWARD_WORD1, WORDING.IOS.FORWARD_WORD2, WORDING.IOS.FORWARD_WORD3 ]:
+                if self.app.session(class_name="Button", partial_text=word.value).exists:
+                    self._forward_wording = word
+                    break
+        if self._forward_wording and self.app.session(class_name="Button", partial_text=self._forward_wording.value).exists:
+            self.app.session(class_name="Button", partial_text=self._forward_wording.value).click(timeout=10.0)
         else:
             self.app.session(partial_text="关于").click(timeout=10.0)
             self.app.session(partial_text="推荐给朋友").click(timeout=10.0)
 
         return self.forward_miniprogram_inside(name, text, create_new_chat)
 
     def forward_miniprogram_inside(
@@ -489,28 +515,35 @@
         if isinstance(name, str):
             name = [name]
         if len(name) > 1:  # 多于一个人是需要新建群
             create_new_chat = True
         if not create_new_chat and self.app.session(text="暂无最近聊天").exists:
             create_new_chat = True
         if create_new_chat:
-            self.app.session(class_name="StaticText", text="创建新的聊天").click(timeout=10.0)
+            if self._new_chat_wording is None:
+                for word in [ WORDING.IOS.CREATE_CHAT1, WORDING.IOS.CREATE_CHAT2 ]:
+                    if self.app.session(class_name="StaticText", text=word.value).exists:
+                        self._new_chat_wording = word
+                        break
+                if not self._new_chat_wording:
+                    raise RuntimeError("无法创建新聊天")
+            self.app.session(class_name="StaticText", text=self._new_chat_wording.value).click(timeout=10.0)
         for _name in name:
             self.app.session(
-                class_name="TextField" if create_new_chat else "SearchField", text="搜索"
+                class_name="TextField" if create_new_chat else "SearchField", text=WORDING.COMMON.SEARCH.value
             ).set_text(_name)
             # count = 10
             time.sleep(1.5)  # 一定需要等待搜索出该用户
             self.app.session(
                 class_name="StaticText", partial_text=_name, index=-1
             ).click(timeout=10.0)
             # count -= 1
         if create_new_chat:
-            self.app.session(class_name="Button", partial_text="完成").click(timeout=10.0)
-        self.app.session(class_name="Button", text="发送").click(timeout=10.0)
+            self.app.session(class_name="Button", partial_text=WORDING.COMMON.DONE.value).click(timeout=10.0)
+        self.app.session(class_name="Button", text=WORDING.COMMON.SEND.value).click(timeout=10.0)
 
     def send_custom_message(self, message: str = None):
         """
         处理小程序 im 发送自定义消息
         :param message: 消息内容
         :return:
         """
```

### Comparing `minium-1.3.dev2/minium/utils/injectjs.py` & `minium-1.4.0/minium/utils/injectjs.py`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/createContext.js` & `minium-1.4.0/minium/utils/js/es5/createContext.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/helpers.js` & `minium-1.4.0/minium/utils/js/es5/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/hookWxMethod.js` & `minium-1.4.0/minium/utils/js/es5/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/ideMockChooseLocation.js` & `minium-1.4.0/minium/utils/js/es5/ideMockChooseLocation.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
         function d() {
             var b = {};
             b.确定 = function() {
                 return a(f), f
             }, b[f.name] = function() {
                 return a(f), f
             };
-            var c = function(c) {
+            var c = function _loop(c) {
                 b[c] = function() {
                     return a(i[c]), i[c]
                 }
             };
             for (var d in i) c(d);
             b.取消 = function() {
                 return a(g), g
@@ -31,19 +31,19 @@
             g = {
                 errMsg: "chooseLocation:fail cancel"
             },
             h = {
                 errMsg: "chooseLocation:fail auth deny"
             },
             i = {};
-        for (var k in f) void 0 !== b[k] && (f[k] = b[k]);
-        for (var m in c) i[m] = Object.assign({}, f, c[m]);
+        for (var j in f) void 0 !== b[j] && (f[j] = b[j]);
+        for (var k in c) i[k] = Object.assign({}, f, c[k]);
         if (!0 === global.__minium_auth_setting["scope.userLocation"]) return d();
         if (!1 === global.__minium_auth_setting["scope.userLocation"]) return e();
-        var j = {};
-        return j.允许 = function() {
+        var m = {};
+        return m.允许 = function() {
             return global.__minium_auth_setting["scope.userLocation"] = !0, d()
-        }, j.拒绝 = function() {
+        }, m.拒绝 = function() {
             return global.__minium_auth_setting["scope.userLocation"] = !1, e()
-        }, j.确定 = j.允许, j.取消 = j.拒绝, console.warn("[minium] mock wx.chooseLocation, you can use `native.allow_get_location` to handle it"), global.__minium_mock_auth_modal(j)
+        }, m.确定 = m.允许, m.取消 = m.拒绝, console.warn("[minium] mock wx.chooseLocation, you can use `native.allow_get_location` to handle it"), global.__minium_mock_auth_modal(m)
     })
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/ideMockGetLocation.js` & `minium-1.4.0/minium/utils/js/es5/ideMockGetLocation.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 function miniGetLocation(a, b) {
     return new Promise(function(c) {
         function d() {
             return c(f), f
         }
 
         function e() {
-            return c(g), g
+            return c(h), h
         }
         var f;
-        for (var i in f = "gcj02" === a.type ? {
+        for (var g in f = "gcj02" === a.type ? {
                 speed: -1,
                 steps: 0,
                 errMsg: "getLocation:ok",
                 provider: "gps",
                 buildingId: "",
                 longitude: 113.32489013671875,
                 latitude: 23.099933624267578,
@@ -30,21 +30,21 @@
                 longitude: 113.31950378417969,
                 latitude: 23.102487564086914,
                 verticalAccuracy: 10,
                 floorName: "1000",
                 accuracy: 65,
                 direction: -1,
                 horizontalAccuracy: 65
-            }, a.altitude && (f.altitude = 23.102540969848633), f) void 0 !== b[i] && (f[i] = b[i]);
-        var g = {
+            }, a.altitude && (f.altitude = 23.102540969848633), f) void 0 !== b[g] && (f[g] = b[g]);
+        var h = {
             errMsg: "getLocation:fail auth deny"
         };
         if (!0 === global.__minium_auth_setting["scope.userLocation"]) return d();
         if (!1 === global.__minium_auth_setting["scope.userLocation"]) return e();
-        var h = {};
-        return h.允许 = function() {
+        var i = {};
+        return i.允许 = function() {
             return global.__minium_auth_setting["scope.userLocation"] = !0, d()
-        }, h.拒绝 = function() {
+        }, i.拒绝 = function() {
             return global.__minium_auth_setting["scope.userLocation"] = !1, e()
-        }, h.确定 = h.允许, h.取消 = h.拒绝, console.warn("[minium] mock wx.getLocation, you can use `native.allow_get_location` to handle it"), global.__minium_mock_auth_modal(h)
+        }, i.确定 = i.允许, i.取消 = i.拒绝, console.warn("[minium] mock wx.getLocation, you can use `native.allow_get_location` to handle it"), global.__minium_mock_auth_modal(i)
     })
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/ideMockGetWeRunData.js` & `minium-1.4.0/minium/utils/js/es5/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/ideMockModal.js` & `minium-1.4.0/minium/utils/js/es5/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/es5/mockChooseImage.js` & `minium-1.4.0/minium/utils/js/es5/mockChooseImage.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -127,74 +127,74 @@
                     return {
                         name: a.imageName,
                         size: a.size
                     }
                 })
             })
         };
-        var g = !1;
+        var d = !1;
         a.mkdir({
             dirPath: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE"),
             recursive: !1,
             success: function success() {
-                g = !0
+                d = !0
             },
             fail: function fail(a) {
                 var b = a.errMsg;
-                0 <= b.indexOf("file already exists") && (g = !0)
+                0 <= b.indexOf("file already exists") && (d = !0)
             }
         });
-        var d = a.saveFile,
-            e = a.saveFileSync,
-            f = a.getSavedFileList;
+        var e = a.saveFile,
+            f = a.saveFileSync,
+            g = a.getSavedFileList;
         Object.defineProperty(a, "saveFile", {
             configurable: !0,
             get: function get() {
                 return function(b) {
                     var c = b.tempFilePath,
-                        e = b.filePath,
+                        d = b.filePath,
                         f = b.success,
                         g = b.fail,
                         h = b.complete;
                     if (c.startsWith("".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"))) {
                         var i = {
                             srcPath: c,
-                            destPath: e || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(c.split("/").pop())
+                            destPath: d || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(c.split("/").pop())
                         };
                         return f && (i.success = function(a) {
                             a.errMsg = a.errMsg.replace("copyFile", "saveFile"), a.savedFilePath = i.destPath, f(a)
                         }), g && (i.fail = function(a) {
                             a.errMsg = a.errMsg.replace("copyFile", "saveFile"), g(a)
                         }), h && (i.complete = function(a) {
                             a.errMsg = a.errMsg.replace("copyFile", "saveFile"), 0 === a.errMsg.indexOf("saveFile:ok") && (a.savedFilePath = i.destPath), h(a)
                         }), a.copyFile(i)
                     }
-                    return d({
+                    return e({
                         tempFilePath: c,
-                        filePath: e,
+                        filePath: d,
                         success: f,
                         fail: g,
                         complete: h
                     })
                 }
             }
         }), Object.defineProperty(a, "saveFileSync", {
             configurable: !0,
             get: function get() {
                 return function(b, c) {
                     if (b.startsWith("".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"))) {
                         var d = b,
-                            f = c || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(b.split("/").pop());
+                            e = c || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(b.split("/").pop());
                         try {
-                            return a.copyFileSync(d, f), f
+                            return a.copyFileSync(d, e), e
                         } catch (a) {
                             throw a.message.replace("copyFileSync", "saveFileSync")
                         }
                     }
-                    return e(b, c)
+                    return f(b, c)
                 }
             }
         }), Object.defineProperty(a, "getSavedFileList", {
             configurable: !0,
             get: function get() {
                 return function(b) {
                     var c = b.success,
@@ -212,15 +212,15 @@
                                         size: a.stats.size,
                                         createTime: a.stats.lastModifiedTime
                                     }
                                 }))
                             }
                         })
                     }), new Promise(function(a) {
-                        f({
+                        g({
                             complete: function complete(b) {
                                 a(b.fileList || [])
                             }
                         })
                     })]).then(function(a) {
                         var b = global.babelHelpers.slicedToArray(a, 2),
                             e = b[0],
@@ -232,34 +232,36 @@
                         c && c(g), d && d(g)
                     })
                 }
             }
         })
     }
     return new Promise(function(b, c) {
-        a.stat({
-            path: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP/"),
-            recursive: !0,
-            success: function success(a) {
-                return a.stats.length ? void b(a.stats.map(function(a) {
-                    return {
-                        name: a.path.replace(/^\//, ""),
-                        size: a.stats.size
-                    }
-                }).filter(function(a) {
-                    return a.name
-                })) : b([])
+        a.mkdir({
+            dirPath: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"),
+            recursive: !1,
+            success: function success() {
+                b([])
             },
             fail: function fail(d) {
                 var e = d.errMsg;
-                0 <= e.indexOf("no such file or directory") && a.mkdir({
-                    dirPath: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"),
+                return 0 <= e.indexOf("file already exists") ? void a.stat({
+                    path: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP/"),
                     recursive: !0,
-                    success: function success() {
-                        b([])
+                    success: function success(a) {
+                        return console.warn("[debug]fs.stat success"), a.stats.length ? void b(a.stats.map(function(a) {
+                            return {
+                                name: a.path.replace(/^\//, ""),
+                                size: a.stats.size
+                            }
+                        }).filter(function(a) {
+                            return a.name
+                        })) : b([])
                     },
                     fail: c
+                }) : void c({
+                    errMsg: e
                 })
             }
         })
     })
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/mockCloudCall.js` & `minium-1.4.0/minium/utils/js/es5/mockCloudCall.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -39,16 +39,30 @@
                         } return c[b].call(this, d)
                 }
             };
         Object.defineProperty(global, "__minium_cloud_call_mocked", {
             value: !0,
             writable: !1
         });
-        var c = {};
-        ["callContainer", "callFunction"].forEach(function(a) {
-            c[a] = wx.cloud[a], Object.defineProperty(wx.cloud, a, {
+        var c = {},
+            d = ["callContainer", "callFunction"];
+        if (d.forEach(function(a) {
+                c[a] = wx.cloud[a]
+            }), "undefined" != typeof Proxy) {
+            var e = new Proxy(wx.cloud, {
+                get: function get(a, c) {
+                    return -1 === d.indexOf(c) ? a[c] : b(c)
+                }
+            });
+            wx.cloud = e, Object.defineProperty(wx, "cloud", {
                 writable: !0,
-                value: b(a)
+                value: e
             })
+        } else d.forEach(function(a) {
+            var c = b(a);
+            Object.defineProperty(wx.cloud, a, {
+                writable: !0,
+                value: c
+            }), wx.cloud[a] = c
         })
     }
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/mockNetwork.js` & `minium-1.4.0/minium/utils/js/es5/mockNetwork.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,41 @@
 function mockNetwork() {
     if (!global["__minium_%(interface)s_network_mocked"]) {
-        var b = function(a, c) {
-            if (global.babelHelpers["typeof"](a) !== global.babelHelpers["typeof"](c)) return !1;
-            switch (global.babelHelpers["typeof"](a)) {
+        var a = function(b, c) {
+            if (global.babelHelpers["typeof"](b) !== global.babelHelpers["typeof"](c)) return !1;
+            switch (global.babelHelpers["typeof"](b)) {
                 case "string":
-                    var d = new RegExp(a);
+                    var d = new RegExp(b);
                     return !!d.exec(c);
                 case "number":
-                    return a === c;
+                    return b === c;
                 case "object":
-                    if (a instanceof Array) {
-                        if (a.length != c.length) return !1;
-                        for (var e = 0; e < a.length; e++)
-                            if (!b(a[e], c[e])) return !1;
+                    if (b instanceof Array) {
+                        if (b.length != c.length) return !1;
+                        for (var e = 0; e < b.length; e++)
+                            if (!a(b[e], c[e])) return !1;
                         return !0
                     }
-                    for (var f in a)
+                    for (var f in b)
                         if ("success" != f && "fail" != f && "complete" != f && "_miniMockType" != f) {
                             if (void 0 === c[f]) return !1;
-                            if (!b(a[f], c[f])) return !1
+                            if (!a(b[f], c[f])) return !1
                         } return !0;
             }
             return !1
         };
         Object.defineProperty(global, "__minium_%(interface)s_network_mocked", {
             value: !0,
             writable: !1
-        }), global["__minium_%(interface)sTask"] = function() {
+        }), global["__minium_%(interface)s_network_mock_rule"] || (global["__minium_%(interface)s_network_mock_rule"] = []), global["__minium_%(interface)sTask"] = function() {
             "use strict";
 
             function a(b, c, d) {
                 var e = this;
-                global.babelHelpers.classCallCheck(this, a), this.success = b, this.fail = c, this.callback = d, this.chunkCallback = [], this.headersReceivedCallback = [], this.progressUpdateCallback = [], setTimeout(function() {
+                global.babelHelpers.classCallCheck(this, a), this.success = b, this.fail = c, this.callback = d, this.chunkCallback = [], this.headersReceivedCallback = [], this.progressUpdateCallback = [], this.fd = setTimeout(function() {
                     e.headersReceivedCallback.forEach(function(a) {
                         e.success && a({
                             header: e.success.header
                         })
                     }), e.chunkCallback.forEach(function(a) {
                         e.success && a(e.success.data)
                     }), e.progressUpdateCallback.forEach(function(a) {
@@ -45,15 +45,17 @@
                             totalBytesExpectedToWrite: 100
                         })
                     }), d(e.success || e.fail)
                 })
             }
             return global.babelHelpers.createClass(a, [{
                 key: "abort",
-                value: function abort() {}
+                value: function abort() {
+                    clearTimeout(this.fd)
+                }
             }, {
                 key: "offChunkReceived",
                 value: function offChunkReceived(a) {
                     var b = this.chunkCallback.indexOf(a); - 1 !== b && this.chunkCallback.splice(b, 1)
                 }
             }, {
                 key: "offHeadersReceived",
@@ -73,32 +75,32 @@
             }, {
                 key: "onProgressUpdate",
                 value: function onProgressUpdate(a) {
                     this.progressUpdateCallback.push(a)
                 }
             }]), a
         }();
-        var a = wx["%(interface)s"];
+        var b = wx["%(interface)s"];
         Object.defineProperty(wx, "%(interface)s", {
             configurable: !0,
             get: function get() {
                 return function(c) {
                     for (var d, e = 0; e < global["__minium_%(interface)s_network_mock_rule"].length; e++)
-                        if (d = global["__minium_%(interface)s_network_mock_rule"][e], b(d, c)) {
+                        if (d = global["__minium_%(interface)s_network_mock_rule"][e], a(d, c)) {
                             if (1 === d._miniMockType) {
                                 var f = global["__minium_%(interface)s_network_mock_rule"].splice(e, 1),
                                     g = global.babelHelpers.slicedToArray(f, 1);
                                 d = g[0]
                             }
-                            if (console.log("@@@@rule match", d), d.success) return new global["__minium_%(interface)sTask"](d.success, void 0, function(a) {
+                            if (console.log("@@@@rule match", d), c.__miniumMocked = !0, d.success) return new global["__minium_%(interface)sTask"](d.success, void 0, function(a) {
                                 c.success && c.success(a), c.complete && c.complete(a)
                             });
                             if (d.fail) return new global["__minium_%(interface)sTask"](void 0, d.fail, function(a) {
                                 c.fail && c.fail(a), c.complete && c.complete(a)
                             });
                             if (1 === d._miniMockType) return
-                        } return a(c)
+                        } return b(c)
                 }
             }
         })
     }
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/networkPannel.js` & `minium-1.4.0/minium/utils/js/es5/networkPannel.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 function enableNetworkPanel() {
     var a = wx.request;
     if (!global.__minium_request_hooked) {
         Object.defineProperty(global, "__minium_request_hooked", {
             value: !0,
             writable: !1
         });
-        var e = Object.getOwnPropertyDescriptor(wx, "request");
-        if (e && !1 === e.configurable) return void console.warn("[minitest] Cannot redefine property: request");
-        var b = function(a) {
+        var b = Object.getOwnPropertyDescriptor(wx, "request");
+        if (b && !1 === b.configurable) return void console.warn("[minitest] Cannot redefine property: request");
+        var c = function(a) {
                 for (var b = 5381, c = a.length; c;) b = 33 * b ^ a.charCodeAt(--c);
                 return b >>> 0
             },
-            c = new Map,
-            d = new Map;
+            d = new Map,
+            e = new Map;
         Object.defineProperty(wx, "request", {
             configurable: !0,
             get: function get() {
-                return function(e) {
-                    if (!global || !global.__minium_get_mini_network_id) return a(e);
-                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == e.url) return a(e);
+                return function(b) {
+                    if (!global || !global.__minium_get_mini_network_id) return a(b);
+                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == b.url) return a(b);
                     var f = global.__minium_get_mini_network_id(),
-                        g = Object.assign({}, e);
+                        g = Object.assign({}, b);
                     delete g.success, delete g.fail, delete g.complete;
                     var h, i = Date.now();
                     try {
-                        var k = JSON.stringify(g);
-                        h = b(k), c.has(h) && c.get(h) > i && (k = ""), c.set(h, i + 21e3), mini_send_request(f, k, i, h)
+                        var j = JSON.stringify(g);
+                        h = c(j), d.has(h) && d.get(h) > i && (j = ""), d.set(h, i + 21e3), mini_send_request(f, j, i, h)
                     } catch (a) {
                         mini_send_request(f, JSON.stringify({
                             url: g.url,
                             err: a.toString()
                         }), i, 0)
                     }
-                    var j = e.complete;
-                    return e.complete = function(a) {
-                        var c = Object.assign({}, a);
-                        delete c.profile;
-                        var e = JSON.stringify(c),
-                            g = b(e),
-                            h = Date.now();
-                        d.has(g) && d.get(g) > h && (e = ""), d.set(g, h + 21e3), mini_request_callback(f, e, h, g), j && j(a)
-                    }, a(e)
+                    var k = b.complete;
+                    return b.complete = function(a) {
+                        var d = Object.assign({}, a);
+                        delete d.profile;
+                        var g = JSON.stringify(d),
+                            h = c(g),
+                            i = Date.now();
+                        e.has(h) && e.get(h) > i && (g = ""), e.set(h, i + 21e3), mini_request_callback(f, g, i, h, b.__miniumMocked), k && k(a)
+                    }, a(b)
                 }
             }
         })
     }
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/requestStack.js` & `minium-1.4.0/minium/utils/js/es5/requestStack.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,35 @@
 function miniumRequestStack() {
     if (!global.__minium_request_stack) {
         global.__minium_request_stack = new Map, global.__minium_wait_util = function() {
-            var a = 0 < arguments.length && arguments[0] !== void 0 ? arguments[0] : 0,
-                b = 1 < arguments.length && arguments[1] !== void 0 ? arguments[1] : 20,
+            var a = 0 < arguments.length && void 0 !== arguments[0] ? arguments[0] : 0,
+                b = 1 < arguments.length && void 0 !== arguments[1] ? arguments[1] : 20,
                 c = (getCurrentPages().pop() || {}).__wxWebviewId__;
             return new Promise(function(d) {
                 var e = 10 * b,
                     f = setInterval(function() {
                         e--;
                         var b = global.__minium_request_stack.has(c) ? global.__minium_request_stack.get(c).size : 0;
                         console.debug("[minitest] current stack size: ", b), b <= a ? (clearInterval(f), d(!0)) : 0 > e && (clearInterval(f), d(!1))
                     }, 100)
             })
         };
         var a = wx.request;
-        Object.defineProperty(wx, "request", {
+        return Object.defineProperty(wx, "request", {
             configurable: !0,
             get: function get() {
                 return function(b) {
                     if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == b.url) return a(b);
                     var c, d = (getCurrentPages().pop() || {}).__wxWebviewId__;
                     global.__minium_request_stack.has(d) ? c = global.__minium_request_stack.get(d) : (c = new Map, global.__minium_request_stack.set(d, c));
                     var e, f = b.complete;
                     b.complete = function(a) {
                         c["delete"](e), 0 === c.size && global.__minium_request_stack["delete"](d), f && f(a)
                     };
                     var g = a(b);
                     return e = g && g.uniqueId || Math.random(), c.set(e, Date.now()), g
                 }
             }
-        })
+        }), !0
     }
+    return !1
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/es5/testAsync.js` & `minium-1.4.0/minium/utils/js/es5/testAsync.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -77,31 +77,31 @@
             }
         })
     }
 
     function i(a, b, d) {
         var e = "suspendedStart";
         return function(f, g) {
-            if ("executing" === e) throw new Error("Generator is already running");
-            if ("completed" === e) {
+            if ("executing" == e) throw new Error("Generator is already running");
+            if ("completed" == e) {
                 if ("throw" === f) throw g;
                 return o()
             }
             for (d.method = f, d.arg = g;;) {
                 var h = d.delegate;
                 if (h) {
                     var i = j(h, d);
                     if (i) {
                         if (i === x) continue;
                         return i
                     }
                 }
                 if ("next" === d.method) d.sent = d._sent = d.arg;
                 else if ("throw" === d.method) {
-                    if ("suspendedStart" === e) throw e = "completed", d.arg;
+                    if ("suspendedStart" == e) throw e = "completed", d.arg;
                     d.dispatchException(d.arg)
                 } else "return" === d.method && d.abrupt("return", d.arg);
                 e = "executing";
                 var k = c(a, b, d);
                 if ("normal" === k.type) {
                     if (e = d.done ? "completed" : "suspendedYield", k.arg === x) continue;
                     return {
@@ -111,26 +111,21 @@
                 }
                 "throw" === k.type && (e = "completed", d.method = "throw", d.arg = k.arg)
             }
         }
     }
 
     function j(a, b) {
-        var d = a.iterator[b.method];
-        if (void 0 === d) {
-            if (b.delegate = null, "throw" === b.method) {
-                if (a.iterator["return"] && (b.method = "return", b.arg = void 0, j(a, b), "throw" === b.method)) return x;
-                b.method = "throw", b.arg = new TypeError("The iterator does not provide a 'throw' method")
-            }
-            return x
-        }
-        var e = c(d, a.iterator, b.arg);
-        if ("throw" === e.type) return b.method = "throw", b.arg = e.arg, b.delegate = null, x;
-        var f = e.arg;
-        return f ? f.done ? (b[a.resultName] = f.value, b.next = a.nextLoc, "return" !== b.method && (b.method = "next", b.arg = void 0), b.delegate = null, x) : f : (b.method = "throw", b.arg = new TypeError("iterator result is not an object"), b.delegate = null, x)
+        var d = b.method,
+            e = a.iterator[d];
+        if (void 0 === e) return b.delegate = null, "throw" === d && a.iterator["return"] && (b.method = "return", b.arg = void 0, j(a, b), "throw" === b.method) || "return" !== d && (b.method = "throw", b.arg = new TypeError("The iterator does not provide a '" + d + "' method")), x;
+        var f = c(e, a.iterator, b.arg);
+        if ("throw" === f.type) return b.method = "throw", b.arg = f.arg, b.delegate = null, x;
+        var g = f.arg;
+        return g ? g.done ? (b[a.resultName] = g.value, b.next = a.nextLoc, "return" !== b.method && (b.method = "next", b.arg = void 0), b.delegate = null, x) : g : (b.method = "throw", b.arg = new TypeError("iterator result is not an object"), b.delegate = null, x)
     }
 
     function k(a) {
         var b = {
             tryLoc: a[0]
         };
         1 in a && (b.catchLoc = a[1]), 2 in a && (b.finallyLoc = a[2], b.afterLoc = a[3]), this.tryEntries.push(b)
```

### Comparing `minium-1.3.dev2/minium/utils/js/min/helpers.js` & `minium-1.4.0/minium/utils/js/min/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/hookWxMethod.js` & `minium-1.4.0/minium/utils/js/min/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/ideMockChooseLocation.js` & `minium-1.4.0/minium/utils/js/min/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/ideMockGetLocation.js` & `minium-1.4.0/minium/utils/js/min/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/ideMockGetWeRunData.js` & `minium-1.4.0/minium/utils/js/min/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/ideMockModal.js` & `minium-1.4.0/minium/utils/js/min/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.3.dev2/minium/utils/js/min/mockChooseImage.js` & `minium-1.4.0/minium/utils/js/min/mockChooseImage.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -210,32 +210,34 @@
                     };
                     t && t(a), s && s(a)
                 }))
             }
         })
     }
     return new Promise(((t, s) => {
-        e.stat({
-            path: `${wx.env.USER_DATA_PATH}/.MINIUM_TMP/`,
-            recursive: !0,
-            success: e => {
-                if (!e.stats.length) return t([]);
-                t(e.stats.map((e => ({
-                    name: e.path.replace(/^\//, ""),
-                    size: e.stats.size
-                }))).filter((e => e.name)))
+        e.mkdir({
+            dirPath: `${wx.env.USER_DATA_PATH}/.MINIUM_TMP`,
+            recursive: !1,
+            success() {
+                t([])
             },
             fail: ({
                 errMsg: i
             }) => {
-                i.indexOf("no such file or directory") >= 0 && e.mkdir({
-                    dirPath: `${wx.env.USER_DATA_PATH}/.MINIUM_TMP`,
+                i.indexOf("file already exists") >= 0 ? e.stat({
+                    path: `${wx.env.USER_DATA_PATH}/.MINIUM_TMP/`,
                     recursive: !0,
-                    success() {
-                        t([])
+                    success: e => {
+                        if (console.warn("[debug]fs.stat success"), !e.stats.length) return t([]);
+                        t(e.stats.map((e => ({
+                            name: e.path.replace(/^\//, ""),
+                            size: e.stats.size
+                        }))).filter((e => e.name)))
                     },
                     fail: s
+                }) : s({
+                    errMsg: i
                 })
             }
         })
     }))
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/min/mockNetwork.js` & `minium-1.4.0/minium/utils/js/min/mockNetwork.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,83 +1,85 @@
 function mockNetwork() {
     if (!global["__minium_%(interface)s_network_mocked"]) {
-        function e(s, i) {
-            if (typeof s != typeof i) return !1;
-            switch (typeof s) {
+        function e(i, s) {
+            if (typeof i != typeof s) return !1;
+            switch (typeof i) {
                 case "string":
-                    return !!new RegExp(s).exec(i);
+                    return !!new RegExp(i).exec(s);
                 case "number":
-                    return s === i;
+                    return i === s;
                 case "object":
-                    if (s instanceof Array) {
-                        if (s.length != i.length) return !1;
-                        for (var c = 0; c < s.length; c++)
-                            if (!e(s[c], i[c])) return !1;
+                    if (i instanceof Array) {
+                        if (i.length != s.length) return !1;
+                        for (var c = 0; c < i.length; c++)
+                            if (!e(i[c], s[c])) return !1;
                         return !0
                     }
-                    for (var t in s)
+                    for (var t in i)
                         if ("success" != t && "fail" != t && "complete" != t && "_miniMockType" != t) {
-                            if (void 0 === i[t]) return !1;
-                            if (!e(s[t], i[t])) return !1
+                            if (void 0 === s[t]) return !1;
+                            if (!e(i[t], s[t])) return !1
                         } return !0
             }
             return !1
         }
         Object.defineProperty(global, "__minium_%(interface)s_network_mocked", {
             value: !0,
             writable: !1
-        }), global["__minium_%(interface)sTask"] = class {
-            constructor(e, s, i) {
-                this.success = e, this.fail = s, this.callback = i, this.chunkCallback = [], this.headersReceivedCallback = [], this.progressUpdateCallback = [], setTimeout((() => {
+        }), global["__minium_%(interface)s_network_mock_rule"] || (global["__minium_%(interface)s_network_mock_rule"] = []), global["__minium_%(interface)sTask"] = class {
+            constructor(e, i, s) {
+                this.success = e, this.fail = i, this.callback = s, this.chunkCallback = [], this.headersReceivedCallback = [], this.progressUpdateCallback = [], this.fd = setTimeout((() => {
                     this.headersReceivedCallback.forEach((e => {
                         this.success && e({
                             header: this.success.header
                         })
                     })), this.chunkCallback.forEach((e => {
                         this.success && e(this.success.data)
                     })), this.progressUpdateCallback.forEach((e => {
                         this.success && e({
                             progress: 100,
                             totalBytesWritten: 100,
                             totalBytesExpectedToWrite: 100
                         })
-                    })), i(this.success || this.fail)
+                    })), s(this.success || this.fail)
                 }))
             }
-            abort() {}
+            abort() {
+                clearTimeout(this.fd)
+            }
             offChunkReceived(e) {
-                var s = this.chunkCallback.indexOf(e); - 1 !== s && this.chunkCallback.splice(s, 1)
+                var i = this.chunkCallback.indexOf(e); - 1 !== i && this.chunkCallback.splice(i, 1)
             }
             offHeadersReceived(e) {
-                var s = this.headersReceivedCallback.indexOf(e); - 1 !== s && this.headersReceivedCallback.splice(s, 1)
+                var i = this.headersReceivedCallback.indexOf(e); - 1 !== i && this.headersReceivedCallback.splice(i, 1)
             }
             onChunkReceived(e) {
                 this.chunkCallback.push(e)
             }
             onHeadersReceived(e) {
                 this.headersReceivedCallback.push(e)
             }
             onProgressUpdate(e) {
                 this.progressUpdateCallback.push(e)
             }
         };
-        var s = wx["%(interface)s"];
+        var i = wx["%(interface)s"];
         Object.defineProperty(wx, "%(interface)s", {
             configurable: !0,
-            get: () => function(i) {
+            get: () => function(s) {
                 for (var c = 0; c < global["__minium_%(interface)s_network_mock_rule"].length; c++) {
                     var t = global["__minium_%(interface)s_network_mock_rule"][c];
-                    if (e(t, i)) {
-                        if (1 === t._miniMockType && ([t] = global["__minium_%(interface)s_network_mock_rule"].splice(c, 1)), console.log("@@@@rule match", t), t.success) return new global["__minium_%(interface)sTask"](t.success, void 0, (e => {
-                            i.success && i.success(e), i.complete && i.complete(e)
+                    if (e(t, s)) {
+                        if (1 === t._miniMockType && ([t] = global["__minium_%(interface)s_network_mock_rule"].splice(c, 1)), console.log("@@@@rule match", t), s.__miniumMocked = !0, t.success) return new global["__minium_%(interface)sTask"](t.success, void 0, (e => {
+                            s.success && s.success(e), s.complete && s.complete(e)
                         }));
                         if (t.fail) return new global["__minium_%(interface)sTask"](void 0, t.fail, (e => {
-                            i.fail && i.fail(e), i.complete && i.complete(e)
+                            s.fail && s.fail(e), s.complete && s.complete(e)
                         }));
                         if (1 === t._miniMockType) return
                     }
                 }
-                return s(i)
+                return i(s)
             }
         })
     }
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/min/networkPannel.js` & `minium-1.4.0/minium/utils/js/min/networkPannel.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,40 +9,40 @@
         if (t && !1 === t.configurable) return void console.warn("[minitest] Cannot redefine property: request");
         let r = function(e) {
                 let t = 5381,
                     r = e.length;
                 for (; r;) t = 33 * t ^ e.charCodeAt(--r);
                 return t >>> 0
             },
-            n = new Map,
-            i = new Map;
+            i = new Map,
+            n = new Map;
         Object.defineProperty(wx, "request", {
             configurable: !0,
             get: () => function(t) {
                 if (!global || !global.__minium_get_mini_network_id) return e(t);
                 if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == t.url) return e(t);
                 let l, o = global.__minium_get_mini_network_id(),
                     s = Object.assign({}, t);
                 delete s.success, delete s.fail, delete s.complete;
                 let u = Date.now();
                 try {
                     let e = JSON.stringify(s);
-                    l = r(e), n.has(l) && n.get(l) > u && (e = ""), n.set(l, u + 21e3), mini_send_request(o, e, u, l)
+                    l = r(e), i.has(l) && i.get(l) > u && (e = ""), i.set(l, u + 21e3), mini_send_request(o, e, u, l)
                 } catch (e) {
                     mini_send_request(o, JSON.stringify({
                         url: s.url,
                         err: e.toString()
                     }), u, 0)
                 }
-                let a = t.complete;
+                let _ = t.complete;
                 return t.complete = e => {
-                    let t = Object.assign({}, e);
-                    delete t.profile;
-                    let n = JSON.stringify(t),
-                        l = r(n),
-                        s = Date.now();
-                    i.has(l) && i.get(l) > s && (n = ""), i.set(l, s + 21e3), mini_request_callback(o, n, s, l), a && a(e)
+                    let i = Object.assign({}, e);
+                    delete i.profile;
+                    let l = JSON.stringify(i),
+                        s = r(l),
+                        u = Date.now();
+                    n.has(s) && n.get(s) > u && (l = ""), n.set(s, u + 21e3), mini_request_callback(o, l, u, s, t.__miniumMocked), _ && _(e)
                 }, e(t)
             }
         })
     }
 }
```

### Comparing `minium-1.3.dev2/minium/utils/js/min/requestStack.js` & `minium-1.4.0/minium/utils/js/min/requestStack.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,31 @@
 function miniumRequestStack() {
     if (!global.__minium_request_stack) {
         global.__minium_request_stack = new Map, global.__minium_wait_util = function(e = 0, t = 20) {
-            var _ = (getCurrentPages().pop() || {}).__wxWebviewId__;
-            return new Promise((a => {
-                var r = 10 * t,
+            var r = (getCurrentPages().pop() || {}).__wxWebviewId__;
+            return new Promise((_ => {
+                var a = 10 * t,
                     i = setInterval((() => {
-                        r--;
-                        var t = global.__minium_request_stack.has(_) ? global.__minium_request_stack.get(_).size : 0;
-                        console.debug("[minitest] current stack size: ", t), t <= e ? (clearInterval(i), a(!0)) : r < 0 && (clearInterval(i), a(!1))
+                        a--;
+                        var t = global.__minium_request_stack.has(r) ? global.__minium_request_stack.get(r).size : 0;
+                        console.debug("[minitest] current stack size: ", t), t <= e ? (clearInterval(i), _(!0)) : a < 0 && (clearInterval(i), _(!1))
                     }), 100)
             }))
         };
         var e = wx.request;
-        Object.defineProperty(wx, "request", {
+        return Object.defineProperty(wx, "request", {
             configurable: !0,
             get: () => function(t) {
                 if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == t.url) return e(t);
-                var _, a = (getCurrentPages().pop() || {}).__wxWebviewId__;
-                global.__minium_request_stack.has(a) ? _ = global.__minium_request_stack.get(a) : (_ = new Map, global.__minium_request_stack.set(a, _));
-                var r, i = t.complete;
+                var r, _ = (getCurrentPages().pop() || {}).__wxWebviewId__;
+                global.__minium_request_stack.has(_) ? r = global.__minium_request_stack.get(_) : (r = new Map, global.__minium_request_stack.set(_, r));
+                var a, i = t.complete;
                 t.complete = e => {
-                    _.delete(r), 0 === _.size && global.__minium_request_stack.delete(a), i && i(e)
+                    r.delete(a), 0 === r.size && global.__minium_request_stack.delete(_), i && i(e)
                 };
                 var n = e(t);
-                return r = n && n.uniqueId || Math.random(), _.set(r, Date.now()), n
+                return a = n && n.uniqueId || Math.random(), r.set(a, Date.now()), n
             }
-        })
+        }), !0
     }
+    return !1
 }
```

### Comparing `minium-1.3.dev2/minium/utils/utils.py` & `minium-1.4.0/minium/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,41 +4,43 @@
 Author:         yopofeng
 Filename:       utils.py
 Create time:    2021/9/24 21:21
 Description:
 
 """
 import time
-from functools import wraps
 import typing
+from typing import overload
 import types
 import platform
 import re
 import sys
 import inspect
 import threading
 import logging
 import os
 import asyncio
 import functools
 import concurrent.futures
+import json
+import socket
 
 logger = logging.getLogger("minium")
 
 
 def timeout(duration, interval=1):
     """
     重试超时装饰器,在超时之前会每隔{interval}秒重试一次
     注意：被修饰的函数必须要有非空返回,这是重试终止的条件！！！
     :param duration: seconds
     :return:
     """
 
     def spin_until_true(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             timeout = time.time() + duration
             execed = False
             r = None
             while not (r or timeout < time.time() and execed):
                 r = func(*args, **kwargs)
                 execed = True
@@ -50,84 +52,101 @@
         return wrapper
 
     return spin_until_true
 
 
 def retry(cnt, expected_exception=None):
     """
-    重试固定次数装饰器, 被修饰函数没有raise error则直接返回，有则最多执行${cnt}次
+    重试固定次数装饰器, 被修饰函数没有raise error则直接返回, 有则最多执行${cnt}次
     :cnt: 重试次数，函数最多被执行 ${cnt} 次
-    :expected_exception: 命中预期的错误才重试，None为所有错误
+    :expected_exception: 命中预期的错误(isinstance(e, expected_exception))才重试, None为所有错误
     """
 
     def try_until_no_error(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             _cnt = 0
             while _cnt < cnt:
                 try:
                     _cnt += 1
-                    # print("try %d" % _cnt)
                     return func(*args, **kwargs)
                 except:
                     if _cnt >= cnt:
                         raise
                     e = sys.exc_info()[1]
-                    if expected_exception and isinstance(
-                        expected_exception, (tuple, list)
-                    ):
-                        if e.__class__ in expected_exception:
-                            continue
-                    elif expected_exception:
-                        if e.__class__ == expected_exception:
-                            continue
-                    else:
+                    if expected_exception is None or isinstance(e, expected_exception):
+                        logger.warning(
+                            f'{f"第 {_cnt} 次" if _cnt < cnt else "最后一次"}重新运行{func.__name__}'
+                        )
+                        logger.info(f'原因: {e.__class__.__name__}{str(e.args)}')
                         continue
                     raise
 
         return wrapper
 
     return try_until_no_error
 
 
+CatchableType = typing.Union[types.FunctionType, types.MethodType]
+
+
+@overload
+def catch(wrapped: CatchableType, *args: typing.Tuple[Exception, ...]) -> CatchableType:
+    ...
+
+
+@overload
+def catch(*args: typing.Tuple[Exception, ...]) -> CatchableType:
+    ...
+
+
 def catch(*args):
     """
     抓获指定/所有exception
     :wrapped: 被修饰的函数, 如果为空则作为修饰器使用
     :expected_exception: 指定/所有exception
     :return: Exception/None
+
+    etc.
+    @catch
+    def catchAllException():
+        raise Exception("test")
+
+    @catch(ValueError, RuntimeError)
+    def catchValueAndRuntimeError():
+        raise ValueError("test")
+
+    def raiseValueError():
+        raise ValueError("test")
+    catch(raiseValueError)() -> ValueError("test")
+    catch(raiseValueError, ValueError)() -> ValueError("test")
+    catch(raiseValueError, ValueError, RuntimeError)() -> ValueError("test")
+    catch(ValueError, RuntimeError)(raiseValueError)() -> ValueError("test")
+    catch(raiseValueError, RuntimeError)() -> raise ValueError("test")
     """
     wrapped = None
     expected_exception = None
     if len(args) == 0:
         expected_exception = None
-    elif len(args) == 1:
+    elif len(args) >= 1:
         if inspect.isfunction(args[0]) or inspect.ismethod(args[0]):
             wrapped = args[0]
+            expected_exception = args[1:] or None
         else:
-            expected_exception = args[0]
-    elif len(args) == 2:
-        wrapped, expected_exception = args
-    else:
-        raise TypeError(f"catch takes at most 2 argument but {len(args)} were given")
+            expected_exception = args
 
     def try_catch(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 func(*args, **kwargs)
             except:
                 e = sys.exc_info()[1]
-                if expected_exception and isinstance(expected_exception, (tuple, list)):
-                    if e.__class__ in expected_exception:
-                        return e
-                elif expected_exception:
-                    if e.__class__ == expected_exception:
-                        return e
-                else:
+                if expected_exception is None or isinstance(e, expected_exception):
+                    logger.error("catch error: %s", e)
                     return e
                 raise
 
         return wrapper
 
     if wrapped:
         return try_catch(wrapped)
@@ -184,15 +203,15 @@
 def wait(timeout, default=None):
     """
     等待修饰器
     等待timeout时间, 如果函数没有返回则返回default
     """
 
     def spin_until_true(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             t = WaitThread(target=func, args=args, kwargs=kwargs)
             t.setDaemon(True)
             t.start()
             try:
                 return t.get_result(timeout)
             except WaitTimeoutError:
@@ -342,15 +361,15 @@
 
 
 async def async_wait(
     fut, timeout, loop: ProcessSafeEventLoop or asyncio.AbstractEventLoop = None
 ):
     """
     reference asyncio.wait_for
-    wait fut done, when timeout, raise 
+    wait fut done, when timeout, raise
     """
     if loop is None:
         loop = asyncio.get_running_loop()
     elif isinstance(loop, ProcessSafeEventLoop):
         loop = loop.loop
     else:
         loop = loop
@@ -394,15 +413,18 @@
                 raise WaitTimeoutError()
     finally:
         timeout_handle.cancel()
 
 
 class AsyncCondition(asyncio.Condition):
     def __init__(
-        self, lock: asyncio.Lock = None, *, loop: asyncio.AbstractEventLoop or ProcessSafeEventLoop = None
+        self,
+        lock: asyncio.Lock = None,
+        *,
+        loop: asyncio.AbstractEventLoop or ProcessSafeEventLoop = None,
     ) -> None:
         if isinstance(loop, ProcessSafeEventLoop):
             loop = loop.loop
         if sys.version_info < (3, 10):
             super().__init__(lock, loop=loop)
         else:  # loop参数将在3.10废除
             asyncio.set_event_loop(loop)
@@ -414,17 +436,19 @@
         if timeout is None:
             return await coro
         try:
             return await async_wait(coro, timeout=timeout, loop=loop)
         except WaitTimeoutError:
             return False
 
+
 Future = typing.Union[asyncio.futures.Future, concurrent.futures.Future]
 EventLoop = typing.Union[ProcessSafeEventLoop, asyncio.BaseEventLoop]
 
+
 def get_result(
     fut: Future,
     timeout=None,
     default=None,
 ):
     # asyncio.futures.Future.result 去掉了timeout参数
     if isinstance(fut, concurrent.futures.Future):
@@ -439,7 +463,52 @@
         return asyncio.run_coroutine_threadsafe(
             async_wait(fut, timeout=timeout, loop=loop), loop=loop
         ).result()
     except WaitTimeoutError as ext:
         if default is not None:
             return default
         raise WaitTimeoutError() from ext
+
+
+class Object(dict):
+    def __init__(self, __map=None, **kwargs):
+        if __map:
+            kwargs.update(__map)
+        extend = {}
+        for k, v in kwargs.items():
+            if hasattr(dict, k):  # dict本来的属性不可覆盖
+                extend[k] = v
+                continue
+            setattr(self, k, v)
+        super(Object, self).__init__(self.__dict__, **extend)
+
+    def __getattr__(self, __k):
+        try:
+            return self[__k]
+        except KeyError:
+            return None
+
+    def __setattr__(self, __k, __v):
+        if isinstance(__v, dict):
+            __v = Object(__v)
+        if isinstance(__v, list):
+            for index, v in enumerate(__v):
+                if isinstance(v, dict):
+                    __v[index] = Object(v)
+        if hasattr(self.__class__, __k):
+            super(Object, self).__setattr__(__k, __v)
+        else:
+            self[__k] = __v
+
+    @classmethod
+    def parse_from_file(cls, file_path):
+        if not os.path.isfile(file_path):
+            raise RuntimeError(f"{file_path} not exists")
+        with open(file_path, "r", encoding="utf8") as fp:
+            return cls(json.load(fp))
+        
+def pick_unuse_port():
+    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    s.bind(("localhost", 0))
+    addr, port = s.getsockname()
+    s.close()
+    return port
```

### Comparing `minium-1.3.dev2/minium.egg-info/SOURCES.txt` & `minium-1.4.0/minium.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 minium/framework/logcolor.py
 minium/framework/miniconfig.py
 minium/framework/miniddt.py
 minium/framework/minidoctor.py
 minium/framework/minilimit.py
 minium/framework/miniprogram.py
 minium/framework/miniresult.py
-minium/framework/miniretry.py
 minium/framework/minisuite.py
 minium/framework/minitest.py
 minium/framework/report.py
 minium/framework/session.py
 minium/framework/wording.py
 minium/framework/dist/favicon.ico
 minium/framework/dist/index.html
@@ -53,14 +52,15 @@
 minium/miniprogram/base_driver/element.py
 minium/miniprogram/base_driver/minium.py
 minium/miniprogram/base_driver/minium_log.py
 minium/miniprogram/base_driver/minium_object.py
 minium/miniprogram/base_driver/page.py
 minium/miniprogram/base_driver/prefixer.py
 minium/miniprogram/base_driver/version.json
+minium/miniprogram/base_driver/version.py
 minium/miniprogram/base_driver/waiter.py
 minium/native/__init__.py
 minium/native/exception.py
 minium/native/lib/__init__.py
 minium/native/lib/requirements.txt
 minium/native/lib/android_base/__init__.py
 minium/native/lib/at/__init__.py
@@ -149,18 +149,20 @@
 minium/native/qq_native/qbasenative.py
 minium/native/qq_native/qiosnative.py
 minium/native/wx_native/__init__.py
 minium/native/wx_native/androidnative.py
 minium/native/wx_native/basenative.py
 minium/native/wx_native/idenative.py
 minium/native/wx_native/iosnative.py
+minium/native/wx_native/wording.py
 minium/utils/__init__.py
 minium/utils/emitter.py
 minium/utils/eventloop.py
 minium/utils/injectjs.py
+minium/utils/meta.py
 minium/utils/platforms.py
 minium/utils/utils.py
 minium/utils/js/es5/addCloudCallMockRule.js
 minium/utils/js/es5/addNetworkMockRule.js
 minium/utils/js/es5/callContextMethod.js
 minium/utils/js/es5/checkInject.js
 minium/utils/js/es5/cleanCloudCallMockRule.js
@@ -184,14 +186,15 @@
 minium/utils/js/es5/ideMockModal.js
 minium/utils/js/es5/ideMockShowActionSheet.js
 minium/utils/js/es5/ideMockShowModal.js
 minium/utils/js/es5/ideMockSubscribeMessage.js
 minium/utils/js/es5/mockChooseImage.js
 minium/utils/js/es5/mockCloudCall.js
 minium/utils/js/es5/mockNetwork.js
+minium/utils/js/es5/mockRequestStack.js
 minium/utils/js/es5/networkPannel.js
 minium/utils/js/es5/releaseHookWxMethod.js
 minium/utils/js/es5/requestStack.js
 minium/utils/js/es5/startGetPerformance.js
 minium/utils/js/es5/stopGetPerformance.js
 minium/utils/js/es5/testAsync.js
 minium/utils/js/es5/uuid.js
@@ -221,14 +224,15 @@
 minium/utils/js/min/ideMockModal.js
 minium/utils/js/min/ideMockShowActionSheet.js
 minium/utils/js/min/ideMockShowModal.js
 minium/utils/js/min/ideMockSubscribeMessage.js
 minium/utils/js/min/mockChooseImage.js
 minium/utils/js/min/mockCloudCall.js
 minium/utils/js/min/mockNetwork.js
+minium/utils/js/min/mockRequestStack.js
 minium/utils/js/min/networkPannel.js
 minium/utils/js/min/releaseHookWxMethod.js
 minium/utils/js/min/requestStack.js
 minium/utils/js/min/startGetPerformance.js
 minium/utils/js/min/stopGetPerformance.js
 minium/utils/js/min/testAsync.js
 minium/utils/js/min/uuid.js
```

### Comparing `minium-1.3.dev2/setup.py` & `minium-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import sys
 
-__version__ = "1.3.dev2"
+__version__ = "1.4.0"
 
 from setuptools import setup, find_packages
 
 # We do not support Python <3.8
 if sys.version_info < (3, 8):
     print(
         "Unfortunately, your python version is not supported!\n"
```

